# Comparing `tmp/gopro-overlay-0.90.0.tar.gz` & `tmp/gopro-overlay-0.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopro-overlay-0.90.0.tar", last modified: Thu Feb  9 13:18:18 2023, max compression
+gzip compressed data, was "gopro-overlay-0.91.0.tar", last modified: Mon May  1 11:52:21 2023, max compression
```

## Comparing `gopro-overlay-0.90.0.tar` & `gopro-overlay-0.91.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.945474 gopro-overlay-0.90.0/
--rw-rw-r--   0 richja    (1000) richja    (1000)     2097 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/LICENSE.md
--rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.90.0/MANIFEST.in
--rw-rw-r--   0 richja    (1000) richja    (1000)    12972 2023-02-09 13:18:18.945474 gopro-overlay-0.90.0/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)    12159 2023-02-09 13:18:08.000000 gopro-overlay-0.90.0/README.md
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.929474 gopro-overlay-0.90.0/bin/
--rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.90.0/bin/gopro-contrib-data-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.90.0/bin/gopro-cut.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    14640 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/bin/gopro-dashboard.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/bin/gopro-debug.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.90.0/bin/gopro-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/bin/gopro-join.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)     5423 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/bin/gopro-layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3578 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/bin/gopro-rename.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/bin/gopro-to-csv.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/bin/gopro-to-gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.937474 gopro-overlay-0.90.0/gopro_overlay/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.90.0/gopro_overlay/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-02-09 13:16:57.000000 gopro-overlay-0.90.0/gopro_overlay/__version__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     7004 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/arguments.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.90.0/gopro_overlay/common.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/counter.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/date_overlap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.90.0/gopro_overlay/dimensions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/entry.py
--rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.90.0/gopro_overlay/exceptions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1296 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/execution.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/fake.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     9622 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/ffmpeg.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1031 2023-01-05 11:17:11.000000 gopro-overlay-0.90.0/gopro_overlay/ffmpeg_profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1803 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/filenaming.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2183 2022-11-29 16:08:05.000000 gopro-overlay-0.90.0/gopro_overlay/fit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.90.0/gopro_overlay/font.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/framemeta.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/framemeta_gpx.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.90.0/gopro_overlay/functional.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.90.0/gopro_overlay/geo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.90.0/gopro_overlay/geo_render.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      272 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/geocode.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2022-11-27 11:41:41.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd_calculate.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_cori.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_debug.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_grav.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_xyz.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.941474 gopro-overlay-0.90.0/gopro_overlay/icons/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.90.0/gopro_overlay/icons/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.90.0/gopro_overlay/icons/bicycle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.90.0/gopro_overlay/icons/car.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/icons/faq.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/icons/forbidden.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.90.0/gopro_overlay/icons/gauge-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.90.0/gopro_overlay/icons/gauge.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_2d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_3d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_none.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_unknown.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.90.0/gopro_overlay/icons/heartbeat.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.90.0/gopro_overlay/icons/ice-cream-van.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.90.0/gopro_overlay/icons/mountain-range.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.90.0/gopro_overlay/icons/mountain.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.90.0/gopro_overlay/icons/power.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.90.0/gopro_overlay/icons/ruler.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.90.0/gopro_overlay/icons/slope-triangle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.90.0/gopro_overlay/icons/slope.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.90.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.90.0/gopro_overlay/icons/thermometer-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.90.0/gopro_overlay/icons/thermometer.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.90.0/gopro_overlay/icons/user.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.90.0/gopro_overlay/icons/van-black-side-view.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/journey.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3366 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layout_components.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layout_xml.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layout_xml_attribute.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layout_xml_cairo.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.941474 gopro-overlay-0.90.0/gopro_overlay/layouts/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.90.0/gopro_overlay/layouts/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layouts/default-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layouts/default-2704x1520.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layouts/default-3840x2160.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layouts/example-2.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layouts/example.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/layouts/power-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/log.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.90.0/gopro_overlay/models.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.90.0/gopro_overlay/parsing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/point.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.90.0/gopro_overlay/privacy.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.90.0/gopro_overlay/progress_frames.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/rdp.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/smoothing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/timeseries.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/timeseries_process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.90.0/gopro_overlay/timeunits.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/timing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.90.0/gopro_overlay/units.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.941474 gopro-overlay-0.90.0/gopro_overlay/widgets/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/asi.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/bar.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.945474 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/angle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/annotation.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/background.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/bordered.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/box.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/cairo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/cap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/circuit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/colour.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/ellipse.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/face.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/gauge_marker.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/gauge_round_254.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/line.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/needle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/reading.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/scale.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/tick.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/chart.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/compass.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/compass_arrow.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/gradient_bar.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/info.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/map.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/text.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     7815 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/widgets.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.90.0/gopro_overlay/widgets/widgets_experimental.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-02-09 13:18:18.937474 gopro-overlay-0.90.0/gopro_overlay.egg-info/
--rw-rw-r--   0 richja    (1000) richja    (1000)    12972 2023-02-09 13:18:18.000000 gopro-overlay-0.90.0/gopro_overlay.egg-info/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)     4205 2023-02-09 13:18:18.000000 gopro-overlay-0.90.0/gopro_overlay.egg-info/SOURCES.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-02-09 13:18:18.000000 gopro-overlay-0.90.0/gopro_overlay.egg-info/dependency_links.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       20 2023-02-09 13:18:18.000000 gopro-overlay-0.90.0/gopro_overlay.egg-info/entry_points.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-02-09 13:18:18.000000 gopro-overlay-0.90.0/gopro_overlay.egg-info/requires.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-02-09 13:18:18.000000 gopro-overlay-0.90.0/gopro_overlay.egg-info/top_level.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-02-09 13:18:18.945474 gopro-overlay-0.90.0/setup.cfg
--rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-02-09 13:16:57.000000 gopro-overlay-0.90.0/setup.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2097 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/LICENSE.md
+-rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.91.0/MANIFEST.in
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11369 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10556 2023-05-01 11:51:58.000000 gopro-overlay-0.91.0/README.md
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.824821 gopro-overlay-0.91.0/bin/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.91.0/bin/gopro-contrib-data-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.91.0/bin/gopro-cut.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14774 2023-02-09 14:38:27.000000 gopro-overlay-0.91.0/bin/gopro-dashboard.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-debug.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.91.0/bin/gopro-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-join.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)     5501 2023-02-09 13:31:45.000000 gopro-overlay-0.91.0/bin/gopro-layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3578 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-rename.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-to-csv.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-to-gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.828821 gopro-overlay-0.91.0/gopro_overlay/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.91.0/gopro_overlay/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-01 11:49:17.000000 gopro-overlay-0.91.0/gopro_overlay/__version__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7004 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/arguments.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.91.0/gopro_overlay/common.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/counter.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/date_overlap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.91.0/gopro_overlay/dimensions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/entry.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.91.0/gopro_overlay/exceptions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1296 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/execution.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/fake.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9622 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/ffmpeg.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1031 2023-01-05 11:17:11.000000 gopro-overlay-0.91.0/gopro_overlay/ffmpeg_profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1803 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/filenaming.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:34:34.000000 gopro-overlay-0.91.0/gopro_overlay/fit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.91.0/gopro_overlay/font.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/framemeta.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/framemeta_gpx.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.91.0/gopro_overlay/functional.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.91.0/gopro_overlay/geo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.91.0/gopro_overlay/geo_render.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      272 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/geocode.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_calculate.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_cori.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_debug.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_grav.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_xyz.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.832821 gopro-overlay-0.91.0/gopro_overlay/icons/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.91.0/gopro_overlay/icons/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.91.0/gopro_overlay/icons/bicycle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.91.0/gopro_overlay/icons/car.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/faq.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/forbidden.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gauge-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gauge.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_2d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_3d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_none.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_unknown.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.91.0/gopro_overlay/icons/heartbeat.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.91.0/gopro_overlay/icons/ice-cream-van.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.91.0/gopro_overlay/icons/mountain-range.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.91.0/gopro_overlay/icons/mountain.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.91.0/gopro_overlay/icons/power.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.91.0/gopro_overlay/icons/ruler.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.91.0/gopro_overlay/icons/slope-triangle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.91.0/gopro_overlay/icons/slope.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.91.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/thermometer-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.91.0/gopro_overlay/icons/thermometer.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.91.0/gopro_overlay/icons/user.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.91.0/gopro_overlay/icons/van-black-side-view.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/journey.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3341 2023-02-09 13:31:45.000000 gopro-overlay-0.91.0/gopro_overlay/layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_components.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_xml.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_xml_attribute.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_xml_cairo.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/gopro_overlay/layouts/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/default-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/default-2704x1520.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/default-3840x2160.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/example-2.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/example.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/power-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/log.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.91.0/gopro_overlay/models.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.91.0/gopro_overlay/parsing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/point.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.91.0/gopro_overlay/privacy.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.91.0/gopro_overlay/progress_frames.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/rdp.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/smoothing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/timeseries.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/timeseries_process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.91.0/gopro_overlay/timeunits.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/timing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.91.0/gopro_overlay/units.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/gopro_overlay/widgets/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/asi.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/bar.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/angle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/annotation.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/background.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/bordered.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/box.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cairo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/circuit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/colour.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/ellipse.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/face.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_marker.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_round_254.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/line.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/needle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/reading.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/scale.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/tick.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/chart.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/compass.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/compass_arrow.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/gradient_bar.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/info.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/map.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/text.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8111 2023-02-09 13:31:45.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/widgets.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/widgets_experimental.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.828821 gopro-overlay-0.91.0/gopro_overlay.egg-info/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11369 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4205 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/SOURCES.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/dependency_links.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       20 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/entry_points.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/requires.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/top_level.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/setup.cfg
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-01 11:49:17.000000 gopro-overlay-0.91.0/setup.py
```

### Comparing `gopro-overlay-0.90.0/LICENSE.md` & `gopro-overlay-0.91.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/PKG-INFO` & `gopro-overlay-0.91.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.90.0
+Version: 0.91.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Platform: UNKNOWN
@@ -233,15 +233,16 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
-- 0.90.8 [Change] `cairo-circuit` now draws much more quickly. 
+- 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
+- 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
 - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated)
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
 - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean gauge component, with a marker for the current value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker)
 - 0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout files. This may cause some custom layouts to break! - But they wouldn't have been working as intended.
@@ -251,29 +252,12 @@
   - Many thanks to [@jchinte](https://github.com/jchinte) for contributing!
 - 0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but supplying input video
   - [Fix] Give better error message when video and GPX don't overlap in time, but told to sync 
   - Thanks to [@mfloryan](https://github.com/mfloryan) for reporting both of these
 - 0.82.0 [Change] Support for changing units in layouts from the command line. Use `--units-speed` etc to control. Examples are in [docs/bin](docs/bin)
   - Thanks to [@matzeruegge](https://github.com/matzeruegge) for the suggestion.
 - 0.81.0 [Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for reporting 
-- 0.80.0 [Fix] Use speeds from GPX file, in preference to GoPro file, when using GPX and GoPro together.
-  - [Change] Bump Required python version to 3.10
-- 0.79.0 [Fix] Changed GPS filtering reporting, it was a bit off.
-- 0.78.0 [Fix] Gradient calculation had become disabled.
-  - [Feature] Can now filter GPS points by max DOP `--gps-dop-max`
-  - [Feature] Can now filter GPS points by max Speed `--gps-speed-max` `--gps-speed-max-units`
-  - [Feature] Can now filter GPS points by bounding box - Useful if a few points claim to be locked, but are far away. Load GPX file into mapping software to see bounding box easily, for now. `--gps-bbox-lon-lat`
-  - [Change] Outputs except for generated files are now to stderr rather than stdout
-  - [Feature] `gopro-to-csv.py` and `gopro-to-gpx.py` now support `--only-locked` and `--every` to limit number of points (also GPS point filters, as above)
-  - [Change] Change in the way chart handles missing values - stops chart going to 0.
-  - Updated various library dependency versions.
-- 0.77.0 [Change] Disable speed and other calculations when GPS is not locked - stops unbelievable values
-  - [Change] changes to GPS parsing, should make detection of GPS lock more accurate (some 'not locked' values used to be included) still not perfect h/t [@falumas](https://github.com/falumas)
-  - [Change] add new widget "gps-lock-icon" at top of screen to show GPS lock - hopefully not too intrusive - can switch off with `--exclude`
-  - [Change] interpolate GPX/FIT tracks so they update every 0.1s - h/t [@0x10](https://github.com/0x10)
-- 0.76.0 [New Feature] New widget - "cairo_circuit_map" - Much nicer looking circuit map, and first widget that uses new optional "cairo" library.
-  - See examples [Cairo Circuit Map](docs/xml/examples/06-cairo-circuit-map/README.md)
 
 Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.90.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.91.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -97,60 +97,40 @@
 www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
 www.thunderforest.com/) ## References https://github.com/juanmcasillas/
 gopro2gpx https://github.com/JuanIrache/gopro-telemetry https://github.com/
 gopro/gpmf-parser https://coderunner.io/how-to-compress-gopro-movies-and-keep-
 metadata/ ## Other Related Software https://github.com/progweb/gpx2video https:
 //github.com/JuanIrache/gopro-telemetry ## Latest Changes If you find any
 issues with new releases, please discuss in [GitHub Discussions](https://
-github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.90.8 [Change]
-`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
-tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
-component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
-docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
-cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
-were no locked GPS points in the movie. - Thanks [@shahargli](https://
-github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
-discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
-colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
-gauge component, with a marker for the current value.. See docs [docs/xml/
-examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
-0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
-files. This may cause some custom layouts to break! - But they wouldn't have
-been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
-names, aiming for standardisation - [Change/Breaking] Change some `cairo-
-circuit-map` attribute names, aiming for standardisation - 0.84.0 [Feature] New
-component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/
-Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-
-zone-bar) - Many thanks to [@jchinte](https://github.com/jchinte) for
-contributing! - 0.83.0 [Change] No longer require --overlay-size when using --
-use-gpx-only, but supplying input video - [Fix] Give better error message when
-video and GPX don't overlap in time, but told to sync - Thanks to [@mfloryan]
-(https://github.com/mfloryan) for reporting both of these - 0.82.0 [Change]
-Support for changing units in layouts from the command line. Use `--units-
-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
-[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
-[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
-won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
-reporting - 0.80.0 [Fix] Use speeds from GPX file, in preference to GoPro file,
-when using GPX and GoPro together. - [Change] Bump Required python version to
-3.10 - 0.79.0 [Fix] Changed GPS filtering reporting, it was a bit off. - 0.78.0
-[Fix] Gradient calculation had become disabled. - [Feature] Can now filter GPS
-points by max DOP `--gps-dop-max` - [Feature] Can now filter GPS points by max
-Speed `--gps-speed-max` `--gps-speed-max-units` - [Feature] Can now filter GPS
-points by bounding box - Useful if a few points claim to be locked, but are far
-away. Load GPX file into mapping software to see bounding box easily, for now.
-`--gps-bbox-lon-lat` - [Change] Outputs except for generated files are now to
-stderr rather than stdout - [Feature] `gopro-to-csv.py` and `gopro-to-gpx.py`
-now support `--only-locked` and `--every` to limit number of points (also GPS
-point filters, as above) - [Change] Change in the way chart handles missing
-values - stops chart going to 0. - Updated various library dependency versions.
-- 0.77.0 [Change] Disable speed and other calculations when GPS is not locked -
-stops unbelievable values - [Change] changes to GPS parsing, should make
-detection of GPS lock more accurate (some 'not locked' values used to be
-included) still not perfect h/t [@falumas](https://github.com/falumas) -
-[Change] add new widget "gps-lock-icon" at top of screen to show GPS lock -
-hopefully not too intrusive - can switch off with `--exclude` - [Change]
-interpolate GPX/FIT tracks so they update every 0.1s - h/t [@0x10](https://
-github.com/0x10) - 0.76.0 [New Feature] New widget - "cairo_circuit_map" - Much
-nicer looking circuit map, and first widget that uses new optional "cairo"
-library. - See examples [Cairo Circuit Map](docs/xml/examples/06-cairo-circuit-
-map/README.md) Older changes are in [CHANGELOG.md](CHANGELOG.md)
+github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.91.0 [Fix] Ignore
+FIT data items that don't have a GPS location. [#122](https://github.com/
+time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://
+github.com/patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now
+draws much more quickly. - [Change] Map rendering caches tile images more
+efficiently, so draws more quickly. - 0.89.0 [Feature] New component `cairo-
+gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/
+examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-
+round-annotated) - 0.88.0 [Fix] Journey Map broke when no there were no locked
+GPS points in the movie. - Thanks [@shahargli](https://github.com/shahargli)
+for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs,
+now fixed. Removed `alpha`, instead use alpha of each colour. - 0.86.0
+[Feature] New component `cairo-gauge-marker` - a nice clean gauge component,
+with a marker for the current value.. See docs [docs/xml/examples/06-cairo-
+gauge-marker](docs/xml/examples/06-cairo-gauge-marker) - 0.85.0 [Feature/
+Breaking Possibly] Add validation to attributes in layout files. This may cause
+some custom layouts to break! - But they wouldn't have been working as
+intended. - [Change/Breaking] Change some `zone-bar` attribute names, aiming
+for standardisation - [Change/Breaking] Change some `cairo-circuit-map`
+attribute names, aiming for standardisation - 0.84.0 [Feature] New component
+`zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones.
+See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar) -
+Many thanks to [@jchinte](https://github.com/jchinte) for contributing! -
+0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but
+supplying input video - [Fix] Give better error message when video and GPX
+don't overlap in time, but told to sync - Thanks to [@mfloryan](https://
+github.com/mfloryan) for reporting both of these - 0.82.0 [Change] Support for
+changing units in layouts from the command line. Use `--units-speed` etc to
+control. Examples are in [docs/bin](docs/bin) - Thanks to [@matzeruegge](https:
+//github.com/matzeruegge) for the suggestion. - 0.81.0 [Fix] gopro-rename was
+broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to
+[matzeruegge](https://github.com/matzeruegge) for reporting Older changes are
+in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.90.0/README.md` & `gopro-overlay-0.91.0/gopro_overlay.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: gopro-overlay
+Version: 0.91.0
+Summary: Overlay graphics dashboards onto GoPro footage
+Home-page: https://github.com/time4tea/gopro-dashboard-overlay
+Author: James Richardson
+Author-email: james+gopro@time4tea.net
+License: MIT
+Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Environment :: Console
+Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Video
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # Create video overlays from GoPro Videos or any GPX/FIT file
 
 <a href="https://github.com/time4tea/gopro-dashboard-overlay/discussions"><img alt="GitHub Discussions" src="https://img.shields.io/github/discussions/time4tea/gopro-dashboard-overlay?style=for-the-badge"></a>
 <a href="https://pypi.org/project/gopro-overlay/"><img alt="PyPI" src="https://img.shields.io/pypi/v/gopro-overlay?style=for-the-badge"></a>
 <a href="https://hub.docker.com/r/overlaydash/gopro-dashboard-overlay"><img alt="Docker" src="https://img.shields.io/docker/v/overlaydash/gopro-dashboard-overlay?label=Docker&style=for-the-badge"></a>
 
 Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
@@ -211,15 +233,16 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
-- 0.90.8 [Change] `cairo-circuit` now draws much more quickly. 
+- 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
+- 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
 - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated)
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
 - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean gauge component, with a marker for the current value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker)
 - 0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout files. This may cause some custom layouts to break! - But they wouldn't have been working as intended.
@@ -229,27 +252,12 @@
   - Many thanks to [@jchinte](https://github.com/jchinte) for contributing!
 - 0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but supplying input video
   - [Fix] Give better error message when video and GPX don't overlap in time, but told to sync 
   - Thanks to [@mfloryan](https://github.com/mfloryan) for reporting both of these
 - 0.82.0 [Change] Support for changing units in layouts from the command line. Use `--units-speed` etc to control. Examples are in [docs/bin](docs/bin)
   - Thanks to [@matzeruegge](https://github.com/matzeruegge) for the suggestion.
 - 0.81.0 [Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for reporting 
-- 0.80.0 [Fix] Use speeds from GPX file, in preference to GoPro file, when using GPX and GoPro together.
-  - [Change] Bump Required python version to 3.10
-- 0.79.0 [Fix] Changed GPS filtering reporting, it was a bit off.
-- 0.78.0 [Fix] Gradient calculation had become disabled.
-  - [Feature] Can now filter GPS points by max DOP `--gps-dop-max`
-  - [Feature] Can now filter GPS points by max Speed `--gps-speed-max` `--gps-speed-max-units`
-  - [Feature] Can now filter GPS points by bounding box - Useful if a few points claim to be locked, but are far away. Load GPX file into mapping software to see bounding box easily, for now. `--gps-bbox-lon-lat`
-  - [Change] Outputs except for generated files are now to stderr rather than stdout
-  - [Feature] `gopro-to-csv.py` and `gopro-to-gpx.py` now support `--only-locked` and `--every` to limit number of points (also GPS point filters, as above)
-  - [Change] Change in the way chart handles missing values - stops chart going to 0.
-  - Updated various library dependency versions.
-- 0.77.0 [Change] Disable speed and other calculations when GPS is not locked - stops unbelievable values
-  - [Change] changes to GPS parsing, should make detection of GPS lock more accurate (some 'not locked' values used to be included) still not perfect h/t [@falumas](https://github.com/falumas)
-  - [Change] add new widget "gps-lock-icon" at top of screen to show GPS lock - hopefully not too intrusive - can switch off with `--exclude`
-  - [Change] interpolate GPX/FIT tracks so they update every 0.1s - h/t [@0x10](https://github.com/0x10)
-- 0.76.0 [New Feature] New widget - "cairo_circuit_map" - Much nicer looking circuit map, and first widget that uses new optional "cairo" library.
-  - See examples [Cairo Circuit Map](docs/xml/examples/06-cairo-circuit-map/README.md)
 
 Older changes are in [CHANGELOG.md](CHANGELOG.md)
 
+
+
```

#### html2text {}

```diff
@@ -1,34 +1,45 @@
-# Create video overlays from GoPro Videos or any GPX/FIT file [GitHub
-Discussions] [PyPI] [Docker] Discuss on [GitHub Discussions](https://
-github.com/time4tea/gopro-dashboard-overlay/discussions) - Overlaying exciting
-graphics onto GoPro videos with super-exact synchronization - *NEW &
-EXPERIMENTAL* Create videos from any GPX file - no GoPro required - Support
-multiple resolutions, most GoPro models, normal, timelapse & timewarp modes -
-Convert GoPro movie metadata to GPX or CSV files - Cut sections from GoPro
-movies (including metadata) ## Examples ![Example Dashboard Image](examples/
-2022-05-15-example.png) ![Example Dashboard Image](examples/2022-06-11-contrib-
-example.png) ![Example Dashboard Image](examples/2022-07-19-contrib-example-
-plane.jpg) An Example of 'overlay only' mode, which generates movies from GPX
-files ![Example Dashboard Image](examples/2022-11-24-gpx-only-overlay.png)
-Example from [examples/layout](examples/layout) ![Example Dashboard Image]
-(examples/layout/layout-cairo-2704x1520.png) ## Map Styles Almost 30 different
-map styles are supported! - See [map styles](docs/maps/README.md) for more
-*Example* | . | . | . | . | |-------------------------------------|------------
------------------------------------|-------------------------------------------
-------------|-------------------------------------------------------| | ![osm]
-(docs/maps/map_style_osm.png) | ![tf-cycle](docs/maps/map_style_tf-cycle.png) |
-![tf-transport](docs/maps/map_style_tf-transport.png) | ![tf-landscape](docs/
-maps/map_style_tf-landscape.png) | ## Requirements - Python3.10 - ffmpeg
-(you'll need the ffmpeg program installed) - Unixy machine (probably, untested
-on Windows) ## Installation Install locally using `pip`, or use the provided
-Docker image Optional: Some widgets require the `cairo` library - which must be
-installed separately. ### Installing and running with docker The docker image
-is a new thing and still a bit experimental... please file an issue if you find
-any problems. The docker image contains all you need to get started, and uses a
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.91.0 Summary: Overlay
+graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
+gopro-dashboard-overlay Author: James Richardson Author-email:
+james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
+time4tea/gopro-dashboard-overlay Platform: UNKNOWN Classifier: Development
+Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
+License Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
+Classifier: Environment :: Console Classifier: Topic :: Multimedia :: Graphics
+Classifier: Topic :: Multimedia :: Video Requires-Python: >=3.10 Description-
+Content-Type: text/markdown License-File: LICENSE.md # Create video overlays
+from GoPro Videos or any GPX/FIT file [GitHub_Discussions] [PyPI] [Docker]
+Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-
+overlay/discussions) - Overlaying exciting graphics onto GoPro videos with
+super-exact synchronization - *NEW & EXPERIMENTAL* Create videos from any GPX
+file - no GoPro required - Support multiple resolutions, most GoPro models,
+normal, timelapse & timewarp modes - Convert GoPro movie metadata to GPX or CSV
+files - Cut sections from GoPro movies (including metadata) ## Examples !
+[Example Dashboard Image](examples/2022-05-15-example.png) ![Example Dashboard
+Image](examples/2022-06-11-contrib-example.png) ![Example Dashboard Image]
+(examples/2022-07-19-contrib-example-plane.jpg) An Example of 'overlay only'
+mode, which generates movies from GPX files ![Example Dashboard Image]
+(examples/2022-11-24-gpx-only-overlay.png) Example from [examples/layout]
+(examples/layout) ![Example Dashboard Image](examples/layout/layout-cairo-
+2704x1520.png) ## Map Styles Almost 30 different map styles are supported! -
+See [map styles](docs/maps/README.md) for more *Example* | . | . | . | . | |---
+----------------------------------|--------------------------------------------
+---|-------------------------------------------------------|-------------------
+------------------------------------| | ![osm](docs/maps/map_style_osm.png) | !
+[tf-cycle](docs/maps/map_style_tf-cycle.png) | ![tf-transport](docs/maps/
+map_style_tf-transport.png) | ![tf-landscape](docs/maps/map_style_tf-
+landscape.png) | ## Requirements - Python3.10 - ffmpeg (you'll need the ffmpeg
+program installed) - Unixy machine (probably, untested on Windows) ##
+Installation Install locally using `pip`, or use the provided Docker image
+Optional: Some widgets require the `cairo` library - which must be installed
+separately. ### Installing and running with docker The docker image is a new
+thing and still a bit experimental... please file an issue if you find any
+problems. The docker image contains all you need to get started, and uses a
 volume `/work/`, which we suggest you map to the current directory which can
 contain your GoPro files. Note that the docker version doesn't support nvidia
 GPU extensions. The most recent version on docker is: [Docker] ```shell docker
 run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:  [args...] ```
 e.g. ```shell docker run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-
 overlay:0.81.0 gopro-dashboard.py GH010122.MP4 render/docker.MP4 ``` Files
 created by the program will be created with the same uid that owns the mapped
@@ -86,60 +97,40 @@
 www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
 www.thunderforest.com/) ## References https://github.com/juanmcasillas/
 gopro2gpx https://github.com/JuanIrache/gopro-telemetry https://github.com/
 gopro/gpmf-parser https://coderunner.io/how-to-compress-gopro-movies-and-keep-
 metadata/ ## Other Related Software https://github.com/progweb/gpx2video https:
 //github.com/JuanIrache/gopro-telemetry ## Latest Changes If you find any
 issues with new releases, please discuss in [GitHub Discussions](https://
-github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.90.8 [Change]
-`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
-tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
-component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
-docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
-cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
-were no locked GPS points in the movie. - Thanks [@shahargli](https://
-github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
-discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
-colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
-gauge component, with a marker for the current value.. See docs [docs/xml/
-examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
-0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
-files. This may cause some custom layouts to break! - But they wouldn't have
-been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
-names, aiming for standardisation - [Change/Breaking] Change some `cairo-
-circuit-map` attribute names, aiming for standardisation - 0.84.0 [Feature] New
-component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/
-Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-
-zone-bar) - Many thanks to [@jchinte](https://github.com/jchinte) for
-contributing! - 0.83.0 [Change] No longer require --overlay-size when using --
-use-gpx-only, but supplying input video - [Fix] Give better error message when
-video and GPX don't overlap in time, but told to sync - Thanks to [@mfloryan]
-(https://github.com/mfloryan) for reporting both of these - 0.82.0 [Change]
-Support for changing units in layouts from the command line. Use `--units-
-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
-[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
-[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
-won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
-reporting - 0.80.0 [Fix] Use speeds from GPX file, in preference to GoPro file,
-when using GPX and GoPro together. - [Change] Bump Required python version to
-3.10 - 0.79.0 [Fix] Changed GPS filtering reporting, it was a bit off. - 0.78.0
-[Fix] Gradient calculation had become disabled. - [Feature] Can now filter GPS
-points by max DOP `--gps-dop-max` - [Feature] Can now filter GPS points by max
-Speed `--gps-speed-max` `--gps-speed-max-units` - [Feature] Can now filter GPS
-points by bounding box - Useful if a few points claim to be locked, but are far
-away. Load GPX file into mapping software to see bounding box easily, for now.
-`--gps-bbox-lon-lat` - [Change] Outputs except for generated files are now to
-stderr rather than stdout - [Feature] `gopro-to-csv.py` and `gopro-to-gpx.py`
-now support `--only-locked` and `--every` to limit number of points (also GPS
-point filters, as above) - [Change] Change in the way chart handles missing
-values - stops chart going to 0. - Updated various library dependency versions.
-- 0.77.0 [Change] Disable speed and other calculations when GPS is not locked -
-stops unbelievable values - [Change] changes to GPS parsing, should make
-detection of GPS lock more accurate (some 'not locked' values used to be
-included) still not perfect h/t [@falumas](https://github.com/falumas) -
-[Change] add new widget "gps-lock-icon" at top of screen to show GPS lock -
-hopefully not too intrusive - can switch off with `--exclude` - [Change]
-interpolate GPX/FIT tracks so they update every 0.1s - h/t [@0x10](https://
-github.com/0x10) - 0.76.0 [New Feature] New widget - "cairo_circuit_map" - Much
-nicer looking circuit map, and first widget that uses new optional "cairo"
-library. - See examples [Cairo Circuit Map](docs/xml/examples/06-cairo-circuit-
-map/README.md) Older changes are in [CHANGELOG.md](CHANGELOG.md)
+github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.91.0 [Fix] Ignore
+FIT data items that don't have a GPS location. [#122](https://github.com/
+time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://
+github.com/patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now
+draws much more quickly. - [Change] Map rendering caches tile images more
+efficiently, so draws more quickly. - 0.89.0 [Feature] New component `cairo-
+gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/
+examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-
+round-annotated) - 0.88.0 [Fix] Journey Map broke when no there were no locked
+GPS points in the movie. - Thanks [@shahargli](https://github.com/shahargli)
+for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs,
+now fixed. Removed `alpha`, instead use alpha of each colour. - 0.86.0
+[Feature] New component `cairo-gauge-marker` - a nice clean gauge component,
+with a marker for the current value.. See docs [docs/xml/examples/06-cairo-
+gauge-marker](docs/xml/examples/06-cairo-gauge-marker) - 0.85.0 [Feature/
+Breaking Possibly] Add validation to attributes in layout files. This may cause
+some custom layouts to break! - But they wouldn't have been working as
+intended. - [Change/Breaking] Change some `zone-bar` attribute names, aiming
+for standardisation - [Change/Breaking] Change some `cairo-circuit-map`
+attribute names, aiming for standardisation - 0.84.0 [Feature] New component
+`zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones.
+See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar) -
+Many thanks to [@jchinte](https://github.com/jchinte) for contributing! -
+0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but
+supplying input video - [Fix] Give better error message when video and GPX
+don't overlap in time, but told to sync - Thanks to [@mfloryan](https://
+github.com/mfloryan) for reporting both of these - 0.82.0 [Change] Support for
+changing units in layouts from the command line. Use `--units-speed` etc to
+control. Examples are in [docs/bin](docs/bin) - Thanks to [@matzeruegge](https:
+//github.com/matzeruegge) for the suggestion. - 0.81.0 [Fix] gopro-rename was
+broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to
+[matzeruegge](https://github.com/matzeruegge) for reporting Older changes are
+in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.90.0/bin/gopro-contrib-data-extract.py` & `gopro-overlay-0.91.0/bin/gopro-contrib-data-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/bin/gopro-cut.py` & `gopro-overlay-0.91.0/bin/gopro-cut.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/bin/gopro-dashboard.py` & `gopro-overlay-0.91.0/bin/gopro-dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from gopro_overlay.point import Point
 from gopro_overlay.privacy import PrivacyZone, NoPrivacyZone
 from gopro_overlay.timeseries import Timeseries
 from gopro_overlay.timeunits import timeunits, Timeunit
 from gopro_overlay.timing import PoorTimer
 from gopro_overlay.units import units
 from gopro_overlay.widgets.profile import WidgetProfiler
+from gopro_overlay.widgets.widgets import SimpleFrameSupplier
 
 
 def accepter_from_args(include, exclude):
     if include and exclude:
         raise ValueError("Can't use both include and exclude at the same time")
 
     if include:
@@ -303,16 +304,18 @@
             unit_converters = Converters(
                 speed_unit=args.units_speed,
                 distance_unit=args.units_distance,
                 altitude_unit=args.units_altitude,
                 temperature_unit=args.units_temperature,
             )
 
+            frame_supplier = SimpleFrameSupplier(dimensions=dimensions)
+
             overlay = Overlay(
-                dimensions=dimensions,
+                frame=frame_supplier,
                 framemeta=frame_meta,
                 create_widgets=create_desired_layout(
                     layout=args.layout, layout_xml=args.layout_xml,
                     dimensions=dimensions,
                     include=args.include, exclude=args.exclude,
                     renderer=renderer,
                     timeseries=frame_meta,
```

### Comparing `gopro-overlay-0.90.0/bin/gopro-debug.py` & `gopro-overlay-0.91.0/bin/gopro-debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/bin/gopro-extract.py` & `gopro-overlay-0.91.0/bin/gopro-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/bin/gopro-join.py` & `gopro-overlay-0.91.0/bin/gopro-join.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/bin/gopro-layout.py` & `gopro-overlay-0.91.0/bin/gopro-layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from gopro_overlay.geo import CachingRenderer, api_key_finder
 from gopro_overlay.layout import Overlay
 from gopro_overlay.layout_xml import layout_from_xml, load_xml_layout
 from gopro_overlay.log import log
 from gopro_overlay.privacy import NoPrivacyZone
 from gopro_overlay.timeunits import timeunits
 from gopro_overlay.units import units
+from gopro_overlay.widgets.widgets import SimpleFrameSupplier
 
 
 def load_frame(filepath: pathlib.Path, size: Dimension, at_time=timeunits(seconds=2)):
     return Image.frombytes(mode="RGBA", size=size.tuple(), data=ffmpeg.load_frame(filepath, at_time))
 
 
 if __name__ == "__main__":
@@ -114,15 +115,15 @@
                 if updated != last_updated:
                     last_updated = updated
 
                     try:
                         layout = layout_from_xml(load_xml_layout(args.file), renderer, timeseries, font, NoPrivacyZone())
 
                         overlay = Overlay(
-                            dimensions=dimension_from(args.overlay_size),
+                            frame=SimpleFrameSupplier(dimension_from(args.overlay_size)),
                             framemeta=timeseries,
                             create_widgets=layout
                         )
 
                         frame = overlay.draw(timeseries.mid)
 
                         if video_frame is not None:
```

### Comparing `gopro-overlay-0.90.0/bin/gopro-rename.py` & `gopro-overlay-0.91.0/bin/gopro-rename.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/bin/gopro-to-csv.py` & `gopro-overlay-0.91.0/bin/gopro-to-csv.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/bin/gopro-to-gpx.py` & `gopro-overlay-0.91.0/bin/gopro-to-gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/arguments.py` & `gopro-overlay-0.91.0/gopro_overlay/arguments.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/common.py` & `gopro-overlay-0.91.0/gopro_overlay/common.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/dimensions.py` & `gopro-overlay-0.91.0/gopro_overlay/dimensions.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/entry.py` & `gopro-overlay-0.91.0/gopro_overlay/entry.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/execution.py` & `gopro-overlay-0.91.0/gopro_overlay/execution.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/fake.py` & `gopro-overlay-0.91.0/gopro_overlay/fake.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/ffmpeg.py` & `gopro-overlay-0.91.0/gopro_overlay/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/ffmpeg_profile.py` & `gopro-overlay-0.91.0/gopro_overlay/ffmpeg_profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/filenaming.py` & `gopro-overlay-0.91.0/gopro_overlay/filenaming.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/fit.py` & `gopro-overlay-0.91.0/gopro_overlay/fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,12 +49,13 @@
                         items.update(**interpret[field.name](field, units))
 
             if "lat" in items and "lon" in items:
                 items["point"] = Point(lat=items["lat"], lon=items["lon"])
                 del (items["lat"])
                 del (items["lon"])
 
-            entry.update(**items)
-
-            ts.add(entry)
+            # only use fit data items that have lat/lon
+            if "point" in items:
+                entry.update(**items)
+                ts.add(entry)
 
     return ts
```

### Comparing `gopro-overlay-0.90.0/gopro_overlay/framemeta.py` & `gopro-overlay-0.91.0/gopro_overlay/framemeta.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/framemeta_gpx.py` & `gopro-overlay-0.91.0/gopro_overlay/framemeta_gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/geo.py` & `gopro-overlay-0.91.0/gopro_overlay/geo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/geo_render.py` & `gopro-overlay-0.91.0/gopro_overlay/geo_render.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd_calculate.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd_calculate.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_cori.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_cori.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_debug.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_gps.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_grav.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_grav.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpmd_visitors_xyz.py` & `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_xyz.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/gpx.py` & `gopro-overlay-0.91.0/gopro_overlay/gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/bicycle.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/car.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/car.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/faq.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/faq.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/forbidden.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/forbidden.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/gauge-1.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/gauge-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/gauge.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/gauge.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_2d.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_2d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_3d.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_3d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_none.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_none.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/gps_lock_unknown.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_unknown.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/heartbeat.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/heartbeat.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/ice-cream-van.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/ice-cream-van.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/mountain-range.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/mountain-range.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/mountain.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/mountain.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/power.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/power.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/ruler.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/ruler.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/slope-triangle.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/slope-triangle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/slope.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/slope.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/thermometer-1.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/thermometer-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/thermometer.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/thermometer.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/user.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/user.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/icons/van-black-side-view.png` & `gopro-overlay-0.91.0/gopro_overlay/icons/van-black-side-view.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/journey.py` & `gopro-overlay-0.91.0/gopro_overlay/journey.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layout.py` & `gopro-overlay-0.91.0/gopro_overlay/layout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Callable
 
 from PIL import ImageFont, Image, ImageDraw
 
-from .dimensions import Dimension
+from gopro_overlay.widgets.info import ComparativeEnergy
 from .framemeta import FrameMeta
 from .layout_components import moving_map
 from .point import Coordinate
 from .units import units
-from .widgets.widgets import Scene, Translate, Composite, Widget
 from .widgets.text import CachingText, Text
-from gopro_overlay.widgets.info import ComparativeEnergy
+from .widgets.widgets import Scene, Translate, Composite, Widget, FrameSupplier
 
 
 def gps_info(at, entry, font):
     return Composite(
         CachingText(at + Coordinate(0, 0), lambda: "GPS INFO", font, align="right"),
         Text(at + Coordinate(-130, 24), lambda: f"Lat: {entry().point.lat:0.6f}", font, align="right"),
         Text(at + Coordinate(0, 24), lambda: f"Lon: {entry().point.lon:0.6f}", font, align="right"),
@@ -89,16 +88,16 @@
         ]
 
     return create
 
 
 class Overlay:
 
-    def __init__(self, dimensions: Dimension, framemeta: FrameMeta, create_widgets: Callable):
-        self.scene = Scene(dimensions, create_widgets(self.entry))
+    def __init__(self, frame: FrameSupplier, framemeta: FrameMeta, create_widgets: Callable):
+        self.scene = Scene(frame, create_widgets(self.entry))
         self.framemeta = framemeta
         self._entry = None
 
     def entry(self):
         return self._entry
 
     def draw(self, pts) -> Image.Image:
```

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layout_components.py` & `gopro-overlay-0.91.0/gopro_overlay/layout_components.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layout_xml.py` & `gopro-overlay-0.91.0/gopro_overlay/layout_xml.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layout_xml_attribute.py` & `gopro-overlay-0.91.0/gopro_overlay/layout_xml_attribute.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layout_xml_cairo.py` & `gopro-overlay-0.91.0/gopro_overlay/layout_xml_cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layouts/default-1920x1080.xml` & `gopro-overlay-0.91.0/gopro_overlay/layouts/default-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layouts/default-2704x1520.xml` & `gopro-overlay-0.91.0/gopro_overlay/layouts/default-2704x1520.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layouts/default-3840x2160.xml` & `gopro-overlay-0.91.0/gopro_overlay/layouts/default-3840x2160.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layouts/example-2.xml` & `gopro-overlay-0.91.0/gopro_overlay/layouts/example-2.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layouts/example.xml` & `gopro-overlay-0.91.0/gopro_overlay/layouts/example.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/layouts/power-1920x1080.xml` & `gopro-overlay-0.91.0/gopro_overlay/layouts/power-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/models.py` & `gopro-overlay-0.91.0/gopro_overlay/models.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/point.py` & `gopro-overlay-0.91.0/gopro_overlay/point.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/privacy.py` & `gopro-overlay-0.91.0/gopro_overlay/privacy.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/progress_frames.py` & `gopro-overlay-0.91.0/gopro_overlay/progress_frames.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/rdp.py` & `gopro-overlay-0.91.0/gopro_overlay/rdp.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/smoothing.py` & `gopro-overlay-0.91.0/gopro_overlay/smoothing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/timeseries.py` & `gopro-overlay-0.91.0/gopro_overlay/timeseries.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/timeseries_process.py` & `gopro-overlay-0.91.0/gopro_overlay/timeseries_process.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/timeunits.py` & `gopro-overlay-0.91.0/gopro_overlay/timeunits.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/timing.py` & `gopro-overlay-0.91.0/gopro_overlay/timing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/asi.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/asi.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/bar.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/angle.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/angle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/annotation.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/annotation.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/background.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/background.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/bordered.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/bordered.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/cairo.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/cap.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cap.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/circuit.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/circuit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/colour.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/colour.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/ellipse.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/ellipse.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/face.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/face.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/gauge_marker.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_marker.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/gauge_round_254.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_round_254.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/needle.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/needle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/reading.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/reading.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/cairo/scale.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/scale.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/chart.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/chart.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/compass.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/compass.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/compass_arrow.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/compass_arrow.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/gps.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/gradient_bar.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/gradient_bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/info.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/info.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/map.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/map.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/profile.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/text.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/text.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/widgets.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,21 +218,35 @@
             )
 
         rect.putalpha(self.mask)
 
         image.alpha_composite(rect, (0, 0))
 
 
+class FrameSupplier:
+    def drawing_frame(self) -> Image:
+        raise NotImplementedError()
+
+
+class SimpleFrameSupplier(FrameSupplier):
+
+    def __init__(self, dimensions: Dimension):
+        self._dimensions = dimensions
+
+    def drawing_frame(self) -> Image:
+        return Image.new("RGBA", (self._dimensions.x, self._dimensions.y), (0, 0, 0, 0))
+
+
 class Scene:
 
-    def __init__(self, dimensions: Dimension, widgets: List[Widget]):
+    def __init__(self, frame: FrameSupplier, widgets: List[Widget]):
         self._widgets = widgets
-        self._dimensions = dimensions
+        self.frame = frame
 
     def draw(self) -> Image.Image:
-        image = Image.new("RGBA", (self._dimensions.x, self._dimensions.y), (0, 0, 0, 0))
+        image = self.frame.drawing_frame()
         draw = ImageDraw.Draw(image)
 
         for w in self._widgets:
             w.draw(image, draw)
 
         return image
```

### Comparing `gopro-overlay-0.90.0/gopro_overlay/widgets/widgets_experimental.py` & `gopro-overlay-0.91.0/gopro_overlay/widgets/widgets_experimental.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/gopro_overlay.egg-info/PKG-INFO` & `gopro-overlay-0.91.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: gopro-overlay
-Version: 0.90.0
-Summary: Overlay graphics dashboards onto GoPro footage
-Home-page: https://github.com/time4tea/gopro-dashboard-overlay
-Author: James Richardson
-Author-email: james+gopro@time4tea.net
-License: MIT
-Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Environment :: Console
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Video
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Create video overlays from GoPro Videos or any GPX/FIT file
 
 <a href="https://github.com/time4tea/gopro-dashboard-overlay/discussions"><img alt="GitHub Discussions" src="https://img.shields.io/github/discussions/time4tea/gopro-dashboard-overlay?style=for-the-badge"></a>
 <a href="https://pypi.org/project/gopro-overlay/"><img alt="PyPI" src="https://img.shields.io/pypi/v/gopro-overlay?style=for-the-badge"></a>
 <a href="https://hub.docker.com/r/overlaydash/gopro-dashboard-overlay"><img alt="Docker" src="https://img.shields.io/docker/v/overlaydash/gopro-dashboard-overlay?label=Docker&style=for-the-badge"></a>
 
 Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
@@ -233,15 +211,16 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
-- 0.90.8 [Change] `cairo-circuit` now draws much more quickly. 
+- 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
+- 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
 - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated)
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
 - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean gauge component, with a marker for the current value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker)
 - 0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout files. This may cause some custom layouts to break! - But they wouldn't have been working as intended.
@@ -251,29 +230,10 @@
   - Many thanks to [@jchinte](https://github.com/jchinte) for contributing!
 - 0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but supplying input video
   - [Fix] Give better error message when video and GPX don't overlap in time, but told to sync 
   - Thanks to [@mfloryan](https://github.com/mfloryan) for reporting both of these
 - 0.82.0 [Change] Support for changing units in layouts from the command line. Use `--units-speed` etc to control. Examples are in [docs/bin](docs/bin)
   - Thanks to [@matzeruegge](https://github.com/matzeruegge) for the suggestion.
 - 0.81.0 [Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for reporting 
-- 0.80.0 [Fix] Use speeds from GPX file, in preference to GoPro file, when using GPX and GoPro together.
-  - [Change] Bump Required python version to 3.10
-- 0.79.0 [Fix] Changed GPS filtering reporting, it was a bit off.
-- 0.78.0 [Fix] Gradient calculation had become disabled.
-  - [Feature] Can now filter GPS points by max DOP `--gps-dop-max`
-  - [Feature] Can now filter GPS points by max Speed `--gps-speed-max` `--gps-speed-max-units`
-  - [Feature] Can now filter GPS points by bounding box - Useful if a few points claim to be locked, but are far away. Load GPX file into mapping software to see bounding box easily, for now. `--gps-bbox-lon-lat`
-  - [Change] Outputs except for generated files are now to stderr rather than stdout
-  - [Feature] `gopro-to-csv.py` and `gopro-to-gpx.py` now support `--only-locked` and `--every` to limit number of points (also GPS point filters, as above)
-  - [Change] Change in the way chart handles missing values - stops chart going to 0.
-  - Updated various library dependency versions.
-- 0.77.0 [Change] Disable speed and other calculations when GPS is not locked - stops unbelievable values
-  - [Change] changes to GPS parsing, should make detection of GPS lock more accurate (some 'not locked' values used to be included) still not perfect h/t [@falumas](https://github.com/falumas)
-  - [Change] add new widget "gps-lock-icon" at top of screen to show GPS lock - hopefully not too intrusive - can switch off with `--exclude`
-  - [Change] interpolate GPX/FIT tracks so they update every 0.1s - h/t [@0x10](https://github.com/0x10)
-- 0.76.0 [New Feature] New widget - "cairo_circuit_map" - Much nicer looking circuit map, and first widget that uses new optional "cairo" library.
-  - See examples [Cairo Circuit Map](docs/xml/examples/06-cairo-circuit-map/README.md)
 
 Older changes are in [CHANGELOG.md](CHANGELOG.md)
 
-
-
```

#### html2text {}

```diff
@@ -1,45 +1,34 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.90.0 Summary: Overlay
-graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
-gopro-dashboard-overlay Author: James Richardson Author-email:
-james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
-time4tea/gopro-dashboard-overlay Platform: UNKNOWN Classifier: Development
-Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
-License Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
-Classifier: Environment :: Console Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Multimedia :: Video Requires-Python: >=3.10 Description-
-Content-Type: text/markdown License-File: LICENSE.md # Create video overlays
-from GoPro Videos or any GPX/FIT file [GitHub_Discussions] [PyPI] [Docker]
-Discuss on [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-
-overlay/discussions) - Overlaying exciting graphics onto GoPro videos with
-super-exact synchronization - *NEW & EXPERIMENTAL* Create videos from any GPX
-file - no GoPro required - Support multiple resolutions, most GoPro models,
-normal, timelapse & timewarp modes - Convert GoPro movie metadata to GPX or CSV
-files - Cut sections from GoPro movies (including metadata) ## Examples !
-[Example Dashboard Image](examples/2022-05-15-example.png) ![Example Dashboard
-Image](examples/2022-06-11-contrib-example.png) ![Example Dashboard Image]
-(examples/2022-07-19-contrib-example-plane.jpg) An Example of 'overlay only'
-mode, which generates movies from GPX files ![Example Dashboard Image]
-(examples/2022-11-24-gpx-only-overlay.png) Example from [examples/layout]
-(examples/layout) ![Example Dashboard Image](examples/layout/layout-cairo-
-2704x1520.png) ## Map Styles Almost 30 different map styles are supported! -
-See [map styles](docs/maps/README.md) for more *Example* | . | . | . | . | |---
-----------------------------------|--------------------------------------------
----|-------------------------------------------------------|-------------------
-------------------------------------| | ![osm](docs/maps/map_style_osm.png) | !
-[tf-cycle](docs/maps/map_style_tf-cycle.png) | ![tf-transport](docs/maps/
-map_style_tf-transport.png) | ![tf-landscape](docs/maps/map_style_tf-
-landscape.png) | ## Requirements - Python3.10 - ffmpeg (you'll need the ffmpeg
-program installed) - Unixy machine (probably, untested on Windows) ##
-Installation Install locally using `pip`, or use the provided Docker image
-Optional: Some widgets require the `cairo` library - which must be installed
-separately. ### Installing and running with docker The docker image is a new
-thing and still a bit experimental... please file an issue if you find any
-problems. The docker image contains all you need to get started, and uses a
+# Create video overlays from GoPro Videos or any GPX/FIT file [GitHub
+Discussions] [PyPI] [Docker] Discuss on [GitHub Discussions](https://
+github.com/time4tea/gopro-dashboard-overlay/discussions) - Overlaying exciting
+graphics onto GoPro videos with super-exact synchronization - *NEW &
+EXPERIMENTAL* Create videos from any GPX file - no GoPro required - Support
+multiple resolutions, most GoPro models, normal, timelapse & timewarp modes -
+Convert GoPro movie metadata to GPX or CSV files - Cut sections from GoPro
+movies (including metadata) ## Examples ![Example Dashboard Image](examples/
+2022-05-15-example.png) ![Example Dashboard Image](examples/2022-06-11-contrib-
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
+maps/map_style_tf-landscape.png) | ## Requirements - Python3.10 - ffmpeg
+(you'll need the ffmpeg program installed) - Unixy machine (probably, untested
+on Windows) ## Installation Install locally using `pip`, or use the provided
+Docker image Optional: Some widgets require the `cairo` library - which must be
+installed separately. ### Installing and running with docker The docker image
+is a new thing and still a bit experimental... please file an issue if you find
+any problems. The docker image contains all you need to get started, and uses a
 volume `/work/`, which we suggest you map to the current directory which can
 contain your GoPro files. Note that the docker version doesn't support nvidia
 GPU extensions. The most recent version on docker is: [Docker] ```shell docker
 run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:  [args...] ```
 e.g. ```shell docker run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-
 overlay:0.81.0 gopro-dashboard.py GH010122.MP4 render/docker.MP4 ``` Files
 created by the program will be created with the same uid that owns the mapped
@@ -97,60 +86,40 @@
 www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
 www.thunderforest.com/) ## References https://github.com/juanmcasillas/
 gopro2gpx https://github.com/JuanIrache/gopro-telemetry https://github.com/
 gopro/gpmf-parser https://coderunner.io/how-to-compress-gopro-movies-and-keep-
 metadata/ ## Other Related Software https://github.com/progweb/gpx2video https:
 //github.com/JuanIrache/gopro-telemetry ## Latest Changes If you find any
 issues with new releases, please discuss in [GitHub Discussions](https://
-github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.90.8 [Change]
-`cairo-circuit` now draws much more quickly. - [Change] Map rendering caches
-tile images more efficiently, so draws more quickly. - 0.89.0 [Feature] New
-component `cairo-gauge-round-annotated` - A bit like a car speedometer - See
-docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-
-cairo-gauge-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there
-were no locked GPS points in the movie. - Thanks [@shahargli](https://
-github.com/shahargli) for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` -
-discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each
-colour. - 0.86.0 [Feature] New component `cairo-gauge-marker` - a nice clean
-gauge component, with a marker for the current value.. See docs [docs/xml/
-examples/06-cairo-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) -
-0.85.0 [Feature/Breaking Possibly] Add validation to attributes in layout
-files. This may cause some custom layouts to break! - But they wouldn't have
-been working as intended. - [Change/Breaking] Change some `zone-bar` attribute
-names, aiming for standardisation - [Change/Breaking] Change some `cairo-
-circuit-map` attribute names, aiming for standardisation - 0.84.0 [Feature] New
-component `zone-bar` - a 3-zone bar control that can be used for HR/Cadence/
-Power zones. See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-
-zone-bar) - Many thanks to [@jchinte](https://github.com/jchinte) for
-contributing! - 0.83.0 [Change] No longer require --overlay-size when using --
-use-gpx-only, but supplying input video - [Fix] Give better error message when
-video and GPX don't overlap in time, but told to sync - Thanks to [@mfloryan]
-(https://github.com/mfloryan) for reporting both of these - 0.82.0 [Change]
-Support for changing units in layouts from the command line. Use `--units-
-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
-[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
-[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
-won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
-reporting - 0.80.0 [Fix] Use speeds from GPX file, in preference to GoPro file,
-when using GPX and GoPro together. - [Change] Bump Required python version to
-3.10 - 0.79.0 [Fix] Changed GPS filtering reporting, it was a bit off. - 0.78.0
-[Fix] Gradient calculation had become disabled. - [Feature] Can now filter GPS
-points by max DOP `--gps-dop-max` - [Feature] Can now filter GPS points by max
-Speed `--gps-speed-max` `--gps-speed-max-units` - [Feature] Can now filter GPS
-points by bounding box - Useful if a few points claim to be locked, but are far
-away. Load GPX file into mapping software to see bounding box easily, for now.
-`--gps-bbox-lon-lat` - [Change] Outputs except for generated files are now to
-stderr rather than stdout - [Feature] `gopro-to-csv.py` and `gopro-to-gpx.py`
-now support `--only-locked` and `--every` to limit number of points (also GPS
-point filters, as above) - [Change] Change in the way chart handles missing
-values - stops chart going to 0. - Updated various library dependency versions.
-- 0.77.0 [Change] Disable speed and other calculations when GPS is not locked -
-stops unbelievable values - [Change] changes to GPS parsing, should make
-detection of GPS lock more accurate (some 'not locked' values used to be
-included) still not perfect h/t [@falumas](https://github.com/falumas) -
-[Change] add new widget "gps-lock-icon" at top of screen to show GPS lock -
-hopefully not too intrusive - can switch off with `--exclude` - [Change]
-interpolate GPX/FIT tracks so they update every 0.1s - h/t [@0x10](https://
-github.com/0x10) - 0.76.0 [New Feature] New widget - "cairo_circuit_map" - Much
-nicer looking circuit map, and first widget that uses new optional "cairo"
-library. - See examples [Cairo Circuit Map](docs/xml/examples/06-cairo-circuit-
-map/README.md) Older changes are in [CHANGELOG.md](CHANGELOG.md)
+github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.91.0 [Fix] Ignore
+FIT data items that don't have a GPS location. [#122](https://github.com/
+time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://
+github.com/patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now
+draws much more quickly. - [Change] Map rendering caches tile images more
+efficiently, so draws more quickly. - 0.89.0 [Feature] New component `cairo-
+gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/
+examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-
+round-annotated) - 0.88.0 [Fix] Journey Map broke when no there were no locked
+GPS points in the movie. - Thanks [@shahargli](https://github.com/shahargli)
+for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs,
+now fixed. Removed `alpha`, instead use alpha of each colour. - 0.86.0
+[Feature] New component `cairo-gauge-marker` - a nice clean gauge component,
+with a marker for the current value.. See docs [docs/xml/examples/06-cairo-
+gauge-marker](docs/xml/examples/06-cairo-gauge-marker) - 0.85.0 [Feature/
+Breaking Possibly] Add validation to attributes in layout files. This may cause
+some custom layouts to break! - But they wouldn't have been working as
+intended. - [Change/Breaking] Change some `zone-bar` attribute names, aiming
+for standardisation - [Change/Breaking] Change some `cairo-circuit-map`
+attribute names, aiming for standardisation - 0.84.0 [Feature] New component
+`zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones.
+See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar) -
+Many thanks to [@jchinte](https://github.com/jchinte) for contributing! -
+0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but
+supplying input video - [Fix] Give better error message when video and GPX
+don't overlap in time, but told to sync - Thanks to [@mfloryan](https://
+github.com/mfloryan) for reporting both of these - 0.82.0 [Change] Support for
+changing units in layouts from the command line. Use `--units-speed` etc to
+control. Examples are in [docs/bin](docs/bin) - Thanks to [@matzeruegge](https:
+//github.com/matzeruegge) for the suggestion. - 0.81.0 [Fix] gopro-rename was
+broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to
+[matzeruegge](https://github.com/matzeruegge) for reporting Older changes are
+in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.90.0/gopro_overlay.egg-info/SOURCES.txt` & `gopro-overlay-0.91.0/gopro_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.90.0/setup.py` & `gopro-overlay-0.91.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 test_requirements = [
     "pytest"
 ]
 
 setup(
     name="gopro-overlay",
-    version="0.90.0",
+    version="0.91.0",
     description="Overlay graphics dashboards onto GoPro footage",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/time4tea/gopro-dashboard-overlay",
     author="James Richardson",
     author_email="james+gopro@time4tea.net",
     license="MIT",
```

