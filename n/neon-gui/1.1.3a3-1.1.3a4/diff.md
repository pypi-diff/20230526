# Comparing `tmp/neon_gui-1.1.3a3-py3-none-any.whl.zip` & `tmp/neon_gui-1.1.3a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 9725 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1831 b- defN 23-May-17 21:13 neon_gui/__init__.py
--rw-r--r--  2.0 unx     2701 b- defN 23-May-17 21:13 neon_gui/__main__.py
--rw-r--r--  2.0 unx     3885 b- defN 23-May-17 21:13 neon_gui/service.py
--rw-r--r--  2.0 unx     5572 b- defN 23-May-17 21:13 neon_gui/utils.py
--rw-r--r--  2.0 unx     1635 b- defN 23-May-17 21:13 neon_gui-1.1.3a3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1344 b- defN 23-May-17 21:13 neon_gui-1.1.3a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 21:13 neon_gui-1.1.3a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-May-17 21:13 neon_gui-1.1.3a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-17 21:13 neon_gui-1.1.3a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      805 b- defN 23-May-17 21:13 neon_gui-1.1.3a3.dist-info/RECORD
-10 files, 17934 bytes uncompressed, 8351 bytes compressed:  53.4%
+Zip file size: 11233 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-26 21:34 neon_gui/__init__.py
+-rw-r--r--  2.0 unx     2575 b- defN 23-May-26 21:34 neon_gui/__main__.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-May-26 21:34 neon_gui/cli.py
+-rw-r--r--  2.0 unx     3853 b- defN 23-May-26 21:34 neon_gui/service.py
+-rw-r--r--  2.0 unx     5572 b- defN 23-May-26 21:34 neon_gui/utils.py
+-rw-r--r--  2.0 unx     1635 b- defN 23-May-26 21:34 neon_gui-1.1.3a4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1402 b- defN 23-May-26 21:34 neon_gui-1.1.3a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 21:34 neon_gui-1.1.3a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       97 b- defN 23-May-26 21:34 neon_gui-1.1.3a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-26 21:34 neon_gui-1.1.3a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      877 b- defN 23-May-26 21:34 neon_gui-1.1.3a4.dist-info/RECORD
+11 files, 20651 bytes uncompressed, 9753 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: neon_gui/__init__.py
 Comment: 
 
 Filename: neon_gui/__main__.py
 Comment: 
 
+Filename: neon_gui/cli.py
+Comment: 
+
 Filename: neon_gui/service.py
 Comment: 
 
 Filename: neon_gui/utils.py
 Comment: 
 
-Filename: neon_gui-1.1.3a3.dist-info/LICENSE.md
+Filename: neon_gui-1.1.3a4.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_gui-1.1.3a3.dist-info/METADATA
+Filename: neon_gui-1.1.3a4.dist-info/METADATA
 Comment: 
 
-Filename: neon_gui-1.1.3a3.dist-info/WHEEL
+Filename: neon_gui-1.1.3a4.dist-info/WHEEL
 Comment: 
 
-Filename: neon_gui-1.1.3a3.dist-info/entry_points.txt
+Filename: neon_gui-1.1.3a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_gui-1.1.3a3.dist-info/top_level.txt
+Filename: neon_gui-1.1.3a4.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_gui-1.1.3a3.dist-info/RECORD
+Filename: neon_gui-1.1.3a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_gui/__main__.py

```diff
@@ -25,27 +25,24 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ovos_utils import wait_for_exit_signal
 from ovos_utils.log import LOG
 from neon_gui.service import NeonGUIService
-from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
-from ovos_utils.process_utils import PIDLock as Lock
+from ovos_utils.process_utils import reset_sigint_handler, PIDLock
 
 
 def main(*args, **kwargs):
-    init_config_dir()
     init_log(log_name="gui")
     malloc_running = start_malloc(stack_depth=4)
-    from ovos_utils.process_utils import reset_sigint_handler
     reset_sigint_handler()
-    Lock("gui")
+    PIDLock("gui")
 
     gui = NeonGUIService(*args, **kwargs)
     gui.start()
     wait_for_exit_signal()
     if malloc_running:
         try:
             print_malloc(snapshot_malloc())
```

## neon_gui/service.py

```diff
@@ -45,39 +45,39 @@
         add_neon_about_data()
         LOG.info(f"Updated GUI About Data")
         ready_hook()
     return wrapper
 
 
 def on_stopping():
-    LOG.info('Messagebus service is shutting down...')
+    LOG.info('GUI service is shutting down...')
 
 
 def on_error(e='Unknown'):
-    LOG.error('Messagebus service failed to launch ({}).'.format(repr(e)))
+    LOG.error('GUI service failed to launch ({}).'.format(repr(e)))
 
 
 def on_alive():
-    LOG.debug("Messagebus client alive")
+    LOG.debug("GUI client alive")
 
 
 def on_started():
-    LOG.debug("Messagebus client started")
+    LOG.debug("GUI client started")
 
 
 class NeonGUIService(Thread, GUIService):
     def __init__(self, ready_hook=on_ready, error_hook=on_error,
                  stopping_hook=on_stopping, alive_hook=on_alive,
                  started_hook=on_started, gui_config=None, daemonic=False,):
         if gui_config:
             from neon_gui.utils import patch_config
             patch_config(gui_config)
         Thread.__init__(self)
-        self.setDaemon(daemonic)
-        self.setName('GUI')
+        self.daemon = daemonic
+        self.name = 'GUI'
         self.started = Event()
         ready_hook = wrapped_ready_hook(ready_hook)
         GUIService.__init__(self, alive_hook=alive_hook,
                             started_hook=started_hook, ready_hook=ready_hook,
                             error_hook=error_hook, stopping_hook=stopping_hook)
 
     def run(self):
```

## Comparing `neon_gui-1.1.3a3.dist-info/LICENSE.md` & `neon_gui-1.1.3a4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_gui-1.1.3a3.dist-info/METADATA` & `neon_gui-1.1.3a4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: neon-gui
-Version: 1.1.3a3
+Version: 1.1.3a4
 Summary: Neon GUI Module
 Home-page: https://github.com/NeonGeckoCom/neon_gui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: neon-utils[network] (~=1.1)
 Requires-Dist: ovos-utils (>=0.0.25,~=0.0)
 Requires-Dist: tornado (~=6.0)
 Requires-Dist: ovos-bus-client (~=0.0.3)
 Requires-Dist: ovos-gui (>=0.0.3a2,~=0.0.2)
 Requires-Dist: ovos-config (~=0.0.4)
+Requires-Dist: ovos-plugin-manager (>=0.0.23a22,~=0.0.22)
 Provides-Extra: docker
 
 # Neon GUI
 GUI Module for Neon Core. This module extracts the GUI components from the 
 [Mycroft Mark 2 Skill](https://github.com/MycroftAI/skill-mark-2) and the `enclosure` module
 from [mycroft-core](https://github.com/MycroftAI/mycroft-core/tree/dev/mycroft/enclosure).
```

