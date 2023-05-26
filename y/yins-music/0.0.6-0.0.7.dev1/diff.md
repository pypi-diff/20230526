# Comparing `tmp/yins-music-0.0.6.tar.gz` & `tmp/yins-music-0.0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yins-music-0.0.6.tar", last modified: Sat May 20 07:56:28 2023, max compression
+gzip compressed data, was "yins-music-0.0.7.dev1.tar", last modified: Fri May 26 01:48:30 2023, max compression
```

## Comparing `yins-music-0.0.6.tar` & `yins-music-0.0.7.dev1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 07:56:28.514541 yins-music-0.0.6/
--rw-rw-rw-   0        0        0     7815 2023-05-20 07:52:21.000000 yins-music-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       15 2023-05-20 07:52:21.000000 yins-music-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    12226 2023-05-20 07:56:28.513541 yins-music-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    10043 2023-05-20 07:52:21.000000 yins-music-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 07:56:28.515541 yins-music-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     8093 2023-05-20 07:52:21.000000 yins-music-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:56:28.510547 yins-music-0.0.6/yins_music.egg-info/
--rw-rw-rw-   0        0        0    12226 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 07:56:28.000000 yins-music-0.0.6/yins_music.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-26 01:48:16.000000 yins-music-0.0.7.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:48:30.144095 yins-music-0.0.7.dev1/yins_music.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:48:30.000000 yins-music-0.0.7.dev1/yins_music.egg-info/top_level.txt
```

### Comparing `yins-music-0.0.6/LICENSE` & `yins-music-0.0.7.dev1/LICENSE`

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

### Comparing `yins-music-0.0.6/PKG-INFO` & `yins-music-0.0.7.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,330 +1,330 @@
-Metadata-Version: 2.1
-Name: yins-music
-Version: 0.0.6
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
+Version: 0.0.7.dev1
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
-Metadata-Version: 2.1 Name: yins-music Version: 0.0.6 Summary: a library
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev1 Summary: a library
 connecting the tgcalls Python binding with MTProto Home-page: https://
 github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
 License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
 Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
 t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
 python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
 chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
```

### Comparing `yins-music-0.0.6/README.md` & `yins-music-0.0.7.dev1/yins_music.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,283 +1,330 @@
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
+Version: 0.0.7.dev1
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
@@ -1,7 +1,36 @@
+Metadata-Version: 2.1 Name: yins-music Version: 0.0.7.dev1 Summary: a library
+connecting the tgcalls Python binding with MTProto Home-page: https://
+github.com/MarshalX/tgcalls Author: AyiinXd Author-email: ayiinxd0307@gmail.com
+License: LGPLv3 Project-URL: Documentation, https://tgcalls.org/ Project-URL:
+Telegram Channel, https://t.me/tgcallslib Project-URL: Telegram Chat, https://
+t.me/tgcallschat Project-URL: Author, https://github.com/AyiinXd Keywords:
+python,library,telegram,async,asynchronous,webrtc,lib,voice-chat,voip,group-
+chat,video-call,calls,fipper,telethon,pytgcalls,tgcalls Classifier: Development
+Status :: 5 - Production/Stable Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU Lesser General Public License v3 (LGPLv3) Classifier: Operating System
+:: OS Independent Classifier: Operating System :: MacOS Classifier: Operating
+System :: Unix Classifier: Topic :: Internet Classifier: Topic :: Multimedia
+Classifier: Topic :: Multimedia :: Video Classifier: Topic :: Multimedia ::
+Video :: Capture Classifier: Topic :: Multimedia :: Sound/Audio Classifier:
+Topic :: Multimedia :: Sound/Audio :: Capture/Recording Classifier: Topic ::
+Communications Classifier: Topic :: Communications :: Internet Phone
+Classifier: Topic :: Communications :: Telephony Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: Implementation Classifier: Programming Language :: Python ::
+Implementation :: CPython Requires-Python: ~=3.7 Description-Content-Type:
+text/markdown Provides-Extra: fipper Provides-Extra: telethon License-File:
+LICENSE
                                   [tgcalls]
  Voice chats, private incoming and outgoing calls in Telegram for Developers
                 Examples â¢ Documentation â¢ Channel â¢ Chat
 ## Telegram WebRTC (VoIP) [![Mentioned in Awesome Telegram Calls](https://
 awesome.re/mentioned-badge-flat.svg)](https://github.com/tgcalls/awesome-
 tgcalls) This project consists of two main parts: [tgcalls](#tgcalls),
 [pytgcalls](#pytgcalls). The first is a C++ Python extension. The second uses
```

