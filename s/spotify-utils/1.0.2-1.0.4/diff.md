# Comparing `tmp/spotify-utils-1.0.2.tar.gz` & `tmp/spotify_utils-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-utils-1.0.2.tar", max compression
+gzip compressed data, was "spotify_utils-1.0.4.tar", max compression
```

## Comparing `spotify-utils-1.0.2.tar` & `spotify_utils-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    34888 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/LICENSE
--rw-r--r--   0        0        0     7818 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/README.md
--rw-r--r--   0        0        0      721 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/__init__.py
--rw-r--r--   0        0        0      501 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/config.py
--rw-r--r--   0        0        0      473 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/main.py
--rw-r--r--   0        0        0        0 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/settings.toml
--rw-r--r--   0        0        0        0 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/src/__init__.py
--rw-r--r--   0        0        0      794 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/src/auth.py
--rw-r--r--   0        0        0      733 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/src/file_operations.py
--rw-r--r--   0        0        0     7346 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/src/playlists.py
--rw-r--r--   0        0        0      114 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/src/user.py
--rw-r--r--   0        0        0     5395 2022-05-12 22:10:34.476413 spotify-utils-1.0.2/spotify_utils/templates/playlists.html
--rw-r--r--   0        0        0     9028 2022-05-12 22:10:37.768078 spotify-utils-1.0.2/setup.py
--rw-r--r--   0        0        0     8713 2022-05-12 22:10:37.768587 spotify-utils-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34888 2023-05-26 15:31:13.042242 spotify_utils-1.0.4/LICENSE
+-rw-r--r--   0        0        0     7570 2023-05-26 15:31:13.042242 spotify_utils-1.0.4/README.md
+-rw-r--r--   0        0        0      721 2023-05-26 15:31:13.043242 spotify_utils-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 15:31:13.066241 spotify_utils-1.0.4/spotify_utils/__init__.py
+-rw-r--r--   0        0        0      501 2023-05-26 15:31:13.043242 spotify_utils-1.0.4/spotify_utils/config.py
+-rw-r--r--   0        0        0      473 2023-05-26 15:31:13.043242 spotify_utils-1.0.4/spotify_utils/main.py
+-rw-r--r--   0        0        0        0 2023-05-26 15:31:13.066241 spotify_utils-1.0.4/spotify_utils/settings.toml
+-rw-r--r--   0        0        0        0 2023-05-26 15:31:13.066241 spotify_utils-1.0.4/spotify_utils/src/__init__.py
+-rw-r--r--   0        0        0      794 2023-05-26 15:31:13.043242 spotify_utils-1.0.4/spotify_utils/src/auth.py
+-rw-r--r--   0        0        0      733 2023-05-26 15:31:13.043242 spotify_utils-1.0.4/spotify_utils/src/file_operations.py
+-rw-r--r--   0        0        0     7346 2023-05-26 15:31:13.043242 spotify_utils-1.0.4/spotify_utils/src/playlists.py
+-rw-r--r--   0        0        0      114 2023-05-26 15:31:13.043242 spotify_utils-1.0.4/spotify_utils/src/user.py
+-rw-r--r--   0        0        0     5395 2023-05-26 15:31:13.044242 spotify_utils-1.0.4/spotify_utils/templates/playlists.html
+-rw-r--r--   0        0        0     8528 1970-01-01 00:00:00.000000 spotify_utils-1.0.4/PKG-INFO
```

### Comparing `spotify-utils-1.0.2/LICENSE` & `spotify_utils-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify-utils-1.0.2/README.md` & `spotify_utils-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,56 @@
+Metadata-Version: 2.1
+Name: spotify-utils
+Version: 1.0.4
+Summary: An awesome and easy-to-use CLI for various Spotify® utility tasks
+Home-page: https://gitlab.com/sustineo/spotify-utils
+License: GPL-3.0-only
+Keywords: spotify,CLI,utilities
+Author: Fabian Eulitz
+Author-email: dev@sustineo.de
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: spotipy (>=2.23.0,<3.0.0)
+Requires-Dist: tabulate (>=0.8.10,<0.9.0)
+Requires-Dist: typer (>=0.4.2,<0.5.0)
+Project-URL: Repository, https://gitlab.com/sustineo/spotify-utils
+Description-Content-Type: text/markdown
+
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 
-[![GitHub issues](https://img.shields.io/github/issues/fabieu/spotify-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/issues)
-[![PyPI](https://img.shields.io/pypi/v/spotify-utils?style=flat-square)](https://pypi.org/project/spotify-utils/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-utils?style=flat-square)](https://pypi.org/project/spotify-utils/)
-[![CircleCI](https://img.shields.io/circleci/build/github/fabieu/spotify-utils?style=flat-square&token=129776381708fd465360ca07ccf7fecec9346def)](https://github.com/fabieu/spotify-utils)
-[![GitHub](https://img.shields.io/github/license/fabieu/spotify-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/blob/main/LICENSE)
+![PyPI](https://img.shields.io/pypi/v/spotify-utils?style=for-the-badge)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-utils?style=for-the-badge)
+![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/spotify-utils?style=for-the-badge)
+![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/spotify-utils?style=for-the-badge)
+![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/spotify-utils?style=for-the-badge)
+![GitLab](https://img.shields.io/gitlab/license/sustineo/spotify-utils?style=for-the-badge)
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/fabieu/spotify-utils">
-    <img src="https://raw.githubusercontent.com/fabieu/spotify-utils/main/docs/assets/media_player.svg" alt="Logo" width="200" height="200">
+  <a href="https://gitlab.com/sustineo/spotify-utils">
+    <img src="https://gitlab.com/sustineo/spotify-utils/-/raw/main/docs/assets/media_player.svg" alt="Logo" width="200" height="200">
   </a>
 
   <h2 align="center">spotify-utils</h2>
 
   <p align="center">
     An awesome and easy-to-use CLI for various Spotify&reg; utility tasks!
     <br />
-    <a href=https://github.com/fabieu/spotify-utils/issues/new/choose">Report Bug</a>
+    <a href=https://gitlab.com/sustineo/spotify-utils/-/issues">Report Bug</a>
     ·
-    <a href="https://github.com/fabieu/spotify-utils/issues/new/choose">Request Feature</a>
+    <a href="https://gitlab.com/sustineo/spotify-utils/-/issues">Request Feature</a>
   </p>
 </div>
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
@@ -148,26 +173,26 @@
 
 ### Export playlist as beautiful HTML file
 
 ```text
 spotify-utils playlists export --html
 ```
 
-![HTML export](https://raw.githubusercontent.com/fabieu/spotify-utils/main/docs/assets/examples/html_export.png)
+![HTML export](https://gitlab.com/sustineo/spotify-utils/-/raw/main/docs/assets/examples/html_export.png)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
 - [ ] Improve help sections of the CLI
 - [ ] Add additional functionality
 
-See the [open issues](https://github.com/fabieu/spotify-utils/issues) for a full list of proposed features (and known issues).
+See the [open issues](https://gitlab.com/sustineo/spotify-utils/-/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
 
 ## Contributing
 
@@ -194,16 +219,14 @@
 
 <!-- CONTACT -->
 
 ## Contact
 
 Fabian Eulitz - [@sustineo\_](https://twitter.com/sustineo_) - dev@sustineo.de
 
-Project Link: [https://github.com/fabieu/spotify-utils](https://github.com/fabieu/spotify-utils)
-
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ACKNOWLEDGMENTS -->
 
 ## Acknowledgments
 
 - [Typer](https://github.com/tiangolo/typer)
@@ -215,7 +238,8 @@
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Disclaimer
 
 This project isn’t endorsed by Spotify AB and doesn’t reflect the views or opinions of Spotify AB or anyone officially involved in producing or managing Spotify&reg;
 
 <p align="right">(<a href="#top">back to top</a>)</p>
+
```

#### html2text {}

```diff
@@ -1,18 +1,29 @@
- [![GitHub issues](https://img.shields.io/github/issues/fabieu/spotify-
-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/issues) [!
-[PyPI](https://img.shields.io/pypi/v/spotify-utils?style=flat-square)](https://
-pypi.org/project/spotify-utils/) [![PyPI - Python Version](https://
-img.shields.io/pypi/pyversions/spotify-utils?style=flat-square)](https://
-pypi.org/project/spotify-utils/) [![CircleCI](https://img.shields.io/circleci/
-build/github/fabieu/spotify-utils?style=flat-
-square&token=129776381708fd465360ca07ccf7fecec9346def)](https://github.com/
-fabieu/spotify-utils) [![GitHub](https://img.shields.io/github/license/fabieu/
-spotify-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/blob/
-main/LICENSE)
+Metadata-Version: 2.1 Name: spotify-utils Version: 1.0.4 Summary: An awesome
+and easy-to-use CLI for various SpotifyÂ® utility tasks Home-page: https://
+gitlab.com/sustineo/spotify-utils License: GPL-3.0-only Keywords:
+spotify,CLI,utilities Author: Fabian Eulitz Author-email: dev@sustineo.de
+Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
+(>=3.1.2,<4.0.0) Requires-Dist: dynaconf (>=3.1.12,<4.0.0) Requires-Dist:
+spotipy (>=2.23.0,<3.0.0) Requires-Dist: tabulate (>=0.8.10,<0.9.0) Requires-
+Dist: typer (>=0.4.2,<0.5.0) Project-URL: Repository, https://gitlab.com/
+sustineo/spotify-utils Description-Content-Type: text/markdown
+ ![PyPI](https://img.shields.io/pypi/v/spotify-utils?style=for-the-badge) !
+[PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-
+utils?style=for-the-badge) ![Gitlab pipeline status](https://img.shields.io/
+gitlab/pipeline-status/sustineo/spotify-utils?style=for-the-badge) ![GitLab
+issues](https://img.shields.io/gitlab/issues/open/sustineo/spotify-
+utils?style=for-the-badge) ![GitLab merge requests](https://img.shields.io/
+gitlab/merge-requests/open-raw/sustineo/spotify-utils?style=for-the-badge) !
+[GitLab](https://img.shields.io/gitlab/license/sustineo/spotify-
+utils?style=for-the-badge)
                                     [Logo]
                            ***** spotify-utils *****
       An awesome and easy-to-use CLI for various Spotify® utility tasks!
                          Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
@@ -66,20 +77,20 @@
 spotify-utils playlists duplicates --verbose ``` Found 43 duplicate tracks
 across 20 playlists | | name | artists | playlists | track_id | |---|----------
 ------|-------------------------|------------------------|---------------------
 ---| | 0 | Piercing Light | League of Legends, Mako | Rock, Sonos Mainstream |
 0163ud7I4Vb0ID5K7WBkq9 | | 1 |Edge Of The Earth | Thirty Seconds To Mars| Rock,
 Pop|0g9IOJwdElaCZEvcqGRP4b | | ... |... |... |... |... | ### Export playlist as
 beautiful HTML file ```text spotify-utils playlists export --html ``` ![HTML
-export](https://raw.githubusercontent.com/fabieu/spotify-utils/main/docs/
-assets/examples/html_export.png)
+export](https://gitlab.com/sustineo/spotify-utils/-/raw/main/docs/assets/
+examples/html_export.png)
                                                                   (back_to_top)
  ## Roadmap - [ ] Improve help sections of the CLI - [ ] Add additional
-functionality See the [open issues](https://github.com/fabieu/spotify-utils/
-issues) for a full list of proposed features (and known issues).
+functionality See the [open issues](https://gitlab.com/sustineo/spotify-utils/-
+/issues) for a full list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
@@ -87,16 +98,15 @@
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (back_to_top)
  ## License Distributed under the GPL-3.0 License. See [LICENSE](LICENSE) for
 more information.
                                                                   (back_to_top)
  ## Contact Fabian Eulitz - [@sustineo\_](https://twitter.com/sustineo_) -
-dev@sustineo.de Project Link: [https://github.com/fabieu/spotify-utils](https:/
-/github.com/fabieu/spotify-utils)
+dev@sustineo.de
                                                                   (back_to_top)
  ## Acknowledgments - [Typer](https://github.com/tiangolo/typer) - [Spotipy]
 (https://github.com/plamere/spotipy) - [Vermin](https://github.com/netromdk/
 vermin) - [Shields.io](https://shields.io) - [Choose an Open Source License]
 (https://choosealicense.com)
                                                                   (back_to_top)
 ## Disclaimer This project isnât endorsed by Spotify AB and doesnât reflect
```

### Comparing `spotify-utils-1.0.2/pyproject.toml` & `spotify_utils-1.0.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "spotify-utils"
-version = "1.0.2"
+version = "1.0.4"
 description = "An awesome and easy-to-use CLI for various Spotify® utility tasks"
 license = "GPL-3.0-only"
 authors = ["Fabian Eulitz <dev@sustineo.de>"]
-documentation = ""
-repository = "https://github.com/fabieu/spotify-utils"
-keywords = ["spotify", "utility"]
+repository = "https://gitlab.com/sustineo/spotify-utils"
+keywords = ["spotify", "CLI", "utilities"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-spotipy = "^2.19.0"
-typer = "^0.4.1"
-tabulate = "^0.8.9"
+spotipy = "^2.23.0"
+typer = "^0.4.2"
+tabulate = "^0.8.10"
 Jinja2 = "^3.1.2"
-dynaconf = "^3.1.8"
+dynaconf = "^3.1.12"
 
-[tool.poetry.dev-dependencies]
-autopep8 = "^1.6.0"
-pytest = "^7.1.2"
-vermin = "^1.3.3"
+[tool.poetry.group.dev.dependencies]
+autopep8 = "^1.7.0"
+pytest = "^7.3.1"
+vermin = "^1.5.1"
 
 [tool.poetry.scripts]
 spotify-utils = "spotify_utils.main:app"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spotify-utils-1.0.2/spotify_utils/src/auth.py` & `spotify_utils-1.0.4/spotify_utils/src/auth.py`

 * *Files identical despite different names*

### Comparing `spotify-utils-1.0.2/spotify_utils/src/file_operations.py` & `spotify_utils-1.0.4/spotify_utils/src/file_operations.py`

 * *Files identical despite different names*

### Comparing `spotify-utils-1.0.2/spotify_utils/src/playlists.py` & `spotify_utils-1.0.4/spotify_utils/src/playlists.py`

 * *Files identical despite different names*

### Comparing `spotify-utils-1.0.2/spotify_utils/templates/playlists.html` & `spotify_utils-1.0.4/spotify_utils/templates/playlists.html`

 * *Files identical despite different names*

### Comparing `spotify-utils-1.0.2/PKG-INFO` & `spotify_utils-1.0.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,32 @@
-Metadata-Version: 2.1
-Name: spotify-utils
-Version: 1.0.2
-Summary: An awesome and easy-to-use CLI for various Spotify® utility tasks
-Home-page: https://github.com/fabieu/spotify-utils
-License: GPL-3.0-only
-Keywords: spotify,utility
-Author: Fabian Eulitz
-Author-email: dev@sustineo.de
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: dynaconf (>=3.1.8,<4.0.0)
-Requires-Dist: spotipy (>=2.19.0,<3.0.0)
-Requires-Dist: tabulate (>=0.8.9,<0.9.0)
-Requires-Dist: typer (>=0.4.1,<0.5.0)
-Project-URL: Repository, https://github.com/fabieu/spotify-utils
-Description-Content-Type: text/markdown
-
 <div id="top"></div>
 <!-- PROJECT SHIELDS -->
 
-[![GitHub issues](https://img.shields.io/github/issues/fabieu/spotify-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/issues)
-[![PyPI](https://img.shields.io/pypi/v/spotify-utils?style=flat-square)](https://pypi.org/project/spotify-utils/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-utils?style=flat-square)](https://pypi.org/project/spotify-utils/)
-[![CircleCI](https://img.shields.io/circleci/build/github/fabieu/spotify-utils?style=flat-square&token=129776381708fd465360ca07ccf7fecec9346def)](https://github.com/fabieu/spotify-utils)
-[![GitHub](https://img.shields.io/github/license/fabieu/spotify-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/blob/main/LICENSE)
+![PyPI](https://img.shields.io/pypi/v/spotify-utils?style=for-the-badge)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-utils?style=for-the-badge)
+![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline-status/sustineo/spotify-utils?style=for-the-badge)
+![GitLab issues](https://img.shields.io/gitlab/issues/open/sustineo/spotify-utils?style=for-the-badge)
+![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open-raw/sustineo/spotify-utils?style=for-the-badge)
+![GitLab](https://img.shields.io/gitlab/license/sustineo/spotify-utils?style=for-the-badge)
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/fabieu/spotify-utils">
-    <img src="https://raw.githubusercontent.com/fabieu/spotify-utils/main/docs/assets/media_player.svg" alt="Logo" width="200" height="200">
+  <a href="https://gitlab.com/sustineo/spotify-utils">
+    <img src="https://gitlab.com/sustineo/spotify-utils/-/raw/main/docs/assets/media_player.svg" alt="Logo" width="200" height="200">
   </a>
 
   <h2 align="center">spotify-utils</h2>
 
   <p align="center">
     An awesome and easy-to-use CLI for various Spotify&reg; utility tasks!
     <br />
-    <a href=https://github.com/fabieu/spotify-utils/issues/new/choose">Report Bug</a>
+    <a href=https://gitlab.com/sustineo/spotify-utils/-/issues">Report Bug</a>
     ·
-    <a href="https://github.com/fabieu/spotify-utils/issues/new/choose">Request Feature</a>
+    <a href="https://gitlab.com/sustineo/spotify-utils/-/issues">Request Feature</a>
   </p>
 </div>
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
@@ -171,26 +149,26 @@
 
 ### Export playlist as beautiful HTML file
 
 ```text
 spotify-utils playlists export --html
 ```
 
-![HTML export](https://raw.githubusercontent.com/fabieu/spotify-utils/main/docs/assets/examples/html_export.png)
+![HTML export](https://gitlab.com/sustineo/spotify-utils/-/raw/main/docs/assets/examples/html_export.png)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ROADMAP -->
 
 ## Roadmap
 
 - [ ] Improve help sections of the CLI
 - [ ] Add additional functionality
 
-See the [open issues](https://github.com/fabieu/spotify-utils/issues) for a full list of proposed features (and known issues).
+See the [open issues](https://gitlab.com/sustineo/spotify-utils/-/issues) for a full list of proposed features (and known issues).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- CONTRIBUTING -->
 
 ## Contributing
 
@@ -217,16 +195,14 @@
 
 <!-- CONTACT -->
 
 ## Contact
 
 Fabian Eulitz - [@sustineo\_](https://twitter.com/sustineo_) - dev@sustineo.de
 
-Project Link: [https://github.com/fabieu/spotify-utils](https://github.com/fabieu/spotify-utils)
-
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 <!-- ACKNOWLEDGMENTS -->
 
 ## Acknowledgments
 
 - [Typer](https://github.com/tiangolo/typer)
@@ -238,8 +214,7 @@
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Disclaimer
 
 This project isn’t endorsed by Spotify AB and doesn’t reflect the views or opinions of Spotify AB or anyone officially involved in producing or managing Spotify&reg;
 
 <p align="right">(<a href="#top">back to top</a>)</p>
-
```

#### html2text {}

```diff
@@ -1,30 +1,16 @@
-Metadata-Version: 2.1 Name: spotify-utils Version: 1.0.2 Summary: An awesome
-and easy-to-use CLI for various SpotifyÂ® utility tasks Home-page: https://
-github.com/fabieu/spotify-utils License: GPL-3.0-only Keywords: spotify,utility
-Author: Fabian Eulitz Author-email: dev@sustineo.de Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Requires-Dist: Jinja2
-(>=3.1.2,<4.0.0) Requires-Dist: dynaconf (>=3.1.8,<4.0.0) Requires-Dist:
-spotipy (>=2.19.0,<3.0.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0) Requires-
-Dist: typer (>=0.4.1,<0.5.0) Project-URL: Repository, https://github.com/
-fabieu/spotify-utils Description-Content-Type: text/markdown
- [![GitHub issues](https://img.shields.io/github/issues/fabieu/spotify-
-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/issues) [!
-[PyPI](https://img.shields.io/pypi/v/spotify-utils?style=flat-square)](https://
-pypi.org/project/spotify-utils/) [![PyPI - Python Version](https://
-img.shields.io/pypi/pyversions/spotify-utils?style=flat-square)](https://
-pypi.org/project/spotify-utils/) [![CircleCI](https://img.shields.io/circleci/
-build/github/fabieu/spotify-utils?style=flat-
-square&token=129776381708fd465360ca07ccf7fecec9346def)](https://github.com/
-fabieu/spotify-utils) [![GitHub](https://img.shields.io/github/license/fabieu/
-spotify-utils?style=flat-square)](https://github.com/fabieu/spotify-utils/blob/
-main/LICENSE)
+ ![PyPI](https://img.shields.io/pypi/v/spotify-utils?style=for-the-badge) !
+[PyPI - Python Version](https://img.shields.io/pypi/pyversions/spotify-
+utils?style=for-the-badge) ![Gitlab pipeline status](https://img.shields.io/
+gitlab/pipeline-status/sustineo/spotify-utils?style=for-the-badge) ![GitLab
+issues](https://img.shields.io/gitlab/issues/open/sustineo/spotify-
+utils?style=for-the-badge) ![GitLab merge requests](https://img.shields.io/
+gitlab/merge-requests/open-raw/sustineo/spotify-utils?style=for-the-badge) !
+[GitLab](https://img.shields.io/gitlab/license/sustineo/spotify-
+utils?style=for-the-badge)
                                     [Logo]
                            ***** spotify-utils *****
       An awesome and easy-to-use CLI for various Spotify® utility tasks!
                          Report_Bug Â· Request_Feature
   Table of Contents
    1. About_The_Project
           o Built_With
@@ -78,20 +64,20 @@
 spotify-utils playlists duplicates --verbose ``` Found 43 duplicate tracks
 across 20 playlists | | name | artists | playlists | track_id | |---|----------
 ------|-------------------------|------------------------|---------------------
 ---| | 0 | Piercing Light | League of Legends, Mako | Rock, Sonos Mainstream |
 0163ud7I4Vb0ID5K7WBkq9 | | 1 |Edge Of The Earth | Thirty Seconds To Mars| Rock,
 Pop|0g9IOJwdElaCZEvcqGRP4b | | ... |... |... |... |... | ### Export playlist as
 beautiful HTML file ```text spotify-utils playlists export --html ``` ![HTML
-export](https://raw.githubusercontent.com/fabieu/spotify-utils/main/docs/
-assets/examples/html_export.png)
+export](https://gitlab.com/sustineo/spotify-utils/-/raw/main/docs/assets/
+examples/html_export.png)
                                                                   (back_to_top)
  ## Roadmap - [ ] Improve help sections of the CLI - [ ] Add additional
-functionality See the [open issues](https://github.com/fabieu/spotify-utils/
-issues) for a full list of proposed features (and known issues).
+functionality See the [open issues](https://gitlab.com/sustineo/spotify-utils/-
+/issues) for a full list of proposed features (and known issues).
                                                                   (back_to_top)
  ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
@@ -99,16 +85,15 @@
 AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
 AmazingFeature`) 5. Open a Pull Request
                                                                   (back_to_top)
  ## License Distributed under the GPL-3.0 License. See [LICENSE](LICENSE) for
 more information.
                                                                   (back_to_top)
  ## Contact Fabian Eulitz - [@sustineo\_](https://twitter.com/sustineo_) -
-dev@sustineo.de Project Link: [https://github.com/fabieu/spotify-utils](https:/
-/github.com/fabieu/spotify-utils)
+dev@sustineo.de
                                                                   (back_to_top)
  ## Acknowledgments - [Typer](https://github.com/tiangolo/typer) - [Spotipy]
 (https://github.com/plamere/spotipy) - [Vermin](https://github.com/netromdk/
 vermin) - [Shields.io](https://shields.io) - [Choose an Open Source License]
 (https://choosealicense.com)
                                                                   (back_to_top)
 ## Disclaimer This project isnât endorsed by Spotify AB and doesnât reflect
```

