# Comparing `tmp/omemo-dr-0.99.3.tar.gz` & `tmp/omemo-dr-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omemo-dr-0.99.3.tar", last modified: Mon May 22 23:25:27 2023, max compression
+gzip compressed data, was "omemo-dr-1.0.0.tar", last modified: Fri May 26 17:38:18 2023, max compression
```

## Comparing `omemo-dr-0.99.3.tar` & `omemo-dr-1.0.0.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/
--rw-rw-rw-   0 root         (0) root         (0)    35122 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    43030 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1962 2023-05-11 21:04:20.000000 omemo-dr-0.99.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.260476 omemo-dr-0.99.3/curve25519/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.260476 omemo-dr-0.99.3/curve25519/curve/
--rw-rw-rw-   0 root         (0) root         (0)    31932 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/curve25519-donna.c
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/curve25519-donna.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.276477 omemo-dr-0.99.3/curve25519/curve/ed25519/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.280478 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/compare.c
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/compare.h
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/convert.c
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/crypto_additions.h
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/crypto_hash_sha512.h
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.c
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.h
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ed_sigs.c
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ed_sigs.h
--rw-rw-rw-   0 root         (0) root         (0)     2236 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/elligator.c
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_edy_to_montx.c
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_isequal.c
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_isreduced.c
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_mont_rhs.c
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_montx_to_edy.c
--rw-rw-rw-   0 root         (0) root         (0)     1355 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_sqrt.c
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_isneutral.c
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_montx_to_p3.c
--rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_neg.c
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_p3_to_montx.c
--rw-rw-rw-   0 root         (0) root         (0)     3141 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_scalarmult.c
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_scalarmult_cofactor.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_constants.h
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_crypto_additions.h
--rw-rw-rw-   0 root         (0) root         (0)     2660 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h
--rw-rw-rw-   0 root         (0) root         (0)     1034 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_labelset.h
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h
--rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_x.h
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/keygen.c
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/keygen.h
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/open_modified.c
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_clamp.c
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_cmov.c
--rw-rw-rw-   0 root         (0) root         (0)      996 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_neg.c
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sign_modified.c
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/utility.c
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/utility.h
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.c
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.h
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/zeroize.c
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/additions/zeroize.h
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/api.h
--rw-rw-rw-   0 root         (0) root         (0)    76457 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/base.h
--rw-rw-rw-   0 root         (0) root         (0)     2388 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/base2.h
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/d.h
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/d2.h
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe.h
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_0.c
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_1.c
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_add.c
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_cmov.c
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_copy.c
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_frombytes.c
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_invert.c
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_isnegative.c
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_isnonzero.c
--rw-rw-rw-   0 root         (0) root         (0)    10744 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_mul.c
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_neg.c
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_pow22523.c
--rw-rw-rw-   0 root         (0) root         (0)     5980 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq.c
--rw-rw-rw-   0 root         (0) root         (0)     6106 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq2.c
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sub.c
--rw-rw-rw-   0 root         (0) root         (0)     3189 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/fe_tobytes.c
--rw-rw-rw-   0 root         (0) root         (0)     2869 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge.h
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_add.c
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_add.h
--rw-rw-rw-   0 root         (0) root         (0)     2371 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_double_scalarmult.c
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_frombytes.c
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_madd.c
--rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_madd.h
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_msub.c
--rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_msub.h
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p1p1_to_p2.c
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p1p1_to_p3.c
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_0.c
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_dbl.c
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_dbl.h
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_0.c
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_dbl.c
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_to_cached.c
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_to_p2.c
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p3_tobytes.c
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_precomp_0.c
--rw-rw-rw-   0 root         (0) root         (0)     2477 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_scalarmult_base.c
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_sub.c
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_sub.h
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/ge_tobytes.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_int32.h
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_int64.h
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign.h
--rw-rw-rw-   0 root         (0) root         (0)     2034 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_uint32.h
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_uint64.h
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/
--rw-rw-rw-   0 root         (0) root         (0)     6416 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/blocks.c
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/hash.c
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/open.c
--rw-rw-rw-   0 root         (0) root         (0)     5518 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/pow22523.h
--rw-rw-rw-   0 root         (0) root         (0)     5527 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/pow225521.h
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sc.h
--rw-rw-rw-   0 root         (0) root         (0)    12494 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sc_muladd.c
--rw-rw-rw-   0 root         (0) root         (0)     8139 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sc_reduce.c
--rw-rw-rw-   0 root         (0) root         (0)      817 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sign.c
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/sqrtm1.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.284478 omemo-dr-0.99.3/curve25519/curve/ed25519/tests/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_fast_tests.h
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_slow_tests.h
--rw-rw-rw-   0 root         (0) root         (0)     8040 2023-04-09 19:22:07.000000 omemo-dr-0.99.3/curve25519/curve25519module.c
--rw-rw-rw-   0 root         (0) root         (0)     4973 2023-05-18 19:49:38.000000 omemo-dr-0.99.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-03-26 20:37:13.000000 omemo-dr-0.99.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.260476 omemo-dr-0.99.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr/
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-22 23:23:19.000000 omemo-dr-0.99.3/src/omemo_dr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2254 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/aes.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-20 17:36:45.000000 omemo-dr-0.99.3/src/omemo_dr/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr/curve/
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/curve/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr/ecc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/curve.py
--rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/djbec.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-08 20:42:25.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/ec.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ecc/eckeypair.py
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-20 18:34:28.000000 omemo-dr-0.99.3/src/omemo_dr/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/identitykey.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/identitykeypair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/kdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/derivedmessagesecrets.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/derivedrootsecrets.py
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/hkdf.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/kdf/messagekeys.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-07 15:19:42.000000 omemo-dr-0.99.3/src/omemo_dr/observable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/protocol/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/ciphertextmessage.py
--rw-rw-rw-   0 root         (0) root         (0)     4076 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_keyexchange.py
--rw-rw-rw-   0 root         (0) root         (0)     5152 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5046 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/prekeywhispermessage.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/whisper_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4943 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/protocol/whispermessage.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/ratchet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/aliceparameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/bobparameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/chainkey.py
--rw-rw-rw-   0 root         (0) root         (0)     5271 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/ratchetingsession.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-05-06 21:36:18.000000 omemo-dr-0.99.3/src/omemo_dr/ratchet/rootkey.py
--rw-rw-rw-   0 root         (0) root         (0)    19094 2023-05-20 17:44:31.000000 omemo-dr-0.99.3/src/omemo_dr/session_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5487 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/sessionbuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10889 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/sessioncipher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.292479 omemo-dr-0.99.3/src/omemo_dr/state/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/state/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3196 2023-05-20 18:34:28.000000 omemo-dr-0.99.3/src/omemo_dr/state/prekeybundle.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/prekeyrecord.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/sessionrecord.py
--rw-rw-rw-   0 root         (0) root         (0)    12879 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/sessionstate.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/signedprekeyrecord.py
--rw-rw-rw-   0 root         (0) root         (0)     5950 2023-05-11 19:26:44.000000 omemo-dr-0.99.3/src/omemo_dr/state/storage_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4690 2023-05-20 17:44:31.000000 omemo-dr-0.99.3/src/omemo_dr/state/store.py
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/structs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/src/omemo_dr/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/src/omemo_dr/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/src/omemo_dr/util/byteutil.py
--rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-20 17:44:31.000000 omemo-dr-0.99.3/src/omemo_dr/util/keyhelper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-07 18:48:15.000000 omemo-dr-0.99.3/src/omemo_dr/util/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.288478 omemo-dr-0.99.3/src/omemo_dr.egg-info/
--rw-r--r--   0 root         (0) root         (0)    43030 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6842 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-22 23:25:27.000000 omemo-dr-0.99.3/src/omemo_dr.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-05-18 19:27:25.000000 omemo-dr-0.99.3/tests/inmemoryidentitykeystore.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/inmemoryprekeystore.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/inmemorysessionstore.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/inmemorysignedprekeystore.py
--rw-rw-rw-   0 root         (0) root         (0)     3512 2023-05-06 21:18:55.000000 omemo-dr-0.99.3/tests/inmemorystore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/tests/kdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/tests/kdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/tests/kdf/test_hkdf.py
--rw-rw-rw-   0 root         (0) root         (0)    10416 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/tests/test_sessionbuilder.py
--rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-11 18:26:34.000000 omemo-dr-0.99.3/tests/test_sessioncipher.py
--rw-rw-rw-   0 root         (0) root         (0)     9315 2023-05-10 21:35:36.000000 omemo-dr-0.99.3/tests/test_sigs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 23:25:27.296479 omemo-dr-0.99.3/tests/util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-0.99.3/tests/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-03 19:53:25.000000 omemo-dr-0.99.3/tests/util/test_byteutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.932634 omemo-dr-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35122 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    43029 2023-05-26 17:38:18.928634 omemo-dr-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1962 2023-05-11 21:04:20.000000 omemo-dr-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.904631 omemo-dr-1.0.0/curve25519/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.904631 omemo-dr-1.0.0/curve25519/curve/
+-rw-rw-rw-   0 root         (0) root         (0)    31932 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/curve25519-donna.c
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/curve25519-donna.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.912632 omemo-dr-1.0.0/curve25519/curve/ed25519/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.916632 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/compare.c
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/compare.h
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/convert.c
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/crypto_additions.h
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/crypto_hash_sha512.h
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/curve_sigs.c
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/curve_sigs.h
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ed_sigs.c
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ed_sigs.h
+-rw-rw-rw-   0 root         (0) root         (0)     2236 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/elligator.c
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/fe_edy_to_montx.c
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/fe_isequal.c
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/fe_isreduced.c
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/fe_mont_rhs.c
+-rw-rw-rw-   0 root         (0) root         (0)      319 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/fe_montx_to_edy.c
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/fe_sqrt.c
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_isneutral.c
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_montx_to_p3.c
+-rw-rw-rw-   0 root         (0) root         (0)      201 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_p3_to_montx.c
+-rw-rw-rw-   0 root         (0) root         (0)     3141 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_scalarmult.c
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_scalarmult_cofactor.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.916632 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_constants.h
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_crypto_additions.h
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_labelset.h
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_x.h
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/keygen.c
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/keygen.h
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/open_modified.c
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/sc_clamp.c
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/sc_cmov.c
+-rw-rw-rw-   0 root         (0) root         (0)      996 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/sc_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/sign_modified.c
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/utility.c
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/utility.h
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/xeddsa.c
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/xeddsa.h
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/zeroize.c
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/additions/zeroize.h
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/api.h
+-rw-rw-rw-   0 root         (0) root         (0)    76457 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/base.h
+-rw-rw-rw-   0 root         (0) root         (0)     2388 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/base2.h
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/d.h
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/d2.h
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe.h
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_1.c
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_add.c
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_cmov.c
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_copy.c
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_frombytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_invert.c
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_isnegative.c
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_isnonzero.c
+-rw-rw-rw-   0 root         (0) root         (0)    10744 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_mul.c
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_neg.c
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_pow22523.c
+-rw-rw-rw-   0 root         (0) root         (0)     5980 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_sq.c
+-rw-rw-rw-   0 root         (0) root         (0)     6106 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_sq2.c
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_sub.c
+-rw-rw-rw-   0 root         (0) root         (0)     3189 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/fe_tobytes.c
+-rw-rw-rw-   0 root         (0) root         (0)     2869 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge.h
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_add.c
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_add.h
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_double_scalarmult.c
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_frombytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_madd.c
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_madd.h
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_msub.c
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_msub.h
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p1p1_to_p2.c
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p1p1_to_p3.c
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p2_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p2_dbl.c
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p2_dbl.h
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p3_0.c
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p3_dbl.c
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p3_to_cached.c
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p3_to_p2.c
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p3_tobytes.c
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_precomp_0.c
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_scalarmult_base.c
+-rw-rw-rw-   0 root         (0) root         (0)      125 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_sub.c
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_sub.h
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/ge_tobytes.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.920633 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_int32.h
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_int64.h
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_sign.h
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_uint32.h
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_uint64.h
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.920633 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_sha512/
+-rw-rw-rw-   0 root         (0) root         (0)     6416 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_sha512/blocks.c
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_sha512/hash.c
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/open.c
+-rw-rw-rw-   0 root         (0) root         (0)     5518 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/pow22523.h
+-rw-rw-rw-   0 root         (0) root         (0)     5527 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/pow225521.h
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/sc.h
+-rw-rw-rw-   0 root         (0) root         (0)    12494 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/sc_muladd.c
+-rw-rw-rw-   0 root         (0) root         (0)     8139 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/sc_reduce.c
+-rw-rw-rw-   0 root         (0) root         (0)      817 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/sign.c
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/sqrtm1.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.920633 omemo-dr-1.0.0/curve25519/curve/ed25519/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/tests/internal_fast_tests.h
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/curve25519/curve/ed25519/tests/internal_slow_tests.h
+-rw-rw-rw-   0 root         (0) root         (0)     8040 2023-04-09 19:22:07.000000 omemo-dr-1.0.0/curve25519/curve25519module.c
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-05-26 17:36:26.000000 omemo-dr-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 17:38:18.932634 omemo-dr-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-03-26 20:37:13.000000 omemo-dr-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.900631 omemo-dr-1.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.920633 omemo-dr-1.0.0/src/omemo_dr/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-26 17:36:26.000000 omemo-dr-1.0.0/src/omemo_dr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/src/omemo_dr/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-05-20 17:36:45.000000 omemo-dr-1.0.0/src/omemo_dr/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.924633 omemo-dr-1.0.0/src/omemo_dr/curve/
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/src/omemo_dr/curve/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.924633 omemo-dr-1.0.0/src/omemo_dr/ecc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/src/omemo_dr/ecc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/ecc/curve.py
+-rw-rw-rw-   0 root         (0) root         (0)     2713 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/ecc/djbec.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-08 20:42:25.000000 omemo-dr-1.0.0/src/omemo_dr/ecc/ec.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/ecc/eckeypair.py
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-05-20 18:34:28.000000 omemo-dr-1.0.0/src/omemo_dr/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/identitykey.py
+-rw-rw-rw-   0 root         (0) root         (0)     1556 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/identitykeypair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.924633 omemo-dr-1.0.0/src/omemo_dr/kdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/src/omemo_dr/kdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/src/omemo_dr/kdf/derivedmessagesecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/src/omemo_dr/kdf/derivedrootsecrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2023-05-11 18:26:34.000000 omemo-dr-1.0.0/src/omemo_dr/kdf/hkdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/src/omemo_dr/kdf/messagekeys.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-05-07 15:19:42.000000 omemo-dr-1.0.0/src/omemo_dr/observable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.924633 omemo-dr-1.0.0/src/omemo_dr/protocol/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/ciphertextmessage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/omemo_keyexchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     5152 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/omemo_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/omemo_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/prekeywhispermessage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/whisper_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4943 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/protocol/whispermessage.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/src/omemo_dr/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.924633 omemo-dr-1.0.0/src/omemo_dr/ratchet/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/src/omemo_dr/ratchet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/ratchet/aliceparameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-11 18:26:34.000000 omemo-dr-1.0.0/src/omemo_dr/ratchet/bobparameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/ratchet/chainkey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2023-05-11 18:26:34.000000 omemo-dr-1.0.0/src/omemo_dr/ratchet/ratchetingsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-05-06 21:36:18.000000 omemo-dr-1.0.0/src/omemo_dr/ratchet/rootkey.py
+-rw-rw-rw-   0 root         (0) root         (0)    19094 2023-05-20 17:44:31.000000 omemo-dr-1.0.0/src/omemo_dr/session_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5487 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/sessionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10889 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/sessioncipher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.928634 omemo-dr-1.0.0/src/omemo_dr/state/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/src/omemo_dr/state/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2023-05-20 18:34:28.000000 omemo-dr-1.0.0/src/omemo_dr/state/prekeybundle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/state/prekeyrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/state/sessionrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)    12879 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/state/sessionstate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/state/signedprekeyrecord.py
+-rw-rw-rw-   0 root         (0) root         (0)     5950 2023-05-11 19:26:44.000000 omemo-dr-1.0.0/src/omemo_dr/state/storage_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4690 2023-05-20 17:44:31.000000 omemo-dr-1.0.0/src/omemo_dr/state/store.py
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/structs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.928634 omemo-dr-1.0.0/src/omemo_dr/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/src/omemo_dr/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1333 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/src/omemo_dr/util/byteutil.py
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2023-05-20 17:44:31.000000 omemo-dr-1.0.0/src/omemo_dr/util/keyhelper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-05-07 18:48:15.000000 omemo-dr-1.0.0/src/omemo_dr/util/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.920633 omemo-dr-1.0.0/src/omemo_dr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    43029 2023-05-26 17:38:18.000000 omemo-dr-1.0.0/src/omemo_dr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6842 2023-05-26 17:38:18.000000 omemo-dr-1.0.0/src/omemo_dr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 17:38:18.000000 omemo-dr-1.0.0/src/omemo_dr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-26 17:38:18.000000 omemo-dr-1.0.0/src/omemo_dr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-26 17:38:18.000000 omemo-dr-1.0.0/src/omemo_dr.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.928634 omemo-dr-1.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2023-05-18 19:27:25.000000 omemo-dr-1.0.0/tests/inmemoryidentitykeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/tests/inmemoryprekeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/tests/inmemorysessionstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/tests/inmemorysignedprekeystore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3512 2023-05-06 21:18:55.000000 omemo-dr-1.0.0/tests/inmemorystore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.928634 omemo-dr-1.0.0/tests/kdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/tests/kdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-05-11 18:26:34.000000 omemo-dr-1.0.0/tests/kdf/test_hkdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    10416 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/tests/test_sessionbuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-11 18:26:34.000000 omemo-dr-1.0.0/tests/test_sessioncipher.py
+-rw-rw-rw-   0 root         (0) root         (0)     9315 2023-05-10 21:35:36.000000 omemo-dr-1.0.0/tests/test_sigs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:38:18.928634 omemo-dr-1.0.0/tests/util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-26 17:49:30.000000 omemo-dr-1.0.0/tests/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-05-03 19:53:25.000000 omemo-dr-1.0.0/tests/util/test_byteutil.py
```

### Comparing `omemo-dr-0.99.3/LICENSE` & `omemo-dr-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/PKG-INFO` & `omemo-dr-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omemo-dr
-Version: 0.99.3
+Version: 1.0.0
 Summary: OMEMO Double Ratchet
 Author: Philipp Hörist
 Author-email: philipp@hoerist.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `omemo-dr-0.99.3/README.md` & `omemo-dr-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/curve25519-donna.c` & `omemo-dr-1.0.0/curve25519/curve/curve25519-donna.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/compare.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/compare.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/convert.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/convert.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/crypto_additions.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/crypto_additions.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/curve_sigs.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/curve_sigs.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/curve_sigs.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ed_sigs.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ed_sigs.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/elligator.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/elligator.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/fe_sqrt.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/fe_sqrt.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_montx_to_p3.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_montx_to_p3.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/ge_scalarmult.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/ge_scalarmult.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_eddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_labelset.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_labelset.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_veddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/generalized/gen_x.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/generalized/gen_x.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/keygen.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/keygen.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/open_modified.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/open_modified.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sc_neg.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/sc_neg.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/sign_modified.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/sign_modified.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/utility.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/utility.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/xeddsa.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/additions/xeddsa.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/additions/xeddsa.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/base.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/base.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/base2.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/base2.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_add.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_add.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_cmov.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_cmov.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_frombytes.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_frombytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_mul.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_mul.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_neg.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_neg.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_sq.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sq2.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_sq2.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_sub.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_sub.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/fe_tobytes.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/fe_tobytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_add.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_add.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_double_scalarmult.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_double_scalarmult.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_frombytes.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_frombytes.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_madd.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_madd.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_msub.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_msub.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_p2_dbl.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_p2_dbl.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_scalarmult_base.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_scalarmult_base.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/ge_sub.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/ge_sub.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_sign.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_sign_edwards25519sha512batch.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_includes/crypto_verify_32.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/blocks.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_sha512/blocks.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/nacl_sha512/hash.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/nacl_sha512/hash.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/open.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/open.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/pow22523.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/pow22523.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/pow225521.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/pow225521.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/sc_muladd.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/sc_muladd.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/sc_reduce.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/sc_reduce.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/sign.c` & `omemo-dr-1.0.0/curve25519/curve/ed25519/sign.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_fast_tests.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/tests/internal_fast_tests.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve/ed25519/tests/internal_slow_tests.h` & `omemo-dr-1.0.0/curve25519/curve/ed25519/tests/internal_slow_tests.h`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/curve25519/curve25519module.c` & `omemo-dr-1.0.0/curve25519/curve25519module.c`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/pyproject.toml` & `omemo-dr-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "cryptography",
   "protobuf>=4.21.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-  "ruff>=0.0.254",
+  "ruff>=0.0.267",
   "codespell[toml]>=2.2.4",
   "black>=23.1.0"
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "omemo_dr.__version__"}
```

### Comparing `omemo-dr-0.99.3/setup.py` & `omemo-dr-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/aes.py` & `omemo-dr-1.0.0/src/omemo_dr/aes.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/curve/__init__.py` & `omemo-dr-1.0.0/src/omemo_dr/curve/__init__.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/ecc/curve.py` & `omemo-dr-1.0.0/src/omemo_dr/ecc/curve.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/ecc/djbec.py` & `omemo-dr-1.0.0/src/omemo_dr/ecc/djbec.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/exceptions.py` & `omemo-dr-1.0.0/src/omemo_dr/exceptions.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/identitykey.py` & `omemo-dr-1.0.0/src/omemo_dr/identitykey.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/identitykeypair.py` & `omemo-dr-1.0.0/src/omemo_dr/identitykeypair.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/kdf/derivedmessagesecrets.py` & `omemo-dr-1.0.0/src/omemo_dr/kdf/derivedmessagesecrets.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/kdf/hkdf.py` & `omemo-dr-1.0.0/src/omemo_dr/kdf/hkdf.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/observable.py` & `omemo-dr-1.0.0/src/omemo_dr/observable.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_keyexchange.py` & `omemo-dr-1.0.0/src/omemo_dr/protocol/omemo_keyexchange.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_message.py` & `omemo-dr-1.0.0/src/omemo_dr/protocol/omemo_message.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/protocol/omemo_pb2.py` & `omemo-dr-1.0.0/src/omemo_dr/protocol/omemo_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/protocol/prekeywhispermessage.py` & `omemo-dr-1.0.0/src/omemo_dr/protocol/prekeywhispermessage.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/protocol/whisper_pb2.py` & `omemo-dr-1.0.0/src/omemo_dr/protocol/whisper_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/protocol/whispermessage.py` & `omemo-dr-1.0.0/src/omemo_dr/protocol/whispermessage.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/ratchet/aliceparameters.py` & `omemo-dr-1.0.0/src/omemo_dr/ratchet/aliceparameters.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/ratchet/bobparameters.py` & `omemo-dr-1.0.0/src/omemo_dr/ratchet/bobparameters.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/ratchet/chainkey.py` & `omemo-dr-1.0.0/src/omemo_dr/ratchet/chainkey.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/ratchet/ratchetingsession.py` & `omemo-dr-1.0.0/src/omemo_dr/ratchet/ratchetingsession.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/ratchet/rootkey.py` & `omemo-dr-1.0.0/src/omemo_dr/ratchet/rootkey.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/session_manager.py` & `omemo-dr-1.0.0/src/omemo_dr/session_manager.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/sessionbuilder.py` & `omemo-dr-1.0.0/src/omemo_dr/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/sessioncipher.py` & `omemo-dr-1.0.0/src/omemo_dr/sessioncipher.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/state/prekeybundle.py` & `omemo-dr-1.0.0/src/omemo_dr/state/prekeybundle.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/state/prekeyrecord.py` & `omemo-dr-1.0.0/src/omemo_dr/state/prekeyrecord.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/state/sessionrecord.py` & `omemo-dr-1.0.0/src/omemo_dr/state/sessionrecord.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/state/sessionstate.py` & `omemo-dr-1.0.0/src/omemo_dr/state/sessionstate.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/state/signedprekeyrecord.py` & `omemo-dr-1.0.0/src/omemo_dr/state/signedprekeyrecord.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/state/storage_pb2.py` & `omemo-dr-1.0.0/src/omemo_dr/state/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/state/store.py` & `omemo-dr-1.0.0/src/omemo_dr/state/store.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/structs.py` & `omemo-dr-1.0.0/src/omemo_dr/structs.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/util/byteutil.py` & `omemo-dr-1.0.0/src/omemo_dr/util/byteutil.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr/util/keyhelper.py` & `omemo-dr-1.0.0/src/omemo_dr/util/keyhelper.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/src/omemo_dr.egg-info/PKG-INFO` & `omemo-dr-1.0.0/src/omemo_dr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omemo-dr
-Version: 0.99.3
+Version: 1.0.0
 Summary: OMEMO Double Ratchet
 Author: Philipp Hörist
 Author-email: philipp@hoerist.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `omemo-dr-0.99.3/src/omemo_dr.egg-info/SOURCES.txt` & `omemo-dr-1.0.0/src/omemo_dr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/inmemoryidentitykeystore.py` & `omemo-dr-1.0.0/tests/inmemoryidentitykeystore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/inmemoryprekeystore.py` & `omemo-dr-1.0.0/tests/inmemoryprekeystore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/inmemorysessionstore.py` & `omemo-dr-1.0.0/tests/inmemorysessionstore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/inmemorysignedprekeystore.py` & `omemo-dr-1.0.0/tests/inmemorysignedprekeystore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/inmemorystore.py` & `omemo-dr-1.0.0/tests/inmemorystore.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/kdf/test_hkdf.py` & `omemo-dr-1.0.0/tests/kdf/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/test_sessionbuilder.py` & `omemo-dr-1.0.0/tests/test_sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/test_sessioncipher.py` & `omemo-dr-1.0.0/tests/test_sessioncipher.py`

 * *Files identical despite different names*

### Comparing `omemo-dr-0.99.3/tests/test_sigs.py` & `omemo-dr-1.0.0/tests/test_sigs.py`

 * *Files identical despite different names*

