# Comparing `tmp/camerahub-0.9.7.tar.gz` & `tmp/camerahub-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub-0.9.7.tar", last modified: Fri Jun 12 20:47:43 2020, max compression
+gzip compressed data, was "camerahub-0.9.8.tar", last modified: Fri Jun 12 21:15:06 2020, max compression
```

## Comparing `camerahub-0.9.7.tar` & `camerahub-0.9.8.tar`

### file list

```diff
@@ -1,200 +1,200 @@
--rw-r--r--   0        0        0     4006 2020-06-12 20:47:35.971666 camerahub-0.9.7/README.md
--rw-r--r--   0        0        0      132 2020-06-12 20:47:35.971666 camerahub-0.9.7/camerahub/__init__.py
--rw-r--r--   0        0        0     6095 2020-06-12 20:47:35.971666 camerahub-0.9.7/camerahub/settings.py
--rw-r--r--   0        0        0     1067 2020-06-12 20:47:35.971666 camerahub-0.9.7/camerahub/urls.py
--rw-r--r--   0        0        0      395 2020-06-12 20:47:35.975666 camerahub-0.9.7/camerahub/wsgi.py
--rw-r--r--   0        0        0        0 2020-06-12 20:47:35.979667 camerahub-0.9.7/help/__init__.py
--rw-r--r--   0        0        0       64 2020-06-12 20:47:35.979667 camerahub-0.9.7/help/admin.py
--rw-r--r--   0        0        0       83 2020-06-12 20:47:35.979667 camerahub-0.9.7/help/apps.py
--rw-r--r--   0        0        0        0 2020-06-12 20:47:35.979667 camerahub-0.9.7/help/migrations/__init__.py
--rw-r--r--   0        0        0       58 2020-06-12 20:47:35.979667 camerahub-0.9.7/help/models.py
--rw-r--r--   0        0        0     4148 2020-06-12 20:47:35.979667 camerahub-0.9.7/help/templates/about.html
--rw-r--r--   0        0        0     5818 2020-06-12 20:47:35.983667 camerahub-0.9.7/help/templates/concepts.html
--rw-r--r--   0        0        0      903 2020-06-12 20:47:35.983667 camerahub-0.9.7/help/templates/condition.html
--rw-r--r--   0        0        0      232 2020-06-12 20:47:35.983667 camerahub-0.9.7/help/templates/index.html
--rw-r--r--   0        0        0       61 2020-06-12 20:47:35.983667 camerahub-0.9.7/help/tests.py
--rw-r--r--   0        0        0      482 2020-06-12 20:47:35.983667 camerahub-0.9.7/help/urls.py
--rw-r--r--   0        0        0      180 2020-06-12 20:47:35.983667 camerahub-0.9.7/help/views.py
--rw-r--r--   0        0        0     1637 2020-06-12 20:47:39.987684 camerahub-0.9.7/pyproject.toml
--rw-r--r--   0        0        0       79 2020-06-12 20:47:35.991667 camerahub-0.9.7/schema/__init__.py
--rw-r--r--   0        0        0     8974 2020-06-12 20:47:35.991667 camerahub-0.9.7/schema/admin.py
--rw-r--r--   0        0        0      923 2020-06-12 20:47:35.991667 camerahub-0.9.7/schema/apps.py
--rw-r--r--   0        0        0     6574 2020-06-12 20:47:35.991667 camerahub-0.9.7/schema/filters.py
--rw-r--r--   0        0        0     6633 2020-06-12 20:47:35.991667 camerahub-0.9.7/schema/formhelpers.py
--rw-r--r--   0        0        0    25804 2020-06-12 20:47:35.991667 camerahub-0.9.7/schema/forms.py
--rw-r--r--   0        0        0      389 2020-06-12 20:47:35.991667 camerahub-0.9.7/schema/funcs.py
--rw-r--r--   0        0        0   135096 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0001_initial.py
--rw-r--r--   0        0        0     4265 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0002_data.py
--rw-r--r--   0        0        0     4844 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0003_shutter_speeds.py
--rw-r--r--   0        0        0     9847 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0004_manufacturers.py
--rw-r--r--   0        0        0     1043 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0005_formats.py
--rw-r--r--   0        0        0     3418 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0006_negative_sizes.py
--rw-r--r--   0        0        0    10839 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0007_mounts.py
--rw-r--r--   0        0        0    10726 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0008_filmstocks.py
--rw-r--r--   0        0        0     8002 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0009_auto_20191015_0926.py
--rw-r--r--   0        0        0      504 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0010_auto_20191016_1023.py
--rw-r--r--   0        0        0      650 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0011_auto_20191016_1035.py
--rw-r--r--   0        0        0     1356 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0012_auto_20191016_1106.py
--rw-r--r--   0        0        0      301 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0013_delete_filteradapter.py
--rw-r--r--   0        0        0      369 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0014_auto_20191031_1127.py
--rw-r--r--   0        0        0      505 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0015_auto_20191107_1108.py
--rw-r--r--   0        0        0      482 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0016_auto_20191107_2005.py
--rw-r--r--   0        0        0      676 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0017_auto_20191108_1224.py
--rw-r--r--   0        0        0     6947 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0018_auto_20191217_2303.py
--rw-r--r--   0        0        0     6116 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0019_auto_20200110_1728_squashed_0020_auto_20200110_1734.py
--rw-r--r--   0        0        0      681 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0020_create_superuser.py
--rw-r--r--   0        0        0      774 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0021_auto_20200222_1856.py
--rw-r--r--   0        0        0      536 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0022_auto_20200229_1954.py
--rw-r--r--   0        0        0      499 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0023_auto_20200304_2020.py
--rw-r--r--   0        0        0      581 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0024_cameramodel_shoe.py
--rw-r--r--   0        0        0      222 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0025_convert_shoe_data.py
--rw-r--r--   0        0        0      442 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0026_auto_20200305_1032.py
--rw-r--r--   0        0        0     8120 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0027_auto_20200306_2156.py
--rw-r--r--   0        0        0      590 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0028_cameramodel_x_sync.py
--rw-r--r--   0        0        0      332 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0029_remove_paperstock_tonable.py
--rw-r--r--   0        0        0      621 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0030_auto_20200317_1344.py
--rw-r--r--   0        0        0      796 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0031_auto_20200317_1404.py
--rw-r--r--   0        0        0      417 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0032_battery_compatible_with.py
--rw-r--r--   0        0        0      607 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0033_auto_20200317_1416.py
--rw-r--r--   0        0        0      895 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0034_auto_20200317_2149.py
--rw-r--r--   0        0        0      409 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0035_cameramodel_slug.py
--rw-r--r--   0        0        0      728 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0036_cameramodel_slug.py
--rw-r--r--   0        0        0      565 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0037_auto_20200321_2101.py
--rw-r--r--   0        0        0      580 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0038_auto_20200321_2115.py
--rw-r--r--   0        0        0     1462 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0039_auto_20200321_2236.py
--rw-r--r--   0        0        0     2410 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0040_auto_20200321_2330.py
--rw-r--r--   0        0        0     3148 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0041_slugs.py
--rw-r--r--   0        0        0      490 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0042_cameramodel_mirror_lockup.py
--rw-r--r--   0        0        0      574 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0043_auto_20200323_2001.py
--rw-r--r--   0        0        0      340 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0044_remove_cameramodel_coupled_metering.py
--rw-r--r--   0        0        0     1183 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0045_auto_20200323_2203.py
--rw-r--r--   0        0        0     1337 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0046_auto_20200323_2226.py
--rw-r--r--   0        0        0     2637 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0047_auto_20200323_2236.py
--rw-r--r--   0        0        0    13093 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0048_auto_20200324_0839.py
--rw-r--r--   0        0        0     6417 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0049_auto_20200327_2231.py
--rw-r--r--   0        0        0      814 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0050_auto_20200327_2303.py
--rw-r--r--   0        0        0      508 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0051_auto_20200331_1448.py
--rw-r--r--   0        0        0      471 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0052_cameramodel_url.py
--rw-r--r--   0        0        0     2408 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0053_auto_20200427_2111.py
--rw-r--r--   0        0        0     2467 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0054_auto_20200504_2104.py
--rw-r--r--   0        0        0      537 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0055_auto_20200514_0912.py
--rw-r--r--   0        0        0     3530 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0056_auto_20200514_1120.py
--rw-r--r--   0        0        0      334 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0057_remove_camera_display_lens.py
--rw-r--r--   0        0        0      693 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0058_auto_20200517_2016.py
--rw-r--r--   0        0        0      669 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0059_auto_20200521_2050.py
--rw-r--r--   0        0        0      791 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0060_auto_20200527_1946.py
--rw-r--r--   0        0        0      900 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0061_zoom_ratio.py
--rw-r--r--   0        0        0      761 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0062_auto_20200529_2059.py
--rw-r--r--   0        0        0      786 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0063_closest_focus.py
--rw-r--r--   0        0        0      915 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/0064_auto_20200610_2131.py
--rw-r--r--   0        0        0        0 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/migrations/__init__.py
--rw-r--r--   0        0        0   103857 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/models.py
--rw-r--r--   0        0        0       76 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/static/css/styles.css
--rw-r--r--   0        0        0     3262 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/static/favicon.ico
--rw-r--r--   0        0        0     9235 2020-06-12 20:47:35.995667 camerahub-0.9.7/schema/static/logos/combinedlogo188.png
--rw-r--r--   0        0        0     1934 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/about.svg
--rw-r--r--   0        0        0     5069 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/accessory.svg
--rw-r--r--   0        0        0      641 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/add.svg
--rw-r--r--   0        0        0     1459 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/archive.svg
--rw-r--r--   0        0        0      827 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/battery.svg
--rw-r--r--   0        0        0     7738 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/bulkfilm.svg
--rw-r--r--   0        0        0     1483 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/camera.svg
--rw-r--r--   0        0        0     3070 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/cameramodel.svg
--rw-r--r--   0        0        0     2953 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/condition.svg
--rw-r--r--   0        0        0     5097 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/developer.svg
--rw-r--r--   0        0        0     1061 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/edit.svg
--rw-r--r--   0        0        0     1014 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/enlarger.svg
--rw-r--r--   0        0        0     2202 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/exhibition.svg
--rw-r--r--   0        0        0     6641 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/exposureprogram.svg
--rw-r--r--   0        0        0     1658 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/facebook.svg
--rw-r--r--   0        0        0     1237 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/film.svg
--rw-r--r--   0        0        0     1237 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/filmstock.svg
--rw-r--r--   0        0        0     8332 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/filter.svg
--rw-r--r--   0        0        0     1900 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/flash.svg
--rw-r--r--   0        0        0     3686 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/flashprotocol.svg
--rw-r--r--   0        0        0      329 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/format.svg
--rw-r--r--   0        0        0     5317 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/github.svg
--rw-r--r--   0        0        0     1651 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/help.svg
--rw-r--r--   0        0        0      837 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/home.svg
--rw-r--r--   0        0        0      936 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/icons8.svg
--rw-r--r--   0        0        0     4695 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/lens.svg
--rw-r--r--   0        0        0     4695 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/lensmodel.svg
--rw-r--r--   0        0        0      852 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/login.svg
--rw-r--r--   0        0        0     1621 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/manufacturer.svg
--rw-r--r--   0        0        0     5530 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/mount.svg
--rw-r--r--   0        0        0     3540 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/mountadapter.svg
--rw-r--r--   0        0        0      737 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/negative.svg
--rw-r--r--   0        0        0     1873 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/negativesize.svg
--rw-r--r--   0        0        0      823 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/no.svg
--rw-r--r--   0        0        0     5842 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/order.svg
--rw-r--r--   0        0        0     1903 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/paperstock.svg
--rw-r--r--   0        0        0     1534 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/password.svg
--rw-r--r--   0        0        0     3704 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/person.svg
--rw-r--r--   0        0        0     1042 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/print.svg
--rw-r--r--   0        0        0     2728 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/process.svg
--rw-r--r--   0        0        0     3738 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/register.svg
--rw-r--r--   0        0        0     4316 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/repair.svg
--rw-r--r--   0        0        0     1974 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/scan.svg
--rw-r--r--   0        0        0      771 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/search.svg
--rw-r--r--   0        0        0      963 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/shutterspeed.svg
--rw-r--r--   0        0        0      317 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/stats.svg
--rw-r--r--   0        0        0     1380 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/tag.svg
--rw-r--r--   0        0        0     4488 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/teleconverter.svg
--rw-r--r--   0        0        0     3996 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/toner.svg
--rw-r--r--   0        0        0      637 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/static/svg/yes.svg
--rw-r--r--   0        0        0    19960 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/tables.py
--rw-r--r--   0        0        0     1649 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/base.html
--rw-r--r--   0        0        0      222 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/create.html
--rw-r--r--   0        0        0      411 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/detail.html
--rw-r--r--   0        0        0      659 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/footer.html
--rw-r--r--   0        0        0      498 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/heading.html
--rw-r--r--   0        0        0     1407 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/index.html
--rw-r--r--   0        0        0      697 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/list.html
--rw-r--r--   0        0        0     6404 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/nav.html
--rw-r--r--   0        0        0     1675 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/accessory_detail.html
--rw-r--r--   0        0        0      766 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/archive_detail.html
--rw-r--r--   0        0        0     1230 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/battery_detail.html
--rw-r--r--   0        0        0     1609 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/bulkfilm_detail.html
--rw-r--r--   0        0        0     2277 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/camera_detail.html
--rw-r--r--   0        0        0    11843 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/cameramodel_detail.html
--rw-r--r--   0        0        0     1729 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/developer_detail.html
--rw-r--r--   0        0        0     1587 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/enlarger_detail.html
--rw-r--r--   0        0        0     4043 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/film_detail.html
--rw-r--r--   0        0        0     2290 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/filmstock_detail.html
--rw-r--r--   0        0        0      379 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/filter_detail.html
--rw-r--r--   0        0        0     2852 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/flash_detail.html
--rw-r--r--   0        0        0      837 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/flashprotocol_detail.html
--rw-r--r--   0        0        0      998 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/format_detail.html
--rw-r--r--   0        0        0     1859 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/lens_detail.html
--rw-r--r--   0        0        0     6595 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/lensmodel_detail.html
--rw-r--r--   0        0        0     1725 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/manufacturer_detail.html
--rw-r--r--   0        0        0       63 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/meteringtype_detail.html
--rw-r--r--   0        0        0     2580 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/mount_detail.html
--rw-r--r--   0        0        0      938 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/mountadapter_detail.html
--rw-r--r--   0        0        0     2830 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/negative_detail.html
--rw-r--r--   0        0        0     1203 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/negativesize_detail.html
--rw-r--r--   0        0        0      884 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/order_detail.html
--rw-r--r--   0        0        0     1726 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/paperstock_detail.html
--rw-r--r--   0        0        0      171 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/person_detail.html
--rw-r--r--   0        0        0     3058 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/print_detail.html
--rw-r--r--   0        0        0      928 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/process_detail.html
--rw-r--r--   0        0        0      825 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/repair_detail.html
--rw-r--r--   0        0        0      980 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/scan_detail.html
--rw-r--r--   0        0        0     1288 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/teleconverter_detail.html
--rw-r--r--   0        0        0     1570 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/schema/toner_detail.html
--rw-r--r--   0        0        0      936 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/search.html
--rw-r--r--   0        0        0      760 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/stats.html
--rw-r--r--   0        0        0      553 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/tag-detail.html
--rw-r--r--   0        0        0      512 2020-06-12 20:47:35.999667 camerahub-0.9.7/schema/templates/tag-list.html
--rw-r--r--   0        0        0      227 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/templates/update.html
--rw-r--r--   0        0        0      182 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/templates/watson/includes/search_result_item.html
--rw-r--r--   0        0        0      257 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/templates/watson/includes/search_results.html
--rw-r--r--   0        0        0        0 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/templatetags/__init__.py
--rw-r--r--   0        0        0      172 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/templatetags/boolicontag.py
--rw-r--r--   0        0        0      455 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/templatetags/model_name.py
--rw-r--r--   0        0        0      155 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/templatetags/version.py
--rw-r--r--   0        0        0       61 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/tests.py
--rw-r--r--   0        0        0    11425 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/urls.py
--rw-r--r--   0        0        0    31560 2020-06-12 20:47:36.003666 camerahub-0.9.7/schema/views.py
--rw-r--r--   0        0        0     5754 2020-06-12 20:47:43.424922 camerahub-0.9.7/setup.py
--rw-r--r--   0        0        0     6029 2020-06-12 20:47:43.426174 camerahub-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     4006 2020-06-12 21:14:56.408316 camerahub-0.9.8/README.md
+-rw-r--r--   0        0        0      132 2020-06-12 21:14:56.408316 camerahub-0.9.8/camerahub/__init__.py
+-rw-r--r--   0        0        0     6095 2020-06-12 21:14:56.408316 camerahub-0.9.8/camerahub/settings.py
+-rw-r--r--   0        0        0     1067 2020-06-12 21:14:56.408316 camerahub-0.9.8/camerahub/urls.py
+-rw-r--r--   0        0        0      395 2020-06-12 21:14:56.408316 camerahub-0.9.8/camerahub/wsgi.py
+-rw-r--r--   0        0        0        0 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/__init__.py
+-rw-r--r--   0        0        0       64 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/admin.py
+-rw-r--r--   0        0        0       83 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/apps.py
+-rw-r--r--   0        0        0        0 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/migrations/__init__.py
+-rw-r--r--   0        0        0       58 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/models.py
+-rw-r--r--   0        0        0     4148 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/templates/about.html
+-rw-r--r--   0        0        0     5818 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/templates/concepts.html
+-rw-r--r--   0        0        0      903 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/templates/condition.html
+-rw-r--r--   0        0        0      232 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/templates/index.html
+-rw-r--r--   0        0        0       61 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/tests.py
+-rw-r--r--   0        0        0      482 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/urls.py
+-rw-r--r--   0        0        0      180 2020-06-12 21:14:56.416316 camerahub-0.9.8/help/views.py
+-rw-r--r--   0        0        0     1637 2020-06-12 21:15:02.500351 camerahub-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0       79 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/__init__.py
+-rw-r--r--   0        0        0     8974 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/admin.py
+-rw-r--r--   0        0        0      923 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/apps.py
+-rw-r--r--   0        0        0     6574 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/filters.py
+-rw-r--r--   0        0        0     6633 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/formhelpers.py
+-rw-r--r--   0        0        0    25804 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/forms.py
+-rw-r--r--   0        0        0      389 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/funcs.py
+-rw-r--r--   0        0        0   135096 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4265 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0002_data.py
+-rw-r--r--   0        0        0     4844 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0003_shutter_speeds.py
+-rw-r--r--   0        0        0     9847 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0004_manufacturers.py
+-rw-r--r--   0        0        0     1043 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0005_formats.py
+-rw-r--r--   0        0        0     3418 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0006_negative_sizes.py
+-rw-r--r--   0        0        0    10839 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0007_mounts.py
+-rw-r--r--   0        0        0    10726 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0008_filmstocks.py
+-rw-r--r--   0        0        0     8002 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0009_auto_20191015_0926.py
+-rw-r--r--   0        0        0      504 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0010_auto_20191016_1023.py
+-rw-r--r--   0        0        0      650 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0011_auto_20191016_1035.py
+-rw-r--r--   0        0        0     1356 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0012_auto_20191016_1106.py
+-rw-r--r--   0        0        0      301 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0013_delete_filteradapter.py
+-rw-r--r--   0        0        0      369 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0014_auto_20191031_1127.py
+-rw-r--r--   0        0        0      505 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0015_auto_20191107_1108.py
+-rw-r--r--   0        0        0      482 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0016_auto_20191107_2005.py
+-rw-r--r--   0        0        0      676 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0017_auto_20191108_1224.py
+-rw-r--r--   0        0        0     6947 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0018_auto_20191217_2303.py
+-rw-r--r--   0        0        0     6116 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0019_auto_20200110_1728_squashed_0020_auto_20200110_1734.py
+-rw-r--r--   0        0        0      681 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0020_create_superuser.py
+-rw-r--r--   0        0        0      774 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0021_auto_20200222_1856.py
+-rw-r--r--   0        0        0      536 2020-06-12 21:14:56.424316 camerahub-0.9.8/schema/migrations/0022_auto_20200229_1954.py
+-rw-r--r--   0        0        0      499 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0023_auto_20200304_2020.py
+-rw-r--r--   0        0        0      581 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0024_cameramodel_shoe.py
+-rw-r--r--   0        0        0      222 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0025_convert_shoe_data.py
+-rw-r--r--   0        0        0      442 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0026_auto_20200305_1032.py
+-rw-r--r--   0        0        0     8120 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0027_auto_20200306_2156.py
+-rw-r--r--   0        0        0      590 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0028_cameramodel_x_sync.py
+-rw-r--r--   0        0        0      332 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0029_remove_paperstock_tonable.py
+-rw-r--r--   0        0        0      621 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0030_auto_20200317_1344.py
+-rw-r--r--   0        0        0      796 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0031_auto_20200317_1404.py
+-rw-r--r--   0        0        0      417 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0032_battery_compatible_with.py
+-rw-r--r--   0        0        0      607 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0033_auto_20200317_1416.py
+-rw-r--r--   0        0        0      895 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0034_auto_20200317_2149.py
+-rw-r--r--   0        0        0      409 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0035_cameramodel_slug.py
+-rw-r--r--   0        0        0      728 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0036_cameramodel_slug.py
+-rw-r--r--   0        0        0      565 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0037_auto_20200321_2101.py
+-rw-r--r--   0        0        0      580 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0038_auto_20200321_2115.py
+-rw-r--r--   0        0        0     1462 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0039_auto_20200321_2236.py
+-rw-r--r--   0        0        0     2410 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0040_auto_20200321_2330.py
+-rw-r--r--   0        0        0     3148 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0041_slugs.py
+-rw-r--r--   0        0        0      490 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0042_cameramodel_mirror_lockup.py
+-rw-r--r--   0        0        0      574 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0043_auto_20200323_2001.py
+-rw-r--r--   0        0        0      340 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0044_remove_cameramodel_coupled_metering.py
+-rw-r--r--   0        0        0     1183 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0045_auto_20200323_2203.py
+-rw-r--r--   0        0        0     1337 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0046_auto_20200323_2226.py
+-rw-r--r--   0        0        0     2637 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0047_auto_20200323_2236.py
+-rw-r--r--   0        0        0    13093 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0048_auto_20200324_0839.py
+-rw-r--r--   0        0        0     6417 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0049_auto_20200327_2231.py
+-rw-r--r--   0        0        0      814 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0050_auto_20200327_2303.py
+-rw-r--r--   0        0        0      508 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0051_auto_20200331_1448.py
+-rw-r--r--   0        0        0      471 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0052_cameramodel_url.py
+-rw-r--r--   0        0        0     2408 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0053_auto_20200427_2111.py
+-rw-r--r--   0        0        0     2467 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0054_auto_20200504_2104.py
+-rw-r--r--   0        0        0      537 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0055_auto_20200514_0912.py
+-rw-r--r--   0        0        0     3530 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0056_auto_20200514_1120.py
+-rw-r--r--   0        0        0      334 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0057_remove_camera_display_lens.py
+-rw-r--r--   0        0        0      693 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0058_auto_20200517_2016.py
+-rw-r--r--   0        0        0      669 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0059_auto_20200521_2050.py
+-rw-r--r--   0        0        0      791 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0060_auto_20200527_1946.py
+-rw-r--r--   0        0        0      900 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0061_zoom_ratio.py
+-rw-r--r--   0        0        0      761 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0062_auto_20200529_2059.py
+-rw-r--r--   0        0        0      786 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0063_closest_focus.py
+-rw-r--r--   0        0        0      915 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/0064_auto_20200610_2131.py
+-rw-r--r--   0        0        0        0 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/migrations/__init__.py
+-rw-r--r--   0        0        0   103857 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/models.py
+-rw-r--r--   0        0        0       76 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/css/styles.css
+-rw-r--r--   0        0        0     3262 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/favicon.ico
+-rw-r--r--   0        0        0     9235 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/logos/combinedlogo188.png
+-rw-r--r--   0        0        0     1934 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/about.svg
+-rw-r--r--   0        0        0     5069 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/accessory.svg
+-rw-r--r--   0        0        0      641 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/add.svg
+-rw-r--r--   0        0        0     1459 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/archive.svg
+-rw-r--r--   0        0        0      827 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/battery.svg
+-rw-r--r--   0        0        0     7738 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/bulkfilm.svg
+-rw-r--r--   0        0        0     1483 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/camera.svg
+-rw-r--r--   0        0        0     3070 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/cameramodel.svg
+-rw-r--r--   0        0        0     2953 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/condition.svg
+-rw-r--r--   0        0        0     5097 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/developer.svg
+-rw-r--r--   0        0        0     1061 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/edit.svg
+-rw-r--r--   0        0        0     1014 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/enlarger.svg
+-rw-r--r--   0        0        0     2202 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/exhibition.svg
+-rw-r--r--   0        0        0     6641 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/exposureprogram.svg
+-rw-r--r--   0        0        0     1658 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/facebook.svg
+-rw-r--r--   0        0        0     1237 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/film.svg
+-rw-r--r--   0        0        0     1237 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/filmstock.svg
+-rw-r--r--   0        0        0     8332 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/filter.svg
+-rw-r--r--   0        0        0     1900 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/flash.svg
+-rw-r--r--   0        0        0     3686 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/flashprotocol.svg
+-rw-r--r--   0        0        0      329 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/format.svg
+-rw-r--r--   0        0        0     5317 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/github.svg
+-rw-r--r--   0        0        0     1651 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/help.svg
+-rw-r--r--   0        0        0      837 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/home.svg
+-rw-r--r--   0        0        0      936 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/icons8.svg
+-rw-r--r--   0        0        0     4695 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/lens.svg
+-rw-r--r--   0        0        0     4695 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/lensmodel.svg
+-rw-r--r--   0        0        0      852 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/login.svg
+-rw-r--r--   0        0        0     1621 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/manufacturer.svg
+-rw-r--r--   0        0        0     5530 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/mount.svg
+-rw-r--r--   0        0        0     3540 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/mountadapter.svg
+-rw-r--r--   0        0        0      737 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/negative.svg
+-rw-r--r--   0        0        0     1873 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/negativesize.svg
+-rw-r--r--   0        0        0      823 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/no.svg
+-rw-r--r--   0        0        0     5842 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/order.svg
+-rw-r--r--   0        0        0     1903 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/paperstock.svg
+-rw-r--r--   0        0        0     1534 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/password.svg
+-rw-r--r--   0        0        0     3704 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/person.svg
+-rw-r--r--   0        0        0     1042 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/print.svg
+-rw-r--r--   0        0        0     2728 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/process.svg
+-rw-r--r--   0        0        0     3738 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/register.svg
+-rw-r--r--   0        0        0     4316 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/repair.svg
+-rw-r--r--   0        0        0     1974 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/scan.svg
+-rw-r--r--   0        0        0      771 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/search.svg
+-rw-r--r--   0        0        0      963 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/shutterspeed.svg
+-rw-r--r--   0        0        0      317 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/stats.svg
+-rw-r--r--   0        0        0     1380 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/tag.svg
+-rw-r--r--   0        0        0     4488 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/teleconverter.svg
+-rw-r--r--   0        0        0     3996 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/toner.svg
+-rw-r--r--   0        0        0      637 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/static/svg/yes.svg
+-rw-r--r--   0        0        0    19960 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/tables.py
+-rw-r--r--   0        0        0     1649 2020-06-12 21:14:56.428316 camerahub-0.9.8/schema/templates/base.html
+-rw-r--r--   0        0        0      222 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/create.html
+-rw-r--r--   0        0        0      411 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/detail.html
+-rw-r--r--   0        0        0      659 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/footer.html
+-rw-r--r--   0        0        0      498 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/heading.html
+-rw-r--r--   0        0        0     1407 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/index.html
+-rw-r--r--   0        0        0      697 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/list.html
+-rw-r--r--   0        0        0     6404 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/nav.html
+-rw-r--r--   0        0        0     1675 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/accessory_detail.html
+-rw-r--r--   0        0        0      766 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/archive_detail.html
+-rw-r--r--   0        0        0     1230 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/battery_detail.html
+-rw-r--r--   0        0        0     1609 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/bulkfilm_detail.html
+-rw-r--r--   0        0        0     2277 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/camera_detail.html
+-rw-r--r--   0        0        0    11843 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/cameramodel_detail.html
+-rw-r--r--   0        0        0     1729 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/developer_detail.html
+-rw-r--r--   0        0        0     1587 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/enlarger_detail.html
+-rw-r--r--   0        0        0     4043 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/film_detail.html
+-rw-r--r--   0        0        0     2290 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/filmstock_detail.html
+-rw-r--r--   0        0        0      379 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/filter_detail.html
+-rw-r--r--   0        0        0     2852 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/flash_detail.html
+-rw-r--r--   0        0        0      837 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/flashprotocol_detail.html
+-rw-r--r--   0        0        0      998 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/format_detail.html
+-rw-r--r--   0        0        0     1859 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/lens_detail.html
+-rw-r--r--   0        0        0     6595 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/lensmodel_detail.html
+-rw-r--r--   0        0        0     1725 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/manufacturer_detail.html
+-rw-r--r--   0        0        0       63 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/meteringtype_detail.html
+-rw-r--r--   0        0        0     2580 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/mount_detail.html
+-rw-r--r--   0        0        0      938 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/mountadapter_detail.html
+-rw-r--r--   0        0        0     2830 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/negative_detail.html
+-rw-r--r--   0        0        0     1203 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/negativesize_detail.html
+-rw-r--r--   0        0        0      884 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/order_detail.html
+-rw-r--r--   0        0        0     1726 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/paperstock_detail.html
+-rw-r--r--   0        0        0      171 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/person_detail.html
+-rw-r--r--   0        0        0     3058 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/print_detail.html
+-rw-r--r--   0        0        0      928 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/process_detail.html
+-rw-r--r--   0        0        0      825 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/repair_detail.html
+-rw-r--r--   0        0        0      980 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/scan_detail.html
+-rw-r--r--   0        0        0     1288 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/teleconverter_detail.html
+-rw-r--r--   0        0        0     1570 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/schema/toner_detail.html
+-rw-r--r--   0        0        0      936 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/search.html
+-rw-r--r--   0        0        0      760 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/stats.html
+-rw-r--r--   0        0        0      553 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/tag-detail.html
+-rw-r--r--   0        0        0      512 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/tag-list.html
+-rw-r--r--   0        0        0      227 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/update.html
+-rw-r--r--   0        0        0      182 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/watson/includes/search_result_item.html
+-rw-r--r--   0        0        0      257 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templates/watson/includes/search_results.html
+-rw-r--r--   0        0        0        0 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templatetags/__init__.py
+-rw-r--r--   0        0        0      172 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templatetags/boolicontag.py
+-rw-r--r--   0        0        0      455 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templatetags/model_name.py
+-rw-r--r--   0        0        0      155 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/templatetags/version.py
+-rw-r--r--   0        0        0       61 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/tests.py
+-rw-r--r--   0        0        0    11425 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/urls.py
+-rw-r--r--   0        0        0    31560 2020-06-12 21:14:56.432316 camerahub-0.9.8/schema/views.py
+-rw-r--r--   0        0        0     5754 2020-06-12 21:15:06.226092 camerahub-0.9.8/setup.py
+-rw-r--r--   0        0        0     6029 2020-06-12 21:15:06.227394 camerahub-0.9.8/PKG-INFO
```

### Comparing `camerahub-0.9.7/README.md` & `camerahub-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/camerahub/settings.py` & `camerahub-0.9.8/camerahub/settings.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/camerahub/urls.py` & `camerahub-0.9.8/camerahub/urls.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/help/templates/about.html` & `camerahub-0.9.8/help/templates/about.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/help/templates/concepts.html` & `camerahub-0.9.8/help/templates/concepts.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/help/templates/condition.html` & `camerahub-0.9.8/help/templates/condition.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/pyproject.toml` & `camerahub-0.9.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub"
-version = "0.9.7"
+version = "0.9.8"
 description = "App for cataloguing vintage cameras, lenses, films, negatives & prints"
 authors = ["Jonathan Gazeley <camerahub@jonathangazeley.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://camerahub.info/"
 repository = "https://github.com/djjudas21/camerahub"
 packages = [
```

### Comparing `camerahub-0.9.7/schema/admin.py` & `camerahub-0.9.8/schema/admin.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/apps.py` & `camerahub-0.9.8/schema/apps.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/filters.py` & `camerahub-0.9.8/schema/filters.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/formhelpers.py` & `camerahub-0.9.8/schema/formhelpers.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/forms.py` & `camerahub-0.9.8/schema/forms.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0001_initial.py` & `camerahub-0.9.8/schema/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0002_data.py` & `camerahub-0.9.8/schema/migrations/0002_data.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0003_shutter_speeds.py` & `camerahub-0.9.8/schema/migrations/0003_shutter_speeds.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0004_manufacturers.py` & `camerahub-0.9.8/schema/migrations/0004_manufacturers.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0005_formats.py` & `camerahub-0.9.8/schema/migrations/0005_formats.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0006_negative_sizes.py` & `camerahub-0.9.8/schema/migrations/0006_negative_sizes.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0007_mounts.py` & `camerahub-0.9.8/schema/migrations/0007_mounts.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0008_filmstocks.py` & `camerahub-0.9.8/schema/migrations/0008_filmstocks.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0009_auto_20191015_0926.py` & `camerahub-0.9.8/schema/migrations/0009_auto_20191015_0926.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0011_auto_20191016_1035.py` & `camerahub-0.9.8/schema/migrations/0011_auto_20191016_1035.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0012_auto_20191016_1106.py` & `camerahub-0.9.8/schema/migrations/0012_auto_20191016_1106.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0017_auto_20191108_1224.py` & `camerahub-0.9.8/schema/migrations/0017_auto_20191108_1224.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0018_auto_20191217_2303.py` & `camerahub-0.9.8/schema/migrations/0018_auto_20191217_2303.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0019_auto_20200110_1728_squashed_0020_auto_20200110_1734.py` & `camerahub-0.9.8/schema/migrations/0019_auto_20200110_1728_squashed_0020_auto_20200110_1734.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0020_create_superuser.py` & `camerahub-0.9.8/schema/migrations/0020_create_superuser.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0021_auto_20200222_1856.py` & `camerahub-0.9.8/schema/migrations/0021_auto_20200222_1856.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0022_auto_20200229_1954.py` & `camerahub-0.9.8/schema/migrations/0022_auto_20200229_1954.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0024_cameramodel_shoe.py` & `camerahub-0.9.8/schema/migrations/0024_cameramodel_shoe.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0027_auto_20200306_2156.py` & `camerahub-0.9.8/schema/migrations/0027_auto_20200306_2156.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0028_cameramodel_x_sync.py` & `camerahub-0.9.8/schema/migrations/0028_cameramodel_x_sync.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0030_auto_20200317_1344.py` & `camerahub-0.9.8/schema/migrations/0030_auto_20200317_1344.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0031_auto_20200317_1404.py` & `camerahub-0.9.8/schema/migrations/0031_auto_20200317_1404.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0033_auto_20200317_1416.py` & `camerahub-0.9.8/schema/migrations/0033_auto_20200317_1416.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0034_auto_20200317_2149.py` & `camerahub-0.9.8/schema/migrations/0034_auto_20200317_2149.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0036_cameramodel_slug.py` & `camerahub-0.9.8/schema/migrations/0036_cameramodel_slug.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0037_auto_20200321_2101.py` & `camerahub-0.9.8/schema/migrations/0037_auto_20200321_2101.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0038_auto_20200321_2115.py` & `camerahub-0.9.8/schema/migrations/0038_auto_20200321_2115.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0039_auto_20200321_2236.py` & `camerahub-0.9.8/schema/migrations/0039_auto_20200321_2236.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0040_auto_20200321_2330.py` & `camerahub-0.9.8/schema/migrations/0040_auto_20200321_2330.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0041_slugs.py` & `camerahub-0.9.8/schema/migrations/0041_slugs.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0043_auto_20200323_2001.py` & `camerahub-0.9.8/schema/migrations/0043_auto_20200323_2001.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0045_auto_20200323_2203.py` & `camerahub-0.9.8/schema/migrations/0045_auto_20200323_2203.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0046_auto_20200323_2226.py` & `camerahub-0.9.8/schema/migrations/0046_auto_20200323_2226.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0047_auto_20200323_2236.py` & `camerahub-0.9.8/schema/migrations/0047_auto_20200323_2236.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0048_auto_20200324_0839.py` & `camerahub-0.9.8/schema/migrations/0048_auto_20200324_0839.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0049_auto_20200327_2231.py` & `camerahub-0.9.8/schema/migrations/0049_auto_20200327_2231.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0050_auto_20200327_2303.py` & `camerahub-0.9.8/schema/migrations/0050_auto_20200327_2303.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0053_auto_20200427_2111.py` & `camerahub-0.9.8/schema/migrations/0053_auto_20200427_2111.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0054_auto_20200504_2104.py` & `camerahub-0.9.8/schema/migrations/0054_auto_20200504_2104.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0055_auto_20200514_0912.py` & `camerahub-0.9.8/schema/migrations/0055_auto_20200514_0912.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0056_auto_20200514_1120.py` & `camerahub-0.9.8/schema/migrations/0056_auto_20200514_1120.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0058_auto_20200517_2016.py` & `camerahub-0.9.8/schema/migrations/0058_auto_20200517_2016.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0059_auto_20200521_2050.py` & `camerahub-0.9.8/schema/migrations/0059_auto_20200521_2050.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0060_auto_20200527_1946.py` & `camerahub-0.9.8/schema/migrations/0060_auto_20200527_1946.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0061_zoom_ratio.py` & `camerahub-0.9.8/schema/migrations/0061_zoom_ratio.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0062_auto_20200529_2059.py` & `camerahub-0.9.8/schema/migrations/0062_auto_20200529_2059.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0063_closest_focus.py` & `camerahub-0.9.8/schema/migrations/0063_closest_focus.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/migrations/0064_auto_20200610_2131.py` & `camerahub-0.9.8/schema/migrations/0064_auto_20200610_2131.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/models.py` & `camerahub-0.9.8/schema/models.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/favicon.ico` & `camerahub-0.9.8/schema/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/logos/combinedlogo188.png` & `camerahub-0.9.8/schema/static/logos/combinedlogo188.png`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/about.svg` & `camerahub-0.9.8/schema/static/svg/about.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/accessory.svg` & `camerahub-0.9.8/schema/static/svg/accessory.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/add.svg` & `camerahub-0.9.8/schema/static/svg/add.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/archive.svg` & `camerahub-0.9.8/schema/static/svg/archive.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/battery.svg` & `camerahub-0.9.8/schema/static/svg/battery.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/bulkfilm.svg` & `camerahub-0.9.8/schema/static/svg/bulkfilm.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/camera.svg` & `camerahub-0.9.8/schema/static/svg/camera.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/cameramodel.svg` & `camerahub-0.9.8/schema/static/svg/cameramodel.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/condition.svg` & `camerahub-0.9.8/schema/static/svg/condition.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/developer.svg` & `camerahub-0.9.8/schema/static/svg/developer.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/edit.svg` & `camerahub-0.9.8/schema/static/svg/edit.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/enlarger.svg` & `camerahub-0.9.8/schema/static/svg/enlarger.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/exhibition.svg` & `camerahub-0.9.8/schema/static/svg/exhibition.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/exposureprogram.svg` & `camerahub-0.9.8/schema/static/svg/exposureprogram.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/facebook.svg` & `camerahub-0.9.8/schema/static/svg/facebook.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/film.svg` & `camerahub-0.9.8/schema/static/svg/film.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/filmstock.svg` & `camerahub-0.9.8/schema/static/svg/filmstock.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/filter.svg` & `camerahub-0.9.8/schema/static/svg/filter.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/flash.svg` & `camerahub-0.9.8/schema/static/svg/flash.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/flashprotocol.svg` & `camerahub-0.9.8/schema/static/svg/flashprotocol.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/github.svg` & `camerahub-0.9.8/schema/static/svg/github.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/help.svg` & `camerahub-0.9.8/schema/static/svg/help.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/home.svg` & `camerahub-0.9.8/schema/static/svg/home.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/icons8.svg` & `camerahub-0.9.8/schema/static/svg/icons8.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/lens.svg` & `camerahub-0.9.8/schema/static/svg/lens.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/lensmodel.svg` & `camerahub-0.9.8/schema/static/svg/lensmodel.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/login.svg` & `camerahub-0.9.8/schema/static/svg/login.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/manufacturer.svg` & `camerahub-0.9.8/schema/static/svg/manufacturer.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/mount.svg` & `camerahub-0.9.8/schema/static/svg/mount.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/mountadapter.svg` & `camerahub-0.9.8/schema/static/svg/mountadapter.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/negative.svg` & `camerahub-0.9.8/schema/static/svg/negative.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/negativesize.svg` & `camerahub-0.9.8/schema/static/svg/negativesize.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/no.svg` & `camerahub-0.9.8/schema/static/svg/no.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/order.svg` & `camerahub-0.9.8/schema/static/svg/order.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/paperstock.svg` & `camerahub-0.9.8/schema/static/svg/paperstock.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/password.svg` & `camerahub-0.9.8/schema/static/svg/password.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/person.svg` & `camerahub-0.9.8/schema/static/svg/person.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/print.svg` & `camerahub-0.9.8/schema/static/svg/print.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/process.svg` & `camerahub-0.9.8/schema/static/svg/process.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/register.svg` & `camerahub-0.9.8/schema/static/svg/register.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/repair.svg` & `camerahub-0.9.8/schema/static/svg/repair.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/scan.svg` & `camerahub-0.9.8/schema/static/svg/scan.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/search.svg` & `camerahub-0.9.8/schema/static/svg/search.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/shutterspeed.svg` & `camerahub-0.9.8/schema/static/svg/shutterspeed.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/tag.svg` & `camerahub-0.9.8/schema/static/svg/tag.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/teleconverter.svg` & `camerahub-0.9.8/schema/static/svg/teleconverter.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/toner.svg` & `camerahub-0.9.8/schema/static/svg/toner.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/static/svg/yes.svg` & `camerahub-0.9.8/schema/static/svg/yes.svg`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/tables.py` & `camerahub-0.9.8/schema/tables.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/base.html` & `camerahub-0.9.8/schema/templates/base.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/footer.html` & `camerahub-0.9.8/schema/templates/footer.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/index.html` & `camerahub-0.9.8/schema/templates/index.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/list.html` & `camerahub-0.9.8/schema/templates/list.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/nav.html` & `camerahub-0.9.8/schema/templates/nav.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/accessory_detail.html` & `camerahub-0.9.8/schema/templates/schema/accessory_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/archive_detail.html` & `camerahub-0.9.8/schema/templates/schema/archive_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/battery_detail.html` & `camerahub-0.9.8/schema/templates/schema/battery_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/bulkfilm_detail.html` & `camerahub-0.9.8/schema/templates/schema/bulkfilm_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/camera_detail.html` & `camerahub-0.9.8/schema/templates/schema/camera_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/cameramodel_detail.html` & `camerahub-0.9.8/schema/templates/schema/cameramodel_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/developer_detail.html` & `camerahub-0.9.8/schema/templates/schema/developer_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/enlarger_detail.html` & `camerahub-0.9.8/schema/templates/schema/enlarger_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/film_detail.html` & `camerahub-0.9.8/schema/templates/schema/film_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/filmstock_detail.html` & `camerahub-0.9.8/schema/templates/schema/filmstock_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/flash_detail.html` & `camerahub-0.9.8/schema/templates/schema/flash_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/flashprotocol_detail.html` & `camerahub-0.9.8/schema/templates/schema/flashprotocol_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/format_detail.html` & `camerahub-0.9.8/schema/templates/schema/format_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/lens_detail.html` & `camerahub-0.9.8/schema/templates/schema/lens_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/lensmodel_detail.html` & `camerahub-0.9.8/schema/templates/schema/lensmodel_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/manufacturer_detail.html` & `camerahub-0.9.8/schema/templates/schema/manufacturer_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/mount_detail.html` & `camerahub-0.9.8/schema/templates/schema/mount_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/mountadapter_detail.html` & `camerahub-0.9.8/schema/templates/schema/mountadapter_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/negative_detail.html` & `camerahub-0.9.8/schema/templates/schema/negative_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/negativesize_detail.html` & `camerahub-0.9.8/schema/templates/schema/negativesize_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/order_detail.html` & `camerahub-0.9.8/schema/templates/schema/order_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/paperstock_detail.html` & `camerahub-0.9.8/schema/templates/schema/paperstock_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/print_detail.html` & `camerahub-0.9.8/schema/templates/schema/print_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/process_detail.html` & `camerahub-0.9.8/schema/templates/schema/process_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/repair_detail.html` & `camerahub-0.9.8/schema/templates/schema/repair_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/scan_detail.html` & `camerahub-0.9.8/schema/templates/schema/scan_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/teleconverter_detail.html` & `camerahub-0.9.8/schema/templates/schema/teleconverter_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/schema/toner_detail.html` & `camerahub-0.9.8/schema/templates/schema/toner_detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/search.html` & `camerahub-0.9.8/schema/templates/search.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/stats.html` & `camerahub-0.9.8/schema/templates/stats.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/tag-detail.html` & `camerahub-0.9.8/schema/templates/tag-detail.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/templates/tag-list.html` & `camerahub-0.9.8/schema/templates/tag-list.html`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/urls.py` & `camerahub-0.9.8/schema/urls.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/schema/views.py` & `camerahub-0.9.8/schema/views.py`

 * *Files identical despite different names*

### Comparing `camerahub-0.9.7/setup.py` & `camerahub-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
  'uWSGI>=2.0.0,<3.0.0']
 
 extras_require = \
 {'pgsql': ['psycopg2-binary>=2.8,<3.0']}
 
 setup_kwargs = {
     'name': 'camerahub',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': 'App for cataloguing vintage cameras, lenses, films, negatives & prints',
     'long_description': '# CameraHub\n\nCameraHub is a web app for film photography that can be used to track cameras, lenses, accessories, films, negatives and prints, to fully\ncatalogue a collection of photographic equipment as well as the pictures that are made with them.\n\nIt replaces an earlier command-line project, called [PhotoDB](https://github.com/djjudas21/photodb-perl), which has now been deprecated.\n\n## Installing CameraHub\n\nThere are several ways of installing CameraHub, depending on your needs:\n\n* With Pip\n* [From source](docs/INSTALL_SOURCE.md)\n* [With Docker](docs/INSTALL-DOCKER.md)\n* [With Kubernetes](docs/INSTALL-KUBERNETES.md)\n\n## Configuring CameraHub\n\nCameraHub requires almost no additional config to run with default settings. However it is insecure in this configuration so at least `CAMERAHUB_SECRET_KEY` and\n`CAMERAHUB_PROD` must be set if you are running in production.\n\nThe following environment variables are supported:\n\n| Variable                   | Use                                                                                              | Default                      |\n|----------------------------|--------------------------------------------------------------------------------------------------|------------------------------|\n| `CAMERAHUB_ADMIN_EMAIL`    | email address for the `admin` account                                                            | `admin@example.com`          |\n| `CAMERAHUB_ADMIN_PASSWORD` | password for the `admin` account                                                                 | `admin`                      |\n| `CAMERAHUB_DB_ENGINE`      | [database engine](https://docs.djangoproject.com/en/3.0/ref/settings/#engine)                    | `django.db.backends.sqlite3` |\n| `CAMERAHUB_DB_HOST`        | [database hostname or IP address](https://docs.djangoproject.com/en/3.0/ref/settings/#host)      |                              |\n| `CAMERAHUB_DB_NAME`        | [database schema or path to SQLite db](https://docs.djangoproject.com/en/3.0/ref/settings/#name) | `db/db.sqlite3`              |\n| `CAMERAHUB_DB_PASS`        | [database password](https://docs.djangoproject.com/en/3.0/ref/settings/#password)                |                              |\n| `CAMERAHUB_DB_PORT`        | [database port](https://docs.djangoproject.com/en/3.0/ref/settings/#port)                        |                              |\n| `CAMERAHUB_DB_USER`        | [database username](https://docs.djangoproject.com/en/3.0/ref/settings/#user)                    |                              |\n| `CAMERAHUB_PROD`           | enable [Django production mode](https://docs.djangoproject.com/en/3.0/ref/settings/#debug)       | `false`                      |\n| `CAMERAHUB_SECRET_KEY`     | random secret value. Generate [here](https://miniwebtool.com/django-secret-key-generator/)       | `OverrideMe!`                |\n| `CAMERAHUB_SENDGRID_KEY`   | API key for Sendgrid email backend                                                               |                              |\n| `CAMERAHUB_FROM_EMAIL`     | [from email address](https://docs.djangoproject.com/en/3.0/ref/settings/#default-from-email)     | `noreply@camerahub.info`     |\n| `CAMERAHUB_DOMAIN`         | [site domain](https://docs.djangoproject.com/en/3.0/ref/settings/#allowed-hosts)                 | `camerahub.info`             |\n| `CAMERAHUB_REDIS`          | enable [Redis caching](https://docs.djangoproject.com/en/3.0/topics/cache/)                      | `false`                      |\n| `CAMERAHUB_REDIS_HOST`     | Redis hostname or IP address                                                                     | `127.0.0.1`                  |\n| `CAMERAHUB_REDIS_PORT`     | Redis port                                                                                       | `6379`                       |\n\n## See also\n\n* [Screenshots](docs/SCREENSHOTS.md)\n* [Contributing](docs/CONTRIBUTING.md)\n* [Changelog](https://github.com/djjudas21/camerahub/releases)\n* [Icons](docs/ICONS.md)\n',
     'author': 'Jonathan Gazeley',
     'author_email': 'camerahub@jonathangazeley.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://camerahub.info/',
```

### Comparing `camerahub-0.9.7/PKG-INFO` & `camerahub-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub
-Version: 0.9.7
+Version: 0.9.8
 Summary: App for cataloguing vintage cameras, lenses, films, negatives & prints
 Home-page: https://camerahub.info/
 License: Apache-2.0
 Author: Jonathan Gazeley
 Author-email: camerahub@jonathangazeley.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
```

