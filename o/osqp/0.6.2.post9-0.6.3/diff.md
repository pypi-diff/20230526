# Comparing `tmp/osqp-0.6.2.post9.tar.gz` & `tmp/osqp-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osqp-0.6.2.post9.tar", last modified: Fri Apr 14 21:06:18 2023, max compression
+gzip compressed data, was "osqp-0.6.3.tar", last modified: Fri May 26 00:58:44 2023, max compression
```

## Comparing `osqp-0.6.2.post9.tar` & `osqp-0.6.3.tar`

### file list

```diff
@@ -1,230 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.385226 osqp-0.6.2.post9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.github/workflows/build_aarch64.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/osqp_sources/
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/osqp_sources/configure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/configure/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/FindPythonModule.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/FindR.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/osqp_configure.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/include/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/auxil.h
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/cs.h
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/ctrlc.h
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/glob_opts.h
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/kkt.h
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/lin_alg.h
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/lin_sys.h
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/osqp.h
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/polish.h
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/proj.h
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c
--rw-r--r--   0 runner    (1001) docker     (123)    64841 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c
--rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.git
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.401227 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/minunit.h
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_identity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_rank_deficient.h
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_singleton.h
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_sym_structure.h
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_tril_structure.h
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_two_by_two.h
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.c
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.401227 osqp-0.6.2.post9/osqp_sources/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31823 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/auxil.c
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/cs.c
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/ctrlc.c
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/error.c
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/kkt.c
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/lin_alg.c
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/lin_sys.c
--rw-r--r--   0 runner    (1001) docker     (123)    47667 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/osqp.c
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/polish.c
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/proj.c
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/scaling.c
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/util.c
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/src/extension/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.401227 osqp-0.6.2.post9/src/extension/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpinfopy.h
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpmodulemethods.h
--rw-r--r--   0 runner    (1001) docker     (123)    41043 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpobjectpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpresultspy.h
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqputilspy.h
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpworkspacepy.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/extension/src/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/src/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/src/osqpmodule.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/code_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/emosqpmodule.c
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/example.c
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/src/osqp/codegen/sources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/codegen/sources/configure/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/configure/osqp_configure.h.in
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/configure/qdldl_types.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.409227 osqp-0.6.2.post9/src/osqp/codegen/sources/include/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/auxil.h
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/error.h
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/glob_opts.h
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/kkt.h
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/lin_alg.h
--rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/osqp.h
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/proj.h
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl_interface.h
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/types.h
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.409227 osqp-0.6.2.post9/src/osqp/codegen/sources/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31823 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/auxil.c
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/error.c
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/kkt.c
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/lin_alg.c
--rw-r--r--   0 runner    (1001) docker     (123)    47667 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/osqp.c
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/proj.c
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl.c
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl_interface.c
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/scaling.c
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/util.c
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/src/osqp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/basic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/codegen_matrices_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/codegen_vectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/derivative_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/dual_infeasibility_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/feasibility_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/mkl_pardiso_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/multithread_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/non_convex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/polishing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/primal_infeasibility_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/src/osqp/tests/solutions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_basic_QP.npz
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_feasibility_problem.npz
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_random.npz
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_simple.npz
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_unconstrained.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_solve.npz
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_unconstrained_problem.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A_allind.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_allind.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indA.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_allind.npz
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_bounds.npz
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_l.npz
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_q.npz
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_u.npz
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/unconstrained_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/update_matrices_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/warm_start_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/src/osqppurepy/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqppurepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63336 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqppurepy/_osqp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqppurepy/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.525247 osqp-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.497246 osqp-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.501247 osqp-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-26 00:46:02.000000 osqp-0.6.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-26 00:46:02.000000 osqp-0.6.3/.github/workflows/build_aarch64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-26 00:46:02.000000 osqp-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 00:46:02.000000 osqp-0.6.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 00:46:02.000000 osqp-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-26 00:46:02.000000 osqp-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-26 00:58:44.525247 osqp-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-26 00:46:02.000000 osqp-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.501247 osqp-0.6.3/osqp_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.501247 osqp-0.6.3/osqp_sources/configure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.501247 osqp-0.6.3/osqp_sources/configure/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/configure/cmake/FindPythonModule.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/configure/cmake/FindR.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/configure/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/configure/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/configure/osqp_configure.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/configure/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.505246 osqp-0.6.3/osqp_sources/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/auxil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/cs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/ctrlc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/glob_opts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/kkt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/lin_alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/lin_sys.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/osqp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/polish.h
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/proj.h
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/util.h
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/include/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.505246 osqp-0.6.3/osqp_sources/lin_sys/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.505246 osqp-0.6.3/osqp_sources/lin_sys/direct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.505246 osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.505246 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.505246 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.505246 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c
+-rw-r--r--   0 runner    (1001) docker     (123)    64841 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.509247 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/minunit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_rank_deficient.h
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_singleton.h
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_sym_structure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_tril_structure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_two_by_two.h
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 00:46:05.000000 osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/lib_handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/lin_sys/lib_handler.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.513247 osqp-0.6.3/osqp_sources/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31805 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/auxil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/cs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/ctrlc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/error.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/kkt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/lin_alg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/lin_sys.c
+-rw-r--r--   0 runner    (1001) docker     (123)    48336 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/osqp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/polish.c
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/proj.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/scaling.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-26 00:46:03.000000 osqp-0.6.3/osqp_sources/src/util.c
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-26 00:46:02.000000 osqp-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 00:46:02.000000 osqp-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:58:44.525247 osqp-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-05-26 00:46:02.000000 osqp-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.501247 osqp-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.497246 osqp-0.6.3/src/extension/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.513247 osqp-0.6.3/src/extension/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/include/osqpinfopy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/include/osqpmodulemethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41043 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/include/osqpobjectpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/include/osqpresultspy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/include/osqputilspy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/include/osqpworkspacepy.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.513247 osqp-0.6.3/src/extension/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/src/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-26 00:46:02.000000 osqp-0.6.3/src/extension/src/osqpmodule.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.513247 osqp-0.6.3/src/osqp/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.513247 osqp-0.6.3/src/osqp/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/code_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.517247 osqp-0.6.3/src/osqp/codegen/files_to_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/files_to_generate/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/files_to_generate/emosqpmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/files_to_generate/example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/files_to_generate/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.501247 osqp-0.6.3/src/osqp/codegen/sources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.517247 osqp-0.6.3/src/osqp/codegen/sources/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/configure/osqp_configure.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/configure/qdldl_types.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.517247 osqp-0.6.3/src/osqp/codegen/sources/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/auxil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/glob_opts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/kkt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/lin_alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/osqp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/proj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/qdldl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/qdldl_interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/util.h
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/include/version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.517247 osqp-0.6.3/src/osqp/codegen/sources/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31805 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/auxil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/error.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/kkt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/lin_alg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    48336 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/osqp.c
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/proj.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/qdldl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/qdldl_interface.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/scaling.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp/codegen/sources/src/util.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/codegen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.521247 osqp-0.6.3/src/osqp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/codegen_matrices_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/codegen_vectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/derivative_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/dual_infeasibility_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/feasibility_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/mkl_pardiso_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/multithread_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/non_convex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/polishing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/primal_infeasibility_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.521247 osqp-0.6.3/src/osqp/tests/solutions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_basic_QP.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_feasibility_problem.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_polish_random.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_polish_simple.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_polish_unconstrained.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_solve.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_unconstrained_problem.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_A.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_A_allind.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_P.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_allind.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_indA.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_indP.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_P_allind.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_bounds.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_l.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_q.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/solutions/test_update_u.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/unconstrained_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/update_matrices_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/tests/warm_start_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.513247 osqp-0.6.3/src/osqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-26 00:58:44.000000 osqp-0.6.3/src/osqp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:58:44.525247 osqp-0.6.3/src/osqppurepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqppurepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63330 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqppurepy/_osqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-26 00:46:02.000000 osqp-0.6.3/src/osqppurepy/interface.py
```

### Comparing `osqp-0.6.2.post9/.github/workflows/build.yml` & `osqp-0.6.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/.github/workflows/build_aarch64.yml` & `osqp-0.6.3/.github/workflows/build_aarch64.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/.gitignore` & `osqp-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/LICENSE` & `osqp-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/PKG-INFO` & `osqp-0.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osqp
-Version: 0.6.2.post9
+Version: 0.6.3
 Summary: OSQP: The Operator Splitting QP Solver
 Home-page: https://osqp.org/
 Author: Bartolomeo Stellato, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
 License-File: LICENSE
```

### Comparing `osqp-0.6.2.post9/README.rst` & `osqp-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Minimum version required
 cmake_minimum_required (VERSION 3.2)
 
 # Project name
 project (osqp)
 
+set(OSQP_VERSION "0.0.0" CACHE STRING "The version number of OSQP")
+if(NOT OSQP_VERSION STREQUAL "0.0.0")
+    configure_file (
+        "${PROJECT_SOURCE_DIR}/configure/version.h.in"
+        "${PROJECT_SOURCE_DIR}/include/version.h"
+    )
+endif()
+
 # Export compile commands
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
 
 # Set the output folder where your program will be created
 set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/out)
 set(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/out)
 
@@ -137,14 +145,15 @@
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)  # -fPIC
 
 
 if (NOT MSVC)
 
     if (COVERAGE)
         set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} --coverage")
+        set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} --coverage")
 	if(FORTRAN)
 		set(CMAKE_FORTRAN_FLAGS "${CMAKE_FORTRAN_FLAGS} --coverage")
 	endif(FORTRAN)
     endif()
 
     if (DEBUG)
         set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -O0 -g")
@@ -407,32 +416,37 @@
         OUTPUT ${codegen_test_headers}
         COMMENT "Generating unittests data files using Python"
     )
 
     # Direct linear solver testing
     include_directories(tests)
     add_executable(osqp_tester
-                ${PROJECT_SOURCE_DIR}/tests/osqp_tester.c
-                ${PROJECT_SOURCE_DIR}/tests/osqp_tester.h
-		${PROJECT_SOURCE_DIR}/tests/minunit.h
-                ${test_headers}
-                ${codegen_test_headers})
-    target_link_libraries (osqp_tester osqpstatic)
+            ${PROJECT_SOURCE_DIR}/tests/osqp_tester.cpp
+            ${PROJECT_SOURCE_DIR}/tests/osqp_tester.h
+            ${test_headers}
+            ${codegen_test_headers}
+            )
+    set_target_properties(osqp_tester
+            PROPERTIES
+                CXX_STANDARD 11
+                CXX_STANDARD_REQUIRED YES
+                CXX_EXTENSIONS NO
+            )
+    target_link_libraries (osqp_tester osqpstatic ${CMAKE_DL_LIBS})
 
     # Add custom memory target
     add_executable(osqp_tester_custom_memory
-                   EXCLUDE_FROM_ALL
-                   ${PROJECT_SOURCE_DIR}/tests/osqp_tester.c
-                   ${PROJECT_SOURCE_DIR}/tests/osqp_tester.h
-	           ${PROJECT_SOURCE_DIR}/tests/minunit.h
-                   ${test_headers}
-                   ${codegen_test_headers}
+            EXCLUDE_FROM_ALL
+            ${PROJECT_SOURCE_DIR}/tests/osqp_tester.cpp
+            ${PROJECT_SOURCE_DIR}/tests/osqp_tester.h
+            ${test_headers}
+            ${codegen_test_headers}
 		   ${PROJECT_SOURCE_DIR}/tests/custom_memory/custom_memory.c
 		   ${PROJECT_SOURCE_DIR}/tests/custom_memory/custom_memory.h
 		)
-    target_link_libraries (osqp_tester_custom_memory osqpstatic)
+    target_link_libraries (osqp_tester_custom_memory osqpstatic ${CMAKE_DL_LIBS})
 
     # Add testing
     include(CTest)
     enable_testing()
     add_test(NAME tester COMMAND $<TARGET_FILE:osqp_tester>)
 endif()
```

### Comparing `osqp-0.6.2.post9/osqp_sources/configure/cmake/FindPythonModule.cmake` & `osqp-0.6.3/osqp_sources/configure/cmake/FindPythonModule.cmake`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/configure/cmake/FindR.cmake` & `osqp-0.6.3/osqp_sources/configure/cmake/FindR.cmake`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/configure/cmake/cmake_uninstall.cmake.in` & `osqp-0.6.3/osqp_sources/configure/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/configure/osqp_configure.h.in` & `osqp-0.6.3/osqp_sources/configure/osqp_configure.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/include/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Add the OSQP headers
 set(
     osqp_headers
+    "${CMAKE_CURRENT_SOURCE_DIR}/version.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/auxil.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/constants.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/error.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/glob_opts.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/lin_alg.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/osqp.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/osqp_configure.h"
```

### Comparing `osqp-0.6.2.post9/osqp_sources/include/auxil.h` & `osqp-0.6.3/osqp_sources/include/auxil.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/constants.h` & `osqp-0.6.3/osqp_sources/include/constants.h`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 extern "C" {
 # endif // ifdef __cplusplus
 
 
 /*******************
 * OSQP Versioning *
 *******************/
-# define OSQP_VERSION ("0.6.2") /* string literals automatically null-terminated
-                                   */
+#include "version.h"
 
 /******************
 * Solver Status  *
 ******************/
 # define OSQP_DUAL_INFEASIBLE_INACCURATE (4)
 # define OSQP_PRIMAL_INFEASIBLE_INACCURATE (3)
 # define OSQP_SOLVED_INACCURATE (2)
@@ -29,15 +28,15 @@
 # define OSQP_NON_CVX (-7)              /* problem non convex */
 # define OSQP_UNSOLVED (-10)            /* Unsolved. Only setup function has been called */
 
 
 /*************************
 * Linear System Solvers *
 *************************/
-enum linsys_solver_type { QDLDL_SOLVER, MKL_PARDISO_SOLVER };
+enum linsys_solver_type { QDLDL_SOLVER, MKL_PARDISO_SOLVER, UNKNOWN_SOLVER=99 };
 extern const char * LINSYS_SOLVER_NAME[];
 
 
 /******************
 * Solver Errors  *
 ******************/
 enum osqp_error_type {
```

### Comparing `osqp-0.6.2.post9/osqp_sources/include/cs.h` & `osqp-0.6.3/osqp_sources/include/cs.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/ctrlc.h` & `osqp-0.6.3/osqp_sources/include/ctrlc.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/error.h` & `osqp-0.6.3/osqp_sources/include/error.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/glob_opts.h` & `osqp-0.6.3/osqp_sources/include/glob_opts.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/kkt.h` & `osqp-0.6.3/osqp_sources/include/kkt.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/lin_alg.h` & `osqp-0.6.3/osqp_sources/include/lin_alg.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/lin_sys.h` & `osqp-0.6.3/osqp_sources/include/lin_sys.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/osqp.h` & `osqp-0.6.3/osqp_sources/include/osqp.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/proj.h` & `osqp-0.6.3/osqp_sources/include/proj.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/scaling.h` & `osqp-0.6.3/osqp_sources/include/scaling.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/types.h` & `osqp-0.6.3/osqp_sources/include/types.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/include/util.h` & `osqp-0.6.3/osqp_sources/include/util.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/lin_sys/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/lin_sys/direct/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
              c_int*,         // iparam
              const c_int*,   //msglvl
              c_float*,       // b
              c_float*,       // x
              c_int*          // error
              );
 c_int mkl_set_interface_layer(c_int);
-c_int mkl_get_max_threads();
+c_int mkl_get_max_threads(void);
 
 // Free LDL Factorization structure
 void free_linsys_solver_pardiso(pardiso_solver *s) {
     if (s) {
 
         // Free pardiso solver using internal function
         s->phase = PARDISO_CLEANUP;
```

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 // Interfaces for Pardiso functions
 typedef void (*pardiso_t)(void**, const c_int*, const c_int*, const c_int*,
                           const c_int*, const c_int*, const c_float*,
                           const c_int*, const c_int*, c_int*,
                           const c_int*, c_int*, const c_int*, c_float*,
                           c_float*, c_int*);
 typedef int (*mkl_set_ifl_t)(int);
-typedef int (*mkl_get_mt_t)();
+typedef int (*mkl_get_mt_t)(void);
 
 
 // Handlers are static variables
 static soHandle_t Pardiso_handle = OSQP_NULL;
 static pardiso_t func_pardiso = OSQP_NULL;
 static mkl_set_ifl_t func_mkl_set_interface_layer = OSQP_NULL;
 static mkl_get_mt_t func_mkl_get_max_threads = OSQP_NULL;
@@ -51,15 +51,15 @@
 	}
 }
 
 c_int mkl_set_interface_layer(c_int code) {
     return (c_int)func_mkl_set_interface_layer((int)code);
 }
 
-c_int mkl_get_max_threads() {
+c_int mkl_get_max_threads(void) {
     return (c_int)func_mkl_get_max_threads();
 }
 
 
 c_int lh_load_pardiso(const char* libname) {
     // DEBUG
     // if (Pardiso_handle) return 0;
@@ -83,15 +83,15 @@
     func_mkl_get_max_threads = (mkl_get_mt_t)lh_load_sym(Pardiso_handle,
                                                     "MKL_Get_Max_Threads");
     if (!func_mkl_get_max_threads) return 1;
 
     return 0;
 }
 
-c_int lh_unload_pardiso() {
+c_int lh_unload_pardiso(void) {
 
     if (Pardiso_handle == OSQP_NULL) return 0;
 
     return lh_unload_lib(Pardiso_handle);
 
     /* If multiple OSQP objects are laoded, the lines below cause a crash */
     // Pardiso_handle = OSQP_NULL;
```

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  */
 c_int lh_load_pardiso(const char* libname);
 
 /**
  * Unloads the loaded Pardiso shared library.
  * @return Zero on success, nonzero on failure.
  */
-c_int lh_unload_pardiso();
+c_int lh_unload_pardiso(void);
 
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /*PARADISOLOADER_H*/
```

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h` & `osqp-0.6.3/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.c` & `osqp-0.6.3/osqp_sources/lin_sys/lib_handler.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.h` & `osqp-0.6.3/osqp_sources/lin_sys/lib_handler.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/CMakeLists.txt` & `osqp-0.6.3/osqp_sources/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/auxil.c` & `osqp-0.6.3/osqp_sources/src/auxil.c`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
   return 0;
 }
 
 c_int is_dual_infeasible(OSQPWorkspace *work, c_float eps_dual_inf) {
   // This function checks for the scaled dual infeasibility termination
   // criteria.
   //
-  // 1) q * delta_x < eps * || delta_x ||
+  // 1) q * delta_x < 0
   //
   // 2) ||P * delta_x || < eps * || delta_x ||
   //
   // 3) -> (A * delta_x)_i > -eps * || delta_x ||,    l_i != -inf
   //    -> (A * delta_x)_i <  eps * || delta_x ||,    u_i != inf
   //
```

### Comparing `osqp-0.6.2.post9/osqp_sources/src/cs.c` & `osqp-0.6.3/osqp_sources/src/cs.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/ctrlc.c` & `osqp-0.6.3/osqp_sources/src/ctrlc.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/error.c` & `osqp-0.6.3/osqp_sources/src/error.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/kkt.c` & `osqp-0.6.3/osqp_sources/src/kkt.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/lin_alg.c` & `osqp-0.6.3/osqp_sources/src/lin_alg.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/lin_sys.c` & `osqp-0.6.3/osqp_sources/src/lin_sys.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/osqp.c` & `osqp-0.6.3/osqp_sources/src/osqp.c`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,28 @@
 
         // Make sure the interval is not 0 and at least check_termination times
         work->settings->adaptive_rho_interval = c_max(
           work->settings->adaptive_rho_interval,
           work->settings->check_termination);
       } // If time condition is met
     }   // If adaptive rho enabled and interval set to auto
-# endif // PROFILING
+# else // PROFILING
+    if (work->settings->adaptive_rho && !work->settings->adaptive_rho_interval) {
+      // Set adaptive_rho_interval to constant value
+      if (work->settings->check_termination) {
+        // If check_termination is enabled, we set it to a multiple of the check
+        // termination interval
+        work->settings->adaptive_rho_interval = ADAPTIVE_RHO_MULTIPLE_TERMINATION *
+                                                work->settings->check_termination;
+      } else {
+        // If check_termination is disabled we set it to a predefined fix number
+        work->settings->adaptive_rho_interval = ADAPTIVE_RHO_FIXED;
+      }
+    }
+# endif /* ifdef PROFILING */
 
     // Adapt rho
     if (work->settings->adaptive_rho &&
         work->settings->adaptive_rho_interval &&
         (iter % work->settings->adaptive_rho_interval == 0)) {
       // Update info with the residuals if it hasn't been done before
 # ifdef PRINTING
```

### Comparing `osqp-0.6.2.post9/osqp_sources/src/polish.c` & `osqp-0.6.3/osqp_sources/src/polish.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/proj.c` & `osqp-0.6.3/osqp_sources/src/proj.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/scaling.c` & `osqp-0.6.3/osqp_sources/src/scaling.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/osqp_sources/src/util.c` & `osqp-0.6.3/osqp_sources/src/util.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/setup.py` & `osqp-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/extension/include/osqpinfopy.h` & `osqp-0.6.3/src/extension/include/osqpinfopy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/extension/include/osqpmodulemethods.h` & `osqp-0.6.3/src/extension/include/osqpmodulemethods.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/extension/include/osqpobjectpy.h` & `osqp-0.6.3/src/extension/include/osqpobjectpy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/extension/include/osqpresultspy.h` & `osqp-0.6.3/src/extension/include/osqpresultspy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/extension/include/osqputilspy.h` & `osqp-0.6.3/src/extension/include/osqputilspy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/extension/include/osqpworkspacepy.h` & `osqp-0.6.3/src/extension/include/osqpworkspacepy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/extension/src/osqpmodule.c` & `osqp-0.6.3/src/extension/src/osqpmodule.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/code_generator.py` & `osqp-0.6.3/src/osqp/codegen/code_generator.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/CMakeLists.txt` & `osqp-0.6.3/src/osqp/codegen/files_to_generate/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/emosqpmodule.c` & `osqp-0.6.3/src/osqp/codegen/files_to_generate/emosqpmodule.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/example.c` & `osqp-0.6.3/src/osqp/codegen/files_to_generate/example.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/setup.py` & `osqp-0.6.3/src/osqp/codegen/files_to_generate/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                             libraries=libraries,
                             include_dirs=include_dirs,
                             sources=sources_files,
                             extra_compile_args=compile_args)
 
 
 setup(name='PYTHON_EXT_NAME',
-      version='0.6.2.post9',
+      version='0.6.3',
       author='Bartolomeo Stellato, Goran Banjac',
       author_email='bartolomeo.stellato@gmail.com',
       description='This is the Python module for embedded OSQP: ' +
                   'Operator Splitting solver for Quadratic Programs.',
       setup_requires=["numpy >= 1.7"],
       install_requires=["numpy >= 1.7", "future"],
       license='Apache 2.0',
```

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/configure/osqp_configure.h.in` & `osqp-0.6.3/src/osqp/codegen/sources/configure/osqp_configure.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/configure/qdldl_types.h.in` & `osqp-0.6.3/src/osqp/codegen/sources/configure/qdldl_types.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/CMakeLists.txt` & `osqp-0.6.3/src/osqp/codegen/sources/include/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Add the OSQP headers
 set(
     osqp_headers
+    "${CMAKE_CURRENT_SOURCE_DIR}/version.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/auxil.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/constants.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/error.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/glob_opts.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/lin_alg.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/osqp.h"
     "${CMAKE_CURRENT_SOURCE_DIR}/osqp_configure.h"
```

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/auxil.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/auxil.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/constants.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/constants.h`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 extern "C" {
 # endif // ifdef __cplusplus
 
 
 /*******************
 * OSQP Versioning *
 *******************/
-# define OSQP_VERSION ("0.6.2") /* string literals automatically null-terminated
-                                   */
+#include "version.h"
 
 /******************
 * Solver Status  *
 ******************/
 # define OSQP_DUAL_INFEASIBLE_INACCURATE (4)
 # define OSQP_PRIMAL_INFEASIBLE_INACCURATE (3)
 # define OSQP_SOLVED_INACCURATE (2)
@@ -29,15 +28,15 @@
 # define OSQP_NON_CVX (-7)              /* problem non convex */
 # define OSQP_UNSOLVED (-10)            /* Unsolved. Only setup function has been called */
 
 
 /*************************
 * Linear System Solvers *
 *************************/
-enum linsys_solver_type { QDLDL_SOLVER, MKL_PARDISO_SOLVER };
+enum linsys_solver_type { QDLDL_SOLVER, MKL_PARDISO_SOLVER, UNKNOWN_SOLVER=99 };
 extern const char * LINSYS_SOLVER_NAME[];
 
 
 /******************
 * Solver Errors  *
 ******************/
 enum osqp_error_type {
```

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/error.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/error.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/glob_opts.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/glob_opts.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/kkt.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/kkt.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/lin_alg.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/lin_alg.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/osqp.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/osqp.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/proj.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/proj.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/qdldl.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl_interface.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/qdldl_interface.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/scaling.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/scaling.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/types.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/types.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/include/util.h` & `osqp-0.6.3/src/osqp/codegen/sources/include/util.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/CMakeLists.txt` & `osqp-0.6.3/src/osqp/codegen/sources/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/auxil.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/auxil.c`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
   return 0;
 }
 
 c_int is_dual_infeasible(OSQPWorkspace *work, c_float eps_dual_inf) {
   // This function checks for the scaled dual infeasibility termination
   // criteria.
   //
-  // 1) q * delta_x < eps * || delta_x ||
+  // 1) q * delta_x < 0
   //
   // 2) ||P * delta_x || < eps * || delta_x ||
   //
   // 3) -> (A * delta_x)_i > -eps * || delta_x ||,    l_i != -inf
   //    -> (A * delta_x)_i <  eps * || delta_x ||,    u_i != inf
   //
```

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/error.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/error.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/kkt.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/kkt.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/lin_alg.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/lin_alg.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/osqp.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/osqp.c`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,28 @@
 
         // Make sure the interval is not 0 and at least check_termination times
         work->settings->adaptive_rho_interval = c_max(
           work->settings->adaptive_rho_interval,
           work->settings->check_termination);
       } // If time condition is met
     }   // If adaptive rho enabled and interval set to auto
-# endif // PROFILING
+# else // PROFILING
+    if (work->settings->adaptive_rho && !work->settings->adaptive_rho_interval) {
+      // Set adaptive_rho_interval to constant value
+      if (work->settings->check_termination) {
+        // If check_termination is enabled, we set it to a multiple of the check
+        // termination interval
+        work->settings->adaptive_rho_interval = ADAPTIVE_RHO_MULTIPLE_TERMINATION *
+                                                work->settings->check_termination;
+      } else {
+        // If check_termination is disabled we set it to a predefined fix number
+        work->settings->adaptive_rho_interval = ADAPTIVE_RHO_FIXED;
+      }
+    }
+# endif /* ifdef PROFILING */
 
     // Adapt rho
     if (work->settings->adaptive_rho &&
         work->settings->adaptive_rho_interval &&
         (iter % work->settings->adaptive_rho_interval == 0)) {
       // Update info with the residuals if it hasn't been done before
 # ifdef PRINTING
```

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/proj.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/proj.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/qdldl.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl_interface.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/qdldl_interface.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/scaling.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/scaling.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/sources/src/util.c` & `osqp-0.6.3/src/osqp/codegen/sources/src/util.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/codegen/utils.py` & `osqp-0.6.3/src/osqp/codegen/utils.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/interface.py` & `osqp-0.6.3/src/osqp/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Python interface module for OSQP solver v0.6.2.post9
+Python interface module for OSQP solver v0.6.3
 """
 from __future__ import print_function
 from builtins import object
 import osqp._osqp as _osqp  # Internal low level module
 import numpy as np
 import scipy.sparse as spa
 from warnings import warn
```

### Comparing `osqp-0.6.2.post9/src/osqp/tests/basic_test.py` & `osqp-0.6.3/src/osqp/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/codegen_matrices_test.py` & `osqp-0.6.3/src/osqp/tests/codegen_matrices_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/codegen_vectors_test.py` & `osqp-0.6.3/src/osqp/tests/codegen_vectors_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/derivative_test.py` & `osqp-0.6.3/src/osqp/tests/derivative_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/dual_infeasibility_test.py` & `osqp-0.6.3/src/osqp/tests/dual_infeasibility_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/feasibility_test.py` & `osqp-0.6.3/src/osqp/tests/feasibility_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/mkl_pardiso_test.py` & `osqp-0.6.3/src/osqp/tests/mkl_pardiso_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/multithread_test.py` & `osqp-0.6.3/src/osqp/tests/multithread_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/non_convex_test.py` & `osqp-0.6.3/src/osqp/tests/non_convex_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/polishing_test.py` & `osqp-0.6.3/src/osqp/tests/polishing_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/primal_infeasibility_test.py` & `osqp-0.6.3/src/osqp/tests/primal_infeasibility_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_basic_QP.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_basic_QP.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_feasibility_problem.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_feasibility_problem.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_random.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_polish_random.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_simple.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_polish_simple.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_unconstrained.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_polish_unconstrained.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_solve.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_solve.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_unconstrained_problem.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_unconstrained_problem.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_A.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A_allind.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_A_allind.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_P.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_allind.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_allind.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indA.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_indA.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_indP.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_allind.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_P_allind.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_bounds.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_bounds.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_l.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_l.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_q.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_q.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_u.npz` & `osqp-0.6.3/src/osqp/tests/solutions/test_update_u.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/unconstrained_test.py` & `osqp-0.6.3/src/osqp/tests/unconstrained_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/update_matrices_test.py` & `osqp-0.6.3/src/osqp/tests/update_matrices_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/tests/warm_start_test.py` & `osqp-0.6.3/src/osqp/tests/warm_start_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp/utils.py` & `osqp-0.6.3/src/osqp/utils.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post9/src/osqp.egg-info/PKG-INFO` & `osqp-0.6.3/src/osqp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osqp
-Version: 0.6.2.post9
+Version: 0.6.3
 Summary: OSQP: The Operator Splitting QP Solver
 Home-page: https://osqp.org/
 Author: Bartolomeo Stellato, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
 License-File: LICENSE
```

### Comparing `osqp-0.6.2.post9/src/osqp.egg-info/SOURCES.txt` & `osqp-0.6.3/src/osqp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pyproject.toml
 requirements.txt
 setup.py
 .github/workflows/build.yml
 .github/workflows/build_aarch64.yml
 osqp_sources/CMakeLists.txt
 osqp_sources/configure/osqp_configure.h.in
+osqp_sources/configure/version.h.in
 osqp_sources/configure/cmake/FindPythonModule.cmake
 osqp_sources/configure/cmake/FindR.cmake
 osqp_sources/configure/cmake/Utils.cmake
 osqp_sources/configure/cmake/cmake_uninstall.cmake.in
 osqp_sources/include/.gitignore
 osqp_sources/include/CMakeLists.txt
 osqp_sources/include/auxil.h
@@ -27,14 +28,15 @@
 osqp_sources/include/lin_sys.h
 osqp_sources/include/osqp.h
 osqp_sources/include/polish.h
 osqp_sources/include/proj.h
 osqp_sources/include/scaling.h
 osqp_sources/include/types.h
 osqp_sources/include/util.h
+osqp_sources/include/version.h
 osqp_sources/lin_sys/CMakeLists.txt
 osqp_sources/lin_sys/lib_handler.c
 osqp_sources/lin_sys/lib_handler.h
 osqp_sources/lin_sys/direct/CMakeLists.txt
 osqp_sources/lin_sys/direct/pardiso/CMakeLists.txt
 osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c
 osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h
@@ -136,14 +138,15 @@
 src/osqp/codegen/sources/include/osqp.h
 src/osqp/codegen/sources/include/proj.h
 src/osqp/codegen/sources/include/qdldl.h
 src/osqp/codegen/sources/include/qdldl_interface.h
 src/osqp/codegen/sources/include/scaling.h
 src/osqp/codegen/sources/include/types.h
 src/osqp/codegen/sources/include/util.h
+src/osqp/codegen/sources/include/version.h
 src/osqp/codegen/sources/src/CMakeLists.txt
 src/osqp/codegen/sources/src/auxil.c
 src/osqp/codegen/sources/src/error.c
 src/osqp/codegen/sources/src/kkt.c
 src/osqp/codegen/sources/src/lin_alg.c
 src/osqp/codegen/sources/src/osqp.c
 src/osqp/codegen/sources/src/proj.c
```

### Comparing `osqp-0.6.2.post9/src/osqppurepy/_osqp.py` & `osqp-0.6.3/src/osqppurepy/_osqp.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 class OSQP(object):
     """OSQP solver lower level interface
     Attributes
     ----------
     work    - workspace
     """
     def __init__(self):
-        self._version = "0.6.2.post9"
+        self._version = "0.6.3"
 
     @property
     def version(self):
         """Return solver version
         """
         return self._version
```

### Comparing `osqp-0.6.2.post9/src/osqppurepy/interface.py` & `osqp-0.6.3/src/osqppurepy/interface.py`

 * *Files identical despite different names*

