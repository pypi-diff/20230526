# Comparing `tmp/pyzmq-25.0.2.tar.gz` & `tmp/pyzmq-25.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzmq-25.0.2.tar", last modified: Mon Mar 20 10:24:29 2023, max compression
+gzip compressed data, was "pyzmq-25.1.0.tar", last modified: Fri May 26 18:34:57 2023, max compression
```

## Comparing `pyzmq-25.0.2.tar` & `pyzmq-25.1.0.tar`

### file list

```diff
@@ -1,632 +1,689 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.774571 pyzmq-25.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-03-20 10:23:58.000000 pyzmq-25.0.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-03-20 10:23:58.000000 pyzmq-25.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-03-20 10:23:58.000000 pyzmq-25.0.2/LICENSE.BSD
--rw-r--r--   0 runner    (1001) docker     (122)    36008 2023-03-20 10:23:58.000000 pyzmq-25.0.2/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (122)      945 2023-03-20 10:23:58.000000 pyzmq-25.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-03-20 10:24:29.770571 pyzmq-25.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3486 2023-03-20 10:23:58.000000 pyzmq-25.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/
--rw-r--r--   0 runner    (1001) docker     (122)      191 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/_cffi.c
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/build_cffi.py
--rw-r--r--   0 runner    (1001) docker     (122)     8765 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/bundle.py
--rw-r--r--   0 runner    (1001) docker     (122)      225 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/check_sys_un.c
--rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4825 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/detect.py
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/dummy.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/include_darwin/
--rw-r--r--   0 runner    (1001) docker     (122)    11979 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/include_darwin/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/include_freebsd/
--rw-r--r--   0 runner    (1001) docker     (122)    11973 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/include_freebsd/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/include_linux/
--rw-r--r--   0 runner    (1001) docker     (122)    11973 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/include_linux/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/include_linux-armv/
--rw-r--r--   0 runner    (1001) docker     (122)    11796 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/include_linux-armv/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/include_linux-musl/
--rw-r--r--   0 runner    (1001) docker     (122)    11949 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/include_linux-musl/platform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/include_win32/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/include_win32/platform.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/include_win32/stdint.h
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/initlibzmq.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2203 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/msg.py
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/buildutils/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/templates/constant_enums.pxi
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/templates/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-03-20 10:23:58.000000 pyzmq-25.0.2/buildutils/vers.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.686565 pyzmq-25.0.2/bundled/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.694566 pyzmq-25.0.2/bundled/zeromq/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.686565 pyzmq-25.0.2/bundled/zeromq/external/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.698566 pyzmq-25.0.2/bundled/zeromq/external/wepoll/
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/external/wepoll/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/external/wepoll/license.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/external/wepoll/version.txt
--rw-r--r--   0 runner    (1001) docker     (122)    67905 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/external/wepoll/wepoll.c
--rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/external/wepoll/wepoll.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.698566 pyzmq-25.0.2/bundled/zeromq/include/
--rw-r--r--   0 runner    (1001) docker     (122)    30485 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/include/zmq.h
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/include/zmq_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.734569 pyzmq-25.0.2/bundled/zeromq/src/
--rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4224 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4370 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/array.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8854 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/atomic_counter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9468 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/atomic_ptr.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6102 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/blob.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/channel.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/channel.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/client.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/client.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8759 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/clock.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/clock.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/command.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/compat.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8141 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/condition_variable.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/config.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    26054 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ctx.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8388 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ctx.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9388 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/curve_client.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2780 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/curve_client.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    12182 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/curve_client_tools.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/curve_mechanism_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/curve_mechanism_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    18657 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/curve_server.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/curve_server.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3566 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dbuffer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3811 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dealer.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dealer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6899 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/decoder_allocators.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/decoder_allocators.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6025 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/devpoll.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/devpoll.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dgram.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2420 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dgram.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8764 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dish.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3579 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dish.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6665 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dist.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/dist.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5996 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/endpoint.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/endpoint.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6368 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/epoll.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/epoll.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    14985 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/err.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9104 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/err.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/fd.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4678 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/fq.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/fq.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gather.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gather.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/generic_mtrie.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    25261 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/generic_mtrie_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6889 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gssapi_client.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gssapi_client.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    11907 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gssapi_mechanism_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4506 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gssapi_mechanism_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7175 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gssapi_server.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/gssapi_server.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/i_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/i_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/i_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/i_mailbox.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/i_poll_events.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3054 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/io_object.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2835 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/io_object.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3369 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/io_thread.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/io_thread.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    28337 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ip.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3484 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ip.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    20596 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ip_resolver.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ip_resolver.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ipc_address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ipc_address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5781 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ipc_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ipc_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ipc_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2961 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ipc_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/kqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/kqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5777 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/lb.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/lb.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/libzmq.pc.in
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/libzmq.vers
--rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/likely.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mailbox.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mailbox.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3941 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mailbox_safe.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mailbox_safe.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13586 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mechanism.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mechanism.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mechanism_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mechanism_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/metadata.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/metadata.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    19649 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/msg.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10581 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/msg.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1561 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mtrie.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mtrie.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/mutex.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    26543 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/norm_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5608 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/norm_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7911 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/null_mechanism.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/null_mechanism.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13950 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/object.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6842 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/object.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    38451 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/options.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11026 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/options.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5884 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/own.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5310 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/own.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pair.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2339 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pair.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/peer.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/peer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8945 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pgm_receiver.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4286 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pgm_receiver.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7522 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pgm_sender.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pgm_sender.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    23464 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pgm_socket.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pgm_socket.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    17813 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pipe.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9733 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pipe.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/plain_client.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/plain_client.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/plain_common.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8971 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/plain_server.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/plain_server.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/platform.hpp.in
--rw-r--r--   0 runner    (1001) docker     (122)     5681 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/poll.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/poll.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/poller.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4770 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/poller_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/poller_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/polling_util.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5151 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/polling_util.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6558 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pollset.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pollset.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/precompiled.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/precompiled.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    26994 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/proxy.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1755 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/proxy.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pub.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pub.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pull.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/pull.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/push.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/push.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/radio.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/radio.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    21125 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/radix_tree.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/radix_tree.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6192 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/random.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/random.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2670 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/raw_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/raw_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/raw_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1927 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/raw_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/raw_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/raw_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/reaper.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/reaper.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/rep.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/rep.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9365 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/req.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3642 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/req.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    16617 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/router.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4450 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/router.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2636 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/scatter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2279 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/scatter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/secure_allocator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    20576 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/select.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/select.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5506 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/server.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/server.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    24036 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/session_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/session_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    11941 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/signaler.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/signaler.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    69471 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socket_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14347 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socket_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    19769 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socket_poller.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4735 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socket_poller.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socks.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4401 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socks.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13946 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socks_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/socks_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stdint.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9305 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream_connecter_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4081 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream_connecter_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    22556 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream_engine_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6451 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream_engine_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4086 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream_listener_base.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2845 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/stream_listener_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2671 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/sub.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/sub.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13889 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3319 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10085 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp_address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp_address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9387 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8781 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2514 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tcp_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    12211 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/thread.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4359 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/thread.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5130 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/timers.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/timers.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tipc_address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tipc_address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5336 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tipc_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tipc_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5346 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tipc_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tipc_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/trie.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2873 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/trie.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    21210 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tweetnacl.c
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/tweetnacl.h
--rw-r--r--   0 runner    (1001) docker     (122)     6322 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/udp_address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/udp_address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    17943 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/udp_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2547 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/udp_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v1_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v1_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3635 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v1_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v1_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6102 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v2_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v2_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3808 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v2_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v2_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v2_protocol.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4289 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v3_1_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1980 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/v3_1_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3521 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/version.rc.in
--rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci_address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci_address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8887 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7951 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/vmci_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/windows.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3941 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/wire.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4739 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8816 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_connecter.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_connecter.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9004 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_decoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5460 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_encoder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    39665 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5399 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_listener.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_listener.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ws_protocol.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/wss_address.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/wss_address.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6657 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/wss_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/wss_engine.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    14616 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/xpub.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5107 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/xpub.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8667 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/xsub.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/xsub.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7012 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ypipe.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ypipe_base.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/ypipe_conflate.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7259 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/yqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10538 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/zap_client.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/zap_client.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    43610 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/zmq.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/zmq_draft.h
--rw-r--r--   0 runner    (1001) docker     (122)    10286 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/zmq_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    19910 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/zmtp_engine.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-03-20 10:24:29.000000 pyzmq-25.0.2/bundled/zeromq/src/zmtp_engine.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.734569 pyzmq-25.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)     1456 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/autogen_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.734569 pyzmq-25.0.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.738569 pyzmq-25.0.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     8686 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/_static/zeromq.ico
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.738569 pyzmq-25.0.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.auth.asyncio.rst
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.auth.ioloop.rst
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.auth.rst
--rw-r--r--   0 runner    (1001) docker     (122)      353 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.auth.thread.rst
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.decorators.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.devices.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.eventloop.future.rst
--rw-r--r--   0 runner    (1001) docker     (122)      170 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.eventloop.ioloop.rst
--rw-r--r--   0 runner    (1001) docker     (122)      353 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.eventloop.zmqstream.rst
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.green.rst
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.log.handlers.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.rst
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.ssh.tunnel.rst
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.utils.jsonapi.rst
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.utils.monitor.rst
--rw-r--r--   0 runner    (1001) docker     (122)      242 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.utils.win32.rst
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/api/zmq.utils.z85.rst
--rw-r--r--   0 runner    (1001) docker     (122)    37481 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (122)     7421 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.738569 pyzmq-25.0.2/docs/source/howto/
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/devices.md
--rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/draft.md
--rw-r--r--   0 runner    (1001) docker     (122)     8531 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/eventloop.md
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     9610 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/logging.md
--rw-r--r--   0 runner    (1001) docker     (122)     7619 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/morethanbindings.md
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/serialization.md
--rw-r--r--   0 runner    (1001) docker     (122)     2868 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/howto/ssh.md
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.738569 pyzmq-25.0.2/docs/source/notes/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/notes/index.md
--rw-r--r--   0 runner    (1001) docker     (122)     7076 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/notes/pyversions.md
--rw-r--r--   0 runner    (1001) docker     (122)     8843 2023-03-20 10:23:58.000000 pyzmq-25.0.2/docs/source/notes/unicode.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/asyncio/
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/asyncio/coroutines.py
--rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/asyncio/helloworld_pubsub_dealerrouter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2289 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/asyncio/router_router.py
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/asyncio/tornado_asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/chat/
--rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/chat/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/chat/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/cython/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/cython/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/cython/cyzmq.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/cython/example.py
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/cython/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/device/
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/draft/
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/draft/client-server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/draft/install.sh
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/draft/radio-dish.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/eventloop/
--rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/eventloop/asyncweb.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/eventloop/coroutines.py
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/eventloop/echo.py
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/eventloop/echofuture.py
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/eventloop/echostream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/gevent/
--rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/gevent/poll.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/gevent/reqrep.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/gevent/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/heartbeat/
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/heartbeat/heart.py
--rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/heartbeat/heartbeater.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/heartbeat/ping.py
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/heartbeat/pong.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/logger/
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/logger/zmqlogger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.742569 pyzmq-25.0.2/examples/mongodb/
--rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/mongodb/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3234 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/mongodb/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.746569 pyzmq-25.0.2/examples/monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/monitoring/simple_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5001 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/monitoring/zmq_monitor_class.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.746569 pyzmq-25.0.2/examples/poll/
--rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/poll/pair.py
--rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/poll/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/poll/reqrep.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.746569 pyzmq-25.0.2/examples/pubsub/
--rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/pubsub/publisher.py
--rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/pubsub/subscriber.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2033 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/pubsub/topics_pub.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1773 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/pubsub/topics_sub.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.746569 pyzmq-25.0.2/examples/security/
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/asyncio-ironhouse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/generate_certificates.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/grasslands.py
--rw-r--r--   0 runner    (1001) docker     (122)     4265 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/ioloop-ironhouse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/ironhouse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/stonehouse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2215 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/strawhouse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2353 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/security/woodhouse.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.746569 pyzmq-25.0.2/examples/serialization/
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/serialization/serialsocket.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.746569 pyzmq-25.0.2/examples/win32-interrupt/
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/win32-interrupt/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-03-20 10:23:58.000000 pyzmq-25.0.2/examples/win32-interrupt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.746569 pyzmq-25.0.2/perf/
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-03-20 10:23:58.000000 pyzmq-25.0.2/perf/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-03-20 10:23:58.000000 pyzmq-25.0.2/perf/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)     4538 2023-03-20 10:23:58.000000 pyzmq-25.0.2/perf/collect.py
--rw-r--r--   0 runner    (1001) docker     (122)   167790 2023-03-20 10:23:58.000000 pyzmq-25.0.2/perf/perf.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-03-20 10:23:58.000000 pyzmq-25.0.2/perf/perf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3127 2023-03-20 10:23:58.000000 pyzmq-25.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.750570 pyzmq-25.0.2/pyzmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-03-20 10:24:29.000000 pyzmq-25.0.2/pyzmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    16995 2023-03-20 10:24:29.000000 pyzmq-25.0.2/pyzmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 10:24:29.000000 pyzmq-25.0.2/pyzmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 10:24:17.000000 pyzmq-25.0.2/pyzmq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-03-20 10:24:29.000000 pyzmq-25.0.2/pyzmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        4 2023-03-20 10:24:29.000000 pyzmq-25.0.2/pyzmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-20 10:24:29.774571 pyzmq-25.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-03-20 10:23:58.000000 pyzmq-25.0.2/setup.cfg.android
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 10:23:58.000000 pyzmq-25.0.2/setup.cfg.template
--rwxr-xr-x   0 runner    (1001) docker     (122)    46767 2023-03-20 10:23:58.000000 pyzmq-25.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.750570 pyzmq-25.0.2/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-03-20 10:23:58.000000 pyzmq-25.0.2/tools/backend_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-03-20 10:23:58.000000 pyzmq-25.0.2/tools/install_libzmq.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3786 2023-03-20 10:23:58.000000 pyzmq-25.0.2/tools/run_with_env.cmd
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-03-20 10:23:58.000000 pyzmq-25.0.2/tools/showvcvars.py
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-03-20 10:23:58.000000 pyzmq-25.0.2/tools/test_wheel.py
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-03-20 10:23:58.000000 pyzmq-25.0.2/tools/wheel-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.750570 pyzmq-25.0.2/zmq/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4007 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/_future.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/_typing.py
--rw-r--r--   0 runner    (1001) docker     (122)     6271 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/asyncio.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.750570 pyzmq-25.0.2/zmq/auth/
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/auth/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)    16337 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4331 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/auth/certs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/auth/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/auth/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.750570 pyzmq-25.0.2/zmq/backend/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.754570 pyzmq-25.0.2/zmq/backend/cffi/
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/_cdefs.h
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/_poll.py
--rw-r--r--   0 runner    (1001) docker     (122)     1899 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/error.py
--rw-r--r--   0 runner    (1001) docker     (122)     6547 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/message.py
--rw-r--r--   0 runner    (1001) docker     (122)    11450 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cffi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.758570 pyzmq-25.0.2/zmq/backend/cython/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   233872 2023-03-20 10:24:06.000000 pyzmq-25.0.2/zmq/backend/cython/_device.c
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/_device.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   299037 2023-03-20 10:24:07.000000 pyzmq-25.0.2/zmq/backend/cython/_poll.c
--rw-r--r--   0 runner    (1001) docker     (122)     5616 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/_poll.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   219410 2023-03-20 10:24:07.000000 pyzmq-25.0.2/zmq/backend/cython/_proxy_steerable.c
--rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/_proxy_steerable.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   140815 2023-03-20 10:24:07.000000 pyzmq-25.0.2/zmq/backend/cython/_version.c
--rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/_version.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      968 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/checkrc.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     7025 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/constant_enums.pxi
--rw-r--r--   0 runner    (1001) docker     (122)   286944 2023-03-20 10:24:07.000000 pyzmq-25.0.2/zmq/backend/cython/context.c
--rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/context.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/context.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   146864 2023-03-20 10:24:07.000000 pyzmq-25.0.2/zmq/backend/cython/error.c
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/error.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     4564 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/libzmq.pxd
--rw-r--r--   0 runner    (1001) docker     (122)   467388 2023-03-20 10:24:08.000000 pyzmq-25.0.2/zmq/backend/cython/message.c
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/message.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    13681 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/message.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   653075 2023-03-20 10:24:08.000000 pyzmq-25.0.2/zmq/backend/cython/socket.c
--rw-r--r--   0 runner    (1001) docker     (122)     2104 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/socket.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    26369 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/socket.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   190524 2023-03-20 10:24:08.000000 pyzmq-25.0.2/zmq/backend/cython/utils.c
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/cython/utils.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/backend/select.py
--rw-r--r--   0 runner    (1001) docker     (122)    26123 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     5076 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.762570 pyzmq-25.0.2/zmq/devices/
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9564 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (122)   291594 2023-03-20 10:24:09.000000 pyzmq-25.0.2/zmq/devices/monitoredqueue.c
--rw-r--r--   0 runner    (1001) docker     (122)     6386 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/monitoredqueue.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/monitoredqueue.py
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/monitoredqueue.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/monitoredqueuedevice.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/proxydevice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/devices/proxysteerabledevice.py
--rw-r--r--   0 runner    (1001) docker     (122)     5392 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.762570 pyzmq-25.0.2/zmq/eventloop/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/eventloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6444 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/eventloop/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/eventloop/future.py
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/eventloop/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (122)    23704 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/eventloop/zmqstream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.762570 pyzmq-25.0.2/zmq/green/
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/green/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10827 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/green/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/green/device.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.762570 pyzmq-25.0.2/zmq/green/eventloop/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/green/eventloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/green/eventloop/ioloop.py
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/green/eventloop/zmqstream.py
--rw-r--r--   0 runner    (1001) docker     (122)     2950 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/green/poll.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.762570 pyzmq-25.0.2/zmq/include/
--rw-r--r--   0 runner    (1001) docker     (122)    30485 2023-03-20 10:24:29.000000 pyzmq-25.0.2/zmq/include/zmq.h
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-03-20 10:24:29.000000 pyzmq-25.0.2/zmq/include/zmq_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.762570 pyzmq-25.0.2/zmq/log/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/log/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/log/handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.762570 pyzmq-25.0.2/zmq/ssh/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/ssh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3358 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/ssh/forward.py
--rw-r--r--   0 runner    (1001) docker     (122)    13286 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/ssh/tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.766571 pyzmq-25.0.2/zmq/sugar/
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2603 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/attrsettr.py
--rw-r--r--   0 runner    (1001) docker     (122)    14400 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/context.py
--rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/poll.py
--rw-r--r--   0 runner    (1001) docker     (122)    33871 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (122)     3700 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/tracker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/sugar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.770571 pyzmq-25.0.2/zmq/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      642 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/cython_ext.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     9544 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (122)    14426 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     8945 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_cffi_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    12600 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_cython.py
--rw-r--r--   0 runner    (1001) docker     (122)     9623 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     6004 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_draft.py
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (122)      533 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_etc.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_ext.py
--rw-r--r--   0 runner    (1001) docker     (122)    10608 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_includes.py
--rw-r--r--   0 runner    (1001) docker     (122)      641 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_ioloop.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (122)    11260 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_monqueue.py
--rw-r--r--   0 runner    (1001) docker     (122)      885 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_multipart.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_mypy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_pair.py
--rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_poll.py
--rw-r--r--   0 runner    (1001) docker     (122)     3718 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_proxy_steerable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_reqrep.py
--rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_retry_eintr.py
--rw-r--r--   0 runner    (1001) docker     (122)     7805 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_security.py
--rw-r--r--   0 runner    (1001) docker     (122)    23190 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_win32_shim.py
--rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_z85.py
--rw-r--r--   0 runner    (1001) docker     (122)     4195 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/tests/test_zmqstream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 10:24:29.770571 pyzmq-25.0.2/zmq/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7031 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/buffers.pxd
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-03-20 10:24:29.000000 pyzmq-25.0.2/zmq/utils/compiler.json
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-03-20 10:24:29.000000 pyzmq-25.0.2/zmq/utils/config.json
--rw-r--r--   0 runner    (1001) docker     (122)     6125 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/garbage.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/getpid_compat.h
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/interop.py
--rw-r--r--   0 runner    (1001) docker     (122)      522 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/ipcmaxlen.h
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/jsonapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/mutex.h
--rw-r--r--   0 runner    (1001) docker     (122)      284 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/pyversion_compat.h
--rw-r--r--   0 runner    (1001) docker     (122)     1376 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/strtypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/win32.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/z85.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmq/utils/zmq_compat.h
--rw-r--r--   0 runner    (1001) docker     (122)     4103 2023-03-20 10:23:58.000000 pyzmq-25.0.2/zmqversion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.889535 pyzmq-25.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.753534 pyzmq-25.1.0/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (122)     2034 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.753534 pyzmq-25.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.753534 pyzmq-25.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.753534 pyzmq-25.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     5189 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     5070 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.mailmap
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.753534 pyzmq-25.1.0/.obs/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.obs/workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-26 18:34:14.000000 pyzmq-25.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-05-26 18:34:14.000000 pyzmq-25.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-05-26 18:34:14.000000 pyzmq-25.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1545 2023-05-26 18:34:14.000000 pyzmq-25.1.0/LICENSE.BSD
+-rw-r--r--   0 runner    (1001) docker     (122)    36008 2023-05-26 18:34:14.000000 pyzmq-25.1.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-26 18:34:14.000000 pyzmq-25.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-26 18:34:57.889535 pyzmq-25.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3486 2023-05-26 18:34:14.000000 pyzmq-25.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.757534 pyzmq-25.1.0/RELICENSE/
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2757 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/authors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      721 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/chrislaws.md
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/ellisonbg.md
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/frankwiles.md
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/juliantaylor.md
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/ledgerx.md
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/lothiraldan.md
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/minrk.md
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/takluyver.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.757534 pyzmq-25.1.0/RELICENSE/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/templates/relicense-template-bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/templates/relicense-template-mplv2-any-osi.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-26 18:34:14.000000 pyzmq-25.1.0/RELICENSE/templates/relicense-template-mplv2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-05-26 18:34:14.000000 pyzmq-25.1.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-26 18:34:14.000000 pyzmq-25.1.0/Vagrantfile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.757534 pyzmq-25.1.0/buildutils/
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/_cffi.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/build_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8765 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/check_sys_un.c
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4825 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/detect.py
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/dummy.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.757534 pyzmq-25.1.0/buildutils/include_darwin/
+-rw-r--r--   0 runner    (1001) docker     (122)    11979 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/include_darwin/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/buildutils/include_freebsd/
+-rw-r--r--   0 runner    (1001) docker     (122)    11973 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/include_freebsd/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/buildutils/include_linux/
+-rw-r--r--   0 runner    (1001) docker     (122)    11973 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/include_linux/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/buildutils/include_linux-armv/
+-rw-r--r--   0 runner    (1001) docker     (122)    11796 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/include_linux-armv/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/buildutils/include_linux-musl/
+-rw-r--r--   0 runner    (1001) docker     (122)    11949 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/include_linux-musl/platform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/buildutils/include_win32/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/include_win32/platform.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/include_win32/stdint.h
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/initlibzmq.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2203 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/msg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/buildutils/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/templates/constant_enums.pxi
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/templates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-26 18:34:14.000000 pyzmq-25.1.0/buildutils/vers.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.741534 pyzmq-25.1.0/bundled/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/bundled/zeromq/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.741534 pyzmq-25.1.0/bundled/zeromq/external/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/bundled/zeromq/external/wepoll/
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/external/wepoll/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/external/wepoll/license.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/external/wepoll/version.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    67905 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/external/wepoll/wepoll.c
+-rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/external/wepoll/wepoll.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.761534 pyzmq-25.1.0/bundled/zeromq/include/
+-rw-r--r--   0 runner    (1001) docker     (122)    30485 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/include/zmq.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/include/zmq_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.833535 pyzmq-25.1.0/bundled/zeromq/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4224 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4370 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/array.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8854 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/atomic_counter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9468 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/atomic_ptr.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6102 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/blob.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4350 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/channel.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/channel.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/client.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2430 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/client.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8759 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/clock.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/clock.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/command.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/compat.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8141 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/condition_variable.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3778 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/config.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    26054 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ctx.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8388 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ctx.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9388 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/curve_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2780 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/curve_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12182 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/curve_client_tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11117 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/curve_mechanism_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3675 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/curve_mechanism_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    18657 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/curve_server.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/curve_server.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3566 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dbuffer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3811 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dealer.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dealer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6899 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4810 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/decoder_allocators.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4423 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/decoder_allocators.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6025 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/devpoll.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/devpoll.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dgram.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2420 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dgram.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8764 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dish.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3579 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dish.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6665 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dist.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3832 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/dist.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5996 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/endpoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2471 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/endpoint.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6368 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/epoll.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3128 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/epoll.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14985 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/err.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9104 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/err.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/fd.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4678 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/fq.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/fq.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gather.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gather.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/generic_mtrie.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    25261 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/generic_mtrie_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6889 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gssapi_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2854 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gssapi_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11907 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gssapi_mechanism_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4506 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gssapi_mechanism_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7175 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gssapi_server.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/gssapi_server.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2165 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/i_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2130 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/i_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2919 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/i_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/i_mailbox.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/i_poll_events.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3054 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/io_object.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2835 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/io_object.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3369 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/io_thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2977 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/io_thread.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    28337 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ip.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3484 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ip.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20596 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ip_resolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ip_resolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3690 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ipc_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ipc_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5781 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ipc_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2607 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ipc_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ipc_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2961 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ipc_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6269 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/kqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/kqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5777 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/lb.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/lb.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/libzmq.pc.in
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/libzmq.vers
+-rw-r--r--   0 runner    (1001) docker     (122)     1672 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/likely.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mailbox.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mailbox.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3941 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mailbox_safe.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mailbox_safe.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13586 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mechanism.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mechanism.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mechanism_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mechanism_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2095 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/metadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2167 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/metadata.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19649 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/msg.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10581 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/msg.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1561 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mtrie.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mtrie.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/mutex.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    26543 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/norm_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5608 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/norm_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7911 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/null_mechanism.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/null_mechanism.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13950 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/object.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6842 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/object.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    38451 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/options.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11026 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/options.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5884 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/own.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5310 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/own.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pair.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2339 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pair.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/peer.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2163 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/peer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8945 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pgm_receiver.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4286 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pgm_receiver.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7522 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pgm_sender.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pgm_sender.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    23464 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pgm_socket.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pgm_socket.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    17813 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pipe.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9733 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pipe.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/plain_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2461 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/plain_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/plain_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8971 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/plain_server.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/plain_server.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11153 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/platform.hpp.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5681 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/poll.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3334 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/poll.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/poller.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4770 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/poller_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7116 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/poller_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/polling_util.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5151 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/polling_util.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6558 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pollset.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pollset.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/precompiled.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/precompiled.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    26994 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/proxy.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1755 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/proxy.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pub.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pub.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pull.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/pull.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2435 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/push.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/push.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/radio.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3505 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/radio.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    21125 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/radix_tree.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/radix_tree.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6192 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/random.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/random.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2670 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/raw_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/raw_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/raw_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1927 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/raw_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/raw_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2436 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/raw_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3906 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/reaper.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/reaper.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/rep.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/rep.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9365 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/req.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3642 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/req.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16617 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/router.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4450 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/router.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2636 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/scatter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2279 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/scatter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/secure_allocator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20576 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/select.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4856 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/select.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5506 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/server.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/server.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    24036 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/session_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/session_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11941 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/signaler.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2879 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/signaler.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    69471 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socket_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14347 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socket_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19769 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socket_poller.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4735 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socket_poller.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10238 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socks.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4401 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socks.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13946 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socks_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/socks_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2242 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stdint.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9305 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3131 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream_connecter_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4081 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream_connecter_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    22556 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream_engine_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6451 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream_engine_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4086 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream_listener_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2845 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/stream_listener_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2671 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/sub.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1914 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/sub.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13889 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3319 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10085 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9387 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8781 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2514 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tcp_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12211 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/thread.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4359 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/thread.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5130 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/timers.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/timers.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tipc_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tipc_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5336 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tipc_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2662 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tipc_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5346 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tipc_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tipc_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/trie.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2873 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/trie.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    21210 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tweetnacl.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/tweetnacl.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6322 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/udp_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/udp_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    17943 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/udp_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2547 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/udp_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5040 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v1_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v1_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3635 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v1_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v1_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6102 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v2_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v2_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3808 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v2_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v2_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v2_protocol.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4289 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v3_1_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1980 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/v3_1_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3521 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/version.rc.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2231 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8887 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7951 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/vmci_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3349 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/windows.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3941 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/wire.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4739 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2518 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8816 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_connecter.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3343 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_connecter.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9004 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_decoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5460 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_encoder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    39665 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5399 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10748 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_listener.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_listener.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ws_protocol.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/wss_address.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/wss_address.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6657 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/wss_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2320 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/wss_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14616 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/xpub.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5107 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/xpub.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8667 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/xsub.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4014 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/xsub.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7012 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ypipe.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ypipe_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3798 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/ypipe_conflate.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7259 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/yqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10538 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/zap_client.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3376 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/zap_client.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    43610 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/zmq.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/zmq_draft.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10286 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/zmq_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19910 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/zmtp_engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4159 2023-05-26 18:34:57.000000 pyzmq-25.1.0/bundled/zeromq/src/zmtp_engine.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-26 18:34:14.000000 pyzmq-25.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.833535 pyzmq-25.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     3631 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1456 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/autogen_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.833535 pyzmq-25.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.833535 pyzmq-25.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     8686 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/_static/zeromq.ico
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.837535 pyzmq-25.1.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.auth.asyncio.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.auth.ioloop.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      353 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.auth.thread.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.decorators.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1951 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.eventloop.future.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.eventloop.ioloop.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      353 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.eventloop.zmqstream.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.green.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.log.handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.ssh.tunnel.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.utils.jsonapi.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.utils.monitor.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      242 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.utils.win32.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/api/zmq.utils.z85.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    38453 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7421 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.841534 pyzmq-25.1.0/docs/source/howto/
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/devices.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/draft.md
+-rw-r--r--   0 runner    (1001) docker     (122)     8531 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/eventloop.md
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9610 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/logging.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7619 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/morethanbindings.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/serialization.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2868 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/howto/ssh.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.841534 pyzmq-25.1.0/docs/source/notes/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/notes/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7076 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/notes/pyversions.md
+-rw-r--r--   0 runner    (1001) docker     (122)     8843 2023-05-26 18:34:14.000000 pyzmq-25.1.0/docs/source/notes/unicode.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.841534 pyzmq-25.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.841534 pyzmq-25.1.0/examples/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/asyncio/coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/asyncio/helloworld_pubsub_dealerrouter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2289 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/asyncio/router_router.py
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/asyncio/tornado_asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.841534 pyzmq-25.1.0/examples/chat/
+-rw-r--r--   0 runner    (1001) docker     (122)     1343 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/chat/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/chat/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.841534 pyzmq-25.1.0/examples/cython/
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/cython/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/cython/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/cython/cyzmq.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/cython/example.py
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/cython/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.841534 pyzmq-25.1.0/examples/device/
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.845535 pyzmq-25.1.0/examples/draft/
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/draft/client-server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/draft/install.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/draft/radio-dish.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.845535 pyzmq-25.1.0/examples/eventloop/
+-rw-r--r--   0 runner    (1001) docker     (122)     2039 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/eventloop/asyncweb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/eventloop/coroutines.py
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/eventloop/echo.py
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/eventloop/echofuture.py
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/eventloop/echostream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.845535 pyzmq-25.1.0/examples/gevent/
+-rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/gevent/poll.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/gevent/reqrep.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/gevent/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.845535 pyzmq-25.1.0/examples/heartbeat/
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/heartbeat/heart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/heartbeat/heartbeater.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/heartbeat/ping.py
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/heartbeat/pong.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.845535 pyzmq-25.1.0/examples/logger/
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/logger/zmqlogger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.845535 pyzmq-25.1.0/examples/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (122)     1555 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/mongodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3256 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/mongodb/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.845535 pyzmq-25.1.0/examples/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/monitoring/simple_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5001 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/monitoring/zmq_monitor_class.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.849535 pyzmq-25.1.0/examples/poll/
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/poll/pair.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1401 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/poll/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/poll/reqrep.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.849535 pyzmq-25.1.0/examples/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/pubsub/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1849 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/pubsub/subscriber.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2033 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/pubsub/topics_pub.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1773 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/pubsub/topics_sub.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.849535 pyzmq-25.1.0/examples/security/
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/asyncio-ironhouse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/generate_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/grasslands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4265 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/ioloop-ironhouse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/ironhouse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/stonehouse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2215 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/strawhouse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2353 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/security/woodhouse.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.849535 pyzmq-25.1.0/examples/serialization/
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/serialization/serialsocket.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.849535 pyzmq-25.1.0/examples/win32-interrupt/
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/win32-interrupt/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-05-26 18:34:14.000000 pyzmq-25.1.0/examples/win32-interrupt/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-05-26 18:34:14.000000 pyzmq-25.1.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.849535 pyzmq-25.1.0/mypy_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-26 18:34:14.000000 pyzmq-25.1.0/mypy_tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-05-26 18:34:14.000000 pyzmq-25.1.0/mypy_tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-26 18:34:14.000000 pyzmq-25.1.0/mypy_tests/test_toplevel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.745534 pyzmq-25.1.0/packaging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.853535 pyzmq-25.1.0/packaging/debian/
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (122)     2298 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/debian/control
+-rw-r--r--   0 runner    (1001) docker     (122)     6045 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/debian/pyzmq.dsc.obs
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1708 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.853535 pyzmq-25.1.0/packaging/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.853535 pyzmq-25.1.0/packaging/obs/
+-rw-r--r--   0 runner    (1001) docker     (122)     2338 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/obs/_service
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.853535 pyzmq-25.1.0/packaging/redhat/
+-rw-r--r--   0 runner    (1001) docker     (122)     7812 2023-05-26 18:34:14.000000 pyzmq-25.1.0/packaging/redhat/python-pyzmq.spec
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.853535 pyzmq-25.1.0/perf/
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-26 18:34:14.000000 pyzmq-25.1.0/perf/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-05-26 18:34:14.000000 pyzmq-25.1.0/perf/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     4538 2023-05-26 18:34:14.000000 pyzmq-25.1.0/perf/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)   167790 2023-05-26 18:34:14.000000 pyzmq-25.1.0/perf/perf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-05-26 18:34:14.000000 pyzmq-25.1.0/perf/perf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3295 2023-05-26 18:34:14.000000 pyzmq-25.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-05-26 18:34:14.000000 pyzmq-25.1.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.857535 pyzmq-25.1.0/pyzmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-26 18:34:57.000000 pyzmq-25.1.0/pyzmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18064 2023-05-26 18:34:57.000000 pyzmq-25.1.0/pyzmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 18:34:57.000000 pyzmq-25.1.0/pyzmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 18:34:44.000000 pyzmq-25.1.0/pyzmq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-26 18:34:57.000000 pyzmq-25.1.0/pyzmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-26 18:34:57.000000 pyzmq-25.1.0/pyzmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 18:34:57.889535 pyzmq-25.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-05-26 18:34:14.000000 pyzmq-25.1.0/setup.cfg.android
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-05-26 18:34:14.000000 pyzmq-25.1.0/setup.cfg.template
+-rwxr-xr-x   0 runner    (1001) docker     (122)    46587 2023-05-26 18:34:14.000000 pyzmq-25.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-05-26 18:34:14.000000 pyzmq-25.1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.857535 pyzmq-25.1.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-26 18:34:14.000000 pyzmq-25.1.0/tools/backend_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1973 2023-05-26 18:34:14.000000 pyzmq-25.1.0/tools/install_libzmq.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3786 2023-05-26 18:34:14.000000 pyzmq-25.1.0/tools/run_with_env.cmd
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-26 18:34:14.000000 pyzmq-25.1.0/tools/showvcvars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-05-26 18:34:14.000000 pyzmq-25.1.0/tools/test_sdist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-05-26 18:34:14.000000 pyzmq-25.1.0/tools/test_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-26 18:34:14.000000 pyzmq-25.1.0/tools/wheel-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.857535 pyzmq-25.1.0/zmq/
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     4007 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/_future.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6271 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/asyncio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.861535 pyzmq-25.1.0/zmq/auth/
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1799 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/auth/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16337 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4331 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/auth/certs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/auth/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4092 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/auth/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.861535 pyzmq-25.1.0/zmq/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.861535 pyzmq-25.1.0/zmq/backend/cffi/
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/_cdefs.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1899 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6547 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/message.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11450 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cffi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.869535 pyzmq-25.1.0/zmq/backend/cython/
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   235785 2023-05-26 18:34:43.000000 pyzmq-25.1.0/zmq/backend/cython/_device.c
+-rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/_device.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   301006 2023-05-26 18:34:44.000000 pyzmq-25.1.0/zmq/backend/cython/_poll.c
+-rw-r--r--   0 runner    (1001) docker     (122)     5616 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/_poll.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   221323 2023-05-26 18:34:44.000000 pyzmq-25.1.0/zmq/backend/cython/_proxy_steerable.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/_proxy_steerable.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   140815 2023-05-26 18:34:27.000000 pyzmq-25.1.0/zmq/backend/cython/_version.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1449 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/_version.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      968 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/checkrc.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     7025 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/constant_enums.pxi
+-rw-r--r--   0 runner    (1001) docker     (122)   288736 2023-05-26 18:34:44.000000 pyzmq-25.1.0/zmq/backend/cython/context.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1408 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     4118 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   147308 2023-05-26 18:34:41.000000 pyzmq-25.1.0/zmq/backend/cython/error.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/error.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     4564 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/libzmq.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)   469218 2023-05-26 18:34:42.000000 pyzmq-25.1.0/zmq/backend/cython/message.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/message.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    13681 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/message.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   655194 2023-05-26 18:34:42.000000 pyzmq-25.1.0/zmq/backend/cython/socket.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2104 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/socket.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)    26369 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/socket.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)   190524 2023-05-26 18:34:29.000000 pyzmq-25.1.0/zmq/backend/cython/utils.c
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/cython/utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/backend/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26123 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5076 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.873535 pyzmq-25.1.0/zmq/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9564 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)   293507 2023-05-26 18:34:43.000000 pyzmq-25.1.0/zmq/devices/monitoredqueue.c
+-rw-r--r--   0 runner    (1001) docker     (122)     6386 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/monitoredqueue.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)     1021 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/monitoredqueue.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/monitoredqueue.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/monitoredqueuedevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/proxydevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/devices/proxysteerabledevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5392 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.873535 pyzmq-25.1.0/zmq/eventloop/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/eventloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6444 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/eventloop/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/eventloop/future.py
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/eventloop/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23704 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/eventloop/zmqstream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.873535 pyzmq-25.1.0/zmq/green/
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/green/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10827 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/green/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/green/device.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.873535 pyzmq-25.1.0/zmq/green/eventloop/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/green/eventloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/green/eventloop/ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/green/eventloop/zmqstream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2950 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/green/poll.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.877535 pyzmq-25.1.0/zmq/log/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3913 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/log/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7108 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/log/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.877535 pyzmq-25.1.0/zmq/ssh/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/ssh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3358 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/ssh/forward.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13286 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/ssh/tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.877535 pyzmq-25.1.0/zmq/sugar/
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2603 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/attrsettr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14400 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5725 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/poll.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34093 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3700 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/sugar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.885535 pyzmq-25.1.0/zmq/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8169 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      642 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/cython_ext.pyx
+-rw-r--r--   0 runner    (1001) docker     (122)     9544 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14426 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8945 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_cffi_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12600 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_cython.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9623 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6004 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_draft.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      533 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_etc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10608 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_includes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_ioloop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11260 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3059 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8285 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_monqueue.py
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1683 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_pair.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_poll.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3718 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_proxy_steerable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_reqrep.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2874 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_retry_eintr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7805 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23610 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_win32_shim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_z85.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4195 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/tests/test_zmqstream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:57.889535 pyzmq-25.1.0/zmq/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7031 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/buffers.pxd
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-05-26 18:34:57.000000 pyzmq-25.1.0/zmq/utils/compiler.json
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-05-26 18:34:57.000000 pyzmq-25.1.0/zmq/utils/config.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6125 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/garbage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/getpid_compat.h
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/interop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/ipcmaxlen.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/jsonapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (122)      284 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/pyversion_compat.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1376 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/strtypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/win32.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/z85.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmq/utils/zmq_compat.h
+-rw-r--r--   0 runner    (1001) docker     (122)     4103 2023-05-26 18:34:14.000000 pyzmq-25.1.0/zmqversion.py
```

### Comparing `pyzmq-25.0.2/AUTHORS.md` & `pyzmq-25.1.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/CONTRIBUTING.md` & `pyzmq-25.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/LICENSE.BSD` & `pyzmq-25.1.0/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/LICENSE.LESSER` & `pyzmq-25.1.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/PKG-INFO` & `pyzmq-25.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzmq
-Version: 25.0.2
+Version: 25.1.0
 Summary: Python bindings for 0MQ
 Home-page: https://pyzmq.readthedocs.org
 Author: Brian E. Granger, Min Ragan-Kelley
 Author-email: zeromq-dev@lists.zeromq.org
 License: LGPL+BSD
 Project-URL: Source, https://github.com/zeromq/pyzmq
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyzmq-25.0.2/README.md` & `pyzmq-25.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/_cffi.c` & `pyzmq-25.1.0/buildutils/_cffi.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/build_cffi.py` & `pyzmq-25.1.0/buildutils/build_cffi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/bundle.py` & `pyzmq-25.1.0/buildutils/bundle.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/config.py` & `pyzmq-25.1.0/buildutils/config.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/constants.py` & `pyzmq-25.1.0/buildutils/constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/detect.py` & `pyzmq-25.1.0/buildutils/detect.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/include_darwin/platform.hpp` & `pyzmq-25.1.0/buildutils/include_darwin/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/include_freebsd/platform.hpp` & `pyzmq-25.1.0/buildutils/include_freebsd/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/include_linux/platform.hpp` & `pyzmq-25.1.0/buildutils/include_linux/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/include_linux-armv/platform.hpp` & `pyzmq-25.1.0/buildutils/include_linux-armv/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/include_linux-musl/platform.hpp` & `pyzmq-25.1.0/buildutils/include_linux-musl/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/include_win32/platform.hpp` & `pyzmq-25.1.0/buildutils/include_win32/platform.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/initlibzmq.cpp` & `pyzmq-25.1.0/buildutils/initlibzmq.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/misc.py` & `pyzmq-25.1.0/buildutils/misc.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/msg.py` & `pyzmq-25.1.0/buildutils/msg.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/buildutils/patch.py` & `pyzmq-25.1.0/buildutils/patch.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/COPYING` & `pyzmq-25.1.0/bundled/zeromq/COPYING`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/external/wepoll/README.md` & `pyzmq-25.1.0/bundled/zeromq/external/wepoll/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/external/wepoll/license.txt` & `pyzmq-25.1.0/bundled/zeromq/external/wepoll/license.txt`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/external/wepoll/wepoll.c` & `pyzmq-25.1.0/bundled/zeromq/external/wepoll/wepoll.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/external/wepoll/wepoll.h` & `pyzmq-25.1.0/bundled/zeromq/external/wepoll/wepoll.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/include/zmq.h` & `pyzmq-25.1.0/bundled/zeromq/include/zmq.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/include/zmq_utils.h` & `pyzmq-25.1.0/bundled/zeromq/include/zmq_utils.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/array.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/array.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/atomic_counter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/atomic_counter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/atomic_ptr.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/atomic_ptr.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/blob.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/blob.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/channel.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/channel.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/channel.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/channel.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/client.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/client.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/clock.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/clock.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/clock.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/clock.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/command.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/command.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/compat.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/compat.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/condition_variable.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/condition_variable.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/config.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/config.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ctx.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ctx.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ctx.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ctx.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/curve_client.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/curve_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/curve_client.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/curve_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/curve_client_tools.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/curve_client_tools.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/curve_mechanism_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/curve_mechanism_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/curve_mechanism_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/curve_mechanism_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/curve_server.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/curve_server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/curve_server.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/curve_server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dbuffer.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/dbuffer.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dealer.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/dealer.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dealer.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/dealer.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/decoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/decoder_allocators.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/decoder_allocators.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/decoder_allocators.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/decoder_allocators.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/devpoll.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/devpoll.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/devpoll.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/devpoll.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dgram.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/dgram.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dgram.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/dgram.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dish.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/dish.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dish.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/dish.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dist.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/dist.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/dist.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/dist.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/encoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/endpoint.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/endpoint.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/endpoint.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/endpoint.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/epoll.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/epoll.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/epoll.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/epoll.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/err.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/err.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/err.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/err.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/fd.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/fd.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/fq.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/fq.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/fq.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/fq.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gather.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/gather.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gather.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/gather.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/generic_mtrie.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/generic_mtrie.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/generic_mtrie_impl.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/generic_mtrie_impl.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gssapi_client.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/gssapi_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gssapi_client.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/gssapi_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gssapi_mechanism_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/gssapi_mechanism_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gssapi_mechanism_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/gssapi_mechanism_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gssapi_server.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/gssapi_server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/gssapi_server.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/gssapi_server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/i_decoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/i_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/i_encoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/i_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/i_engine.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/i_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/i_mailbox.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/i_mailbox.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/i_poll_events.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/i_poll_events.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/io_object.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/io_object.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/io_object.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/io_object.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/io_thread.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/io_thread.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/io_thread.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/io_thread.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ip.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ip.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ip.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ip.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ip_resolver.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ip_resolver.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ip_resolver.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ip_resolver.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ipc_address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ipc_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ipc_address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ipc_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ipc_connecter.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ipc_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ipc_connecter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ipc_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ipc_listener.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ipc_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ipc_listener.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ipc_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/kqueue.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/kqueue.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/kqueue.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/kqueue.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/lb.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/lb.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/lb.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/lb.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/likely.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/likely.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/macros.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/macros.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mailbox.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/mailbox.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mailbox.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/mailbox.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mailbox_safe.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/mailbox_safe.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mailbox_safe.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/mailbox_safe.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mechanism.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/mechanism.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mechanism.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/mechanism.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mechanism_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/mechanism_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mechanism_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/mechanism_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/metadata.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/metadata.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/metadata.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/metadata.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/msg.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/msg.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/msg.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/msg.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mtrie.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/mtrie.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mtrie.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/mtrie.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/mutex.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/mutex.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/norm_engine.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/norm_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/norm_engine.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/norm_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/null_mechanism.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/null_mechanism.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/null_mechanism.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/null_mechanism.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/object.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/object.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/object.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/object.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/options.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/options.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/options.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/options.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/own.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/own.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/own.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/own.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pair.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pair.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pair.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pair.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/peer.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/peer.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/peer.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/peer.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pgm_receiver.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pgm_receiver.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pgm_receiver.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pgm_receiver.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pgm_sender.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pgm_sender.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pgm_sender.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pgm_sender.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pgm_socket.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pgm_socket.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pgm_socket.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pgm_socket.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pipe.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pipe.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pipe.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pipe.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/plain_client.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/plain_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/plain_client.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/plain_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/plain_common.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/plain_common.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/plain_server.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/plain_server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/plain_server.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/plain_server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/platform.hpp.in` & `pyzmq-25.1.0/bundled/zeromq/src/platform.hpp.in`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/poll.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/poll.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/poll.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/poll.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/poller.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/poller.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/poller_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/poller_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/poller_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/poller_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/polling_util.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/polling_util.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/polling_util.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/polling_util.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pollset.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pollset.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pollset.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pollset.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/precompiled.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/precompiled.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/precompiled.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/precompiled.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/proxy.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/proxy.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/proxy.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/proxy.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pub.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pub.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pull.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/pull.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/pull.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/pull.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/push.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/push.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/push.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/push.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/radio.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/radio.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/radio.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/radio.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/radix_tree.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/radix_tree.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/radix_tree.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/radix_tree.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/random.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/random.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/random.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/random.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/raw_decoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/raw_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/raw_decoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/raw_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/raw_encoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/raw_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/raw_encoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/raw_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/raw_engine.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/raw_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/raw_engine.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/raw_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/reaper.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/reaper.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/reaper.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/reaper.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/rep.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/rep.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/rep.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/rep.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/req.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/req.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/req.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/req.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/router.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/router.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/router.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/router.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/scatter.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/scatter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/scatter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/scatter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/secure_allocator.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/secure_allocator.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/select.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/select.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/select.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/select.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/server.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/server.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/server.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/server.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/session_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/session_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/session_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/session_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/signaler.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/signaler.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/signaler.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/signaler.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socket_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/socket_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socket_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/socket_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socket_poller.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/socket_poller.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socket_poller.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/socket_poller.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socks.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/socks.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socks.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/socks.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socks_connecter.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/socks_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/socks_connecter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/socks_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stdint.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/stdint.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream_connecter_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream_connecter_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream_connecter_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream_connecter_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream_engine_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream_engine_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream_engine_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream_engine_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream_listener_base.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream_listener_base.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/stream_listener_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/stream_listener_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/sub.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/sub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/sub.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/sub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp_address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp_address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp_connecter.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp_connecter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp_listener.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tcp_listener.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/tcp_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/thread.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/thread.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/thread.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/thread.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/timers.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/timers.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/timers.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/timers.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tipc_address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/tipc_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tipc_address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/tipc_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tipc_connecter.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/tipc_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tipc_connecter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/tipc_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tipc_listener.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/tipc_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tipc_listener.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/tipc_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/trie.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/trie.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/trie.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/trie.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tweetnacl.c` & `pyzmq-25.1.0/bundled/zeromq/src/tweetnacl.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/tweetnacl.h` & `pyzmq-25.1.0/bundled/zeromq/src/tweetnacl.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/udp_address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/udp_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/udp_address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/udp_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/udp_engine.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/udp_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/udp_engine.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/udp_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v1_decoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/v1_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v1_decoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/v1_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v1_encoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/v1_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v1_encoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/v1_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v2_decoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/v2_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v2_decoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/v2_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v2_encoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/v2_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v2_encoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/v2_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v2_protocol.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/v2_protocol.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v3_1_encoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/v3_1_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/v3_1_encoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/v3_1_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/version.rc.in` & `pyzmq-25.1.0/bundled/zeromq/src/version.rc.in`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci_address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci_address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci_connecter.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci_connecter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci_listener.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/vmci_listener.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/vmci_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/windows.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/windows.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/wire.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/wire.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_connecter.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_connecter.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_connecter.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_connecter.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_decoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_decoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_decoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_decoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_encoder.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_encoder.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_encoder.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_engine.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_engine.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_listener.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_listener.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_listener.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_listener.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ws_protocol.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ws_protocol.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/wss_address.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/wss_address.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/wss_address.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/wss_address.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/wss_engine.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/wss_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/wss_engine.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/wss_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/xpub.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/xpub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/xpub.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/xpub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/xsub.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/xsub.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/xsub.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/xsub.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ypipe.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ypipe.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ypipe_base.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ypipe_base.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/ypipe_conflate.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/ypipe_conflate.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/yqueue.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/yqueue.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/zap_client.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/zap_client.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/zap_client.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/zap_client.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/zmq.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/zmq.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/zmq_draft.h` & `pyzmq-25.1.0/bundled/zeromq/src/zmq_draft.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/zmq_utils.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/zmq_utils.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/zmtp_engine.cpp` & `pyzmq-25.1.0/bundled/zeromq/src/zmtp_engine.cpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/bundled/zeromq/src/zmtp_engine.hpp` & `pyzmq-25.1.0/bundled/zeromq/src/zmtp_engine.hpp`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/Makefile` & `pyzmq-25.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/autogen_api.py` & `pyzmq-25.1.0/docs/autogen_api.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/_static/logo.png` & `pyzmq-25.1.0/docs/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/_static/zeromq.ico` & `pyzmq-25.1.0/docs/source/_static/zeromq.ico`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/api/zmq.asyncio.rst` & `pyzmq-25.1.0/docs/source/api/zmq.asyncio.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/api/zmq.devices.rst` & `pyzmq-25.1.0/docs/source/api/zmq.devices.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/api/zmq.eventloop.future.rst` & `pyzmq-25.1.0/docs/source/api/zmq.eventloop.future.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/api/zmq.rst` & `pyzmq-25.1.0/docs/source/api/zmq.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/api/zmq.ssh.tunnel.rst` & `pyzmq-25.1.0/docs/source/api/zmq.ssh.tunnel.rst`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/changelog.md` & `pyzmq-25.1.0/docs/source/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 # Changes in PyZMQ
 
 This is a coarse summary of changes in pyzmq versions.
 For a full changelog, consult the [git log](https://github.com/zeromq/pyzmq/commits).
 
 ## 25
 
+### 25.1.0
+
+pyzmq 25.1 mostly changes some packaging details of pyzmq, including support for installation from source on Python 3.12 beta 1.
+
+Enhancements:
+
+- Include address in error message when bind/connect fail.
+
+Packaging changes:
+
+- Fix inclusion of some test files in source distributions.
+- Add Cython as a build-time dependency in `build-system.requires` metadata, following current [recommendations][cython-build-requires] of the Cython maintainers.
+  We still ship generated Cython sources in source distributions, so it is not a _strict_ dependency for packagers using `--no-build-isolation`, but pip will install Cython as part of building pyzmq from source.
+  This makes it more likely that past pyzmq releases will install on future Python releases, which often require an update to Cython but not pyzmq itself.
+  For Python 3.12, Cython >=3.0.0b3 is required.
+
 ### 25.0.2
 
 - Fix handling of shadow sockets in ZMQStream when the original sockets have been closed. A regression in 25.0.0, seen with jupyter-client 7.
 
 ### 25.0.1
 
 Tiny bugfix release that should only affect users of {class}`~.PUBHandler` or pyzmq repackagers.
@@ -867,15 +883,15 @@
 - {class}`~.Context` objects can now set default options when they create a socket. These
   are set and accessed as attributes to the context.  Socket options that do not apply to a
   socket (e.g. SUBSCRIBE on non-SUB sockets) will simply be ignored.
 - {meth}`~.ZMQStream.on_recv_stream` has been added, which adds the stream itself as a
   second argument to the callback, making it easier to use a single callback on multiple
   streams.
 - A {attr}`~Frame.more` boolean attribute has been added to the {class}`~.Frame` (née
-  Message) class, so that frames can be identified as terminal without extra queires of
+  Message) class, so that frames can be identified as terminal without extra queries of
   {attr}`~.Socket.rcvmore`.
 
 ### Experimental New Stuff
 
 These features are marked 'experimental', which means that their APIs are not
 set in stone, and may be removed or changed in incompatible ways in later releases.
 
@@ -979,8 +995,9 @@
 
 ## 2.1.4
 
 - First version with binary distribution support
 - Added {meth}`~Context.instance()` method for using a single Context throughout an application
   without passing references around.
 
+[cython-build-requires]: https://groups.google.com/g/cython-users/c/ZqKFQmS0JdA/m/1FrK1ApYBAAJ
 [pyczmq]: https://github.com/zeromq/pyczmq
```

### Comparing `pyzmq-25.0.2/docs/source/conf.py` & `pyzmq-25.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/howto/devices.md` & `pyzmq-25.1.0/docs/source/howto/devices.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/howto/draft.md` & `pyzmq-25.1.0/docs/source/howto/draft.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/howto/eventloop.md` & `pyzmq-25.1.0/docs/source/howto/eventloop.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/howto/logging.md` & `pyzmq-25.1.0/docs/source/howto/logging.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/howto/morethanbindings.md` & `pyzmq-25.1.0/docs/source/howto/morethanbindings.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/howto/serialization.md` & `pyzmq-25.1.0/docs/source/howto/serialization.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/howto/ssh.md` & `pyzmq-25.1.0/docs/source/howto/ssh.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/index.md` & `pyzmq-25.1.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/notes/pyversions.md` & `pyzmq-25.1.0/docs/source/notes/pyversions.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/docs/source/notes/unicode.md` & `pyzmq-25.1.0/docs/source/notes/unicode.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/asyncio/coroutines.py` & `pyzmq-25.1.0/examples/asyncio/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/asyncio/helloworld_pubsub_dealerrouter.py` & `pyzmq-25.1.0/examples/asyncio/helloworld_pubsub_dealerrouter.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/asyncio/router_router.py` & `pyzmq-25.1.0/examples/asyncio/router_router.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/asyncio/tornado_asyncio.py` & `pyzmq-25.1.0/examples/asyncio/tornado_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/chat/display.py` & `pyzmq-25.1.0/examples/chat/display.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/chat/prompt.py` & `pyzmq-25.1.0/examples/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/cython/README.md` & `pyzmq-25.1.0/examples/cython/README.md`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/cython/cyzmq.pyx` & `pyzmq-25.1.0/examples/cython/cyzmq.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/cython/example.py` & `pyzmq-25.1.0/examples/cython/example.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/device/device.py` & `pyzmq-25.1.0/examples/device/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/draft/client-server.py` & `pyzmq-25.1.0/examples/draft/client-server.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/draft/install.sh` & `pyzmq-25.1.0/examples/draft/install.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/draft/radio-dish.py` & `pyzmq-25.1.0/examples/draft/radio-dish.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/eventloop/asyncweb.py` & `pyzmq-25.1.0/examples/eventloop/asyncweb.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/eventloop/coroutines.py` & `pyzmq-25.1.0/examples/eventloop/coroutines.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/eventloop/echo.py` & `pyzmq-25.1.0/examples/eventloop/echo.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/gevent/poll.py` & `pyzmq-25.1.0/examples/gevent/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/gevent/reqrep.py` & `pyzmq-25.1.0/examples/gevent/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/gevent/simple.py` & `pyzmq-25.1.0/examples/gevent/simple.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/heartbeat/heart.py` & `pyzmq-25.1.0/examples/heartbeat/heart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/heartbeat/heartbeater.py` & `pyzmq-25.1.0/examples/heartbeat/heartbeater.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/heartbeat/ping.py` & `pyzmq-25.1.0/examples/heartbeat/ping.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/heartbeat/pong.py` & `pyzmq-25.1.0/examples/heartbeat/pong.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/logger/zmqlogger.py` & `pyzmq-25.1.0/examples/logger/zmqlogger.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/mongodb/client.py` & `pyzmq-25.1.0/examples/mongodb/client.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/mongodb/controller.py` & `pyzmq-25.1.0/examples/mongodb/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #  the file LICENSE.BSD, distributed as part of this software.
 # -----------------------------------------------------------------------------
 
 import json
 from typing import Any, Dict, Optional, Union
 
 import pymongo
-import pymongo.json_util
+from bson import json_util
 
 import zmq
 
 
 class MongoZMQ:
     """
     ZMQ server that adds/fetches documents (ie dictionaries) to a MongoDB.
@@ -28,33 +28,33 @@
         bind_addr: address to bind zmq socket on
         db_name: name of database to write to (created if doesn't exist)
         table_name: name of mongodb 'table' in the db to write to (created if doesn't exist)
         """
         self._bind_addr = bind_addr
         self._db_name = db_name
         self._table_name = table_name
-        self._conn = pymongo.Connection()
+        self._conn: pymongo.MongoClient = pymongo.MongoClient()
         self._db = self._conn[self._db_name]
         self._table = self._db[self._table_name]
 
     def _doc_to_json(self, doc: Any) -> str:
-        return json.dumps(doc, default=pymongo.json_util.default)
+        return json.dumps(doc, default=json_util.default)
 
     def add_document(self, doc: Dict) -> Optional[str]:
         """
         Inserts a document (dictionary) into mongo database table
         """
         print(f'adding document {doc}')
         try:
             self._table.insert(doc)
         except Exception as e:
             return 'Error: %s' % e
         return None
 
-    def get_document_by_keys(self, keys: Dict[str, Any]) -> Union[Dict, str]:
+    def get_document_by_keys(self, keys: Dict[str, Any]) -> Union[Dict, str, None]:
         """
         Attempts to return a single document from database table that matches
         each key/value in keys dictionary.
         """
         print('attempting to retrieve document using keys: %s' % keys)
         try:
             return self._table.find_one(keys)
```

### Comparing `pyzmq-25.0.2/examples/monitoring/simple_monitor.py` & `pyzmq-25.1.0/examples/monitoring/simple_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/monitoring/zmq_monitor_class.py` & `pyzmq-25.1.0/examples/monitoring/zmq_monitor_class.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/poll/pair.py` & `pyzmq-25.1.0/examples/poll/pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/poll/pubsub.py` & `pyzmq-25.1.0/examples/poll/pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/poll/reqrep.py` & `pyzmq-25.1.0/examples/poll/reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/pubsub/publisher.py` & `pyzmq-25.1.0/examples/pubsub/publisher.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/pubsub/subscriber.py` & `pyzmq-25.1.0/examples/pubsub/subscriber.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/pubsub/topics_pub.py` & `pyzmq-25.1.0/examples/pubsub/topics_pub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/pubsub/topics_sub.py` & `pyzmq-25.1.0/examples/pubsub/topics_sub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/asyncio-ironhouse.py` & `pyzmq-25.1.0/examples/security/asyncio-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/generate_certificates.py` & `pyzmq-25.1.0/examples/security/generate_certificates.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/grasslands.py` & `pyzmq-25.1.0/examples/security/grasslands.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/ioloop-ironhouse.py` & `pyzmq-25.1.0/examples/security/ioloop-ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/ironhouse.py` & `pyzmq-25.1.0/examples/security/ironhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/stonehouse.py` & `pyzmq-25.1.0/examples/security/stonehouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/strawhouse.py` & `pyzmq-25.1.0/examples/security/strawhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/security/woodhouse.py` & `pyzmq-25.1.0/examples/security/woodhouse.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/serialization/serialsocket.py` & `pyzmq-25.1.0/examples/serialization/serialsocket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/win32-interrupt/display.py` & `pyzmq-25.1.0/examples/win32-interrupt/display.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/examples/win32-interrupt/prompt.py` & `pyzmq-25.1.0/examples/win32-interrupt/prompt.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/perf/Makefile` & `pyzmq-25.1.0/perf/Makefile`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/perf/collect.py` & `pyzmq-25.1.0/perf/collect.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/perf/perf.ipynb` & `pyzmq-25.1.0/perf/perf.ipynb`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/perf/perf.py` & `pyzmq-25.1.0/perf/perf.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/pyproject.toml` & `pyzmq-25.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 skip = [
     "zmq/__init__.py"
 ]
 
 [build-system]
 requires = [
     "setuptools",
+    "setuptools_scm[toml]",
     "wheel",
     "packaging",
     "cffi; implementation_name == 'pypy'",
+    "cython>=0.29; implementation_name == 'cpython'",
+    "cython>=3.0.0b3; implementation_name == 'cpython' and python_version >= '3.12'",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/zeromq/pyzmq"
 
 [tool.tbump.version]
-current = "25.0.2"
+current = "25.1.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?P<pre>((a|b|rc|)\d+)|.dev\d*|)
```

### Comparing `pyzmq-25.0.2/pyzmq.egg-info/PKG-INFO` & `pyzmq-25.1.0/pyzmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzmq
-Version: 25.0.2
+Version: 25.1.0
 Summary: Python bindings for 0MQ
 Home-page: https://pyzmq.readthedocs.org
 Author: Brian E. Granger, Min Ragan-Kelley
 Author-email: zeromq-dev@lists.zeromq.org
 License: LGPL+BSD
 Project-URL: Source, https://github.com/zeromq/pyzmq
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyzmq-25.0.2/pyzmq.egg-info/SOURCES.txt` & `pyzmq-25.1.0/pyzmq.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,51 @@
+.coveragerc
+.flake8
+.gitignore
+.mailmap
+.pre-commit-config.yaml
+.prettierignore
+.readthedocs.yml
 AUTHORS.md
 CONTRIBUTING.md
 LICENSE.BSD
 LICENSE.LESSER
 MANIFEST.in
 README.md
+SECURITY.md
+Vagrantfile
+codecov.yml
+mypy.ini
 pyproject.toml
+pytest.ini
 setup.cfg.android
 setup.cfg.template
 setup.py
+test-requirements.txt
 zmqversion.py
+.circleci/config.yml
+.github/dependabot.yml
+.github/ISSUE_TEMPLATE/bug.yml
+.github/ISSUE_TEMPLATE/config.yml
+.github/workflows/test.yml
+.github/workflows/wheels.yml
+.obs/workflows.yml
+RELICENSE/README.md
+RELICENSE/authors.py
+RELICENSE/chrislaws.md
+RELICENSE/ellisonbg.md
+RELICENSE/frankwiles.md
+RELICENSE/juliantaylor.md
+RELICENSE/ledgerx.md
+RELICENSE/lothiraldan.md
+RELICENSE/minrk.md
+RELICENSE/takluyver.md
+RELICENSE/templates/relicense-template-bsd.txt
+RELICENSE/templates/relicense-template-mplv2-any-osi.txt
+RELICENSE/templates/relicense-template-mplv2.txt
 buildutils/__init__.py
 buildutils/_cffi.c
 buildutils/build_cffi.py
 buildutils/bundle.py
 buildutils/check_sys_un.c
 buildutils/config.py
 buildutils/constants.py
@@ -360,14 +393,15 @@
 examples/README.md
 examples/asyncio/coroutines.py
 examples/asyncio/helloworld_pubsub_dealerrouter.py
 examples/asyncio/router_router.py
 examples/asyncio/tornado_asyncio.py
 examples/chat/display.py
 examples/chat/prompt.py
+examples/cython/.gitignore
 examples/cython/README.md
 examples/cython/cyzmq.pyx
 examples/cython/example.py
 examples/cython/setup.py
 examples/device/device.py
 examples/draft/client-server.py
 examples/draft/install.sh
@@ -403,14 +437,26 @@
 examples/security/ironhouse.py
 examples/security/stonehouse.py
 examples/security/strawhouse.py
 examples/security/woodhouse.py
 examples/serialization/serialsocket.py
 examples/win32-interrupt/display.py
 examples/win32-interrupt/prompt.py
+mypy_tests/test_context.py
+mypy_tests/test_socket.py
+mypy_tests/test_toplevel.py
+packaging/debian/changelog
+packaging/debian/compat
+packaging/debian/control
+packaging/debian/copyright
+packaging/debian/pyzmq.dsc.obs
+packaging/debian/rules
+packaging/debian/source/format
+packaging/obs/_service
+packaging/redhat/python-pyzmq.spec
 perf/Dockerfile
 perf/Makefile
 perf/collect.py
 perf/perf.ipynb
 perf/perf.py
 pyzmq.egg-info/PKG-INFO
 pyzmq.egg-info/SOURCES.txt
@@ -418,14 +464,15 @@
 pyzmq.egg-info/not-zip-safe
 pyzmq.egg-info/requires.txt
 pyzmq.egg-info/top_level.txt
 tools/backend_imports.py
 tools/install_libzmq.sh
 tools/run_with_env.cmd
 tools/showvcvars.py
+tools/test_sdist.py
 tools/test_wheel.py
 tools/wheel-requirements.txt
 zmq/__init__.pxd
 zmq/__init__.py
 zmq/__init__.pyi
 zmq/_future.py
 zmq/_typing.py
@@ -496,16 +543,14 @@
 zmq/green/__init__.py
 zmq/green/core.py
 zmq/green/device.py
 zmq/green/poll.py
 zmq/green/eventloop/__init__.py
 zmq/green/eventloop/ioloop.py
 zmq/green/eventloop/zmqstream.py
-zmq/include/zmq.h
-zmq/include/zmq_utils.h
 zmq/log/__init__.py
 zmq/log/__main__.py
 zmq/log/handlers.py
 zmq/ssh/__init__.py
 zmq/ssh/forward.py
 zmq/ssh/tunnel.py
 zmq/sugar/__init__.py
```

### Comparing `pyzmq-25.0.2/setup.cfg.template` & `pyzmq-25.1.0/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/setup.py` & `pyzmq-25.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -418,15 +418,15 @@
         if cfg.get('zmq_draft_api'):
             settings['define_macros'].append(('ZMQ_BUILD_DRAFT_API', 1))
 
         use_static_zmq = cfg.get('use_static_zmq', 'False').upper()
         if use_static_zmq in ('TRUE', '1'):
             settings['define_macros'].append(('ZMQ_STATIC', '1'))
 
-        if os.environ.get("PYZMQ_CYTHON_COVERAGE"):
+        if os.environ.get("PYZMQ_CYTHON_COVERAGE", "") not in {"", "0"}:
             settings['define_macros'].append(('CYTHON_TRACE', '1'))
 
         # include internal directories
         settings.setdefault('include_dirs', [])
         settings['include_dirs'] += [pjoin('zmq', sub) for sub in ('utils',)]
 
         settings.setdefault('libraries', [])
@@ -1184,14 +1184,17 @@
     },
 }
 
 # require cython 0.29
 min_cython_version = "0.29"
 cython_language_level = "3str"
 
+if sys.version_info >= (3, 12):
+    min_cython_version = "3.0.0b3"
+
 try:
     import Cython
 
     if V(Cython.__version__) < V(min_cython_version):
         raise ImportError(
             "Cython >= %s required for cython build, found %s"
             % (min_cython_version, Cython.__version__)
@@ -1273,15 +1276,15 @@
         ext = Extension(f"zmq.{submod}.{pkg}", sources=sources, **ext_kwargs)
         extensions.append(ext)
 
 if cython:
     # set binding so that compiled methods can be inspected
     # set language-level to 3str, requires Cython 0.29
     cython_directives = {"binding": True, "language_level": "3str"}
-    if os.environ.get("PYZMQ_CYTHON_COVERAGE"):
+    if os.environ.get("PYZMQ_CYTHON_COVERAGE", "") not in {"", "0"}:
         cython_directives["linetrace"] = True
     extensions = cythonize(extensions, compiler_directives=cython_directives)
 
 if pypy:
     extensions = []
 
 if pypy or os.environ.get("PYZMQ_BACKEND_CFFI"):
@@ -1318,15 +1321,15 @@
 # -----------------------------------------------------------------------------
 
 with open('README.md', encoding='utf-8') as f:
     long_desc = f.read()
 
 setup_args = dict(
     name="pyzmq",
-    version="25.0.2",
+    version="25.1.0",
     packages=find_packages(),
     ext_modules=extensions,
     cffi_modules=cffi_modules,
     package_data=package_data,
     author="Brian E. Granger, Min Ragan-Kelley",
     author_email="zeromq-dev@lists.zeromq.org",
     url="https://pyzmq.readthedocs.org",
@@ -1358,15 +1361,9 @@
     ],
     zip_safe=False,
     python_requires=">=3.6",
     install_requires=[
         "cffi; implementation_name == 'pypy'",
     ],
 )
-if not os.path.exists(os.path.join("zmq", "backend", "cython", "socket.c")):
-    # this generally means pip install from git
-    # which requires Cython
-    setup_args.setdefault("setup_requires", []).append(
-        f"cython>={min_cython_version}; implementation_name == 'cpython'",
-    )
 
 setup(**setup_args)
```

### Comparing `pyzmq-25.0.2/tools/install_libzmq.sh` & `pyzmq-25.1.0/tools/install_libzmq.sh`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/tools/run_with_env.cmd` & `pyzmq-25.1.0/tools/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/tools/test_wheel.py` & `pyzmq-25.1.0/tools/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/__init__.py` & `pyzmq-25.1.0/zmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/__init__.pyi` & `pyzmq-25.1.0/zmq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/_future.py` & `pyzmq-25.1.0/zmq/_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/asyncio.py` & `pyzmq-25.1.0/zmq/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/auth/asyncio.py` & `pyzmq-25.1.0/zmq/auth/asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/auth/base.py` & `pyzmq-25.1.0/zmq/auth/base.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/auth/certs.py` & `pyzmq-25.1.0/zmq/auth/certs.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/auth/ioloop.py` & `pyzmq-25.1.0/zmq/auth/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/auth/thread.py` & `pyzmq-25.1.0/zmq/auth/thread.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/__init__.py` & `pyzmq-25.1.0/zmq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/__init__.pyi` & `pyzmq-25.1.0/zmq/backend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/__init__.py` & `pyzmq-25.1.0/zmq/backend/cffi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/_cdefs.h` & `pyzmq-25.1.0/zmq/backend/cffi/_cdefs.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/_poll.py` & `pyzmq-25.1.0/zmq/backend/cffi/_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/context.py` & `pyzmq-25.1.0/zmq/backend/cffi/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/devices.py` & `pyzmq-25.1.0/zmq/backend/cffi/devices.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/message.py` & `pyzmq-25.1.0/zmq/backend/cffi/message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/socket.py` & `pyzmq-25.1.0/zmq/backend/cffi/socket.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cffi/utils.py` & `pyzmq-25.1.0/zmq/backend/cffi/utils.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/__init__.py` & `pyzmq-25.1.0/zmq/backend/cython/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_device.c` & `pyzmq-25.1.0/zmq/backend/cython/_device.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,24 +93,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -218,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -567,35 +571,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1225,26 +1229,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1383,22 +1387,30 @@
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -2948,15 +2960,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -3004,43 +3016,38 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -3226,15 +3233,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__backend__cython___device) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4357,84 +4364,102 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -4996,17 +5021,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -5073,15 +5103,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -5125,15 +5158,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -5434,15 +5467,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5706,15 +5739,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_device.pyx` & `pyzmq-25.1.0/zmq/backend/cython/_device.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_poll.c` & `pyzmq-25.1.0/zmq/backend/cython/_poll.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,24 +93,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -218,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -567,35 +571,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1383,26 +1387,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1450,22 +1454,30 @@
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -3640,15 +3652,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1000 = PyInt_FromLong(1000); if (unlikely(!__pyx_int_1000)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
@@ -3697,44 +3709,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(2, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(2, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(2, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(3, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(3, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -3926,15 +3933,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__backend__cython___poll) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4570,28 +4577,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -4733,18 +4740,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* GetAttr */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
 #if CYTHON_USE_TYPE_SLOTS
 #if PY_MAJOR_VERSION >= 3
     if (likely(PyUnicode_Check(n)))
@@ -4917,15 +4922,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -5419,61 +5424,79 @@
     Py_DECREF(args);
     Py_DECREF(function);
 done:
     return result;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -6035,17 +6058,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -6112,15 +6140,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -6164,15 +6195,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -6473,15 +6504,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6745,15 +6776,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6941,15 +6972,15 @@
                         } else if (8 * sizeof(short) >= 4 * PyLong_SHIFT) {
                             return (short) (((((((((short)digits[3]) << PyLong_SHIFT) | (short)digits[2]) << PyLong_SHIFT) | (short)digits[1]) << PyLong_SHIFT) | (short)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7137,15 +7168,15 @@
                         } else if (8 * sizeof(ZMQ_FD_T) >= 4 * PyLong_SHIFT) {
                             return (ZMQ_FD_T) (((((((((ZMQ_FD_T)digits[3]) << PyLong_SHIFT) | (ZMQ_FD_T)digits[2]) << PyLong_SHIFT) | (ZMQ_FD_T)digits[1]) << PyLong_SHIFT) | (ZMQ_FD_T)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_poll.pyx` & `pyzmq-25.1.0/zmq/backend/cython/_poll.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_proxy_steerable.c` & `pyzmq-25.1.0/zmq/backend/cython/_proxy_steerable.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,24 +93,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -218,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -567,35 +571,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1290,26 +1294,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1383,22 +1387,30 @@
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -2605,15 +2617,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -2661,43 +2673,38 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(5, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(5, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(6, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(6, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -2883,15 +2890,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__backend__cython___proxy_steerable) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -3998,84 +4005,102 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -4637,17 +4662,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -4714,15 +4744,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -4766,15 +4799,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -5151,15 +5184,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -5347,15 +5380,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_proxy_steerable.pyx` & `pyzmq-25.1.0/zmq/backend/cython/_proxy_steerable.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_version.c` & `pyzmq-25.1.0/zmq/backend/cython/_version.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/_version.pyx` & `pyzmq-25.1.0/zmq/backend/cython/_version.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/checkrc.pxd` & `pyzmq-25.1.0/zmq/backend/cython/checkrc.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/constant_enums.pxi` & `pyzmq-25.1.0/zmq/backend/cython/constant_enums.pxi`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/context.c` & `pyzmq-25.1.0/zmq/backend/cython/context.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/getpid_compat.h",
             "zmq/utils/pyversion_compat.h",
@@ -25,16 +25,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -94,24 +94,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -219,15 +223,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -258,15 +262,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -568,35 +572,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1162,26 +1166,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1350,22 +1354,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
@@ -3530,15 +3542,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -3735,15 +3747,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -3811,32 +3823,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -4021,15 +4030,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__backend__cython__context) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -4664,15 +4673,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -4902,28 +4911,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -5408,61 +5417,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -6004,17 +6031,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -6081,15 +6113,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -6133,15 +6168,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -6442,15 +6477,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6638,15 +6673,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -6910,15 +6945,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/backend/cython/context.pxd` & `pyzmq-25.1.0/zmq/backend/cython/context.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/context.pyx` & `pyzmq-25.1.0/zmq/backend/cython/context.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/error.c` & `pyzmq-25.1.0/zmq/backend/cython/error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -24,16 +24,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -93,24 +93,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -218,15 +222,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -257,15 +261,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -567,35 +571,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1579,15 +1583,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -1815,15 +1819,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__backend__cython__error) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -2524,17 +2528,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -2601,15 +2610,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -2703,15 +2715,15 @@
     tstate->curexc_value = 0;
     tstate->curexc_traceback = 0;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -3012,15 +3024,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -3284,15 +3296,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/backend/cython/error.pyx` & `pyzmq-25.1.0/zmq/backend/cython/error.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/libzmq.pxd` & `pyzmq-25.1.0/zmq/backend/cython/libzmq.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/message.c` & `pyzmq-25.1.0/zmq/backend/cython/message.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/mutex.h",
             "zmq/utils/pyversion_compat.h",
@@ -26,16 +26,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -95,24 +95,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -220,15 +224,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -259,15 +263,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -569,35 +573,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1195,26 +1199,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1404,22 +1408,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
@@ -7204,15 +7216,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_3zmq_7backend_6cython_7message_Frame __pyx_vtable_3zmq_7backend_6cython_7message_Frame;
 
 static PyObject *__pyx_tp_new_3zmq_7backend_6cython_7message_Frame(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_3zmq_7backend_6cython_7message_Frame *p;
@@ -7468,15 +7480,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -7734,15 +7746,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -7851,32 +7863,29 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8068,15 +8077,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__backend__cython__message) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -8854,28 +8863,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -9023,15 +9032,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -9233,17 +9242,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -9666,61 +9673,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -10392,17 +10417,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -10469,15 +10499,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -10521,15 +10554,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -10830,15 +10863,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -11026,15 +11059,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -11222,15 +11255,15 @@
                         } else if (8 * sizeof(pyzmq_uint32_t) >= 4 * PyLong_SHIFT) {
                             return (pyzmq_uint32_t) (((((((((pyzmq_uint32_t)digits[3]) << PyLong_SHIFT) | (pyzmq_uint32_t)digits[2]) << PyLong_SHIFT) | (pyzmq_uint32_t)digits[1]) << PyLong_SHIFT) | (pyzmq_uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -11532,15 +11565,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/backend/cython/message.pxd` & `pyzmq-25.1.0/zmq/backend/cython/message.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/message.pyx` & `pyzmq-25.1.0/zmq/backend/cython/message.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/socket.c` & `pyzmq-25.1.0/zmq/backend/cython/socket.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/getpid_compat.h",
             "zmq/utils/ipcmaxlen.h",
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -96,24 +96,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -221,15 +225,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -260,15 +264,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -570,35 +574,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1342,26 +1346,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1561,22 +1565,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -11205,15 +11217,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -11730,15 +11742,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -11814,45 +11826,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(7, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(7, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(8, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(8, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(9, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(9, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.message"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.message", "MessageTracker", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker) __PYX_ERR(4, 34, __pyx_L1_error)
-  __pyx_ptype_3zmq_7backend_6cython_7message_Frame = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.message", "Frame", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_Frame), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_7message_Frame) __PYX_ERR(4, 40, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.message", "MessageTracker", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7message_MessageTracker),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7message_MessageTracker) __PYX_ERR(4, 34, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7message_Frame = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.message", "Frame", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7message_Frame), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7message_Frame),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7message_Frame) __PYX_ERR(4, 40, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7message_Frame = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7message_Frame*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7message_Frame->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7message_Frame)) __PYX_ERR(4, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -12043,15 +12049,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__backend__cython__socket) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -13204,28 +13210,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -13644,15 +13650,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -13709,17 +13715,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -14014,61 +14018,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -14630,17 +14652,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -14707,15 +14734,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -14759,15 +14789,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -15106,15 +15136,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15302,15 +15332,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15498,15 +15528,15 @@
                         } else if (8 * sizeof(pyzmq_int64_t) >= 4 * PyLong_SHIFT) {
                             return (pyzmq_int64_t) (((((((((pyzmq_int64_t)digits[3]) << PyLong_SHIFT) | (pyzmq_int64_t)digits[2]) << PyLong_SHIFT) | (pyzmq_int64_t)digits[1]) << PyLong_SHIFT) | (pyzmq_int64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -15808,15 +15838,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/backend/cython/socket.pxd` & `pyzmq-25.1.0/zmq/backend/cython/socket.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/socket.pyx` & `pyzmq-25.1.0/zmq/backend/cython/socket.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/utils.c` & `pyzmq-25.1.0/zmq/backend/cython/utils.c`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/cython/utils.pyx` & `pyzmq-25.1.0/zmq/backend/cython/utils.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/backend/select.py` & `pyzmq-25.1.0/zmq/backend/select.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/constants.py` & `pyzmq-25.1.0/zmq/constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/decorators.py` & `pyzmq-25.1.0/zmq/decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/__init__.py` & `pyzmq-25.1.0/zmq/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/basedevice.py` & `pyzmq-25.1.0/zmq/devices/basedevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/monitoredqueue.c` & `pyzmq-25.1.0/zmq/devices/monitoredqueue.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "zmq/utils/pyversion_compat.h",
             "zmq/utils/zmq_compat.h"
@@ -25,16 +25,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -94,24 +94,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -219,15 +223,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -258,15 +262,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -568,35 +572,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1227,26 +1231,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1385,22 +1389,30 @@
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
@@ -4634,15 +4646,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
@@ -4690,43 +4702,38 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_7context_Context = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.context", "Context", sizeof(struct __pyx_obj_3zmq_7backend_6cython_7context_Context), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_7context_Context),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_7context_Context) __PYX_ERR(6, 26, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_7context_Context = (struct __pyx_vtabstruct_3zmq_7backend_6cython_7context_Context*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_7context_Context->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_7context_Context)) __PYX_ERR(6, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("zmq.backend.cython.socket"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(7, 33, __pyx_L1_error)
+  __pyx_ptype_3zmq_7backend_6cython_6socket_Socket = __Pyx_ImportType_0_29_35(__pyx_t_1, "zmq.backend.cython.socket", "Socket", sizeof(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_3zmq_7backend_6cython_6socket_Socket),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_3zmq_7backend_6cython_6socket_Socket) __PYX_ERR(7, 33, __pyx_L1_error)
   __pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket = (struct __pyx_vtabstruct_3zmq_7backend_6cython_6socket_Socket*)__Pyx_GetVtable(__pyx_ptype_3zmq_7backend_6cython_6socket_Socket->tp_dict); if (unlikely(!__pyx_vtabptr_3zmq_7backend_6cython_6socket_Socket)) __PYX_ERR(7, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -4912,15 +4919,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_zmq__devices__monitoredqueue) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -6055,84 +6062,102 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -6694,17 +6719,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -6771,15 +6801,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -6823,15 +6856,15 @@
         PyObject_GC_Track(op);
     }
     return op;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -7208,15 +7241,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -7404,15 +7437,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pyzmq-25.0.2/zmq/devices/monitoredqueue.pxd` & `pyzmq-25.1.0/zmq/devices/monitoredqueue.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/monitoredqueue.py` & `pyzmq-25.1.0/zmq/devices/monitoredqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/monitoredqueue.pyx` & `pyzmq-25.1.0/zmq/devices/monitoredqueue.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/monitoredqueuedevice.py` & `pyzmq-25.1.0/zmq/devices/monitoredqueuedevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/proxydevice.py` & `pyzmq-25.1.0/zmq/devices/proxydevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/devices/proxysteerabledevice.py` & `pyzmq-25.1.0/zmq/devices/proxysteerabledevice.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/error.py` & `pyzmq-25.1.0/zmq/error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/eventloop/_deprecated.py` & `pyzmq-25.1.0/zmq/eventloop/_deprecated.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/eventloop/future.py` & `pyzmq-25.1.0/zmq/eventloop/future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/eventloop/ioloop.py` & `pyzmq-25.1.0/zmq/eventloop/ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/eventloop/zmqstream.py` & `pyzmq-25.1.0/zmq/eventloop/zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/green/__init__.py` & `pyzmq-25.1.0/zmq/green/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/green/core.py` & `pyzmq-25.1.0/zmq/green/core.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/green/device.py` & `pyzmq-25.1.0/zmq/green/device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/green/poll.py` & `pyzmq-25.1.0/zmq/green/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/log/__main__.py` & `pyzmq-25.1.0/zmq/log/__main__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/log/handlers.py` & `pyzmq-25.1.0/zmq/log/handlers.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/ssh/forward.py` & `pyzmq-25.1.0/zmq/ssh/forward.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/ssh/tunnel.py` & `pyzmq-25.1.0/zmq/ssh/tunnel.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/__init__.py` & `pyzmq-25.1.0/zmq/sugar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/attrsettr.py` & `pyzmq-25.1.0/zmq/sugar/attrsettr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/context.py` & `pyzmq-25.1.0/zmq/sugar/context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/frame.py` & `pyzmq-25.1.0/zmq/sugar/frame.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/poll.py` & `pyzmq-25.1.0/zmq/sugar/poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/socket.py` & `pyzmq-25.1.0/zmq/sugar/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,19 @@
         addr : str
             The address string. This has the form 'protocol://interface:port',
             for example 'tcp://127.0.0.1:5555'. Protocols supported include
             tcp, udp, pgm, epgm, inproc and ipc. If the address is unicode, it is
             encoded to utf-8 first.
 
         """
-        super().bind(addr)
+        try:
+            super().bind(addr)
+        except ZMQError as e:
+            e.strerror += f" (addr={addr!r})"
+            raise
         return self._bind_cm(addr)
 
     def connect(self: T, addr: str) -> _SocketContext[T]:
         """s.connect(addr)
 
         Connect to a remote 0MQ socket.
 
@@ -316,15 +320,19 @@
         addr : str
             The address string. This has the form 'protocol://interface:port',
             for example 'tcp://127.0.0.1:5555'. Protocols supported are
             tcp, udp, pgm, inproc and ipc. If the address is unicode, it is
             encoded to utf-8 first.
 
         """
-        super().connect(addr)
+        try:
+            super().connect(addr)
+        except ZMQError as e:
+            e.strerror += f" (addr={addr!r})"
+            raise
         return self._connect_cm(addr)
 
     # -------------------------------------------------------------------------
     # Deprecated aliases
     # -------------------------------------------------------------------------
 
     @property
```

### Comparing `pyzmq-25.0.2/zmq/sugar/stopwatch.py` & `pyzmq-25.1.0/zmq/sugar/stopwatch.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/tracker.py` & `pyzmq-25.1.0/zmq/sugar/tracker.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/sugar/version.py` & `pyzmq-25.1.0/zmq/sugar/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Distributed under the terms of the Modified BSD License.
 
 import re
 from typing import Match, Tuple, Union, cast
 
 from zmq.backend import zmq_version_info
 
-__version__: str = "25.0.2"
+__version__: str = "25.1.0"
 _version_pat = re.compile(r"(\d+)\.(\d+)\.(\d+)(.*)")
 _match = cast(Match, _version_pat.match(__version__))
 _version_groups = _match.groups()
 
 VERSION_MAJOR = int(_version_groups[0])
 VERSION_MINOR = int(_version_groups[1])
 VERSION_PATCH = int(_version_groups[2])
```

### Comparing `pyzmq-25.0.2/zmq/tests/__init__.py` & `pyzmq-25.1.0/zmq/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/conftest.py` & `pyzmq-25.1.0/zmq/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/cython_ext.pyx` & `pyzmq-25.1.0/zmq/tests/cython_ext.pyx`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_asyncio.py` & `pyzmq-25.1.0/zmq/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_auth.py` & `pyzmq-25.1.0/zmq/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_cffi_backend.py` & `pyzmq-25.1.0/zmq/tests/test_cffi_backend.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_constants.py` & `pyzmq-25.1.0/zmq/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_context.py` & `pyzmq-25.1.0/zmq/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_cython.py` & `pyzmq-25.1.0/zmq/tests/test_cython.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import sys
 
 import pytest
 
 import zmq
 
+pyximport = pytest.importorskip("pyximport")
+
 HERE = os.path.dirname(__file__)
 cython_ext = os.path.join(HERE, "cython_ext.pyx")
 
 
 @pytest.mark.skipif(
     not os.path.exists(cython_ext),
     reason=f"Requires cython test file {cython_ext}",
@@ -17,16 +19,14 @@
     'zmq.backend.cython' not in sys.modules, reason="Requires cython backend"
 )
 @pytest.mark.skipif(
     sys.platform.startswith('win'), reason="Don't try runtime Cython on Windows"
 )
 @pytest.mark.parametrize('language_level', [3, 2])
 def test_cython(language_level, request, tmpdir):
-    import pyximport
-
     assert 'zmq.tests.cython_ext' not in sys.modules
 
     importers = pyximport.install(
         setup_args=dict(include_dirs=zmq.get_includes()),
         language_level=language_level,
         build_dir=str(tmpdir),
     )
```

### Comparing `pyzmq-25.0.2/zmq/tests/test_decorators.py` & `pyzmq-25.1.0/zmq/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_device.py` & `pyzmq-25.1.0/zmq/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_draft.py` & `pyzmq-25.1.0/zmq/tests/test_draft.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_error.py` & `pyzmq-25.1.0/zmq/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_etc.py` & `pyzmq-25.1.0/zmq/tests/test_etc.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_ext.py` & `pyzmq-25.1.0/zmq/tests/test_ext.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_future.py` & `pyzmq-25.1.0/zmq/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_imports.py` & `pyzmq-25.1.0/zmq/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_includes.py` & `pyzmq-25.1.0/zmq/tests/test_includes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_ioloop.py` & `pyzmq-25.1.0/zmq/tests/test_ioloop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_log.py` & `pyzmq-25.1.0/zmq/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_message.py` & `pyzmq-25.1.0/zmq/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_monitor.py` & `pyzmq-25.1.0/zmq/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_monqueue.py` & `pyzmq-25.1.0/zmq/tests/test_monqueue.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_multipart.py` & `pyzmq-25.1.0/zmq/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_mypy.py` & `pyzmq-25.1.0/zmq/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_pair.py` & `pyzmq-25.1.0/zmq/tests/test_pair.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_poll.py` & `pyzmq-25.1.0/zmq/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_proxy_steerable.py` & `pyzmq-25.1.0/zmq/tests/test_proxy_steerable.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_pubsub.py` & `pyzmq-25.1.0/zmq/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_reqrep.py` & `pyzmq-25.1.0/zmq/tests/test_reqrep.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_retry_eintr.py` & `pyzmq-25.1.0/zmq/tests/test_retry_eintr.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_security.py` & `pyzmq-25.1.0/zmq/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_socket.py` & `pyzmq-25.1.0/zmq/tests/test_socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,26 @@
             s.bind_to_random_port('rand://*')
         except zmq.ZMQError as e:
             assert e.errno == zmq.EPROTONOSUPPORT
 
         s.close()
         ctx.term()
 
+    def test_bind_connect_addr_error(self):
+        with self.socket(zmq.PUSH) as s:
+            url = "tcp://1.2.3.4.5:1234567"
+            with pytest.raises(zmq.ZMQError) as exc:
+                s.bind(url)
+            assert url in str(exc.value)
+
+            url = "noproc://no/such/file"
+            with pytest.raises(zmq.ZMQError) as exc:
+                s.connect(url)
+            assert url in str(exc.value)
+
     def test_identity(self):
         s = self.context.socket(zmq.PULL)
         self.sockets.append(s)
         ident = b'identity\0\0'
         s.identity = ident
         assert s.get(zmq.IDENTITY) == ident
```

### Comparing `pyzmq-25.0.2/zmq/tests/test_version.py` & `pyzmq-25.1.0/zmq/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_win32_shim.py` & `pyzmq-25.1.0/zmq/tests/test_win32_shim.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_z85.py` & `pyzmq-25.1.0/zmq/tests/test_z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/tests/test_zmqstream.py` & `pyzmq-25.1.0/zmq/tests/test_zmqstream.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/buffers.pxd` & `pyzmq-25.1.0/zmq/utils/buffers.pxd`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/garbage.py` & `pyzmq-25.1.0/zmq/utils/garbage.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/interop.py` & `pyzmq-25.1.0/zmq/utils/interop.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/ipcmaxlen.h` & `pyzmq-25.1.0/zmq/utils/ipcmaxlen.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/jsonapi.py` & `pyzmq-25.1.0/zmq/utils/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/monitor.py` & `pyzmq-25.1.0/zmq/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/mutex.h` & `pyzmq-25.1.0/zmq/utils/mutex.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/strtypes.py` & `pyzmq-25.1.0/zmq/utils/strtypes.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/win32.py` & `pyzmq-25.1.0/zmq/utils/win32.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/z85.py` & `pyzmq-25.1.0/zmq/utils/z85.py`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmq/utils/zmq_compat.h` & `pyzmq-25.1.0/zmq/utils/zmq_compat.h`

 * *Files identical despite different names*

### Comparing `pyzmq-25.0.2/zmqversion.py` & `pyzmq-25.1.0/zmqversion.py`

 * *Files identical despite different names*

