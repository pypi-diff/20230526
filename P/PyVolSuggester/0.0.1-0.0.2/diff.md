# Comparing `tmp/pyvolsuggester-0.0.1.tar.gz` & `tmp/pyvolsuggester-0.0.2.tar.gz`

## Comparing `pyvolsuggester-0.0.1.tar` & `pyvolsuggester-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    15822 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.1/src/PyVolSuggester/Suggester.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.1/src/PyVolSuggester/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.1/License.txt
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.1/README.md
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.2/src/PyVolSuggester/Suggester.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.2/src/PyVolSuggester/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.2/License.txt
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.2/README.md
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 pyvolsuggester-0.0.2/PKG-INFO
```

### Comparing `pyvolsuggester-0.0.1/src/PyVolSuggester/Suggester.py` & `pyvolsuggester-0.0.2/src/PyVolSuggester/Suggester.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 def zero_crossing_rate():
     global file, wav_file, plot_path, new_dir
     print("\nGenerated Zero Crossing Rate Plot...")
     file_name = os.path.basename(wav_file)
 
     y, sr = librosa.load(wav_file)
     zcrs = librosa.feature.zero_crossing_rate(y)
-    print(f"Zero crossing rate: {sum(librosa.zero_crossings(y))}")
+    # print(f"Zero crossing rate: {sum(librosa.zero_crossings(y))}")
     plt.figure(figsize=(15, 3))
     plt.plot(zcrs[0])
     plt.title(file_name + ' - Zero Crossing Rate')
     # plt.legend()
 
     ## saving the plot
     print("Saved " + file_name + ' - Zero Crossing Rate.jpg')
@@ -406,28 +406,26 @@
 
     plt.show()
 
 
 ## function defined to get suggestion on volume
 def suggest_volume():
     global avg_rms
-    print("\nSuggestion on volumne : ")
+    print("\nSuggestion on volumne : ", end = ' ')
 
     if(avg_rms>0.00001):
-        print("High")
+        print("High Volume")
     else:
-        print("Low")
+        print("Low Volume")
 
 
 ## defining main function
 def main():
     global file
     print("Select Audio file : ")
     file = filedialog.askopenfilename(title="Select an Audio file", filetypes=[("Audio Files", "*.mp3"), ("All Files", "*.*")])
     if (file != ""):
         print(file)
+        mp3towav()
         # playsound(file)
-
-        ## calling play_pause_stop function
-        # play_pause_stop(file)
     else:
         print("No File Selected")
```

### Comparing `pyvolsuggester-0.0.1/License.txt` & `pyvolsuggester-0.0.2/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-0.0.1/README.md` & `pyvolsuggester-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,14 @@
 
 ### Package Usage
 ```
 - from PyVolSuggester import Suggester
     - This command will install all the uninstalled required libraries used in script.
 - Suggester.main()
     - This will prompt user for input of audio file selection.
-- Suggester.mp3towav()
-	- This will convert the selected .mp3 audio file to .wav file.
 - Suggester.extract()
 	- This will extract the generic features of the selected audio file.
 - Suggester.play_pause_stop()
 	- This will allow user to play, plause and stop the audio file.
 - Suggester.amplitude_wave()
 	- This will generate a amplitude over time plot and save it as an image to output directory.
 - Suggester.spectogram()
```

### Comparing `pyvolsuggester-0.0.1/pyproject.toml` & `pyvolsuggester-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,82 @@
 
-[project]
+[project] ## --------------------------------------------------------------------------------------------------------------------------------------
 # This is the name of your project. The first time you publish this
 # package, this name will be registered for you. It will determine how
 # users can install this project, e.g.:
 #
 # $ pip install sampleproject
 #
 # And where it will live on PyPI: https://pypi.org/project/sampleproject/
 #
 # There are some restrictions on what makes a valid project name
 # specification here:
 # https://packaging.python.org/specifications/core-metadata/#name
-name = "PyVolSuggester"  # Required
+name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.1"  # Required
+version = "0.0.2"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
-description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional
+description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
 # the body of text which users will see when they visit PyPI.
 #
 # Often, this is the same as your README, so you can just read it in from
 # that file directly (as we have already done above)
 #
 # This field corresponds to the "Description" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#description-optional
-readme = "README.md" # Optional
+readme = "README.md" # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-requires-python = ">=3.7"
+requires-python = ">=3.7" ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is either text indicating the license for the distribution, or a file
 # that contains the license
 # https://packaging.python.org/en/latest/specifications/core-metadata/#license
-license = {file = "License.txt"}
+license = {file = "License.txt"} ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This field adds keywords for your project which will appear on the
 # project page. What does your project relate to?
 #
 # Note that this is a list of additional keywords, separated
 # by commas, to be used to assist searching for the distribution in a
 # larger catalog.
 keywords = ["audio", "audio-feature-extraction", "volumne-suggester", "amplitude-wave", "spectogram", "RMS/Energy-spectogram", "zero-crossing-rate", "mel-frequency-cepstral-coefficients", "mel-frequency-spectogram", "chroma-feature", "tempogram"]  # Optional
+  ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This should be your name or the name of the organization who originally
 # authored the project, and a valid email address corresponding to the name
 # listed.
 authors = [
   {name="Akash Rajak", email="aakashrajak02@gmail.com"}
-]# Optional
+]# Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This should be your name or the names of the organization who currently
 # maintains the project, and a valid email address corresponding to the name
 # listed.
 maintainers = [
   {name="Akash Rajak", email="aakashrajak02@gmail.com" }
-] # Optional
+] # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Classifiers help users find your project by categorizing it.
 #
 # For a list of valid classifiers, see https://pypi.org/classifiers/
-classifiers = [  # Optional
+classifiers = [  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
   "Development Status :: 3 - Alpha",
 
   # Indicate who your project is intended for
@@ -111,45 +112,45 @@
 # dependencies). Users will be able to install these using the "extras"
 # syntax, for example:
 #
 #   $ pip install sampleproject[dev]
 #
 # Similar to `dependencies` above, these must be valid existing
 # projects.
-[project.optional-dependencies] # Optional
+[project.optional-dependencies] # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 #dev = ["check-manifest"]
 #test = ["coverage"]
 
 # List URLs that are relevant to your project
 #
 # This field corresponds to the "Project-URL" and "Home-Page" metadata fields:
 # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
 # https://packaging.python.org/specifications/core-metadata/#home-page-optional
 #
 # Examples listed include a pattern for specifying where the package tracks
 # issues, where the source is hosted, where to say thanks to the package
 # maintainers, and where to support the project financially. The key is
 # what's used to render the link text on PyPI.
-#[project.urls]  # Optional
-#"Homepage" = "https://github.com/pypa/sampleproject"
-#"Bug Reports" = "https://github.com/pypa/sampleproject/issues"
-#"Funding" = "https://donate.pypi.org"
+[project.urls]  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
+"Homepage" = "https://github.com/akash-rajak/PyVolSuggester"
+"Bug Reports" = "https://github.com/akash-rajak/PyVolSuggester/issues"
+"Funding" = "https://donate.pypi.org"
 #"Say Thanks!" = "http://saythanks.io/to/example"
-#"Source" = "https://github.com/pypa/sampleproject/"
+"Source" = "https://github.com/akash-rajak/PyVolSuggester"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 #[project.scripts]  # Optional
 #sample = "sample:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 #[tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 #package-data = {"sample" = ["*.dat"]}
 
-[build-system]
+[build-system] ## --------------------------------------------------------------------------------------------------------------------------------------
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `pyvolsuggester-0.0.1/PKG-INFO` & `pyvolsuggester-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Metadata-Version: 2.1
 Name: PyVolSuggester
-Version: 0.0.1
+Version: 0.0.2
 Summary: Does audio feature extraction and suggest the feasible volumne for better feeling and experience.
+Project-URL: Homepage, https://github.com/akash-rajak/PyVolSuggester
+Project-URL: Bug Reports, https://github.com/akash-rajak/PyVolSuggester/issues
+Project-URL: Funding, https://donate.pypi.org
+Project-URL: Source, https://github.com/akash-rajak/PyVolSuggester
 Author-email: Akash Rajak <aakashrajak02@gmail.com>
 Maintainer-email: Akash Rajak <aakashrajak02@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Akash Rajak]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -120,16 +124,14 @@
 
 ### Package Usage
 ```
 - from PyVolSuggester import Suggester
     - This command will install all the uninstalled required libraries used in script.
 - Suggester.main()
     - This will prompt user for input of audio file selection.
-- Suggester.mp3towav()
-	- This will convert the selected .mp3 audio file to .wav file.
 - Suggester.extract()
 	- This will extract the generic features of the selected audio file.
 - Suggester.play_pause_stop()
 	- This will allow user to play, plause and stop the audio file.
 - Suggester.amplitude_wave()
 	- This will generate a amplitude over time plot and save it as an image to output directory.
 - Suggester.spectogram()
```

