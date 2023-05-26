# Comparing `tmp/transpector-0.1.0.tar.gz` & `tmp/transpector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpector-0.1.0.tar", last modified: Thu May 25 23:31:55 2023, max compression
+gzip compressed data, was "transpector-0.1.1.tar", last modified: Fri May 26 12:18:28 2023, max compression
```

## Comparing `transpector-0.1.0.tar` & `transpector-0.1.1.tar`

### file list

```diff
@@ -1,324 +1,324 @@
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.872902 transpector-0.1.0/
--rw-r--r--   0 rkopel001   (501) staff       (20)       88 2023-05-25 23:31:34.000000 transpector-0.1.0/MANIFEST.in
--rw-r--r--   0 rkopel001   (501) staff       (20)     3879 2023-05-25 23:31:55.872379 transpector-0.1.0/PKG-INFO
--rw-r--r--   0 rkopel001   (501) staff       (20)     3589 2023-05-25 14:16:58.000000 transpector-0.1.0/README.md
--rw-r--r--   0 rkopel001   (501) staff       (20)       38 2023-05-25 23:31:55.873023 transpector-0.1.0/setup.cfg
--rw-r--r--   0 rkopel001   (501) staff       (20)      959 2023-05-25 23:19:59.000000 transpector-0.1.0/setup.py
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.468718 transpector-0.1.0/transpector/
--rw-r--r--   0 rkopel001   (501) staff       (20)        0 2023-05-25 10:48:07.000000 transpector-0.1.0/transpector/__init__.py
--rw-r--r--   0 rkopel001   (501) staff       (20)      107 2023-05-25 14:36:12.000000 transpector-0.1.0/transpector/__main__.py
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.477218 transpector-0.1.0/transpector/frontend_dist/
--rw-r--r--   0 rkopel001   (501) staff       (20)     2113 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/404.html
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.462485 transpector-0.1.0/transpector/frontend_dist/_next/
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.463944 transpector-0.1.0/transpector/frontend_dist/_next/static/
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.478493 transpector-0.1.0/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/
--rw-r--r--   0 rkopel001   (501) staff       (20)      762 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/_buildManifest.js
--rw-r--r--   0 rkopel001   (501) staff       (20)       80 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/_ssgManifest.js
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.688090 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/
--rw-r--r--   0 rkopel001   (501) staff       (20)    19026 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/08548717-255a240eeda86295.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     8184 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/0e226fb0-fb7c5a372698c63c.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    89456 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/0f7a40cd.b588aa398396b85f.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1890 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1053.adb29a47c34b267a.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2736 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1084.8bd09a422bf924f1.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    25359 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1390.ba90fcba98c196ac.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    22042 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1426.873d7ab40d9ecad4.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2523 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1446.729b459281b981b9.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    12619 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1448.4cb302a7eed94256.js
--rw-r--r--   0 rkopel001   (501) staff       (20)  1570034 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1630-8d43febe391012b1.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     5867 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1650.06a77268379b94b2.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3814 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1660.76cc05d00e5034ad.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     6890 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/177.e4e8e92e618e66e8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     9505 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1770.ffd38031b937c10a.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2125 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1873.ad239337a916524b.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1054 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1920.e6bf04b81039b68b.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    18412 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2016.8b2b4ce7334096dd.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2146 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2040.2b48b43e5c9bbd94.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     8348 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2119.0cb64fe9bc609787.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    27292 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2136.3c7248e1cb33b0f2.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3723 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/228.bcd421992bab4a0b.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    11724 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2314.ce3a0e1828ad2d06.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    94884 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2386.d1eeedc6355d2049.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    10927 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2406.04743ed8b26fbb4f.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   160515 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2443530c-a9cf9b7299898cfe.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    10384 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2542.82fcb9f7206aadce.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     5211 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2602.b42aa7598d8adcd0.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      685 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2675.3af9b237ab623dbf.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   101917 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2750.8797475277eda6ef.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1617 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2877.4a5ca5df09892683.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    69738 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/29107295.54c46f60208f68c8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    55439 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2953.31d72d469664b813.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    72786 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2964.49fbbbec2f07a6f8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    23772 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2dc05096-4dd543d4a3a048a7.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2921 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/305.89841c282a61cef8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4086 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3203.4b4ad54c6039f230.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2402 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3283.4aa4cab7aec29491.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    65304 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/328748d6.0b27772991a6dc26.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2234 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3314.141e2dca41748fac.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2453 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3465.77dee7ec6cc7e947.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2613 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3482.f8558073446e8bd9.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     8006 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3509.b3d99b2815ff8ca5.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3426 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3519.2a44d25a006ebc05.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     7524 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3520.e86e9887c97ae6f2.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3535 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/370.d28d8b4dda7a28fa.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    15199 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3724.66a3078f81accdec.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    30640 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3804.c70bbd7bc76d209e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    59965 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3871.21b541b2261ca2f9.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4211 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3883.5e03e3a398cf3720.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2664 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3993.45bba5349434ad56.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    13246 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3a2b0ac0-2053cf76b055ba83.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4206 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/402.3f3e56dcc798bafe.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1334 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4111.b2921dceac574faf.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4232 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4144.d7264e550bf9aa39.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2340 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4163.d52adce0c4cb89c5.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3977 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4212.15885059e8078ec8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     9771 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4293.9de2fa8f5848563f.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     6561 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4323.a71ccfb6a77dd78e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     5258 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4439.7f32805042ce478e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2886 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4511.dbd0c0aaa63f1ec9.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   758310 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/455abed8.d5960d955583aa92.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2477 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4732.fbcbca870e2812a4.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    40100 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4778.28eb8509a085a653.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2948 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4796.c545e50f2ff935e7.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4220 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4812.8df1cf6b1556ba3d.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2653 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4879.862b5a386c6b86a0.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    68534 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4920.de9b149d5b43b1cf.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   153338 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4ad82c5e.bc4ef951e8cee9c1.js
--rw-r--r--   0 rkopel001   (501) staff       (20)  2167173 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5058.7731b57a8664939b.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    12445 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5122.8964bdfb44ce724e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     6044 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5134.a121d8d21d1c9247.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    41704 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/524.b3b12dce2d0006ba.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4281 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5372.156686248b75341d.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4518 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5648.267f082c55c2b106.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    14314 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5746.e3e7d81cb21002fe.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     6650 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5753.b7dbc47d5bb85861.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2049 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5815.a2728b3992c996c3.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3404 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5819.6eac58d8c93262b3.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      281 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5861.ffe9286214f4218e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     6462 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5879.01cab74f0917f36d.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      289 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5934.6b3da8b1ac28dae5.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    77343 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5a3f41a5-57457efe4b67e95a.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4349 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6059.397bb834d11ff6b5.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4061 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6062.831fce20a86c4ab8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     5420 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6092.d604d5262c942c63.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4981 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6121.07bf76517bbc2dd2.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2794 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/617.359b421db498d43e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      971 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6395.6e51d035839ff4ba.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1217 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6443.a1c9257ad6c47d80.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3353 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6471.cb795f11f73576f4.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    15204 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6560.f1429c4fdca1ee34.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4956 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6665.8350b94f2a309c5f.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    54883 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6686.11f6e20ed4b47fa6.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2625 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6692.dd74b5f83817cb40.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3678 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/673.5310afdb2da5faad.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3152 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6732.d813e460e261d8ef.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2078 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6991.be0212d2d320173c.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3975 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7001.c72447cd49593124.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    73700 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/702997f1.9212a75de09d4df0.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2010 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7213.d8a3150d04a604bc.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    19425 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/72acface-e5ed40f38f904ff0.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     5221 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7315.3ca5dd95b74450ea.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3093 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7365.72718ce4ca51b05b.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     9103 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7370.ab056e5d030e94cf.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     7831 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7421.6e55431a3f7b261d.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      433 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7475.0017763814cf5003.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   210199 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7508.2855b0706bf26f67.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1903 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7525.f7c93eb403c6c9c0.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     9490 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/754.f37798f24a28a360.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3644 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/758.62bb49093c001300.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     8006 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7590.da33099f28f7343c.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1269 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7601.1bdb63794564ce90.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2148 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7663.9a6c03f54df26cbc.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      896 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7762.b997013a52e9b865.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    78956 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7775.2e2aeeafc84a7ad4.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3161 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/786.fa5e21d15f3bc824.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    22218 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7917.d0a43af9dcac157e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2131 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7988.0fe9a294bf19405d.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    25846 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8007.6958f6f4c9375211.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      889 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8029.aa6c08cba91dd332.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    77266 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8037.1900481db2939e93.js
--rw-r--r--   0 rkopel001   (501) staff       (20)  2074632 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8042.7102477834119306.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      955 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8142.d8e6c66ac26970a0.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1752 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8171.da41f4d3690366fc.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4707 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8283.f41216fedc310fb2.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    54581 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8331.c05961d3317723f8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2657 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8393.4276c63baa000f93.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    38840 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8512.04a122c7abe09f85.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     7446 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8561.e0ae2c126e26850c.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   542986 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/85b6cb10.3db11306353dd6b4.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    12372 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8678.80cf7703c175b81a.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2424 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/870.c1277ad0599a1203.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2864 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8724.c7b83652d073185b.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1972 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8770.44d2f8c73be18acf.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    39671 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8825.95fe69ef240ad226.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      886 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/889.4a330cc153172197.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2890 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8910.ec6846732bff95bc.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     6280 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8915.056c1402f901ae7d.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      791 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9071.fc8362f20765bef4.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1481 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9121.9917041a899b93b8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   120197 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9230.d131be9aadfc6a17.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2255 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9232.61d440e4c3b2b427.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    84400 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9277.a16c07843c073298.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    16920 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9296.4f23080e808bc92e.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     3967 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9558.9bf5494ebdf03040.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    37392 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9607.c428674d5c072f92.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     1713 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9713.f1d5b41171c6487d.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4652 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9781.7a6517b3f4614b45.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   198192 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9826.cf4131d537c8ed72.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     4211 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9831.296c1ea16c1953c3.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     2538 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9972.fd259588474eb11b.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    36456 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/ab5c09eb-707dbcabaaeae5ad.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   105703 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/ac0f5318.05716e5c42c8263f.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    20749 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/b1bb7d45-c13bcc9c04a6e2b5.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    86635 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/b637e9a5.5e5cb870404af256.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   129215 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/bd65aaa0.fe3593ec9d17d461.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      283 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/f287e01f-a4871307686885f5.js
--rw-r--r--   0 rkopel001   (501) staff       (20)   275117 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/main-3ced503a3320a6c1.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    88170 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/main-app-59a34855dfcb93b1.js
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.690267 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/pages/
--rw-r--r--   0 rkopel001   (501) staff       (20)     1382 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/pages/_app-949612246a7b1393.js
--rw-r--r--   0 rkopel001   (501) staff       (20)      248 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/pages/_error-48231c25f4fdaf06.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    33986 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/pages/index-84f6f8c197ff4895.js
--rw-r--r--   0 rkopel001   (501) staff       (20)    91460 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 rkopel001   (501) staff       (20)     8762 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/webpack-82c067397cfcc59a.js
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.691561 transpector-0.1.0/transpector/frontend_dist/_next/static/css/
--rw-r--r--   0 rkopel001   (501) staff       (20)    11293 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/css/45eccb5d7dcc0d8c.css
--rw-r--r--   0 rkopel001   (501) staff       (20)    12236 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/css/88da4da6c702ca4f.css
--rw-r--r--   0 rkopel001   (501) staff       (20)   254796 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/css/9b22a190adf5cd66.css
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.869411 transpector-0.1.0/transpector/frontend_dist/_next/static/media/
--rw-r--r--   0 rkopel001   (501) staff       (20)     1042 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/add-above.ee286b1c.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1121 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/add-below.bcf3422e.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      176 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/add.8f2126a6.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      306 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/bad.2c188c60.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      661 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/bell.bccaf100.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      308 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/blank.a4bbd63d.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      899 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/bug-dot.326bc45a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      534 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/bug.e30064ad.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     2430 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/build.e3fdf668.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      246 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/caret-down-empty-thin.f6894985.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      231 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/caret-down-empty.16b5c137.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      206 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/caret-down.1600b64a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      211 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/caret-left.d607c024.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      211 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/caret-right.45b8bd09.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      248 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/caret-up-empty-thin.912759a9.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      203 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/caret-up.9b98d201.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1086 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/case-sensitive.eaefe455.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      209 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/check.0991dc26.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      265 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/circle-empty.4dad54e2.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      158 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/circle.114607e4.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      396 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/clear.f255d27d.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      505 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/close.563b4f49.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      388 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/code-check.99d4f00e.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      262 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/code.fbdeee94.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      423 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/collapse-all.41b2dc7a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      406 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/console.57361ea6.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      340 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/copy.2bfc5d39.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      572 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/copyright.f38f4ec0.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      551 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/cut.18edde39.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      265 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/delete.a777a562.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      182 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/download.e0245bbf.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1325 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/duplicate.8815451e.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      290 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/edit.7fbc6db4.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      231 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/ellipses.dba28113.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      214 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/error.0caf9ea6.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      442 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/expand-all.81b631fe.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      433 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/extension.50386a9c.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)    89988 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.0e53fe4f.woff
--rw-r--r--   0 rkopel001   (501) staff       (20)    76736 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.7edea186.woff2
--rw-r--r--   0 rkopel001   (501) staff       (20)   133988 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.9c02eaf6.ttf
--rw-r--r--   0 rkopel001   (501) staff       (20)   747927 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.a76d53bf.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)   134294 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.b2970adc.eot
--rw-r--r--   0 rkopel001   (501) staff       (20)    16276 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.04dd5282.woff
--rw-r--r--   0 rkopel001   (501) staff       (20)    33736 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.7346017c.ttf
--rw-r--r--   0 rkopel001   (501) staff       (20)    34034 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.a0140e7c.eot
--rw-r--r--   0 rkopel001   (501) staff       (20)    13224 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.e2b3a9dc.woff2
--rw-r--r--   0 rkopel001   (501) staff       (20)   144714 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.ee37fbcc.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)    78268 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.620019ed.woff2
--rw-r--r--   0 rkopel001   (501) staff       (20)   203030 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.974801a4.eot
--rw-r--r--   0 rkopel001   (501) staff       (20)   918991 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.cd7322bf.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)   202744 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.d5b0a356.ttf
--rw-r--r--   0 rkopel001   (501) staff       (20)   101648 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.e67670b0.woff
--rw-r--r--   0 rkopel001   (501) staff       (20)      200 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/fast-forward.f82230c4.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      178 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/file-upload.44fd837e.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      412 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/file.80a9f304.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      503 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/filter-dot.47fa93c4.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      187 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/filter-list.9e70c93a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      414 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/filter.538fe88b.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      396 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/folder-favorite.7f8c9bd5.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      236 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/folder.0d235aaf.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      248 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/home.32ae995c.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      826 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/html5.ea435392.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      401 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/image.82357447.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1581 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/info.4d82eb41.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      288 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/inspector.791cc05d.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      877 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/json.a2c296bb.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      954 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/julia.499ac74e.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1109 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/jupyter-favicon.b19d8551.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     2729 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/jupyter.a48871a7.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     4156 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/jupyterlab-wordmark.6280567a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      321 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/kernel.273d3780.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      385 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/keyboard.3b314c65.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      360 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/launch.6417683d.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      268 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/launcher.0453ed19.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      155 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/line-form.3e38ab09.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      352 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/link.170ecd8b.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      324 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/list.c48a0dd4.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      379 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/markdown.60974264.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      549 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/move-down.5e4a3948.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      559 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/move-up.fa81409d.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      275 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/new-folder.e3dd5db9.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      848 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/not-trusted.8bc17823.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      284 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/notebook.9b4747ea.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      300 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/numbering.60a6786d.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      279 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/offline-bolt.8d942d9a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      805 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/palette.14c4709b.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      361 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/paste.3d3cadcf.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1266 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/pdf.f6a1dc59.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1840 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/python.0ffed0a2.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      424 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/r-kernel.cb4265e1.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     2683 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/react.c81f1b87.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      335 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/redo.ecef5f0c.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      356 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/refresh.dae7f1f4.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      564 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/regex.fa85da44.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      174 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/run.cbdeb7c0.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      313 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/running.9890c96a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      303 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/save.2c9f21a7.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      388 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/search.77371ff0.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      811 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/settings.454fe53f.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1279 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/share.ccbe241a.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      287 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/spreadsheet.486ad38c.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      220 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/stop.88696d03.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      237 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/tab.67683cb0.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      258 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/table-rows.1053696f.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      768 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/tag.8887c8e5.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     2537 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/terminal.0a8eb862.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      238 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/text-editor.52a85e17.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      487 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/toc.05490e17.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      261 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/tree-view.0a94d13b.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      777 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/trusted.3ac2122f.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      283 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/undo.0c5afedd.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      208 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/user.a13160b1.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1069 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/users.cba8edb3.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      331 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/vega.c0ae7146.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     1636 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/word.c993422c.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      375 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/_next/static/media/yaml.267ef972.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)    25931 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/favicon.ico
--rw-r--r--   0 rkopel001   (501) staff       (20)     2312 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/index.html
--rw-r--r--   0 rkopel001   (501) staff       (20)     1375 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/next.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)      629 2023-05-23 14:44:18.000000 transpector-0.1.0/transpector/frontend_dist/vercel.svg
--rw-r--r--   0 rkopel001   (501) staff       (20)     2448 2023-05-12 10:41:56.000000 transpector-0.1.0/transpector/jupyter_server_config.py
--rw-r--r--   0 rkopel001   (501) staff       (20)     8043 2023-05-25 14:49:54.000000 transpector-0.1.0/transpector/launch.py
--rw-r--r--   0 rkopel001   (501) staff       (20)     9171 2023-05-25 14:20:21.000000 transpector-0.1.0/transpector/main.py
--rw-r--r--   0 rkopel001   (501) staff       (20)     2471 2023-05-17 13:01:46.000000 transpector-0.1.0/transpector/model.py
--rw-r--r--   0 rkopel001   (501) staff       (20)     6829 2023-05-10 15:05:12.000000 transpector-0.1.0/transpector/model_setup.py
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.870666 transpector-0.1.0/transpector/notebooks/
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.871584 transpector-0.1.0/transpector/notebooks/.ipynb_checkpoints/
--rw-r--r--   0 rkopel001   (501) staff       (20)    14073 2023-05-23 11:35:42.000000 transpector-0.1.0/transpector/notebooks/.ipynb_checkpoints/main-checkpoint.ipynb
--rw-r--r--   0 rkopel001   (501) staff       (20)        0 2023-05-25 14:54:23.000000 transpector-0.1.0/transpector/notebooks/__init__.py
--rw-r--r--   0 rkopel001   (501) staff       (20)    14670 2023-05-25 14:20:31.000000 transpector-0.1.0/transpector/notebooks/main.ipynb
-drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-25 23:31:55.474129 transpector-0.1.0/transpector.egg-info/
--rw-r--r--   0 rkopel001   (501) staff       (20)     3879 2023-05-25 23:31:51.000000 transpector-0.1.0/transpector.egg-info/PKG-INFO
--rw-r--r--   0 rkopel001   (501) staff       (20)    20615 2023-05-25 23:31:51.000000 transpector-0.1.0/transpector.egg-info/SOURCES.txt
--rw-r--r--   0 rkopel001   (501) staff       (20)        1 2023-05-25 23:31:51.000000 transpector-0.1.0/transpector.egg-info/dependency_links.txt
--rw-r--r--   0 rkopel001   (501) staff       (20)       58 2023-05-25 23:31:51.000000 transpector-0.1.0/transpector.egg-info/entry_points.txt
--rw-r--r--   0 rkopel001   (501) staff       (20)      118 2023-05-25 23:31:51.000000 transpector-0.1.0/transpector.egg-info/requires.txt
--rw-r--r--   0 rkopel001   (501) staff       (20)       12 2023-05-25 23:31:51.000000 transpector-0.1.0/transpector.egg-info/top_level.txt
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:28.002411 transpector-0.1.1/
+-rw-r--r--   0 rkopel001   (501) staff       (20)       88 2023-05-25 23:31:34.000000 transpector-0.1.1/MANIFEST.in
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4232 2023-05-26 12:18:28.002103 transpector-0.1.1/PKG-INFO
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3940 2023-05-26 12:14:01.000000 transpector-0.1.1/README.md
+-rw-r--r--   0 rkopel001   (501) staff       (20)       38 2023-05-26 12:18:28.002482 transpector-0.1.1/setup.cfg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      893 2023-05-26 12:18:05.000000 transpector-0.1.1/setup.py
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:25.985128 transpector-0.1.1/transpector/
+-rw-r--r--   0 rkopel001   (501) staff       (20)        0 2023-05-25 10:48:07.000000 transpector-0.1.1/transpector/__init__.py
+-rw-r--r--   0 rkopel001   (501) staff       (20)      107 2023-05-25 14:36:12.000000 transpector-0.1.1/transpector/__main__.py
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:26.005860 transpector-0.1.1/transpector/frontend_dist/
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2113 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/404.html
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:25.965716 transpector-0.1.1/transpector/frontend_dist/_next/
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:25.966836 transpector-0.1.1/transpector/frontend_dist/_next/static/
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:26.013213 transpector-0.1.1/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/
+-rw-r--r--   0 rkopel001   (501) staff       (20)      762 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/_buildManifest.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)       80 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/_ssgManifest.js
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:27.773290 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/
+-rw-r--r--   0 rkopel001   (501) staff       (20)    19026 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/08548717-255a240eeda86295.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     8184 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/0e226fb0-fb7c5a372698c63c.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    89456 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/0f7a40cd.b588aa398396b85f.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1890 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1053.adb29a47c34b267a.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2736 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1084.8bd09a422bf924f1.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    25359 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1390.ba90fcba98c196ac.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    22042 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1426.873d7ab40d9ecad4.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2523 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1446.729b459281b981b9.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    12619 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1448.4cb302a7eed94256.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)  1570034 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1630-8d43febe391012b1.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     5867 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1650.06a77268379b94b2.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3814 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1660.76cc05d00e5034ad.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     6890 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/177.e4e8e92e618e66e8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     9505 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1770.ffd38031b937c10a.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2125 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1873.ad239337a916524b.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1054 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1920.e6bf04b81039b68b.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    18412 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2016.8b2b4ce7334096dd.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2146 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2040.2b48b43e5c9bbd94.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     8348 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2119.0cb64fe9bc609787.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    27292 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2136.3c7248e1cb33b0f2.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3723 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/228.bcd421992bab4a0b.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    11724 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2314.ce3a0e1828ad2d06.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    94884 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2386.d1eeedc6355d2049.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    10927 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2406.04743ed8b26fbb4f.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   160515 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2443530c-a9cf9b7299898cfe.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    10384 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2542.82fcb9f7206aadce.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     5211 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2602.b42aa7598d8adcd0.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      685 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2675.3af9b237ab623dbf.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   101917 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2750.8797475277eda6ef.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1617 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2877.4a5ca5df09892683.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    69738 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/29107295.54c46f60208f68c8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    55439 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2953.31d72d469664b813.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    72786 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2964.49fbbbec2f07a6f8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    23772 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2dc05096-4dd543d4a3a048a7.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2921 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/305.89841c282a61cef8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4086 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3203.4b4ad54c6039f230.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2402 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3283.4aa4cab7aec29491.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    65304 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/328748d6.0b27772991a6dc26.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2234 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3314.141e2dca41748fac.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2453 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3465.77dee7ec6cc7e947.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2613 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3482.f8558073446e8bd9.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     8006 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3509.b3d99b2815ff8ca5.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3426 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3519.2a44d25a006ebc05.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     7524 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3520.e86e9887c97ae6f2.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3535 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/370.d28d8b4dda7a28fa.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    15199 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3724.66a3078f81accdec.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    30640 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3804.c70bbd7bc76d209e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    59965 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3871.21b541b2261ca2f9.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4211 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3883.5e03e3a398cf3720.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2664 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3993.45bba5349434ad56.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    13246 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3a2b0ac0-2053cf76b055ba83.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4206 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/402.3f3e56dcc798bafe.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1334 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4111.b2921dceac574faf.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4232 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4144.d7264e550bf9aa39.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2340 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4163.d52adce0c4cb89c5.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3977 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4212.15885059e8078ec8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     9771 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4293.9de2fa8f5848563f.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     6561 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4323.a71ccfb6a77dd78e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     5258 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4439.7f32805042ce478e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2886 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4511.dbd0c0aaa63f1ec9.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   758310 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/455abed8.d5960d955583aa92.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2477 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4732.fbcbca870e2812a4.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    40100 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4778.28eb8509a085a653.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2948 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4796.c545e50f2ff935e7.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4220 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4812.8df1cf6b1556ba3d.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2653 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4879.862b5a386c6b86a0.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    68534 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4920.de9b149d5b43b1cf.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   153338 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4ad82c5e.bc4ef951e8cee9c1.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)  2167173 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5058.7731b57a8664939b.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    12445 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5122.8964bdfb44ce724e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     6044 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5134.a121d8d21d1c9247.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    41704 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/524.b3b12dce2d0006ba.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4281 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5372.156686248b75341d.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4518 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5648.267f082c55c2b106.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    14314 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5746.e3e7d81cb21002fe.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     6650 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5753.b7dbc47d5bb85861.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2049 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5815.a2728b3992c996c3.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3404 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5819.6eac58d8c93262b3.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      281 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5861.ffe9286214f4218e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     6462 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5879.01cab74f0917f36d.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      289 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5934.6b3da8b1ac28dae5.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    77343 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5a3f41a5-57457efe4b67e95a.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4349 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6059.397bb834d11ff6b5.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4061 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6062.831fce20a86c4ab8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     5420 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6092.d604d5262c942c63.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4981 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6121.07bf76517bbc2dd2.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2794 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/617.359b421db498d43e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      971 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6395.6e51d035839ff4ba.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1217 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6443.a1c9257ad6c47d80.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3353 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6471.cb795f11f73576f4.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    15204 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6560.f1429c4fdca1ee34.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4956 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6665.8350b94f2a309c5f.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    54883 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6686.11f6e20ed4b47fa6.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2625 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6692.dd74b5f83817cb40.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3678 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/673.5310afdb2da5faad.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3152 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6732.d813e460e261d8ef.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2078 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6991.be0212d2d320173c.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3975 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7001.c72447cd49593124.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    73700 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/702997f1.9212a75de09d4df0.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2010 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7213.d8a3150d04a604bc.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    19425 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/72acface-e5ed40f38f904ff0.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     5221 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7315.3ca5dd95b74450ea.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3093 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7365.72718ce4ca51b05b.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     9103 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7370.ab056e5d030e94cf.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     7831 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7421.6e55431a3f7b261d.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      433 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7475.0017763814cf5003.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   210199 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7508.2855b0706bf26f67.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1903 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7525.f7c93eb403c6c9c0.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     9490 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/754.f37798f24a28a360.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3644 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/758.62bb49093c001300.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     8006 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7590.da33099f28f7343c.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1269 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7601.1bdb63794564ce90.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2148 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7663.9a6c03f54df26cbc.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      896 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7762.b997013a52e9b865.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    78956 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7775.2e2aeeafc84a7ad4.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3161 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/786.fa5e21d15f3bc824.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    22218 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7917.d0a43af9dcac157e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2131 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7988.0fe9a294bf19405d.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    25846 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8007.6958f6f4c9375211.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      889 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8029.aa6c08cba91dd332.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    77266 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8037.1900481db2939e93.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)  2074632 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8042.7102477834119306.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      955 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8142.d8e6c66ac26970a0.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1752 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8171.da41f4d3690366fc.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4707 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8283.f41216fedc310fb2.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    54581 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8331.c05961d3317723f8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2657 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8393.4276c63baa000f93.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    38840 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8512.04a122c7abe09f85.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     7446 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8561.e0ae2c126e26850c.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   542986 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/85b6cb10.3db11306353dd6b4.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    12372 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8678.80cf7703c175b81a.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2424 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/870.c1277ad0599a1203.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2864 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8724.c7b83652d073185b.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1972 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8770.44d2f8c73be18acf.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    39671 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8825.95fe69ef240ad226.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      886 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/889.4a330cc153172197.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2890 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8910.ec6846732bff95bc.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     6280 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8915.056c1402f901ae7d.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      791 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9071.fc8362f20765bef4.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1481 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9121.9917041a899b93b8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   120197 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9230.d131be9aadfc6a17.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2255 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9232.61d440e4c3b2b427.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    84400 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9277.a16c07843c073298.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    16920 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9296.4f23080e808bc92e.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     3967 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9558.9bf5494ebdf03040.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    37392 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9607.c428674d5c072f92.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1713 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9713.f1d5b41171c6487d.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4652 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9781.7a6517b3f4614b45.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   198192 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9826.cf4131d537c8ed72.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4211 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9831.296c1ea16c1953c3.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2538 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9972.fd259588474eb11b.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    36456 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/ab5c09eb-707dbcabaaeae5ad.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   105703 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/ac0f5318.05716e5c42c8263f.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    20749 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/b1bb7d45-c13bcc9c04a6e2b5.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    86635 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/b637e9a5.5e5cb870404af256.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   129215 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/bd65aaa0.fe3593ec9d17d461.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      283 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/f287e01f-a4871307686885f5.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)   275117 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/main-3ced503a3320a6c1.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    88170 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/main-app-59a34855dfcb93b1.js
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:27.797567 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/pages/
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1382 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/pages/_app-949612246a7b1393.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)      248 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/pages/_error-48231c25f4fdaf06.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    33986 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/pages/index-84f6f8c197ff4895.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)    91460 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 rkopel001   (501) staff       (20)     8762 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/webpack-82c067397cfcc59a.js
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:27.810840 transpector-0.1.1/transpector/frontend_dist/_next/static/css/
+-rw-r--r--   0 rkopel001   (501) staff       (20)    11293 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/css/45eccb5d7dcc0d8c.css
+-rw-r--r--   0 rkopel001   (501) staff       (20)    12236 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/css/88da4da6c702ca4f.css
+-rw-r--r--   0 rkopel001   (501) staff       (20)   254796 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/css/9b22a190adf5cd66.css
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:27.990789 transpector-0.1.1/transpector/frontend_dist/_next/static/media/
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1042 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/add-above.ee286b1c.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1121 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/add-below.bcf3422e.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      176 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/add.8f2126a6.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      306 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/bad.2c188c60.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      661 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/bell.bccaf100.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      308 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/blank.a4bbd63d.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      899 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/bug-dot.326bc45a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      534 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/bug.e30064ad.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2430 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/build.e3fdf668.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      246 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/caret-down-empty-thin.f6894985.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      231 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/caret-down-empty.16b5c137.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      206 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/caret-down.1600b64a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      211 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/caret-left.d607c024.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      211 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/caret-right.45b8bd09.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      248 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/caret-up-empty-thin.912759a9.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      203 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/caret-up.9b98d201.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1086 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/case-sensitive.eaefe455.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      209 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/check.0991dc26.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      265 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/circle-empty.4dad54e2.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      158 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/circle.114607e4.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      396 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/clear.f255d27d.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      505 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/close.563b4f49.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      388 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/code-check.99d4f00e.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      262 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/code.fbdeee94.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      423 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/collapse-all.41b2dc7a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      406 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/console.57361ea6.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      340 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/copy.2bfc5d39.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      572 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/copyright.f38f4ec0.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      551 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/cut.18edde39.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      265 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/delete.a777a562.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      182 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/download.e0245bbf.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1325 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/duplicate.8815451e.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      290 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/edit.7fbc6db4.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      231 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/ellipses.dba28113.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      214 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/error.0caf9ea6.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      442 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/expand-all.81b631fe.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      433 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/extension.50386a9c.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)    89988 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.0e53fe4f.woff
+-rw-r--r--   0 rkopel001   (501) staff       (20)    76736 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.7edea186.woff2
+-rw-r--r--   0 rkopel001   (501) staff       (20)   133988 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.9c02eaf6.ttf
+-rw-r--r--   0 rkopel001   (501) staff       (20)   747927 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.a76d53bf.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)   134294 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.b2970adc.eot
+-rw-r--r--   0 rkopel001   (501) staff       (20)    16276 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.04dd5282.woff
+-rw-r--r--   0 rkopel001   (501) staff       (20)    33736 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.7346017c.ttf
+-rw-r--r--   0 rkopel001   (501) staff       (20)    34034 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.a0140e7c.eot
+-rw-r--r--   0 rkopel001   (501) staff       (20)    13224 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.e2b3a9dc.woff2
+-rw-r--r--   0 rkopel001   (501) staff       (20)   144714 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.ee37fbcc.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)    78268 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.620019ed.woff2
+-rw-r--r--   0 rkopel001   (501) staff       (20)   203030 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.974801a4.eot
+-rw-r--r--   0 rkopel001   (501) staff       (20)   918991 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.cd7322bf.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)   202744 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.d5b0a356.ttf
+-rw-r--r--   0 rkopel001   (501) staff       (20)   101648 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.e67670b0.woff
+-rw-r--r--   0 rkopel001   (501) staff       (20)      200 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/fast-forward.f82230c4.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      178 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/file-upload.44fd837e.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      412 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/file.80a9f304.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      503 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/filter-dot.47fa93c4.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      187 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/filter-list.9e70c93a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      414 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/filter.538fe88b.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      396 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/folder-favorite.7f8c9bd5.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      236 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/folder.0d235aaf.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      248 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/home.32ae995c.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      826 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/html5.ea435392.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      401 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/image.82357447.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1581 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/info.4d82eb41.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      288 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/inspector.791cc05d.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      877 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/json.a2c296bb.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      954 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/julia.499ac74e.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1109 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/jupyter-favicon.b19d8551.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2729 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/jupyter.a48871a7.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4156 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/jupyterlab-wordmark.6280567a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      321 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/kernel.273d3780.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      385 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/keyboard.3b314c65.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      360 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/launch.6417683d.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      268 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/launcher.0453ed19.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      155 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/line-form.3e38ab09.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      352 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/link.170ecd8b.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      324 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/list.c48a0dd4.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      379 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/markdown.60974264.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      549 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/move-down.5e4a3948.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      559 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/move-up.fa81409d.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      275 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/new-folder.e3dd5db9.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      848 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/not-trusted.8bc17823.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      284 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/notebook.9b4747ea.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      300 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/numbering.60a6786d.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      279 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/offline-bolt.8d942d9a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      805 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/palette.14c4709b.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      361 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/paste.3d3cadcf.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1266 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/pdf.f6a1dc59.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1840 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/python.0ffed0a2.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      424 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/r-kernel.cb4265e1.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2683 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/react.c81f1b87.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      335 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/redo.ecef5f0c.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      356 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/refresh.dae7f1f4.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      564 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/regex.fa85da44.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      174 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/run.cbdeb7c0.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      313 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/running.9890c96a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      303 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/save.2c9f21a7.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      388 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/search.77371ff0.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      811 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/settings.454fe53f.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1279 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/share.ccbe241a.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      287 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/spreadsheet.486ad38c.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      220 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/stop.88696d03.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      237 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/tab.67683cb0.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      258 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/table-rows.1053696f.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      768 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/tag.8887c8e5.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2537 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/terminal.0a8eb862.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      238 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/text-editor.52a85e17.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      487 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/toc.05490e17.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      261 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/tree-view.0a94d13b.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      777 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/trusted.3ac2122f.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      283 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/undo.0c5afedd.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      208 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/user.a13160b1.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1069 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/users.cba8edb3.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      331 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/vega.c0ae7146.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1636 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/word.c993422c.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      375 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/_next/static/media/yaml.267ef972.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)    25931 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/favicon.ico
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2312 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/index.html
+-rw-r--r--   0 rkopel001   (501) staff       (20)     1375 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/next.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)      629 2023-05-23 14:44:18.000000 transpector-0.1.1/transpector/frontend_dist/vercel.svg
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2448 2023-05-12 10:41:56.000000 transpector-0.1.1/transpector/jupyter_server_config.py
+-rw-r--r--   0 rkopel001   (501) staff       (20)     8043 2023-05-25 14:49:54.000000 transpector-0.1.1/transpector/launch.py
+-rw-r--r--   0 rkopel001   (501) staff       (20)     9171 2023-05-25 14:20:21.000000 transpector-0.1.1/transpector/main.py
+-rw-r--r--   0 rkopel001   (501) staff       (20)     2471 2023-05-17 13:01:46.000000 transpector-0.1.1/transpector/model.py
+-rw-r--r--   0 rkopel001   (501) staff       (20)     6829 2023-05-10 15:05:12.000000 transpector-0.1.1/transpector/model_setup.py
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:27.998713 transpector-0.1.1/transpector/notebooks/
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:28.001532 transpector-0.1.1/transpector/notebooks/.ipynb_checkpoints/
+-rw-r--r--   0 rkopel001   (501) staff       (20)    14073 2023-05-23 11:35:42.000000 transpector-0.1.1/transpector/notebooks/.ipynb_checkpoints/main-checkpoint.ipynb
+-rw-r--r--   0 rkopel001   (501) staff       (20)        0 2023-05-25 14:54:23.000000 transpector-0.1.1/transpector/notebooks/__init__.py
+-rw-r--r--   0 rkopel001   (501) staff       (20)    14670 2023-05-25 14:20:31.000000 transpector-0.1.1/transpector/notebooks/main.ipynb
+drwxr-xr-x   0 rkopel001   (501) staff       (20)        0 2023-05-26 12:18:25.993341 transpector-0.1.1/transpector.egg-info/
+-rw-r--r--   0 rkopel001   (501) staff       (20)     4232 2023-05-26 12:18:22.000000 transpector-0.1.1/transpector.egg-info/PKG-INFO
+-rw-r--r--   0 rkopel001   (501) staff       (20)    20615 2023-05-26 12:18:22.000000 transpector-0.1.1/transpector.egg-info/SOURCES.txt
+-rw-r--r--   0 rkopel001   (501) staff       (20)        1 2023-05-26 12:18:22.000000 transpector-0.1.1/transpector.egg-info/dependency_links.txt
+-rw-r--r--   0 rkopel001   (501) staff       (20)       57 2023-05-26 12:18:22.000000 transpector-0.1.1/transpector.egg-info/entry_points.txt
+-rw-r--r--   0 rkopel001   (501) staff       (20)      118 2023-05-26 12:18:22.000000 transpector-0.1.1/transpector.egg-info/requires.txt
+-rw-r--r--   0 rkopel001   (501) staff       (20)       12 2023-05-26 12:18:22.000000 transpector-0.1.1/transpector.egg-info/top_level.txt
```

### Comparing `transpector-0.1.0/PKG-INFO` & `transpector-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: transpector
-Version: 0.1.0
+Version: 0.1.1
 Summary: Visually inspect, analyse and debug transformer models. Aimed at reducing cycle times for interpretability research and lowering the barrier to entry.
-Home-page: UNKNOWN
 Author: Rob Kopel
 License: LICENSE
-Platform: UNKNOWN
+Description-Content-Type: text/markdown
 
-# Transpector
+# 🔬 Transpector
 Visually inspect, analyse and debug transformer models. Aimed at reducing cycle times for interpretability research and lowering the barrier to entry.
 ## Getting Started
 
+To use Transpector first install the package `pip install transpector` then you can start it from the command line with `transpector`. Once it's ready, navigate to `http://127.0.0.1:8000/index.html` to get started.
+
+#### Using Transpector
+
+Coming soon!
 ## Developing locally
 
 In it's development setting currently you have to run two parts, a python script kicking off Jupyter Server (this spawns a fastAPI backend in the same event loop as the IPython Kernal), and a Next JS Server. Next JS will be compiled and served as a static file from fastAPI eventually.
 
 To run Next JS
 ```bash
 npm run dev
@@ -39,15 +43,15 @@
 And finally, use our installed package to run the server:
 ```
 transpector run
 ```
 
 ## To Do
 
-### Milestone 2
+#### Milestone 2️⃣
 - [ ] Add ability to split each token into seperate node
 - [ ] Inferencing layer cutoff
 - [ ] Causal tracing
 - [ ] Knowledge editing
 - [ ] Basic Layernorm visuals (what would be useful?)
 - [ ] Text pane batch input
 - [ ] Full dataset input
@@ -61,15 +65,15 @@
 - [ ] Custom model support
 - [ ] Select many nodes and multi-node selection menus
 - [ ] Research replication using transpector
 - [ ] Ability to add notes to activations, weights and nodes
 
 
 
-### Milestone 1
+#### Milestone 1️⃣
 - [ ] Add icons on the edges
 - [ ] Node resizing and rerendering (for canvas nodes)
 - [ ] Weight Analysis: Visualise weights
 - [ ] Weight Analysis: What is the OV circuit trying to copy given a token
 - [ ] Weight Analysis: What is the KQ circuit attention position distribution 
 - [ ] Visual layer folding
 - [ ] Activation freezing
@@ -79,20 +83,21 @@
 - [ ] Optimisation: WebGPU rendering
 - [ ] Optimisation: Remove dead data
 - [ ] Non blocking model updating
 - [ ] KQV composition visualisation
 - [ ] Residual stream analysis visualisation
 - [ ] Notebook scrolling bugs
 - [ ] Improve global state control
-- [ ] Python static hosting
-- [ ] Python package 
-- [ ] Make gifs of features
 - [ ] Compute/ GPU flags/controls from UI
 - [ ] Add correct shortformer positional embedding links
 - [ ] Move to same data structure in py/ js and ws for syncing
+- [ ] Basic usage tutorial
+- [ ] Make gifs of features
+- [ ] Baisc architecture diagram
+- [ ] Pypi package
 - [ ] Add in app credits
 - [ ] Individual activation level ablations
 - [ ] Basic MLP visuals (what would be useful?)
 - [x] Ablations
 - [x] Canvas summed pattern and result rendering
 - [x] Add readme credits
 - [x] Model Outputs
@@ -100,14 +105,16 @@
 - [x] Layernorm nodes
 - [x] Text pane visibility
 - [x] Notebook loading pre existing kernel
 - [x] Upgrade model selection pane
 - [x] Improve typing coverage
 - [x] Next static export
 - [x] Python kickoff script
+- [x] Python static hosting
+- [x] Python package 
 - [x] Model Pane Upgrade
 - [x] Nodes disabled, default and highlighted feature
 - [x] Jupyter-UI upgrade
 - [x] Refactor Nodes and edges code
 - [x] Layernaming bugs
 - [x] Visual spacing optimisation
 - [x] Layer groups
@@ -117,8 +124,7 @@
 - [x] Tokenization node
 - [x] Residual stream node
 - [x] Attention text visualisation
 
 
 ## Credits
 This work has only been possible through the usage of Transformer Lens by Neel Nanda and has been heavily inspired by circuitviz by Alan Cooney
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `transpector-0.1.0/README.md` & `transpector-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-# Transpector
+# 🔬 Transpector
 Visually inspect, analyse and debug transformer models. Aimed at reducing cycle times for interpretability research and lowering the barrier to entry.
 ## Getting Started
 
+To use Transpector first install the package `pip install transpector` then you can start it from the command line with `transpector`. Once it's ready, navigate to `http://127.0.0.1:8000/index.html` to get started.
+
+#### Using Transpector
+
+Coming soon!
 ## Developing locally
 
 In it's development setting currently you have to run two parts, a python script kicking off Jupyter Server (this spawns a fastAPI backend in the same event loop as the IPython Kernal), and a Next JS Server. Next JS will be compiled and served as a static file from fastAPI eventually.
 
 To run Next JS
 ```bash
 npm run dev
@@ -30,15 +35,15 @@
 And finally, use our installed package to run the server:
 ```
 transpector run
 ```
 
 ## To Do
 
-### Milestone 2
+#### Milestone 2️⃣
 - [ ] Add ability to split each token into seperate node
 - [ ] Inferencing layer cutoff
 - [ ] Causal tracing
 - [ ] Knowledge editing
 - [ ] Basic Layernorm visuals (what would be useful?)
 - [ ] Text pane batch input
 - [ ] Full dataset input
@@ -52,15 +57,15 @@
 - [ ] Custom model support
 - [ ] Select many nodes and multi-node selection menus
 - [ ] Research replication using transpector
 - [ ] Ability to add notes to activations, weights and nodes
 
 
 
-### Milestone 1
+#### Milestone 1️⃣
 - [ ] Add icons on the edges
 - [ ] Node resizing and rerendering (for canvas nodes)
 - [ ] Weight Analysis: Visualise weights
 - [ ] Weight Analysis: What is the OV circuit trying to copy given a token
 - [ ] Weight Analysis: What is the KQ circuit attention position distribution 
 - [ ] Visual layer folding
 - [ ] Activation freezing
@@ -70,20 +75,21 @@
 - [ ] Optimisation: WebGPU rendering
 - [ ] Optimisation: Remove dead data
 - [ ] Non blocking model updating
 - [ ] KQV composition visualisation
 - [ ] Residual stream analysis visualisation
 - [ ] Notebook scrolling bugs
 - [ ] Improve global state control
-- [ ] Python static hosting
-- [ ] Python package 
-- [ ] Make gifs of features
 - [ ] Compute/ GPU flags/controls from UI
 - [ ] Add correct shortformer positional embedding links
 - [ ] Move to same data structure in py/ js and ws for syncing
+- [ ] Basic usage tutorial
+- [ ] Make gifs of features
+- [ ] Baisc architecture diagram
+- [ ] Pypi package
 - [ ] Add in app credits
 - [ ] Individual activation level ablations
 - [ ] Basic MLP visuals (what would be useful?)
 - [x] Ablations
 - [x] Canvas summed pattern and result rendering
 - [x] Add readme credits
 - [x] Model Outputs
@@ -91,14 +97,16 @@
 - [x] Layernorm nodes
 - [x] Text pane visibility
 - [x] Notebook loading pre existing kernel
 - [x] Upgrade model selection pane
 - [x] Improve typing coverage
 - [x] Next static export
 - [x] Python kickoff script
+- [x] Python static hosting
+- [x] Python package 
 - [x] Model Pane Upgrade
 - [x] Nodes disabled, default and highlighted feature
 - [x] Jupyter-UI upgrade
 - [x] Refactor Nodes and edges code
 - [x] Layernaming bugs
 - [x] Visual spacing optimisation
 - [x] Layer groups
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `transpector-0.1.0/transpector/frontend_dist/404.html` & `transpector-0.1.1/transpector/frontend_dist/404.html`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/_buildManifest.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/_dq4DfiSJ4c6dFR3vFJ4O/_buildManifest.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/08548717-255a240eeda86295.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/08548717-255a240eeda86295.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/0e226fb0-fb7c5a372698c63c.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/0e226fb0-fb7c5a372698c63c.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/0f7a40cd.b588aa398396b85f.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/0f7a40cd.b588aa398396b85f.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1053.adb29a47c34b267a.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1053.adb29a47c34b267a.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1084.8bd09a422bf924f1.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1084.8bd09a422bf924f1.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1390.ba90fcba98c196ac.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1390.ba90fcba98c196ac.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1426.873d7ab40d9ecad4.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1426.873d7ab40d9ecad4.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1446.729b459281b981b9.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1446.729b459281b981b9.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1448.4cb302a7eed94256.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1448.4cb302a7eed94256.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1630-8d43febe391012b1.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1630-8d43febe391012b1.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1650.06a77268379b94b2.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1650.06a77268379b94b2.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1660.76cc05d00e5034ad.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1660.76cc05d00e5034ad.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/177.e4e8e92e618e66e8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/177.e4e8e92e618e66e8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1770.ffd38031b937c10a.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1770.ffd38031b937c10a.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1873.ad239337a916524b.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1873.ad239337a916524b.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/1920.e6bf04b81039b68b.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/1920.e6bf04b81039b68b.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2016.8b2b4ce7334096dd.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2016.8b2b4ce7334096dd.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2040.2b48b43e5c9bbd94.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2040.2b48b43e5c9bbd94.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2119.0cb64fe9bc609787.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2119.0cb64fe9bc609787.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2136.3c7248e1cb33b0f2.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2136.3c7248e1cb33b0f2.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/228.bcd421992bab4a0b.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/228.bcd421992bab4a0b.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2314.ce3a0e1828ad2d06.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2314.ce3a0e1828ad2d06.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2386.d1eeedc6355d2049.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2386.d1eeedc6355d2049.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2406.04743ed8b26fbb4f.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2406.04743ed8b26fbb4f.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2443530c-a9cf9b7299898cfe.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2443530c-a9cf9b7299898cfe.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2542.82fcb9f7206aadce.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2542.82fcb9f7206aadce.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2602.b42aa7598d8adcd0.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2602.b42aa7598d8adcd0.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2675.3af9b237ab623dbf.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2675.3af9b237ab623dbf.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2750.8797475277eda6ef.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2750.8797475277eda6ef.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2877.4a5ca5df09892683.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2877.4a5ca5df09892683.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/29107295.54c46f60208f68c8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/29107295.54c46f60208f68c8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2953.31d72d469664b813.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2953.31d72d469664b813.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2964.49fbbbec2f07a6f8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2964.49fbbbec2f07a6f8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/2dc05096-4dd543d4a3a048a7.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/2dc05096-4dd543d4a3a048a7.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/305.89841c282a61cef8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/305.89841c282a61cef8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3203.4b4ad54c6039f230.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3203.4b4ad54c6039f230.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3283.4aa4cab7aec29491.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3283.4aa4cab7aec29491.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/328748d6.0b27772991a6dc26.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/328748d6.0b27772991a6dc26.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3314.141e2dca41748fac.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3314.141e2dca41748fac.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3465.77dee7ec6cc7e947.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3465.77dee7ec6cc7e947.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3482.f8558073446e8bd9.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3482.f8558073446e8bd9.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3509.b3d99b2815ff8ca5.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3509.b3d99b2815ff8ca5.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3519.2a44d25a006ebc05.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3519.2a44d25a006ebc05.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3520.e86e9887c97ae6f2.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3520.e86e9887c97ae6f2.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/370.d28d8b4dda7a28fa.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/370.d28d8b4dda7a28fa.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3724.66a3078f81accdec.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3724.66a3078f81accdec.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3804.c70bbd7bc76d209e.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3804.c70bbd7bc76d209e.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3871.21b541b2261ca2f9.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3871.21b541b2261ca2f9.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3883.5e03e3a398cf3720.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3883.5e03e3a398cf3720.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3993.45bba5349434ad56.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3993.45bba5349434ad56.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/3a2b0ac0-2053cf76b055ba83.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/3a2b0ac0-2053cf76b055ba83.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/402.3f3e56dcc798bafe.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/402.3f3e56dcc798bafe.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4111.b2921dceac574faf.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4111.b2921dceac574faf.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4144.d7264e550bf9aa39.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4144.d7264e550bf9aa39.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4163.d52adce0c4cb89c5.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4163.d52adce0c4cb89c5.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4212.15885059e8078ec8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4212.15885059e8078ec8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4293.9de2fa8f5848563f.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4293.9de2fa8f5848563f.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4323.a71ccfb6a77dd78e.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4323.a71ccfb6a77dd78e.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4439.7f32805042ce478e.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4439.7f32805042ce478e.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4511.dbd0c0aaa63f1ec9.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4511.dbd0c0aaa63f1ec9.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/455abed8.d5960d955583aa92.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/455abed8.d5960d955583aa92.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4732.fbcbca870e2812a4.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4732.fbcbca870e2812a4.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4778.28eb8509a085a653.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4778.28eb8509a085a653.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4796.c545e50f2ff935e7.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4796.c545e50f2ff935e7.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4812.8df1cf6b1556ba3d.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4812.8df1cf6b1556ba3d.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4879.862b5a386c6b86a0.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4879.862b5a386c6b86a0.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4920.de9b149d5b43b1cf.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4920.de9b149d5b43b1cf.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/4ad82c5e.bc4ef951e8cee9c1.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/4ad82c5e.bc4ef951e8cee9c1.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5058.7731b57a8664939b.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5058.7731b57a8664939b.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5122.8964bdfb44ce724e.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5122.8964bdfb44ce724e.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5134.a121d8d21d1c9247.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5134.a121d8d21d1c9247.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/524.b3b12dce2d0006ba.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/524.b3b12dce2d0006ba.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5372.156686248b75341d.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5372.156686248b75341d.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5648.267f082c55c2b106.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5648.267f082c55c2b106.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5746.e3e7d81cb21002fe.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5746.e3e7d81cb21002fe.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5753.b7dbc47d5bb85861.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5753.b7dbc47d5bb85861.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5815.a2728b3992c996c3.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5815.a2728b3992c996c3.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5819.6eac58d8c93262b3.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5819.6eac58d8c93262b3.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5879.01cab74f0917f36d.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5879.01cab74f0917f36d.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/5a3f41a5-57457efe4b67e95a.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/5a3f41a5-57457efe4b67e95a.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6059.397bb834d11ff6b5.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6059.397bb834d11ff6b5.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6062.831fce20a86c4ab8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6062.831fce20a86c4ab8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6092.d604d5262c942c63.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6092.d604d5262c942c63.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6121.07bf76517bbc2dd2.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6121.07bf76517bbc2dd2.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/617.359b421db498d43e.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/617.359b421db498d43e.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6395.6e51d035839ff4ba.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6395.6e51d035839ff4ba.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6443.a1c9257ad6c47d80.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6443.a1c9257ad6c47d80.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6471.cb795f11f73576f4.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6471.cb795f11f73576f4.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6560.f1429c4fdca1ee34.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6560.f1429c4fdca1ee34.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6665.8350b94f2a309c5f.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6665.8350b94f2a309c5f.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6686.11f6e20ed4b47fa6.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6686.11f6e20ed4b47fa6.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6692.dd74b5f83817cb40.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6692.dd74b5f83817cb40.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/673.5310afdb2da5faad.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/673.5310afdb2da5faad.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6732.d813e460e261d8ef.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6732.d813e460e261d8ef.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/6991.be0212d2d320173c.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/6991.be0212d2d320173c.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7001.c72447cd49593124.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7001.c72447cd49593124.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/702997f1.9212a75de09d4df0.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/702997f1.9212a75de09d4df0.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7213.d8a3150d04a604bc.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7213.d8a3150d04a604bc.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/72acface-e5ed40f38f904ff0.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/72acface-e5ed40f38f904ff0.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7315.3ca5dd95b74450ea.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7315.3ca5dd95b74450ea.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7365.72718ce4ca51b05b.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7365.72718ce4ca51b05b.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7370.ab056e5d030e94cf.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7370.ab056e5d030e94cf.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7421.6e55431a3f7b261d.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7421.6e55431a3f7b261d.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7508.2855b0706bf26f67.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7508.2855b0706bf26f67.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7525.f7c93eb403c6c9c0.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7525.f7c93eb403c6c9c0.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/754.f37798f24a28a360.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/754.f37798f24a28a360.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/758.62bb49093c001300.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/758.62bb49093c001300.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7590.da33099f28f7343c.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7590.da33099f28f7343c.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7601.1bdb63794564ce90.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7601.1bdb63794564ce90.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7663.9a6c03f54df26cbc.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7663.9a6c03f54df26cbc.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7762.b997013a52e9b865.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7762.b997013a52e9b865.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7775.2e2aeeafc84a7ad4.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7775.2e2aeeafc84a7ad4.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/786.fa5e21d15f3bc824.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/786.fa5e21d15f3bc824.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7917.d0a43af9dcac157e.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7917.d0a43af9dcac157e.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/7988.0fe9a294bf19405d.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/7988.0fe9a294bf19405d.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8007.6958f6f4c9375211.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8007.6958f6f4c9375211.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8029.aa6c08cba91dd332.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8029.aa6c08cba91dd332.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8037.1900481db2939e93.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8037.1900481db2939e93.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8042.7102477834119306.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8042.7102477834119306.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8142.d8e6c66ac26970a0.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8142.d8e6c66ac26970a0.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8171.da41f4d3690366fc.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8171.da41f4d3690366fc.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8283.f41216fedc310fb2.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8283.f41216fedc310fb2.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8331.c05961d3317723f8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8331.c05961d3317723f8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8393.4276c63baa000f93.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8393.4276c63baa000f93.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8512.04a122c7abe09f85.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8512.04a122c7abe09f85.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8561.e0ae2c126e26850c.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8561.e0ae2c126e26850c.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/85b6cb10.3db11306353dd6b4.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/85b6cb10.3db11306353dd6b4.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8678.80cf7703c175b81a.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8678.80cf7703c175b81a.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/870.c1277ad0599a1203.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/870.c1277ad0599a1203.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8724.c7b83652d073185b.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8724.c7b83652d073185b.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8770.44d2f8c73be18acf.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8770.44d2f8c73be18acf.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8825.95fe69ef240ad226.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8825.95fe69ef240ad226.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/889.4a330cc153172197.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/889.4a330cc153172197.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8910.ec6846732bff95bc.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8910.ec6846732bff95bc.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/8915.056c1402f901ae7d.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/8915.056c1402f901ae7d.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9071.fc8362f20765bef4.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9071.fc8362f20765bef4.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9121.9917041a899b93b8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9121.9917041a899b93b8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9230.d131be9aadfc6a17.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9230.d131be9aadfc6a17.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9232.61d440e4c3b2b427.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9232.61d440e4c3b2b427.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9277.a16c07843c073298.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9277.a16c07843c073298.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9296.4f23080e808bc92e.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9296.4f23080e808bc92e.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9558.9bf5494ebdf03040.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9558.9bf5494ebdf03040.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9607.c428674d5c072f92.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9607.c428674d5c072f92.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9713.f1d5b41171c6487d.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9713.f1d5b41171c6487d.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9781.7a6517b3f4614b45.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9781.7a6517b3f4614b45.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9826.cf4131d537c8ed72.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9826.cf4131d537c8ed72.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9831.296c1ea16c1953c3.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9831.296c1ea16c1953c3.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/9972.fd259588474eb11b.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/9972.fd259588474eb11b.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/ab5c09eb-707dbcabaaeae5ad.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/ab5c09eb-707dbcabaaeae5ad.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/ac0f5318.05716e5c42c8263f.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/ac0f5318.05716e5c42c8263f.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/b1bb7d45-c13bcc9c04a6e2b5.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/b1bb7d45-c13bcc9c04a6e2b5.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/b637e9a5.5e5cb870404af256.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/b637e9a5.5e5cb870404af256.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/bd65aaa0.fe3593ec9d17d461.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/bd65aaa0.fe3593ec9d17d461.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/main-3ced503a3320a6c1.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/main-3ced503a3320a6c1.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/main-app-59a34855dfcb93b1.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/main-app-59a34855dfcb93b1.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/pages/_app-949612246a7b1393.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/pages/_app-949612246a7b1393.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/pages/index-84f6f8c197ff4895.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/pages/index-84f6f8c197ff4895.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/chunks/webpack-82c067397cfcc59a.js` & `transpector-0.1.1/transpector/frontend_dist/_next/static/chunks/webpack-82c067397cfcc59a.js`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/css/45eccb5d7dcc0d8c.css` & `transpector-0.1.1/transpector/frontend_dist/_next/static/css/45eccb5d7dcc0d8c.css`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/css/88da4da6c702ca4f.css` & `transpector-0.1.1/transpector/frontend_dist/_next/static/css/88da4da6c702ca4f.css`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/css/9b22a190adf5cd66.css` & `transpector-0.1.1/transpector/frontend_dist/_next/static/css/9b22a190adf5cd66.css`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/add-above.ee286b1c.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/add-above.ee286b1c.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/add-below.bcf3422e.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/add-below.bcf3422e.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/bell.bccaf100.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/bell.bccaf100.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/bug-dot.326bc45a.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/bug-dot.326bc45a.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/bug.e30064ad.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/bug.e30064ad.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/build.e3fdf668.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/build.e3fdf668.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/case-sensitive.eaefe455.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/case-sensitive.eaefe455.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/copyright.f38f4ec0.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/copyright.f38f4ec0.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/cut.18edde39.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/cut.18edde39.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/duplicate.8815451e.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/duplicate.8815451e.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.0e53fe4f.woff` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.0e53fe4f.woff`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.7edea186.woff2` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.7edea186.woff2`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.9c02eaf6.ttf` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.9c02eaf6.ttf`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.a76d53bf.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.a76d53bf.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-brands-400.b2970adc.eot` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-brands-400.b2970adc.eot`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.04dd5282.woff` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.04dd5282.woff`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.7346017c.ttf` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.7346017c.ttf`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.a0140e7c.eot` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.a0140e7c.eot`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.e2b3a9dc.woff2` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.e2b3a9dc.woff2`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-regular-400.ee37fbcc.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-regular-400.ee37fbcc.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.620019ed.woff2` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.620019ed.woff2`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.974801a4.eot` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.974801a4.eot`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.cd7322bf.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.cd7322bf.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.d5b0a356.ttf` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.d5b0a356.ttf`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/fa-solid-900.e67670b0.woff` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/fa-solid-900.e67670b0.woff`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/html5.ea435392.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/html5.ea435392.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/info.4d82eb41.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/info.4d82eb41.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/json.a2c296bb.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/json.a2c296bb.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/julia.499ac74e.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/julia.499ac74e.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/jupyter-favicon.b19d8551.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/jupyter-favicon.b19d8551.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/jupyter.a48871a7.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/jupyter.a48871a7.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/jupyterlab-wordmark.6280567a.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/jupyterlab-wordmark.6280567a.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/move-down.5e4a3948.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/move-down.5e4a3948.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/move-up.fa81409d.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/move-up.fa81409d.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/not-trusted.8bc17823.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/not-trusted.8bc17823.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/palette.14c4709b.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/palette.14c4709b.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/pdf.f6a1dc59.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/pdf.f6a1dc59.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/python.0ffed0a2.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/python.0ffed0a2.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/react.c81f1b87.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/react.c81f1b87.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/regex.fa85da44.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/regex.fa85da44.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/settings.454fe53f.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/settings.454fe53f.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/share.ccbe241a.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/share.ccbe241a.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/tag.8887c8e5.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/tag.8887c8e5.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/terminal.0a8eb862.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/terminal.0a8eb862.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/trusted.3ac2122f.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/trusted.3ac2122f.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/users.cba8edb3.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/users.cba8edb3.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/_next/static/media/word.c993422c.svg` & `transpector-0.1.1/transpector/frontend_dist/_next/static/media/word.c993422c.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/favicon.ico` & `transpector-0.1.1/transpector/frontend_dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/index.html` & `transpector-0.1.1/transpector/frontend_dist/index.html`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/next.svg` & `transpector-0.1.1/transpector/frontend_dist/next.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/frontend_dist/vercel.svg` & `transpector-0.1.1/transpector/frontend_dist/vercel.svg`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/jupyter_server_config.py` & `transpector-0.1.1/transpector/jupyter_server_config.py`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/launch.py` & `transpector-0.1.1/transpector/launch.py`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/main.py` & `transpector-0.1.1/transpector/main.py`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/model.py` & `transpector-0.1.1/transpector/model.py`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/model_setup.py` & `transpector-0.1.1/transpector/model_setup.py`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/notebooks/.ipynb_checkpoints/main-checkpoint.ipynb` & `transpector-0.1.1/transpector/notebooks/.ipynb_checkpoints/main-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector/notebooks/main.ipynb` & `transpector-0.1.1/transpector/notebooks/main.ipynb`

 * *Files identical despite different names*

### Comparing `transpector-0.1.0/transpector.egg-info/PKG-INFO` & `transpector-0.1.1/transpector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: transpector
-Version: 0.1.0
+Version: 0.1.1
 Summary: Visually inspect, analyse and debug transformer models. Aimed at reducing cycle times for interpretability research and lowering the barrier to entry.
-Home-page: UNKNOWN
 Author: Rob Kopel
 License: LICENSE
-Platform: UNKNOWN
+Description-Content-Type: text/markdown
 
-# Transpector
+# 🔬 Transpector
 Visually inspect, analyse and debug transformer models. Aimed at reducing cycle times for interpretability research and lowering the barrier to entry.
 ## Getting Started
 
+To use Transpector first install the package `pip install transpector` then you can start it from the command line with `transpector`. Once it's ready, navigate to `http://127.0.0.1:8000/index.html` to get started.
+
+#### Using Transpector
+
+Coming soon!
 ## Developing locally
 
 In it's development setting currently you have to run two parts, a python script kicking off Jupyter Server (this spawns a fastAPI backend in the same event loop as the IPython Kernal), and a Next JS Server. Next JS will be compiled and served as a static file from fastAPI eventually.
 
 To run Next JS
 ```bash
 npm run dev
@@ -39,15 +43,15 @@
 And finally, use our installed package to run the server:
 ```
 transpector run
 ```
 
 ## To Do
 
-### Milestone 2
+#### Milestone 2️⃣
 - [ ] Add ability to split each token into seperate node
 - [ ] Inferencing layer cutoff
 - [ ] Causal tracing
 - [ ] Knowledge editing
 - [ ] Basic Layernorm visuals (what would be useful?)
 - [ ] Text pane batch input
 - [ ] Full dataset input
@@ -61,15 +65,15 @@
 - [ ] Custom model support
 - [ ] Select many nodes and multi-node selection menus
 - [ ] Research replication using transpector
 - [ ] Ability to add notes to activations, weights and nodes
 
 
 
-### Milestone 1
+#### Milestone 1️⃣
 - [ ] Add icons on the edges
 - [ ] Node resizing and rerendering (for canvas nodes)
 - [ ] Weight Analysis: Visualise weights
 - [ ] Weight Analysis: What is the OV circuit trying to copy given a token
 - [ ] Weight Analysis: What is the KQ circuit attention position distribution 
 - [ ] Visual layer folding
 - [ ] Activation freezing
@@ -79,20 +83,21 @@
 - [ ] Optimisation: WebGPU rendering
 - [ ] Optimisation: Remove dead data
 - [ ] Non blocking model updating
 - [ ] KQV composition visualisation
 - [ ] Residual stream analysis visualisation
 - [ ] Notebook scrolling bugs
 - [ ] Improve global state control
-- [ ] Python static hosting
-- [ ] Python package 
-- [ ] Make gifs of features
 - [ ] Compute/ GPU flags/controls from UI
 - [ ] Add correct shortformer positional embedding links
 - [ ] Move to same data structure in py/ js and ws for syncing
+- [ ] Basic usage tutorial
+- [ ] Make gifs of features
+- [ ] Baisc architecture diagram
+- [ ] Pypi package
 - [ ] Add in app credits
 - [ ] Individual activation level ablations
 - [ ] Basic MLP visuals (what would be useful?)
 - [x] Ablations
 - [x] Canvas summed pattern and result rendering
 - [x] Add readme credits
 - [x] Model Outputs
@@ -100,14 +105,16 @@
 - [x] Layernorm nodes
 - [x] Text pane visibility
 - [x] Notebook loading pre existing kernel
 - [x] Upgrade model selection pane
 - [x] Improve typing coverage
 - [x] Next static export
 - [x] Python kickoff script
+- [x] Python static hosting
+- [x] Python package 
 - [x] Model Pane Upgrade
 - [x] Nodes disabled, default and highlighted feature
 - [x] Jupyter-UI upgrade
 - [x] Refactor Nodes and edges code
 - [x] Layernaming bugs
 - [x] Visual spacing optimisation
 - [x] Layer groups
@@ -117,8 +124,7 @@
 - [x] Tokenization node
 - [x] Residual stream node
 - [x] Attention text visualisation
 
 
 ## Credits
 This work has only been possible through the usage of Transformer Lens by Neel Nanda and has been heavily inspired by circuitviz by Alan Cooney
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `transpector-0.1.0/transpector.egg-info/SOURCES.txt` & `transpector-0.1.1/transpector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

