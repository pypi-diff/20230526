# Comparing `tmp/yins-music-0.0.7.dev2.tar.gz` & `tmp/yins-music-0.0.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yins-music-0.0.7.dev2.tar", last modified: Fri May 26 05:43:06 2023, max compression
+gzip compressed data, was "yins-music-0.0.7.dev3.tar", last modified: Fri May 26 05:51:12 2023, max compression
```

## Comparing `yins-music-0.0.7.dev2.tar` & `yins-music-0.0.7.dev3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/dispatcher/dispatcher_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/group_call_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/group_call_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/implementation/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_native.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/mtproto/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/base_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/base_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_discarded_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_participant_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/update_group_call_participants_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/update_group_call_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/fipper_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7954 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto/telethon_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/mtproto_client_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/pytgcalls/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-26 05:42:53.000000 yins-music-0.0.7.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 05:43:06.264225 yins-music-0.0.7.dev2/yins_music.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 05:43:06.000000 yins-music-0.0.7.dev2/yins_music.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:12.121978 yins-music-0.0.7.dev3/
+-rw-rw-rw-   0        0        0     7815 2023-05-20 07:52:21.000000 yins-music-0.0.7.dev3/LICENSE
+-rw-rw-rw-   0        0        0       15 2023-05-20 07:52:21.000000 yins-music-0.0.7.dev3/MANIFEST.in
+-rw-rw-rw-   0        0        0    12231 2023-05-26 05:51:12.120978 yins-music-0.0.7.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0    10043 2023-05-20 07:52:21.000000 yins-music-0.0.7.dev3/README.md
+-rw-rw-rw-   0        0        0      292 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:11.721220 yins-music-0.0.7.dev3/pytgcalls/
+-rw-rw-rw-   0        0        0     1415 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:11.773194 yins-music-0.0.7.dev3/pytgcalls/dispatcher/
+-rw-rw-rw-   0        0        0     1197 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/dispatcher/__init__.py
+-rw-rw-rw-   0        0        0     1104 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/dispatcher/action.py
+-rw-rw-rw-   0        0        0     3402 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/dispatcher/dispatcher.py
+-rw-rw-rw-   0        0        0     2413 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/dispatcher/dispatcher_mixin.py
+-rw-rw-rw-   0        0        0     1260 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/exceptions.py
+-rw-rw-rw-   0        0        0     5519 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/group_call_factory.py
+-rw-rw-rw-   0        0        0     1064 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/group_call_type.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:11.878128 yins-music-0.0.7.dev3/pytgcalls/implementation/
+-rw-rw-rw-   0        0        0     1653 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/implementation/__init__.py
+-rw-rw-rw-   0        0        0     9852 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/implementation/group_call.py
+-rw-rw-rw-   0        0        0    16924 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/implementation/group_call_base.py
+-rw-rw-rw-   0        0        0     2614 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/implementation/group_call_device.py
+-rw-rw-rw-   0        0        0     5506 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/implementation/group_call_file.py
+-rw-rw-rw-   0        0        0     7401 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/implementation/group_call_native.py
+-rw-rw-rw-   0        0        0     4292 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/implementation/group_call_raw.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:11.941089 yins-music-0.0.7.dev3/pytgcalls/mtproto/
+-rw-rw-rw-   0        0        0     1055 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/__init__.py
+-rw-rw-rw-   0        0        0     5067 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/base_bridge.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:12.004051 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/
+-rw-rw-rw-   0        0        0     1314 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/__init__.py
+-rw-rw-rw-   0        0        0     1141 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/base_wrapper.py
+-rw-rw-rw-   0        0        0     1088 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/group_call_discarded_wrapper.py
+-rw-rw-rw-   0        0        0     4055 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/group_call_participant_wrapper.py
+-rw-rw-rw-   0        0        0     1191 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/group_call_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:12.041031 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/update/
+-rw-rw-rw-   0        0        0     1193 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/update/__init__.py
+-rw-rw-rw-   0        0        0     1307 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/update/update_group_call_participants_wrapper.py
+-rw-rw-rw-   0        0        0     1353 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/data/update/update_group_call_wrapper.py
+-rw-rw-rw-   0        0        0     1052 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/exceptions.py
+-rw-rw-rw-   0        0        0     9307 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/fipper_bridge.py
+-rw-rw-rw-   0        0        0     8162 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto/telethon_bridge.py
+-rw-rw-rw-   0        0        0     1059 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/mtproto_client_type.py
+-rw-rw-rw-   0        0        0     9958 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/pytgcalls/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 05:51:12.121978 yins-music-0.0.7.dev3/setup.cfg
+-rw-rw-rw-   0        0        0     3899 2023-05-26 05:49:58.000000 yins-music-0.0.7.dev3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:51:12.118981 yins-music-0.0.7.dev3/yins_music.egg-info/
+-rw-rw-rw-   0        0        0    12231 2023-05-26 05:51:11.000000 yins-music-0.0.7.dev3/yins_music.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1391 2023-05-26 05:51:11.000000 yins-music-0.0.7.dev3/yins_music.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 05:51:11.000000 yins-music-0.0.7.dev3/yins_music.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-26 05:51:11.000000 yins-music-0.0.7.dev3/yins_music.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 05:51:11.000000 yins-music-0.0.7.dev3/yins_music.egg-info/top_level.txt
```

### Comparing `yins-music-0.0.7.dev2/LICENSE` & `yins-music-0.0.7.dev3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-                   GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-
-  This version of the GNU Lesser General Public License incorporates
-the terms and conditions of version 3 of the GNU General Public
-License, supplemented by the additional permissions listed below.
-
-  0. Additional Definitions.
-
-  As used herein, "this License" refers to version 3 of the GNU Lesser
-General Public License, and the "GNU GPL" refers to version 3 of the GNU
-General Public License.
-
-  "The Library" refers to a covered work governed by this License,
-other than an Application or a Combined Work as defined below.
-
-  An "Application" is any work that makes use of an interface provided
-by the Library, but which is not otherwise based on the Library.
-Defining a subclass of a class defined by the Library is deemed a mode
-of using an interface provided by the Library.
-
-  A "Combined Work" is a work produced by combining or linking an
-Application with the Library.  The particular version of the Library
-with which the Combined Work was made is also called the "Linked
-Version".
-
-  The "Minimal Corresponding Source" for a Combined Work means the
-Corresponding Source for the Combined Work, excluding any source code
-for portions of the Combined Work that, considered in isolation, are
-based on the Application, and not on the Linked Version.
-
-  The "Corresponding Application Code" for a Combined Work means the
-object code and/or source code for the Application, including any data
-and utility programs needed for reproducing the Combined Work from the
-Application, but excluding the System Libraries of the Combined Work.
-
-  1. Exception to Section 3 of the GNU GPL.
-
-  You may convey a covered work under sections 3 and 4 of this License
-without being bound by section 3 of the GNU GPL.
-
-  2. Conveying Modified Versions.
-
-  If you modify a copy of the Library, and, in your modifications, a
-facility refers to a function or data to be supplied by an Application
-that uses the facility (other than as an argument passed when the
-facility is invoked), then you may convey a copy of the modified
-version:
-
-   a) under this License, provided that you make a good faith effort to
-   ensure that, in the event an Application does not supply the
-   function or data, the facility still operates, and performs
-   whatever part of its purpose remains meaningful, or
-
-   b) under the GNU GPL, with none of the additional permissions of
-   this License applicable to that copy.
-
-  3. Object Code Incorporating Material from Library Header Files.
-
-  The object code form of an Application may incorporate material from
-a header file that is part of the Library.  You may convey such object
-code under terms of your choice, provided that, if the incorporated
-material is not limited to numerical parameters, data structure
-layouts and accessors, or small macros, inline functions and templates
-(ten or fewer lines in length), you do both of the following:
-
-   a) Give prominent notice with each copy of the object code that the
-   Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the object code with a copy of the GNU GPL and this license
-   document.
-
-  4. Combined Works.
-
-  You may convey a Combined Work under terms of your choice that,
-taken together, effectively do not restrict modification of the
-portions of the Library contained in the Combined Work and reverse
-engineering for debugging such modifications, if you also do each of
-the following:
-
-   a) Give prominent notice with each copy of the Combined Work that
-   the Library is used in it and that the Library and its use are
-   covered by this License.
-
-   b) Accompany the Combined Work with a copy of the GNU GPL and this license
-   document.
-
-   c) For a Combined Work that displays copyright notices during
-   execution, include the copyright notice for the Library among
-   these notices, as well as a reference directing the user to the
-   copies of the GNU GPL and this license document.
-
-   d) Do one of the following:
-
-       0) Convey the Minimal Corresponding Source under the terms of this
-       License, and the Corresponding Application Code in a form
-       suitable for, and under terms that permit, the user to
-       recombine or relink the Application with a modified version of
-       the Linked Version to produce a modified Combined Work, in the
-       manner specified by section 6 of the GNU GPL for conveying
-       Corresponding Source.
-
-       1) Use a suitable shared library mechanism for linking with the
-       Library.  A suitable mechanism is one that (a) uses at run time
-       a copy of the Library already present on the user's computer
-       system, and (b) will operate properly with a modified version
-       of the Library that is interface-compatible with the Linked
-       Version.
-
-   e) Provide Installation Information, but only if you would otherwise
-   be required to provide such information under section 6 of the
-   GNU GPL, and only to the extent that such information is
-   necessary to install and execute a modified version of the
-   Combined Work produced by recombining or relinking the
-   Application with a modified version of the Linked Version. (If
-   you use option 4d0, the Installation Information must accompany
-   the Minimal Corresponding Source and Corresponding Application
-   Code. If you use option 4d1, you must provide the Installation
-   Information in the manner specified by section 6 of the GNU GPL
-   for conveying Corresponding Source.)
-
-  5. Combined Libraries.
-
-  You may place library facilities that are a work based on the
-Library side by side in a single library together with other library
-facilities that are not Applications and are not covered by this
-License, and convey such a combined library under terms of your
-choice, if you do both of the following:
-
-   a) Accompany the combined library with a copy of the same work based
-   on the Library, uncombined with any other library facilities,
-   conveyed under the terms of this License.
-
-   b) Give prominent notice with the combined library that part of it
-   is a work based on the Library, and explaining where to find the
-   accompanying uncombined form of the same work.
-
-  6. Revised Versions of the GNU Lesser General Public License.
-
-  The Free Software Foundation may publish revised and/or new versions
-of the GNU Lesser General Public License from time to time. Such new
-versions will be similar in spirit to the present version, but may
-differ in detail to address new problems or concerns.
-
-  Each version is given a distinguishing version number. If the
-Library as you received it specifies that a certain numbered version
-of the GNU Lesser General Public License "or any later version"
-applies to it, you have the option of following the terms and
-conditions either of that published version or of any later version
-published by the Free Software Foundation. If the Library as you
-received it does not specify a version number of the GNU Lesser
-General Public License, you may choose any version of the GNU Lesser
-General Public License ever published by the Free Software Foundation.
-
-  If the Library as you received it specifies that a proxy can decide
-whether future versions of the GNU Lesser General Public License shall
-apply, that proxy's public statement of acceptance of any version is
-permanent authorization for you to choose that version for the
+                   GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+
+  This version of the GNU Lesser General Public License incorporates
+the terms and conditions of version 3 of the GNU General Public
+License, supplemented by the additional permissions listed below.
+
+  0. Additional Definitions.
+
+  As used herein, "this License" refers to version 3 of the GNU Lesser
+General Public License, and the "GNU GPL" refers to version 3 of the GNU
+General Public License.
+
+  "The Library" refers to a covered work governed by this License,
+other than an Application or a Combined Work as defined below.
+
+  An "Application" is any work that makes use of an interface provided
+by the Library, but which is not otherwise based on the Library.
+Defining a subclass of a class defined by the Library is deemed a mode
+of using an interface provided by the Library.
+
+  A "Combined Work" is a work produced by combining or linking an
+Application with the Library.  The particular version of the Library
+with which the Combined Work was made is also called the "Linked
+Version".
+
+  The "Minimal Corresponding Source" for a Combined Work means the
+Corresponding Source for the Combined Work, excluding any source code
+for portions of the Combined Work that, considered in isolation, are
+based on the Application, and not on the Linked Version.
+
+  The "Corresponding Application Code" for a Combined Work means the
+object code and/or source code for the Application, including any data
+and utility programs needed for reproducing the Combined Work from the
+Application, but excluding the System Libraries of the Combined Work.
+
+  1. Exception to Section 3 of the GNU GPL.
+
+  You may convey a covered work under sections 3 and 4 of this License
+without being bound by section 3 of the GNU GPL.
+
+  2. Conveying Modified Versions.
+
+  If you modify a copy of the Library, and, in your modifications, a
+facility refers to a function or data to be supplied by an Application
+that uses the facility (other than as an argument passed when the
+facility is invoked), then you may convey a copy of the modified
+version:
+
+   a) under this License, provided that you make a good faith effort to
+   ensure that, in the event an Application does not supply the
+   function or data, the facility still operates, and performs
+   whatever part of its purpose remains meaningful, or
+
+   b) under the GNU GPL, with none of the additional permissions of
+   this License applicable to that copy.
+
+  3. Object Code Incorporating Material from Library Header Files.
+
+  The object code form of an Application may incorporate material from
+a header file that is part of the Library.  You may convey such object
+code under terms of your choice, provided that, if the incorporated
+material is not limited to numerical parameters, data structure
+layouts and accessors, or small macros, inline functions and templates
+(ten or fewer lines in length), you do both of the following:
+
+   a) Give prominent notice with each copy of the object code that the
+   Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the object code with a copy of the GNU GPL and this license
+   document.
+
+  4. Combined Works.
+
+  You may convey a Combined Work under terms of your choice that,
+taken together, effectively do not restrict modification of the
+portions of the Library contained in the Combined Work and reverse
+engineering for debugging such modifications, if you also do each of
+the following:
+
+   a) Give prominent notice with each copy of the Combined Work that
+   the Library is used in it and that the Library and its use are
+   covered by this License.
+
+   b) Accompany the Combined Work with a copy of the GNU GPL and this license
+   document.
+
+   c) For a Combined Work that displays copyright notices during
+   execution, include the copyright notice for the Library among
+   these notices, as well as a reference directing the user to the
+   copies of the GNU GPL and this license document.
+
+   d) Do one of the following:
+
+       0) Convey the Minimal Corresponding Source under the terms of this
+       License, and the Corresponding Application Code in a form
+       suitable for, and under terms that permit, the user to
+       recombine or relink the Application with a modified version of
+       the Linked Version to produce a modified Combined Work, in the
+       manner specified by section 6 of the GNU GPL for conveying
+       Corresponding Source.
+
+       1) Use a suitable shared library mechanism for linking with the
+       Library.  A suitable mechanism is one that (a) uses at run time
+       a copy of the Library already present on the user's computer
+       system, and (b) will operate properly with a modified version
+       of the Library that is interface-compatible with the Linked
+       Version.
+
+   e) Provide Installation Information, but only if you would otherwise
+   be required to provide such information under section 6 of the
+   GNU GPL, and only to the extent that such information is
+   necessary to install and execute a modified version of the
+   Combined Work produced by recombining or relinking the
+   Application with a modified version of the Linked Version. (If
+   you use option 4d0, the Installation Information must accompany
+   the Minimal Corresponding Source and Corresponding Application
+   Code. If you use option 4d1, you must provide the Installation
+   Information in the manner specified by section 6 of the GNU GPL
+   for conveying Corresponding Source.)
+
+  5. Combined Libraries.
+
+  You may place library facilities that are a work based on the
+Library side by side in a single library together with other library
+facilities that are not Applications and are not covered by this
+License, and convey such a combined library under terms of your
+choice, if you do both of the following:
+
+   a) Accompany the combined library with a copy of the same work based
+   on the Library, uncombined with any other library facilities,
+   conveyed under the terms of this License.
+
+   b) Give prominent notice with the combined library that part of it
+   is a work based on the Library, and explaining where to find the
+   accompanying uncombined form of the same work.
+
+  6. Revised Versions of the GNU Lesser General Public License.
+
+  The Free Software Foundation may publish revised and/or new versions
+of the GNU Lesser General Public License from time to time. Such new
+versions will be similar in spirit to the present version, but may
+differ in detail to address new problems or concerns.
+
+  Each version is given a distinguishing version number. If the
+Library as you received it specifies that a certain numbered version
+of the GNU Lesser General Public License "or any later version"
+applies to it, you have the option of following the terms and
+conditions either of that published version or of any later version
+published by the Free Software Foundation. If the Library as you
+received it does not specify a version number of the GNU Lesser
+General Public License, you may choose any version of the GNU Lesser
+General Public License ever published by the Free Software Foundation.
+
+  If the Library as you received it specifies that a proxy can decide
+whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is
+permanent authorization for you to choose that version for the
 Library.
```

### Comparing `yins-music-0.0.7.dev2/PKG-INFO` & `yins-music-0.0.7.dev3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-Metadata-Version: 2.1
-Name: yins-music
-Version: 0.0.7.dev2
-Summary: a library connecting the tgcalls Python binding with MTProto
-Home-page: https://github.com/MarshalX/tgcalls
-Author: AyiinXd
-Author-email: ayiinxd0307@gmail.com
-License: LGPLv3
-Project-URL: Documentation, https://tgcalls.org/
-Project-URL: Telegram Channel, https://t.me/tgcallslib
-Project-URL: Telegram Chat, https://t.me/tgcallschat
-Project-URL: Author, https://github.com/AyiinXd
-Keywords: python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Topic :: Internet
-Classifier: Topic :: Multimedia
-Classifier: Topic :: Multimedia :: Video
-Classifier: Topic :: Multimedia :: Video :: Capture
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
-Classifier: Topic :: Communications
-Classifier: Topic :: Communications :: Internet Phone
-Classifier: Topic :: Communications :: Telephony
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: fipper
-Provides-Extra: telethon
-License-File: LICENSE
-
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/logo.png" alt="tgcalls">
-    </a>
-    <br>
-    <b>Voice chats, private incoming and outgoing calls in Telegram for Developers</b>
-    <br>
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/examples">
-        Examples
-    </a>
-    •
-    <a href="https://tgcalls.org">
-        Documentation
-    </a>
-    •
-    <a href="https://t.me/tgcallslib">
-        Channel
-    </a>
-    •
-    <a href="https://t.me/tgcallschat">
-        Chat
-    </a>
-</p>
-
-## Telegram WebRTC (VoIP) [![Mentioned in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)
-
-This project consists of two main parts: [tgcalls](#tgcalls), [pytgcalls](#pytgcalls).
-The first is a C++ Python extension.
-The second uses the extension along with MTProto and provides high level SDK.
-All together, it allows you to create userbots that can record and
-broadcast in voice chats, make and receive private calls.
-
-#### Fipper's snippet
-```python
-from fipper import Client, filters
-from fipper.utils import MAX_CHANNEL_ID
-
-from pytgcalls import GroupCallFactory
-
-app = Client('pytgcalls')
-group_call = GroupCallFactory(app).get_file_group_call('input.raw')
-
-
-@group_call.on_network_status_changed
-async def on_network_changed(context, is_connected):
-    chat_id = MAX_CHANNEL_ID - context.full_chat.id
-    if is_connected:
-        await app.send_message(chat_id, 'Successfully joined!')
-    else:
-        await app.send_message(chat_id, 'Disconnected from voice chat..')
-
-
-@app.on_message(filters.outgoing & filters.command('join'))
-async def join_handler(_, message):
-    await group_call.start(message.chat.id)
-
-
-app.run()
-```
-
-#### Telethon's snippet
-```python
-from telethon import TelegramClient, events
-
-from pytgcalls import GroupCallFactory
-
-app = TelegramClient('pytgcalls', api_id, api_hash).start()
-group_call_factory = GroupCallFactory(app, GroupCallFactory.MTPROTO_CLIENT_TYPE.TELETHON)
-group_call = group_call_factory.get_file_group_call('input.raw')
-
-
-@app.on(events.NewMessage(outgoing=True, pattern=r'^/join$'))
-async def join_handler(event):
-    chat = await event.get_chat()
-    await group_call.start(chat.id)
-
-app.run_until_disconnected()
-```
-
-### Features
-
-- Python solution.
-- Prebuilt wheels for macOS, Linux and Windows.
-- Supporting popular MTProto libraries: Fipper, Telethon.
-- Abstract class to implement own MTProto bridge.
-- Work with voice chats in channels and chats.
-- Multiply voice chats ([example](https://github.com/MarshalX/tgcalls/blob/main/examples/radio_as_smart_plugin.py)).
-- System of custom handlers on events.
-- Join as channels or chats.
-- Join using invite (speaker) links.
-- Speaking status with voice activity detection.
-- Mute/unmute, pause/resume, stop/play, volume control and more...
-
-### Available sources of input/output data transfers
-
-- Raw (`GroupCallRaw`, [example with pyav](https://github.com/MarshalX/tgcalls/blob/main/examples/pyav.py),
-[example of restreaming](https://github.com/MarshalX/tgcalls/blob/main/examples/restream_using_raw_data.py))
-  — to send and receive data in `bytes` directly from Python.
-- File (`GroupCallFile`, [playout example](https://github.com/MarshalX/tgcalls/blob/main/examples/file_playout.py),
-  [recording example](https://github.com/MarshalX/tgcalls/blob/main/examples/recorder_as_smart_plugin.py))
-  — to use audio files including named pipe (FIFO).
-- Device (`GroupCallDevice`, [example](https://github.com/MarshalX/tgcalls/blob/main/examples/device_playout.py)) — 
-to use system virtual devices. Please don't use it with real microphone, headphones, etc.
-
-Note: All audio data is transmitted in PCM 16 bit, 48k. 
-[Example how to convert files using FFmpeg](#audio-file-formats).
-
-### Requirements
-
-- Python 3.7 or higher.
-- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).
-
-### TODO list
-- Incoming and Outgoing private calls 
-(already there and working, but not in the release version).
-- Group Video Calls
-[and more...](https://github.com/MarshalX/tgcalls/issues)
-
-### Installing
-
-#### For Fipper
-``` bash
-pip3 install -U pytgcalls[pyrogram]
-```
-
-#### For Telethon
-``` bash
-pip3 install -U pytgcalls[telethon]
-```
-
-<hr>
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/tgcalls.png" alt="tgcalls">
-    </a>
-    <br>
-    <a href="https://pypi.org/project/tgcalls/">
-        PyPi
-    </a>
-    •
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/tgcalls">
-        Sources
-    </a>
-</p>
-
-## tgcalls 
-
-The first part of the project is C++ extensions for Python. [Pybind11](https://github.com/pybind/pybind11)
-was used to write it. Binding occurs to the [tgcalls](https://github.com/TelegramMessenger/tgcalls)
-library by Telegram, which is used in all official clients. 
-To implement the binding, the code of Telegram Desktop and Telegram Android was studied.
-Changes have been made to the Telegram library. 
-All modified code is [available as a subtree](https://github.com/MarshalX/tgcalls/tree/main/tgcalls/third_party/lib_tgcalls)
-in this repository. The main ideas of the changes is to improve 
-the sound quality and to add ability to work with third party audio device modules.
-In addition, this binding implemented custom audio modules. These modules are allowing
-transfer audio data directly from Python via bytes, transfer and control 
-the playback/recording of a file or a virtual system device.
-
-### How to build
-
-Short answer for Linux:
-```bash
-git clone git@github.com:MarshalX/tgcalls.git --recursive
-cd tgcalls
-```
-For x86_64:
-```bash
-docker-compose up tgcalls_x86_64
-```
-For AArch64 (ARM64):
-```bash
-docker-compose up tgcalls_aarch64
-```
-
-Python wheels will be available in `dist` folder in root of `tgcalls`.
-
-More info:
-- [Manylinux](build/manylinux/dev).
-- [Ubuntu](build/ubuntu).
-- [macOS](build/macos).
-- [Windows](build/windows).
-
-Also, you can investigate into [manylinux GitHub Actions builds](build/manylinux).
-
-### Documentation
-
-Temporarily, instead of documentation, you can use [an example](pytgcalls/pytgcalls)
-along with MTProto.
-
-<hr>
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/pytgcalls.png" alt="pytgcalls">
-    </a>
-    <br>
-    <a href="https://tgcalls.org">
-        Documentation
-    </a>
-    •
-    <a href="https://pypi.org/project/pytgcalls/">
-        PyPi
-    </a>
-    •
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/pytgcalls">
-        Sources
-    </a>
-</p>
-
-## pytgcalls 
-
-This project is implementation of using [tgcalls](#tgcalls) 
-Python binding together with [MTProto](https://core.telegram.org/mtproto).
-By default, this library are supports [Fipper](https://github.com/pyrogram/pyrogram)
-and [Telethon](https://github.com/LonamiWebs/Telethon) clients for working 
-with Telegram Mobile Protocol. 
-You can write your own implementation of abstract class to work with other libraries.
-
-### Learning by example
-
-Visit [this page](https://github.com/MarshalX/tgcalls/tree/main/examples) to discover the official examples.
-
-### Documentation
-
-`pytgcalls`'s documentation lives at [tgcalls.org](https://tgcalls.org).
-
-### Audio file formats
-
-RAW files are now used. You will have to convert to this format yourself
-using ffmpeg. The example how to transcode files from a code is available [here](https://github.com/MarshalX/tgcalls/blob/e0b2d667728cc92cc0da437b9c85bcc909e4ac9c/examples/player_as_smart_plugin.py#L41).
-
-From mp3 to raw (to play in voice chat):
-```
-ffmpeg -i input.mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-From raw to mp3 (files with recordings):
-```
-ffmpeg -f s16le -ac 2 -ar 48000 -acodec pcm_s16le -i output.raw clear_output.mp3
-```
-
-For playout live stream you can use this one:
-```
-ffmpeg -y -i http://stream2.cnmns.net/hope-mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-For YouTube videos and live streams you can use youtube-dl:
-```
-ffmpeg -i "$(youtube-dl -x -g "https://youtu.be/xhXq9BNndhw")" -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-And set input.raw as input filename.
-
-<hr>
-
-### Getting help
-
-You can get help in several ways:
-- We have a community of developers helping each other in our 
-[Telegram group](https://t.me/tgcallschat).
-- Report bugs, request new features or ask questions by creating 
-[an issue](https://github.com/MarshalX/tgcalls/issues/new) or 
-[a discussion](https://github.com/MarshalX/tgcalls/discussions/new).
-
-### Contributing
-
-Contributions of all sizes are welcome.
-
-### Special thanks to
-
-- [@FrayxRulez](https://github.com/FrayxRulez) for amazing code of [Unigram](https://github.com/UnigramDev/Unigram).
-- [@john-preston](https://github.com/john-preston) for [Telegram Desktop](https://github.com/telegramdesktop/tdesktop) and [tgcalls](https://github.com/TelegramMessenger/tgcalls).
-- [@bakatrouble](https://github.com/bakatrouble/) for help and inspiration by [pytgvoip](https://github.com/bakatrouble/pytgvoip).
-- [@delivrance](https://github.com/delivrance) for [Fipper](https://github.com/pyrogram/pyrogram).
-- [@Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon).
-
-### License
-
-You may copy, distribute and modify the software provided that modifications
-are described and licensed for free under [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html).
-Derivatives works (including modifications or anything statically
-linked to the library) can only be redistributed under LGPL-3, but
-applications that use the library don't have to be.
+Metadata-Version: 2.1
+Name: yins-music
+Version: 0.0.7.dev3
+Summary: a library connecting the tgcalls Python binding with MTProto
+Home-page: https://github.com/MarshalX/tgcalls
+Author: AyiinXd
+Author-email: ayiinxd0307@gmail.com
+License: LGPLv3
+Project-URL: Documentation, https://tgcalls.org/
+Project-URL: Telegram Channel, https://t.me/tgcallslib
+Project-URL: Telegram Chat, https://t.me/tgcallschat
+Project-URL: Author, https://github.com/AyiinXd
+Keywords: python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Classifier: Topic :: Internet
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Video
+Classifier: Topic :: Multimedia :: Video :: Capture
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Internet Phone
+Classifier: Topic :: Communications :: Telephony
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: fipper
+Provides-Extra: telethon
+License-File: LICENSE
+
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/logo.png" alt="tgcalls">
+    </a>
+    <br>
+    <b>Voice chats, private incoming and outgoing calls in Telegram for Developers</b>
+    <br>
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/examples">
+        Examples
+    </a>
+    •
+    <a href="https://tgcalls.org">
+        Documentation
+    </a>
+    •
+    <a href="https://t.me/tgcallslib">
+        Channel
+    </a>
+    •
+    <a href="https://t.me/tgcallschat">
+        Chat
+    </a>
+</p>
+
+## Telegram WebRTC (VoIP) [![Mentioned in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)
+
+This project consists of two main parts: [tgcalls](#tgcalls), [pytgcalls](#pytgcalls).
+The first is a C++ Python extension.
+The second uses the extension along with MTProto and provides high level SDK.
+All together, it allows you to create userbots that can record and
+broadcast in voice chats, make and receive private calls.
+
+#### Fipper's snippet
+```python
+from fipper import Client, filters
+from fipper.utils import MAX_CHANNEL_ID
+
+from pytgcalls import GroupCallFactory
+
+app = Client('pytgcalls')
+group_call = GroupCallFactory(app).get_file_group_call('input.raw')
+
+
+@group_call.on_network_status_changed
+async def on_network_changed(context, is_connected):
+    chat_id = MAX_CHANNEL_ID - context.full_chat.id
+    if is_connected:
+        await app.send_message(chat_id, 'Successfully joined!')
+    else:
+        await app.send_message(chat_id, 'Disconnected from voice chat..')
+
+
+@app.on_message(filters.outgoing & filters.command('join'))
+async def join_handler(_, message):
+    await group_call.start(message.chat.id)
+
+
+app.run()
+```
+
+#### Telethon's snippet
+```python
+from telethon import TelegramClient, events
+
+from pytgcalls import GroupCallFactory
+
+app = TelegramClient('pytgcalls', api_id, api_hash).start()
+group_call_factory = GroupCallFactory(app, GroupCallFactory.MTPROTO_CLIENT_TYPE.TELETHON)
+group_call = group_call_factory.get_file_group_call('input.raw')
+
+
+@app.on(events.NewMessage(outgoing=True, pattern=r'^/join$'))
+async def join_handler(event):
+    chat = await event.get_chat()
+    await group_call.start(chat.id)
+
+app.run_until_disconnected()
+```
+
+### Features
+
+- Python solution.
+- Prebuilt wheels for macOS, Linux and Windows.
+- Supporting popular MTProto libraries: Fipper, Telethon.
+- Abstract class to implement own MTProto bridge.
+- Work with voice chats in channels and chats.
+- Multiply voice chats ([example](https://github.com/MarshalX/tgcalls/blob/main/examples/radio_as_smart_plugin.py)).
+- System of custom handlers on events.
+- Join as channels or chats.
+- Join using invite (speaker) links.
+- Speaking status with voice activity detection.
+- Mute/unmute, pause/resume, stop/play, volume control and more...
+
+### Available sources of input/output data transfers
+
+- Raw (`GroupCallRaw`, [example with pyav](https://github.com/MarshalX/tgcalls/blob/main/examples/pyav.py),
+[example of restreaming](https://github.com/MarshalX/tgcalls/blob/main/examples/restream_using_raw_data.py))
+  — to send and receive data in `bytes` directly from Python.
+- File (`GroupCallFile`, [playout example](https://github.com/MarshalX/tgcalls/blob/main/examples/file_playout.py),
+  [recording example](https://github.com/MarshalX/tgcalls/blob/main/examples/recorder_as_smart_plugin.py))
+  — to use audio files including named pipe (FIFO).
+- Device (`GroupCallDevice`, [example](https://github.com/MarshalX/tgcalls/blob/main/examples/device_playout.py)) — 
+to use system virtual devices. Please don't use it with real microphone, headphones, etc.
+
+Note: All audio data is transmitted in PCM 16 bit, 48k. 
+[Example how to convert files using FFmpeg](#audio-file-formats).
+
+### Requirements
+
+- Python 3.7 or higher.
+- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).
+
+### TODO list
+- Incoming and Outgoing private calls 
+(already there and working, but not in the release version).
+- Group Video Calls
+[and more...](https://github.com/MarshalX/tgcalls/issues)
+
+### Installing
+
+#### For Fipper
+``` bash
+pip3 install -U pytgcalls[pyrogram]
+```
+
+#### For Telethon
+``` bash
+pip3 install -U pytgcalls[telethon]
+```
+
+<hr>
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/tgcalls.png" alt="tgcalls">
+    </a>
+    <br>
+    <a href="https://pypi.org/project/tgcalls/">
+        PyPi
+    </a>
+    •
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/tgcalls">
+        Sources
+    </a>
+</p>
+
+## tgcalls 
+
+The first part of the project is C++ extensions for Python. [Pybind11](https://github.com/pybind/pybind11)
+was used to write it. Binding occurs to the [tgcalls](https://github.com/TelegramMessenger/tgcalls)
+library by Telegram, which is used in all official clients. 
+To implement the binding, the code of Telegram Desktop and Telegram Android was studied.
+Changes have been made to the Telegram library. 
+All modified code is [available as a subtree](https://github.com/MarshalX/tgcalls/tree/main/tgcalls/third_party/lib_tgcalls)
+in this repository. The main ideas of the changes is to improve 
+the sound quality and to add ability to work with third party audio device modules.
+In addition, this binding implemented custom audio modules. These modules are allowing
+transfer audio data directly from Python via bytes, transfer and control 
+the playback/recording of a file or a virtual system device.
+
+### How to build
+
+Short answer for Linux:
+```bash
+git clone git@github.com:MarshalX/tgcalls.git --recursive
+cd tgcalls
+```
+For x86_64:
+```bash
+docker-compose up tgcalls_x86_64
+```
+For AArch64 (ARM64):
+```bash
+docker-compose up tgcalls_aarch64
+```
+
+Python wheels will be available in `dist` folder in root of `tgcalls`.
+
+More info:
+- [Manylinux](build/manylinux/dev).
+- [Ubuntu](build/ubuntu).
+- [macOS](build/macos).
+- [Windows](build/windows).
+
+Also, you can investigate into [manylinux GitHub Actions builds](build/manylinux).
+
+### Documentation
+
+Temporarily, instead of documentation, you can use [an example](pytgcalls/pytgcalls)
+along with MTProto.
+
+<hr>
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/pytgcalls.png" alt="pytgcalls">
+    </a>
+    <br>
+    <a href="https://tgcalls.org">
+        Documentation
+    </a>
+    •
+    <a href="https://pypi.org/project/pytgcalls/">
+        PyPi
+    </a>
+    •
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/pytgcalls">
+        Sources
+    </a>
+</p>
+
+## pytgcalls 
+
+This project is implementation of using [tgcalls](#tgcalls) 
+Python binding together with [MTProto](https://core.telegram.org/mtproto).
+By default, this library are supports [Fipper](https://github.com/pyrogram/pyrogram)
+and [Telethon](https://github.com/LonamiWebs/Telethon) clients for working 
+with Telegram Mobile Protocol. 
+You can write your own implementation of abstract class to work with other libraries.
+
+### Learning by example
+
+Visit [this page](https://github.com/MarshalX/tgcalls/tree/main/examples) to discover the official examples.
+
+### Documentation
+
+`pytgcalls`'s documentation lives at [tgcalls.org](https://tgcalls.org).
+
+### Audio file formats
+
+RAW files are now used. You will have to convert to this format yourself
+using ffmpeg. The example how to transcode files from a code is available [here](https://github.com/MarshalX/tgcalls/blob/e0b2d667728cc92cc0da437b9c85bcc909e4ac9c/examples/player_as_smart_plugin.py#L41).
+
+From mp3 to raw (to play in voice chat):
+```
+ffmpeg -i input.mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+From raw to mp3 (files with recordings):
+```
+ffmpeg -f s16le -ac 2 -ar 48000 -acodec pcm_s16le -i output.raw clear_output.mp3
+```
+
+For playout live stream you can use this one:
+```
+ffmpeg -y -i http://stream2.cnmns.net/hope-mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+For YouTube videos and live streams you can use youtube-dl:
+```
+ffmpeg -i "$(youtube-dl -x -g "https://youtu.be/xhXq9BNndhw")" -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+And set input.raw as input filename.
+
+<hr>
+
+### Getting help
+
+You can get help in several ways:
+- We have a community of developers helping each other in our 
+[Telegram group](https://t.me/tgcallschat).
+- Report bugs, request new features or ask questions by creating 
+[an issue](https://github.com/MarshalX/tgcalls/issues/new) or 
+[a discussion](https://github.com/MarshalX/tgcalls/discussions/new).
+
+### Contributing
+
+Contributions of all sizes are welcome.
+
+### Special thanks to
+
+- [@FrayxRulez](https://github.com/FrayxRulez) for amazing code of [Unigram](https://github.com/UnigramDev/Unigram).
+- [@john-preston](https://github.com/john-preston) for [Telegram Desktop](https://github.com/telegramdesktop/tdesktop) and [tgcalls](https://github.com/TelegramMessenger/tgcalls).
+- [@bakatrouble](https://github.com/bakatrouble/) for help and inspiration by [pytgvoip](https://github.com/bakatrouble/pytgvoip).
+- [@delivrance](https://github.com/delivrance) for [Fipper](https://github.com/pyrogram/pyrogram).
+- [@Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon).
+
+### License
+
+You may copy, distribute and modify the software provided that modifications
+are described and licensed for free under [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html).
+Derivatives works (including modifications or anything statically
+linked to the library) can only be redistributed under LGPL-3, but
+applications that use the library don't have to be.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev2 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev3 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```

### Comparing `yins-music-0.0.7.dev2/README.md` & `yins-music-0.0.7.dev3/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/logo.png" alt="tgcalls">
-    </a>
-    <br>
-    <b>Voice chats, private incoming and outgoing calls in Telegram for Developers</b>
-    <br>
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/examples">
-        Examples
-    </a>
-    •
-    <a href="https://tgcalls.org">
-        Documentation
-    </a>
-    •
-    <a href="https://t.me/tgcallslib">
-        Channel
-    </a>
-    •
-    <a href="https://t.me/tgcallschat">
-        Chat
-    </a>
-</p>
-
-## Telegram WebRTC (VoIP) [![Mentioned in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)
-
-This project consists of two main parts: [tgcalls](#tgcalls), [pytgcalls](#pytgcalls).
-The first is a C++ Python extension.
-The second uses the extension along with MTProto and provides high level SDK.
-All together, it allows you to create userbots that can record and
-broadcast in voice chats, make and receive private calls.
-
-#### Fipper's snippet
-```python
-from fipper import Client, filters
-from fipper.utils import MAX_CHANNEL_ID
-
-from pytgcalls import GroupCallFactory
-
-app = Client('pytgcalls')
-group_call = GroupCallFactory(app).get_file_group_call('input.raw')
-
-
-@group_call.on_network_status_changed
-async def on_network_changed(context, is_connected):
-    chat_id = MAX_CHANNEL_ID - context.full_chat.id
-    if is_connected:
-        await app.send_message(chat_id, 'Successfully joined!')
-    else:
-        await app.send_message(chat_id, 'Disconnected from voice chat..')
-
-
-@app.on_message(filters.outgoing & filters.command('join'))
-async def join_handler(_, message):
-    await group_call.start(message.chat.id)
-
-
-app.run()
-```
-
-#### Telethon's snippet
-```python
-from telethon import TelegramClient, events
-
-from pytgcalls import GroupCallFactory
-
-app = TelegramClient('pytgcalls', api_id, api_hash).start()
-group_call_factory = GroupCallFactory(app, GroupCallFactory.MTPROTO_CLIENT_TYPE.TELETHON)
-group_call = group_call_factory.get_file_group_call('input.raw')
-
-
-@app.on(events.NewMessage(outgoing=True, pattern=r'^/join$'))
-async def join_handler(event):
-    chat = await event.get_chat()
-    await group_call.start(chat.id)
-
-app.run_until_disconnected()
-```
-
-### Features
-
-- Python solution.
-- Prebuilt wheels for macOS, Linux and Windows.
-- Supporting popular MTProto libraries: Fipper, Telethon.
-- Abstract class to implement own MTProto bridge.
-- Work with voice chats in channels and chats.
-- Multiply voice chats ([example](https://github.com/MarshalX/tgcalls/blob/main/examples/radio_as_smart_plugin.py)).
-- System of custom handlers on events.
-- Join as channels or chats.
-- Join using invite (speaker) links.
-- Speaking status with voice activity detection.
-- Mute/unmute, pause/resume, stop/play, volume control and more...
-
-### Available sources of input/output data transfers
-
-- Raw (`GroupCallRaw`, [example with pyav](https://github.com/MarshalX/tgcalls/blob/main/examples/pyav.py),
-[example of restreaming](https://github.com/MarshalX/tgcalls/blob/main/examples/restream_using_raw_data.py))
-  — to send and receive data in `bytes` directly from Python.
-- File (`GroupCallFile`, [playout example](https://github.com/MarshalX/tgcalls/blob/main/examples/file_playout.py),
-  [recording example](https://github.com/MarshalX/tgcalls/blob/main/examples/recorder_as_smart_plugin.py))
-  — to use audio files including named pipe (FIFO).
-- Device (`GroupCallDevice`, [example](https://github.com/MarshalX/tgcalls/blob/main/examples/device_playout.py)) — 
-to use system virtual devices. Please don't use it with real microphone, headphones, etc.
-
-Note: All audio data is transmitted in PCM 16 bit, 48k. 
-[Example how to convert files using FFmpeg](#audio-file-formats).
-
-### Requirements
-
-- Python 3.7 or higher.
-- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).
-
-### TODO list
-- Incoming and Outgoing private calls 
-(already there and working, but not in the release version).
-- Group Video Calls
-[and more...](https://github.com/MarshalX/tgcalls/issues)
-
-### Installing
-
-#### For Fipper
-``` bash
-pip3 install -U pytgcalls[pyrogram]
-```
-
-#### For Telethon
-``` bash
-pip3 install -U pytgcalls[telethon]
-```
-
-<hr>
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/tgcalls.png" alt="tgcalls">
-    </a>
-    <br>
-    <a href="https://pypi.org/project/tgcalls/">
-        PyPi
-    </a>
-    •
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/tgcalls">
-        Sources
-    </a>
-</p>
-
-## tgcalls 
-
-The first part of the project is C++ extensions for Python. [Pybind11](https://github.com/pybind/pybind11)
-was used to write it. Binding occurs to the [tgcalls](https://github.com/TelegramMessenger/tgcalls)
-library by Telegram, which is used in all official clients. 
-To implement the binding, the code of Telegram Desktop and Telegram Android was studied.
-Changes have been made to the Telegram library. 
-All modified code is [available as a subtree](https://github.com/MarshalX/tgcalls/tree/main/tgcalls/third_party/lib_tgcalls)
-in this repository. The main ideas of the changes is to improve 
-the sound quality and to add ability to work with third party audio device modules.
-In addition, this binding implemented custom audio modules. These modules are allowing
-transfer audio data directly from Python via bytes, transfer and control 
-the playback/recording of a file or a virtual system device.
-
-### How to build
-
-Short answer for Linux:
-```bash
-git clone git@github.com:MarshalX/tgcalls.git --recursive
-cd tgcalls
-```
-For x86_64:
-```bash
-docker-compose up tgcalls_x86_64
-```
-For AArch64 (ARM64):
-```bash
-docker-compose up tgcalls_aarch64
-```
-
-Python wheels will be available in `dist` folder in root of `tgcalls`.
-
-More info:
-- [Manylinux](build/manylinux/dev).
-- [Ubuntu](build/ubuntu).
-- [macOS](build/macos).
-- [Windows](build/windows).
-
-Also, you can investigate into [manylinux GitHub Actions builds](build/manylinux).
-
-### Documentation
-
-Temporarily, instead of documentation, you can use [an example](pytgcalls/pytgcalls)
-along with MTProto.
-
-<hr>
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/pytgcalls.png" alt="pytgcalls">
-    </a>
-    <br>
-    <a href="https://tgcalls.org">
-        Documentation
-    </a>
-    •
-    <a href="https://pypi.org/project/pytgcalls/">
-        PyPi
-    </a>
-    •
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/pytgcalls">
-        Sources
-    </a>
-</p>
-
-## pytgcalls 
-
-This project is implementation of using [tgcalls](#tgcalls) 
-Python binding together with [MTProto](https://core.telegram.org/mtproto).
-By default, this library are supports [Fipper](https://github.com/pyrogram/pyrogram)
-and [Telethon](https://github.com/LonamiWebs/Telethon) clients for working 
-with Telegram Mobile Protocol. 
-You can write your own implementation of abstract class to work with other libraries.
-
-### Learning by example
-
-Visit [this page](https://github.com/MarshalX/tgcalls/tree/main/examples) to discover the official examples.
-
-### Documentation
-
-`pytgcalls`'s documentation lives at [tgcalls.org](https://tgcalls.org).
-
-### Audio file formats
-
-RAW files are now used. You will have to convert to this format yourself
-using ffmpeg. The example how to transcode files from a code is available [here](https://github.com/MarshalX/tgcalls/blob/e0b2d667728cc92cc0da437b9c85bcc909e4ac9c/examples/player_as_smart_plugin.py#L41).
-
-From mp3 to raw (to play in voice chat):
-```
-ffmpeg -i input.mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-From raw to mp3 (files with recordings):
-```
-ffmpeg -f s16le -ac 2 -ar 48000 -acodec pcm_s16le -i output.raw clear_output.mp3
-```
-
-For playout live stream you can use this one:
-```
-ffmpeg -y -i http://stream2.cnmns.net/hope-mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-For YouTube videos and live streams you can use youtube-dl:
-```
-ffmpeg -i "$(youtube-dl -x -g "https://youtu.be/xhXq9BNndhw")" -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-And set input.raw as input filename.
-
-<hr>
-
-### Getting help
-
-You can get help in several ways:
-- We have a community of developers helping each other in our 
-[Telegram group](https://t.me/tgcallschat).
-- Report bugs, request new features or ask questions by creating 
-[an issue](https://github.com/MarshalX/tgcalls/issues/new) or 
-[a discussion](https://github.com/MarshalX/tgcalls/discussions/new).
-
-### Contributing
-
-Contributions of all sizes are welcome.
-
-### Special thanks to
-
-- [@FrayxRulez](https://github.com/FrayxRulez) for amazing code of [Unigram](https://github.com/UnigramDev/Unigram).
-- [@john-preston](https://github.com/john-preston) for [Telegram Desktop](https://github.com/telegramdesktop/tdesktop) and [tgcalls](https://github.com/TelegramMessenger/tgcalls).
-- [@bakatrouble](https://github.com/bakatrouble/) for help and inspiration by [pytgvoip](https://github.com/bakatrouble/pytgvoip).
-- [@delivrance](https://github.com/delivrance) for [Fipper](https://github.com/pyrogram/pyrogram).
-- [@Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon).
-
-### License
-
-You may copy, distribute and modify the software provided that modifications
-are described and licensed for free under [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html).
-Derivatives works (including modifications or anything statically
-linked to the library) can only be redistributed under LGPL-3, but
-applications that use the library don't have to be.
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/logo.png" alt="tgcalls">
+    </a>
+    <br>
+    <b>Voice chats, private incoming and outgoing calls in Telegram for Developers</b>
+    <br>
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/examples">
+        Examples
+    </a>
+    •
+    <a href="https://tgcalls.org">
+        Documentation
+    </a>
+    •
+    <a href="https://t.me/tgcallslib">
+        Channel
+    </a>
+    •
+    <a href="https://t.me/tgcallschat">
+        Chat
+    </a>
+</p>
+
+## Telegram WebRTC (VoIP) [![Mentioned in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)
+
+This project consists of two main parts: [tgcalls](#tgcalls), [pytgcalls](#pytgcalls).
+The first is a C++ Python extension.
+The second uses the extension along with MTProto and provides high level SDK.
+All together, it allows you to create userbots that can record and
+broadcast in voice chats, make and receive private calls.
+
+#### Fipper's snippet
+```python
+from fipper import Client, filters
+from fipper.utils import MAX_CHANNEL_ID
+
+from pytgcalls import GroupCallFactory
+
+app = Client('pytgcalls')
+group_call = GroupCallFactory(app).get_file_group_call('input.raw')
+
+
+@group_call.on_network_status_changed
+async def on_network_changed(context, is_connected):
+    chat_id = MAX_CHANNEL_ID - context.full_chat.id
+    if is_connected:
+        await app.send_message(chat_id, 'Successfully joined!')
+    else:
+        await app.send_message(chat_id, 'Disconnected from voice chat..')
+
+
+@app.on_message(filters.outgoing & filters.command('join'))
+async def join_handler(_, message):
+    await group_call.start(message.chat.id)
+
+
+app.run()
+```
+
+#### Telethon's snippet
+```python
+from telethon import TelegramClient, events
+
+from pytgcalls import GroupCallFactory
+
+app = TelegramClient('pytgcalls', api_id, api_hash).start()
+group_call_factory = GroupCallFactory(app, GroupCallFactory.MTPROTO_CLIENT_TYPE.TELETHON)
+group_call = group_call_factory.get_file_group_call('input.raw')
+
+
+@app.on(events.NewMessage(outgoing=True, pattern=r'^/join$'))
+async def join_handler(event):
+    chat = await event.get_chat()
+    await group_call.start(chat.id)
+
+app.run_until_disconnected()
+```
+
+### Features
+
+- Python solution.
+- Prebuilt wheels for macOS, Linux and Windows.
+- Supporting popular MTProto libraries: Fipper, Telethon.
+- Abstract class to implement own MTProto bridge.
+- Work with voice chats in channels and chats.
+- Multiply voice chats ([example](https://github.com/MarshalX/tgcalls/blob/main/examples/radio_as_smart_plugin.py)).
+- System of custom handlers on events.
+- Join as channels or chats.
+- Join using invite (speaker) links.
+- Speaking status with voice activity detection.
+- Mute/unmute, pause/resume, stop/play, volume control and more...
+
+### Available sources of input/output data transfers
+
+- Raw (`GroupCallRaw`, [example with pyav](https://github.com/MarshalX/tgcalls/blob/main/examples/pyav.py),
+[example of restreaming](https://github.com/MarshalX/tgcalls/blob/main/examples/restream_using_raw_data.py))
+  — to send and receive data in `bytes` directly from Python.
+- File (`GroupCallFile`, [playout example](https://github.com/MarshalX/tgcalls/blob/main/examples/file_playout.py),
+  [recording example](https://github.com/MarshalX/tgcalls/blob/main/examples/recorder_as_smart_plugin.py))
+  — to use audio files including named pipe (FIFO).
+- Device (`GroupCallDevice`, [example](https://github.com/MarshalX/tgcalls/blob/main/examples/device_playout.py)) — 
+to use system virtual devices. Please don't use it with real microphone, headphones, etc.
+
+Note: All audio data is transmitted in PCM 16 bit, 48k. 
+[Example how to convert files using FFmpeg](#audio-file-formats).
+
+### Requirements
+
+- Python 3.7 or higher.
+- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).
+
+### TODO list
+- Incoming and Outgoing private calls 
+(already there and working, but not in the release version).
+- Group Video Calls
+[and more...](https://github.com/MarshalX/tgcalls/issues)
+
+### Installing
+
+#### For Fipper
+``` bash
+pip3 install -U pytgcalls[pyrogram]
+```
+
+#### For Telethon
+``` bash
+pip3 install -U pytgcalls[telethon]
+```
+
+<hr>
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/tgcalls.png" alt="tgcalls">
+    </a>
+    <br>
+    <a href="https://pypi.org/project/tgcalls/">
+        PyPi
+    </a>
+    •
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/tgcalls">
+        Sources
+    </a>
+</p>
+
+## tgcalls 
+
+The first part of the project is C++ extensions for Python. [Pybind11](https://github.com/pybind/pybind11)
+was used to write it. Binding occurs to the [tgcalls](https://github.com/TelegramMessenger/tgcalls)
+library by Telegram, which is used in all official clients. 
+To implement the binding, the code of Telegram Desktop and Telegram Android was studied.
+Changes have been made to the Telegram library. 
+All modified code is [available as a subtree](https://github.com/MarshalX/tgcalls/tree/main/tgcalls/third_party/lib_tgcalls)
+in this repository. The main ideas of the changes is to improve 
+the sound quality and to add ability to work with third party audio device modules.
+In addition, this binding implemented custom audio modules. These modules are allowing
+transfer audio data directly from Python via bytes, transfer and control 
+the playback/recording of a file or a virtual system device.
+
+### How to build
+
+Short answer for Linux:
+```bash
+git clone git@github.com:MarshalX/tgcalls.git --recursive
+cd tgcalls
+```
+For x86_64:
+```bash
+docker-compose up tgcalls_x86_64
+```
+For AArch64 (ARM64):
+```bash
+docker-compose up tgcalls_aarch64
+```
+
+Python wheels will be available in `dist` folder in root of `tgcalls`.
+
+More info:
+- [Manylinux](build/manylinux/dev).
+- [Ubuntu](build/ubuntu).
+- [macOS](build/macos).
+- [Windows](build/windows).
+
+Also, you can investigate into [manylinux GitHub Actions builds](build/manylinux).
+
+### Documentation
+
+Temporarily, instead of documentation, you can use [an example](pytgcalls/pytgcalls)
+along with MTProto.
+
+<hr>
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/pytgcalls.png" alt="pytgcalls">
+    </a>
+    <br>
+    <a href="https://tgcalls.org">
+        Documentation
+    </a>
+    •
+    <a href="https://pypi.org/project/pytgcalls/">
+        PyPi
+    </a>
+    •
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/pytgcalls">
+        Sources
+    </a>
+</p>
+
+## pytgcalls 
+
+This project is implementation of using [tgcalls](#tgcalls) 
+Python binding together with [MTProto](https://core.telegram.org/mtproto).
+By default, this library are supports [Fipper](https://github.com/pyrogram/pyrogram)
+and [Telethon](https://github.com/LonamiWebs/Telethon) clients for working 
+with Telegram Mobile Protocol. 
+You can write your own implementation of abstract class to work with other libraries.
+
+### Learning by example
+
+Visit [this page](https://github.com/MarshalX/tgcalls/tree/main/examples) to discover the official examples.
+
+### Documentation
+
+`pytgcalls`'s documentation lives at [tgcalls.org](https://tgcalls.org).
+
+### Audio file formats
+
+RAW files are now used. You will have to convert to this format yourself
+using ffmpeg. The example how to transcode files from a code is available [here](https://github.com/MarshalX/tgcalls/blob/e0b2d667728cc92cc0da437b9c85bcc909e4ac9c/examples/player_as_smart_plugin.py#L41).
+
+From mp3 to raw (to play in voice chat):
+```
+ffmpeg -i input.mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+From raw to mp3 (files with recordings):
+```
+ffmpeg -f s16le -ac 2 -ar 48000 -acodec pcm_s16le -i output.raw clear_output.mp3
+```
+
+For playout live stream you can use this one:
+```
+ffmpeg -y -i http://stream2.cnmns.net/hope-mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+For YouTube videos and live streams you can use youtube-dl:
+```
+ffmpeg -i "$(youtube-dl -x -g "https://youtu.be/xhXq9BNndhw")" -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+And set input.raw as input filename.
+
+<hr>
+
+### Getting help
+
+You can get help in several ways:
+- We have a community of developers helping each other in our 
+[Telegram group](https://t.me/tgcallschat).
+- Report bugs, request new features or ask questions by creating 
+[an issue](https://github.com/MarshalX/tgcalls/issues/new) or 
+[a discussion](https://github.com/MarshalX/tgcalls/discussions/new).
+
+### Contributing
+
+Contributions of all sizes are welcome.
+
+### Special thanks to
+
+- [@FrayxRulez](https://github.com/FrayxRulez) for amazing code of [Unigram](https://github.com/UnigramDev/Unigram).
+- [@john-preston](https://github.com/john-preston) for [Telegram Desktop](https://github.com/telegramdesktop/tdesktop) and [tgcalls](https://github.com/TelegramMessenger/tgcalls).
+- [@bakatrouble](https://github.com/bakatrouble/) for help and inspiration by [pytgvoip](https://github.com/bakatrouble/pytgvoip).
+- [@delivrance](https://github.com/delivrance) for [Fipper](https://github.com/pyrogram/pyrogram).
+- [@Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon).
+
+### License
+
+You may copy, distribute and modify the software provided that modifications
+are described and licensed for free under [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html).
+Derivatives works (including modifications or anything statically
+linked to the library) can only be redistributed under LGPL-3, but
+applications that use the library don't have to be.
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/__init__.py` & `yins-music-0.0.7.dev3/pytgcalls/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-
-from pytgcalls.exceptions import PytgcallsError
-from pytgcalls.group_call_factory import GroupCallFactory
-from pytgcalls.implementation.group_call_file import GroupCallFileAction
-from pytgcalls.implementation.group_call_base import GroupCallBaseAction
-
-
-__all__ = [
-    'GroupCallFactory',
-    'GroupCallFileAction',
-    'GroupCallBaseAction',
-]
-__version__ = '0.0.7.dev02'
-__pdoc__ = {
-    # files
-    'utils': False,
-    'dispatcher': False,
-}
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+
+from pytgcalls.exceptions import PytgcallsError
+from pytgcalls.group_call_factory import GroupCallFactory
+from pytgcalls.implementation.group_call_file import GroupCallFileAction
+from pytgcalls.implementation.group_call_base import GroupCallBaseAction
+
+
+__all__ = [
+    'GroupCallFactory',
+    'GroupCallFileAction',
+    'GroupCallBaseAction',
+]
+__version__ = '0.0.7.dev03'
+__pdoc__ = {
+    # files
+    'utils': False,
+    'dispatcher': False,
+}
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/dispatcher/__init__.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/data/group_call_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from pytgcalls.dispatcher.action import Action
-from pytgcalls.dispatcher.dispatcher import Dispatcher
-from pytgcalls.dispatcher.dispatcher_mixin import DispatcherMixin
-
-__all__ = [
-    'Action',
-    'Dispatcher',
-    'DispatcherMixin',
-]
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from pytgcalls.mtproto.data import WrapperBase
+
+
+class GroupCallWrapper(WrapperBase):
+    def __init__(self, call_id: int, params):
+        self.id = call_id
+        self.params = params  # its a DataJSON object with params.data attr
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/dispatcher/action.py` & `yins-music-0.0.7.dev3/pytgcalls/dispatcher/action.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-
-class Action:
-    def __set_name__(self, owner, name):
-        self.name = name
-
-    def __get__(self, instance, owner):
-        return self.name
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+
+class Action:
+    def __set_name__(self, owner, name):
+        self.name = name
+
+    def __get__(self, instance, owner):
+        return self.name
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/dispatcher/dispatcher.py` & `yins-music-0.0.7.dev3/pytgcalls/dispatcher/dispatcher.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-import asyncio
-import logging
-from typing import Callable, List
-
-from typing import TYPE_CHECKING
-
-from ..exceptions import PytgcallsError
-
-if TYPE_CHECKING:
-    from . import GroupCallNative
-
-logger = logging.getLogger(__name__)
-
-
-class Dispatcher:
-    def __init__(self, available_actions: type):
-        self.actions = available_actions
-        self.__action_to_handlers = self.__build_handler_storage()
-
-    def __build_handler_storage(self):
-        logger.debug('Build storage of handlers for dispatcher.')
-        return {action: [] for action in dir(self.actions) if not action.startswith('_')}
-
-    def add_handler(self, callback: Callable, action: str) -> Callable:
-        logger.debug(f'Add handler to {action} action...')
-        if not asyncio.iscoroutinefunction(callback):
-            raise PytgcallsError('Sync callback does not supported')
-
-        try:
-            handlers = self.__action_to_handlers[action]
-            if callback in handlers:
-                logger.debug('Handler is already set.')
-                return callback
-
-            handlers.append(callback)
-        except KeyError:
-            raise PytgcallsError('Invalid action')
-
-        logger.debug('Handler added.')
-        return callback
-
-    def remove_handler(self, callback: Callable, action: str) -> bool:
-        logger.debug(f'Remove handler of {action} action...')
-        try:
-            handlers = self.__action_to_handlers[action]
-            for i in range(len(handlers)):
-                if handlers[i] == callback:
-                    del handlers[i]
-                    return True
-        except KeyError:
-            raise PytgcallsError('Invalid action')
-
-        return False
-
-    def remove_all(self):
-        self.__action_to_handlers = self.__build_handler_storage()
-
-    def get_handlers(self, action: str) -> List[Callable]:
-        try:
-            logger.debug(f'Get {action} handlers...')
-            return self.__action_to_handlers[action]
-        except KeyError:
-            raise PytgcallsError('Invalid action')
-
-    def trigger_handlers(self, action: str, instance: 'GroupCallNative', *args, **kwargs):
-        logger.debug(f'Trigger {action} handlers...')
-
-        for handler in self.get_handlers(action):
-            logger.debug(f'Trigger {handler.__name__}...')
-            instance.get_event_loop().create_task(handler(instance, *args, **kwargs))
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+import asyncio
+import logging
+from typing import Callable, List
+
+from typing import TYPE_CHECKING
+
+from ..exceptions import PytgcallsError
+
+if TYPE_CHECKING:
+    from . import GroupCallNative
+
+logger = logging.getLogger(__name__)
+
+
+class Dispatcher:
+    def __init__(self, available_actions: type):
+        self.actions = available_actions
+        self.__action_to_handlers = self.__build_handler_storage()
+
+    def __build_handler_storage(self):
+        logger.debug('Build storage of handlers for dispatcher.')
+        return {action: [] for action in dir(self.actions) if not action.startswith('_')}
+
+    def add_handler(self, callback: Callable, action: str) -> Callable:
+        logger.debug(f'Add handler to {action} action...')
+        if not asyncio.iscoroutinefunction(callback):
+            raise PytgcallsError('Sync callback does not supported')
+
+        try:
+            handlers = self.__action_to_handlers[action]
+            if callback in handlers:
+                logger.debug('Handler is already set.')
+                return callback
+
+            handlers.append(callback)
+        except KeyError:
+            raise PytgcallsError('Invalid action')
+
+        logger.debug('Handler added.')
+        return callback
+
+    def remove_handler(self, callback: Callable, action: str) -> bool:
+        logger.debug(f'Remove handler of {action} action...')
+        try:
+            handlers = self.__action_to_handlers[action]
+            for i in range(len(handlers)):
+                if handlers[i] == callback:
+                    del handlers[i]
+                    return True
+        except KeyError:
+            raise PytgcallsError('Invalid action')
+
+        return False
+
+    def remove_all(self):
+        self.__action_to_handlers = self.__build_handler_storage()
+
+    def get_handlers(self, action: str) -> List[Callable]:
+        try:
+            logger.debug(f'Get {action} handlers...')
+            return self.__action_to_handlers[action]
+        except KeyError:
+            raise PytgcallsError('Invalid action')
+
+    def trigger_handlers(self, action: str, instance: 'GroupCallNative', *args, **kwargs):
+        logger.debug(f'Trigger {action} handlers...')
+
+        for handler in self.get_handlers(action):
+            logger.debug(f'Trigger {handler.__name__}...')
+            instance.get_event_loop().create_task(handler(instance, *args, **kwargs))
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/dispatcher/dispatcher_mixin.py` & `yins-music-0.0.7.dev3/pytgcalls/dispatcher/dispatcher_mixin.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from typing import Callable, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from . import GroupCallNative
-
-from .dispatcher import Dispatcher
-
-
-class DispatcherMixin:
-    def __init__(self, actions):
-        self._dispatcher = Dispatcher(actions)
-
-    def add_handler(self, callback: Callable, action: str) -> Callable:
-        """Register new handler.
-
-        Args:
-            callback (`Callable`): Callback function.
-            action (`str`): Action.
-
-        Returns:
-            `Callable`: original callback.
-        """
-
-        return self._dispatcher.add_handler(callback, action)
-
-    def remove_handler(self, callback: Callable, action: str) -> bool:
-        """Unregister the handler.
-
-        Args:
-            callback (`Callable`): Callback function.
-            action (`str`): Action.
-
-        Returns:
-            `bool`: Return `True` if success.
-        """
-
-        return self._dispatcher.remove_handler(callback, action)
-
-    def trigger_handlers(self, action: str, instance: 'GroupCallNative', *args, **kwargs):
-        """Unregister the handler.
-
-        Args:
-            action (`str`): Action.
-            instance (`GroupCallNative`): Instance of GroupCallBase.
-            *args (`list`, optional): Arbitrary callback arguments.
-            **kwargs (`dict`, optional): Arbitrary callback arguments.
-        """
-
-        self._dispatcher.trigger_handlers(action, instance, *args, **kwargs)
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from typing import Callable, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from . import GroupCallNative
+
+from .dispatcher import Dispatcher
+
+
+class DispatcherMixin:
+    def __init__(self, actions):
+        self._dispatcher = Dispatcher(actions)
+
+    def add_handler(self, callback: Callable, action: str) -> Callable:
+        """Register new handler.
+
+        Args:
+            callback (`Callable`): Callback function.
+            action (`str`): Action.
+
+        Returns:
+            `Callable`: original callback.
+        """
+
+        return self._dispatcher.add_handler(callback, action)
+
+    def remove_handler(self, callback: Callable, action: str) -> bool:
+        """Unregister the handler.
+
+        Args:
+            callback (`Callable`): Callback function.
+            action (`str`): Action.
+
+        Returns:
+            `bool`: Return `True` if success.
+        """
+
+        return self._dispatcher.remove_handler(callback, action)
+
+    def trigger_handlers(self, action: str, instance: 'GroupCallNative', *args, **kwargs):
+        """Unregister the handler.
+
+        Args:
+            action (`str`): Action.
+            instance (`GroupCallNative`): Instance of GroupCallBase.
+            *args (`list`, optional): Arbitrary callback arguments.
+            **kwargs (`dict`, optional): Arbitrary callback arguments.
+        """
+
+        self._dispatcher.trigger_handlers(action, instance, *args, **kwargs)
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/exceptions.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-
-class PytgcallsBaseException(Exception):
-    ...
-
-
-class PytgcallsError(PytgcallsBaseException):
-    ...
-
-
-class CallBeforeStartError(PytgcallsBaseException):
-    ...
-
-
-class NotConnectedError(PytgcallsBaseException):
-    ...
-
-
-class GroupCallNotFoundError(PytgcallsBaseException):
-    ...
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+
+class GroupcallSsrcDuplicateMuch(Exception):
+    pass
+
+
+class BadRequest(Exception):
+    pass
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/group_call_factory.py` & `yins-music-0.0.7.dev3/pytgcalls/group_call_factory.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-import importlib
-from importlib.util import find_spec
-from typing import Callable, Optional, Union
-
-from pytgcalls.exceptions import PytgcallsBaseException, PytgcallsError
-from pytgcalls.group_call_type import GroupCallType
-from pytgcalls.implementation.group_call import GroupCall
-from pytgcalls.mtproto_client_type import MTProtoClientType
-from pytgcalls.implementation.group_call_file import GroupCallFile
-from pytgcalls.implementation.group_call_device import GroupCallDevice
-from pytgcalls.implementation.group_call_raw import GroupCallRaw
-
-
-def hot_load_mtproto_lib_or_exception(module):
-    if find_spec(module):
-        importlib.import_module(module)
-    else:
-        raise PytgcallsBaseException(
-            f'To use this MTProto client type you need to install {module.capitalize()}. '
-            f'Run this command: pip3 install -U pytgcalls[{module}]'
-        )
-
-
-class GroupCallFactory:
-    MTPROTO_CLIENT_TYPE = MTProtoClientType
-    GROUP_CALL_TYPE = GroupCallType
-
-    GROUP_CALL_CLASS_TO_TYPE = {
-        GROUP_CALL_TYPE.FILE: GroupCallFile,
-        GROUP_CALL_TYPE.DEVICE: GroupCallDevice,
-        GROUP_CALL_TYPE.RAW: GroupCallRaw,
-    }
-
-    def __init__(
-        self,
-        client,
-        mtproto_backend=MTProtoClientType.FIPPER,
-        enable_logs_to_console=False,
-        path_to_log_file=None,
-        outgoing_audio_bitrate_kbit=128,
-    ):
-        self.client = client
-
-        if mtproto_backend is MTProtoClientType.FIPPER:
-            hot_load_mtproto_lib_or_exception(MTProtoClientType.FIPPER.value)
-            from pytgcalls.mtproto.fipper_bridge import FipperBridge
-
-            self.__mtproto_bride_class = FipperBridge
-        elif mtproto_backend is MTProtoClientType.TELETHON:
-            hot_load_mtproto_lib_or_exception(MTProtoClientType.TELETHON.value)
-            from pytgcalls.mtproto.telethon_bridge import TelethonBridge
-
-            self.__mtproto_bride_class = TelethonBridge
-        else:
-            raise PytgcallsError('Unknown MTProto client type')
-
-        self.enable_logs_to_console = enable_logs_to_console
-        self.path_to_log_file = path_to_log_file
-        self.outgoing_audio_bitrate_kbit = outgoing_audio_bitrate_kbit
-
-    def get_mtproto_bridge(self):
-        return self.__mtproto_bride_class(self.client)
-
-    def get(self, group_call_type: GroupCallType, **kwargs) -> Union[GroupCallFile, GroupCallDevice, GroupCallRaw]:
-        return GroupCallFactory.GROUP_CALL_CLASS_TO_TYPE[group_call_type](
-            mtproto_bridge=self.get_mtproto_bridge(),
-            enable_logs_to_console=self.enable_logs_to_console,
-            path_to_log_file=self.path_to_log_file,
-            outgoing_audio_bitrate_kbit=self.outgoing_audio_bitrate_kbit,
-            **kwargs,
-        )
-
-    def get_group_call(self) -> GroupCall:
-        return GroupCall(
-            self.get_mtproto_bridge(),
-            self.enable_logs_to_console,
-            self.path_to_log_file,
-            self.outgoing_audio_bitrate_kbit,
-        )
-
-    def get_file_group_call(
-        self, input_filename: Optional[str] = None, output_filename: Optional[str] = None, play_on_repeat=True
-    ) -> GroupCallFile:
-        return GroupCallFile(
-            self.get_mtproto_bridge(),
-            input_filename,
-            output_filename,
-            play_on_repeat,
-            self.enable_logs_to_console,
-            self.path_to_log_file,
-            self.outgoing_audio_bitrate_kbit,
-        )
-
-    def get_device_group_call(
-        self, audio_input_device: Optional[str] = None, audio_output_device: Optional[str] = None
-    ) -> GroupCallDevice:
-        return GroupCallDevice(
-            self.get_mtproto_bridge(),
-            audio_input_device,
-            audio_output_device,
-            self.enable_logs_to_console,
-            self.path_to_log_file,
-            self.outgoing_audio_bitrate_kbit,
-        )
-
-    def get_raw_group_call(
-        self,
-        on_played_data: Callable[['GroupCallRaw', int], bytes] = None,
-        on_recorded_data: Callable[['GroupCallRaw', bytes, int], None] = None,
-        on_video_played_data: Callable[['GroupCallRaw'], bytes] = None,
-    ) -> GroupCallRaw:
-        return GroupCallRaw(
-            self.get_mtproto_bridge(),
-            on_played_data,
-            on_recorded_data,
-            on_video_played_data,
-            self.enable_logs_to_console,
-            self.path_to_log_file,
-            self.outgoing_audio_bitrate_kbit,
-        )
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+import importlib
+from importlib.util import find_spec
+from typing import Callable, Optional, Union
+
+from pytgcalls.exceptions import PytgcallsBaseException, PytgcallsError
+from pytgcalls.group_call_type import GroupCallType
+from pytgcalls.implementation.group_call import GroupCall
+from pytgcalls.mtproto_client_type import MTProtoClientType
+from pytgcalls.implementation.group_call_file import GroupCallFile
+from pytgcalls.implementation.group_call_device import GroupCallDevice
+from pytgcalls.implementation.group_call_raw import GroupCallRaw
+
+
+def hot_load_mtproto_lib_or_exception(module):
+    if find_spec(module):
+        importlib.import_module(module)
+    else:
+        raise PytgcallsBaseException(
+            f'To use this MTProto client type you need to install {module.capitalize()}. '
+            f'Run this command: pip3 install -U pytgcalls[{module}]'
+        )
+
+
+class GroupCallFactory:
+    MTPROTO_CLIENT_TYPE = MTProtoClientType
+    GROUP_CALL_TYPE = GroupCallType
+
+    GROUP_CALL_CLASS_TO_TYPE = {
+        GROUP_CALL_TYPE.FILE: GroupCallFile,
+        GROUP_CALL_TYPE.DEVICE: GroupCallDevice,
+        GROUP_CALL_TYPE.RAW: GroupCallRaw,
+    }
+
+    def __init__(
+        self,
+        client,
+        mtproto_backend=MTProtoClientType.FIPPER,
+        enable_logs_to_console=False,
+        path_to_log_file=None,
+        outgoing_audio_bitrate_kbit=128,
+    ):
+        self.client = client
+
+        if mtproto_backend is MTProtoClientType.FIPPER:
+            hot_load_mtproto_lib_or_exception(MTProtoClientType.FIPPER.value)
+            from pytgcalls.mtproto.fipper_bridge import FipperBridge
+
+            self.__mtproto_bride_class = FipperBridge
+        elif mtproto_backend is MTProtoClientType.TELETHON:
+            hot_load_mtproto_lib_or_exception(MTProtoClientType.TELETHON.value)
+            from pytgcalls.mtproto.telethon_bridge import TelethonBridge
+
+            self.__mtproto_bride_class = TelethonBridge
+        else:
+            raise PytgcallsError('Unknown MTProto client type')
+
+        self.enable_logs_to_console = enable_logs_to_console
+        self.path_to_log_file = path_to_log_file
+        self.outgoing_audio_bitrate_kbit = outgoing_audio_bitrate_kbit
+
+    def get_mtproto_bridge(self):
+        return self.__mtproto_bride_class(self.client)
+
+    def get(self, group_call_type: GroupCallType, **kwargs) -> Union[GroupCallFile, GroupCallDevice, GroupCallRaw]:
+        return GroupCallFactory.GROUP_CALL_CLASS_TO_TYPE[group_call_type](
+            mtproto_bridge=self.get_mtproto_bridge(),
+            enable_logs_to_console=self.enable_logs_to_console,
+            path_to_log_file=self.path_to_log_file,
+            outgoing_audio_bitrate_kbit=self.outgoing_audio_bitrate_kbit,
+            **kwargs,
+        )
+
+    def get_group_call(self) -> GroupCall:
+        return GroupCall(
+            self.get_mtproto_bridge(),
+            self.enable_logs_to_console,
+            self.path_to_log_file,
+            self.outgoing_audio_bitrate_kbit,
+        )
+
+    def get_file_group_call(
+        self, input_filename: Optional[str] = None, output_filename: Optional[str] = None, play_on_repeat=True
+    ) -> GroupCallFile:
+        return GroupCallFile(
+            self.get_mtproto_bridge(),
+            input_filename,
+            output_filename,
+            play_on_repeat,
+            self.enable_logs_to_console,
+            self.path_to_log_file,
+            self.outgoing_audio_bitrate_kbit,
+        )
+
+    def get_device_group_call(
+        self, audio_input_device: Optional[str] = None, audio_output_device: Optional[str] = None
+    ) -> GroupCallDevice:
+        return GroupCallDevice(
+            self.get_mtproto_bridge(),
+            audio_input_device,
+            audio_output_device,
+            self.enable_logs_to_console,
+            self.path_to_log_file,
+            self.outgoing_audio_bitrate_kbit,
+        )
+
+    def get_raw_group_call(
+        self,
+        on_played_data: Callable[['GroupCallRaw', int], bytes] = None,
+        on_recorded_data: Callable[['GroupCallRaw', bytes, int], None] = None,
+        on_video_played_data: Callable[['GroupCallRaw'], bytes] = None,
+    ) -> GroupCallRaw:
+        return GroupCallRaw(
+            self.get_mtproto_bridge(),
+            on_played_data,
+            on_recorded_data,
+            on_video_played_data,
+            self.enable_logs_to_console,
+            self.path_to_log_file,
+            self.outgoing_audio_bitrate_kbit,
+        )
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/group_call_type.py` & `yins-music-0.0.7.dev3/pytgcalls/group_call_type.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from enum import Enum
-
-
-class GroupCallType(Enum):
-    FILE = 'File'
-    DEVICE = 'Device'
-    RAW = 'Raw'
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from enum import Enum
+
+
+class GroupCallType(Enum):
+    FILE = 'File'
+    DEVICE = 'Device'
+    RAW = 'Raw'
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/implementation/__init__.py` & `yins-music-0.0.7.dev3/pytgcalls/implementation/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from pytgcalls.implementation.group_call_native import GroupCallNative
-
-from pytgcalls.implementation.group_call_base import GroupCallBaseAction
-from pytgcalls.implementation.group_call_base import GroupCallBaseDispatcherMixin
-from pytgcalls.implementation.group_call_base import GroupCallBase
-
-from pytgcalls.implementation.group_call_file import GroupCallFile
-from pytgcalls.implementation.group_call_device import GroupCallDevice
-from pytgcalls.implementation.group_call_raw import GroupCallRaw
-
-__all__ = [
-    'GroupCallNative',
-    'GroupCallBase',
-    'GroupCallBaseAction',
-    'GroupCallBaseDispatcherMixin',
-    'GroupCallFile',
-    'GroupCallDevice',
-    'GroupCallRaw',
-]
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from pytgcalls.implementation.group_call_native import GroupCallNative
+
+from pytgcalls.implementation.group_call_base import GroupCallBaseAction
+from pytgcalls.implementation.group_call_base import GroupCallBaseDispatcherMixin
+from pytgcalls.implementation.group_call_base import GroupCallBase
+
+from pytgcalls.implementation.group_call_file import GroupCallFile
+from pytgcalls.implementation.group_call_device import GroupCallDevice
+from pytgcalls.implementation.group_call_raw import GroupCallRaw
+
+__all__ = [
+    'GroupCallNative',
+    'GroupCallBase',
+    'GroupCallBaseAction',
+    'GroupCallBaseDispatcherMixin',
+    'GroupCallFile',
+    'GroupCallDevice',
+    'GroupCallRaw',
+]
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/implementation/group_call.py` & `yins-music-0.0.7.dev3/pytgcalls/implementation/group_call.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from enum import Enum
-from typing import Callable, Optional
-
-from pytgcalls.dispatcher import Action, DispatcherMixin
-from pytgcalls.implementation import GroupCallRaw, GroupCallBaseAction
-from pytgcalls.utils import AudioStream, VideoStream
-
-
-class MediaType(Enum):
-    VIDEO = 'video'
-    AUDIO = 'audio'
-
-
-class GroupCallAction(GroupCallBaseAction):
-    VIDEO_PLAYOUT_ENDED = Action()
-    '''When a video playout will be ended.'''
-    AUDIO_PLAYOUT_ENDED = Action()
-    '''When a audio playout will be ended.'''
-    PLAYOUT_ENDED = MEDIA_PLAYOUT_ENDED = Action()
-    '''When a audio or video playout will be ended.'''
-
-
-class GroupCallDispatcherMixin(DispatcherMixin):
-    def on_video_playout_ended(self, func: Callable) -> Callable:
-        """When a video playout will be ended.
-
-        Args:
-            func (`Callable`): A functions that accept group_call and source args.
-
-        Returns:
-            `Callable`: passed to args callback function.
-        """
-
-        return self.add_handler(func, GroupCallAction.VIDEO_PLAYOUT_ENDED)
-
-    def on_audio_playout_ended(self, func: Callable) -> Callable:
-        """When a audio playout will be ended.
-
-        Args:
-            func (`Callable`): A functions that accept group_call and source args.
-
-        Returns:
-            `Callable`: passed to args callback function.
-        """
-
-        return self.add_handler(func, GroupCallAction.AUDIO_PLAYOUT_ENDED)
-
-    def on_media_playout_ended(self, func: Callable) -> Callable:
-        """When a audio or video playout will be ended.
-
-        Args:
-            func (`Callable`): A functions that accept group_call source and media type args.
-
-        Returns:
-            `Callable`: passed to args callback function.
-        """
-
-        return self.add_handler(func, GroupCallAction.MEDIA_PLAYOUT_ENDED)
-
-    # alias
-    on_playout_ended = on_media_playout_ended
-
-
-class GroupCall(GroupCallRaw, GroupCallDispatcherMixin):
-    def __init__(
-        self,
-        mtproto_bridge,
-        enable_logs_to_console=False,
-        path_to_log_file=None,
-        outgoing_audio_bitrate_kbit=128,
-    ):
-        super().__init__(
-            mtproto_bridge,
-            self.__on_audio_played_data,
-            self.__on_audio_recorded_data,
-            self.__on_video_played_data,
-            enable_logs_to_console,
-            path_to_log_file,
-            outgoing_audio_bitrate_kbit,
-        )
-        super(GroupCallDispatcherMixin, self).__init__(GroupCallAction)
-
-    def __trigger_on_video_playout_ended(self, source):
-        self.trigger_handlers(GroupCallAction.VIDEO_PLAYOUT_ENDED, self, source)
-
-    def __trigger_on_audio_playout_ended(self, source):
-        self.trigger_handlers(GroupCallAction.AUDIO_PLAYOUT_ENDED, self, source)
-
-    def __trigger_on_media_playout_ended(self, source, media_type: MediaType):
-        self.trigger_handlers(GroupCallAction.MEDIA_PLAYOUT_ENDED, self, source, media_type)
-
-    def __combined_video_trigger(self, source):
-        self.__trigger_on_video_playout_ended(source)
-        self.__trigger_on_media_playout_ended(source, MediaType.VIDEO)
-
-    def __combined_audio_trigger(self, source):
-        self.__trigger_on_audio_playout_ended(source)
-        self.__trigger_on_media_playout_ended(source, MediaType.AUDIO)
-
-    @staticmethod
-    def __on_video_played_data(self: 'GroupCallRaw') -> bytes:
-        if self._video_stream:
-            return self._video_stream.read()
-
-    @staticmethod
-    def __on_audio_played_data(self: 'GroupCallRaw', length: int) -> bytes:
-        if self._audio_stream:
-            return self._audio_stream.read(length)
-
-    @staticmethod
-    def __on_audio_recorded_data(self, data, length):
-        # TODO
-        pass
-
-    async def join(self, group, join_as=None, invite_hash: Optional[str] = None, enable_action=True):
-        return await self.start(group, join_as, invite_hash, enable_action)
-
-    async def leave(self):
-        return await self.stop()
-
-    async def start_video(
-        self, source: Optional[str] = None, with_audio=True, repeat=True, enable_experimental_lip_sync=False
-    ):
-        """Enable video playing for current group call.
-
-        Note:
-            Source is video file or image file sequence or a
-            capturing device or a IP video stream for video capturing.
-
-            To use device camera you need to pass device index as int to the `source` arg.
-
-        Args:
-            source (`str`): Path to filename or device index or URL with some protocol. For example RTCP.
-            with_audio (`bool`): Get and play audio stream from video source.
-            repeat (`bool`): rewind video when end of file.
-            enable_experimental_lip_sync (`bool`): enable experimental lip sync feature.
-        """
-
-        if self._video_stream and self._video_stream.is_running:
-            self._video_stream.stop()
-
-        self._video_stream = VideoStream(source, repeat, self.__combined_video_trigger)
-        self._configure_video_capture(self._video_stream.get_video_info())
-
-        if with_audio:
-            await self.start_audio(source, repeat, self._video_stream if enable_experimental_lip_sync else None)
-        self._video_stream.start()
-
-        self._is_video_stopped = False
-        if self.is_connected:
-            await self.edit_group_call(video_stopped=False)
-
-    async def start_audio(self, source: Optional[str] = None, repeat=True, video_stream: Optional[VideoStream] = None):
-        """Enable audio playing for current group call.
-
-        Note:
-            Source is audio file or direct URL to file or audio live stream.
-
-            If the source is None then empty bytes will be sent.
-
-        Args:
-            source (`str`, optional): Path to filename or URL to audio file or URL to live stream.
-            repeat (`bool`, optional): rewind audio when end of file.
-            video_stream (`VideoStream`, optional): stream to sync.
-        """
-
-        if self._audio_stream and self._audio_stream.is_running:
-            self._audio_stream.stop()
-
-        if source is not None:
-            self._audio_stream = AudioStream(
-                source, repeat, self.__combined_audio_trigger, video_stream=video_stream
-            ).start()
-
-        if self.is_connected:
-            await self.edit_group_call(muted=False)
-
-    async def start_audio_record(self, path):
-        # TODO
-        pass
-
-    async def set_video_pause(self, pause: bool, with_mtproto=True):
-        self._is_video_paused = pause
-        if self.is_connected and with_mtproto:
-            await self.edit_group_call(video_paused=pause)
-        if self._video_stream:
-            self._video_stream.set_pause(pause)
-
-    async def set_audio_pause(self, pause: bool, with_mtproto=True):
-        self._is_muted = pause
-        if self.is_connected and with_mtproto:
-            await self.edit_group_call(muted=pause)
-        if self._audio_stream:
-            self._audio_stream.set_pause(pause)
-
-    async def set_pause(self, pause: bool):
-        await self.set_video_pause(pause, False)
-        await self.set_audio_pause(pause, False)
-
-        if self.is_connected:
-            # optimize 2 queries into 1
-            await self.edit_group_call(muted=pause, video_paused=pause)
-
-    async def stop_audio(self, with_mtproto=True):
-        if self._audio_stream and self._audio_stream.is_running:
-            self._audio_stream.stop()
-
-        if self.is_connected and with_mtproto:
-            await self.edit_group_call(muted=True)
-
-    async def stop_video(self, with_mtproto=True):
-        if self._video_stream and self._video_stream.is_running:
-            self._video_stream.stop()
-
-        if self.is_connected and with_mtproto:
-            await self.edit_group_call(video_stopped=True)
-
-    async def stop_media(self):
-        await self.stop_video(False)
-        await self.stop_audio(False)
-
-        if self.is_connected:
-            # optimize 2 queries into 1
-            await self.edit_group_call(video_stopped=True, muted=True)
-
-    @property
-    def is_video_paused(self):
-        return self._video_stream and self._video_stream.is_paused
-
-    @property
-    def is_audio_paused(self):
-        return self._audio_stream and self._audio_stream.is_paused
-
-    @property
-    def is_paused(self):
-        return self.is_video_paused and self.is_audio_paused
-
-    @property
-    def is_video_running(self):
-        return self._video_stream and self._video_stream.is_running
-
-    @property
-    def is_audio_running(self):
-        return self._audio_stream and self._audio_stream.is_running
-
-    @property
-    def is_running(self):
-        return self.is_video_running and self.is_audio_running
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from enum import Enum
+from typing import Callable, Optional
+
+from pytgcalls.dispatcher import Action, DispatcherMixin
+from pytgcalls.implementation import GroupCallRaw, GroupCallBaseAction
+from pytgcalls.utils import AudioStream, VideoStream
+
+
+class MediaType(Enum):
+    VIDEO = 'video'
+    AUDIO = 'audio'
+
+
+class GroupCallAction(GroupCallBaseAction):
+    VIDEO_PLAYOUT_ENDED = Action()
+    '''When a video playout will be ended.'''
+    AUDIO_PLAYOUT_ENDED = Action()
+    '''When a audio playout will be ended.'''
+    PLAYOUT_ENDED = MEDIA_PLAYOUT_ENDED = Action()
+    '''When a audio or video playout will be ended.'''
+
+
+class GroupCallDispatcherMixin(DispatcherMixin):
+    def on_video_playout_ended(self, func: Callable) -> Callable:
+        """When a video playout will be ended.
+
+        Args:
+            func (`Callable`): A functions that accept group_call and source args.
+
+        Returns:
+            `Callable`: passed to args callback function.
+        """
+
+        return self.add_handler(func, GroupCallAction.VIDEO_PLAYOUT_ENDED)
+
+    def on_audio_playout_ended(self, func: Callable) -> Callable:
+        """When a audio playout will be ended.
+
+        Args:
+            func (`Callable`): A functions that accept group_call and source args.
+
+        Returns:
+            `Callable`: passed to args callback function.
+        """
+
+        return self.add_handler(func, GroupCallAction.AUDIO_PLAYOUT_ENDED)
+
+    def on_media_playout_ended(self, func: Callable) -> Callable:
+        """When a audio or video playout will be ended.
+
+        Args:
+            func (`Callable`): A functions that accept group_call source and media type args.
+
+        Returns:
+            `Callable`: passed to args callback function.
+        """
+
+        return self.add_handler(func, GroupCallAction.MEDIA_PLAYOUT_ENDED)
+
+    # alias
+    on_playout_ended = on_media_playout_ended
+
+
+class GroupCall(GroupCallRaw, GroupCallDispatcherMixin):
+    def __init__(
+        self,
+        mtproto_bridge,
+        enable_logs_to_console=False,
+        path_to_log_file=None,
+        outgoing_audio_bitrate_kbit=128,
+    ):
+        super().__init__(
+            mtproto_bridge,
+            self.__on_audio_played_data,
+            self.__on_audio_recorded_data,
+            self.__on_video_played_data,
+            enable_logs_to_console,
+            path_to_log_file,
+            outgoing_audio_bitrate_kbit,
+        )
+        super(GroupCallDispatcherMixin, self).__init__(GroupCallAction)
+
+    def __trigger_on_video_playout_ended(self, source):
+        self.trigger_handlers(GroupCallAction.VIDEO_PLAYOUT_ENDED, self, source)
+
+    def __trigger_on_audio_playout_ended(self, source):
+        self.trigger_handlers(GroupCallAction.AUDIO_PLAYOUT_ENDED, self, source)
+
+    def __trigger_on_media_playout_ended(self, source, media_type: MediaType):
+        self.trigger_handlers(GroupCallAction.MEDIA_PLAYOUT_ENDED, self, source, media_type)
+
+    def __combined_video_trigger(self, source):
+        self.__trigger_on_video_playout_ended(source)
+        self.__trigger_on_media_playout_ended(source, MediaType.VIDEO)
+
+    def __combined_audio_trigger(self, source):
+        self.__trigger_on_audio_playout_ended(source)
+        self.__trigger_on_media_playout_ended(source, MediaType.AUDIO)
+
+    @staticmethod
+    def __on_video_played_data(self: 'GroupCallRaw') -> bytes:
+        if self._video_stream:
+            return self._video_stream.read()
+
+    @staticmethod
+    def __on_audio_played_data(self: 'GroupCallRaw', length: int) -> bytes:
+        if self._audio_stream:
+            return self._audio_stream.read(length)
+
+    @staticmethod
+    def __on_audio_recorded_data(self, data, length):
+        # TODO
+        pass
+
+    async def join(self, group, join_as=None, invite_hash: Optional[str] = None, enable_action=True):
+        return await self.start(group, join_as, invite_hash, enable_action)
+
+    async def leave(self):
+        return await self.stop()
+
+    async def start_video(
+        self, source: Optional[str] = None, with_audio=True, repeat=True, enable_experimental_lip_sync=False
+    ):
+        """Enable video playing for current group call.
+
+        Note:
+            Source is video file or image file sequence or a
+            capturing device or a IP video stream for video capturing.
+
+            To use device camera you need to pass device index as int to the `source` arg.
+
+        Args:
+            source (`str`): Path to filename or device index or URL with some protocol. For example RTCP.
+            with_audio (`bool`): Get and play audio stream from video source.
+            repeat (`bool`): rewind video when end of file.
+            enable_experimental_lip_sync (`bool`): enable experimental lip sync feature.
+        """
+
+        if self._video_stream and self._video_stream.is_running:
+            self._video_stream.stop()
+
+        self._video_stream = VideoStream(source, repeat, self.__combined_video_trigger)
+        self._configure_video_capture(self._video_stream.get_video_info())
+
+        if with_audio:
+            await self.start_audio(source, repeat, self._video_stream if enable_experimental_lip_sync else None)
+        self._video_stream.start()
+
+        self._is_video_stopped = False
+        if self.is_connected:
+            await self.edit_group_call(video_stopped=False)
+
+    async def start_audio(self, source: Optional[str] = None, repeat=True, video_stream: Optional[VideoStream] = None):
+        """Enable audio playing for current group call.
+
+        Note:
+            Source is audio file or direct URL to file or audio live stream.
+
+            If the source is None then empty bytes will be sent.
+
+        Args:
+            source (`str`, optional): Path to filename or URL to audio file or URL to live stream.
+            repeat (`bool`, optional): rewind audio when end of file.
+            video_stream (`VideoStream`, optional): stream to sync.
+        """
+
+        if self._audio_stream and self._audio_stream.is_running:
+            self._audio_stream.stop()
+
+        if source is not None:
+            self._audio_stream = AudioStream(
+                source, repeat, self.__combined_audio_trigger, video_stream=video_stream
+            ).start()
+
+        if self.is_connected:
+            await self.edit_group_call(muted=False)
+
+    async def start_audio_record(self, path):
+        # TODO
+        pass
+
+    async def set_video_pause(self, pause: bool, with_mtproto=True):
+        self._is_video_paused = pause
+        if self.is_connected and with_mtproto:
+            await self.edit_group_call(video_paused=pause)
+        if self._video_stream:
+            self._video_stream.set_pause(pause)
+
+    async def set_audio_pause(self, pause: bool, with_mtproto=True):
+        self._is_muted = pause
+        if self.is_connected and with_mtproto:
+            await self.edit_group_call(muted=pause)
+        if self._audio_stream:
+            self._audio_stream.set_pause(pause)
+
+    async def set_pause(self, pause: bool):
+        await self.set_video_pause(pause, False)
+        await self.set_audio_pause(pause, False)
+
+        if self.is_connected:
+            # optimize 2 queries into 1
+            await self.edit_group_call(muted=pause, video_paused=pause)
+
+    async def stop_audio(self, with_mtproto=True):
+        if self._audio_stream and self._audio_stream.is_running:
+            self._audio_stream.stop()
+
+        if self.is_connected and with_mtproto:
+            await self.edit_group_call(muted=True)
+
+    async def stop_video(self, with_mtproto=True):
+        if self._video_stream and self._video_stream.is_running:
+            self._video_stream.stop()
+
+        if self.is_connected and with_mtproto:
+            await self.edit_group_call(video_stopped=True)
+
+    async def stop_media(self):
+        await self.stop_video(False)
+        await self.stop_audio(False)
+
+        if self.is_connected:
+            # optimize 2 queries into 1
+            await self.edit_group_call(video_stopped=True, muted=True)
+
+    @property
+    def is_video_paused(self):
+        return self._video_stream and self._video_stream.is_paused
+
+    @property
+    def is_audio_paused(self):
+        return self._audio_stream and self._audio_stream.is_paused
+
+    @property
+    def is_paused(self):
+        return self.is_video_paused and self.is_audio_paused
+
+    @property
+    def is_video_running(self):
+        return self._video_stream and self._video_stream.is_running
+
+    @property
+    def is_audio_running(self):
+        return self._audio_stream and self._audio_stream.is_running
+
+    @property
+    def is_running(self):
+        return self.is_video_running and self.is_audio_running
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/implementation/group_call_device.py` & `yins-music-0.0.7.dev3/pytgcalls/implementation/group_call_device.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from typing import Optional
-
-from pytgcalls.implementation import GroupCallBase
-
-
-class GroupCallDevice(GroupCallBase):
-    def __init__(
-        self,
-        mtproto_bridge,
-        audio_input_device: Optional[str] = None,
-        audio_output_device: Optional[str] = None,
-        enable_logs_to_console=False,
-        path_to_log_file=None,
-        outgoing_audio_bitrate_kbit=128,
-    ):
-        super().__init__(mtproto_bridge, enable_logs_to_console, path_to_log_file, outgoing_audio_bitrate_kbit)
-
-        self.__is_playout_paused = False
-        self.__is_recording_paused = False
-
-        self.__audio_input_device = audio_input_device or ''
-        self.__audio_output_device = audio_output_device or ''
-
-    def _setup_and_start_group_call(self):
-        self._start_native_group_call(self.__audio_input_device, self.__audio_output_device)
-
-    @property
-    def audio_input_device(self):
-        """Get audio input device name or GUID
-
-        Note:
-            To get system recording device list you can use `get_recording_devices()` method.
-        """
-
-        return self.__audio_input_device
-
-    @audio_input_device.setter
-    def audio_input_device(self, name=None):
-        self.set_audio_input_device(name)
-
-    @property
-    def audio_output_device(self):
-        """Get audio output device name or GUID
-
-        Note:
-            To get system playout device list you can use `get_playout_devices()` method.
-        """
-
-        return self.__audio_output_device
-
-    @audio_output_device.setter
-    def audio_output_device(self, name=None):
-        self.set_audio_output_device(name)
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from typing import Optional
+
+from pytgcalls.implementation import GroupCallBase
+
+
+class GroupCallDevice(GroupCallBase):
+    def __init__(
+        self,
+        mtproto_bridge,
+        audio_input_device: Optional[str] = None,
+        audio_output_device: Optional[str] = None,
+        enable_logs_to_console=False,
+        path_to_log_file=None,
+        outgoing_audio_bitrate_kbit=128,
+    ):
+        super().__init__(mtproto_bridge, enable_logs_to_console, path_to_log_file, outgoing_audio_bitrate_kbit)
+
+        self.__is_playout_paused = False
+        self.__is_recording_paused = False
+
+        self.__audio_input_device = audio_input_device or ''
+        self.__audio_output_device = audio_output_device or ''
+
+    def _setup_and_start_group_call(self):
+        self._start_native_group_call(self.__audio_input_device, self.__audio_output_device)
+
+    @property
+    def audio_input_device(self):
+        """Get audio input device name or GUID
+
+        Note:
+            To get system recording device list you can use `get_recording_devices()` method.
+        """
+
+        return self.__audio_input_device
+
+    @audio_input_device.setter
+    def audio_input_device(self, name=None):
+        self.set_audio_input_device(name)
+
+    @property
+    def audio_output_device(self):
+        """Get audio output device name or GUID
+
+        Note:
+            To get system playout device list you can use `get_playout_devices()` method.
+        """
+
+        return self.__audio_output_device
+
+    @audio_output_device.setter
+    def audio_output_device(self, name=None):
+        self.set_audio_output_device(name)
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/__init__.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/data/update/update_group_call_participants_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from pytgcalls.mtproto.base_bridge import MTProtoBridgeBase
-
-__all__ = [
-    'MTProtoBridgeBase',
-]
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from typing import List, TYPE_CHECKING
+
+from pytgcalls.mtproto.data import WrapperBase
+
+if TYPE_CHECKING:
+    from pytgcalls.mtproto.data import GroupCallParticipantWrapper
+
+
+class UpdateGroupCallParticipantsWrapper(WrapperBase):
+    def __init__(self, participants: List['GroupCallParticipantWrapper']):
+        self.participants = participants
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/data/__init__.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/data/update/update_group_call_wrapper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from .base_wrapper import WrapperBase
-from .group_call_wrapper import GroupCallWrapper
-from .group_call_discarded_wrapper import GroupCallDiscardedWrapper
-from .group_call_participant_wrapper import GroupCallParticipantWrapper
-
-__all__ = [
-    'WrapperBase',
-    'GroupCallWrapper',
-    'GroupCallDiscardedWrapper',
-    'GroupCallParticipantWrapper',
-]
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from typing import TYPE_CHECKING, Union
+
+from pytgcalls.mtproto.data import WrapperBase
+
+if TYPE_CHECKING:
+    from pytgcalls.mtproto.data import GroupCallWrapper, GroupCallDiscardedWrapper
+
+
+class UpdateGroupCallWrapper(WrapperBase):
+    def __init__(self, chat_id: int, call: Union['GroupCallWrapper', 'GroupCallDiscardedWrapper']):
+        self.chat_id = chat_id
+        self.call = call
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/data/base_wrapper.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/data/update/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-
-class WrapperBase:
-    __slots__ = '__dict__'
-
-    def __repr__(self):
-        return f'<{self.__class__.__name__}>({vars(self)})'
-
-    def __str__(self):
-        return repr(self)
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from .update_group_call_participants_wrapper import UpdateGroupCallParticipantsWrapper
+from .update_group_call_wrapper import UpdateGroupCallWrapper
+
+__all__ = [
+    'UpdateGroupCallParticipantsWrapper',
+    'UpdateGroupCallWrapper',
+]
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_discarded_wrapper.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/data/group_call_discarded_wrapper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from pytgcalls.mtproto.data import WrapperBase
-
-
-class GroupCallDiscardedWrapper(WrapperBase):
-    def __init__(self):
-        pass
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from pytgcalls.mtproto.data import WrapperBase
+
+
+class GroupCallDiscardedWrapper(WrapperBase):
+    def __init__(self):
+        pass
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/data/group_call_participant_wrapper.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/data/group_call_participant_wrapper.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from datetime import datetime
-from typing import Optional, Union
-
-from pytgcalls.mtproto.data import WrapperBase
-
-
-class GroupCallParticipantWrapper(WrapperBase):
-    """Group Call Participant wrapper for any MTProto client.
-
-    Note:
-        `peer` will be `raw.base.Peer` when you are using Fipper bridge.
-
-        `peer` will be `TypePeer` when you are using Telethon bridge.
-
-        `date` and `active_date`will be `int` when you are using Fipper bridge.
-
-        `date` and `active_date`will be `datetime` when you are using Telethon bridge.
-
-        `video_joined` always will be `None` for Fipper until it will update.
-    """
-
-    def __init__(
-        self,
-        peer: Union['raw.base.Peer', 'TypePeer'],
-        date: Optional[Union[int, datetime]],
-        source: int,
-        muted: Optional[bool] = None,
-        left: Optional[bool] = None,
-        can_self_unmute: Optional[bool] = None,
-        just_joined: Optional[bool] = None,
-        versioned: Optional[bool] = None,
-        min: Optional[bool] = None,
-        muted_by_you: Optional[bool] = None,
-        volume_by_admin: Optional[bool] = None,
-        is_self: Optional[bool] = None,
-        video_joined: Optional[bool] = None,
-        active_date: Optional[Union[int, datetime]] = None,
-        volume: Optional[int] = None,
-        about: Optional[str] = None,
-        raise_hand_rating: Optional[int] = None,
-        **kwargs,  # to bypass new attr from layers
-    ):
-        self.peer = peer
-        '''Peer (as joined) of the group call participant'''
-        self.date = date
-        self.source = source
-        '''User's audio channel synchronization source identifier'''
-        self.muted = muted
-        '''True, if the participant is muted for all users'''
-        self.left = left
-        '''True, if the participant left the group call'''
-        self.can_self_unmute = can_self_unmute
-        '''True, if the participant is muted for all users, but can unmute themselves'''
-        self.just_joined = just_joined
-        self.versioned = versioned
-        self.min = min
-        self.muted_by_you = muted_by_you
-        '''True, if the current user can mute the participant only for self'''
-        self.volume_by_admin = volume_by_admin
-        self.is_self = is_self
-        '''True, if the participant is the current user'''
-        self.video_joined = video_joined
-        self.active_date = active_date
-        self.volume = volume
-        '''Participant's volume level'''
-        self.about = about
-        '''The participant user's bio or the participant chat's description'''
-        self.raise_hand_rating = raise_hand_rating
-
-    @classmethod
-    def create(cls, participant):
-        if hasattr(participant, '__slots__'):  # fipper
-            attrs = participant.__slots__
-            args_for_init = {}
-            for attr in attrs:
-                args_for_init[attr] = getattr(participant, attr, None)
-
-            return cls(**args_for_init)
-        else:  # telethon
-            return cls(**vars(participant))
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from datetime import datetime
+from typing import Optional, Union
+
+from pytgcalls.mtproto.data import WrapperBase
+
+
+class GroupCallParticipantWrapper(WrapperBase):
+    """Group Call Participant wrapper for any MTProto client.
+
+    Note:
+        `peer` will be `raw.base.Peer` when you are using Fipper bridge.
+
+        `peer` will be `TypePeer` when you are using Telethon bridge.
+
+        `date` and `active_date`will be `int` when you are using Fipper bridge.
+
+        `date` and `active_date`will be `datetime` when you are using Telethon bridge.
+
+        `video_joined` always will be `None` for Fipper until it will update.
+    """
+
+    def __init__(
+        self,
+        peer: Union['raw.base.Peer', 'TypePeer'],
+        date: Optional[Union[int, datetime]],
+        source: int,
+        muted: Optional[bool] = None,
+        left: Optional[bool] = None,
+        can_self_unmute: Optional[bool] = None,
+        just_joined: Optional[bool] = None,
+        versioned: Optional[bool] = None,
+        min: Optional[bool] = None,
+        muted_by_you: Optional[bool] = None,
+        volume_by_admin: Optional[bool] = None,
+        is_self: Optional[bool] = None,
+        video_joined: Optional[bool] = None,
+        active_date: Optional[Union[int, datetime]] = None,
+        volume: Optional[int] = None,
+        about: Optional[str] = None,
+        raise_hand_rating: Optional[int] = None,
+        **kwargs,  # to bypass new attr from layers
+    ):
+        self.peer = peer
+        '''Peer (as joined) of the group call participant'''
+        self.date = date
+        self.source = source
+        '''User's audio channel synchronization source identifier'''
+        self.muted = muted
+        '''True, if the participant is muted for all users'''
+        self.left = left
+        '''True, if the participant left the group call'''
+        self.can_self_unmute = can_self_unmute
+        '''True, if the participant is muted for all users, but can unmute themselves'''
+        self.just_joined = just_joined
+        self.versioned = versioned
+        self.min = min
+        self.muted_by_you = muted_by_you
+        '''True, if the current user can mute the participant only for self'''
+        self.volume_by_admin = volume_by_admin
+        self.is_self = is_self
+        '''True, if the participant is the current user'''
+        self.video_joined = video_joined
+        self.active_date = active_date
+        self.volume = volume
+        '''Participant's volume level'''
+        self.about = about
+        '''The participant user's bio or the participant chat's description'''
+        self.raise_hand_rating = raise_hand_rating
+
+    @classmethod
+    def create(cls, participant):
+        if hasattr(participant, '__slots__'):  # fipper
+            attrs = participant.__slots__
+            args_for_init = {}
+            for attr in attrs:
+                args_for_init[attr] = getattr(participant, attr, None)
+
+            return cls(**args_for_init)
+        else:  # telethon
+            return cls(**vars(participant))
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/data/update/update_group_call_wrapper.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/data/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from typing import TYPE_CHECKING, Union
-
-from pytgcalls.mtproto.data import WrapperBase
-
-if TYPE_CHECKING:
-    from pytgcalls.mtproto.data import GroupCallWrapper, GroupCallDiscardedWrapper
-
-
-class UpdateGroupCallWrapper(WrapperBase):
-    def __init__(self, chat_id: int, call: Union['GroupCallWrapper', 'GroupCallDiscardedWrapper']):
-        self.chat_id = chat_id
-        self.call = call
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from .base_wrapper import WrapperBase
+from .group_call_wrapper import GroupCallWrapper
+from .group_call_discarded_wrapper import GroupCallDiscardedWrapper
+from .group_call_participant_wrapper import GroupCallParticipantWrapper
+
+__all__ = [
+    'WrapperBase',
+    'GroupCallWrapper',
+    'GroupCallDiscardedWrapper',
+    'GroupCallParticipantWrapper',
+]
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/exceptions.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-
-class GroupcallSsrcDuplicateMuch(Exception):
-    pass
-
-
-class BadRequest(Exception):
-    pass
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from pytgcalls.mtproto.base_bridge import MTProtoBridgeBase
+
+__all__ = [
+    'MTProtoBridgeBase',
+]
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto/fipper_bridge.py` & `yins-music-0.0.7.dev3/pytgcalls/mtproto/fipper_bridge.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from asyncio import AbstractEventLoop
-from typing import Callable
-
-from fipper.errors import (
-    BadRequest as FipperBadRequest,
-    GroupcallSsrcDuplicateMuch as FipperGroupcallSsrcDuplicateMuch,
-)
-from fipper.handlers import RawUpdateHandler
-from fipper.raw import functions, types
-from fipper.raw.types import (
-    GroupCallDiscarded as FipperGroupCallDiscarded,
-    InputPeerChannel,
-    InputPeerChat,
-    UpdateGroupCallConnection,
-)
-from fipper.utils import get_peer_id
-
-from pytgcalls import PytgcallsError
-from pytgcalls.mtproto.data import GroupCallDiscardedWrapper, GroupCallWrapper, GroupCallParticipantWrapper
-from pytgcalls.mtproto.data.update import UpdateGroupCallWrapper, UpdateGroupCallParticipantsWrapper
-from pytgcalls.mtproto.exceptions import BadRequest, GroupcallSsrcDuplicateMuch
-from pytgcalls.utils import int_ssrc
-
-from fipper import Client, ContinuePropagation
-
-from pytgcalls.mtproto import MTProtoBridgeBase
-
-
-class FipperBridge(MTProtoBridgeBase):
-    def __init__(self, client: Client):
-        super().__init__(client)
-
-        # compatibility with pyro > 2.0
-        if getattr(client, 'send', None) is None:
-            setattr(client, 'send', getattr(client, 'invoke'))
-
-        self._update_to_handler = {
-            types.UpdateGroupCallParticipants: self._process_group_call_participants_update,
-            types.UpdateGroupCall: self._process_group_call_update,
-        }
-
-        self._handler_group = None
-        self._update_handler = RawUpdateHandler(self._process_update)
-
-    async def _process_update(self, _, update, users, chats):
-        if type(update) not in self._update_to_handler.keys():
-            raise ContinuePropagation
-
-        if not self.group_call or not update.call or update.call.id != self.group_call.id:
-            raise ContinuePropagation
-        self.group_call = update.call
-
-        await self._update_to_handler[type(update)](update)
-
-    async def _process_group_call_participants_update(self, update):
-        participants = [GroupCallParticipantWrapper.create(p) for p in update.participants]
-        wrapped_update = UpdateGroupCallParticipantsWrapper(participants)
-
-        await self.group_call_participants_update_callback(wrapped_update)
-
-    async def _process_group_call_update(self, update):
-        if not isinstance(update.call, FipperGroupCallDiscarded):
-            return
-
-        call = GroupCallDiscardedWrapper()  # no info needed
-        wrapped_update = UpdateGroupCallWrapper(update.chat_id, call)
-
-        await self.group_call_update_callback(wrapped_update)
-
-    async def _process_group_call_connection(self, update):
-        # TODO update to new layer when fipper will release new stable version on pypi
-        call = GroupCallWrapper('placeholder', update.params)
-        wrapped_update = UpdateGroupCallWrapper('placeholder', call)
-
-        await self.group_call_update_callback(wrapped_update)
-
-    async def check_group_call(self) -> bool:
-        if not self.group_call or not self.my_ssrc:
-            return False
-
-        try:
-            in_group_call = await (
-                self.client.send(functions.phone.CheckGroupCall(call=self.group_call, source=int_ssrc(self.my_ssrc)))
-            )
-        except FipperBadRequest as e:
-            # compatibility with pyro > 2.0
-            if getattr(e, 'x', None) is None:
-                setattr(e, 'x', getattr(e, 'value'))
-
-            if e.x != '[400 GROUPCALL_JOIN_MISSING]':
-                raise BadRequest(e.x)
-
-            in_group_call = False
-
-        return in_group_call
-
-    async def leave_current_group_call(self):
-        if not self.full_chat or not self.full_chat.call or not self.my_ssrc:
-            return
-
-        response = await self.client.send(
-            functions.phone.LeaveGroupCall(call=self.full_chat.call, source=int_ssrc(self.my_ssrc))
-        )
-        await self.handle_updates(response)
-
-    async def edit_group_call_member(
-        self, peer, volume: int = None, muted=False, video_stopped=True, video_paused=False
-    ):
-        response = await self.client.send(
-            functions.phone.EditGroupCallParticipant(
-                call=self.full_chat.call,
-                participant=peer,
-                muted=muted,
-                volume=volume,
-                video_stopped=video_stopped,
-                video_paused=video_paused,
-            )
-        )
-        await self.handle_updates(response)
-
-    async def get_and_set_self_peer(self):
-        self.my_peer = await self.client.resolve_peer(await self.client.storage.user_id())
-
-        return self.my_peer
-
-    async def get_and_set_group_call(self, group):
-        """Get group call input of chat.
-
-        Args:
-            group (`InputPeerChannel` | `InputPeerChat` | `str` | `int`): Chat ID in any form.
-
-        Returns:
-            `InputGroupCall`.
-        """
-
-        self.chat_peer = group
-        if type(group) not in [InputPeerChannel, InputPeerChat]:
-            self.chat_peer = await self.client.resolve_peer(group)
-
-        if isinstance(self.chat_peer, InputPeerChannel):
-            self.full_chat = (
-                await (self.client.send(functions.channels.GetFullChannel(channel=self.chat_peer)))
-            ).full_chat
-        elif isinstance(self.chat_peer, InputPeerChat):
-            self.full_chat = (
-                await (self.client.send(functions.messages.GetFullChat(chat_id=self.chat_peer.chat_id)))
-            ).full_chat
-
-        if self.full_chat is None:
-            raise PytgcallsError(f'Can\'t get full chat by {group}')
-
-        self.group_call = self.full_chat.call
-
-        return self.group_call
-
-    def unregister_update_handlers(self):
-        if self._handler_group:
-            self.client.remove_handler(self._update_handler, self._handler_group)
-            self._handler_group = None
-
-    def register_update_handlers(self):
-        if self.group_call.id > 0:
-            self._handler_group = -self.group_call.id
-        self._handler_group = self.group_call.id
-
-        self.client.add_handler(self._update_handler, self._handler_group)
-
-    async def resolve_and_set_join_as(self, join_as):
-        my_peer = await self.get_and_set_self_peer()
-
-        if join_as is None:
-            self.join_as = self.full_chat.groupcall_default_join_as
-            if self.join_as:
-                # convert Peer to InputPeer
-                self.join_as = await self.client.resolve_peer(get_peer_id(self.join_as))
-            else:
-                self.join_as = my_peer
-        elif isinstance(join_as, str) or isinstance(join_as, int):
-            self.join_as = await self.client.resolve_peer(join_as)
-        else:
-            self.join_as = join_as
-
-    async def send_speaking_group_call_action(self):
-        await self.client.send(
-            functions.messages.SetTyping(peer=self.chat_peer, action=types.SpeakingInGroupCallAction())
-        )
-
-    async def join_group_call(
-        self, invite_hash: str, params: str, muted: bool, video_stopped: bool, pre_update_processing: Callable
-    ):
-        try:
-            response = await self.client.send(
-                functions.phone.JoinGroupCall(
-                    call=self.group_call,
-                    join_as=self.join_as,
-                    invite_hash=invite_hash,
-                    params=types.DataJSON(data=params),
-                    muted=muted,
-                    video_stopped=video_stopped,
-                )
-            )
-
-            pre_update_processing()
-
-            # it is here cuz we need to associate params for connection with group call
-            for update in response.updates:
-                if isinstance(update, UpdateGroupCallConnection):
-                    await self._process_group_call_connection(update)
-
-            await self.handle_updates(response)
-        except FipperGroupcallSsrcDuplicateMuch as e:
-            # compatibility with pyro > 2.0
-            if getattr(e, 'x', None) is None:
-                setattr(e, 'x', getattr(e, 'value'))
-
-            raise GroupcallSsrcDuplicateMuch(e.x)
-
-    async def handle_updates(self, updates):
-        await self.client.handle_updates(updates)
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from asyncio import AbstractEventLoop
+from typing import Callable
+
+from fipper.errors import (
+    BadRequest as FipperBadRequest,
+    GroupcallSsrcDuplicateMuch as FipperGroupcallSsrcDuplicateMuch,
+)
+from fipper.handlers import RawUpdateHandler
+from fipper.raw import functions, types
+from fipper.raw.types import (
+    GroupCallDiscarded as FipperGroupCallDiscarded,
+    InputPeerChannel,
+    InputPeerChat,
+    UpdateGroupCallConnection,
+)
+from fipper.utils import get_peer_id
+
+from pytgcalls import PytgcallsError
+from pytgcalls.mtproto.data import GroupCallDiscardedWrapper, GroupCallWrapper, GroupCallParticipantWrapper
+from pytgcalls.mtproto.data.update import UpdateGroupCallWrapper, UpdateGroupCallParticipantsWrapper
+from pytgcalls.mtproto.exceptions import BadRequest, GroupcallSsrcDuplicateMuch
+from pytgcalls.utils import int_ssrc
+
+from fipper import Client, ContinuePropagation
+
+from pytgcalls.mtproto import MTProtoBridgeBase
+
+
+class FipperBridge(MTProtoBridgeBase):
+    def __init__(self, client: Client):
+        super().__init__(client)
+
+        # compatibility with pyro > 2.0
+        if getattr(client, 'send', None) is None:
+            setattr(client, 'send', getattr(client, 'invoke'))
+
+        self._update_to_handler = {
+            types.UpdateGroupCallParticipants: self._process_group_call_participants_update,
+            types.UpdateGroupCall: self._process_group_call_update,
+        }
+
+        self._handler_group = None
+        self._update_handler = RawUpdateHandler(self._process_update)
+
+    async def _process_update(self, _, update, users, chats):
+        if type(update) not in self._update_to_handler.keys():
+            raise ContinuePropagation
+
+        if not self.group_call or not update.call or update.call.id != self.group_call.id:
+            raise ContinuePropagation
+        self.group_call = update.call
+
+        await self._update_to_handler[type(update)](update)
+
+    async def _process_group_call_participants_update(self, update):
+        participants = [GroupCallParticipantWrapper.create(p) for p in update.participants]
+        wrapped_update = UpdateGroupCallParticipantsWrapper(participants)
+
+        await self.group_call_participants_update_callback(wrapped_update)
+
+    async def _process_group_call_update(self, update):
+        if not isinstance(update.call, FipperGroupCallDiscarded):
+            return
+
+        call = GroupCallDiscardedWrapper()  # no info needed
+        wrapped_update = UpdateGroupCallWrapper(update.chat_id, call)
+
+        await self.group_call_update_callback(wrapped_update)
+
+    async def _process_group_call_connection(self, update):
+        # TODO update to new layer when fipper will release new stable version on pypi
+        call = GroupCallWrapper('placeholder', update.params)
+        wrapped_update = UpdateGroupCallWrapper('placeholder', call)
+
+        await self.group_call_update_callback(wrapped_update)
+
+    async def check_group_call(self) -> bool:
+        if not self.group_call or not self.my_ssrc:
+            return False
+
+        try:
+            in_group_call = await (
+                self.client.send(functions.phone.CheckGroupCall(call=self.group_call, source=int_ssrc(self.my_ssrc)))
+            )
+        except FipperBadRequest as e:
+            # compatibility with pyro > 2.0
+            if getattr(e, 'x', None) is None:
+                setattr(e, 'x', getattr(e, 'value'))
+
+            if e.x != '[400 GROUPCALL_JOIN_MISSING]':
+                raise BadRequest(e.x)
+
+            in_group_call = False
+
+        return in_group_call
+
+    async def leave_current_group_call(self):
+        if not self.full_chat or not self.full_chat.call or not self.my_ssrc:
+            return
+
+        response = await self.client.send(
+            functions.phone.LeaveGroupCall(call=self.full_chat.call, source=int_ssrc(self.my_ssrc))
+        )
+        await self.handle_updates(response)
+
+    async def edit_group_call_member(
+        self, peer, volume: int = None, muted=False, video_stopped=True, video_paused=False
+    ):
+        response = await self.client.send(
+            functions.phone.EditGroupCallParticipant(
+                call=self.full_chat.call,
+                participant=peer,
+                muted=muted,
+                volume=volume,
+                video_stopped=video_stopped,
+                video_paused=video_paused,
+            )
+        )
+        await self.handle_updates(response)
+
+    async def get_and_set_self_peer(self):
+        self.my_peer = await self.client.resolve_peer(await self.client.storage.user_id())
+
+        return self.my_peer
+
+    async def get_and_set_group_call(self, group):
+        """Get group call input of chat.
+
+        Args:
+            group (`InputPeerChannel` | `InputPeerChat` | `str` | `int`): Chat ID in any form.
+
+        Returns:
+            `InputGroupCall`.
+        """
+
+        self.chat_peer = group
+        if type(group) not in [InputPeerChannel, InputPeerChat]:
+            self.chat_peer = await self.client.resolve_peer(group)
+
+        if isinstance(self.chat_peer, InputPeerChannel):
+            self.full_chat = (
+                await (self.client.send(functions.channels.GetFullChannel(channel=self.chat_peer)))
+            ).full_chat
+        elif isinstance(self.chat_peer, InputPeerChat):
+            self.full_chat = (
+                await (self.client.send(functions.messages.GetFullChat(chat_id=self.chat_peer.chat_id)))
+            ).full_chat
+
+        if self.full_chat is None:
+            raise PytgcallsError(f'Can\'t get full chat by {group}')
+
+        self.group_call = self.full_chat.call
+
+        return self.group_call
+
+    def unregister_update_handlers(self):
+        if self._handler_group:
+            self.client.remove_handler(self._update_handler, self._handler_group)
+            self._handler_group = None
+
+    def register_update_handlers(self):
+        if self.group_call.id > 0:
+            self._handler_group = -self.group_call.id
+        self._handler_group = self.group_call.id
+
+        self.client.add_handler(self._update_handler, self._handler_group)
+
+    async def resolve_and_set_join_as(self, join_as):
+        my_peer = await self.get_and_set_self_peer()
+
+        if join_as is None:
+            self.join_as = self.full_chat.groupcall_default_join_as
+            if self.join_as:
+                # convert Peer to InputPeer
+                self.join_as = await self.client.resolve_peer(get_peer_id(self.join_as))
+            else:
+                self.join_as = my_peer
+        elif isinstance(join_as, str) or isinstance(join_as, int):
+            self.join_as = await self.client.resolve_peer(join_as)
+        else:
+            self.join_as = join_as
+
+    async def send_speaking_group_call_action(self):
+        await self.client.send(
+            functions.messages.SetTyping(peer=self.chat_peer, action=types.SpeakingInGroupCallAction())
+        )
+
+    async def join_group_call(
+        self, invite_hash: str, params: str, muted: bool, video_stopped: bool, pre_update_processing: Callable
+    ):
+        try:
+            response = await self.client.send(
+                functions.phone.JoinGroupCall(
+                    call=self.group_call,
+                    join_as=self.join_as,
+                    invite_hash=invite_hash,
+                    params=types.DataJSON(data=params),
+                    muted=muted,
+                    video_stopped=video_stopped,
+                )
+            )
+
+            pre_update_processing()
+
+            # it is here cuz we need to associate params for connection with group call
+            for update in response.updates:
+                if isinstance(update, UpdateGroupCallConnection):
+                    await self._process_group_call_connection(update)
+
+            await self.handle_updates(response)
+        except FipperGroupcallSsrcDuplicateMuch as e:
+            # compatibility with pyro > 2.0
+            if getattr(e, 'x', None) is None:
+                setattr(e, 'x', getattr(e, 'value'))
+
+            raise GroupcallSsrcDuplicateMuch(e.x)
+
+    async def handle_updates(self, updates):
+        await self.client.handle_updates(updates)
```

### Comparing `yins-music-0.0.7.dev2/pytgcalls/mtproto_client_type.py` & `yins-music-0.0.7.dev3/pytgcalls/dispatcher/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from enum import Enum
-
-
-class MTProtoClientType(Enum):
-    FIPPER = 'fipper'
-    TELETHON = 'telethon'
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from pytgcalls.dispatcher.action import Action
+from pytgcalls.dispatcher.dispatcher import Dispatcher
+from pytgcalls.dispatcher.dispatcher_mixin import DispatcherMixin
+
+__all__ = [
+    'Action',
+    'Dispatcher',
+    'DispatcherMixin',
+]
```

### Comparing `yins-music-0.0.7.dev2/setup.py` & `yins-music-0.0.7.dev3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-#  tgcalls - a Python binding for C++ library by Telegram
-#  pytgcalls - a library connecting the Python binding with MTProto
-#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
-#
-#  This file is part of tgcalls and pytgcalls.
-#
-#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License v3
-#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
-
-from os import path
-import re
-
-from setuptools import setup, find_packages
-
-base_path = path.abspath(path.dirname(__file__))
-packages = find_packages()
-
-with open(path.join(base_path, 'pytgcalls/__init__.py'), encoding='utf-8') as f:
-    version = re.findall(r"__version__ = '(.+)'", f.read())[0]
-
-with open(path.join(base_path, 'README.md'), 'r', encoding='utf-8') as f:
-    readme = f.read()
-
-setup(
-    name='yins-music',
-    version=version,
-    author='AyiinXd',
-    author_email='ayiinxd0307@gmail.com',
-    license='LGPLv3',
-    url='https://github.com/MarshalX/tgcalls',
-    keywords='python, library, telegram, async, asynchronous, webrtc, lib, voice-chat, '
-    'voip, group-chat, video-call, calls, fipper, telethon, pytgcalls, tgcalls',
-    description='a library connecting the tgcalls Python binding with MTProto',
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    packages=packages,
-    install_requires=[
-        'tgcalls == 3.0.0.dev6',
-        'av~=8.0',
-        'opencv-python-headless~=4.5'
-    ],
-    extras_require={
-        'fipper': ['fipper >= 0.0.1.dev3'],
-        'telethon': ['telethon >= 1.24.0'],
-    },
-    python_requires="~=3.7",
-    include_package_data=True,
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Natural Language :: English',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Operating System :: OS Independent',
-        'Operating System :: MacOS',
-        'Operating System :: Unix',
-        'Topic :: Internet',
-        'Topic :: Multimedia',
-        'Topic :: Multimedia :: Video',
-        'Topic :: Multimedia :: Video :: Capture',
-        'Topic :: Multimedia :: Sound/Audio',
-        'Topic :: Multimedia :: Sound/Audio :: Capture/Recording',
-        'Topic :: Communications',
-        'Topic :: Communications :: Internet Phone',
-        'Topic :: Communications :: Telephony',
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        "Programming Language :: Python :: Implementation",
-        "Programming Language :: Python :: Implementation :: CPython",
-    ],
-    project_urls={
-        'Documentation': 'https://tgcalls.org/',
-        'Telegram Channel': 'https://t.me/tgcallslib',
-        'Telegram Chat': 'https://t.me/tgcallschat',
-        'Author': 'https://github.com/AyiinXd',
-    },
-)
+#  tgcalls - a Python binding for C++ library by Telegram
+#  pytgcalls - a library connecting the Python binding with MTProto
+#  Copyright (C) 2020-2021 Il`ya (Marshal) <https://github.com/MarshalX>
+#
+#  This file is part of tgcalls and pytgcalls.
+#
+#  tgcalls and pytgcalls is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
+#
+#  tgcalls and pytgcalls is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
+#
+#  You should have received a copy of the GNU Lesser General Public License v3
+#  along with tgcalls. If not, see <http://www.gnu.org/licenses/>.
+
+from os import path
+import re
+
+from setuptools import setup, find_packages
+
+base_path = path.abspath(path.dirname(__file__))
+packages = find_packages()
+
+with open(path.join(base_path, 'pytgcalls/__init__.py'), encoding='utf-8') as f:
+    version = re.findall(r"__version__ = '(.+)'", f.read())[0]
+
+with open(path.join(base_path, 'README.md'), 'r', encoding='utf-8') as f:
+    readme = f.read()
+
+setup(
+    name='yins-music',
+    version=version,
+    author='AyiinXd',
+    author_email='ayiinxd0307@gmail.com',
+    license='LGPLv3',
+    url='https://github.com/MarshalX/tgcalls',
+    keywords='python, library, telegram, async, asynchronous, webrtc, lib, voice-chat, '
+    'voip, group-chat, video-call, calls, fipper, telethon, pytgcalls, tgcalls',
+    description='a library connecting the tgcalls Python binding with MTProto',
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    packages=packages,
+    install_requires=[
+        'tgcalls == 3.0.0.dev5',
+        'av~=8.0',
+        'opencv-python-headless~=4.5'
+    ],
+    extras_require={
+        'fipper': ['fipper >= 0.0.1.dev3'],
+        'telethon': ['telethon >= 1.24.0'],
+    },
+    python_requires="~=3.7",
+    include_package_data=True,
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Natural Language :: English',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
+        'Operating System :: OS Independent',
+        'Operating System :: MacOS',
+        'Operating System :: Unix',
+        'Topic :: Internet',
+        'Topic :: Multimedia',
+        'Topic :: Multimedia :: Video',
+        'Topic :: Multimedia :: Video :: Capture',
+        'Topic :: Multimedia :: Sound/Audio',
+        'Topic :: Multimedia :: Sound/Audio :: Capture/Recording',
+        'Topic :: Communications',
+        'Topic :: Communications :: Internet Phone',
+        'Topic :: Communications :: Telephony',
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        "Programming Language :: Python :: Implementation",
+        "Programming Language :: Python :: Implementation :: CPython",
+    ],
+    project_urls={
+        'Documentation': 'https://tgcalls.org/',
+        'Telegram Channel': 'https://t.me/tgcallslib',
+        'Telegram Chat': 'https://t.me/tgcallschat',
+        'Author': 'https://github.com/AyiinXd',
+    },
+)
```

### Comparing `yins-music-0.0.7.dev2/yins_music.egg-info/PKG-INFO` & `yins-music-0.0.7.dev3/yins_music.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-Metadata-Version: 2.1
-Name: yins-music
-Version: 0.0.7.dev2
-Summary: a library connecting the tgcalls Python binding with MTProto
-Home-page: https://github.com/MarshalX/tgcalls
-Author: AyiinXd
-Author-email: ayiinxd0307@gmail.com
-License: LGPLv3
-Project-URL: Documentation, https://tgcalls.org/
-Project-URL: Telegram Channel, https://t.me/tgcallslib
-Project-URL: Telegram Chat, https://t.me/tgcallschat
-Project-URL: Author, https://github.com/AyiinXd
-Keywords: python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Classifier: Topic :: Internet
-Classifier: Topic :: Multimedia
-Classifier: Topic :: Multimedia :: Video
-Classifier: Topic :: Multimedia :: Video :: Capture
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
-Classifier: Topic :: Communications
-Classifier: Topic :: Communications :: Internet Phone
-Classifier: Topic :: Communications :: Telephony
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: fipper
-Provides-Extra: telethon
-License-File: LICENSE
-
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/logo.png" alt="tgcalls">
-    </a>
-    <br>
-    <b>Voice chats, private incoming and outgoing calls in Telegram for Developers</b>
-    <br>
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/examples">
-        Examples
-    </a>
-    •
-    <a href="https://tgcalls.org">
-        Documentation
-    </a>
-    •
-    <a href="https://t.me/tgcallslib">
-        Channel
-    </a>
-    •
-    <a href="https://t.me/tgcallschat">
-        Chat
-    </a>
-</p>
-
-## Telegram WebRTC (VoIP) [![Mentioned in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)
-
-This project consists of two main parts: [tgcalls](#tgcalls), [pytgcalls](#pytgcalls).
-The first is a C++ Python extension.
-The second uses the extension along with MTProto and provides high level SDK.
-All together, it allows you to create userbots that can record and
-broadcast in voice chats, make and receive private calls.
-
-#### Fipper's snippet
-```python
-from fipper import Client, filters
-from fipper.utils import MAX_CHANNEL_ID
-
-from pytgcalls import GroupCallFactory
-
-app = Client('pytgcalls')
-group_call = GroupCallFactory(app).get_file_group_call('input.raw')
-
-
-@group_call.on_network_status_changed
-async def on_network_changed(context, is_connected):
-    chat_id = MAX_CHANNEL_ID - context.full_chat.id
-    if is_connected:
-        await app.send_message(chat_id, 'Successfully joined!')
-    else:
-        await app.send_message(chat_id, 'Disconnected from voice chat..')
-
-
-@app.on_message(filters.outgoing & filters.command('join'))
-async def join_handler(_, message):
-    await group_call.start(message.chat.id)
-
-
-app.run()
-```
-
-#### Telethon's snippet
-```python
-from telethon import TelegramClient, events
-
-from pytgcalls import GroupCallFactory
-
-app = TelegramClient('pytgcalls', api_id, api_hash).start()
-group_call_factory = GroupCallFactory(app, GroupCallFactory.MTPROTO_CLIENT_TYPE.TELETHON)
-group_call = group_call_factory.get_file_group_call('input.raw')
-
-
-@app.on(events.NewMessage(outgoing=True, pattern=r'^/join$'))
-async def join_handler(event):
-    chat = await event.get_chat()
-    await group_call.start(chat.id)
-
-app.run_until_disconnected()
-```
-
-### Features
-
-- Python solution.
-- Prebuilt wheels for macOS, Linux and Windows.
-- Supporting popular MTProto libraries: Fipper, Telethon.
-- Abstract class to implement own MTProto bridge.
-- Work with voice chats in channels and chats.
-- Multiply voice chats ([example](https://github.com/MarshalX/tgcalls/blob/main/examples/radio_as_smart_plugin.py)).
-- System of custom handlers on events.
-- Join as channels or chats.
-- Join using invite (speaker) links.
-- Speaking status with voice activity detection.
-- Mute/unmute, pause/resume, stop/play, volume control and more...
-
-### Available sources of input/output data transfers
-
-- Raw (`GroupCallRaw`, [example with pyav](https://github.com/MarshalX/tgcalls/blob/main/examples/pyav.py),
-[example of restreaming](https://github.com/MarshalX/tgcalls/blob/main/examples/restream_using_raw_data.py))
-  — to send and receive data in `bytes` directly from Python.
-- File (`GroupCallFile`, [playout example](https://github.com/MarshalX/tgcalls/blob/main/examples/file_playout.py),
-  [recording example](https://github.com/MarshalX/tgcalls/blob/main/examples/recorder_as_smart_plugin.py))
-  — to use audio files including named pipe (FIFO).
-- Device (`GroupCallDevice`, [example](https://github.com/MarshalX/tgcalls/blob/main/examples/device_playout.py)) — 
-to use system virtual devices. Please don't use it with real microphone, headphones, etc.
-
-Note: All audio data is transmitted in PCM 16 bit, 48k. 
-[Example how to convert files using FFmpeg](#audio-file-formats).
-
-### Requirements
-
-- Python 3.7 or higher.
-- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).
-
-### TODO list
-- Incoming and Outgoing private calls 
-(already there and working, but not in the release version).
-- Group Video Calls
-[and more...](https://github.com/MarshalX/tgcalls/issues)
-
-### Installing
-
-#### For Fipper
-``` bash
-pip3 install -U pytgcalls[pyrogram]
-```
-
-#### For Telethon
-``` bash
-pip3 install -U pytgcalls[telethon]
-```
-
-<hr>
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/tgcalls.png" alt="tgcalls">
-    </a>
-    <br>
-    <a href="https://pypi.org/project/tgcalls/">
-        PyPi
-    </a>
-    •
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/tgcalls">
-        Sources
-    </a>
-</p>
-
-## tgcalls 
-
-The first part of the project is C++ extensions for Python. [Pybind11](https://github.com/pybind/pybind11)
-was used to write it. Binding occurs to the [tgcalls](https://github.com/TelegramMessenger/tgcalls)
-library by Telegram, which is used in all official clients. 
-To implement the binding, the code of Telegram Desktop and Telegram Android was studied.
-Changes have been made to the Telegram library. 
-All modified code is [available as a subtree](https://github.com/MarshalX/tgcalls/tree/main/tgcalls/third_party/lib_tgcalls)
-in this repository. The main ideas of the changes is to improve 
-the sound quality and to add ability to work with third party audio device modules.
-In addition, this binding implemented custom audio modules. These modules are allowing
-transfer audio data directly from Python via bytes, transfer and control 
-the playback/recording of a file or a virtual system device.
-
-### How to build
-
-Short answer for Linux:
-```bash
-git clone git@github.com:MarshalX/tgcalls.git --recursive
-cd tgcalls
-```
-For x86_64:
-```bash
-docker-compose up tgcalls_x86_64
-```
-For AArch64 (ARM64):
-```bash
-docker-compose up tgcalls_aarch64
-```
-
-Python wheels will be available in `dist` folder in root of `tgcalls`.
-
-More info:
-- [Manylinux](build/manylinux/dev).
-- [Ubuntu](build/ubuntu).
-- [macOS](build/macos).
-- [Windows](build/windows).
-
-Also, you can investigate into [manylinux GitHub Actions builds](build/manylinux).
-
-### Documentation
-
-Temporarily, instead of documentation, you can use [an example](pytgcalls/pytgcalls)
-along with MTProto.
-
-<hr>
-<p align="center">
-    <a href="https://github.com/MarshalX/tgcalls">
-        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/pytgcalls.png" alt="pytgcalls">
-    </a>
-    <br>
-    <a href="https://tgcalls.org">
-        Documentation
-    </a>
-    •
-    <a href="https://pypi.org/project/pytgcalls/">
-        PyPi
-    </a>
-    •
-    <a href="https://github.com/MarshalX/tgcalls/tree/main/pytgcalls">
-        Sources
-    </a>
-</p>
-
-## pytgcalls 
-
-This project is implementation of using [tgcalls](#tgcalls) 
-Python binding together with [MTProto](https://core.telegram.org/mtproto).
-By default, this library are supports [Fipper](https://github.com/pyrogram/pyrogram)
-and [Telethon](https://github.com/LonamiWebs/Telethon) clients for working 
-with Telegram Mobile Protocol. 
-You can write your own implementation of abstract class to work with other libraries.
-
-### Learning by example
-
-Visit [this page](https://github.com/MarshalX/tgcalls/tree/main/examples) to discover the official examples.
-
-### Documentation
-
-`pytgcalls`'s documentation lives at [tgcalls.org](https://tgcalls.org).
-
-### Audio file formats
-
-RAW files are now used. You will have to convert to this format yourself
-using ffmpeg. The example how to transcode files from a code is available [here](https://github.com/MarshalX/tgcalls/blob/e0b2d667728cc92cc0da437b9c85bcc909e4ac9c/examples/player_as_smart_plugin.py#L41).
-
-From mp3 to raw (to play in voice chat):
-```
-ffmpeg -i input.mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-From raw to mp3 (files with recordings):
-```
-ffmpeg -f s16le -ac 2 -ar 48000 -acodec pcm_s16le -i output.raw clear_output.mp3
-```
-
-For playout live stream you can use this one:
-```
-ffmpeg -y -i http://stream2.cnmns.net/hope-mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-For YouTube videos and live streams you can use youtube-dl:
-```
-ffmpeg -i "$(youtube-dl -x -g "https://youtu.be/xhXq9BNndhw")" -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
-```
-
-And set input.raw as input filename.
-
-<hr>
-
-### Getting help
-
-You can get help in several ways:
-- We have a community of developers helping each other in our 
-[Telegram group](https://t.me/tgcallschat).
-- Report bugs, request new features or ask questions by creating 
-[an issue](https://github.com/MarshalX/tgcalls/issues/new) or 
-[a discussion](https://github.com/MarshalX/tgcalls/discussions/new).
-
-### Contributing
-
-Contributions of all sizes are welcome.
-
-### Special thanks to
-
-- [@FrayxRulez](https://github.com/FrayxRulez) for amazing code of [Unigram](https://github.com/UnigramDev/Unigram).
-- [@john-preston](https://github.com/john-preston) for [Telegram Desktop](https://github.com/telegramdesktop/tdesktop) and [tgcalls](https://github.com/TelegramMessenger/tgcalls).
-- [@bakatrouble](https://github.com/bakatrouble/) for help and inspiration by [pytgvoip](https://github.com/bakatrouble/pytgvoip).
-- [@delivrance](https://github.com/delivrance) for [Fipper](https://github.com/pyrogram/pyrogram).
-- [@Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon).
-
-### License
-
-You may copy, distribute and modify the software provided that modifications
-are described and licensed for free under [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html).
-Derivatives works (including modifications or anything statically
-linked to the library) can only be redistributed under LGPL-3, but
-applications that use the library don't have to be.
+Metadata-Version: 2.1
+Name: yins-music
+Version: 0.0.7.dev3
+Summary: a library connecting the tgcalls Python binding with MTProto
+Home-page: https://github.com/MarshalX/tgcalls
+Author: AyiinXd
+Author-email: ayiinxd0307@gmail.com
+License: LGPLv3
+Project-URL: Documentation, https://tgcalls.org/
+Project-URL: Telegram Channel, https://t.me/tgcallslib
+Project-URL: Telegram Chat, https://t.me/tgcallschat
+Project-URL: Author, https://github.com/AyiinXd
+Keywords: python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Classifier: Topic :: Internet
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Video
+Classifier: Topic :: Multimedia :: Video :: Capture
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
+Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Internet Phone
+Classifier: Topic :: Communications :: Telephony
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: ~=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: fipper
+Provides-Extra: telethon
+License-File: LICENSE
+
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/logo.png" alt="tgcalls">
+    </a>
+    <br>
+    <b>Voice chats, private incoming and outgoing calls in Telegram for Developers</b>
+    <br>
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/examples">
+        Examples
+    </a>
+    •
+    <a href="https://tgcalls.org">
+        Documentation
+    </a>
+    •
+    <a href="https://t.me/tgcallslib">
+        Channel
+    </a>
+    •
+    <a href="https://t.me/tgcallschat">
+        Chat
+    </a>
+</p>
+
+## Telegram WebRTC (VoIP) [![Mentioned in Awesome Telegram Calls](https://awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-tgcalls)
+
+This project consists of two main parts: [tgcalls](#tgcalls), [pytgcalls](#pytgcalls).
+The first is a C++ Python extension.
+The second uses the extension along with MTProto and provides high level SDK.
+All together, it allows you to create userbots that can record and
+broadcast in voice chats, make and receive private calls.
+
+#### Fipper's snippet
+```python
+from fipper import Client, filters
+from fipper.utils import MAX_CHANNEL_ID
+
+from pytgcalls import GroupCallFactory
+
+app = Client('pytgcalls')
+group_call = GroupCallFactory(app).get_file_group_call('input.raw')
+
+
+@group_call.on_network_status_changed
+async def on_network_changed(context, is_connected):
+    chat_id = MAX_CHANNEL_ID - context.full_chat.id
+    if is_connected:
+        await app.send_message(chat_id, 'Successfully joined!')
+    else:
+        await app.send_message(chat_id, 'Disconnected from voice chat..')
+
+
+@app.on_message(filters.outgoing & filters.command('join'))
+async def join_handler(_, message):
+    await group_call.start(message.chat.id)
+
+
+app.run()
+```
+
+#### Telethon's snippet
+```python
+from telethon import TelegramClient, events
+
+from pytgcalls import GroupCallFactory
+
+app = TelegramClient('pytgcalls', api_id, api_hash).start()
+group_call_factory = GroupCallFactory(app, GroupCallFactory.MTPROTO_CLIENT_TYPE.TELETHON)
+group_call = group_call_factory.get_file_group_call('input.raw')
+
+
+@app.on(events.NewMessage(outgoing=True, pattern=r'^/join$'))
+async def join_handler(event):
+    chat = await event.get_chat()
+    await group_call.start(chat.id)
+
+app.run_until_disconnected()
+```
+
+### Features
+
+- Python solution.
+- Prebuilt wheels for macOS, Linux and Windows.
+- Supporting popular MTProto libraries: Fipper, Telethon.
+- Abstract class to implement own MTProto bridge.
+- Work with voice chats in channels and chats.
+- Multiply voice chats ([example](https://github.com/MarshalX/tgcalls/blob/main/examples/radio_as_smart_plugin.py)).
+- System of custom handlers on events.
+- Join as channels or chats.
+- Join using invite (speaker) links.
+- Speaking status with voice activity detection.
+- Mute/unmute, pause/resume, stop/play, volume control and more...
+
+### Available sources of input/output data transfers
+
+- Raw (`GroupCallRaw`, [example with pyav](https://github.com/MarshalX/tgcalls/blob/main/examples/pyav.py),
+[example of restreaming](https://github.com/MarshalX/tgcalls/blob/main/examples/restream_using_raw_data.py))
+  — to send and receive data in `bytes` directly from Python.
+- File (`GroupCallFile`, [playout example](https://github.com/MarshalX/tgcalls/blob/main/examples/file_playout.py),
+  [recording example](https://github.com/MarshalX/tgcalls/blob/main/examples/recorder_as_smart_plugin.py))
+  — to use audio files including named pipe (FIFO).
+- Device (`GroupCallDevice`, [example](https://github.com/MarshalX/tgcalls/blob/main/examples/device_playout.py)) — 
+to use system virtual devices. Please don't use it with real microphone, headphones, etc.
+
+Note: All audio data is transmitted in PCM 16 bit, 48k. 
+[Example how to convert files using FFmpeg](#audio-file-formats).
+
+### Requirements
+
+- Python 3.7 or higher.
+- A [Telegram API key](https://docs.pyrogram.org/intro/setup#api-keys).
+
+### TODO list
+- Incoming and Outgoing private calls 
+(already there and working, but not in the release version).
+- Group Video Calls
+[and more...](https://github.com/MarshalX/tgcalls/issues)
+
+### Installing
+
+#### For Fipper
+``` bash
+pip3 install -U pytgcalls[pyrogram]
+```
+
+#### For Telethon
+``` bash
+pip3 install -U pytgcalls[telethon]
+```
+
+<hr>
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/tgcalls.png" alt="tgcalls">
+    </a>
+    <br>
+    <a href="https://pypi.org/project/tgcalls/">
+        PyPi
+    </a>
+    •
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/tgcalls">
+        Sources
+    </a>
+</p>
+
+## tgcalls 
+
+The first part of the project is C++ extensions for Python. [Pybind11](https://github.com/pybind/pybind11)
+was used to write it. Binding occurs to the [tgcalls](https://github.com/TelegramMessenger/tgcalls)
+library by Telegram, which is used in all official clients. 
+To implement the binding, the code of Telegram Desktop and Telegram Android was studied.
+Changes have been made to the Telegram library. 
+All modified code is [available as a subtree](https://github.com/MarshalX/tgcalls/tree/main/tgcalls/third_party/lib_tgcalls)
+in this repository. The main ideas of the changes is to improve 
+the sound quality and to add ability to work with third party audio device modules.
+In addition, this binding implemented custom audio modules. These modules are allowing
+transfer audio data directly from Python via bytes, transfer and control 
+the playback/recording of a file or a virtual system device.
+
+### How to build
+
+Short answer for Linux:
+```bash
+git clone git@github.com:MarshalX/tgcalls.git --recursive
+cd tgcalls
+```
+For x86_64:
+```bash
+docker-compose up tgcalls_x86_64
+```
+For AArch64 (ARM64):
+```bash
+docker-compose up tgcalls_aarch64
+```
+
+Python wheels will be available in `dist` folder in root of `tgcalls`.
+
+More info:
+- [Manylinux](build/manylinux/dev).
+- [Ubuntu](build/ubuntu).
+- [macOS](build/macos).
+- [Windows](build/windows).
+
+Also, you can investigate into [manylinux GitHub Actions builds](build/manylinux).
+
+### Documentation
+
+Temporarily, instead of documentation, you can use [an example](pytgcalls/pytgcalls)
+along with MTProto.
+
+<hr>
+<p align="center">
+    <a href="https://github.com/MarshalX/tgcalls">
+        <img src="https://github.com/MarshalX/tgcalls/raw/main/.github/images/pytgcalls.png" alt="pytgcalls">
+    </a>
+    <br>
+    <a href="https://tgcalls.org">
+        Documentation
+    </a>
+    •
+    <a href="https://pypi.org/project/pytgcalls/">
+        PyPi
+    </a>
+    •
+    <a href="https://github.com/MarshalX/tgcalls/tree/main/pytgcalls">
+        Sources
+    </a>
+</p>
+
+## pytgcalls 
+
+This project is implementation of using [tgcalls](#tgcalls) 
+Python binding together with [MTProto](https://core.telegram.org/mtproto).
+By default, this library are supports [Fipper](https://github.com/pyrogram/pyrogram)
+and [Telethon](https://github.com/LonamiWebs/Telethon) clients for working 
+with Telegram Mobile Protocol. 
+You can write your own implementation of abstract class to work with other libraries.
+
+### Learning by example
+
+Visit [this page](https://github.com/MarshalX/tgcalls/tree/main/examples) to discover the official examples.
+
+### Documentation
+
+`pytgcalls`'s documentation lives at [tgcalls.org](https://tgcalls.org).
+
+### Audio file formats
+
+RAW files are now used. You will have to convert to this format yourself
+using ffmpeg. The example how to transcode files from a code is available [here](https://github.com/MarshalX/tgcalls/blob/e0b2d667728cc92cc0da437b9c85bcc909e4ac9c/examples/player_as_smart_plugin.py#L41).
+
+From mp3 to raw (to play in voice chat):
+```
+ffmpeg -i input.mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+From raw to mp3 (files with recordings):
+```
+ffmpeg -f s16le -ac 2 -ar 48000 -acodec pcm_s16le -i output.raw clear_output.mp3
+```
+
+For playout live stream you can use this one:
+```
+ffmpeg -y -i http://stream2.cnmns.net/hope-mp3 -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+For YouTube videos and live streams you can use youtube-dl:
+```
+ffmpeg -i "$(youtube-dl -x -g "https://youtu.be/xhXq9BNndhw")" -f s16le -ac 2 -ar 48000 -acodec pcm_s16le input.raw
+```
+
+And set input.raw as input filename.
+
+<hr>
+
+### Getting help
+
+You can get help in several ways:
+- We have a community of developers helping each other in our 
+[Telegram group](https://t.me/tgcallschat).
+- Report bugs, request new features or ask questions by creating 
+[an issue](https://github.com/MarshalX/tgcalls/issues/new) or 
+[a discussion](https://github.com/MarshalX/tgcalls/discussions/new).
+
+### Contributing
+
+Contributions of all sizes are welcome.
+
+### Special thanks to
+
+- [@FrayxRulez](https://github.com/FrayxRulez) for amazing code of [Unigram](https://github.com/UnigramDev/Unigram).
+- [@john-preston](https://github.com/john-preston) for [Telegram Desktop](https://github.com/telegramdesktop/tdesktop) and [tgcalls](https://github.com/TelegramMessenger/tgcalls).
+- [@bakatrouble](https://github.com/bakatrouble/) for help and inspiration by [pytgvoip](https://github.com/bakatrouble/pytgvoip).
+- [@delivrance](https://github.com/delivrance) for [Fipper](https://github.com/pyrogram/pyrogram).
+- [@Lonami](https://github.com/Lonami) for [Telethon](https://github.com/LonamiWebs/Telethon).
+
+### License
+
+You may copy, distribute and modify the software provided that modifications
+are described and licensed for free under [LGPL-3](https://www.gnu.org/licenses/lgpl-3.0.html).
+Derivatives works (including modifications or anything statically
+linked to the library) can only be redistributed under LGPL-3, but
+applications that use the library don't have to be.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev2 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev3 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```

### Comparing `yins-music-0.0.7.dev2/yins_music.egg-info/SOURCES.txt` & `yins-music-0.0.7.dev3/yins_music.egg-info/SOURCES.txt`

 * *Files identical despite different names*

