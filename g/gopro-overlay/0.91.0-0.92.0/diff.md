# Comparing `tmp/gopro-overlay-0.91.0.tar.gz` & `tmp/gopro-overlay-0.92.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopro-overlay-0.91.0.tar", last modified: Mon May  1 11:52:21 2023, max compression
+gzip compressed data, was "gopro-overlay-0.92.0.tar", last modified: Mon May  8 10:40:59 2023, max compression
```

## Comparing `gopro-overlay-0.91.0.tar` & `gopro-overlay-0.92.0.tar`

### file list

```diff
@@ -1,145 +1,146 @@
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/
--rw-rw-r--   0 richja    (1000) richja    (1000)     2097 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/LICENSE.md
--rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.91.0/MANIFEST.in
--rw-rw-r--   0 richja    (1000) richja    (1000)    11369 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)    10556 2023-05-01 11:51:58.000000 gopro-overlay-0.91.0/README.md
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.824821 gopro-overlay-0.91.0/bin/
--rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.91.0/bin/gopro-contrib-data-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.91.0/bin/gopro-cut.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    14774 2023-02-09 14:38:27.000000 gopro-overlay-0.91.0/bin/gopro-dashboard.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-debug.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.91.0/bin/gopro-extract.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-join.py
--rwxrwxr-x   0 richja    (1000) richja    (1000)     5501 2023-02-09 13:31:45.000000 gopro-overlay-0.91.0/bin/gopro-layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3578 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-rename.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-to-csv.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/bin/gopro-to-gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.828821 gopro-overlay-0.91.0/gopro_overlay/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.91.0/gopro_overlay/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-01 11:49:17.000000 gopro-overlay-0.91.0/gopro_overlay/__version__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     7004 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/arguments.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.91.0/gopro_overlay/common.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/counter.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/date_overlap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.91.0/gopro_overlay/dimensions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/entry.py
--rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.91.0/gopro_overlay/exceptions.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1296 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/execution.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/fake.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     9622 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/ffmpeg.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1031 2023-01-05 11:17:11.000000 gopro-overlay-0.91.0/gopro_overlay/ffmpeg_profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1803 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/filenaming.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:34:34.000000 gopro-overlay-0.91.0/gopro_overlay/fit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.91.0/gopro_overlay/font.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/framemeta.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/framemeta_gpx.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.91.0/gopro_overlay/functional.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.91.0/gopro_overlay/geo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.91.0/gopro_overlay/geo_render.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      272 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/geocode.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_calculate.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_cori.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_debug.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_grav.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_xyz.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/gpx.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.832821 gopro-overlay-0.91.0/gopro_overlay/icons/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.91.0/gopro_overlay/icons/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.91.0/gopro_overlay/icons/bicycle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.91.0/gopro_overlay/icons/car.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/faq.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/forbidden.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gauge-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gauge.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_2d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_3d.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_none.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_unknown.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.91.0/gopro_overlay/icons/heartbeat.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.91.0/gopro_overlay/icons/ice-cream-van.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.91.0/gopro_overlay/icons/mountain-range.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.91.0/gopro_overlay/icons/mountain.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.91.0/gopro_overlay/icons/power.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.91.0/gopro_overlay/icons/ruler.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.91.0/gopro_overlay/icons/slope-triangle.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.91.0/gopro_overlay/icons/slope.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.91.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.91.0/gopro_overlay/icons/thermometer-1.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.91.0/gopro_overlay/icons/thermometer.png
--rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.91.0/gopro_overlay/icons/user.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.91.0/gopro_overlay/icons/van-black-side-view.png
--rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/journey.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3341 2023-02-09 13:31:45.000000 gopro-overlay-0.91.0/gopro_overlay/layout.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_components.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_xml.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_xml_attribute.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layout_xml_cairo.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/gopro_overlay/layouts/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/default-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/default-2704x1520.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/default-3840x2160.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/example-2.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/example.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/layouts/power-1920x1080.xml
--rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/log.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.91.0/gopro_overlay/models.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.91.0/gopro_overlay/parsing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/point.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.91.0/gopro_overlay/privacy.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.91.0/gopro_overlay/progress_frames.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/rdp.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/smoothing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/timeseries.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/timeseries_process.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.91.0/gopro_overlay/timeunits.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/timing.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.91.0/gopro_overlay/units.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/gopro_overlay/widgets/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/asi.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/bar.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/
--rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/__init__.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/angle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/annotation.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/background.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/bordered.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/box.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cairo.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cap.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/circuit.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/colour.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/ellipse.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/face.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_marker.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_round_254.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/line.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/needle.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/reading.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/scale.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/tick.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/chart.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/compass.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/compass_arrow.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/gps.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/gradient_bar.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/info.py
--rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/map.py
--rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/profile.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/text.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     8111 2023-02-09 13:31:45.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/widgets.py
--rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.91.0/gopro_overlay/widgets/widgets_experimental.py
-drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-01 11:52:21.828821 gopro-overlay-0.91.0/gopro_overlay.egg-info/
--rw-rw-r--   0 richja    (1000) richja    (1000)    11369 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/PKG-INFO
--rw-rw-r--   0 richja    (1000) richja    (1000)     4205 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/SOURCES.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/dependency_links.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       20 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/entry_points.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/requires.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-01 11:52:21.000000 gopro-overlay-0.91.0/gopro_overlay.egg-info/top_level.txt
--rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-01 11:52:21.836821 gopro-overlay-0.91.0/setup.cfg
--rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-01 11:49:17.000000 gopro-overlay-0.91.0/setup.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.541097 gopro-overlay-0.92.0/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2097 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/LICENSE.md
+-rw-rw-r--   0 richja    (1000) richja    (1000)       70 2022-02-02 12:18:46.000000 gopro-overlay-0.92.0/MANIFEST.in
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11713 2023-05-08 10:40:59.537097 gopro-overlay-0.92.0/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10900 2023-05-08 10:40:44.000000 gopro-overlay-0.92.0/README.md
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.525097 gopro-overlay-0.92.0/bin/
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3153 2022-05-23 15:18:05.000000 gopro-overlay-0.92.0/bin/gopro-contrib-data-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1450 2022-02-03 15:47:43.000000 gopro-overlay-0.92.0/bin/gopro-cut.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14862 2023-05-08 10:30:40.000000 gopro-overlay-0.92.0/bin/gopro-dashboard.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      770 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/bin/gopro-debug.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)      596 2022-11-29 16:44:06.000000 gopro-overlay-0.92.0/bin/gopro-extract.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1035 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/bin/gopro-join.py
+-rwxrwxr-x   0 richja    (1000) richja    (1000)     5527 2023-05-06 09:06:40.000000 gopro-overlay-0.92.0/bin/gopro-layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3578 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/bin/gopro-rename.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5783 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/bin/gopro-to-csv.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3412 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/bin/gopro-to-gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.529097 gopro-overlay-0.92.0/gopro_overlay/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-02-02 11:42:38.000000 gopro-overlay-0.92.0/gopro_overlay/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      299 2023-05-08 10:38:15.000000 gopro-overlay-0.92.0/gopro_overlay/__version__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7168 2023-05-06 10:52:50.000000 gopro-overlay-0.92.0/gopro_overlay/arguments.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5447 2023-05-08 10:30:40.000000 gopro-overlay-0.92.0/gopro_overlay/buffering.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      690 2022-11-29 17:00:53.000000 gopro-overlay-0.92.0/gopro_overlay/common.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      207 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/counter.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      483 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/date_overlap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      531 2023-02-07 21:58:09.000000 gopro-overlay-0.92.0/gopro_overlay/dimensions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1719 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/entry.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)       34 2022-11-23 14:47:58.000000 gopro-overlay-0.92.0/gopro_overlay/exceptions.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1345 2023-05-06 10:59:08.000000 gopro-overlay-0.92.0/gopro_overlay/execution.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/fake.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9730 2023-05-08 10:12:47.000000 gopro-overlay-0.92.0/gopro_overlay/ffmpeg.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1031 2023-01-05 11:17:11.000000 gopro-overlay-0.92.0/gopro_overlay/ffmpeg_profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1803 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/filenaming.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2279 2023-05-01 11:53:38.000000 gopro-overlay-0.92.0/gopro_overlay/fit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      122 2021-12-03 14:46:33.000000 gopro-overlay-0.92.0/gopro_overlay/font.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10542 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/framemeta.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3000 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/framemeta_gpx.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      478 2022-05-27 13:38:56.000000 gopro-overlay-0.92.0/gopro_overlay/functional.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5703 2023-02-08 14:26:51.000000 gopro-overlay-0.92.0/gopro_overlay/geo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2426 2023-02-09 10:45:34.000000 gopro-overlay-0.92.0/gopro_overlay/geo_render.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      272 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/geocode.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8689 2023-03-15 08:32:52.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3275 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd_calculate.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3482 2022-11-23 14:02:47.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3420 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_cori.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      525 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_debug.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8588 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2859 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_grav.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4709 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_xyz.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2963 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/gpx.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.533097 gopro-overlay-0.92.0/gopro_overlay/icons/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.92.0/gopro_overlay/icons/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13448 2021-09-30 11:08:46.000000 gopro-overlay-0.92.0/gopro_overlay/icons/bicycle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8077 2021-09-30 11:08:22.000000 gopro-overlay-0.92.0/gopro_overlay/icons/car.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    22971 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/icons/faq.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    34059 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/icons/forbidden.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    19173 2021-09-20 15:22:09.000000 gopro-overlay-0.92.0/gopro_overlay/icons/gauge-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15425 2021-09-20 15:24:33.000000 gopro-overlay-0.92.0/gopro_overlay/icons/gauge.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    12719 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_2d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     9239 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_3d.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    32100 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_none.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    28140 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_unknown.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13732 2021-09-21 11:34:05.000000 gopro-overlay-0.92.0/gopro_overlay/icons/heartbeat.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5700 2021-09-30 11:09:17.000000 gopro-overlay-0.92.0/gopro_overlay/icons/ice-cream-van.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    20413 2021-09-20 15:26:49.000000 gopro-overlay-0.92.0/gopro_overlay/icons/mountain-range.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    13636 2021-09-20 15:27:04.000000 gopro-overlay-0.92.0/gopro_overlay/icons/mountain.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8451 2022-11-06 20:16:59.000000 gopro-overlay-0.92.0/gopro_overlay/icons/power.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    14622 2021-09-20 15:58:10.000000 gopro-overlay-0.92.0/gopro_overlay/icons/ruler.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15485 2021-09-20 15:27:45.000000 gopro-overlay-0.92.0/gopro_overlay/icons/slope-triangle.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10147 2021-09-20 15:27:28.000000 gopro-overlay-0.92.0/gopro_overlay/icons/slope.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    15997 2021-09-20 15:22:31.000000 gopro-overlay-0.92.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     7655 2021-09-20 15:26:02.000000 gopro-overlay-0.92.0/gopro_overlay/icons/thermometer-1.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10579 2021-09-20 15:25:42.000000 gopro-overlay-0.92.0/gopro_overlay/icons/thermometer.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11096 2021-09-30 11:51:55.000000 gopro-overlay-0.92.0/gopro_overlay/icons/user.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6958 2021-09-30 11:09:29.000000 gopro-overlay-0.92.0/gopro_overlay/icons/van-black-side-view.png
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2074 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/journey.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3337 2023-05-06 09:06:40.000000 gopro-overlay-0.92.0/gopro_overlay/layout.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1025 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layout_components.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    26241 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layout_xml.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1067 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layout_xml_attribute.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5498 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layout_xml_cairo.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.537097 gopro-overlay-0.92.0/gopro_overlay/layouts/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2021-09-22 14:27:16.000000 gopro-overlay-0.92.0/gopro_overlay/layouts/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3294 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layouts/default-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3515 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layouts/default-2704x1520.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3302 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layouts/default-3840x2160.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1510 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layouts/example-2.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8388 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layouts/example.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3802 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/layouts/power-1920x1080.xml
+-rw-rw-r--   0 richja    (1000) richja    (1000)      145 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/log.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      736 2021-09-30 11:21:57.000000 gopro-overlay-0.92.0/gopro_overlay/models.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      294 2022-02-09 11:24:51.000000 gopro-overlay-0.92.0/gopro_overlay/parsing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6672 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/point.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      575 2021-09-22 14:35:02.000000 gopro-overlay-0.92.0/gopro_overlay/privacy.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      329 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      891 2022-05-21 21:20:30.000000 gopro-overlay-0.92.0/gopro_overlay/progress_frames.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2297 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/rdp.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1224 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/smoothing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2966 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/timeseries.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3005 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/timeseries_process.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1974 2022-09-24 19:15:22.000000 gopro-overlay-0.92.0/gopro_overlay/timeunits.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1287 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/timing.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      365 2022-11-29 15:04:43.000000 gopro-overlay-0.92.0/gopro_overlay/units.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.537097 gopro-overlay-0.92.0/gopro_overlay/widgets/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2022-11-02 15:56:34.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4453 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/asi.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2121 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/bar.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.537097 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/
+-rw-rw-r--   0 richja    (1000) richja    (1000)        0 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/__init__.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2227 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/angle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3671 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/annotation.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      643 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/background.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     6174 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/bordered.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      183 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/box.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3676 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/cairo.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1825 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/cap.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4190 2023-02-09 12:46:37.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/circuit.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1835 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/colour.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4777 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/ellipse.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      833 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/face.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     5749 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/gauge_marker.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4184 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/gauge_round_254.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      424 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/line.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3619 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/needle.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      513 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/reading.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1923 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/scale.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      189 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/tick.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2412 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/chart.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3451 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/compass.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2226 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/compass_arrow.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      517 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/gps.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3687 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/gradient_bar.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     2204 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/info.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)    10811 2023-02-08 14:26:51.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/map.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)      789 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/profile.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     3107 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/text.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     8038 2023-05-06 09:06:40.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/widgets.py
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1509 2023-02-07 21:54:02.000000 gopro-overlay-0.92.0/gopro_overlay/widgets/widgets_experimental.py
+drwxrwxr-x   0 richja    (1000) richja    (1000)        0 2023-05-08 10:40:59.529097 gopro-overlay-0.92.0/gopro_overlay.egg-info/
+-rw-rw-r--   0 richja    (1000) richja    (1000)    11713 2023-05-08 10:40:59.000000 gopro-overlay-0.92.0/gopro_overlay.egg-info/PKG-INFO
+-rw-rw-r--   0 richja    (1000) richja    (1000)     4232 2023-05-08 10:40:59.000000 gopro-overlay-0.92.0/gopro_overlay.egg-info/SOURCES.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)        1 2023-05-08 10:40:59.000000 gopro-overlay-0.92.0/gopro_overlay.egg-info/dependency_links.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       20 2023-05-08 10:40:59.000000 gopro-overlay-0.92.0/gopro_overlay.egg-info/entry_points.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)      132 2023-05-08 10:40:59.000000 gopro-overlay-0.92.0/gopro_overlay.egg-info/requires.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       14 2023-05-08 10:40:59.000000 gopro-overlay-0.92.0/gopro_overlay.egg-info/top_level.txt
+-rw-rw-r--   0 richja    (1000) richja    (1000)       38 2023-05-08 10:40:59.541097 gopro-overlay-0.92.0/setup.cfg
+-rw-rw-r--   0 richja    (1000) richja    (1000)     1933 2023-05-08 10:38:15.000000 gopro-overlay-0.92.0/setup.py
```

### Comparing `gopro-overlay-0.91.0/LICENSE.md` & `gopro-overlay-0.92.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/PKG-INFO` & `gopro-overlay-0.92.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.91.0
+Version: 0.92.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Platform: UNKNOWN
@@ -58,14 +58,15 @@
 
 
 ## Requirements
 
 
 - Python3.10
 - ffmpeg (you'll need the ffmpeg program installed)
+- libraqm (needed by [Pillow](https://pypi.org/project/Pillow/))
 - Unixy machine (probably, untested on Windows)
 
 ## Installation
 
 Install locally using `pip`, or use the provided Docker image
 
 Optional: Some widgets require the `cairo` library - which must be installed separately.
@@ -202,15 +203,15 @@
 
 ## Related Software
 
 - https://github.com/julesgraus/interactiveGoProDashboardTool - An interactive helper to build the command line for the dashboard program
 
 ## Known Bugs / Issues
 
-- Only tested on a GoPro Hero 9, that's all I have. Sample files for other devices are welcomed.
+- Only tested on a GoPro Hero 9/11, that's all I have. Sample files for other devices are welcomed.
 
 ## Icons
 
 Icon files in [icons](gopro_overlay/icons) are not covered by the MIT licence
 
 ## Map Data
 
@@ -233,14 +234,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
 - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated)
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.91.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.92.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -26,111 +26,115 @@
 See [map styles](docs/maps/README.md) for more *Example* | . | . | . | . | |---
 ----------------------------------|--------------------------------------------
 ---|-------------------------------------------------------|-------------------
 ------------------------------------| | ![osm](docs/maps/map_style_osm.png) | !
 [tf-cycle](docs/maps/map_style_tf-cycle.png) | ![tf-transport](docs/maps/
 map_style_tf-transport.png) | ![tf-landscape](docs/maps/map_style_tf-
 landscape.png) | ## Requirements - Python3.10 - ffmpeg (you'll need the ffmpeg
-program installed) - Unixy machine (probably, untested on Windows) ##
-Installation Install locally using `pip`, or use the provided Docker image
-Optional: Some widgets require the `cairo` library - which must be installed
-separately. ### Installing and running with docker The docker image is a new
-thing and still a bit experimental... please file an issue if you find any
-problems. The docker image contains all you need to get started, and uses a
-volume `/work/`, which we suggest you map to the current directory which can
-contain your GoPro files. Note that the docker version doesn't support nvidia
-GPU extensions. The most recent version on docker is: [Docker] ```shell docker
-run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:  [args...] ```
-e.g. ```shell docker run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-
-overlay:0.81.0 gopro-dashboard.py GH010122.MP4 render/docker.MP4 ``` Files
-created by the program will be created with the same uid that owns the mapped
-directory. You can use the `--cache-dir` and `--config-dir` command line
-arguments to configure where the cache and config dirs are, thereby making it
-easier to use persistent mapped volumes. ### Installing and running with pip
-```shell python -m venv venv venv/bin/pip install gopro-overlay ``` The Roboto
-font needs to be installed on your system. You could install it with one of the
-following commands maybe. ```bash pacman -S ttf-roboto apt install truetype-
-roboto apt install fonts-roboto ``` #### (Optional) Installing pycairo
-Optionally, install `pycairo` ```shell venv/bin/pip install pycairo==1.23.0 ```
-You might need to install some system libraries - This is what the pycairo docs
-suggest: Ubuntu/Debian: `sudo apt install libcairo2-dev pkg-config python3-dev`
-macOS/Homebrew: `brew install cairo pkg-config` ## Overlaying a dashboard
-```shell venv/bin/gopro-dashboard.py ``` The GPS track in Hero 9 (at least)
-seems to be very poor. If you supply a GPX file from a Garmin or whatever, the
-program will use this instead for the GPS. Privacy allows you to set a privacy
-zone. Various widgets will not draw points within that zone. The data recorded
-in the GoPro video will uses GPS time, which (broadly) is UTC. The renderer
-will use your local timezone to interpret this, and use the local timezone.
-This may produce strange results if you go on holiday somewhere, but then
-render the files when you get back home! On linux you can use the TZ variable
-to change the timezone that's used. ### Example For full instructions on all
-command lines see [docs/bin](docs/bin) ```shell venv/bin/gopro-dashboard.py --
-gpx ~/Downloads/Morning_Ride.gpx --privacy 52.000,-0.40000,0.50 ~/gopro/
-GH020073.MP4 GH020073-dashboard.MP4 ``` ## Writeups There's a great writeup of
-how to use the software to make an overlay from a GPX file at https://
-blog.cubieserver.de/2022/creating-gpx-overlay-videos-on-linux/ (Nov 2022) ###
-Format of the Dashboard Configuration file Several dashboards are built-in to
-the software, but the dashboard layout is highly configurable, controlled by an
-XML file. For more information on the (extensive) configurability of the layout
-please see [docs/xml](docs/xml) and lots of [examples](docs/xml/examples/
-README.md) ## FFMPEG Control & GPUs *Experimental* FFMPEG has **a lot** of
-options! This program comes with some mostly sensible defaults, but to use GPUs
-and control the output much more carefully, including framerates and bitrates,
-you can use a JSON file containing a number of 'profiles' and select the
-profile you want when running the program. For more details on how to select
-these, and an example of Nvidia GPU, please see [docs/bin](docs/bin) Please
-also see [PERFORMANCE.md](PERFORMANCE.md) ## Converting to GPX files ```shell
-venv/bin/gopro-to-gpx.py  [output-file] ``` ## Joining a sequence of MP4 files
-together Use the gopro-join.py command. Given a single file from the sequence,
-it will find and join together all the files. If you have any problems with
-this, please do raise an issue - I don't have that much test data. The joined
-file almost certainly won't work in the GoPro tools! - But it should work with
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
+it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:0.81.0 gopro-
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
+example of Nvidia GPU, please see [docs/bin](docs/bin) Please also see
+[PERFORMANCE.md](PERFORMANCE.md) ## Converting to GPX files ```shell venv/bin/
+gopro-to-gpx.py  [output-file] ``` ## Joining a sequence of MP4 files together
+Use the gopro-join.py command. Given a single file from the sequence, it will
+find and join together all the files. If you have any problems with this,
+please do raise an issue - I don't have that much test data. The joined file
+almost certainly won't work in the GoPro tools! - But it should work with
 `gopro-dashboard.py` - I will look into the additional technical stuff required
 to make it work in the GoPro tools. *This will require a lot of disk space!*
 ```shell venv/bin/gopro-join.py /media/sdcard/DCIM/100GOPRO/GH030170.MP4 /data/
 gopro/nice-ride.MP4 ``` ## Cutting a section from a GoPro file You can cut a
 section of the gopro file, with metadata. ## Related Software - https://
 github.com/julesgraus/interactiveGoProDashboardTool - An interactive helper to
 build the command line for the dashboard program ## Known Bugs / Issues - Only
-tested on a GoPro Hero 9, that's all I have. Sample files for other devices are
-welcomed. ## Icons Icon files in [icons](gopro_overlay/icons) are not covered
-by the MIT licence ## Map Data Data Â© [OpenStreetMap contributors](http://
-www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
+tested on a GoPro Hero 9/11, that's all I have. Sample files for other devices
+are welcomed. ## Icons Icon files in [icons](gopro_overlay/icons) are not
+covered by the MIT licence ## Map Data Data Â© [OpenStreetMap contributors]
+(http://www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
 www.thunderforest.com/) ## References https://github.com/juanmcasillas/
 gopro2gpx https://github.com/JuanIrache/gopro-telemetry https://github.com/
 gopro/gpmf-parser https://coderunner.io/how-to-compress-gopro-movies-and-keep-
 metadata/ ## Other Related Software https://github.com/progweb/gpx2video https:
 //github.com/JuanIrache/gopro-telemetry ## Latest Changes If you find any
 issues with new releases, please discuss in [GitHub Discussions](https://
-github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.91.0 [Fix] Ignore
-FIT data items that don't have a GPS location. [#122](https://github.com/
-time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://
-github.com/patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now
-draws much more quickly. - [Change] Map rendering caches tile images more
-efficiently, so draws more quickly. - 0.89.0 [Feature] New component `cairo-
-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/
-examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-
-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there were no locked
-GPS points in the movie. - Thanks [@shahargli](https://github.com/shahargli)
-for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs,
-now fixed. Removed `alpha`, instead use alpha of each colour. - 0.86.0
-[Feature] New component `cairo-gauge-marker` - a nice clean gauge component,
-with a marker for the current value.. See docs [docs/xml/examples/06-cairo-
-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) - 0.85.0 [Feature/
-Breaking Possibly] Add validation to attributes in layout files. This may cause
-some custom layouts to break! - But they wouldn't have been working as
-intended. - [Change/Breaking] Change some `zone-bar` attribute names, aiming
-for standardisation - [Change/Breaking] Change some `cairo-circuit-map`
-attribute names, aiming for standardisation - 0.84.0 [Feature] New component
-`zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones.
-See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar) -
-Many thanks to [@jchinte](https://github.com/jchinte) for contributing! -
-0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but
-supplying input video - [Fix] Give better error message when video and GPX
-don't overlap in time, but told to sync - Thanks to [@mfloryan](https://
-github.com/mfloryan) for reporting both of these - 0.82.0 [Change] Support for
-changing units in layouts from the command line. Use `--units-speed` etc to
-control. Examples are in [docs/bin](docs/bin) - Thanks to [@matzeruegge](https:
-//github.com/matzeruegge) for the suggestion. - 0.81.0 [Fix] gopro-rename was
-broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to
-[matzeruegge](https://github.com/matzeruegge) for reporting Older changes are
-in [CHANGELOG.md](CHANGELOG.md)
+github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.92.0 [Feature] `--
+double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster
+rendering, but may not work on all architectures. Speed improvements highly
+dependent on `ffmpeg` performance. Likely much faster when using `--generate
+overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't
+have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
+raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
+[Change] Map rendering caches tile images more efficiently, so draws more
+quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
+like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
+annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
+Journey Map broke when no there were no locked GPS points in the movie. -
+Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
+Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
+instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
+gauge-marker` - a nice clean gauge component, with a marker for the current
+value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
+06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
+attributes in layout files. This may cause some custom layouts to break! - But
+they wouldn't have been working as intended. - [Change/Breaking] Change some
+`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
+Change some `cairo-circuit-map` attribute names, aiming for standardisation -
+0.84.0 [Feature] New component `zone-bar` - a 3-zone bar control that can be
+used for HR/Cadence/Power zones. See docs in [docs/xml/examples/07-zone-bar]
+(docs/xml/examples/07-zone-bar) - Many thanks to [@jchinte](https://github.com/
+jchinte) for contributing! - 0.83.0 [Change] No longer require --overlay-size
+when using --use-gpx-only, but supplying input video - [Fix] Give better error
+message when video and GPX don't overlap in time, but told to sync - Thanks to
+[@mfloryan](https://github.com/mfloryan) for reporting both of these - 0.82.0
+[Change] Support for changing units in layouts from the command line. Use `--
+units-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
+[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
+[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
+won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
+reporting Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.91.0/README.md` & `gopro-overlay-0.92.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 
 ## Requirements
 
 
 - Python3.10
 - ffmpeg (you'll need the ffmpeg program installed)
+- libraqm (needed by [Pillow](https://pypi.org/project/Pillow/))
 - Unixy machine (probably, untested on Windows)
 
 ## Installation
 
 Install locally using `pip`, or use the provided Docker image
 
 Optional: Some widgets require the `cairo` library - which must be installed separately.
@@ -180,15 +181,15 @@
 
 ## Related Software
 
 - https://github.com/julesgraus/interactiveGoProDashboardTool - An interactive helper to build the command line for the dashboard program
 
 ## Known Bugs / Issues
 
-- Only tested on a GoPro Hero 9, that's all I have. Sample files for other devices are welcomed.
+- Only tested on a GoPro Hero 9/11, that's all I have. Sample files for other devices are welcomed.
 
 ## Icons
 
 Icon files in [icons](gopro_overlay/icons) are not covered by the MIT licence
 
 ## Map Data
 
@@ -211,14 +212,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
 - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated)
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
```

#### html2text {}

```diff
@@ -15,20 +15,21 @@
 map styles are supported! - See [map styles](docs/maps/README.md) for more
 *Example* | . | . | . | . | |-------------------------------------|------------
 -----------------------------------|-------------------------------------------
 ------------|-------------------------------------------------------| | ![osm]
 (docs/maps/map_style_osm.png) | ![tf-cycle](docs/maps/map_style_tf-cycle.png) |
 ![tf-transport](docs/maps/map_style_tf-transport.png) | ![tf-landscape](docs/
 maps/map_style_tf-landscape.png) | ## Requirements - Python3.10 - ffmpeg
-(you'll need the ffmpeg program installed) - Unixy machine (probably, untested
-on Windows) ## Installation Install locally using `pip`, or use the provided
-Docker image Optional: Some widgets require the `cairo` library - which must be
-installed separately. ### Installing and running with docker The docker image
-is a new thing and still a bit experimental... please file an issue if you find
-any problems. The docker image contains all you need to get started, and uses a
+(you'll need the ffmpeg program installed) - libraqm (needed by [Pillow](https:
+//pypi.org/project/Pillow/)) - Unixy machine (probably, untested on Windows) ##
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
@@ -76,50 +77,53 @@
 `gopro-dashboard.py` - I will look into the additional technical stuff required
 to make it work in the GoPro tools. *This will require a lot of disk space!*
 ```shell venv/bin/gopro-join.py /media/sdcard/DCIM/100GOPRO/GH030170.MP4 /data/
 gopro/nice-ride.MP4 ``` ## Cutting a section from a GoPro file You can cut a
 section of the gopro file, with metadata. ## Related Software - https://
 github.com/julesgraus/interactiveGoProDashboardTool - An interactive helper to
 build the command line for the dashboard program ## Known Bugs / Issues - Only
-tested on a GoPro Hero 9, that's all I have. Sample files for other devices are
-welcomed. ## Icons Icon files in [icons](gopro_overlay/icons) are not covered
-by the MIT licence ## Map Data Data Â© [OpenStreetMap contributors](http://
-www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
+tested on a GoPro Hero 9/11, that's all I have. Sample files for other devices
+are welcomed. ## Icons Icon files in [icons](gopro_overlay/icons) are not
+covered by the MIT licence ## Map Data Data Â© [OpenStreetMap contributors]
+(http://www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
 www.thunderforest.com/) ## References https://github.com/juanmcasillas/
 gopro2gpx https://github.com/JuanIrache/gopro-telemetry https://github.com/
 gopro/gpmf-parser https://coderunner.io/how-to-compress-gopro-movies-and-keep-
 metadata/ ## Other Related Software https://github.com/progweb/gpx2video https:
 //github.com/JuanIrache/gopro-telemetry ## Latest Changes If you find any
 issues with new releases, please discuss in [GitHub Discussions](https://
-github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.91.0 [Fix] Ignore
-FIT data items that don't have a GPS location. [#122](https://github.com/
-time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://
-github.com/patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now
-draws much more quickly. - [Change] Map rendering caches tile images more
-efficiently, so draws more quickly. - 0.89.0 [Feature] New component `cairo-
-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/
-examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-
-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there were no locked
-GPS points in the movie. - Thanks [@shahargli](https://github.com/shahargli)
-for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs,
-now fixed. Removed `alpha`, instead use alpha of each colour. - 0.86.0
-[Feature] New component `cairo-gauge-marker` - a nice clean gauge component,
-with a marker for the current value.. See docs [docs/xml/examples/06-cairo-
-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) - 0.85.0 [Feature/
-Breaking Possibly] Add validation to attributes in layout files. This may cause
-some custom layouts to break! - But they wouldn't have been working as
-intended. - [Change/Breaking] Change some `zone-bar` attribute names, aiming
-for standardisation - [Change/Breaking] Change some `cairo-circuit-map`
-attribute names, aiming for standardisation - 0.84.0 [Feature] New component
-`zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones.
-See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar) -
-Many thanks to [@jchinte](https://github.com/jchinte) for contributing! -
-0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but
-supplying input video - [Fix] Give better error message when video and GPX
-don't overlap in time, but told to sync - Thanks to [@mfloryan](https://
-github.com/mfloryan) for reporting both of these - 0.82.0 [Change] Support for
-changing units in layouts from the command line. Use `--units-speed` etc to
-control. Examples are in [docs/bin](docs/bin) - Thanks to [@matzeruegge](https:
-//github.com/matzeruegge) for the suggestion. - 0.81.0 [Fix] gopro-rename was
-broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to
-[matzeruegge](https://github.com/matzeruegge) for reporting Older changes are
-in [CHANGELOG.md](CHANGELOG.md)
+github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.92.0 [Feature] `--
+double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster
+rendering, but may not work on all architectures. Speed improvements highly
+dependent on `ffmpeg` performance. Likely much faster when using `--generate
+overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't
+have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
+raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
+[Change] Map rendering caches tile images more efficiently, so draws more
+quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
+like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
+annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
+Journey Map broke when no there were no locked GPS points in the movie. -
+Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
+Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
+instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
+gauge-marker` - a nice clean gauge component, with a marker for the current
+value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
+06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
+attributes in layout files. This may cause some custom layouts to break! - But
+they wouldn't have been working as intended. - [Change/Breaking] Change some
+`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
+Change some `cairo-circuit-map` attribute names, aiming for standardisation -
+0.84.0 [Feature] New component `zone-bar` - a 3-zone bar control that can be
+used for HR/Cadence/Power zones. See docs in [docs/xml/examples/07-zone-bar]
+(docs/xml/examples/07-zone-bar) - Many thanks to [@jchinte](https://github.com/
+jchinte) for contributing! - 0.83.0 [Change] No longer require --overlay-size
+when using --use-gpx-only, but supplying input video - [Fix] Give better error
+message when video and GPX don't overlap in time, but told to sync - Thanks to
+[@mfloryan](https://github.com/mfloryan) for reporting both of these - 0.82.0
+[Change] Support for changing units in layouts from the command line. Use `--
+units-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
+[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
+[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
+won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
+reporting Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.91.0/bin/gopro-contrib-data-extract.py` & `gopro-overlay-0.92.0/bin/gopro-contrib-data-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/bin/gopro-cut.py` & `gopro-overlay-0.92.0/bin/gopro-cut.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/bin/gopro-dashboard.py` & `gopro-overlay-0.92.0/bin/gopro-dashboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from subprocess import TimeoutExpired
 from typing import Optional
 
 import progressbar
 
 from gopro_overlay import timeseries_process, progress_frames, gpx, fit
 from gopro_overlay.arguments import gopro_dashboard_arguments
+from gopro_overlay.buffering import SingleBuffer, DoubleBuffer
 from gopro_overlay.common import temp_file_name
 from gopro_overlay.counter import ReasonCounter
 from gopro_overlay.date_overlap import DateRange
 from gopro_overlay.dimensions import dimension_from
 from gopro_overlay.execution import InProcessExecution
 from gopro_overlay.ffmpeg import FFMPEGOverlayVideo, FFMPEGOverlay, ffmpeg_is_installed, ffmpeg_libx264_is_installed, \
     find_streams, FFMPEGNull
@@ -30,15 +31,14 @@
 from gopro_overlay.point import Point
 from gopro_overlay.privacy import PrivacyZone, NoPrivacyZone
 from gopro_overlay.timeseries import Timeseries
 from gopro_overlay.timeunits import timeunits, Timeunit
 from gopro_overlay.timing import PoorTimer
 from gopro_overlay.units import units
 from gopro_overlay.widgets.profile import WidgetProfiler
-from gopro_overlay.widgets.widgets import SimpleFrameSupplier
 
 
 def accepter_from_args(include, exclude):
     if include and exclude:
         raise ValueError("Can't use both include and exclude at the same time")
 
     if include:
@@ -71,15 +71,15 @@
         return speed_awareness_layout(renderer, font=font)
     elif layout == "xml":
         return layout_from_xml(
             load_xml_layout(layout_xml), renderer, timeseries, font, privacy_zone, include=accepter,
             decorator=profiler, converters=converters
         )
     else:
-        raise ValueError(f"Unsupported layout {args.layout}")
+        raise ValueError(f"Unsupported layout {args.layout_creator}")
 
 
 def load_external(filepath: Path, units) -> Timeseries:
     suffix = filepath.suffix.lower()
     if suffix == ".gpx":
         return gpx.load_timeseries(filepath, units)
     elif suffix == ".fit":
@@ -304,39 +304,34 @@
             unit_converters = Converters(
                 speed_unit=args.units_speed,
                 distance_unit=args.units_distance,
                 altitude_unit=args.units_altitude,
                 temperature_unit=args.units_temperature,
             )
 
-            frame_supplier = SimpleFrameSupplier(dimensions=dimensions)
+            layout_creator = create_desired_layout(layout=args.layout, layout_xml=args.layout_xml, dimensions=dimensions, include=args.include, exclude=args.exclude, renderer=renderer, timeseries=frame_meta, font=font,
+                                                   privacy_zone=privacy_zone,
+                                                   profiler=profiler, converters=unit_converters)
 
-            overlay = Overlay(
-                frame=frame_supplier,
-                framemeta=frame_meta,
-                create_widgets=create_desired_layout(
-                    layout=args.layout, layout_xml=args.layout_xml,
-                    dimensions=dimensions,
-                    include=args.include, exclude=args.exclude,
-                    renderer=renderer,
-                    timeseries=frame_meta,
-                    font=font,
-                    privacy_zone=privacy_zone,
-                    profiler=profiler,
-                    converters=unit_converters
-                )
-            )
+            overlay = Overlay(framemeta=frame_meta, create_widgets=layout_creator)
 
             try:
                 with ffmpeg.generate() as writer:
-                    for index, dt in enumerate(stepper.steps()):
-                        progress.update(index)
-                        frame = draw_timer.time(lambda: overlay.draw(dt))
-                        tobytes = byte_timer.time(lambda: frame.tobytes())
-                        write_timer.time(lambda: writer.write(tobytes))
+
+                    if args.double_buffer:
+                        log("*** NOTE: Double Buffer mode is experimental. It is believed to work fine on Linux. Please raise issues if you see it working or not-working. Thanks ***")
+                        buffer = DoubleBuffer(dimensions, writer)
+                    else:
+                        buffer = SingleBuffer(dimensions, writer)
+
+                    with buffer:
+                        for index, dt in enumerate(stepper.steps()):
+                            progress.update(index)
+                            buffer.draw(lambda frame: overlay.draw(dt, frame))
+
                 log("Finished drawing frames. waiting for ffmpeg to catch up")
                 progress.finish()
 
             except KeyboardInterrupt:
                 log("...Stopping...")
                 pass
             finally:
```

### Comparing `gopro-overlay-0.91.0/bin/gopro-debug.py` & `gopro-overlay-0.92.0/bin/gopro-debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/bin/gopro-extract.py` & `gopro-overlay-0.92.0/bin/gopro-extract.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/bin/gopro-join.py` & `gopro-overlay-0.92.0/bin/gopro-join.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/bin/gopro-layout.py` & `gopro-overlay-0.92.0/bin/gopro-layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,20 +115,20 @@
                 if updated != last_updated:
                     last_updated = updated
 
                     try:
                         layout = layout_from_xml(load_xml_layout(args.file), renderer, timeseries, font, NoPrivacyZone())
 
                         overlay = Overlay(
-                            frame=SimpleFrameSupplier(dimension_from(args.overlay_size)),
                             framemeta=timeseries,
                             create_widgets=layout
                         )
 
-                        frame = overlay.draw(timeseries.mid)
+                        supplier = SimpleFrameSupplier(dimension_from(args.overlay_size))
+                        frame = overlay.draw(timeseries.mid, supplier.drawing_frame())
 
                         if video_frame is not None:
                             frame = Image.alpha_composite(video_frame, frame)
 
                         frame.save("frame.png")
                         log("Saved Image")
```

### Comparing `gopro-overlay-0.91.0/bin/gopro-rename.py` & `gopro-overlay-0.92.0/bin/gopro-rename.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/bin/gopro-to-csv.py` & `gopro-overlay-0.92.0/bin/gopro-to-csv.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/bin/gopro-to-gpx.py` & `gopro-overlay-0.92.0/bin/gopro-to-gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/arguments.py` & `gopro-overlay-0.92.0/gopro_overlay/arguments.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,16 @@
                         help="Use ffmpeg options profile <name> from ~/gopro-graphics/ffmpeg-profiles.json")
 
     parser.add_argument("--config-dir", help="Location of config files (api keys, profiles, ...)", type=pathlib.Path,
                         default=default_config_location)
     parser.add_argument("--cache-dir", help="Location of caches (map tiles, ...)", type=pathlib.Path,
                         default=default_config_location)
 
+    parser.add_argument("--double-buffer", action="store_true", help="Enable HIGHLY EXPERIMENTAL double buffering mode. May speed things up. May not work at all")
+
     only = parser.add_argument_group("GPX Only", "Creating Movies from GPX File only")
 
     only.add_argument("--use-gpx-only", "--use-fit-only", action="store_true",
                       help="Use only the GPX/FIT file - no GoPro location data")
     only.add_argument("--video-time-start", choices=["file-created", "file-modified", "file-accessed"],
                       help="Use file dates for aligning video and GPS information, only when --use-gpx-only - EXPERIMENTAL! - may be changed/removed")
     only.add_argument("--video-time-end", choices=["file-created", "file-modified", "file-accessed"],
```

### Comparing `gopro-overlay-0.91.0/gopro_overlay/common.py` & `gopro-overlay-0.92.0/gopro_overlay/common.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/dimensions.py` & `gopro-overlay-0.92.0/gopro_overlay/dimensions.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/entry.py` & `gopro-overlay-0.92.0/gopro_overlay/entry.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/execution.py` & `gopro-overlay-0.92.0/gopro_overlay/execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
                     process = self.popen(cmd, stdin=subprocess.PIPE, stdout=std, stderr=std)
             else:
                 process = self.popen(cmd, stdin=subprocess.PIPE, stdout=None, stderr=None)
 
             try:
                 yield process.stdin
             finally:
-                process.stdin.flush()
+                if not process.stdin.closed:
+                    process.stdin.flush()
             process.stdin.close()
             # really long wait as FFMPEG processes all the mpeg input file - not sure how to prevent this atm
             process.wait(5 * 60)
         except FileNotFoundError:
             raise IOError(f"Unable to execute the process - is '{cmd[0]}' installed") from None
         except BrokenPipeError:
             if self.redirect:
```

### Comparing `gopro-overlay-0.91.0/gopro_overlay/fake.py` & `gopro-overlay-0.92.0/gopro_overlay/fake.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/ffmpeg.py` & `gopro-overlay-0.92.0/gopro_overlay/ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,17 +240,20 @@
 
     def write(self, buffer) -> int:
         return len(buffer)
 
 
 class FFMPEGNull:
 
+    def __init__(self):
+        self.execution = InProcessExecution(redirect="/dev/null")
+
     @contextlib.contextmanager
     def generate(self):
-        yield DiscardingBytesIO()
+        yield from self.execution.execute(["cat"])
 
 
 class FFMPEGOverlay:
 
     def __init__(self, output: Path, overlay_size: Dimension, options: FFMPEGOptions = None, execution=None):
         self.output = output
         self.overlay_size = overlay_size
```

### Comparing `gopro-overlay-0.91.0/gopro_overlay/ffmpeg_profile.py` & `gopro-overlay-0.92.0/gopro_overlay/ffmpeg_profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/filenaming.py` & `gopro-overlay-0.92.0/gopro_overlay/filenaming.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/fit.py` & `gopro-overlay-0.92.0/gopro_overlay/fit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/framemeta.py` & `gopro-overlay-0.92.0/gopro_overlay/framemeta.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/framemeta_gpx.py` & `gopro-overlay-0.92.0/gopro_overlay/framemeta_gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/geo.py` & `gopro-overlay-0.92.0/gopro_overlay/geo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/geo_render.py` & `gopro-overlay-0.92.0/gopro_overlay/geo_render.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd_calculate.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd_calculate.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_cori.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_cori.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_debug.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_debug.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_gps.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_grav.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_grav.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpmd_visitors_xyz.py` & `gopro-overlay-0.92.0/gopro_overlay/gpmd_visitors_xyz.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/gpx.py` & `gopro-overlay-0.92.0/gopro_overlay/gpx.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/bicycle.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/car.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/car.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/faq.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/faq.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/forbidden.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/forbidden.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/gauge-1.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/gauge-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/gauge.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/gauge.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_2d.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_2d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_3d.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_3d.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_none.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_none.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/gps_lock_unknown.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/gps_lock_unknown.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/heartbeat.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/heartbeat.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/ice-cream-van.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/ice-cream-van.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/mountain-range.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/mountain-range.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/mountain.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/mountain.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/power.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/power.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/ruler.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/ruler.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/slope-triangle.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/slope-triangle.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/slope.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/slope.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/speedometer-variant-tool-symbol.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/thermometer-1.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/thermometer-1.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/thermometer.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/thermometer.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/user.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/user.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/icons/van-black-side-view.png` & `gopro-overlay-0.92.0/gopro_overlay/icons/van-black-side-view.png`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/journey.py` & `gopro-overlay-0.92.0/gopro_overlay/journey.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layout.py` & `gopro-overlay-0.92.0/gopro_overlay/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,18 @@
         ]
 
     return create
 
 
 class Overlay:
 
-    def __init__(self, frame: FrameSupplier, framemeta: FrameMeta, create_widgets: Callable):
-        self.scene = Scene(frame, create_widgets(self.entry))
+    def __init__(self, framemeta: FrameMeta, create_widgets: Callable):
+        self.scene = Scene(create_widgets(self.entry))
         self.framemeta = framemeta
         self._entry = None
 
     def entry(self):
         return self._entry
 
-    def draw(self, pts) -> Image.Image:
+    def draw(self, pts, image: Image.Image) -> Image.Image:
         self._entry = self.framemeta.get(pts)
-        return self.scene.draw()
+        return self.scene.draw(image)
```

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layout_components.py` & `gopro-overlay-0.92.0/gopro_overlay/layout_components.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layout_xml.py` & `gopro-overlay-0.92.0/gopro_overlay/layout_xml.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layout_xml_attribute.py` & `gopro-overlay-0.92.0/gopro_overlay/layout_xml_attribute.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layout_xml_cairo.py` & `gopro-overlay-0.92.0/gopro_overlay/layout_xml_cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layouts/default-1920x1080.xml` & `gopro-overlay-0.92.0/gopro_overlay/layouts/default-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layouts/default-2704x1520.xml` & `gopro-overlay-0.92.0/gopro_overlay/layouts/default-2704x1520.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layouts/default-3840x2160.xml` & `gopro-overlay-0.92.0/gopro_overlay/layouts/default-3840x2160.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layouts/example-2.xml` & `gopro-overlay-0.92.0/gopro_overlay/layouts/example-2.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layouts/example.xml` & `gopro-overlay-0.92.0/gopro_overlay/layouts/example.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/layouts/power-1920x1080.xml` & `gopro-overlay-0.92.0/gopro_overlay/layouts/power-1920x1080.xml`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/models.py` & `gopro-overlay-0.92.0/gopro_overlay/models.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/point.py` & `gopro-overlay-0.92.0/gopro_overlay/point.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/privacy.py` & `gopro-overlay-0.92.0/gopro_overlay/privacy.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/progress_frames.py` & `gopro-overlay-0.92.0/gopro_overlay/progress_frames.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/rdp.py` & `gopro-overlay-0.92.0/gopro_overlay/rdp.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/smoothing.py` & `gopro-overlay-0.92.0/gopro_overlay/smoothing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/timeseries.py` & `gopro-overlay-0.92.0/gopro_overlay/timeseries.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/timeseries_process.py` & `gopro-overlay-0.92.0/gopro_overlay/timeseries_process.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/timeunits.py` & `gopro-overlay-0.92.0/gopro_overlay/timeunits.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/timing.py` & `gopro-overlay-0.92.0/gopro_overlay/timing.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/asi.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/asi.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/bar.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/angle.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/angle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/annotation.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/annotation.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/background.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/background.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/bordered.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/bordered.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cairo.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/cairo.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/cap.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/cap.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/circuit.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/circuit.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/colour.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/colour.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/ellipse.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/ellipse.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/face.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/face.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_marker.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/gauge_marker.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/gauge_round_254.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/gauge_round_254.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/needle.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/needle.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/reading.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/reading.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/cairo/scale.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/cairo/scale.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/chart.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/chart.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/compass.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/compass.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/compass_arrow.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/compass_arrow.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/gps.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/gps.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/gradient_bar.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/gradient_bar.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/info.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/info.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/map.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/map.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/profile.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/profile.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/text.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/text.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/widgets.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,19 +234,17 @@
 
     def drawing_frame(self) -> Image:
         return Image.new("RGBA", (self._dimensions.x, self._dimensions.y), (0, 0, 0, 0))
 
 
 class Scene:
 
-    def __init__(self, frame: FrameSupplier, widgets: List[Widget]):
+    def __init__(self, widgets: List[Widget]):
         self._widgets = widgets
-        self.frame = frame
 
-    def draw(self) -> Image.Image:
-        image = self.frame.drawing_frame()
+    def draw(self, image: Image.Image) -> Image.Image:
         draw = ImageDraw.Draw(image)
 
         for w in self._widgets:
             w.draw(image, draw)
 
-        return image
+        return image
```

### Comparing `gopro-overlay-0.91.0/gopro_overlay/widgets/widgets_experimental.py` & `gopro-overlay-0.92.0/gopro_overlay/widgets/widgets_experimental.py`

 * *Files identical despite different names*

### Comparing `gopro-overlay-0.91.0/gopro_overlay.egg-info/PKG-INFO` & `gopro-overlay-0.92.0/gopro_overlay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopro-overlay
-Version: 0.91.0
+Version: 0.92.0
 Summary: Overlay graphics dashboards onto GoPro footage
 Home-page: https://github.com/time4tea/gopro-dashboard-overlay
 Author: James Richardson
 Author-email: james+gopro@time4tea.net
 License: MIT
 Project-URL: Source, https://github.com/time4tea/gopro-dashboard-overlay
 Platform: UNKNOWN
@@ -58,14 +58,15 @@
 
 
 ## Requirements
 
 
 - Python3.10
 - ffmpeg (you'll need the ffmpeg program installed)
+- libraqm (needed by [Pillow](https://pypi.org/project/Pillow/))
 - Unixy machine (probably, untested on Windows)
 
 ## Installation
 
 Install locally using `pip`, or use the provided Docker image
 
 Optional: Some widgets require the `cairo` library - which must be installed separately.
@@ -202,15 +203,15 @@
 
 ## Related Software
 
 - https://github.com/julesgraus/interactiveGoProDashboardTool - An interactive helper to build the command line for the dashboard program
 
 ## Known Bugs / Issues
 
-- Only tested on a GoPro Hero 9, that's all I have. Sample files for other devices are welcomed.
+- Only tested on a GoPro Hero 9/11, that's all I have. Sample files for other devices are welcomed.
 
 ## Icons
 
 Icon files in [icons](gopro_overlay/icons) are not covered by the MIT licence
 
 ## Map Data
 
@@ -233,14 +234,15 @@
 https://github.com/progweb/gpx2video
 
 https://github.com/JuanIrache/gopro-telemetry
 
 ## Latest Changes
 
 If you find any issues with new releases, please discuss in [GitHub Discussions](https://github.com/time4tea/gopro-dashboard-overlay/discussions)
+- 0.92.0 [Feature] `--double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster rendering, but may not work on all architectures. Speed improvements highly dependent on `ffmpeg` performance. Likely much faster when using `--generate overlay`. Feedback welcomed.
 - 0.91.0 [Fix] Ignore FIT data items that don't have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for raising.
 - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. 
 - [Change] Map rendering caches tile images more efficiently, so draws more quickly.
 - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-round-annotated)
 - 0.88.0 [Fix] Journey Map broke when no there were no locked GPS points in the movie.
   - Thanks [@shahargli](https://github.com/shahargli) for reporting
 - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`, instead use alpha of each colour.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gopro-overlay Version: 0.91.0 Summary: Overlay
+Metadata-Version: 2.1 Name: gopro-overlay Version: 0.92.0 Summary: Overlay
 graphics dashboards onto GoPro footage Home-page: https://github.com/time4tea/
 gopro-dashboard-overlay Author: James Richardson Author-email:
 james+gopro@time4tea.net License: MIT Project-URL: Source, https://github.com/
 time4tea/gopro-dashboard-overlay Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
@@ -26,111 +26,115 @@
 See [map styles](docs/maps/README.md) for more *Example* | . | . | . | . | |---
 ----------------------------------|--------------------------------------------
 ---|-------------------------------------------------------|-------------------
 ------------------------------------| | ![osm](docs/maps/map_style_osm.png) | !
 [tf-cycle](docs/maps/map_style_tf-cycle.png) | ![tf-transport](docs/maps/
 map_style_tf-transport.png) | ![tf-landscape](docs/maps/map_style_tf-
 landscape.png) | ## Requirements - Python3.10 - ffmpeg (you'll need the ffmpeg
-program installed) - Unixy machine (probably, untested on Windows) ##
-Installation Install locally using `pip`, or use the provided Docker image
-Optional: Some widgets require the `cairo` library - which must be installed
-separately. ### Installing and running with docker The docker image is a new
-thing and still a bit experimental... please file an issue if you find any
-problems. The docker image contains all you need to get started, and uses a
-volume `/work/`, which we suggest you map to the current directory which can
-contain your GoPro files. Note that the docker version doesn't support nvidia
-GPU extensions. The most recent version on docker is: [Docker] ```shell docker
-run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:  [args...] ```
-e.g. ```shell docker run -it -v "$(pwd):/work" overlaydash/gopro-dashboard-
-overlay:0.81.0 gopro-dashboard.py GH010122.MP4 render/docker.MP4 ``` Files
-created by the program will be created with the same uid that owns the mapped
-directory. You can use the `--cache-dir` and `--config-dir` command line
-arguments to configure where the cache and config dirs are, thereby making it
-easier to use persistent mapped volumes. ### Installing and running with pip
-```shell python -m venv venv venv/bin/pip install gopro-overlay ``` The Roboto
-font needs to be installed on your system. You could install it with one of the
-following commands maybe. ```bash pacman -S ttf-roboto apt install truetype-
-roboto apt install fonts-roboto ``` #### (Optional) Installing pycairo
-Optionally, install `pycairo` ```shell venv/bin/pip install pycairo==1.23.0 ```
-You might need to install some system libraries - This is what the pycairo docs
-suggest: Ubuntu/Debian: `sudo apt install libcairo2-dev pkg-config python3-dev`
-macOS/Homebrew: `brew install cairo pkg-config` ## Overlaying a dashboard
-```shell venv/bin/gopro-dashboard.py ``` The GPS track in Hero 9 (at least)
-seems to be very poor. If you supply a GPX file from a Garmin or whatever, the
-program will use this instead for the GPS. Privacy allows you to set a privacy
-zone. Various widgets will not draw points within that zone. The data recorded
-in the GoPro video will uses GPS time, which (broadly) is UTC. The renderer
-will use your local timezone to interpret this, and use the local timezone.
-This may produce strange results if you go on holiday somewhere, but then
-render the files when you get back home! On linux you can use the TZ variable
-to change the timezone that's used. ### Example For full instructions on all
-command lines see [docs/bin](docs/bin) ```shell venv/bin/gopro-dashboard.py --
-gpx ~/Downloads/Morning_Ride.gpx --privacy 52.000,-0.40000,0.50 ~/gopro/
-GH020073.MP4 GH020073-dashboard.MP4 ``` ## Writeups There's a great writeup of
-how to use the software to make an overlay from a GPX file at https://
-blog.cubieserver.de/2022/creating-gpx-overlay-videos-on-linux/ (Nov 2022) ###
-Format of the Dashboard Configuration file Several dashboards are built-in to
-the software, but the dashboard layout is highly configurable, controlled by an
-XML file. For more information on the (extensive) configurability of the layout
-please see [docs/xml](docs/xml) and lots of [examples](docs/xml/examples/
-README.md) ## FFMPEG Control & GPUs *Experimental* FFMPEG has **a lot** of
-options! This program comes with some mostly sensible defaults, but to use GPUs
-and control the output much more carefully, including framerates and bitrates,
-you can use a JSON file containing a number of 'profiles' and select the
-profile you want when running the program. For more details on how to select
-these, and an example of Nvidia GPU, please see [docs/bin](docs/bin) Please
-also see [PERFORMANCE.md](PERFORMANCE.md) ## Converting to GPX files ```shell
-venv/bin/gopro-to-gpx.py  [output-file] ``` ## Joining a sequence of MP4 files
-together Use the gopro-join.py command. Given a single file from the sequence,
-it will find and join together all the files. If you have any problems with
-this, please do raise an issue - I don't have that much test data. The joined
-file almost certainly won't work in the GoPro tools! - But it should work with
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
+it -v "$(pwd):/work" overlaydash/gopro-dashboard-overlay:0.81.0 gopro-
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
+example of Nvidia GPU, please see [docs/bin](docs/bin) Please also see
+[PERFORMANCE.md](PERFORMANCE.md) ## Converting to GPX files ```shell venv/bin/
+gopro-to-gpx.py  [output-file] ``` ## Joining a sequence of MP4 files together
+Use the gopro-join.py command. Given a single file from the sequence, it will
+find and join together all the files. If you have any problems with this,
+please do raise an issue - I don't have that much test data. The joined file
+almost certainly won't work in the GoPro tools! - But it should work with
 `gopro-dashboard.py` - I will look into the additional technical stuff required
 to make it work in the GoPro tools. *This will require a lot of disk space!*
 ```shell venv/bin/gopro-join.py /media/sdcard/DCIM/100GOPRO/GH030170.MP4 /data/
 gopro/nice-ride.MP4 ``` ## Cutting a section from a GoPro file You can cut a
 section of the gopro file, with metadata. ## Related Software - https://
 github.com/julesgraus/interactiveGoProDashboardTool - An interactive helper to
 build the command line for the dashboard program ## Known Bugs / Issues - Only
-tested on a GoPro Hero 9, that's all I have. Sample files for other devices are
-welcomed. ## Icons Icon files in [icons](gopro_overlay/icons) are not covered
-by the MIT licence ## Map Data Data Â© [OpenStreetMap contributors](http://
-www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
+tested on a GoPro Hero 9/11, that's all I have. Sample files for other devices
+are welcomed. ## Icons Icon files in [icons](gopro_overlay/icons) are not
+covered by the MIT licence ## Map Data Data Â© [OpenStreetMap contributors]
+(http://www.openstreetmap.org/copyright) Some Maps Â© [Thunderforest](http://
 www.thunderforest.com/) ## References https://github.com/juanmcasillas/
 gopro2gpx https://github.com/JuanIrache/gopro-telemetry https://github.com/
 gopro/gpmf-parser https://coderunner.io/how-to-compress-gopro-movies-and-keep-
 metadata/ ## Other Related Software https://github.com/progweb/gpx2video https:
 //github.com/JuanIrache/gopro-telemetry ## Latest Changes If you find any
 issues with new releases, please discuss in [GitHub Discussions](https://
-github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.91.0 [Fix] Ignore
-FIT data items that don't have a GPS location. [#122](https://github.com/
-time4tea/gopro-dashboard-overlay/issues/122) Thanks [@patkoscsaba](https://
-github.com/patkoscsaba) for raising. - 0.90.0 [Change] `cairo-circuit` now
-draws much more quickly. - [Change] Map rendering caches tile images more
-efficiently, so draws more quickly. - 0.89.0 [Feature] New component `cairo-
-gauge-round-annotated` - A bit like a car speedometer - See docs [docs/xml/
-examples/06-cairo-gauge-round-annotated](docs/xml/examples/06-cairo-gauge-
-round-annotated) - 0.88.0 [Fix] Journey Map broke when no there were no locked
-GPS points in the movie. - Thanks [@shahargli](https://github.com/shahargli)
-for reporting - 0.87.0 [Fix/Breaking Possibly] `chart` - discovered a few bugs,
-now fixed. Removed `alpha`, instead use alpha of each colour. - 0.86.0
-[Feature] New component `cairo-gauge-marker` - a nice clean gauge component,
-with a marker for the current value.. See docs [docs/xml/examples/06-cairo-
-gauge-marker](docs/xml/examples/06-cairo-gauge-marker) - 0.85.0 [Feature/
-Breaking Possibly] Add validation to attributes in layout files. This may cause
-some custom layouts to break! - But they wouldn't have been working as
-intended. - [Change/Breaking] Change some `zone-bar` attribute names, aiming
-for standardisation - [Change/Breaking] Change some `cairo-circuit-map`
-attribute names, aiming for standardisation - 0.84.0 [Feature] New component
-`zone-bar` - a 3-zone bar control that can be used for HR/Cadence/Power zones.
-See docs in [docs/xml/examples/07-zone-bar](docs/xml/examples/07-zone-bar) -
-Many thanks to [@jchinte](https://github.com/jchinte) for contributing! -
-0.83.0 [Change] No longer require --overlay-size when using --use-gpx-only, but
-supplying input video - [Fix] Give better error message when video and GPX
-don't overlap in time, but told to sync - Thanks to [@mfloryan](https://
-github.com/mfloryan) for reporting both of these - 0.82.0 [Change] Support for
-changing units in layouts from the command line. Use `--units-speed` etc to
-control. Examples are in [docs/bin](docs/bin) - Thanks to [@matzeruegge](https:
-//github.com/matzeruegge) for the suggestion. - 0.81.0 [Fix] gopro-rename was
-broken when using `--dirs` - added tests so hopefully won't reoccur. Thanks to
-[matzeruegge](https://github.com/matzeruegge) for reporting Older changes are
-in [CHANGELOG.md](CHANGELOG.md)
+github.com/time4tea/gopro-dashboard-overlay/discussions) - 0.92.0 [Feature] `--
+double-buffer` - EXPERIMENTAL double-buffering. Potentially much faster
+rendering, but may not work on all architectures. Speed improvements highly
+dependent on `ffmpeg` performance. Likely much faster when using `--generate
+overlay`. Feedback welcomed. - 0.91.0 [Fix] Ignore FIT data items that don't
+have a GPS location. [#122](https://github.com/time4tea/gopro-dashboard-
+overlay/issues/122) Thanks [@patkoscsaba](https://github.com/patkoscsaba) for
+raising. - 0.90.0 [Change] `cairo-circuit` now draws much more quickly. -
+[Change] Map rendering caches tile images more efficiently, so draws more
+quickly. - 0.89.0 [Feature] New component `cairo-gauge-round-annotated` - A bit
+like a car speedometer - See docs [docs/xml/examples/06-cairo-gauge-round-
+annotated](docs/xml/examples/06-cairo-gauge-round-annotated) - 0.88.0 [Fix]
+Journey Map broke when no there were no locked GPS points in the movie. -
+Thanks [@shahargli](https://github.com/shahargli) for reporting - 0.87.0 [Fix/
+Breaking Possibly] `chart` - discovered a few bugs, now fixed. Removed `alpha`,
+instead use alpha of each colour. - 0.86.0 [Feature] New component `cairo-
+gauge-marker` - a nice clean gauge component, with a marker for the current
+value.. See docs [docs/xml/examples/06-cairo-gauge-marker](docs/xml/examples/
+06-cairo-gauge-marker) - 0.85.0 [Feature/Breaking Possibly] Add validation to
+attributes in layout files. This may cause some custom layouts to break! - But
+they wouldn't have been working as intended. - [Change/Breaking] Change some
+`zone-bar` attribute names, aiming for standardisation - [Change/Breaking]
+Change some `cairo-circuit-map` attribute names, aiming for standardisation -
+0.84.0 [Feature] New component `zone-bar` - a 3-zone bar control that can be
+used for HR/Cadence/Power zones. See docs in [docs/xml/examples/07-zone-bar]
+(docs/xml/examples/07-zone-bar) - Many thanks to [@jchinte](https://github.com/
+jchinte) for contributing! - 0.83.0 [Change] No longer require --overlay-size
+when using --use-gpx-only, but supplying input video - [Fix] Give better error
+message when video and GPX don't overlap in time, but told to sync - Thanks to
+[@mfloryan](https://github.com/mfloryan) for reporting both of these - 0.82.0
+[Change] Support for changing units in layouts from the command line. Use `--
+units-speed` etc to control. Examples are in [docs/bin](docs/bin) - Thanks to
+[@matzeruegge](https://github.com/matzeruegge) for the suggestion. - 0.81.0
+[Fix] gopro-rename was broken when using `--dirs` - added tests so hopefully
+won't reoccur. Thanks to [matzeruegge](https://github.com/matzeruegge) for
+reporting Older changes are in [CHANGELOG.md](CHANGELOG.md)
```

### Comparing `gopro-overlay-0.91.0/gopro_overlay.egg-info/SOURCES.txt` & `gopro-overlay-0.92.0/gopro_overlay.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 bin/gopro-layout.py
 bin/gopro-rename.py
 bin/gopro-to-csv.py
 bin/gopro-to-gpx.py
 gopro_overlay/__init__.py
 gopro_overlay/__version__.py
 gopro_overlay/arguments.py
+gopro_overlay/buffering.py
 gopro_overlay/common.py
 gopro_overlay/counter.py
 gopro_overlay/date_overlap.py
 gopro_overlay/dimensions.py
 gopro_overlay/entry.py
 gopro_overlay/exceptions.py
 gopro_overlay/execution.py
```

### Comparing `gopro-overlay-0.91.0/setup.py` & `gopro-overlay-0.92.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 test_requirements = [
     "pytest"
 ]
 
 setup(
     name="gopro-overlay",
-    version="0.91.0",
+    version="0.92.0",
     description="Overlay graphics dashboards onto GoPro footage",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/time4tea/gopro-dashboard-overlay",
     author="James Richardson",
     author_email="james+gopro@time4tea.net",
     license="MIT",
```

