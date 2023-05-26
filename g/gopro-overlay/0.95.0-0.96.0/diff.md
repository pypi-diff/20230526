# Comparing `tmp/gopro-overlay-0.95.0.tar.gz` & `tmp/gopro-overlay-0.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopro-overlay-0.95.0.tar", last modified: Tue May 23 11:06:31 2023, max compression
+gzip compressed data, was "gopro-overlay-0.96.0.tar", last modified: Fri May 26 15:11:51 2023, max compression
```

## Comparing `gopro-overlay-0.95.0.tar` & `gopro-overlay-0.96.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/
--rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.95.0/LICENSE.md
--rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.95.0/MANIFEST.in
--rw-rw-r--   0 richja    (1000) richja    (1000)    11380 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)    10587 2023-05-23 11:05:26.000000 gopro-overlay-0.95.0/README.md
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.377513 gopro-overlay-0.95.0/bin/
--rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.95.0/bin/gopro-contrib-data-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.95.0/bin/gopro-cut.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    15036 2023-05-22 09:35:24.000000 gopro-overlay-0.95.0/bin/gopro-dashboard.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-debug.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.95.0/bin/gopro-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-join.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)     5527 2023-05-06 09:06:40.000000 gopro-overlay-0.95.0/bin/gopro-layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3702 2023-05-23 10:54:25.000000 gopro-overlay-0.95.0/bin/gopro-rename.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-to-csv.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/bin/gopro-to-gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.385513 gopro-overlay-0.95.0/gopro_overlay/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.95.0/gopro_overlay/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-23 11:04:16.000000 gopro-overlay-0.95.0/gopro_overlay/__version__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     7063 2023-05-22 08:55:54.000000 gopro-overlay-0.95.0/gopro_overlay/arguments.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.95.0/gopro_overlay/buffering.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.95.0/gopro_overlay/common.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/counter.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/date_overlap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.95.0/gopro_overlay/dimensions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/entry.py
--rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.95.0/gopro_overlay/exceptions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.95.0/gopro_overlay/execution.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/fake.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.95.0/gopro_overlay/ffmpeg.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1285 2023-05-22 09:02:15.000000 gopro-overlay-0.95.0/gopro_overlay/ffmpeg_profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1803 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/filenaming.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.95.0/gopro_overlay/fit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.95.0/gopro_overlay/font.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/framemeta.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/framemeta_gpx.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.95.0/gopro_overlay/functional.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.95.0/gopro_overlay/geo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.95.0/gopro_overlay/geo_render.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-05-23 10:54:25.000000 gopro-overlay-0.95.0/gopro_overlay/geocode.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_calculate.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_cori.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_debug.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_grav.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_xyz.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.389513 gopro-overlay-0.95.0/gopro_overlay/icons/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.95.0/gopro_overlay/icons/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.95.0/gopro_overlay/icons/bicycle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.95.0/gopro_overlay/icons/car.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/faq.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/forbidden.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gauge-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gauge.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_2d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_3d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_none.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_unknown.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.95.0/gopro_overlay/icons/heartbeat.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.95.0/gopro_overlay/icons/ice-cream-van.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.95.0/gopro_overlay/icons/mountain-range.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.95.0/gopro_overlay/icons/mountain.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.95.0/gopro_overlay/icons/power.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.95.0/gopro_overlay/icons/ruler.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.95.0/gopro_overlay/icons/slope-triangle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.95.0/gopro_overlay/icons/slope.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.95.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.95.0/gopro_overlay/icons/thermometer-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.95.0/gopro_overlay/icons/thermometer.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.95.0/gopro_overlay/icons/user.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.95.0/gopro_overlay/icons/van-black-side-view.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/journey.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.95.0/gopro_overlay/layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_components.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_xml.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_xml_attribute.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layout_xml_cairo.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.389513 gopro-overlay-0.95.0/gopro_overlay/layouts/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/default-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/default-2704x1520.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/default-3840x2160.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/example-2.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/example.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/layouts/power-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/log.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.95.0/gopro_overlay/models.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.95.0/gopro_overlay/parsing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/point.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.95.0/gopro_overlay/privacy.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.95.0/gopro_overlay/progress_frames.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/rdp.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/smoothing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/timeseries.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/timeseries_process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.95.0/gopro_overlay/timeunits.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/timing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.95.0/gopro_overlay/units.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.389513 gopro-overlay-0.95.0/gopro_overlay/widgets/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/asi.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/bar.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/angle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/annotation.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/background.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/bordered.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/box.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cairo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/circuit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/colour.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/ellipse.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/face.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_marker.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_round_254.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/line.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/needle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/reading.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/scale.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/tick.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/chart.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/compass.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/compass_arrow.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/gradient_bar.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/info.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/map.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/text.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/widgets.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.95.0/gopro_overlay/widgets/widgets_experimental.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-23 11:06:31.385513 gopro-overlay-0.95.0/gopro_overlay.egg-info/
--rw-rw-r--   0 richja    (1000) richja    (1000)    11380 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)     4192 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/SOURCES.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/dependency_links.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/requires.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-23 11:06:31.000000 gopro-overlay-0.95.0/gopro_overlay.egg-info/top_level.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-23 11:06:31.393513 gopro-overlay-0.95.0/setup.cfg
--rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-23 11:04:16.000000 gopro-overlay-0.95.0/setup.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    35691 2023-05-22 13:30:42.000000 gopro-overlay-0.96.0/LICENSE.md
+-rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.96.0/MANIFEST.in
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11681 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10888 2023-05-26 15:11:29.000000 gopro-overlay-0.96.0/README.md
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.942449 gopro-overlay-0.96.0/bin/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.96.0/bin/gopro-contrib-data-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.96.0/bin/gopro-cut.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15036 2023-05-22 09:35:24.000000 gopro-overlay-0.96.0/bin/gopro-dashboard.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-debug.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.96.0/bin/gopro-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-join.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)     5527 2023-05-06 09:06:40.000000 gopro-overlay-0.96.0/bin/gopro-layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3702 2023-05-23 10:54:25.000000 gopro-overlay-0.96.0/bin/gopro-rename.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-to-csv.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/bin/gopro-to-gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.950449 gopro-overlay-0.96.0/gopro_overlay/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.96.0/gopro_overlay/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-26 15:09:52.000000 gopro-overlay-0.96.0/gopro_overlay/__version__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7063 2023-05-22 08:55:54.000000 gopro-overlay-0.96.0/gopro_overlay/arguments.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.96.0/gopro_overlay/buffering.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.96.0/gopro_overlay/common.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/counter.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/date_overlap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.96.0/gopro_overlay/dimensions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/entry.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.96.0/gopro_overlay/exceptions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.96.0/gopro_overlay/execution.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/fake.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10025 2023-05-22 09:32:45.000000 gopro-overlay-0.96.0/gopro_overlay/ffmpeg.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1285 2023-05-22 09:02:15.000000 gopro-overlay-0.96.0/gopro_overlay/ffmpeg_profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1958 2023-05-26 14:53:43.000000 gopro-overlay-0.96.0/gopro_overlay/filenaming.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.96.0/gopro_overlay/fit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.96.0/gopro_overlay/font.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/framemeta.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/framemeta_gpx.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.96.0/gopro_overlay/functional.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.96.0/gopro_overlay/geo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.96.0/gopro_overlay/geo_render.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-05-23 10:54:25.000000 gopro-overlay-0.96.0/gopro_overlay/geocode.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_calculate.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_cori.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_debug.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_grav.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_xyz.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.950449 gopro-overlay-0.96.0/gopro_overlay/icons/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.96.0/gopro_overlay/icons/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.96.0/gopro_overlay/icons/bicycle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.96.0/gopro_overlay/icons/car.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/faq.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/forbidden.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gauge-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gauge.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_2d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_3d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_none.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_unknown.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.96.0/gopro_overlay/icons/heartbeat.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.96.0/gopro_overlay/icons/ice-cream-van.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.96.0/gopro_overlay/icons/mountain-range.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.96.0/gopro_overlay/icons/mountain.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.96.0/gopro_overlay/icons/power.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.96.0/gopro_overlay/icons/ruler.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.96.0/gopro_overlay/icons/slope-triangle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.96.0/gopro_overlay/icons/slope.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.96.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.96.0/gopro_overlay/icons/thermometer-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.96.0/gopro_overlay/icons/thermometer.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.96.0/gopro_overlay/icons/user.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.96.0/gopro_overlay/icons/van-black-side-view.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/journey.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.96.0/gopro_overlay/layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_components.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_xml.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_xml_attribute.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layout_xml_cairo.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/gopro_overlay/layouts/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/default-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/default-2704x1520.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/default-3840x2160.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/example-2.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/example.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/layouts/power-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/log.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.96.0/gopro_overlay/models.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.96.0/gopro_overlay/parsing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/point.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.96.0/gopro_overlay/privacy.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.96.0/gopro_overlay/progress_frames.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/rdp.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/smoothing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/timeseries.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/timeseries_process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.96.0/gopro_overlay/timeunits.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/timing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.96.0/gopro_overlay/units.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/gopro_overlay/widgets/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/asi.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/bar.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/angle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/annotation.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/background.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/bordered.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/box.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cairo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/circuit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/colour.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/ellipse.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/face.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_marker.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_round_254.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/line.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/needle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/reading.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/scale.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/tick.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/chart.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/compass.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/compass_arrow.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/gradient_bar.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/info.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/map.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/text.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/widgets.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.96.0/gopro_overlay/widgets/widgets_experimental.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-26 15:11:51.950449 gopro-overlay-0.96.0/gopro_overlay.egg-info/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11681 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4192 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/SOURCES.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/dependency_links.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/requires.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-26 15:11:51.000000 gopro-overlay-0.96.0/gopro_overlay.egg-info/top_level.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-26 15:11:51.954449 gopro-overlay-0.96.0/setup.cfg
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-26 15:09:52.000000 gopro-overlay-0.96.0/setup.py
```

### Comparing `gopro-overlay-0.95.0/LICENSE.md` & `gopro-overlay-0.96.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/PKG-INFO` & `gopro-overlay-0.96.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.95.0
+Version: 0.96.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,17 @@
 <a href="https://github.com/time4tea/gopro-dashboard-overlay/discussions"><img alt="GitHub Discussions" src="https://img.shields.io/github/discussions/time4tea/gopro-dashboard-overlay?style=for-the-badge"></a>
 <a href="https://pypi.org/project/gopro-overlay/"><img alt="PyPI" src="https://img.shields.io/pypi/v/gopro-overlay?style=for-the-badge"></a>
 <a href="https://hub.docker.com/r/overlaydash/gopro-dashboard-overlay"><img alt="Docker" src="https://img.shields.io/docker/v/overlaydash/gopro-dashboard-overlay?label=Docker&style=for-the-badge"></a>
 
 Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
 
 - Overlaying exciting graphics onto GoPro videos with super-exact synchronization
-- Create videos from any GPX file - no GoPro required
+- Create videos from any GPX or FIT file - no GoPro required
 - Support multiple resolutions, most GoPro models, normal, timelapse & timewarp modes
+- Support GPUs to create movies at up to 17x realtime
 - Convert GoPro movie metadata to GPX or CSV files
 - Cut sections from GoPro movies (including metadata)
 
 ## Examples
 
 ![Example Dashboard Image](examples/2022-05-15-example.png)
 ![Example Dashboard Image](examples/2022-06-11-contrib-example.png)
@@ -233,14 +234,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly.
```

#### html2text {}

```diff
@@ -1,132 +1,136 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.95.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.96.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Console Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Video Requires-Python: >=3.10 Description-
 Content-Type: text/markdown License-File: LICENSE.md # Create video overlays
 from GoPro Videos or any GPX/FIT file [GitHub_Discussions] [PyPI] [Docker]
 Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-
 overlay/discussions) - Overlaying exciting graphics onto GoPro videos with
-super-exact synchronization - Create videos from any GPX file - no GoPro
+super-exact synchronization - Create videos from any GPX or FIT file - no GoPro
 required - Support multiple resolutions, most GoPro models, normal, timelapse &
-timewarp modes - Convert GoPro movie metadata to GPX or CSV files - Cut
-sections from GoPro movies (including metadata) ## Examples ![Example Dashboard
-Image](examples/2022-05-15-example.png) ![Example Dashboard Image](examples/
-2022-06-11-contrib-example.png) ![Example Dashboard Image](examples/2022-07-19-
-contrib-example-plane.jpg) An Example of 'overlay only' mode, which generates
-movies from GPX files ![Example Dashboard Image](examples/2022-11-24-gpx-only-
-overlay.png) Example from [examples/layout](examples/layout) ![Example
-Dashboard Image](examples/layout/layout-cairo-2704x1520.png) ## Map Styles
-Almost 30 different map styles are supported! - See [map styles](docs/maps/
-README.md) for more *Example* | . | . | . | . | |------------------------------
--------|-----------------------------------------------|-----------------------
---------------------------------|----------------------------------------------
----------| | ![osm](docs/maps/map_style_osm.png) | ![tf-cycle](docs/maps/
-map_style_tf-cycle.png) | ![tf-transport](docs/maps/map_style_tf-transport.png)
-| ![tf-landscape](docs/maps/map_style_tf-landscape.png) | ## Requirements -
-Python3.10 (development is done on Python3.11) - ffmpeg (you'll need the ffmpeg
-program installed) - libraqm (needed by [Pillow](https://pypi.org/project/
-Pillow/)) - Unixy machine (probably, untested on Windows) ## Installation
-Install locally using `pip`, or use the provided Docker image Optional: Some
-widgets require the `cairo` library - which must be installed separately. ###
-Installing and running with docker The docker image is a new thing and still a
-bit experimental... please file an issue if you find any problems. The docker
-image contains all you need to get started, and uses a volume `/work/`, which
-we suggest you map to the current directory which can contain your GoPro files.
-Note that the docker version doesn't support nvidia GPU extensions. The most
-recent version on docker is: [Docker] ```shell docker run -it -v "$(pwd):/work"
-overlaydash/gopro-dashboard-overlay:  [args...] ``` e.g. ```shell docker run -
-it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:0.92.0 gopro-
-dashboard.py GH010122.MP4 render/docker.MP4 ``` Files created by the program
-will be created with the same uid that owns the mapped directory. You can use
-the `--cache-dir` and `--config-dir` command line arguments to configure where
-the cache and config dirs are, thereby making it easier to use persistent
-mapped volumes. ### Installing and running with pip ```shell python -m venv
-venv venv/bin/pip install gopro-overlay ``` The Roboto font needs to be
-installed on your system. You could install it with one of the following
-commands maybe. ```bash pacman -S ttf-roboto apt install truetype-roboto apt
-install fonts-roboto ``` #### (Optional) Installing pycairo Optionally, install
-`pycairo` ```shell venv/bin/pip install pycairo==1.23.0 ``` You might need to
-install some system libraries - This is what the pycairo docs suggest: Ubuntu/
-Debian: `sudo apt install libcairo2-dev pkg-config python3-dev` macOS/Homebrew:
-`brew install cairo pkg-config` ## Overlaying a dashboard ```shell venv/bin/
-gopro-dashboard.py ``` The GPS track in Hero 9 (at least) seems to be very
-poor. If you supply a GPX file from a Garmin or whatever, the program will use
-this instead for the GPS. Privacy allows you to set a privacy zone. Various
-widgets will not draw points within that zone. The data recorded in the GoPro
-video will uses GPS time, which (broadly) is UTC. The renderer will use your
-local timezone to interpret this, and use the local timezone. This may produce
-strange results if you go on holiday somewhere, but then render the files when
-you get back home! On linux you can use the TZ variable to change the timezone
-that's used. ### Example For full instructions on all command lines see [docs/
-bin](docs/bin) ```shell venv/bin/gopro-dashboard.py --gpx ~/Downloads/
-Morning_Ride.gpx --privacy 52.000,-0.40000,0.50 ~/gopro/GH020073.MP4 GH020073-
-dashboard.MP4 ``` ## Writeups There's a great writeup of how to use the
-software to make an overlay from a GPX file at https://blog.cubieserver.de/
-2022/creating-gpx-overlay-videos-on-linux/ (Nov 2022) ### Format of the
-Dashboard Configuration file Several dashboards are built-in to the software,
-but the dashboard layout is highly configurable, controlled by an XML file. For
-more information on the (extensive) configurability of the layout please see
-[docs/xml](docs/xml) and lots of [examples](docs/xml/examples/README.md) ##
-FFMPEG Control & GPUs *Experimental* FFMPEG has **a lot** of options! This
-program comes with some mostly sensible defaults, but to use GPUs and control
-the output much more carefully, including framerates and bitrates, you can use
-a JSON file containing a number of 'profiles' and select the profile you want
-when running the program. For more details on how to select these, and an
-example of Nvidia GPU, please see [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/
-PERFORMANCE_GUIDE.md) Please also see [PERFORMANCE.md](PERFORMANCE.md) ##
-Converting to GPX files ```shell venv/bin/gopro-to-gpx.py  [output-file] ``` ##
-Joining a sequence of MP4 files together Use the gopro-join.py command. Given a
-single file from the sequence, it will find and join together all the files. If
-you have any problems with this, please do raise an issue - I don't have that
-much test data. The joined file almost certainly won't work in the GoPro tools!
-- But it should work with `gopro-dashboard.py` - I will look into the
-additional technical stuff required to make it work in the GoPro tools. *This
-will require a lot of disk space!* ```shell venv/bin/gopro-join.py /media/
-sdcard/DCIM/100GOPRO/GH030170.MP4 /data/gopro/nice-ride.MP4 ``` ## Cutting a
-section from a GoPro file You can cut a section of the gopro file, with
-metadata. ## Related Software - https://github.com/julesgraus/
-interactiveGoProDashboardTool - An interactive helper to build the command line
-for the dashboard program ## Known Bugs / Issues - Only tested on a GoPro Hero
-9/11, that's all I have. Sample files for other devices are welcomed. ## Icons
-Icon files in [icons](gopro_overlay/icons) are not covered by the MIT licence
-## Map Data Data Â© [OpenStreetMap contributors](http://www.openstreetmap.org/
-copyright) Some Maps Â© [Thunderforest](http://www.thunderforest.com/) ##
-References https://github.com/juanmcasillas/gopro2gpx https://github.com/
-JuanIrache/gopro-telemetry https://github.com/gopro/gpmf-parser https://
-coderunner.io/how-to-compress-gopro-movies-and-keep-metadata/ ## Other Related
-Software https://github.com/progweb/gpx2video https://github.com/JuanIrache/
-gopro-telemetry ## Latest Changes If you find any issues with new releases,
-please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-
-dashboard-overlay/discussions) - 0.95.0 [Feature] Add api key support for
-geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
-issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
-[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
-Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
-now possible. It takes a bit of work, but now can render at 12x realtime. See
-[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
-Remove support for `--output-size` as it didn't really work properly anyway. -
-0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
-much faster rendering, but may not work on all architectures. Speed
-improvements highly dependent on `ffmpeg` performance. Likely much faster when
-using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
-items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
-patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
-quickly. - [Change] Map rendering caches tile images more efficiently, so draws
-more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
-A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
-[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
+timewarp modes - Support GPUs to create movies at up to 17x realtime - Convert
+GoPro movie metadata to GPX or CSV files - Cut sections from GoPro movies
+(including metadata) ## Examples ![Example Dashboard Image](examples/2022-05-
+15-example.png) ![Example Dashboard Image](examples/2022-06-11-contrib-
+example.png) ![Example Dashboard Image](examples/2022-07-19-contrib-example-
+plane.jpg) An Example of 'overlay only' mode, which generates movies from GPX
+files ![Example Dashboard Image](examples/2022-11-24-gpx-only-overlay.png)
+Example from [examples/layout](examples/layout) ![Example Dashboard Image]
+(examples/layout/layout-cairo-2704x1520.png) ## Map Styles Almost 30 different
+map styles are supported! - See [map styles](docs/maps/README.md) for more
+*Example* | . | . | . | . | |-------------------------------------|------------
+-----------------------------------|-------------------------------------------
+------------|-------------------------------------------------------| | ![osm]
+(docs/maps/map_style_osm.png) | ![tf-cycle](docs/maps/map_style_tf-cycle.png) |
+![tf-transport](docs/maps/map_style_tf-transport.png) | ![tf-landscape](docs/
+maps/map_style_tf-landscape.png) | ## Requirements - Python3.10 (development is
+done on Python3.11) - ffmpeg (you'll need the ffmpeg program installed) -
+libraqm (needed by [Pillow](https://pypi.org/project/Pillow/)) - Unixy machine
+(probably, untested on Windows) ## Installation Install locally using `pip`, or
+use the provided Docker image Optional: Some widgets require the `cairo`
+library - which must be installed separately. ### Installing and running with
+docker The docker image is a new thing and still a bit experimental... please
+file an issue if you find any problems. The docker image contains all you need
+to get started, and uses a volume `/work/`, which we suggest you map to the
+current directory which can contain your GoPro files. Note that the docker
+version doesn't support nvidia GPU extensions. The most recent version on
+docker is: [Docker] ```shell docker run -it -v "$(pwd):/work" overlaydash/
+gopro-dashboard-overlay:  [args...] ``` e.g. ```shell docker run -it -v "$
+(pwd):/work" overlaydash/gopro-dashboard-overlay:0.92.0 gopro-dashboard.py
+GH010122.MP4 render/docker.MP4 ``` Files created by the program will be created
+with the same uid that owns the mapped directory. You can use the `--cache-dir`
+and `--config-dir` command line arguments to configure where the cache and
+config dirs are, thereby making it easier to use persistent mapped volumes. ###
+Installing and running with pip ```shell python -m venv venv venv/bin/pip
+install gopro-overlay ``` The Roboto font needs to be installed on your system.
+You could install it with one of the following commands maybe. ```bash pacman -
+S ttf-roboto apt install truetype-roboto apt install fonts-roboto ``` ####
+(Optional) Installing pycairo Optionally, install `pycairo` ```shell venv/bin/
+pip install pycairo==1.23.0 ``` You might need to install some system libraries
+- This is what the pycairo docs suggest: Ubuntu/Debian: `sudo apt install
+libcairo2-dev pkg-config python3-dev` macOS/Homebrew: `brew install cairo pkg-
+config` ## Overlaying a dashboard ```shell venv/bin/gopro-dashboard.py ``` The
+GPS track in Hero 9 (at least) seems to be very poor. If you supply a GPX file
+from a Garmin or whatever, the program will use this instead for the GPS.
+Privacy allows you to set a privacy zone. Various widgets will not draw points
+within that zone. The data recorded in the GoPro video will uses GPS time,
+which (broadly) is UTC. The renderer will use your local timezone to interpret
+this, and use the local timezone. This may produce strange results if you go on
+holiday somewhere, but then render the files when you get back home! On linux
+you can use the TZ variable to change the timezone that's used. ### Example For
+full instructions on all command lines see [docs/bin](docs/bin) ```shell venv/
+bin/gopro-dashboard.py --gpx ~/Downloads/Morning_Ride.gpx --privacy 52.000,-
+0.40000,0.50 ~/gopro/GH020073.MP4 GH020073-dashboard.MP4 ``` ## Writeups
+There's a great writeup of how to use the software to make an overlay from a
+GPX file at https://blog.cubieserver.de/2022/creating-gpx-overlay-videos-on-
+linux/ (Nov 2022) ### Format of the Dashboard Configuration file Several
+dashboards are built-in to the software, but the dashboard layout is highly
+configurable, controlled by an XML file. For more information on the
+(extensive) configurability of the layout please see [docs/xml](docs/xml) and
+lots of [examples](docs/xml/examples/README.md) ## FFMPEG Control & GPUs
+*Experimental* FFMPEG has **a lot** of options! This program comes with some
+mostly sensible defaults, but to use GPUs and control the output much more
+carefully, including framerates and bitrates, you can use a JSON file
+containing a number of 'profiles' and select the profile you want when running
+the program. For more details on how to select these, and an example of Nvidia
+GPU, please see [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
+Please also see [PERFORMANCE.md](PERFORMANCE.md) ## Converting to GPX files
+```shell venv/bin/gopro-to-gpx.py  [output-file] ``` ## Joining a sequence of
+MP4 files together Use the gopro-join.py command. Given a single file from the
+sequence, it will find and join together all the files. If you have any
+problems with this, please do raise an issue - I don't have that much test
+data. The joined file almost certainly won't work in the GoPro tools! - But it
+should work with `gopro-dashboard.py` - I will look into the additional
+technical stuff required to make it work in the GoPro tools. *This will require
+a lot of disk space!* ```shell venv/bin/gopro-join.py /media/sdcard/DCIM/
+100GOPRO/GH030170.MP4 /data/gopro/nice-ride.MP4 ``` ## Cutting a section from a
+GoPro file You can cut a section of the gopro file, with metadata. ## Related
+Software - https://github.com/julesgraus/interactiveGoProDashboardTool - An
+interactive helper to build the command line for the dashboard program ## Known
+Bugs / Issues - Only tested on a GoPro Hero 9/11, that's all I have. Sample
+files for other devices are welcomed. ## Icons Icon files in [icons]
+(gopro_overlay/icons) are not covered by the MIT licence ## Map Data Data Â©
+[OpenStreetMap contributors](http://www.openstreetmap.org/copyright) Some Maps
+Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
+github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
+telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
+compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
+github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
+Latest Changes If you find any issues with new releases, please discuss in
+[GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
+discussions) - 0.96.0 [Feature] Hopefully add support for older gopro files
+when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/
+issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising
+and some example code. - 0.95.0 [Feature] Add api key support for geocode.xyz -
+[#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks
+[@mishuha](https://github.com/mishuha) for raising. - 0.94.0 [Change] Update
+docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully
+gpu* decoding/overlay/encoding. Huge performance increase now possible. It
+takes a bit of work, but now can render at 12x realtime. See [docs/bin/
+PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove
+support for `--output-size` as it didn't really work properly anyway. - 0.92.0
+[Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much
+faster rendering, but may not work on all architectures. Speed improvements
+highly dependent on `ffmpeg` performance. Likely much faster when using `--
+generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that
+don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
+raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
+[Change] Map rendering caches tile images more efficiently, so draws more
+quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
+like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
+annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
+Journey Map broke when no there were no locked GPS points in the movie. -
 Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
 Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
 instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
 gauge-marker` - a nice clean gauge component, with a marker for the current
 value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
 06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
 attributes in layout files. This may cause some custom layouts to break! - But
```

### Comparing `gopro-overlay-0.95.0/README.md` & `gopro-overlay-0.96.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 <a href="https://github.com/time4tea/gopro-dashboard-overlay/discussions"><img alt="GitHub Discussions" src="https://img.shields.io/github/discussions/time4tea/gopro-dashboard-overlay?style=for-the-badge"></a>
 <a href="https://pypi.org/project/gopro-overlay/"><img alt="PyPI" src="https://img.shields.io/pypi/v/gopro-overlay?style=for-the-badge"></a>
 <a href="https://hub.docker.com/r/overlaydash/gopro-dashboard-overlay"><img alt="Docker" src="https://img.shields.io/docker/v/overlaydash/gopro-dashboard-overlay?label=Docker&style=for-the-badge"></a>
 
 Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
 
 - Overlaying exciting graphics onto GoPro videos with super-exact synchronization
-- Create videos from any GPX file - no GoPro required
+- Create videos from any GPX or FIT file - no GoPro required
 - Support multiple resolutions, most GoPro models, normal, timelapse & timewarp modes
+- Support GPUs to create movies at up to 17x realtime
 - Convert GoPro movie metadata to GPX or CSV files
 - Cut sections from GoPro movies (including metadata)
 
 ## Examples
 
 ![Example Dashboard Image](examples/2022-05-15-example.png)
 ![Example Dashboard Image](examples/2022-06-11-contrib-example.png)
@@ -212,14 +213,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly.
```

#### html2text {}

```diff
@@ -1,122 +1,125 @@
 # Create video overlays from GoPro Videos or any GPX/FIT file [GitHub
 Discussions] [PyPI] [Docker] Discuss on [GitHub Discussions](https://
 github.com/time4tea/gopro-dashboard-overlay/discussions) - Overlaying exciting
 graphics onto GoPro videos with super-exact synchronization - Create videos
-from any GPX file - no GoPro required - Support multiple resolutions, most
-GoPro models, normal, timelapse & timewarp modes - Convert GoPro movie metadata
-to GPX or CSV files - Cut sections from GoPro movies (including metadata) ##
-Examples ![Example Dashboard Image](examples/2022-05-15-example.png) ![Example
-Dashboard Image](examples/2022-06-11-contrib-example.png) ![Example Dashboard
-Image](examples/2022-07-19-contrib-example-plane.jpg) An Example of 'overlay
-only' mode, which generates movies from GPX files ![Example Dashboard Image]
-(examples/2022-11-24-gpx-only-overlay.png) Example from [examples/layout]
-(examples/layout) ![Example Dashboard Image](examples/layout/layout-cairo-
-2704x1520.png) ## Map Styles Almost 30 different map styles are supported! -
-See [map styles](docs/maps/README.md) for more *Example* | . | . | . | . | |---
-----------------------------------|--------------------------------------------
----|-------------------------------------------------------|-------------------
-------------------------------------| | ![osm](docs/maps/map_style_osm.png) | !
-[tf-cycle](docs/maps/map_style_tf-cycle.png) | ![tf-transport](docs/maps/
-map_style_tf-transport.png) | ![tf-landscape](docs/maps/map_style_tf-
-landscape.png) | ## Requirements - Python3.10 (development is done on
-Python3.11) - ffmpeg (you'll need the ffmpeg program installed) - libraqm
-(needed by [Pillow](https://pypi.org/project/Pillow/)) - Unixy machine
-(probably, untested on Windows) ## Installation Install locally using `pip`, or
-use the provided Docker image Optional: Some widgets require the `cairo`
-library - which must be installed separately. ### Installing and running with
-docker The docker image is a new thing and still a bit experimental... please
-file an issue if you find any problems. The docker image contains all you need
-to get started, and uses a volume `/work/`, which we suggest you map to the
-current directory which can contain your GoPro files. Note that the docker
-version doesn't support nvidia GPU extensions. The most recent version on
-docker is: [Docker] ```shell docker run -it -v "$(pwd):/work" overlaydash/
-gopro-dashboard-overlay:  [args...] ``` e.g. ```shell docker run -it -v "$
-(pwd):/work" overlaydash/gopro-dashboard-overlay:0.92.0 gopro-dashboard.py
-GH010122.MP4 render/docker.MP4 ``` Files created by the program will be created
-with the same uid that owns the mapped directory. You can use the `--cache-dir`
-and `--config-dir` command line arguments to configure where the cache and
-config dirs are, thereby making it easier to use persistent mapped volumes. ###
-Installing and running with pip ```shell python -m venv venv venv/bin/pip
-install gopro-overlay ``` The Roboto font needs to be installed on your system.
-You could install it with one of the following commands maybe. ```bash pacman -
-S ttf-roboto apt install truetype-roboto apt install fonts-roboto ``` ####
-(Optional) Installing pycairo Optionally, install `pycairo` ```shell venv/bin/
-pip install pycairo==1.23.0 ``` You might need to install some system libraries
-- This is what the pycairo docs suggest: Ubuntu/Debian: `sudo apt install
-libcairo2-dev pkg-config python3-dev` macOS/Homebrew: `brew install cairo pkg-
-config` ## Overlaying a dashboard ```shell venv/bin/gopro-dashboard.py ``` The
-GPS track in Hero 9 (at least) seems to be very poor. If you supply a GPX file
-from a Garmin or whatever, the program will use this instead for the GPS.
-Privacy allows you to set a privacy zone. Various widgets will not draw points
-within that zone. The data recorded in the GoPro video will uses GPS time,
-which (broadly) is UTC. The renderer will use your local timezone to interpret
-this, and use the local timezone. This may produce strange results if you go on
-holiday somewhere, but then render the files when you get back home! On linux
-you can use the TZ variable to change the timezone that's used. ### Example For
-full instructions on all command lines see [docs/bin](docs/bin) ```shell venv/
-bin/gopro-dashboard.py --gpx ~/Downloads/Morning_Ride.gpx --privacy 52.000,-
-0.40000,0.50 ~/gopro/GH020073.MP4 GH020073-dashboard.MP4 ``` ## Writeups
-There's a great writeup of how to use the software to make an overlay from a
-GPX file at https://blog.cubieserver.de/2022/creating-gpx-overlay-videos-on-
-linux/ (Nov 2022) ### Format of the Dashboard Configuration file Several
-dashboards are built-in to the software, but the dashboard layout is highly
-configurable, controlled by an XML file. For more information on the
-(extensive) configurability of the layout please see [docs/xml](docs/xml) and
-lots of [examples](docs/xml/examples/README.md) ## FFMPEG Control & GPUs
-*Experimental* FFMPEG has **a lot** of options! This program comes with some
-mostly sensible defaults, but to use GPUs and control the output much more
-carefully, including framerates and bitrates, you can use a JSON file
-containing a number of 'profiles' and select the profile you want when running
-the program. For more details on how to select these, and an example of Nvidia
-GPU, please see [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
-Please also see [PERFORMANCE.md](PERFORMANCE.md) ## Converting to GPX files
-```shell venv/bin/gopro-to-gpx.py  [output-file] ``` ## Joining a sequence of
-MP4 files together Use the gopro-join.py command. Given a single file from the
-sequence, it will find and join together all the files. If you have any
-problems with this, please do raise an issue - I don't have that much test
-data. The joined file almost certainly won't work in the GoPro tools! - But it
-should work with `gopro-dashboard.py` - I will look into the additional
-technical stuff required to make it work in the GoPro tools. *This will require
-a lot of disk space!* ```shell venv/bin/gopro-join.py /media/sdcard/DCIM/
-100GOPRO/GH030170.MP4 /data/gopro/nice-ride.MP4 ``` ## Cutting a section from a
-GoPro file You can cut a section of the gopro file, with metadata. ## Related
-Software - https://github.com/julesgraus/interactiveGoProDashboardTool - An
-interactive helper to build the command line for the dashboard program ## Known
-Bugs / Issues - Only tested on a GoPro Hero 9/11, that's all I have. Sample
-files for other devices are welcomed. ## Icons Icon files in [icons]
-(gopro_overlay/icons) are not covered by the MIT licence ## Map Data Data Â©
-[OpenStreetMap contributors](http://www.openstreetmap.org/copyright) Some Maps
-Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
-github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
-telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
-compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
-github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
-Latest Changes If you find any issues with new releases, please discuss in
-[GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
-discussions) - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117]
-(https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks
-[@mishuha](https://github.com/mishuha) for raising. - 0.94.0 [Change] Update
-docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully
-gpu* decoding/overlay/encoding. Huge performance increase now possible. It
-takes a bit of work, but now can render at 12x realtime. See [docs/bin/
-PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove
-support for `--output-size` as it didn't really work properly anyway. - 0.92.0
-[Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much
-faster rendering, but may not work on all architectures. Speed improvements
-highly dependent on `ffmpeg` performance. Likely much faster when using `--
-generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that
-don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
-raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
-[Change] Map rendering caches tile images more efficiently, so draws more
-quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
-like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
-Journey Map broke when no there were no locked GPS points in the movie. -
+from any GPX or FIT file - no GoPro required - Support multiple resolutions,
+most GoPro models, normal, timelapse & timewarp modes - Support GPUs to create
+movies at up to 17x realtime - Convert GoPro movie metadata to GPX or CSV files
+- Cut sections from GoPro movies (including metadata) ## Examples ![Example
+Dashboard Image](examples/2022-05-15-example.png) ![Example Dashboard Image]
+(examples/2022-06-11-contrib-example.png) ![Example Dashboard Image](examples/
+2022-07-19-contrib-example-plane.jpg) An Example of 'overlay only' mode, which
+generates movies from GPX files ![Example Dashboard Image](examples/2022-11-24-
+gpx-only-overlay.png) Example from [examples/layout](examples/layout) ![Example
+Dashboard Image](examples/layout/layout-cairo-2704x1520.png) ## Map Styles
+Almost 30 different map styles are supported! - See [map styles](docs/maps/
+README.md) for more *Example* | . | . | . | . | |------------------------------
+-------|-----------------------------------------------|-----------------------
+--------------------------------|----------------------------------------------
+---------| | ![osm](docs/maps/map_style_osm.png) | ![tf-cycle](docs/maps/
+map_style_tf-cycle.png) | ![tf-transport](docs/maps/map_style_tf-transport.png)
+| ![tf-landscape](docs/maps/map_style_tf-landscape.png) | ## Requirements -
+Python3.10 (development is done on Python3.11) - ffmpeg (you'll need the ffmpeg
+program installed) - libraqm (needed by [Pillow](https://pypi.org/project/
+Pillow/)) - Unixy machine (probably, untested on Windows) ## Installation
+Install locally using `pip`, or use the provided Docker image Optional: Some
+widgets require the `cairo` library - which must be installed separately. ###
+Installing and running with docker The docker image is a new thing and still a
+bit experimental... please file an issue if you find any problems. The docker
+image contains all you need to get started, and uses a volume `/work/`, which
+we suggest you map to the current directory which can contain your GoPro files.
+Note that the docker version doesn't support nvidia GPU extensions. The most
+recent version on docker is: [Docker] ```shell docker run -it -v "$(pwd):/work"
+overlaydash/gopro-dashboard-overlay:  [args...] ``` e.g. ```shell docker run -
+it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:0.92.0 gopro-
+dashboard.py GH010122.MP4 render/docker.MP4 ``` Files created by the program
+will be created with the same uid that owns the mapped directory. You can use
+the `--cache-dir` and `--config-dir` command line arguments to configure where
+the cache and config dirs are, thereby making it easier to use persistent
+mapped volumes. ### Installing and running with pip ```shell python -m venv
+venv venv/bin/pip install gopro-overlay ``` The Roboto font needs to be
+installed on your system. You could install it with one of the following
+commands maybe. ```bash pacman -S ttf-roboto apt install truetype-roboto apt
+install fonts-roboto ``` #### (Optional) Installing pycairo Optionally, install
+`pycairo` ```shell venv/bin/pip install pycairo==1.23.0 ``` You might need to
+install some system libraries - This is what the pycairo docs suggest: Ubuntu/
+Debian: `sudo apt install libcairo2-dev pkg-config python3-dev` macOS/Homebrew:
+`brew install cairo pkg-config` ## Overlaying a dashboard ```shell venv/bin/
+gopro-dashboard.py ``` The GPS track in Hero 9 (at least) seems to be very
+poor. If you supply a GPX file from a Garmin or whatever, the program will use
+this instead for the GPS. Privacy allows you to set a privacy zone. Various
+widgets will not draw points within that zone. The data recorded in the GoPro
+video will uses GPS time, which (broadly) is UTC. The renderer will use your
+local timezone to interpret this, and use the local timezone. This may produce
+strange results if you go on holiday somewhere, but then render the files when
+you get back home! On linux you can use the TZ variable to change the timezone
+that's used. ### Example For full instructions on all command lines see [docs/
+bin](docs/bin) ```shell venv/bin/gopro-dashboard.py --gpx ~/Downloads/
+Morning_Ride.gpx --privacy 52.000,-0.40000,0.50 ~/gopro/GH020073.MP4 GH020073-
+dashboard.MP4 ``` ## Writeups There's a great writeup of how to use the
+software to make an overlay from a GPX file at https://blog.cubieserver.de/
+2022/creating-gpx-overlay-videos-on-linux/ (Nov 2022) ### Format of the
+Dashboard Configuration file Several dashboards are built-in to the software,
+but the dashboard layout is highly configurable, controlled by an XML file. For
+more information on the (extensive) configurability of the layout please see
+[docs/xml](docs/xml) and lots of [examples](docs/xml/examples/README.md) ##
+FFMPEG Control & GPUs *Experimental* FFMPEG has **a lot** of options! This
+program comes with some mostly sensible defaults, but to use GPUs and control
+the output much more carefully, including framerates and bitrates, you can use
+a JSON file containing a number of 'profiles' and select the profile you want
+when running the program. For more details on how to select these, and an
+example of Nvidia GPU, please see [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/
+PERFORMANCE_GUIDE.md) Please also see [PERFORMANCE.md](PERFORMANCE.md) ##
+Converting to GPX files ```shell venv/bin/gopro-to-gpx.py  [output-file] ``` ##
+Joining a sequence of MP4 files together Use the gopro-join.py command. Given a
+single file from the sequence, it will find and join together all the files. If
+you have any problems with this, please do raise an issue - I don't have that
+much test data. The joined file almost certainly won't work in the GoPro tools!
+- But it should work with `gopro-dashboard.py` - I will look into the
+additional technical stuff required to make it work in the GoPro tools. *This
+will require a lot of disk space!* ```shell venv/bin/gopro-join.py /media/
+sdcard/DCIM/100GOPRO/GH030170.MP4 /data/gopro/nice-ride.MP4 ``` ## Cutting a
+section from a GoPro file You can cut a section of the gopro file, with
+metadata. ## Related Software - https://github.com/julesgraus/
+interactiveGoProDashboardTool - An interactive helper to build the command line
+for the dashboard program ## Known Bugs / Issues - Only tested on a GoPro Hero
+9/11, that's all I have. Sample files for other devices are welcomed. ## Icons
+Icon files in [icons](gopro_overlay/icons) are not covered by the MIT licence
+## Map Data Data Â© [OpenStreetMap contributors](http://www.openstreetmap.org/
+copyright) Some Maps Â© [Thunderforest](http://www.thunderforest.com/) ##
+References https://github.com/juanmcasillas/gopro2gpx https://github.com/
+JuanIrache/gopro-telemetry https://github.com/gopro/gpmf-parser https://
+coderunner.io/how-to-compress-gopro-movies-and-keep-metadata/ ## Other Related
+Software https://github.com/progweb/gpx2video https://github.com/JuanIrache/
+gopro-telemetry ## Latest Changes If you find any issues with new releases,
+please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-
+dashboard-overlay/discussions) - 0.96.0 [Feature] Hopefully add support for
+older gopro files when joining. [#129](https://github.com/time4tea/gopro-
+dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/
+FFMbyBicycle) for raising and some example code. - 0.95.0 [Feature] Add api key
+support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
+- 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0
+[Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance
+increase now possible. It takes a bit of work, but now can render at 12x
+realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) -
+[Breaking] Remove support for `--output-size` as it didn't really work properly
+anyway. - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering.
+Potentially much faster rendering, but may not work on all architectures. Speed
+improvements highly dependent on `ffmpeg` performance. Likely much faster when
+using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
+items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
+dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
+patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
+quickly. - [Change] Map rendering caches tile images more efficiently, so draws
+more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
+A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
+round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
+[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
 Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
 Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
 instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
 gauge-marker` - a nice clean gauge component, with a marker for the current
 value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
 06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
 attributes in layout files. This may cause some custom layouts to break! - But
```

### Comparing `gopro-overlay-0.95.0/bin/gopro-contrib-data-extract.py` & `gopro-overlay-0.96.0/bin/gopro-contrib-data-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-cut.py` & `gopro-overlay-0.96.0/bin/gopro-cut.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-dashboard.py` & `gopro-overlay-0.96.0/bin/gopro-dashboard.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-debug.py` & `gopro-overlay-0.96.0/bin/gopro-debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-extract.py` & `gopro-overlay-0.96.0/bin/gopro-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-join.py` & `gopro-overlay-0.96.0/bin/gopro-join.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-layout.py` & `gopro-overlay-0.96.0/bin/gopro-layout.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-rename.py` & `gopro-overlay-0.96.0/bin/gopro-rename.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-to-csv.py` & `gopro-overlay-0.96.0/bin/gopro-to-csv.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/bin/gopro-to-gpx.py` & `gopro-overlay-0.96.0/bin/gopro-to-gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/arguments.py` & `gopro-overlay-0.96.0/gopro_overlay/arguments.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/buffering.py` & `gopro-overlay-0.96.0/gopro_overlay/buffering.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/common.py` & `gopro-overlay-0.96.0/gopro_overlay/common.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/dimensions.py` & `gopro-overlay-0.96.0/gopro_overlay/dimensions.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/entry.py` & `gopro-overlay-0.96.0/gopro_overlay/entry.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/execution.py` & `gopro-overlay-0.96.0/gopro_overlay/execution.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/fake.py` & `gopro-overlay-0.96.0/gopro_overlay/fake.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/ffmpeg.py` & `gopro-overlay-0.96.0/gopro_overlay/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/ffmpeg_profile.py` & `gopro-overlay-0.96.0/gopro_overlay/ffmpeg_profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/filenaming.py` & `gopro-overlay-0.96.0/gopro_overlay/filenaming.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class Encoding(Enum):
     AVC = 1
     HEVC = 2
 
     @staticmethod
     def from_letter(letter):
-        if letter == "H":
+        if letter == "H" or letter == "P" or letter == "OPR":
             return Encoding.AVC
         elif letter == "X":
             return Encoding.HEVC
         else:
             raise ValueError(f"Unknown encoding letter {letter}")
 
 
@@ -40,23 +40,25 @@
         if match is None:
             raise ValueError(f"Not a valid GoPro filename {filepath}")
 
         self.name = filepath.name
         self.encoding = Encoding.from_letter(match.group(1))
         self.letter = match.group(1)
         self.recording = int(match.group(3))
-        self.sequence = int(match.group(2))
+        self.sequence = int(match.group(2)) if match.group(2) is not None else 0
+        self.extension = match.group(4)
 
     @staticmethod
     def is_valid_filepath(f: Path):
-        return re.search(r"^G([HX])(\d{2})(\d{4}).MP4", f.name)
+        return re.search(r"^G([HXP]|OPR)(\d{2})?(\d{4}).(MP4|mp4)", f.name)
 
     def related_files(self, d: Path, listdir=os.listdir):
-        find = re.compile(r"G{l}\d\d{n}\.MP4".format(
+        find = re.compile(r"G{l}\d\d{n}\.{e}".format(
             l=self.letter,
+            e=self.extension,
             n=f"{self.recording:04}"
         ))
 
         potentials = [ d / name for name in listdir(d) ]
 
         found = [GoProFile(p) for p in potentials if find.match(p.name)]
         found.sort(key=lambda f: f.sequence)
```

### Comparing `gopro-overlay-0.95.0/gopro_overlay/fit.py` & `gopro-overlay-0.96.0/gopro_overlay/fit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/framemeta.py` & `gopro-overlay-0.96.0/gopro_overlay/framemeta.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/framemeta_gpx.py` & `gopro-overlay-0.96.0/gopro_overlay/framemeta_gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/geo.py` & `gopro-overlay-0.96.0/gopro_overlay/geo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/geo_render.py` & `gopro-overlay-0.96.0/gopro_overlay/geo_render.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/geocode.py` & `gopro-overlay-0.96.0/gopro_overlay/geocode.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd_calculate.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd_calculate.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_cori.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_cori.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_debug.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_gps.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_grav.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_grav.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpmd_visitors_xyz.py` & `gopro-overlay-0.96.0/gopro_overlay/gpmd_visitors_xyz.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/gpx.py` & `gopro-overlay-0.96.0/gopro_overlay/gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/bicycle.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/car.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/car.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/faq.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/faq.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/forbidden.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/forbidden.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/gauge-1.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/gauge-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/gauge.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/gauge.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_2d.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_2d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_3d.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_3d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_none.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_none.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/gps_lock_unknown.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/gps_lock_unknown.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/heartbeat.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/heartbeat.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/ice-cream-van.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/ice-cream-van.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/mountain-range.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/mountain-range.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/mountain.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/mountain.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/power.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/power.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/ruler.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/ruler.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/slope-triangle.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/slope-triangle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/slope.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/slope.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/thermometer-1.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/thermometer-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/thermometer.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/thermometer.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/user.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/user.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/icons/van-black-side-view.png` & `gopro-overlay-0.96.0/gopro_overlay/icons/van-black-side-view.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/journey.py` & `gopro-overlay-0.96.0/gopro_overlay/journey.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layout.py` & `gopro-overlay-0.96.0/gopro_overlay/layout.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layout_components.py` & `gopro-overlay-0.96.0/gopro_overlay/layout_components.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layout_xml.py` & `gopro-overlay-0.96.0/gopro_overlay/layout_xml.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layout_xml_attribute.py` & `gopro-overlay-0.96.0/gopro_overlay/layout_xml_attribute.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layout_xml_cairo.py` & `gopro-overlay-0.96.0/gopro_overlay/layout_xml_cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layouts/default-1920x1080.xml` & `gopro-overlay-0.96.0/gopro_overlay/layouts/default-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layouts/default-2704x1520.xml` & `gopro-overlay-0.96.0/gopro_overlay/layouts/default-2704x1520.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layouts/default-3840x2160.xml` & `gopro-overlay-0.96.0/gopro_overlay/layouts/default-3840x2160.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layouts/example-2.xml` & `gopro-overlay-0.96.0/gopro_overlay/layouts/example-2.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layouts/example.xml` & `gopro-overlay-0.96.0/gopro_overlay/layouts/example.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/layouts/power-1920x1080.xml` & `gopro-overlay-0.96.0/gopro_overlay/layouts/power-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/models.py` & `gopro-overlay-0.96.0/gopro_overlay/models.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/point.py` & `gopro-overlay-0.96.0/gopro_overlay/point.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/privacy.py` & `gopro-overlay-0.96.0/gopro_overlay/privacy.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/progress_frames.py` & `gopro-overlay-0.96.0/gopro_overlay/progress_frames.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/rdp.py` & `gopro-overlay-0.96.0/gopro_overlay/rdp.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/smoothing.py` & `gopro-overlay-0.96.0/gopro_overlay/smoothing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/timeseries.py` & `gopro-overlay-0.96.0/gopro_overlay/timeseries.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/timeseries_process.py` & `gopro-overlay-0.96.0/gopro_overlay/timeseries_process.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/timeunits.py` & `gopro-overlay-0.96.0/gopro_overlay/timeunits.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/timing.py` & `gopro-overlay-0.96.0/gopro_overlay/timing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/asi.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/asi.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/bar.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/angle.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/angle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/annotation.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/annotation.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/background.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/background.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/bordered.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/bordered.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cairo.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/cap.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/cap.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/circuit.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/circuit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/colour.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/colour.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/ellipse.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/ellipse.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/face.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/face.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_marker.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_marker.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/gauge_round_254.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/gauge_round_254.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/needle.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/needle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/reading.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/reading.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/cairo/scale.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/cairo/scale.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/chart.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/chart.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/compass.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/compass.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/compass_arrow.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/compass_arrow.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/gps.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/gradient_bar.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/gradient_bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/info.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/info.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/map.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/map.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/profile.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/text.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/text.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/widgets.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay/widgets/widgets_experimental.py` & `gopro-overlay-0.96.0/gopro_overlay/widgets/widgets_experimental.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/gopro_overlay.egg-info/PKG-INFO` & `gopro-overlay-0.96.0/gopro_overlay.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.95.0
+Version: 0.96.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,16 +24,17 @@
 <a href="https://github.com/time4tea/gopro-dashboard-overlay/discussions"><img alt="GitHub Discussions" src="https://img.shields.io/github/discussions/time4tea/gopro-dashboard-overlay?style=for-the-badge"></a>
 <a href="https://pypi.org/project/gopro-overlay/"><img alt="PyPI" src="https://img.shields.io/pypi/v/gopro-overlay?style=for-the-badge"></a>
 <a href="https://hub.docker.com/r/overlaydash/gopro-dashboard-overlay"><img alt="Docker" src="https://img.shields.io/docker/v/overlaydash/gopro-dashboard-overlay?label=Docker&style=for-the-badge"></a>
 
 Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
 
 - Overlaying exciting graphics onto GoPro videos with super-exact synchronization
-- Create videos from any GPX file - no GoPro required
+- Create videos from any GPX or FIT file - no GoPro required
 - Support multiple resolutions, most GoPro models, normal, timelapse & timewarp modes
+- Support GPUs to create movies at up to 17x realtime
 - Convert GoPro movie metadata to GPX or CSV files
 - Cut sections from GoPro movies (including metadata)
 
 ## Examples
 
 ![Example Dashboard Image](examples/2022-05-15-example.png)
 ![Example Dashboard Image](examples/2022-06-11-contrib-example.png)
@@ -233,14 +234,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.96.0 [Feature] Hopefully add support for older gopro files when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising and some example code. 
 - 0.95.0 [Feature] Add api key support for geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising.
 - 0.94.0 [Change] Update docker image to python3.11/ffmpeg 6.0 
 - 0.93.0 [Feature] Support for *fully gpu* decoding/overlay/encoding. Huge performance increase now possible. It takes a bit of work, but now can render at 12x realtime. See [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
   - [Breaking] Remove support for `--output-size` as it didn't really work properly anyway. 
 - 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly.
```

#### html2text {}

```diff
@@ -1,132 +1,136 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.95.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.96.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
 Classifier: Environment :: Console Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Video Requires-Python: >=3.10 Description-
 Content-Type: text/markdown License-File: LICENSE.md # Create video overlays
 from GoPro Videos or any GPX/FIT file [GitHub_Discussions] [PyPI] [Docker]
 Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-
 overlay/discussions) - Overlaying exciting graphics onto GoPro videos with
-super-exact synchronization - Create videos from any GPX file - no GoPro
+super-exact synchronization - Create videos from any GPX or FIT file - no GoPro
 required - Support multiple resolutions, most GoPro models, normal, timelapse &
-timewarp modes - Convert GoPro movie metadata to GPX or CSV files - Cut
-sections from GoPro movies (including metadata) ## Examples ![Example Dashboard
-Image](examples/2022-05-15-example.png) ![Example Dashboard Image](examples/
-2022-06-11-contrib-example.png) ![Example Dashboard Image](examples/2022-07-19-
-contrib-example-plane.jpg) An Example of 'overlay only' mode, which generates
-movies from GPX files ![Example Dashboard Image](examples/2022-11-24-gpx-only-
-overlay.png) Example from [examples/layout](examples/layout) ![Example
-Dashboard Image](examples/layout/layout-cairo-2704x1520.png) ## Map Styles
-Almost 30 different map styles are supported! - See [map styles](docs/maps/
-README.md) for more *Example* | . | . | . | . | |------------------------------
--------|-----------------------------------------------|-----------------------
---------------------------------|----------------------------------------------
----------| | ![osm](docs/maps/map_style_osm.png) | ![tf-cycle](docs/maps/
-map_style_tf-cycle.png) | ![tf-transport](docs/maps/map_style_tf-transport.png)
-| ![tf-landscape](docs/maps/map_style_tf-landscape.png) | ## Requirements -
-Python3.10 (development is done on Python3.11) - ffmpeg (you'll need the ffmpeg
-program installed) - libraqm (needed by [Pillow](https://pypi.org/project/
-Pillow/)) - Unixy machine (probably, untested on Windows) ## Installation
-Install locally using `pip`, or use the provided Docker image Optional: Some
-widgets require the `cairo` library - which must be installed separately. ###
-Installing and running with docker The docker image is a new thing and still a
-bit experimental... please file an issue if you find any problems. The docker
-image contains all you need to get started, and uses a volume `/work/`, which
-we suggest you map to the current directory which can contain your GoPro files.
-Note that the docker version doesn't support nvidia GPU extensions. The most
-recent version on docker is: [Docker] ```shell docker run -it -v "$(pwd):/work"
-overlaydash/gopro-dashboard-overlay:  [args...] ``` e.g. ```shell docker run -
-it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:0.92.0 gopro-
-dashboard.py GH010122.MP4 render/docker.MP4 ``` Files created by the program
-will be created with the same uid that owns the mapped directory. You can use
-the `--cache-dir` and `--config-dir` command line arguments to configure where
-the cache and config dirs are, thereby making it easier to use persistent
-mapped volumes. ### Installing and running with pip ```shell python -m venv
-venv venv/bin/pip install gopro-overlay ``` The Roboto font needs to be
-installed on your system. You could install it with one of the following
-commands maybe. ```bash pacman -S ttf-roboto apt install truetype-roboto apt
-install fonts-roboto ``` #### (Optional) Installing pycairo Optionally, install
-`pycairo` ```shell venv/bin/pip install pycairo==1.23.0 ``` You might need to
-install some system libraries - This is what the pycairo docs suggest: Ubuntu/
-Debian: `sudo apt install libcairo2-dev pkg-config python3-dev` macOS/Homebrew:
-`brew install cairo pkg-config` ## Overlaying a dashboard ```shell venv/bin/
-gopro-dashboard.py ``` The GPS track in Hero 9 (at least) seems to be very
-poor. If you supply a GPX file from a Garmin or whatever, the program will use
-this instead for the GPS. Privacy allows you to set a privacy zone. Various
-widgets will not draw points within that zone. The data recorded in the GoPro
-video will uses GPS time, which (broadly) is UTC. The renderer will use your
-local timezone to interpret this, and use the local timezone. This may produce
-strange results if you go on holiday somewhere, but then render the files when
-you get back home! On linux you can use the TZ variable to change the timezone
-that's used. ### Example For full instructions on all command lines see [docs/
-bin](docs/bin) ```shell venv/bin/gopro-dashboard.py --gpx ~/Downloads/
-Morning_Ride.gpx --privacy 52.000,-0.40000,0.50 ~/gopro/GH020073.MP4 GH020073-
-dashboard.MP4 ``` ## Writeups There's a great writeup of how to use the
-software to make an overlay from a GPX file at https://blog.cubieserver.de/
-2022/creating-gpx-overlay-videos-on-linux/ (Nov 2022) ### Format of the
-Dashboard Configuration file Several dashboards are built-in to the software,
-but the dashboard layout is highly configurable, controlled by an XML file. For
-more information on the (extensive) configurability of the layout please see
-[docs/xml](docs/xml) and lots of [examples](docs/xml/examples/README.md) ##
-FFMPEG Control & GPUs *Experimental* FFMPEG has **a lot** of options! This
-program comes with some mostly sensible defaults, but to use GPUs and control
-the output much more carefully, including framerates and bitrates, you can use
-a JSON file containing a number of 'profiles' and select the profile you want
-when running the program. For more details on how to select these, and an
-example of Nvidia GPU, please see [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/
-PERFORMANCE_GUIDE.md) Please also see [PERFORMANCE.md](PERFORMANCE.md) ##
-Converting to GPX files ```shell venv/bin/gopro-to-gpx.py  [output-file] ``` ##
-Joining a sequence of MP4 files together Use the gopro-join.py command. Given a
-single file from the sequence, it will find and join together all the files. If
-you have any problems with this, please do raise an issue - I don't have that
-much test data. The joined file almost certainly won't work in the GoPro tools!
-- But it should work with `gopro-dashboard.py` - I will look into the
-additional technical stuff required to make it work in the GoPro tools. *This
-will require a lot of disk space!* ```shell venv/bin/gopro-join.py /media/
-sdcard/DCIM/100GOPRO/GH030170.MP4 /data/gopro/nice-ride.MP4 ``` ## Cutting a
-section from a GoPro file You can cut a section of the gopro file, with
-metadata. ## Related Software - https://github.com/julesgraus/
-interactiveGoProDashboardTool - An interactive helper to build the command line
-for the dashboard program ## Known Bugs / Issues - Only tested on a GoPro Hero
-9/11, that's all I have. Sample files for other devices are welcomed. ## Icons
-Icon files in [icons](gopro_overlay/icons) are not covered by the MIT licence
-## Map Data Data Â© [OpenStreetMap contributors](http://www.openstreetmap.org/
-copyright) Some Maps Â© [Thunderforest](http://www.thunderforest.com/) ##
-References https://github.com/juanmcasillas/gopro2gpx https://github.com/
-JuanIrache/gopro-telemetry https://github.com/gopro/gpmf-parser https://
-coderunner.io/how-to-compress-gopro-movies-and-keep-metadata/ ## Other Related
-Software https://github.com/progweb/gpx2video https://github.com/JuanIrache/
-gopro-telemetry ## Latest Changes If you find any issues with new releases,
-please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-
-dashboard-overlay/discussions) - 0.95.0 [Feature] Add api key support for
-geocode.xyz - [#117](https://github.com/time4tea/gopro-dashboard-overlay/
-issues/117) Thanks [@mishuha](https://github.com/mishuha) for raising. - 0.94.0
-[Change] Update docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature]
-Support for *fully gpu* decoding/overlay/encoding. Huge performance increase
-now possible. It takes a bit of work, but now can render at 12x realtime. See
-[docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking]
-Remove support for `--output-size` as it didn't really work properly anyway. -
-0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially
-much faster rendering, but may not work on all architectures. Speed
-improvements highly dependent on `ffmpeg` performance. Likely much faster when
-using `--generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data
-items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-
-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/
-patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now draws much more
-quickly. - [Change] Map rendering caches tile images more efficiently, so draws
-more quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` -
-A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-
-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0
-[Fix] Journey Map broke when no there were no locked GPS points in the movie. -
+timewarp modes - Support GPUs to create movies at up to 17x realtime - Convert
+GoPro movie metadata to GPX or CSV files - Cut sections from GoPro movies
+(including metadata) ## Examples ![Example Dashboard Image](examples/2022-05-
+15-example.png) ![Example Dashboard Image](examples/2022-06-11-contrib-
+example.png) ![Example Dashboard Image](examples/2022-07-19-contrib-example-
+plane.jpg) An Example of 'overlay only' mode, which generates movies from GPX
+files ![Example Dashboard Image](examples/2022-11-24-gpx-only-overlay.png)
+Example from [examples/layout](examples/layout) ![Example Dashboard Image]
+(examples/layout/layout-cairo-2704x1520.png) ## Map Styles Almost 30 different
+map styles are supported! - See [map styles](docs/maps/README.md) for more
+*Example* | . | . | . | . | |-------------------------------------|------------
+-----------------------------------|-------------------------------------------
+------------|-------------------------------------------------------| | ![osm]
+(docs/maps/map_style_osm.png) | ![tf-cycle](docs/maps/map_style_tf-cycle.png) |
+![tf-transport](docs/maps/map_style_tf-transport.png) | ![tf-landscape](docs/
+maps/map_style_tf-landscape.png) | ## Requirements - Python3.10 (development is
+done on Python3.11) - ffmpeg (you'll need the ffmpeg program installed) -
+libraqm (needed by [Pillow](https://pypi.org/project/Pillow/)) - Unixy machine
+(probably, untested on Windows) ## Installation Install locally using `pip`, or
+use the provided Docker image Optional: Some widgets require the `cairo`
+library - which must be installed separately. ### Installing and running with
+docker The docker image is a new thing and still a bit experimental... please
+file an issue if you find any problems. The docker image contains all you need
+to get started, and uses a volume `/work/`, which we suggest you map to the
+current directory which can contain your GoPro files. Note that the docker
+version doesn't support nvidia GPU extensions. The most recent version on
+docker is: [Docker] ```shell docker run -it -v "$(pwd):/work" overlaydash/
+gopro-dashboard-overlay:  [args...] ``` e.g. ```shell docker run -it -v "$
+(pwd):/work" overlaydash/gopro-dashboard-overlay:0.92.0 gopro-dashboard.py
+GH010122.MP4 render/docker.MP4 ``` Files created by the program will be created
+with the same uid that owns the mapped directory. You can use the `--cache-dir`
+and `--config-dir` command line arguments to configure where the cache and
+config dirs are, thereby making it easier to use persistent mapped volumes. ###
+Installing and running with pip ```shell python -m venv venv venv/bin/pip
+install gopro-overlay ``` The Roboto font needs to be installed on your system.
+You could install it with one of the following commands maybe. ```bash pacman -
+S ttf-roboto apt install truetype-roboto apt install fonts-roboto ``` ####
+(Optional) Installing pycairo Optionally, install `pycairo` ```shell venv/bin/
+pip install pycairo==1.23.0 ``` You might need to install some system libraries
+- This is what the pycairo docs suggest: Ubuntu/Debian: `sudo apt install
+libcairo2-dev pkg-config python3-dev` macOS/Homebrew: `brew install cairo pkg-
+config` ## Overlaying a dashboard ```shell venv/bin/gopro-dashboard.py ``` The
+GPS track in Hero 9 (at least) seems to be very poor. If you supply a GPX file
+from a Garmin or whatever, the program will use this instead for the GPS.
+Privacy allows you to set a privacy zone. Various widgets will not draw points
+within that zone. The data recorded in the GoPro video will uses GPS time,
+which (broadly) is UTC. The renderer will use your local timezone to interpret
+this, and use the local timezone. This may produce strange results if you go on
+holiday somewhere, but then render the files when you get back home! On linux
+you can use the TZ variable to change the timezone that's used. ### Example For
+full instructions on all command lines see [docs/bin](docs/bin) ```shell venv/
+bin/gopro-dashboard.py --gpx ~/Downloads/Morning_Ride.gpx --privacy 52.000,-
+0.40000,0.50 ~/gopro/GH020073.MP4 GH020073-dashboard.MP4 ``` ## Writeups
+There's a great writeup of how to use the software to make an overlay from a
+GPX file at https://blog.cubieserver.de/2022/creating-gpx-overlay-videos-on-
+linux/ (Nov 2022) ### Format of the Dashboard Configuration file Several
+dashboards are built-in to the software, but the dashboard layout is highly
+configurable, controlled by an XML file. For more information on the
+(extensive) configurability of the layout please see [docs/xml](docs/xml) and
+lots of [examples](docs/xml/examples/README.md) ## FFMPEG Control & GPUs
+*Experimental* FFMPEG has **a lot** of options! This program comes with some
+mostly sensible defaults, but to use GPUs and control the output much more
+carefully, including framerates and bitrates, you can use a JSON file
+containing a number of 'profiles' and select the profile you want when running
+the program. For more details on how to select these, and an example of Nvidia
+GPU, please see [docs/bin/PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md)
+Please also see [PERFORMANCE.md](PERFORMANCE.md) ## Converting to GPX files
+```shell venv/bin/gopro-to-gpx.py  [output-file] ``` ## Joining a sequence of
+MP4 files together Use the gopro-join.py command. Given a single file from the
+sequence, it will find and join together all the files. If you have any
+problems with this, please do raise an issue - I don't have that much test
+data. The joined file almost certainly won't work in the GoPro tools! - But it
+should work with `gopro-dashboard.py` - I will look into the additional
+technical stuff required to make it work in the GoPro tools. *This will require
+a lot of disk space!* ```shell venv/bin/gopro-join.py /media/sdcard/DCIM/
+100GOPRO/GH030170.MP4 /data/gopro/nice-ride.MP4 ``` ## Cutting a section from a
+GoPro file You can cut a section of the gopro file, with metadata. ## Related
+Software - https://github.com/julesgraus/interactiveGoProDashboardTool - An
+interactive helper to build the command line for the dashboard program ## Known
+Bugs / Issues - Only tested on a GoPro Hero 9/11, that's all I have. Sample
+files for other devices are welcomed. ## Icons Icon files in [icons]
+(gopro_overlay/icons) are not covered by the MIT licence ## Map Data Data Â©
+[OpenStreetMap contributors](http://www.openstreetmap.org/copyright) Some Maps
+Â© [Thunderforest](http://www.thunderforest.com/) ## References https://
+github.com/juanmcasillas/gopro2gpx https://github.com/JuanIrache/gopro-
+telemetry https://github.com/gopro/gpmf-parser https://coderunner.io/how-to-
+compress-gopro-movies-and-keep-metadata/ ## Other Related Software https://
+github.com/progweb/gpx2video https://github.com/JuanIrache/gopro-telemetry ##
+Latest Changes If you find any issues with new releases, please discuss in
+[GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/
+discussions) - 0.96.0 [Feature] Hopefully add support for older gopro files
+when joining. [#129](https://github.com/time4tea/gopro-dashboard-overlay/
+issues/129) Thanks [@FFMbyBicycle](https://github.com/FFMbyBicycle) for raising
+and some example code. - 0.95.0 [Feature] Add api key support for geocode.xyz -
+[#117](https://github.com/time4tea/gopro-dashboard-overlay/issues/117) Thanks
+[@mishuha](https://github.com/mishuha) for raising. - 0.94.0 [Change] Update
+docker image to python3.11/ffmpeg 6.0 - 0.93.0 [Feature] Support for *fully
+gpu* decoding/overlay/encoding. Huge performance increase now possible. It
+takes a bit of work, but now can render at 12x realtime. See [docs/bin/
+PERFORMANCE_GUIDE.md](docs/bin/PERFORMANCE_GUIDE.md) - [Breaking] Remove
+support for `--output-size` as it didn't really work properly anyway. - 0.92.0
+[Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much
+faster rendering, but may not work on all architectures. Speed improvements
+highly dependent on `ffmpeg` performance. Likely much faster when using `--
+generate overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that
+don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
+raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
+[Change] Map rendering caches tile images more efficiently, so draws more
+quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
+like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
+annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
+Journey Map broke when no there were no locked GPS points in the movie. -
 Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
 Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
 instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
 gauge-marker` - a nice clean gauge component, with a marker for the current
 value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
 06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
 attributes in layout files. This may cause some custom layouts to break! - But
```

### Comparing `gopro-overlay-0.95.0/gopro_overlay.egg-info/SOURCES.txt` & `gopro-overlay-0.96.0/gopro_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.95.0/setup.py` & `gopro-overlay-0.96.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 test_requirements = [
     "pytest"
 ]
 
 setup(
     name="gopro-overlay",
-    version="0.95.0",
+    version="0.96.0",
     description="Overlay graphics dashboards onto GoPro footage",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/time4tea/gopro-dashboard-overlay",
     author="James Richardson",
     author_email="james+gopro@time4tea.net",
     license="MIT",
```

