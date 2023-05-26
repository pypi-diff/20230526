# Comparing `tmp/ttkode-0.0.0a14.tar.gz` & `tmp/ttkode-0.0.0a17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttkode-0.0.0a14.tar", last modified: Fri Feb 10 12:08:41 2023, max compression
+gzip compressed data, was "ttkode-0.0.0a17.tar", last modified: Fri May 26 18:33:18 2023, max compression
```

## Comparing `ttkode-0.0.0a14.tar` & `ttkode-0.0.0a17.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-02-10 12:08:41.145755 ttkode-0.0.0a14/
--rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-02-10 12:08:41.145755 ttkode-0.0.0a14/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1673 2023-02-10 12:08:37.000000 ttkode-0.0.0a14/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2023-02-10 12:08:41.145755 ttkode-0.0.0a14/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1285 2023-02-10 12:08:37.000000 ttkode-0.0.0a14/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-02-10 12:08:41.145755 ttkode-0.0.0a14/ttkode/
--rwxrwxr-x   0 one       (1000) one       (1000)     1239 2022-09-28 07:52:57.000000 ttkode-0.0.0a14/ttkode/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1242 2022-09-28 07:52:57.000000 ttkode-0.0.0a14/ttkode/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-02-10 12:08:41.145755 ttkode-0.0.0a14/ttkode/app/
--rw-rw-r--   0 one       (1000) one       (1000)     1319 2022-10-02 12:24:14.000000 ttkode-0.0.0a14/ttkode/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     2831 2022-10-22 20:15:24.000000 ttkode-0.0.0a14/ttkode/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     2135 2023-02-10 12:08:37.000000 ttkode-0.0.0a14/ttkode/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)     6442 2022-11-16 08:57:30.000000 ttkode-0.0.0a14/ttkode/app/kodeformatter.py
--rw-rw-r--   0 one       (1000) one       (1000)     7983 2023-02-10 12:05:59.000000 ttkode-0.0.0a14/ttkode/app/kodetab.py
--rw-rw-r--   0 one       (1000) one       (1000)     6196 2022-11-15 23:03:40.000000 ttkode-0.0.0a14/ttkode/app/kodetextdocument.py
--rw-rw-r--   0 one       (1000) one       (1000)     1440 2022-10-07 16:42:58.000000 ttkode-0.0.0a14/ttkode/app/kodetextedit.py
--rw-rw-r--   0 one       (1000) one       (1000)     4958 2023-01-10 17:23:58.000000 ttkode-0.0.0a14/ttkode/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)     3182 2022-09-28 07:52:57.000000 ttkode-0.0.0a14/ttkode/app/options.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-02-10 12:08:41.145755 ttkode-0.0.0a14/ttkode.egg-info/
--rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-02-10 12:08:41.000000 ttkode-0.0.0a14/ttkode.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)      448 2023-02-10 12:08:41.000000 ttkode-0.0.0a14/ttkode.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2023-02-10 12:08:41.000000 ttkode-0.0.0a14/ttkode.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       39 2023-02-10 12:08:41.000000 ttkode-0.0.0a14/ttkode.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       43 2023-02-10 12:08:41.000000 ttkode-0.0.0a14/ttkode.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)        7 2023-02-10 12:08:41.000000 ttkode-0.0.0a14/ttkode.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/
+-rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1673 2023-05-26 18:33:14.000000 ttkode-0.0.0a17/README.md
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     1286 2023-05-26 18:33:14.000000 ttkode-0.0.0a17/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/ttkode/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1239 2022-09-28 07:52:57.000000 ttkode-0.0.0a17/ttkode/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1242 2022-09-28 07:52:57.000000 ttkode-0.0.0a17/ttkode/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/ttkode/app/
+-rw-rw-r--   0 one       (1000) one       (1000)     1290 2023-05-26 17:28:55.000000 ttkode-0.0.0a17/ttkode/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2817 2023-05-26 17:26:14.000000 ttkode-0.0.0a17/ttkode/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2135 2023-05-26 18:33:14.000000 ttkode-0.0.0a17/ttkode/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6442 2022-11-16 08:57:30.000000 ttkode-0.0.0a17/ttkode/app/kodeformatter.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6196 2022-11-15 23:03:40.000000 ttkode-0.0.0a17/ttkode/app/kodetextdocument.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1440 2022-10-07 16:42:58.000000 ttkode-0.0.0a17/ttkode/app/kodetextedit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6157 2023-05-26 18:24:45.000000 ttkode-0.0.0a17/ttkode/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3182 2022-09-28 07:52:57.000000 ttkode-0.0.0a17/ttkode/app/options.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-26 18:33:18.752757 ttkode-0.0.0a17/ttkode.egg-info/
+-rw-rw-r--   0 one       (1000) one       (1000)     2389 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)      426 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       39 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       44 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        7 2023-05-26 18:33:18.000000 ttkode-0.0.0a17/ttkode.egg-info/top_level.txt
```

### Comparing `ttkode-0.0.0a14/PKG-INFO` & `ttkode-0.0.0a17/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttkode
-Version: 0.0.0a14
+Version: 0.0.0a17
 Summary: Terminal ToolKit Studio Code editor
 Home-page: https://github.com/ceccopierangiolieugenio/ttkode
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ttkode-0.0.0a14/README.md` & `ttkode-0.0.0a17/README.md`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a14/setup.py` & `ttkode-0.0.0a17/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.0.0a14"
+version = "0.0.0a17"
 name = "ttkode"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
@@ -28,15 +28,15 @@
         "Intended Audience :: Information Technology",
         "Topic :: Terminals",
         "Topic :: Software Development :: User Interfaces"],
     include_package_data=False,
     packages=['ttkode','ttkode.app'],
     python_requires=">=3.8",
     install_requires=[
-        'pyTermTk>=0.9.0a43',
+        'pyTermTk>=0.30.0a79',
         'appdirs',
         'pyyaml',
         'pygments'],
     entry_points={
         'console_scripts': [
             'ttkode = ttkode:main',
         ],
```

### Comparing `ttkode-0.0.0a14/ttkode/__init__.py` & `ttkode-0.0.0a17/ttkode/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a14/ttkode/__main__.py` & `ttkode-0.0.0a17/ttkode/__main__.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a14/ttkode/app/__init__.py` & `ttkode-0.0.0a17/ttkode/app/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from .cfg import *
 # from .glbl import *
 from .main import *
-from .kodetab import KodeTab
 from .kodetextdocument import KodeTextDocument
```

### Comparing `ttkode-0.0.0a14/ttkode/app/about.py` & `ttkode-0.0.0a17/ttkode/app/about.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     __slots__=('_image')
     def __init__(self, *args, **kwargs):
         TTkAbout.__init__(self, *args, **kwargs)
         self._name = kwargs.get('name' , 'About' )
         self.setTitle('[PierCecco Cecco] Eugenio Parodi proudly presents...')
         self.resize(56,16)
 
-    def paintEvent(self):
+    def paintEvent(self, canvas):
         c = [0xFF,0xFF,0xFF]
         for y, line in enumerate(About.ttkode):
-            self._canvas.drawText(pos=(13,3+y),text=line, color=TTkColor.fg(f'#{c[0]:02X}{c[1]:02X}{c[2]:02X}'))
+            canvas.drawText(pos=(13,3+y),text=line, color=TTkColor.fg(f'#{c[0]:02X}{c[1]:02X}{c[2]:02X}'))
             c[2]-=0x18
             c[0]-=0x08
-        self._canvas.drawText(pos=(26, 9),text=f"  Version: {TTKodeCfg.version}", color=TTkColor.fg('#AAAAFF'))
-        self._canvas.drawText(pos=(14,11),text=f"Powered By, pyTermTk")
-        self._canvas.drawText(pos=( 2,13),text=f"https://github.com/ceccopierangiolieugenio/ttkode", color=TTkColor.fg('#44FFFF'))
-        self._canvas.drawText(pos=( 2,14),text=f"https://github.com/ceccopierangiolieugenio/pyTermTk", color=TTkColor.fg('#44FFFF'))
+        canvas.drawText(pos=(26, 9),text=f"  Version: {TTKodeCfg.version}", color=TTkColor.fg('#AAAAFF'))
+        canvas.drawText(pos=(14,11),text=f"Powered By, pyTermTk")
+        canvas.drawText(pos=( 2,13),text=f"https://github.com/ceccopierangiolieugenio/ttkode", color=TTkColor.fg('#44FFFF'))
+        canvas.drawText(pos=( 2,14),text=f"https://github.com/ceccopierangiolieugenio/pyTermTk", color=TTkColor.fg('#44FFFF'))
 
-        TTkWindow.paintEvent(self)
+        TTkWindow.paintEvent(self, canvas)
```

### Comparing `ttkode-0.0.0a14/ttkode/app/cfg.py` & `ttkode-0.0.0a17/ttkode/app/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import yaml
 
 class TTKodeCfg:
-    version="0.0.0a14"
+    version="0.0.0a17"
     name="ttkode"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
 
     @staticmethod
```

### Comparing `ttkode-0.0.0a14/ttkode/app/kodeformatter.py` & `ttkode-0.0.0a17/ttkode/app/kodeformatter.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a14/ttkode/app/kodetextdocument.py` & `ttkode-0.0.0a17/ttkode/app/kodetextdocument.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a14/ttkode/app/kodetextedit.py` & `ttkode-0.0.0a17/ttkode/app/kodetextedit.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a14/ttkode/app/main.py` & `ttkode-0.0.0a17/ttkode/app/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -35,26 +35,99 @@
 
 from TermTk import TTk, TTkK, TTkLog, TTkCfg, TTkColor, TTkTheme, TTkTerm, TTkHelper
 from TermTk import TTkString
 from TermTk import TTkColorGradient
 from TermTk import pyTTkSlot, pyTTkSignal
 
 from TermTk import TTkFrame, TTkButton
-from TermTk import TTkTabWidget
+from TermTk import TTkTabWidget, TTkKodeTab
 from TermTk import TTkAbstractScrollArea, TTkAbstractScrollView
 from TermTk import TTkFileDialogPicker
 from TermTk import TTkFileTree, TTkTextEdit
 
 from TermTk import TTkGridLayout
 from TermTk import TTkSplitter
 
 from .cfg  import *
 from .about import *
-from .kodetab import KodeTab
 # from .options import optionsFormLayout, optionsLoadTheme
+from .kodetextedit import KodeTextEditView
+from .kodetextdocument import KodeTextDocument
+
+class TTKode(TTkGridLayout):
+    __slots__ = ('_kodeTab', '_documents')
+    def __init__(self, *, files, **kwargs):
+        self._documents = {}
+
+        super().__init__(**kwargs)
+
+        self.addWidget(splitter := TTkSplitter())
+
+        layoutLeft = TTkGridLayout()
+        splitter.addItem(layoutLeft, 20)
+
+        hSplitter = TTkSplitter(parent=splitter,  orientation=TTkK.HORIZONTAL)
+
+        menuFrame = TTkFrame(border=False, maxHeight=1)
+
+        self._kodeTab = TTkKodeTab(parent=hSplitter, border=False, closable=True)
+
+        fileMenu = menuFrame.menubarTop().addMenu("&File")
+        fileMenu.addMenu("Open").menuButtonClicked.connect(self._showFileDialog)
+        fileMenu.addMenu("Close") # .menuButtonClicked.connect(self._closeFile)
+        fileMenu.addMenu("Exit").menuButtonClicked.connect(lambda _:TTkHelper.quit())
+
+        def _showAbout(btn):
+            TTkHelper.overlay(None, About(), 30,10)
+        def _showAboutTTk(btn):
+            TTkHelper.overlay(None, TTkAbout(), 30,10)
+
+        helpMenu = menuFrame.menubarTop().addMenu("&Help", alignment=TTkK.RIGHT_ALIGN)
+        helpMenu.addMenu("About ...").menuButtonClicked.connect(_showAbout)
+        helpMenu.addMenu("About ttk").menuButtonClicked.connect(_showAboutTTk)
+
+        fileTree = TTkFileTree(path='.')
+
+        layoutLeft.addWidget(menuFrame, 0,0)
+        layoutLeft.addWidget(fileTree, 1,0)
+        layoutLeft.addWidget(quitbtn := TTkButton(border=True, text="Quit", maxHeight=3), 2,0)
+
+        quitbtn.clicked.connect(TTkHelper.quit)
+
+        for file in files:
+            self._openFile(file)
+
+        fileTree.fileActivated.connect(lambda x: self._openFile(x.path()))
+
+    pyTTkSlot()
+    def _showFileDialog(self):
+        filePicker = TTkFileDialogPicker(pos = (3,3), size=(75,24), caption="Pick Something", path=".", fileMode=TTkK.FileMode.AnyFile ,filter="All Files (*);;Python Files (*.py);;Bash scripts (*.sh);;Markdown Files (*.md)")
+        filePicker.pathPicked.connect(self._openFile)
+        TTkHelper.overlay(None, filePicker, 20, 5, True)
+
+    def _openFile(self, filePath):
+        filePath = os.path.realpath(filePath)
+        if filePath in self._documents:
+            doc = self._documents[filePath]['doc']
+        else:
+            with open(filePath, 'r') as f:
+                content = f.read()
+            doc = KodeTextDocument(text=content, filePath=filePath)
+            self._documents[filePath] = {'doc':doc,'tabs':[]}
+        tview = KodeTextEditView(document=doc, readOnly=False)
+        tedit = TTkTextEdit(textEditView=tview, lineNumber=True)
+        doc.kodeHighlightUpdate.connect(tedit.update)
+        label = TTkString(TTkCfg.theme.fileIcon.getIcon(filePath),TTkCfg.theme.fileIconColor) + TTkColor.RST + " " + os.path.basename(filePath)
+
+        self._kodeTab.addTab(tedit, label)
+        self._kodeTab.setCurrentWidget(tedit)
+
+        # def _closeFile():
+        #     if (index := KodeTab.lastUsed.currentIndex()) >= 0:
+        #         KodeTab.lastUsed.removeTab(index)
 
 def main():
     TTKodeCfg.pathCfg = appdirs.user_config_dir("ttkode")
 
     parser = argparse.ArgumentParser()
     # parser.add_argument('-f', help='Full Screen', action='store_true')
     parser.add_argument('-c', help=f'config folder (default: "{TTKodeCfg.pathCfg}")', default=TTKodeCfg.pathCfg)
@@ -71,63 +144,15 @@
 
     # if 'theme' not in TTKodeCfg.options:
     #     TTKodeCfg.options['theme'] = 'NERD'
     # optionsLoadTheme(TTKodeCfg.options['theme'])
 
     TTkTheme.loadTheme(TTkTheme.NERD)
 
-    root = TTk( layout=TTkGridLayout(), title="TTkode",
+    root = TTk( layout=TTKode(files=args.filename), title="TTkode",
                 sigmask=(
                     # TTkTerm.Sigmask.CTRL_C |
                     TTkTerm.Sigmask.CTRL_Q |
                     TTkTerm.Sigmask.CTRL_S |
                     TTkTerm.Sigmask.CTRL_Z ))
 
-    splitter = TTkSplitter(parent=root)
-    layoutLeft = TTkGridLayout()
-    splitter.addItem(layoutLeft, 20)
-
-    hSplitter = TTkSplitter(parent=splitter,  orientation=TTkK.HORIZONTAL)
-
-    menuFrame = TTkFrame(border=False, maxHeight=1)
-
-    KodeTab(parent=hSplitter, border=False, closable=True)
-
-    def _openFile(file):
-        KodeTab.lastUsed.openFile(file)
-    def _closeFile(_):
-        if (index := KodeTab.lastUsed.currentIndex()) >= 0:
-            KodeTab.lastUsed.removeTab(index)
-
-    def _showFileDialog(fm):
-        filePicker = TTkFileDialogPicker(pos = (3,3), size=(75,24), caption="Pick Something", path=".", fileMode=TTkK.FileMode.AnyFile ,filter="All Files (*);;Python Files (*.py);;Bash scripts (*.sh);;Markdown Files (*.md)")
-        filePicker.pathPicked.connect(_openFile)
-        TTkHelper.overlay(None, filePicker, 20, 5, True)
-
-    fileMenu = menuFrame.menubarTop().addMenu("&File")
-    fileMenu.addMenu("Open").menuButtonClicked.connect(_showFileDialog)
-    fileMenu.addMenu("Close").menuButtonClicked.connect(_closeFile)
-    fileMenu.addMenu("Exit").menuButtonClicked.connect(lambda _:TTkHelper.quit())
-
-    def _showAbout(btn):
-        TTkHelper.overlay(None, About(), 30,10)
-    def _showAboutTTk(btn):
-        TTkHelper.overlay(None, TTkAbout(), 30,10)
-
-    helpMenu = menuFrame.menubarTop().addMenu("&Help", alignment=TTkK.RIGHT_ALIGN)
-    helpMenu.addMenu("About ...").menuButtonClicked.connect(_showAbout)
-    helpMenu.addMenu("About ttk").menuButtonClicked.connect(_showAboutTTk)
-
-    fileTree = TTkFileTree(path='.')
-
-    layoutLeft.addWidget(menuFrame, 0,0)
-    layoutLeft.addWidget(fileTree, 1,0)
-    layoutLeft.addWidget(quitbtn := TTkButton(border=True, text="Quit", maxHeight=3), 2,0)
-
-    quitbtn.clicked.connect(root.quit)
-
-    for file in args.filename:
-        _openFile(file)
-
-    fileTree.fileActivated.connect(lambda x: _openFile(x.path()))
-
     root.mainloop()
```

### Comparing `ttkode-0.0.0a14/ttkode/app/options.py` & `ttkode-0.0.0a17/ttkode/app/options.py`

 * *Files identical despite different names*

### Comparing `ttkode-0.0.0a14/ttkode.egg-info/PKG-INFO` & `ttkode-0.0.0a17/ttkode.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttkode
-Version: 0.0.0a14
+Version: 0.0.0a17
 Summary: Terminal ToolKit Studio Code editor
 Home-page: https://github.com/ceccopierangiolieugenio/ttkode
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

