# Comparing `tmp/nxsrecselector-3.26.3.tar.gz` & `tmp/nxsrecselector-3.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nxsrecselector-3.26.3.tar", last modified: Fri Mar 10 08:35:35 2023, max compression
+gzip compressed data, was "nxsrecselector-3.27.0.tar", last modified: Fri May 26 09:17:26 2023, max compression
```

## Comparing `nxsrecselector-3.26.3.tar` & `nxsrecselector-3.27.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.26.3/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.26.3/MANIFEST.in
--rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2017-06-19 15:02:38.000000 nxsrecselector-3.26.3/NXSRecSelector
--rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     4306 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.26.3/man/NXSRecSelector.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.26.3/man/nxsrecconfig.1
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/nxsrecconfig/
--rw-r--r--   0 jkotan   (15949) irc         (39)     6486 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/CheckerThread.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.26.3/nxsrecconfig/Converter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/Describer.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/DynamicComponent.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    19515 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/MacroServerPools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    74598 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/NXSConfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    57988 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/ProfileManager.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-03-09 16:17:52.000000 nxsrecselector-3.26.3/nxsrecconfig/Release.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.26.3/nxsrecconfig/Selection.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/Selector.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    43062 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/Settings.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.26.3/nxsrecconfig/StreamSet.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    28195 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/Utils.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.26.3/nxsrecconfig/__init__.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/nxsrecselector.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/nxsrecselector.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/nxsrecselector.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/nxsrecselector.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.26.3/nxsrecselector.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/nxsrecselector.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/nxsrecselector.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-03-10 08:35:35.000000 nxsrecselector-3.26.3/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.26.3/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2018-10-10 09:18:56.000000 nxsrecselector-3.27.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)       93 2016-05-11 08:07:11.000000 nxsrecselector-3.27.0/MANIFEST.in
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      941 2017-06-19 15:02:38.000000 nxsrecselector-3.27.0/NXSRecSelector
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4306 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.664372 nxsrecselector-3.27.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      938 2017-03-18 22:59:30.000000 nxsrecselector-3.27.0/man/NXSRecSelector.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   109341 2023-03-10 08:35:11.000000 nxsrecselector-3.27.0/man/nxsrecconfig.1
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/nxsrecconfig/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6486 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/CheckerThread.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10979 2020-01-31 13:48:24.000000 nxsrecselector-3.27.0/nxsrecconfig/Converter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23789 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/Describer.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22847 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/DynamicComponent.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19515 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/MacroServerPools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    74862 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/NXSConfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59225 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/ProfileManager.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      930 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/Release.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     9075 2020-01-31 13:48:24.000000 nxsrecselector-3.27.0/nxsrecconfig/Selection.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    16157 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/Selector.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    43477 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/Settings.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5795 2023-03-09 16:17:52.000000 nxsrecselector-3.27.0/nxsrecconfig/StreamSet.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    29259 2023-05-26 09:16:32.000000 nxsrecselector-3.27.0/nxsrecconfig/Utils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1683 2023-02-01 13:37:17.000000 nxsrecselector-3.27.0/nxsrecconfig/__init__.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/nxsrecselector.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7061 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)      710 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-12-01 13:43:40.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       17 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)       13 2023-05-26 09:17:26.000000 nxsrecselector-3.27.0/nxsrecselector.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      213 2023-05-26 09:17:26.668372 nxsrecselector-3.27.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3985 2022-05-18 15:32:00.000000 nxsrecselector-3.27.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nxsrecselector-3.26.3/COPYRIGHT` & `nxsrecselector-3.27.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/NXSRecSelector` & `nxsrecselector-3.27.0/NXSRecSelector`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/PKG-INFO` & `nxsrecselector-3.27.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.26.3
+Version: 3.27.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
```

### Comparing `nxsrecselector-3.26.3/README.rst` & `nxsrecselector-3.27.0/README.rst`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/man/NXSRecSelector.1` & `nxsrecselector-3.27.0/man/NXSRecSelector.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/man/nxsrecconfig.1` & `nxsrecselector-3.27.0/man/nxsrecconfig.1`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/CheckerThread.py` & `nxsrecselector-3.27.0/nxsrecconfig/CheckerThread.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/Converter.py` & `nxsrecselector-3.27.0/nxsrecconfig/Converter.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/Describer.py` & `nxsrecselector-3.27.0/nxsrecconfig/Describer.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/DynamicComponent.py` & `nxsrecselector-3.27.0/nxsrecconfig/DynamicComponent.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/MacroServerPools.py` & `nxsrecselector-3.27.0/nxsrecconfig/MacroServerPools.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/NXSConfig.py` & `nxsrecselector-3.27.0/nxsrecconfig/NXSConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,18 @@
             self.__stg = None
         self.get_device_properties(self.get_device_class())
         numberofthreads = self.NumberOfThreads or None
         defaultpath = self.DefaultNeXusPath or None
         defaultzone = self.DefaultTimeZone or None
         defaultmntgrp = self.DefaultMntGrp or None
         syncsnapshot = bool(self.SyncSnapshot)
+        writepoolmotorpositions = bool(self.WritePoolMotorPositions)
         self.__stg = STG(self, numberofthreads, defaultpath,
-                         defaultzone, defaultmntgrp, syncsnapshot)
+                         defaultzone, defaultmntgrp, syncsnapshot,
+                         writepoolmotorpositions)
         self.set_state(tango.DevState.ON)
         self.__stg.poolBlacklist = self.PoolBlacklist or []
         self.__stg.timerFilters = self.TimerFilters or [
             "*dgg*", "*/timer/*", "*/ctctrl0*"]
         self.__stg.masterTimerFirst = bool(self.MasterTimerFirst)
         self.__stg.mutedChannelFilters = self.MutedChannelFilters \
             or ["*tip551*"]
@@ -1871,14 +1873,18 @@
         [tango.DevVarStringArray,
          "list of record keys for CLIENT datasources",
          []],
         'SyncSnapshot':
         [tango.DevBoolean,
          "preselection merges the current ScanSnapshot",
          [False]],
+        'WritePoolMotorPositions':
+        [tango.DevBoolean,
+         "add dynamic components for all pool motor positions",
+         [False]],
         'MasterTimerFirst':
         [tango.DevBoolean,
          "the master timer channel of MG with the index: 0",
          [False]],
         'DefaultCanFailDataSources':
         [tango.DevVarStringArray,
          "list of default datasources in the CanFail mode",
```

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/ProfileManager.py` & `nxsrecselector-3.27.0/nxsrecconfig/ProfileManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,25 @@
                        'filename']
 
 
 class ProfileManager(object):
 
     """  Manages Measurement Group and Profile from Selector"""
 
-    def __init__(self, selector, syncsnapshot=False):
+    def __init__(self, selector, syncsnapshot=False,
+                 writepoolmotorpositions=False):
         """ constructor
 
         :param selector: selector object
         :type selector: :class:`nxsrecconfig.Selector.Selector`
         :param syncsnapshot: preselection merges current ScanSnapshot
         :type syncsnapshot: :obj:`bool`
+        :param writepoolmotorpositions: add dynamic components
+                                        for all pool motor positions
+        :type writepoolmotorpositions: :obj:`bool`
         """
         #: (:class:`nxsrecconfig.Selector.Selector`) configuration selector
         self.__selector = selector
 
         #: (:obj:`str`) macro server name
         self.__macroServerName = None
         #: (:class:`tango.DeviceProxy` \
@@ -87,14 +91,17 @@
         self.masterTimerFirst = False
         #: (:obj:`bool`) mntgrp with synchronization
         self.__withsynch = True
 
         #: (:obj:`bool`) preselection merges current ScanSnapshot
         self.__syncsnapshot = syncsnapshot
 
+        #: (:obj:`bool`) add dynamic components for all pool motor positions
+        self.__writepoolmotorpositions = writepoolmotorpositions
+
     def __updateMacroServer(self):
         """ updatas MacroServer name
         """
         self.__macroServerName = self.__selector.getMacroServer()
         self.__withsynch = self.__hassynch()
 
     def __updateConfigServer(self):
@@ -138,14 +145,30 @@
             if mntgrps:
                 ind = mntgrps.index(amntgrp)
                 mntgrps[0], mntgrps[ind] = mntgrps[ind], mntgrps[0]
         except ValueError:
             pass
         return mntgrps
 
+    def getPoolMotors(self):
+        """ available mntgrps
+
+        :returns: list of available measurement groups
+        :rtype: :obj:`list` <:obj:`str`>
+        """
+        self.__updateMacroServer()
+        self.__updatePools()
+        motors = None
+        amntgrp = MSUtils.getEnv('ActiveMntGrp', self.__macroServerName)
+        fpool = self.__getActivePool(amntgrp)
+        if fpool:
+            motors = PoolUtils.getMotorPositionAttributes([fpool])
+        motors = motors if motors else []
+        return motors
+
     def components(self):
         """ provides selected components
 
         :returns: list of available selected components
         :rtype: :obj:`list` <:obj:`str`>
         """
         cps = json.loads(self.__selector["ComponentSelection"])
@@ -418,18 +441,27 @@
         """ add preselected components to set of given components
 
         :param components: new selection preselected components
         :type components: :obj:`list` <:obj:`str`>
         """
         if not self.__macroServerName:
             self.__updateMacroServer()
-        snapshot = MSUtils.getEnv(
-            'PreScanSnapshot', self.__macroServerName)
-        tangods = [[ds[1], ds[1], ds[0]] for ds in snapshot]
-        snpds = dict([(ds[1], False) for ds in snapshot])
+        snapshot = []
+        tangods = []
+        snpds = {}
+        if self.__syncsnapshot:
+            snapshot = MSUtils.getEnv(
+                'PreScanSnapshot', self.__macroServerName)
+            tangods = [[ds[1], ds[1], ds[0]] for ds in snapshot]
+        poolds = []
+        if self.__writepoolmotorpositions:
+            poolds = self.getPoolMotors()
+            if poolds:
+                tangods.extend(poolds)
+        snpds = dict([(ds[0], False) for ds in tangods])
         mydsg = {}
         self.createDataSources(tangods, mydsg)
         jpcps = json.loads(self.__selector["ComponentPreselection"])
         jpdss = json.loads(self.__selector["DataSourcePreselection"])
         predss = set(json.loads(self.__selector["PreselectingDataSources"]))
         changed = False
         for cp in components:
@@ -478,21 +510,21 @@
         """
         self.__updateConfigServer()
         if self.__selector.fetchSelection() is False:
             avmg = self.availableMntGrps()
             if self.__selector["MntGrp"] in avmg:
                 self.__selector.deselect()
                 self.importMntGrp()
-                if self.__syncsnapshot:
+                if self.__syncsnapshot or self.__writepoolmotorpositions:
                     self.__addPreselectedComponents(
                         self.defaultPreselectedComponents)
                 self.__selector.resetPreselectedComponents(
                     self.defaultPreselectedComponents)
                 self.__selector.preselect()
-        elif self.__syncsnapshot:
+        elif self.__syncsnapshot or self.__writepoolmotorpositions:
             changed = self.__addPreselectedComponents(
                 self.defaultPreselectedComponents)
             if changed:
                 self.__selector.preselect()
 
     def __createMntGrpConf(self, datasources,
                            componentdatasources, description):
```

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/Release.py` & `nxsrecselector-3.27.0/nxsrecconfig/Release.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  NeXus Sardana Recorder Settings - Release """
 
 #: (:obj:`str`) package version
-__version__ = "3.26.3"
+__version__ = "3.27.0"
```

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/Selection.py` & `nxsrecselector-3.27.0/nxsrecconfig/Selection.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/Selector.py` & `nxsrecselector-3.27.0/nxsrecconfig/Selector.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/Settings.py` & `nxsrecselector-3.27.0/nxsrecconfig/Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,28 @@
 
     """ NeXus Sardana Recorder settings
     """
 
     def __init__(self, server=None, numberofthreads=None,
                  defaultnexuspath=None,
                  defaulttimezone=None, defaultmntgrp=None,
-                 syncsnapshot=False):
+                 syncsnapshot=False, writepoolmotorpositions=False):
         """ contructor
 
         :param server: NXSRecSelector server
         :type server: :class:`nxsrecconfig.NXSConfig.NXSRecSelector`
         :param numberofthreads: number of threads used to check device state
         :type numberofthreads: :obj:`str`
         :param defaultnexuspath:  default dynamic component path
         :type defaultnexuspath: :obj:`str`
         :param syncsnapshot: preselection merges current ScanSnapshot
         :type syncsnapshot: :obj:`bool`
+        :param writepoolmotorpositions: add dynamic components
+                                        for all pool motor positions
+        :type writepoolmotorpositions: :obj:`bool`
         """
         #: (:class:`nxsrecconfig.NXSConfig.NXSRecSelector`) Tango server
         self.__server = server
         #: (:obj:`int`) number of threads
         self.numberOfThreads = numberofthreads or 20
 
         #: (:class:`StreamSet` or :class:`tango.Device_4Impl`) stream set
@@ -86,14 +89,16 @@
         self.defaultTimeZone = defaulttimezone or "Europe/Berlin"
 
         #: (:obj:`str`) default measurement group
         self.defaultMntGrp = defaultmntgrp or "nxsmntgrp"
 
         #: (:obj:`bool`) preselection merges current ScanSnapshot
         self.syncSnapshot = syncsnapshot
+        #: (:obj:`bool`) add dynamic components for all pool motor positions
+        self.writepoolmotorpositions = writepoolmotorpositions
         if PYTG_BUG_213:
             self._streams.error(
                 "Settings::Settings() - "
                 "Reading/Writinh Encoded Attributes for python3 and "
                 "tango < 9.2.5"
                 " is not supported ")
 
@@ -107,15 +112,16 @@
             self.__msp, self.version, self.defaultNeXusPath,
             self.defaultTimeZone, self.defaultMntGrp)
 
         #: (:class:`nxsrecconfg.ProfileManager.ProfileManager) \
         #: profile
         self.__profileManager = ProfileManager(
             self.__selector,
-            syncsnapshot=syncsnapshot
+            syncsnapshot=syncsnapshot,
+            writepoolmotorpositions=writepoolmotorpositions
         )
 
         #: (:obj:`str`) configuration file
         self.profileFile = '/tmp/nxsrecconfig.cfg'
 
         #: (:class:`tango.Database`) tango database
         self.__db = tango.Database()
```

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/StreamSet.py` & `nxsrecselector-3.27.0/nxsrecconfig/StreamSet.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/Utils.py` & `nxsrecselector-3.27.0/nxsrecconfig/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -756,14 +756,43 @@
             chan = json.loads(elm)
             if alias == chan['name']:
                 argout = chan['full_name']
                 break
         return argout
 
     @classmethod
+    def getMotorPositionAttributes(cls, pools):
+        """ find motor names
+
+        :param pools: list of pool devices
+        :type pools: :obj:`list` <:class:`tango.DeviceProxy`>
+        :returns: full name of the measurement group alias
+        :rtype: :obj:`str`
+        :returns: (name , name , motor position attribute)
+        :rtype: :obj:`list` <:obj:`str`,:obj:`str`, :obj:`str`>
+        """
+        lst = []
+        for pool in pools:
+            if pool.MotorList:
+                lst += pool.MotorList
+        argout = []
+        for elm in lst:
+            chan = json.loads(elm)
+            if "name" in elm and "full_name" in elm:
+                name = chan['name']
+                fname = chan['full_name']
+                if name and fname:
+                    if fname.startswith("tango://"):
+                        fname = fname[8:]
+                    if not fname.lower().endswith("/position"):
+                        fname = fname + "/position"
+                argout.append([name, name, fname])
+        return argout
+
+    @classmethod
     def getTimers(cls, pools, filters=None):
         """ provides tiemrs of given pools
 
         :param pools: list of pool devices
         :type pools: :obj:`list` <:class:`tango.DeviceProxy`>
         :param filters: device name filter list
         :type filters: :obj:`list` <:obj:`str`>
```

### Comparing `nxsrecselector-3.26.3/nxsrecconfig/__init__.py` & `nxsrecselector-3.27.0/nxsrecconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/nxsrecselector.egg-info/PKG-INFO` & `nxsrecselector-3.27.0/nxsrecselector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: nxsrecselector
-Version: 3.26.3
+Version: 3.27.0
 Summary: Selector Server for NeXus Sardana recorder
 Home-page: https://github.com/jkotan/nexdatas/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: ========================================
         Welcome to nxsrecconfig's documentation!
```

### Comparing `nxsrecselector-3.26.3/nxsrecselector.egg-info/SOURCES.txt` & `nxsrecselector-3.27.0/nxsrecselector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nxsrecselector-3.26.3/setup.py` & `nxsrecselector-3.27.0/setup.py`

 * *Files identical despite different names*

