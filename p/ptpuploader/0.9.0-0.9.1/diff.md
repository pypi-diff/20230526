# Comparing `tmp/PtpUploader-0.9.0.tar.gz` & `tmp/PtpUploader-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PtpUploader-0.9.0.tar", max compression
+gzip compressed data, was "PtpUploader-0.9.1.tar", max compression
```

## Comparing `PtpUploader-0.9.0.tar` & `PtpUploader-0.9.1.tar`

### file list

```diff
@@ -1,155 +1,156 @@
--rw-r--r--   0        0        0     1390 2022-02-01 20:56:46.050360 PtpUploader-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      534 2022-01-09 18:48:43.901135 PtpUploader-0.9.0/src/PtpUploader/Database.py
--rw-r--r--   0        0        0     5572 2021-11-12 03:05:59.939797 PtpUploader-0.9.0/src/PtpUploader/Helper.py
--rw-r--r--   0        0        0      435 2022-01-26 18:14:18.298719 PtpUploader-0.9.0/src/PtpUploader/ImageHost/Base.py
--rw-r--r--   0        0        0      834 2022-01-30 22:47:54.195405 PtpUploader-0.9.0/src/PtpUploader/ImageHost/Catbox.py
--rw-r--r--   0        0        0     1515 2022-01-30 22:42:55.221430 PtpUploader-0.9.0/src/PtpUploader/ImageHost/ImageUploader.py
--rw-r--r--   0        0        0     1147 2022-01-26 18:14:18.342720 PtpUploader-0.9.0/src/PtpUploader/ImageHost/ImgBB.py
--rw-r--r--   0        0        0     1271 2022-01-26 18:14:18.330720 PtpUploader-0.9.0/src/PtpUploader/ImageHost/PtpImg.py
--rw-r--r--   0        0        0      320 2022-01-26 18:14:18.294719 PtpUploader-0.9.0/src/PtpUploader/ImageHost/__init__.py
--rw-r--r--   0        0        0     3780 2021-10-23 18:03:08.170129 PtpUploader-0.9.0/src/PtpUploader/IncludedFileList.py
--rw-r--r--   0        0        0     1349 2021-11-13 03:18:45.463745 PtpUploader-0.9.0/src/PtpUploader/InformationSource/Imdb.py
--rw-r--r--   0        0        0     1625 2021-10-23 18:02:25.708816 PtpUploader-0.9.0/src/PtpUploader/InformationSource/MoviePoster.py
--rw-r--r--   0        0        0      144 2021-10-23 18:02:12.324403 PtpUploader-0.9.0/src/PtpUploader/InformationSource/__init__.py
--rw-r--r--   0        0        0    19970 2022-01-21 14:19:00.310038 PtpUploader-0.9.0/src/PtpUploader/Job/CheckAnnouncement.py
--rw-r--r--   0        0        0     1438 2021-11-02 02:35:37.787083 PtpUploader-0.9.0/src/PtpUploader/Job/Delete.py
--rw-r--r--   0        0        0      173 2021-10-23 18:04:21.460395 PtpUploader-0.9.0/src/PtpUploader/Job/FinishedJobPhase.py
--rw-r--r--   0        0        0     1456 2021-10-26 01:00:14.730265 PtpUploader-0.9.0/src/PtpUploader/Job/JobRunningState.py
--rw-r--r--   0        0        0      492 2021-10-23 18:04:21.460395 PtpUploader-0.9.0/src/PtpUploader/Job/JobStartMode.py
--rw-r--r--   0        0        0     1389 2021-11-13 17:23:51.379526 PtpUploader-0.9.0/src/PtpUploader/Job/LoadFile.py
--rw-r--r--   0        0        0     7055 2022-01-15 03:35:34.861384 PtpUploader-0.9.0/src/PtpUploader/Job/Supervisor.py
--rw-r--r--   0        0        0    22739 2022-01-30 22:45:04.709750 PtpUploader-0.9.0/src/PtpUploader/Job/Upload.py
--rw-r--r--   0        0        0     2924 2022-01-21 21:03:36.392264 PtpUploader-0.9.0/src/PtpUploader/Job/WorkerBase.py
--rw-r--r--   0        0        0      144 2021-10-23 18:04:21.460395 PtpUploader-0.9.0/src/PtpUploader/Job/__init__.py
--rw-r--r--   0        0        0     2384 2022-01-15 19:59:23.621698 PtpUploader-0.9.0/src/PtpUploader/MyGlobals.py
--rw-r--r--   0        0        0     1870 2021-11-02 02:35:38.003090 PtpUploader-0.9.0/src/PtpUploader/NfoParser.py
--rw-r--r--   0        0        0       82 2020-01-12 18:29:37.664603 PtpUploader-0.9.0/src/PtpUploader/Notifier.example.ini
--rw-r--r--   0        0        0     1285 2021-11-02 02:35:38.159095 PtpUploader-0.9.0/src/PtpUploader/Notifier.py
--rw-r--r--   0        0        0    12484 2022-01-15 03:35:34.861384 PtpUploader-0.9.0/src/PtpUploader/Ptp.py
--rw-r--r--   0        0        0     4512 2021-11-04 18:18:46.496345 PtpUploader-0.9.0/src/PtpUploader/PtpImdbInfo.py
--rw-r--r--   0        0        0     6099 2021-11-13 17:23:51.587532 PtpUploader-0.9.0/src/PtpUploader/PtpMovieSearchResult.py
--rw-r--r--   0        0        0     4814 2021-10-28 23:26:09.171292 PtpUploader-0.9.0/src/PtpUploader/PtpSubtitle.py
--rw-r--r--   0        0        0      843 2021-10-29 04:32:53.333550 PtpUploader-0.9.0/src/PtpUploader/PtpUploaderException.py
--rw-r--r--   0        0        0      735 2021-10-31 19:22:18.833307 PtpUploader-0.9.0/src/PtpUploader/PtpUploaderMessage.py
--rw-r--r--   0        0        0     7689 2022-02-01 08:09:32.526775 PtpUploader-0.9.0/src/PtpUploader/ReleaseDescriptionFormatter.py
--rw-r--r--   0        0        0     8574 2022-01-24 17:20:27.430441 PtpUploader-0.9.0/src/PtpUploader/ReleaseExtractor.py
--rw-r--r--   0        0        0    12032 2022-01-29 20:52:10.398655 PtpUploader-0.9.0/src/PtpUploader/ReleaseInfo.py
--rw-r--r--   0        0        0     6117 2022-01-30 00:21:23.181864 PtpUploader-0.9.0/src/PtpUploader/ReleaseInfoMaker.py
--rw-r--r--   0        0        0     4508 2021-11-08 02:24:36.360394 PtpUploader-0.9.0/src/PtpUploader/ReleaseNameParser.py
--rw-r--r--   0        0        0     1468 2020-01-12 18:29:37.668603 PtpUploader-0.9.0/src/PtpUploader/SceneGroups.txt
--rw-r--r--   0        0        0     1013 2021-10-23 18:03:08.182130 PtpUploader-0.9.0/src/PtpUploader/ScreenshotList.py
--rw-r--r--   0        0        0     8213 2022-01-20 15:35:18.462021 PtpUploader-0.9.0/src/PtpUploader/Settings.py
--rw-r--r--   0        0        0     7218 2021-11-12 03:06:07.588031 PtpUploader-0.9.0/src/PtpUploader/Source/AlphaRatio.py
--rw-r--r--   0        0        0    14130 2022-01-31 23:23:31.641517 PtpUploader-0.9.0/src/PtpUploader/Source/Cinemageddon.py
--rw-r--r--   0        0        0    10741 2021-11-12 03:06:07.588031 PtpUploader-0.9.0/src/PtpUploader/Source/Cinematik.py
--rw-r--r--   0        0        0     8636 2021-11-12 03:06:07.588031 PtpUploader-0.9.0/src/PtpUploader/Source/DigitalHive.py
--rw-r--r--   0        0        0     6148 2021-11-13 03:33:35.175214 PtpUploader-0.9.0/src/PtpUploader/Source/File.py
--rw-r--r--   0        0        0     7994 2021-11-12 03:06:07.588031 PtpUploader-0.9.0/src/PtpUploader/Source/FunFile.py
--rw-r--r--   0        0        0     9834 2021-11-12 03:06:07.588031 PtpUploader-0.9.0/src/PtpUploader/Source/Gft.py
--rw-r--r--   0        0        0     7083 2021-11-02 02:35:38.091093 PtpUploader-0.9.0/src/PtpUploader/Source/HDBits.py
--rw-r--r--   0        0        0     7994 2021-11-12 03:06:07.588031 PtpUploader-0.9.0/src/PtpUploader/Source/HDTorrents.py
--rw-r--r--   0        0        0    17914 2022-01-24 17:40:51.753744 PtpUploader-0.9.0/src/PtpUploader/Source/Karagarga.py
--rw-r--r--   0        0        0     6201 2022-01-15 03:35:34.861384 PtpUploader-0.9.0/src/PtpUploader/Source/Prowlarr.py
--rw-r--r--   0        0        0     8474 2022-01-20 00:40:14.012654 PtpUploader-0.9.0/src/PtpUploader/Source/SourceBase.py
--rw-r--r--   0        0        0     2016 2021-11-12 00:18:15.943330 PtpUploader-0.9.0/src/PtpUploader/Source/SourceFactory.py
--rw-r--r--   0        0        0     1233 2022-01-30 18:34:35.991070 PtpUploader-0.9.0/src/PtpUploader/Source/Torrent.py
--rw-r--r--   0        0        0     7370 2021-11-12 03:06:07.592031 PtpUploader-0.9.0/src/PtpUploader/Source/TorrentBytes.py
--rw-r--r--   0        0        0     8554 2021-11-12 03:06:07.592031 PtpUploader-0.9.0/src/PtpUploader/Source/TorrentLeech.py
--rw-r--r--   0        0        0      144 2021-10-30 20:46:41.976266 PtpUploader-0.9.0/src/PtpUploader/Source/__init__.py
--rw-r--r--   0        0        0     2181 2022-01-30 20:07:22.305437 PtpUploader-0.9.0/src/PtpUploader/Tool/BdInfo.py
--rw-r--r--   0        0        0     4918 2022-01-20 01:11:11.450812 PtpUploader-0.9.0/src/PtpUploader/Tool/Ffmpeg.py
--rw-r--r--   0        0        0     1767 2021-11-12 19:19:36.755586 PtpUploader-0.9.0/src/PtpUploader/Tool/ImageMagick.py
--rw-r--r--   0        0        0     7903 2022-01-29 20:48:56.824203 PtpUploader-0.9.0/src/PtpUploader/Tool/MediaInfo.py
--rw-r--r--   0        0        0     1294 2022-01-25 16:59:19.237679 PtpUploader-0.9.0/src/PtpUploader/Tool/Mktor.py
--rw-r--r--   0        0        0     4007 2022-01-15 21:11:37.486169 PtpUploader-0.9.0/src/PtpUploader/Tool/Mplayer.py
--rw-r--r--   0        0        0     1210 2022-01-15 21:11:20.917616 PtpUploader-0.9.0/src/PtpUploader/Tool/Mpv.py
--rw-r--r--   0        0        0     5751 2022-01-15 16:47:32.906275 PtpUploader-0.9.0/src/PtpUploader/Tool/Rtorrent.py
--rw-r--r--   0        0        0     5355 2022-01-26 18:14:18.446724 PtpUploader-0.9.0/src/PtpUploader/Tool/ScreenshotMaker.py
--rw-r--r--   0        0        0     2509 2021-11-02 02:35:37.875086 PtpUploader-0.9.0/src/PtpUploader/Tool/Transmission.py
--rw-r--r--   0        0        0     2464 2021-10-23 18:04:01.779787 PtpUploader-0.9.0/src/PtpUploader/Tool/Unrar.py
--rw-r--r--   0        0        0      144 2022-01-29 22:34:24.955207 PtpUploader-0.9.0/src/PtpUploader/Tool/__init__.py
--rw-r--r--   0        0        0        0 2022-01-15 02:22:45.488257 PtpUploader-0.9.0/src/PtpUploader/__init__.py
--rw-r--r--   0        0        0     4428 2022-01-30 22:48:22.020333 PtpUploader-0.9.0/src/PtpUploader/config.default.yml
--rw-r--r--   0        0        0      406 2022-01-15 03:35:34.861384 PtpUploader-0.9.0/src/PtpUploader/manage.py
--rw-r--r--   0        0        0        0 2021-10-27 20:19:43.046508 PtpUploader-0.9.0/src/PtpUploader/web/__init__.py
--rw-r--r--   0        0        0     4728 2022-01-30 18:35:12.188266 PtpUploader-0.9.0/src/PtpUploader/web/forms.py
--rw-r--r--   0        0        0        0 2021-10-29 21:49:40.692371 PtpUploader-0.9.0/src/PtpUploader/web/management/commands/__init__.py
--rw-r--r--   0        0        0     9055 2022-01-30 20:05:11.557031 PtpUploader-0.9.0/src/PtpUploader/web/management/commands/runuploader.py
--rw-r--r--   0        0        0     3991 2021-10-29 20:08:05.328481 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0001_initial.py
--rw-r--r--   0        0        0      606 2021-10-29 20:08:05.328481 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0002_auto_20211025_0320.py
--rw-r--r--   0        0        0      710 2021-10-29 20:08:05.328481 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0003_alter_releaseinfo_jobrunningstate.py
--rw-r--r--   0        0        0     1547 2021-10-29 20:08:05.328481 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0004_auto_20211028_2254.py
--rw-r--r--   0        0        0     1058 2021-10-29 04:35:34.782561 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0005_auto_20211029_0135.py
--rw-r--r--   0        0        0      788 2021-10-29 20:24:02.365956 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0006_auto_20211029_2024.py
--rw-r--r--   0        0        0      389 2021-10-29 20:24:29.450789 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0007_alter_releaseinfo_trumpable.py
--rw-r--r--   0        0        0      410 2021-10-29 20:26:10.989915 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0008_alter_releaseinfo_subtitles.py
--rw-r--r--   0        0        0      410 2021-10-29 21:00:32.157341 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0009_alter_releaseinfo_trumpable.py
--rw-r--r--   0        0        0      410 2021-10-31 19:39:36.461201 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0010_alter_releaseinfo_screenshots.py
--rw-r--r--   0        0        0      412 2021-10-31 19:40:02.722008 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0011_alter_releaseinfo_screenshots.py
--rw-r--r--   0        0        0      414 2021-10-31 19:40:09.426214 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0012_alter_releaseinfo_screenshots.py
--rw-r--r--   0        0        0      827 2021-11-04 03:44:33.946564 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0013_auto_20211104_0344.py
--rw-r--r--   0        0        0      379 2022-01-08 21:47:45.866384 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0014_rename_scheduletimeutc_releaseinfo_scheduletime.py
--rw-r--r--   0        0        0      534 2022-01-15 03:38:15.478735 PtpUploader-0.9.0/src/PtpUploader/web/migrations/0015_alter_releaseinfo_scheduletime.py
--rw-r--r--   0        0        0        0 2021-10-23 23:05:43.143377 PtpUploader-0.9.0/src/PtpUploader/web/migrations/__init__.py
--rw-r--r--   0        0        0      164 2021-10-31 19:22:19.909340 PtpUploader-0.9.0/src/PtpUploader/web/models.py
--rw-r--r--   0        0        0     4463 2022-01-30 19:01:05.739834 PtpUploader-0.9.0/src/PtpUploader/web/settings.py
--rw-r--r--   0        0        0      698 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/delete.png
--rw-r--r--   0        0        0     3384 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/edit.png
--rw-r--r--   0        0        0     1469 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/error.png
--rw-r--r--   0        0        0      235 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/favicon.png
--rw-r--r--   0        0        0      654 2021-10-24 18:34:54.468092 PtpUploader-0.9.0/src/PtpUploader/web/static/film.png
--rw-r--r--   0        0        0      744 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/hourglass.png
--rw-r--r--   0        0        0     6138 2021-10-25 12:19:33.173748 PtpUploader-0.9.0/src/PtpUploader/web/static/normalize.css
--rw-r--r--   0        0        0      399 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/pause.png
--rw-r--r--   0        0        0      894 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/ptp.ico
--rw-r--r--   0        0        0      939 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/sad.png
--rw-r--r--   0        0        0      839 2020-01-12 18:29:37.680603 PtpUploader-0.9.0/src/PtpUploader/web/static/scheduled.png
--rw-r--r--   0        0        0   205319 2021-01-26 20:29:14.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/bulma.min.css
--rw-r--r--   0        0        0     6199 2021-11-08 02:59:40.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/datatables.min.css
--rw-r--r--   0        0        0    92883 2021-11-08 02:31:57.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/datatables.min.js
--rw-r--r--   0        0        0  1196706 2021-09-13 19:10:03.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/fontawesome.all.min.js
--rw-r--r--   0        0        0    89501 2021-03-02 17:27:20.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    22538 2020-05-04 16:11:45.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-confirm.min.css
--rw-r--r--   0        0        0    27896 2020-05-04 16:11:45.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-confirm.min.js
--rw-r--r--   0        0        0   253668 2021-08-20 17:47:54.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-ui.min.js
--rw-r--r--   0        0        0     6007 2021-11-10 02:46:39.496020 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.contextMenu.min.css
--rw-r--r--   0        0        0    27928 2020-05-13 14:12:49.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.contextMenu.min.js
--rw-r--r--   0        0        0   130228 2021-11-10 02:48:34.287557 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.fancytree-all-deps.min.js
--rw-r--r--   0        0        0     5855 2020-05-04 16:11:45.000000 PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.ui.position.min.js
--rw-r--r--   0        0        0    16264 2021-10-24 05:37:24.049207 PtpUploader-0.9.0/src/PtpUploader/web/static/script/select2.min.css
--rw-r--r--   0        0        0    73163 2021-10-24 05:36:50.596177 PtpUploader-0.9.0/src/PtpUploader/web/static/script/select2.min.js
--rw-r--r--   0        0        0    17671 2021-11-10 02:48:34.147552 PtpUploader-0.9.0/src/PtpUploader/web/static/script/ui.fancytree.min.css
--rw-r--r--   0        0        0     5510 2021-11-10 02:34:16.225124 PtpUploader-0.9.0/src/PtpUploader/web/static/skin-win8/icons.gif
--rw-r--r--   0        0        0     3234 2021-11-10 02:50:05.178357 PtpUploader-0.9.0/src/PtpUploader/web/static/skin-win8/loading.gif
--rw-r--r--   0        0        0     4286 2020-01-12 18:29:37.692603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/ar.ico
--rw-r--r--   0        0        0      894 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/cg.ico
--rw-r--r--   0        0        0     4286 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/dh.ico
--rw-r--r--   0        0        0      815 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/file.ico
--rw-r--r--   0        0        0     1086 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/gft.ico
--rw-r--r--   0        0        0     5430 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/hdbits.ico
--rw-r--r--   0        0        0     2862 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/kg.ico
--rw-r--r--   0        0        0     1214 2021-10-31 15:28:16.457289 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/prowlarr.ico
--rw-r--r--   0        0        0     3638 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/rtt.ico
--rw-r--r--   0        0        0     4286 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tby.ico
--rw-r--r--   0        0        0     1430 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tds.ico
--rw-r--r--   0        0        0     1406 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tik.ico
--rw-r--r--   0        0        0     3638 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tl.ico
--rw-r--r--   0        0        0      924 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/torrent.ico
--rw-r--r--   0        0        0      911 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/start.png
--rw-r--r--   0        0        0      674 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/stop.png
--rw-r--r--   0        0        0     2882 2021-11-10 03:21:36.592661 PtpUploader-0.9.0/src/PtpUploader/web/static/style.css
--rw-r--r--   0        0        0     1530 2021-10-30 05:01:03.843218 PtpUploader-0.9.0/src/PtpUploader/web/static/style.css.old
--rw-r--r--   0        0        0      682 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/success.png
--rw-r--r--   0        0        0     1849 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/throbber.gif
--rw-r--r--   0        0        0      851 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/static/warning.png
--rw-r--r--   0        0        0     2463 2022-01-09 19:06:54.373383 PtpUploader-0.9.0/src/PtpUploader/web/templates/bulk.html
--rw-r--r--   0        0        0    16535 2022-01-30 14:45:28.072896 PtpUploader-0.9.0/src/PtpUploader/web/templates/edit_job.html
--rw-r--r--   0        0        0      104 2020-01-12 18:29:37.696603 PtpUploader-0.9.0/src/PtpUploader/web/templates/index.html
--rw-r--r--   0        0        0     7474 2022-01-09 16:33:07.205858 PtpUploader-0.9.0/src/PtpUploader/web/templates/jobs.html
--rw-r--r--   0        0        0     2032 2022-01-17 20:58:24.676675 PtpUploader-0.9.0/src/PtpUploader/web/templates/layout.html
--rw-r--r--   0        0        0     1176 2021-10-24 06:13:08.295163 PtpUploader-0.9.0/src/PtpUploader/web/templates/movieAvailabilityCheck.html
--rw-r--r--   0        0        0     1106 2022-01-30 04:31:25.855006 PtpUploader-0.9.0/src/PtpUploader/web/urls.py
--rw-r--r--   0        0        0    15884 2022-02-01 20:11:22.300530 PtpUploader-0.9.0/src/PtpUploader/web/views.py
--rw-r--r--   0        0        0      393 2021-11-02 02:35:38.291099 PtpUploader-0.9.0/src/PtpUploader/web/wsgi.py
--rw-r--r--   0        0        0     1541 2022-02-01 20:57:37.355639 PtpUploader-0.9.0/setup.py
--rw-r--r--   0        0        0     1203 2022-02-01 20:57:37.356096 PtpUploader-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1390 2022-05-20 16:27:18.155434 PtpUploader-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      534 2022-01-09 18:48:43.901135 PtpUploader-0.9.1/src/PtpUploader/Database.py
+-rw-r--r--   0        0        0     5572 2021-11-12 03:05:59.939797 PtpUploader-0.9.1/src/PtpUploader/Helper.py
+-rw-r--r--   0        0        0      435 2022-01-26 18:14:18.298719 PtpUploader-0.9.1/src/PtpUploader/ImageHost/Base.py
+-rw-r--r--   0        0        0      834 2022-02-17 22:45:52.420144 PtpUploader-0.9.1/src/PtpUploader/ImageHost/Catbox.py
+-rw-r--r--   0        0        0     1515 2022-02-17 22:45:52.428144 PtpUploader-0.9.1/src/PtpUploader/ImageHost/ImageUploader.py
+-rw-r--r--   0        0        0     1147 2022-02-17 22:45:52.428144 PtpUploader-0.9.1/src/PtpUploader/ImageHost/ImgBB.py
+-rw-r--r--   0        0        0     1271 2022-02-17 22:45:52.412143 PtpUploader-0.9.1/src/PtpUploader/ImageHost/PtpImg.py
+-rw-r--r--   0        0        0      381 2022-02-17 22:45:26.631279 PtpUploader-0.9.1/src/PtpUploader/ImageHost/__init__.py
+-rw-r--r--   0        0        0     3780 2022-03-20 16:39:36.418942 PtpUploader-0.9.1/src/PtpUploader/IncludedFileList.py
+-rw-r--r--   0        0        0     1349 2021-11-13 03:18:45.463745 PtpUploader-0.9.1/src/PtpUploader/InformationSource/Imdb.py
+-rw-r--r--   0        0        0     1625 2021-10-23 18:02:25.708816 PtpUploader-0.9.1/src/PtpUploader/InformationSource/MoviePoster.py
+-rw-r--r--   0        0        0      144 2021-10-23 18:02:12.324403 PtpUploader-0.9.1/src/PtpUploader/InformationSource/__init__.py
+-rw-r--r--   0        0        0    19970 2022-01-21 14:19:00.310038 PtpUploader-0.9.1/src/PtpUploader/Job/CheckAnnouncement.py
+-rw-r--r--   0        0        0     1438 2021-11-02 02:35:37.787083 PtpUploader-0.9.1/src/PtpUploader/Job/Delete.py
+-rw-r--r--   0        0        0      173 2021-10-23 18:04:21.460395 PtpUploader-0.9.1/src/PtpUploader/Job/FinishedJobPhase.py
+-rw-r--r--   0        0        0     1456 2021-10-26 01:00:14.730265 PtpUploader-0.9.1/src/PtpUploader/Job/JobRunningState.py
+-rw-r--r--   0        0        0      492 2021-10-23 18:04:21.460395 PtpUploader-0.9.1/src/PtpUploader/Job/JobStartMode.py
+-rw-r--r--   0        0        0     1389 2021-11-13 17:23:51.379526 PtpUploader-0.9.1/src/PtpUploader/Job/LoadFile.py
+-rw-r--r--   0        0        0     7055 2022-05-20 15:45:28.921580 PtpUploader-0.9.1/src/PtpUploader/Job/Supervisor.py
+-rw-r--r--   0        0        0    22716 2022-03-20 16:39:36.418942 PtpUploader-0.9.1/src/PtpUploader/Job/Upload.py
+-rw-r--r--   0        0        0     2924 2022-01-21 21:03:36.392264 PtpUploader-0.9.1/src/PtpUploader/Job/WorkerBase.py
+-rw-r--r--   0        0        0      144 2021-10-23 18:04:21.460395 PtpUploader-0.9.1/src/PtpUploader/Job/__init__.py
+-rw-r--r--   0        0        0     2381 2022-02-17 22:45:26.743282 PtpUploader-0.9.1/src/PtpUploader/MyGlobals.py
+-rw-r--r--   0        0        0     1870 2021-11-02 02:35:38.003090 PtpUploader-0.9.1/src/PtpUploader/NfoParser.py
+-rw-r--r--   0        0        0       82 2020-01-12 18:29:37.664603 PtpUploader-0.9.1/src/PtpUploader/Notifier.example.ini
+-rw-r--r--   0        0        0     1285 2021-11-02 02:35:38.159095 PtpUploader-0.9.1/src/PtpUploader/Notifier.py
+-rw-r--r--   0        0        0    13480 2022-05-20 16:17:54.560155 PtpUploader-0.9.1/src/PtpUploader/Ptp.py
+-rw-r--r--   0        0        0     4512 2021-11-04 18:18:46.496345 PtpUploader-0.9.1/src/PtpUploader/PtpImdbInfo.py
+-rw-r--r--   0        0        0     6121 2022-02-21 23:54:13.779562 PtpUploader-0.9.1/src/PtpUploader/PtpMovieSearchResult.py
+-rw-r--r--   0        0        0     4814 2021-10-28 23:26:09.171292 PtpUploader-0.9.1/src/PtpUploader/PtpSubtitle.py
+-rw-r--r--   0        0        0      843 2021-10-29 04:32:53.333550 PtpUploader-0.9.1/src/PtpUploader/PtpUploaderException.py
+-rw-r--r--   0        0        0      735 2021-10-31 19:22:18.833307 PtpUploader-0.9.1/src/PtpUploader/PtpUploaderMessage.py
+-rw-r--r--   0        0        0     7689 2022-03-20 16:39:36.418942 PtpUploader-0.9.1/src/PtpUploader/ReleaseDescriptionFormatter.py
+-rw-r--r--   0        0        0     8575 2022-03-20 16:39:36.418942 PtpUploader-0.9.1/src/PtpUploader/ReleaseExtractor.py
+-rw-r--r--   0        0        0    12032 2022-03-20 16:39:36.418942 PtpUploader-0.9.1/src/PtpUploader/ReleaseInfo.py
+-rw-r--r--   0        0        0     6147 2022-03-20 16:44:05.828041 PtpUploader-0.9.1/src/PtpUploader/ReleaseInfoMaker.py
+-rw-r--r--   0        0        0     4508 2021-11-08 02:24:36.360394 PtpUploader-0.9.1/src/PtpUploader/ReleaseNameParser.py
+-rw-r--r--   0        0        0     1468 2020-01-12 18:29:37.668603 PtpUploader-0.9.1/src/PtpUploader/SceneGroups.txt
+-rw-r--r--   0        0        0     1013 2021-10-23 18:03:08.182130 PtpUploader-0.9.1/src/PtpUploader/ScreenshotList.py
+-rw-r--r--   0        0        0     8374 2022-02-17 22:43:55.172211 PtpUploader-0.9.1/src/PtpUploader/Settings.py
+-rw-r--r--   0        0        0     7218 2021-11-12 03:06:07.588031 PtpUploader-0.9.1/src/PtpUploader/Source/AlphaRatio.py
+-rw-r--r--   0        0        0    14130 2022-01-31 23:23:31.641517 PtpUploader-0.9.1/src/PtpUploader/Source/Cinemageddon.py
+-rw-r--r--   0        0        0    10741 2021-11-12 03:06:07.588031 PtpUploader-0.9.1/src/PtpUploader/Source/Cinematik.py
+-rw-r--r--   0        0        0     8636 2021-11-12 03:06:07.588031 PtpUploader-0.9.1/src/PtpUploader/Source/DigitalHive.py
+-rw-r--r--   0        0        0     6192 2022-02-22 23:50:00.957770 PtpUploader-0.9.1/src/PtpUploader/Source/File.py
+-rw-r--r--   0        0        0     7994 2021-11-12 03:06:07.588031 PtpUploader-0.9.1/src/PtpUploader/Source/FunFile.py
+-rw-r--r--   0        0        0     9834 2021-11-12 03:06:07.588031 PtpUploader-0.9.1/src/PtpUploader/Source/Gft.py
+-rw-r--r--   0        0        0     7083 2021-11-02 02:35:38.091093 PtpUploader-0.9.1/src/PtpUploader/Source/HDBits.py
+-rw-r--r--   0        0        0     7994 2021-11-12 03:06:07.588031 PtpUploader-0.9.1/src/PtpUploader/Source/HDTorrents.py
+-rw-r--r--   0        0        0    18003 2022-02-05 19:22:14.554949 PtpUploader-0.9.1/src/PtpUploader/Source/Karagarga.py
+-rw-r--r--   0        0        0     6201 2022-03-20 16:39:36.418942 PtpUploader-0.9.1/src/PtpUploader/Source/Prowlarr.py
+-rw-r--r--   0        0        0     8474 2022-03-20 16:39:36.418942 PtpUploader-0.9.1/src/PtpUploader/Source/SourceBase.py
+-rw-r--r--   0        0        0     2016 2021-11-12 00:18:15.943330 PtpUploader-0.9.1/src/PtpUploader/Source/SourceFactory.py
+-rw-r--r--   0        0        0     1233 2022-02-17 22:45:52.356141 PtpUploader-0.9.1/src/PtpUploader/Source/Torrent.py
+-rw-r--r--   0        0        0     7370 2021-11-12 03:06:07.592031 PtpUploader-0.9.1/src/PtpUploader/Source/TorrentBytes.py
+-rw-r--r--   0        0        0     8554 2021-11-12 03:06:07.592031 PtpUploader-0.9.1/src/PtpUploader/Source/TorrentLeech.py
+-rw-r--r--   0        0        0      144 2021-10-30 20:46:41.976266 PtpUploader-0.9.1/src/PtpUploader/Source/__init__.py
+-rw-r--r--   0        0        0     2175 2022-02-22 19:33:06.072298 PtpUploader-0.9.1/src/PtpUploader/Tool/BdInfo.py
+-rw-r--r--   0        0        0     4939 2022-02-17 23:06:33.925880 PtpUploader-0.9.1/src/PtpUploader/Tool/Ffmpeg.py
+-rw-r--r--   0        0        0     1767 2021-11-12 19:19:36.755586 PtpUploader-0.9.1/src/PtpUploader/Tool/ImageMagick.py
+-rw-r--r--   0        0        0     7903 2022-01-29 20:48:56.824203 PtpUploader-0.9.1/src/PtpUploader/Tool/MediaInfo.py
+-rw-r--r--   0        0        0     1295 2022-02-17 22:45:52.200136 PtpUploader-0.9.1/src/PtpUploader/Tool/Mktor.py
+-rw-r--r--   0        0        0     4007 2022-01-15 21:11:37.486169 PtpUploader-0.9.1/src/PtpUploader/Tool/Mplayer.py
+-rw-r--r--   0        0        0     1210 2022-01-15 21:11:20.917616 PtpUploader-0.9.1/src/PtpUploader/Tool/Mpv.py
+-rw-r--r--   0        0        0     5752 2022-02-17 22:45:27.235299 PtpUploader-0.9.1/src/PtpUploader/Tool/Rtorrent.py
+-rw-r--r--   0        0        0     5356 2022-02-22 22:07:09.133964 PtpUploader-0.9.1/src/PtpUploader/Tool/ScreenshotMaker.py
+-rw-r--r--   0        0        0     2509 2021-11-02 02:35:37.875086 PtpUploader-0.9.1/src/PtpUploader/Tool/Transmission.py
+-rw-r--r--   0        0        0     2464 2021-10-23 18:04:01.779787 PtpUploader-0.9.1/src/PtpUploader/Tool/Unrar.py
+-rw-r--r--   0        0        0      144 2022-01-29 22:34:24.955207 PtpUploader-0.9.1/src/PtpUploader/Tool/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-15 02:22:45.488257 PtpUploader-0.9.1/src/PtpUploader/__init__.py
+-rw-r--r--   0        0        0     4428 2022-03-20 16:39:36.422942 PtpUploader-0.9.1/src/PtpUploader/config.default.yml
+-rw-r--r--   0        0        0      406 2022-01-15 03:35:34.861384 PtpUploader-0.9.1/src/PtpUploader/manage.py
+-rw-r--r--   0        0        0        0 2021-10-27 20:19:43.046508 PtpUploader-0.9.1/src/PtpUploader/web/__init__.py
+-rw-r--r--   0        0        0     5839 2022-02-17 22:45:52.488146 PtpUploader-0.9.1/src/PtpUploader/web/forms.py
+-rw-r--r--   0        0        0        0 2021-10-29 21:49:40.692371 PtpUploader-0.9.1/src/PtpUploader/web/management/commands/__init__.py
+-rw-r--r--   0        0        0     9080 2022-05-20 15:45:12.929032 PtpUploader-0.9.1/src/PtpUploader/web/management/commands/runuploader.py
+-rw-r--r--   0        0        0     3991 2021-10-29 20:08:05.328481 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0001_initial.py
+-rw-r--r--   0        0        0      606 2021-10-29 20:08:05.328481 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0002_auto_20211025_0320.py
+-rw-r--r--   0        0        0      710 2021-10-29 20:08:05.328481 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0003_alter_releaseinfo_jobrunningstate.py
+-rw-r--r--   0        0        0     1547 2021-10-29 20:08:05.328481 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0004_auto_20211028_2254.py
+-rw-r--r--   0        0        0     1058 2021-10-29 04:35:34.782561 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0005_auto_20211029_0135.py
+-rw-r--r--   0        0        0      788 2021-10-29 20:24:02.365956 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0006_auto_20211029_2024.py
+-rw-r--r--   0        0        0      389 2021-10-29 20:24:29.450789 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0007_alter_releaseinfo_trumpable.py
+-rw-r--r--   0        0        0      410 2021-10-29 20:26:10.989915 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0008_alter_releaseinfo_subtitles.py
+-rw-r--r--   0        0        0      410 2021-10-29 21:00:32.157341 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0009_alter_releaseinfo_trumpable.py
+-rw-r--r--   0        0        0      410 2021-10-31 19:39:36.461201 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0010_alter_releaseinfo_screenshots.py
+-rw-r--r--   0        0        0      412 2021-10-31 19:40:02.722008 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0011_alter_releaseinfo_screenshots.py
+-rw-r--r--   0        0        0      414 2021-10-31 19:40:09.426214 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0012_alter_releaseinfo_screenshots.py
+-rw-r--r--   0        0        0      827 2021-11-04 03:44:33.946564 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0013_auto_20211104_0344.py
+-rw-r--r--   0        0        0      379 2022-01-08 21:47:45.866384 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0014_rename_scheduletimeutc_releaseinfo_scheduletime.py
+-rw-r--r--   0        0        0      534 2022-01-15 03:38:15.478735 PtpUploader-0.9.1/src/PtpUploader/web/migrations/0015_alter_releaseinfo_scheduletime.py
+-rw-r--r--   0        0        0        0 2021-10-23 23:05:43.143377 PtpUploader-0.9.1/src/PtpUploader/web/migrations/__init__.py
+-rw-r--r--   0        0        0      164 2021-10-31 19:22:19.909340 PtpUploader-0.9.1/src/PtpUploader/web/models.py
+-rw-r--r--   0        0        0     4464 2022-02-17 22:45:52.480146 PtpUploader-0.9.1/src/PtpUploader/web/settings.py
+-rw-r--r--   0        0        0      698 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/delete.png
+-rw-r--r--   0        0        0     3384 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/edit.png
+-rw-r--r--   0        0        0     1469 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/error.png
+-rw-r--r--   0        0        0      235 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/favicon.png
+-rw-r--r--   0        0        0      654 2021-10-24 18:34:54.468092 PtpUploader-0.9.1/src/PtpUploader/web/static/film.png
+-rw-r--r--   0        0        0      744 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/hourglass.png
+-rw-r--r--   0        0        0     6138 2021-10-25 12:19:33.173748 PtpUploader-0.9.1/src/PtpUploader/web/static/normalize.css
+-rw-r--r--   0        0        0      399 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/pause.png
+-rw-r--r--   0        0        0      894 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/ptp.ico
+-rw-r--r--   0        0        0      939 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/sad.png
+-rw-r--r--   0        0        0      839 2020-01-12 18:29:37.680603 PtpUploader-0.9.1/src/PtpUploader/web/static/scheduled.png
+-rw-r--r--   0        0        0   205319 2021-01-26 20:29:14.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/bulma.min.css
+-rw-r--r--   0        0        0     6199 2021-11-08 02:59:40.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/datatables.min.css
+-rw-r--r--   0        0        0    92883 2021-11-08 02:31:57.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/datatables.min.js
+-rw-r--r--   0        0        0  1196706 2021-09-13 19:10:03.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/fontawesome.all.min.js
+-rw-r--r--   0        0        0    89501 2021-03-02 17:27:20.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    22538 2020-05-04 16:11:45.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-confirm.min.css
+-rw-r--r--   0        0        0    27896 2020-05-04 16:11:45.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-confirm.min.js
+-rw-r--r--   0        0        0   253668 2021-08-20 17:47:54.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-ui.min.js
+-rw-r--r--   0        0        0     6007 2021-11-10 02:46:39.496020 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.contextMenu.min.css
+-rw-r--r--   0        0        0    27928 2020-05-13 14:12:49.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.contextMenu.min.js
+-rw-r--r--   0        0        0   130228 2021-11-10 02:48:34.287557 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.fancytree-all-deps.min.js
+-rw-r--r--   0        0        0     5855 2020-05-04 16:11:45.000000 PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.ui.position.min.js
+-rw-r--r--   0        0        0    16264 2021-10-24 05:37:24.049207 PtpUploader-0.9.1/src/PtpUploader/web/static/script/select2.min.css
+-rw-r--r--   0        0        0    73163 2021-10-24 05:36:50.596177 PtpUploader-0.9.1/src/PtpUploader/web/static/script/select2.min.js
+-rw-r--r--   0        0        0    17671 2021-11-10 02:48:34.147552 PtpUploader-0.9.1/src/PtpUploader/web/static/script/ui.fancytree.min.css
+-rw-r--r--   0        0        0     5510 2021-11-10 02:34:16.225124 PtpUploader-0.9.1/src/PtpUploader/web/static/skin-win8/icons.gif
+-rw-r--r--   0        0        0     3234 2021-11-10 02:50:05.178357 PtpUploader-0.9.1/src/PtpUploader/web/static/skin-win8/loading.gif
+-rw-r--r--   0        0        0     4286 2020-01-12 18:29:37.692603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/ar.ico
+-rw-r--r--   0        0        0      894 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/cg.ico
+-rw-r--r--   0        0        0     4286 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/dh.ico
+-rw-r--r--   0        0        0      815 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/file.ico
+-rw-r--r--   0        0        0     1086 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/gft.ico
+-rw-r--r--   0        0        0     5430 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/hdbits.ico
+-rw-r--r--   0        0        0     2862 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/kg.ico
+-rw-r--r--   0        0        0     1214 2021-10-31 15:28:16.457289 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/prowlarr.ico
+-rw-r--r--   0        0        0     3638 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/rtt.ico
+-rw-r--r--   0        0        0     4286 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tby.ico
+-rw-r--r--   0        0        0     1430 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tds.ico
+-rw-r--r--   0        0        0     1406 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tik.ico
+-rw-r--r--   0        0        0     3638 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tl.ico
+-rw-r--r--   0        0        0      924 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/torrent.ico
+-rw-r--r--   0        0        0      911 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/start.png
+-rw-r--r--   0        0        0      674 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/stop.png
+-rw-r--r--   0        0        0     2906 2022-02-16 19:03:49.052389 PtpUploader-0.9.1/src/PtpUploader/web/static/style.css
+-rw-r--r--   0        0        0     1530 2021-10-30 05:01:03.843218 PtpUploader-0.9.1/src/PtpUploader/web/static/style.css.old
+-rw-r--r--   0        0        0      682 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/success.png
+-rw-r--r--   0        0        0     1849 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/throbber.gif
+-rw-r--r--   0        0        0      851 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/static/warning.png
+-rw-r--r--   0        0        0     2463 2022-01-09 19:06:54.373383 PtpUploader-0.9.1/src/PtpUploader/web/templates/bulk.html
+-rw-r--r--   0        0        0    16535 2022-01-30 14:45:28.072896 PtpUploader-0.9.1/src/PtpUploader/web/templates/edit_job.html
+-rw-r--r--   0        0        0      104 2020-01-12 18:29:37.696603 PtpUploader-0.9.1/src/PtpUploader/web/templates/index.html
+-rw-r--r--   0        0        0     7474 2022-05-16 20:23:16.887674 PtpUploader-0.9.1/src/PtpUploader/web/templates/jobs.html
+-rw-r--r--   0        0        0     2101 2022-02-16 17:00:01.728913 PtpUploader-0.9.1/src/PtpUploader/web/templates/layout.html
+-rw-r--r--   0        0        0     1176 2021-10-24 06:13:08.295163 PtpUploader-0.9.1/src/PtpUploader/web/templates/movieAvailabilityCheck.html
+-rw-r--r--   0        0        0     2128 2022-02-17 22:17:15.122570 PtpUploader-0.9.1/src/PtpUploader/web/templates/settings.html
+-rw-r--r--   0        0        0     1161 2022-02-16 16:43:05.050965 PtpUploader-0.9.1/src/PtpUploader/web/urls.py
+-rw-r--r--   0        0        0    17330 2022-05-16 20:23:16.887674 PtpUploader-0.9.1/src/PtpUploader/web/views.py
+-rw-r--r--   0        0        0      393 2021-11-02 02:35:38.291099 PtpUploader-0.9.1/src/PtpUploader/web/wsgi.py
+-rw-r--r--   0        0        0     1541 2022-05-20 16:33:01.925907 PtpUploader-0.9.1/setup.py
+-rw-r--r--   0        0        0     1203 2022-05-20 16:33:01.927030 PtpUploader-0.9.1/PKG-INFO
```

### Comparing `PtpUploader-0.9.0/pyproject.toml` & `PtpUploader-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PtpUploader"
-version = "0.9.0"
+version = "0.9.1"
 description = "A small uploader for a mildly popular movie site"
 authors = ["kannibalox <kannibalox@gmail.com>"]
 packages = [
   { include = "PtpUploader", from = "src" }
 ]
 repository = "https://github.com/kannibalox/PtpUploader"
 classifiers = [
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Database.py` & `PtpUploader-0.9.1/src/PtpUploader/Database.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Helper.py` & `PtpUploader-0.9.1/src/PtpUploader/Helper.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ImageHost/Catbox.py` & `PtpUploader-0.9.1/src/PtpUploader/ImageHost/Catbox.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.ImageHost.Base import ImageSite
+from PtpUploader.PtpUploaderException import PtpUploaderException
 
 
 class CatboxMoe(ImageSite):
     def __init__(self, logger=None):
         self.name = "catbox"
         self.endpoint = "https://catbox.moe/user/api.php"
         super().__init__(logger)
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ImageHost/ImageUploader.py` & `PtpUploader-0.9.1/src/PtpUploader/ImageHost/ImageUploader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from PtpUploader.ImageHost.PtpImg import PtpImg
-from PtpUploader.ImageHost.ImgBB import ImgBB
 from PtpUploader.ImageHost.Catbox import CatboxMoe
+from PtpUploader.ImageHost.ImgBB import ImgBB
+from PtpUploader.ImageHost.PtpImg import PtpImg
 from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.Settings import config
 
 
 class ImageUploader:
     @staticmethod
     def Upload(logger, imagePath=None, imageUrl=None):
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ImageHost/ImgBB.py` & `PtpUploader-0.9.1/src/PtpUploader/ImageHost/ImgBB.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.ImageHost.Base import ImageSite
+from PtpUploader.PtpUploaderException import PtpUploaderException
 
 
 class ImgBB(ImageSite):
     def __init__(self, logger=None):
         self.name = "imgbb"
         super().__init__(logger)
         if not self.config.api_key:
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ImageHost/PtpImg.py` & `PtpUploader-0.9.1/src/PtpUploader/ImageHost/PtpImg.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.ImageHost.Base import ImageSite
+from PtpUploader.PtpUploaderException import PtpUploaderException
 
 
 class PtpImg(ImageSite):
     def __init__(self, logger=None):
         self.name = "ptpimg"
         self.endpoint = "https://ptpimg.me/upload.php"
         super().__init__(logger)
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/IncludedFileList.py` & `PtpUploader-0.9.1/src/PtpUploader/IncludedFileList.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/InformationSource/Imdb.py` & `PtpUploader-0.9.1/src/PtpUploader/InformationSource/Imdb.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/InformationSource/MoviePoster.py` & `PtpUploader-0.9.1/src/PtpUploader/InformationSource/MoviePoster.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Job/CheckAnnouncement.py` & `PtpUploader-0.9.1/src/PtpUploader/Job/CheckAnnouncement.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Job/Delete.py` & `PtpUploader-0.9.1/src/PtpUploader/Job/Delete.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Job/JobRunningState.py` & `PtpUploader-0.9.1/src/PtpUploader/Job/JobRunningState.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Job/LoadFile.py` & `PtpUploader-0.9.1/src/PtpUploader/Job/LoadFile.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Job/Supervisor.py` & `PtpUploader-0.9.1/src/PtpUploader/Job/Supervisor.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Job/Upload.py` & `PtpUploader-0.9.1/src/PtpUploader/Job/Upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 import logging
 import os
 import subprocess
 import threading
 
 from django.template import engines
 
-from PtpUploader import Ptp
+from PtpUploader import ImageHost, Ptp
 from PtpUploader.Helper import GetIdxSubtitleLanguages, TimeDifferenceToText
-from PtpUploader import ImageHost
 from PtpUploader.Job.FinishedJobPhase import FinishedJobPhase
 from PtpUploader.Job.JobRunningState import JobRunningState
-from PtpUploader.Job.WorkerBase import WorkerBase
 from PtpUploader.Job.JobStartMode import JobStartMode
+from PtpUploader.Job.WorkerBase import WorkerBase
 from PtpUploader.MyGlobals import MyGlobals
 from PtpUploader.PtpSubtitle import PtpSubtitleId
 from PtpUploader.PtpUploaderException import *
 from PtpUploader.ReleaseDescriptionFormatter import ReleaseDescriptionFormatter
 from PtpUploader.ReleaseInfo import ReleaseInfo
 from PtpUploader.Settings import Settings
 from PtpUploader.Tool import Mktor
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Job/WorkerBase.py` & `PtpUploader-0.9.1/src/PtpUploader/Job/WorkerBase.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/MyGlobals.py` & `PtpUploader-0.9.1/src/PtpUploader/MyGlobals.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,21 +32,22 @@
 
             self.session.mount("https://", CloudflareAdapter())
         except ImportError:
             pass
 
     def InitializeGlobals(self, workingPath):
         from PtpUploader.Settings import config
+
         self.InitializeLogger(workingPath)
         self.PtpSubtitle = PtpSubtitle()
         self.cookie_file: Path = Path(workingPath).joinpath("cookies.pickle")
         self.cookie_file: Path = Path(config.cookie_file).expanduser()
         if self.cookie_file.exists() and self.cookie_file.is_file():
             with self.cookie_file.open("rb") as fh:
-                    self.session.cookies = pickle.load(fh)
+                self.session.cookies = pickle.load(fh)
 
     def SaveCookies(self):
         with self.cookie_file.open("wb") as fh:
             pickle.dump(self.session.cookies, fh)
 
     # workingPath from Settings.WorkingPath.
     def InitializeLogger(self, workingPath):
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/NfoParser.py` & `PtpUploader-0.9.1/src/PtpUploader/NfoParser.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Notifier.py` & `PtpUploader-0.9.1/src/PtpUploader/Notifier.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Ptp.py` & `PtpUploader-0.9.1/src/PtpUploader/Ptp.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 import time
 import traceback
 
 from PtpUploader.MyGlobals import MyGlobals
 from PtpUploader.PtpMovieSearchResult import PtpMovieSearchResult
 from PtpUploader.PtpUploaderException import *
-from PtpUploader.Settings import Settings
+from PtpUploader.Settings import Settings, config
 
 
 def __LoginInternal():
     if not Settings.PtpUserName:
         raise PtpUploaderInvalidLoginException(
             "Couldn't log in to PTP. Your user name is not specified."
         )
@@ -28,32 +28,38 @@
     if passKey is None:
         raise PtpUploaderInvalidLoginException(
             "Couldn't log in to PTP. Pass key not found in the announce URL."
         )
     passKey = passKey.group(1)
 
     MyGlobals.Logger.info("Logging in to PTP.")
+    logged_in = False
+    try:
+        if "passthepopcorn.me" in MyGlobals.session.cookies.list_domains():
+            response = MyGlobals.session.get("https://passthepopcorn.me/upload.php")
+            CheckIfLoggedInFromResponse(response, response.text)
+            Settings.AntiCsrfToken = re.search(
+                r'data-AntiCsrfToken="(.*)"', response.text
+            ).group(1)
+            logged_in = True
+    except PtpUploaderException:
+        pass
 
-    if "passthepopcorn.me" in MyGlobals.session.cookies.list_domains():
-        response = MyGlobals.session.get("https://passthepopcorn.me/upload.php")
-        CheckIfLoggedInFromResponse(response, response.text)
-        Settings.AntiCsrfToken = re.search(
-            r'data-AntiCsrfToken="(.*)"', response.text
-        ).group(1)
-    else:
+    if not logged_in:
         postData = {
             "username": Settings.PtpUserName,
             "password": Settings.PtpPassword,
             "passkey": passKey,
             "keeplogged": "1",
         }
         response = MyGlobals.session.post(
             "https://passthepopcorn.me/ajax.php?action=login", data=postData
         ).text
 
+        print(response)
         jsonLoad = None
         try:
             jsonLoad = json.loads(response)
         except (Exception, ValueError) as e:
             raise PtpUploaderInvalidLoginException(
                 "Got exception while loading JSON login response from PTP. Response: '%s'."
                 % response
@@ -61,20 +67,34 @@
 
         if jsonLoad is None:
             raise PtpUploaderInvalidLoginException(
                 "Got bad JSON response from PTP while trying to log in. Response: '%s'."
                 % response
             )
 
-        if jsonLoad["Result"] != "Ok":
+        if jsonLoad["Result"] == "TfaRequired":
+            postData["TfaCode"] = input("Enter 2FA auth code:")
+            postData["TfaType"] = "normal"
+            response = MyGlobals.session.post(
+                "https://passthepopcorn.me/ajax.php?action=login", data=postData
+            ).text
+            jsonLoad = json.loads(response)
+            if jsonLoad["Result"] != "Ok":
+                raise PtpUploaderInvalidLoginException(
+                    "Failed to login to PTP. Probably due to a bad 2FA auth code. Response: '%s'."
+                    % jsonLoad
+                )
+            Settings.AntiCsrfToken = jsonLoad["AntiCsrfToken"]
+        elif jsonLoad["Result"] != "Ok":
             raise PtpUploaderInvalidLoginException(
-                "Failed to login to PTP. Probably due to the bad user name, password or pass key."
+                "Failed to login to PTP. Probably due to the bad user name, password or pass key. Response: '%s'."
+                % jsonLoad
             )
-
-        Settings.AntiCsrfToken = jsonLoad["Settings.AntiCsrfToken"]
+        else:
+            Settings.AntiCsrfToken = jsonLoad["Settings.AntiCsrfToken"]
         MyGlobals.SaveCookies()
 
 
 def Login():
     maximumTries = 1
 
     while True:
@@ -88,20 +108,20 @@
                 maximumTries -= 1
                 time.sleep(30)  # Wait 30 seconds and retry.
             else:
                 raise
 
 
 def __CheckIfLoggedInFromResponseLogResponse(result, responseBody: str):
-    MyGlobals.Logger.info("MSG: %s" % result.reason)
-    MyGlobals.Logger.info("CODE: %s" % result.status_code)
-    MyGlobals.Logger.info("URL: %s" % result.url)
-    MyGlobals.Logger.info("HEADERS: %s" % result.headers)
-    MyGlobals.Logger.info("STACK: %s" % traceback.format_stack())
-    MyGlobals.Logger.info("RESPONSE BODY: %s" % responseBody)
+    MyGlobals.Logger.debug("MSG: %s" % result.reason)
+    MyGlobals.Logger.debug("CODE: %s" % result.status_code)
+    MyGlobals.Logger.debug("URL: %s" % result.url)
+    MyGlobals.Logger.debug("HEADERS: %s" % result.headers)
+    MyGlobals.Logger.debug("STACK: %s" % traceback.format_stack())
+    MyGlobals.Logger.debug("RESPONSE BODY: %s" % responseBody)
 
 
 def CheckIfLoggedInFromResponse(result, responseBody: str):
     if responseBody.find("""<a href="login.php?act=recover">""") != -1:
         __CheckIfLoggedInFromResponseLogResponse(result, responseBody)
         raise PtpUploaderException(
             "Looks like you are not logged in to PTP. Probably due to the bad user name or password."
@@ -195,14 +215,17 @@
         "release_desc": releaseDescription,
         "nfo_text": releaseInfo.Nfo,
         "AntiCsrfToken": Settings.AntiCsrfToken,
         "subtitles[]": releaseInfo.GetSubtitles(),
         "trumpable[]": releaseInfo.Trumpable,
     }
 
+    if releaseInfo.Source == "Other":
+        paramList["other_source"]: releaseInfo.SourceOther
+
     # personal rip only needed if it is specified
     if releaseInfo.PersonalRip:
         paramList.update({"internalrip": "on"})
 
     # scene only needed if it is specified
     if releaseInfo.SceneRelease:
         paramList.update({"scene": "on"})
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/PtpImdbInfo.py` & `PtpUploader-0.9.1/src/PtpUploader/PtpImdbInfo.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/PtpMovieSearchResult.py` & `PtpUploader-0.9.1/src/PtpUploader/PtpMovieSearchResult.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,25 +138,25 @@
             # PTP wouldn't let us upload something with the same name anyway
             if t["ReleaseName"] == release.ReleaseName:
                 return t
             # Most likely not coincedence
             if t["Size"] == release.Size:
                 return t
 
-            # Find any really close duplicates
+            # Find any really close duplicates (within 3%)
             if t["Source"] == release.Source and t["Codec"] == release.Codec:
-                if abs((release.Size / t["Size"]) - 1) * 100 < 3:
+                if abs((release.Size / int(t["Size"])) - 1) * 100 < 3:
                     return t
 
             # Two slots are available, first check if we can coexist with any of them
             if (
                 release.ResolutionType in [Resolutions.Other, "480p"]
                 and t["Quality"] == "Standard Definition"
             ):
                 if (
-                    abs((release.Size / t["Size"]) - 1) * 100 < 40
+                    abs((release.Size / int(t["Size"])) - 1) * 100 < 40
                 ):  # 4.1.1.1 40% size difference to be able to coexist
                     return t
             if release.ResolutionType == "576p" and t["Resolution"] == "576p":
                 return t
 
         return None
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/PtpSubtitle.py` & `PtpUploader-0.9.1/src/PtpUploader/PtpSubtitle.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/PtpUploaderException.py` & `PtpUploader-0.9.1/src/PtpUploader/PtpUploaderException.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/PtpUploaderMessage.py` & `PtpUploader-0.9.1/src/PtpUploader/PtpUploaderMessage.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ReleaseDescriptionFormatter.py` & `PtpUploader-0.9.1/src/PtpUploader/ReleaseDescriptionFormatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from pathlib import Path
 
 from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.Settings import config
-from PtpUploader.Tool.MediaInfo import MediaInfo, MediaInfoException
 from PtpUploader.Tool import BdInfo
+from PtpUploader.Tool.MediaInfo import MediaInfo, MediaInfoException
 from PtpUploader.Tool.ScreenshotMaker import ScreenshotMaker
 
 
 logger = logging.getLogger(__name__)
 
 
 class ReleaseDescriptionVideoEntry:
@@ -202,20 +202,20 @@
         releaseDescription = ""
 
         if includeReleaseName:
             releaseDescription = (
                 "[size=4][b]%s[/b][/size]\n\n" % self.ReleaseInfo.ReleaseName
             )
 
+        if len(self.ReleaseInfo.ReleaseNotes) > 0:
+            releaseDescription += "%s\n\n" % self.ReleaseInfo.ReleaseNotes
+
         for i, entry in enumerate(self.VideoEntries):
             if i > 0:
                 releaseDescription += "\n\n"
 
             releaseDescription += entry.ToReleaseDescription()
 
-        if len(self.ReleaseInfo.ReleaseNotes) > 0:
-            releaseDescription += "\n\n%s" % self.ReleaseInfo.ReleaseNotes
-
         return releaseDescription
 
     def GetMainMediaInfo(self):
         return self.MainMediaInfo
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ReleaseExtractor.py` & `PtpUploader-0.9.1/src/PtpUploader/ReleaseExtractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import fnmatch
 import os
 
 from pathlib import Path
+
 from unidecode import unidecode
 
 from PtpUploader.MyGlobals import MyGlobals
 from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.Settings import Settings
 from PtpUploader.Tool.Unrar import Unrar
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ReleaseInfo.py` & `PtpUploader-0.9.1/src/PtpUploader/ReleaseInfo.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ReleaseInfoMaker.py` & `PtpUploader-0.9.1/src/PtpUploader/ReleaseInfoMaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import os
 import argparse
+import os
 
 import django
 
+
 os.environ.setdefault("DJANGO_SETTINGS_MODULE", "PtpUploader.web.settings")
 django.setup()
 
 from PtpUploader.IncludedFileList import IncludedFileList
 from PtpUploader.MyGlobals import MyGlobals
 from PtpUploader.PtpUploaderException import *
 from PtpUploader.ReleaseDescriptionFormatter import ReleaseDescriptionFormatter
@@ -70,15 +71,15 @@
                     raise PtpUploaderException(
                         "Codec is set to DVD5, yet release info says that this is not a DVD image."
                     )
 
                 return
 
     def MarkAsBlurayImageIfNeeded(self, releaseInfo):
-        if "BDMV" in os.listdir(self.Path):
+        if os.path.isdir(self.Path) and "BDMV" in os.listdir(self.Path):
             releaseInfo.Codec = "BD25"
 
     def SaveReleaseDescriptionFile(
         self, logger, releaseDescriptionFilePath, createScreens
     ):
         releaseInfo = ReleaseInfo()
         releaseInfo.Logger = logger
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ReleaseNameParser.py` & `PtpUploader-0.9.1/src/PtpUploader/ReleaseNameParser.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/SceneGroups.txt` & `PtpUploader-0.9.1/src/PtpUploader/SceneGroups.txt`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/ScreenshotList.py` & `PtpUploader-0.9.1/src/PtpUploader/ScreenshotList.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Settings.py` & `PtpUploader-0.9.1/src/PtpUploader/Settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 logger = logging.getLogger(__name__)
 config = Dynaconf(
     envvar_prefix=False,
     settings_files=[
         Path(Path(__file__).parent, "config.default.yml"),
         Path("~/.config/ptpuploader/config.yml").expanduser(),
-        ".secrets.yaml",
+        ".secrets.yml",
     ],
     environments=False,
     load_dotenv=True,
 )
 
 
 class Settings:
@@ -96,15 +96,17 @@
                 if groupName:
                     groups.append(groupName)
         return groups
 
     @staticmethod
     def LoadSettings():
         # TODO: These aren't actually required for ReleaseMaker, make it so
-        if not (config.ptp.announce_url and config.ptp.username and config.ptp.password):
+        if not (
+            config.ptp.announce_url and config.ptp.username and config.ptp.password
+        ):
             raise PtpUploaderException(
                 "Make sure the username, password and announce URL are set in the config!"
             )
         if not config.work_dir:
             raise PtpUploaderException(
                 "Make sure the work directory is set in the config!"
             )
@@ -112,15 +114,14 @@
         Settings.AdditionalExtensionsToUpload = config.uploader.additional_files
         Settings.TorrentClient = None
         Settings.IgnoreFile = config.uploader.ignore_files
         Settings.PtpAnnounceUrl = config.ptp.announce_url
         Settings.PtpUserName = config.ptp.username
         Settings.PtpPassword = config.ptp.password
 
-        Settings.ImageHost = config.image_host.use
         Settings.PtpImgApiKey = config.image_host.ptpimg.api_key
         Settings.OnSuccessfulUpload = config.hook.on_upload
 
         Settings.FfmpegPath = config.tools.ffmpeg.path
         Settings.MediaInfoPath = config.tools.mediainfo.path
         Settings.MplayerPath = config.tools.mplayer.path
         Settings.MpvPath = config.tools.mpv.path
@@ -173,27 +174,37 @@
 
         # Create required directories.
         Settings.GetAnnouncementInvalidPath().mkdir(parents=True, exist_ok=True)
         Settings.GetJobLogPath().mkdir(parents=True, exist_ok=True)
         Settings.GetTemporaryPath().mkdir(parents=True, exist_ok=True)
 
     @staticmethod
-    def GetTorrentClient():
-        if Settings.TorrentClient is None:
-            if Settings.TorrentClientName.lower() == "transmission":
-                from PtpUploader.Tool.Transmission import Transmission
+    def CreateClient():
+        use = config.client.use.lower()
+        # Hack to let env var take precedence
+        address = (
+            config["client"][config.client.use.upper()]["ADDRESS"]
+            or config["client"][config.client.use]["address"]
+        )
+        if use == "transmission":
+            from PtpUploader.Tool.Transmission import Transmission
 
-                Settings.TorrentClient = Transmission(
-                    Settings.TorrentClientAddress.split(":")[0],
-                    Settings.TorrentClientAddress.split(":")[1],
-                )
-            else:
-                from PtpUploader.Tool.Rtorrent import Rtorrent
+            Settings.TorrentClient = Transmission(
+                address.split(":")[0],
+                address.split(":")[1],
+            )
+        else:
+            from PtpUploader.Tool.Rtorrent import Rtorrent
+
+            Settings.TorrentClient = Rtorrent(address)
 
-                Settings.TorrentClient = Rtorrent(Settings.TorrentClientAddress)
+    @staticmethod
+    def GetTorrentClient():
+        if Settings.TorrentClient is None:
+            Settings.CreateClient()
         return Settings.TorrentClient
 
     @staticmethod
     def VerifyPaths():
         logger.info("Checking paths")
 
         if shutil.which(Settings.MediaInfoPath) is None:
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/AlphaRatio.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/AlphaRatio.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/Cinemageddon.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/Cinemageddon.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/Cinematik.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/Cinematik.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/DigitalHive.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/DigitalHive.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/File.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import os
 import shutil
 
+from unidecode import unidecode
+
 from PtpUploader.Helper import GetPathSize
 from PtpUploader.IncludedFileList import IncludedFileList
 from PtpUploader.NfoParser import NfoParser
 from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.ReleaseExtractor import ReleaseExtractor
 from PtpUploader.ReleaseNameParser import ReleaseNameParser
 from PtpUploader.Source.SourceBase import SourceBase
@@ -46,15 +48,15 @@
         return True
 
     def GetCustomUploadPath(self, logger, releaseInfo):
         path = releaseInfo.GetReleaseDownloadPath()
         if releaseInfo.SourceIsAFile():
             # In case of single files the parent directory of the file will be the upload directory.
             return os.path.split(path)[0]
-        return os.path.join(path, File.UploadDirectoryName, releaseInfo.ReleaseName)
+        return os.path.join(path, File.UploadDirectoryName, unidecode(releaseInfo.ReleaseName))
 
     def CreateUploadDirectory(self, releaseInfo):
         if not releaseInfo.SourceIsAFile():
             SourceBase.CreateUploadDirectory(self, releaseInfo)
 
     def ExtractRelease(self, logger, releaseInfo, includedFileList):
         if not releaseInfo.SourceIsAFile():
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/FunFile.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/FunFile.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/Gft.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/Gft.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/HDBits.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/HDBits.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/HDTorrents.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/HDTorrents.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/Karagarga.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/Karagarga.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,19 @@
             )
 
         untouched_fail = None
         if "video: untouched" not in ripSpecs.lower():
             untouched_fail = "modified video"
         if "audio: untouched" not in ripSpecs.lower():
             untouched_fail = "modified audio"
-        if "menus: " in ripSpecs.lower() and "menus: untouched" not in ripSpecs.lower():
+        if (
+            "menus: " in ripSpecs.lower()
+            and "menus: untouched" not in ripSpecs.lower()
+            and "menus: n/a" not in ripSpecs.lower()
+        ):
             untouched_fail = "modified menus"
         if (
             "dvd extras: " in ripSpecs.lower()
             and "dvd extras: n/a" not in ripSpecs.lower()
             and "dvd extras: none" not in ripSpecs.lower()
         ) and "dvd extras: untouched" not in ripSpecs.lower():
             untouched_fail = "modified dvd extras"
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/Prowlarr.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/Prowlarr.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/SourceBase.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/SourceBase.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/SourceFactory.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/SourceFactory.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/Torrent.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/Torrent.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import bencode
+
 from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.ReleaseNameParser import ReleaseNameParser
 from PtpUploader.Source.SourceBase import SourceBase
 
-import bencode
-
 
 class Torrent(SourceBase):
     def __init__(self):
         SourceBase.__init__(self)
 
         self.Name = "torrent"
         self.NameInSettings = "TorrentFileSource"
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/TorrentBytes.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/TorrentBytes.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Source/TorrentLeech.py` & `PtpUploader-0.9.1/src/PtpUploader/Source/TorrentLeech.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/BdInfo.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/BdInfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import subprocess
-import re
 import logging
+import re
 import shlex
-from typing import Optional, List
+import subprocess
+
 from pathlib import Path
 from tempfile import TemporaryDirectory
+from typing import List, Optional
 
-from PtpUploader.Settings import config
 from PtpUploader.PtpUploaderException import PtpUploaderException
+from PtpUploader.Settings import config
+
 
 logger = logging.getLogger(__name__)
 
 
 def bdinfo_cmd() -> List[str]:
     if config.tools.bdinfo.path:
         return [
@@ -44,15 +46,15 @@
     proc = subprocess.run(
         bdinfo_cmd() + [str(path), "-l"], check=True, capture_output=True
     )
     longest_mpls: Optional[str] = None
     longest_len: int = 0
     for line in proc.stdout.decode().split("\n"):
         if ".MPLS" in line:
-            length_str = line.split(" ")[14].split(":")
+            length_str = line[26:34].split(':')
             length_sec = sum(
                 [int(x[1]) * (60 ** (2 - x[0])) for x in enumerate(length_str)]
             )
             if length_sec > longest_len:
                 longest_len = length_sec
                 longest_mpls = line.split(" ")[9]
     if longest_mpls:
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/Ffmpeg.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/Ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import re
 import subprocess
+
 from pathlib import Path
 
 from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.Settings import Settings
 from PtpUploader.Tool.MediaInfo import MediaInfo
 
 
@@ -27,18 +28,18 @@
         # Stream #0.0[0x1e0]: Video: mpeg2video, yuv420p, 720x480 [PAR 8:9 DAR 4:3], 7500 kb/s, 29.97 tbr, 90k tbn, 59.94 tbc
         match = re.search(r"(\d+)x(\d+), [SP]AR \d+:\d+ DAR (\d+):(\d+)", result)
         if match is None:
             match = re.search(r"(\d+)x(\d+) \[[SP]AR \d+:\d+ DAR (\d+):(\d+)", result)
         if match is None:
             return
 
-        width = int(match.group(1))
-        height = int(match.group(2))
-        darX = int(match.group(3))
-        darY = int(match.group(4))
+        width: int = int(match.group(1))
+        height: int = int(match.group(2))
+        darX: int = int(match.group(3))
+        darY: int = int(match.group(4))
         # We ignore invalid resolutions, invalid aspect ratios and aspect ratio 1:1.
         if (
             width <= 0
             or height <= 0
             or darX <= 0
             or darY <= 0
             or (darX == 1 and darY == 1)
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/ImageMagick.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/ImageMagick.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/MediaInfo.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/MediaInfo.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/Mktor.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/Mktor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
 import bencode
+
 from pyrosimple.util import metafile
 
 from PtpUploader.Settings import Settings
 
 
 def Make(logger, path, torrentPath):
     def callback(meta):
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/Mplayer.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/Mplayer.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/Mpv.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/Mpv.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/Rtorrent.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/Rtorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         try:
             # TODO: not the most sophisticated way.
             # Even a watch dir with Pyinotify would be better probably. rTorrent could write the info hash to a directory watched by us.
             completed = self.proxy.d.complete(infoHash)
             return completed == 1
         except xmlrpc.HashNotFound as e:
-            raise e # Raise this up to the web UI
+            raise e  # Raise this up to the web UI
         except Exception as e:
             logger.exception(
                 "Got exception while trying to check torrent's completion status. hash: '%s', error: '%s'",
                 infoHash,
                 e,
             )
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/ScreenshotMaker.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/ScreenshotMaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from PtpUploader.PtpUploaderException import PtpUploaderException
 from PtpUploader.Settings import Settings, config
 from PtpUploader.Tool.Ffmpeg import Ffmpeg
 from PtpUploader.Tool.ImageMagick import ImageMagick
 from PtpUploader.Tool.Mplayer import Mplayer
 from PtpUploader.Tool.Mpv import Mpv
 
+
 # Blatantly stolen from https://stackoverflow.com/a/57701186
 @contextlib.contextmanager
 def temporary_filename(suffix=None):
     """Context that introduces a temporary file.
 
     Creates a temporary file, yields its name, and upon context exit, deletes it.
     (In contrast, tempfile.NamedTemporaryFile() provides a 'file' object and
@@ -97,15 +98,15 @@
             )
 
         return urls
 
     # We sort video files by their size (less than 50 MB difference is ignored) and by their name.
     # Sorting by name is needed to ensure that the screenshot is taken from the first video to avoid spoilers when a release contains multiple videos.
     # Sorting by size is needed to ensure that we don't take the screenshots from the sample or extras included.
-    # Ignoring less than 50 MB differnece is needed to make sure that CD1 will be sorted before CD2 even if CD2 is larger than CD1 by 49 MB.
+    # Ignoring less than 50 MB difference is needed to make sure that CD1 will be sorted before CD2 even if CD2 is larger than CD1 by 49 MB.
     @staticmethod
     def SortVideoFiles(files):
         class SortItem:
             def __init__(self, path):
                 self.Path = path
                 self.LowerPath = str(path).lower()
                 self.Size = os.path.getsize(path)
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/Transmission.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/Transmission.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/Tool/Unrar.py` & `PtpUploader-0.9.1/src/PtpUploader/Tool/Unrar.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/config.default.yml` & `PtpUploader-0.9.1/src/PtpUploader/config.default.yml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     key:
     cert:
 # Settings for the upload forms and workers
 uploader:
   # Files that are explicitly video
   video_files: [avi, divx, mkv, mp4, vob, m2ts]
   # Additional files wanted but not technically videos
-  additional_files: [bup, idx, ifo, srt, sub, bdmc, mpls, clpi]
+  additional_files: [bup, idx, ifo, srt, sub, bdmv, mpls, clpi]
   ignore_files: ['.*sample.*', '.*d-z0n3\.assistant\.rar']
   # Controls the default settings for checkboxes on the upload form. Able to be overridden on a per-job basis.
   override_screenshots: false
   force_directoryless_single_file: false
   is_personal: false
   skip_duplicate_checking: false
   release_notes: ''
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/forms.py` & `PtpUploader-0.9.1/src/PtpUploader/web/forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,28 +4,64 @@
     ChoiceField,
     ClearableFileInput,
     FileField,
     Form,
     HiddenInput,
     ModelForm,
     MultipleChoiceField,
+    PasswordInput,
     Textarea,
     TextInput,
 )
 
+from PtpUploader import ImageHost
 from PtpUploader.Job.JobStartMode import JobStartMode
 from PtpUploader.PtpSubtitle import PtpSubtitleId
 from PtpUploader.ReleaseInfo import ReleaseInfo
+from PtpUploader.Settings import config
+
+
+class SettingsForm(Form):
+    image_host_use = ChoiceField(
+        choices=[(x, x) for x in ImageHost.list_hosts()],
+        initial=config.image_host.use,
+        label="Host",
+    )
+    ptp_username = CharField(initial=config.ptp.username, label="Username")
+    ptp_password = CharField(
+        initial=config.ptp.password,
+        label="Password",
+        widget=TextInput(attrs={"type": "password"}),
+    )
+    ptp_announce_url = CharField(initial=config.ptp.announce_url, label="Announce URL")
+    client_use = ChoiceField(
+        choices=[(x, x) for x in ["rtorrent", "transmission"]],
+        initial=config.client.use,
+        label="Use",
+    )
+    client_address = CharField(
+        initial=config.client[config.client.use].address,
+        label="Address",
+        help_text="Automatically determined if not set",
+        required=False,
+    )
 
 
 class BulkReleaseForm(Form):
     Links = CharField(widget=Textarea(attrs={"placeholder": "Links"}), required=False)
     Paths = CharField(widget=Textarea(attrs={"placeholder": "Paths"}), required=False)
     Files = FileField(
-        widget=ClearableFileInput(attrs={"class": "file-input"}), required=False
+        widget=ClearableFileInput(
+            attrs={
+                "class": "file-input",
+                "multiple": "multiple",
+                "accept": "application/x-bittorrent",
+            }
+        ),
+        required=False,
     )
 
 
 class ReleaseForm(ModelForm):
     Type = ChoiceField(choices=ReleaseInfo.TypeChoices.choices, required=False)
     Codec = ChoiceField(choices=ReleaseInfo.CodecChoices.choices, required=False)
     Container = ChoiceField(
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/management/commands/runuploader.py` & `PtpUploader-0.9.1/src/PtpUploader/web/management/commands/runuploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import errno
 import os
 import re
 import socket
 import sys
-from pathlib import Path
 
 from datetime import datetime
+from pathlib import Path
 
 from django.conf import settings
 from django.contrib.staticfiles.handlers import StaticFilesHandler
 from django.core.management.base import BaseCommand, CommandError
 from django.core.servers.basehttp import WSGIServer, get_internal_wsgi_application
 from django.utils import autoreload
 from django.utils.regex_helper import _lazy_re_compile
-
 from werkzeug import run_simple
-from werkzeug.serving import make_ssl_devcert
-from werkzeug.serving import WSGIRequestHandler
+from werkzeug.serving import WSGIRequestHandler, make_ssl_devcert
 
+from PtpUploader import Ptp
 from PtpUploader.Job import Supervisor
 from PtpUploader.MyGlobals import MyGlobals
 from PtpUploader.Settings import Settings, config
 
 
 naiveip_re = _lazy_re_compile(
     r"""^(?:
@@ -107,15 +106,15 @@
 
         Settings.LoadSettings()
 
         call_command("migrate")
 
         MyGlobals.InitializeGlobals(Settings.WorkingPath)
         MyGlobals.SourceFactory = SourceFactory()
-        MyGlobals.Logger.info("Initializing database.")
+        MyGlobals.Logger.info("Initializing database...")
 
         # Reset any possibling interrupted jobs
         for releaseInfo in ReleaseInfo.objects.filter(
             JobRunningState__in=[
                 JobRunningState.WaitingForStart,
                 JobRunningState.InProgress,
             ]
@@ -164,14 +163,15 @@
     def run(self, **options):
         """Run the server, using the autoreloader if needed."""
         use_reloader = options["use_reloader"]
 
         if use_reloader:
             autoreload.run_with_reloader(self.inner_run, **options)
         else:
+            Ptp.Login()
             MyGlobals.PtpUploader = Supervisor.JobSupervisor()
             MyGlobals.PtpUploader.start()
             self.inner_run(None, **options)
 
     def ssl_context(self):
         if config.web.ssl.enabled:
             if config.web.ssl.cert and config.web.ssl.key:
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0001_initial.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0002_auto_20211025_0320.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0002_auto_20211025_0320.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0003_alter_releaseinfo_jobrunningstate.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0003_alter_releaseinfo_jobrunningstate.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0004_auto_20211028_2254.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0004_auto_20211028_2254.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0005_auto_20211029_0135.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0005_auto_20211029_0135.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0006_auto_20211029_2024.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0006_auto_20211029_2024.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0013_auto_20211104_0344.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0013_auto_20211104_0344.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/migrations/0015_alter_releaseinfo_scheduletime.py` & `PtpUploader-0.9.1/src/PtpUploader/web/migrations/0015_alter_releaseinfo_scheduletime.py`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/settings.py` & `PtpUploader-0.9.1/src/PtpUploader/web/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 https://docs.djangoproject.com/en/3.2/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/3.2/ref/settings/
 """
 
 import os
+
 from pathlib import Path
 
 import dynaconf
 
 from PtpUploader.Settings import Settings
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/delete.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/delete.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/edit.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/edit.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/error.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/error.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/film.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/film.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/hourglass.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/hourglass.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/normalize.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/normalize.css`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/ptp.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/ptp.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/sad.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/sad.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/scheduled.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/scheduled.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/bulma.min.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/bulma.min.css`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/datatables.min.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/datatables.min.css`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/datatables.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/datatables.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/fontawesome.all.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/fontawesome.all.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-3.6.0.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-confirm.min.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-confirm.min.css`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-confirm.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-confirm.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery-ui.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.contextMenu.min.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.contextMenu.min.css`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.contextMenu.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.contextMenu.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.fancytree-all-deps.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.fancytree-all-deps.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/jquery.ui.position.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/jquery.ui.position.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/select2.min.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/select2.min.css`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/select2.min.js` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/select2.min.js`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/script/ui.fancytree.min.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/script/ui.fancytree.min.css`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/skin-win8/icons.gif` & `PtpUploader-0.9.1/src/PtpUploader/web/static/skin-win8/icons.gif`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/skin-win8/loading.gif` & `PtpUploader-0.9.1/src/PtpUploader/web/static/skin-win8/loading.gif`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/ar.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/ar.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/cg.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/cg.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/dh.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/dh.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/file.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/file.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/gft.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/gft.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/hdbits.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/hdbits.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/kg.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/kg.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/prowlarr.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/prowlarr.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/rtt.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/rtt.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tby.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tby.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tds.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tds.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tik.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tik.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/tl.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/tl.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/source_icon/torrent.ico` & `PtpUploader-0.9.1/src/PtpUploader/web/static/source_icon/torrent.ico`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/start.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/start.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/stop.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/stop.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/style.css` & `PtpUploader-0.9.1/src/PtpUploader/web/static/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 }
 
 #editjob_table td.label
 {
     text-align: right;
 }
 
-input[type="text"], input[type="search"], textarea, button, select, textarea, span.select2, span.select2-selection--multiple.select2-selection {
+input[type="text"], input[type="password"], input[type="search"], textarea, button, select, textarea, span.select2, span.select2-selection--multiple.select2-selection {
     background-color : #363636;
     border: thin solid #30373d;
     border-radius: 3px;
     color: white;
 }
 
 span.select2-selection__choice__display, span.select2-dropdown, #uploader li.select2-selection__choice {
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/style.css.old` & `PtpUploader-0.9.1/src/PtpUploader/web/static/style.css.old`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/success.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/success.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/throbber.gif` & `PtpUploader-0.9.1/src/PtpUploader/web/static/throbber.gif`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/static/warning.png` & `PtpUploader-0.9.1/src/PtpUploader/web/static/warning.png`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/templates/bulk.html` & `PtpUploader-0.9.1/src/PtpUploader/web/templates/bulk.html`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/templates/edit_job.html` & `PtpUploader-0.9.1/src/PtpUploader/web/templates/edit_job.html`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/templates/jobs.html` & `PtpUploader-0.9.1/src/PtpUploader/web/templates/jobs.html`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/templates/layout.html` & `PtpUploader-0.9.1/src/PtpUploader/web/templates/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             <div class="navbar-item has-dropdown is-hoverable">
 	      <a class="navbar-link" href="{% url "upload" %}">Upload</a>
               <div class="navbar-dropdown">
 	        <a class="navbar-item" href="{% url "bulk_upload" %}">Bulk</a>
                 <a class="navbar-item" href="{% url "upload" %}">Single</a>
               </div>
             </div>
+	    <a class="navbar-item" href="{% url "settings" %}">Settings</a>
           </div>
         </div>
       </nav>
       <nav>
 	<ul>
 	</ul>
       </nav>
```

#### html2text {}

```diff
@@ -11,10 +11,11 @@
 PP
 
  %}">Jobs
  %}">Upload
  %}">Bulk
 
  %}">Single
+ %}">Settings
 
 
 {% block body %} {% endblock %}
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/templates/movieAvailabilityCheck.html` & `PtpUploader-0.9.1/src/PtpUploader/web/templates/movieAvailabilityCheck.html`

 * *Files identical despite different names*

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/urls.py` & `PtpUploader-0.9.1/src/PtpUploader/web/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     path("", lambda r: redirect("/jobs"), name="index"),
     path("jobs", views.jobs, name="jobs"),
     path("ajax/jobs", views.jobs_json, name="jobs_json"),
     path("ajax/localdir", views.local_dir, name="local_dir"),
     path("ajax/getlatest", views.jobs_get_latest, name="jobs_get_latest"),
     path("ajax/create", views.create, name="ajax_create"),
     path("upload", views.edit_job, name="upload"),
+    path("settings", views.settings, name="settings"),
     path("upload/bulk", views.bulk_upload, name="bulk_upload"),
     path("movieAvailabilityCheck", views.jobs, name="movieAvailabilityCheck"),
     path("quit", views.jobs, name="quit"),
     path("job/<int:r_id>/log", views.log, name="log"),
     path("job/<int:r_id>/stop", views.stop_job, name="stop_job"),
     path("job/<int:r_id>/start", views.start_job, name="start_job"),
     path("job/<int:r_id>/edit", views.edit_job, name="edit_job"),
```

### Comparing `PtpUploader-0.9.0/src/PtpUploader/web/views.py` & `PtpUploader-0.9.1/src/PtpUploader/web/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 import os
-import urllib
 import time
+import urllib
 
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict
 
+import dynaconf
+
 from django.contrib.auth.decorators import login_required
+from django.core.exceptions import PermissionDenied
 from django.http import HttpResponse, HttpResponseRedirect, JsonResponse
 from django.shortcuts import get_object_or_404, render
 from django.templatetags.static import static
 from django.urls import reverse
 from django.utils import timezone
-from django.core.exceptions import PermissionDenied
 from django.views.decorators.csrf import csrf_exempt
 
 from PtpUploader import Ptp
 from PtpUploader.Helper import SizeToText, TimeDifferenceToText
 from PtpUploader.Job.JobRunningState import JobRunningState
 from PtpUploader.Job.JobStartMode import JobStartMode
 from PtpUploader.MyGlobals import MyGlobals
@@ -131,14 +133,45 @@
             "TorrentId": torrentId,
             "UploadedAgo": TimeDifferenceToText(difference).lower(),
         }
     )
 
 
 @login_required
+def settings(request):
+    if request.method == "POST":
+        form = forms.SettingsForm(request.POST)
+        if form.is_valid():
+            config.image_host.use = form.cleaned_data["image_host_use"]
+            config.ptp.username = form.cleaned_data["ptp_username"]
+            config.ptp.password = form.cleaned_data["ptp_password"]
+            config.ptp.announce_url = form.cleaned_data["ptp_announce_url"]
+            dynaconf.loaders.yaml_loader.write(
+                Path("~/.config/ptpuploader/config.yml").expanduser(),
+                {
+                    "ptp": {
+                        "username": form.cleaned_data["ptp_username"],
+                        "password": form.cleaned_data["ptp_password"],
+                        "announce_url": form.cleaned_data["ptp_announce_url"],
+                    },
+                    "client": {
+                        "use": form.cleaned_data["client_use"],
+                        form.cleaned_data["client_use"]: {
+                            "address": form.cleaned_data["client_address"]
+                        },
+                    },
+                    "image_host": {"use": form.cleaned_data["image_host_use"]},
+                },
+            )
+    else:
+        form = forms.SettingsForm()
+    return render(request, "settings.html", {"form": form})
+
+
+@login_required
 def bulk_upload(request):
     if request.method == "POST":
         # create a form instance and populate it with data from the request:
         form = forms.BulkReleaseForm(request.POST)
         # check whether it's valid:
         if form.is_valid():
             for link in form.cleaned_data["Links"].split("\n"):
@@ -324,14 +357,16 @@
     release.ImdbId = request.POST["imdbUrl"]
     source, source_id = MyGlobals.SourceFactory.GetSourceAndIdByUrl(
         request.POST["SourceUrl"]
     )
     if source is not None:
         release.AnnouncementSourceName = source.Name
         release.AnnouncementId = source_id
+    release.JobStartMode = JobStartMode.Manual
+    release.StopBeforeUploading = True
     release.save()
     response = JsonResponse({"result": "OK", "jobId": release.Id})
     response["Access-Control-Allow-Origin"] = "*"
     return response
 
 
 @login_required
```

### Comparing `PtpUploader-0.9.0/setup.py` & `PtpUploader-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 entry_points = \
 {'console_scripts': ['PtpUploader = PtpUploader.manage:run',
                      'ReleaseInfoMaker = PtpUploader.ReleaseInfoMaker:run']}
 
 setup_kwargs = {
     'name': 'ptpuploader',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'A small uploader for a mildly popular movie site',
     'long_description': None,
     'author': 'kannibalox',
     'author_email': 'kannibalox@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kannibalox/PtpUploader',
```

### Comparing `PtpUploader-0.9.0/PKG-INFO` & `PtpUploader-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptpuploader
-Version: 0.9.0
+Version: 0.9.1
 Summary: A small uploader for a mildly popular movie site
 Home-page: https://github.com/kannibalox/PtpUploader
 Author: kannibalox
 Author-email: kannibalox@gmail.com
 Requires-Python: >3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

