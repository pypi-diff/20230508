# Comparing `tmp/not1mm-23.5.6.tar.gz` & `tmp/not1mm-23.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.5.6.tar", last modified: Sat May  6 21:00:03 2023, max compression
+gzip compressed data, was "not1mm-23.5.7.tar", last modified: Mon May  8 01:19:53 2023, max compression
```

## Comparing `not1mm-23.5.6.tar` & `not1mm-23.5.7.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.640622 not1mm-23.5.6/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.6/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23714 2023-05-06 21:00:03.639622 not1mm-23.5.6/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22969 2023-05-06 20:55:00.000000 not1mm-23.5.6/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.540621 not1mm-23.5.6/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.6/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    77957 2023-05-06 20:37:05.000000 not1mm-23.5.6/not1mm/__main__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18633 2023-05-06 20:41:34.000000 not1mm-23.5.6/not1mm/bandmap.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.567621 not1mm-23.5.6/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.6/not1mm/data/Combinear.qss
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.6/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.6/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.6/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.6/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.6/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.6/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.6/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.6/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.6/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.6/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.6/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.6/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.6/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.6/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.6/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.6/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.6/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.6/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43767 2023-05-05 23:13:09.000000 not1mm-23.5.6/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.6/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.6/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.599622 not1mm-23.5.6/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.6/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.6/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.6/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.6/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.6/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.6/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.6/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.6/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.6/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.6/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.6/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.6/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.6/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.6/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.6/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.6/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.6/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.6/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.6/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.6/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.6/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.6/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.6/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.6/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.6/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.6/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.6/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.6/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.6/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.6/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.6/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.6/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.6/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.6/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.6/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.6/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.6/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.6/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.6/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.6/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.6/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.6/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.6/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.6/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.6/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.6/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.6/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.6/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.6/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.6/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.6/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.6/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.630622 not1mm-23.5.6/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.6/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.6/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12468 2023-04-25 15:08:00.000000 not1mm-23.5.6/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.6/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.6/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.6/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.6/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.6/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.6/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.6/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.6/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.6/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.6/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.6/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.6/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.6/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-06 20:59:18.000000 not1mm-23.5.6/not1mm/lib/version.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30050 2023-05-05 15:32:10.000000 not1mm-23.5.6/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.638622 not1mm-23.5.6/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.6/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.6/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.6/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.6/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.6/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.6/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.6/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.6/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.6/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.6/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.6/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15022 2023-05-05 16:10:06.000000 not1mm-23.5.6/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.6/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.6/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.6/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.6/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.6/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.6/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.6/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.6/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.638622 not1mm-23.5.6/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.6/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.544621 not1mm-23.5.6/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23714 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-06 21:00:03.000000 not1mm-23.5.6/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-06 20:59:08.000000 not1mm-23.5.6/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-06 21:00:03.640622 not1mm-23.5.6/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-06 21:00:03.639622 not1mm-23.5.6/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.6/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.741575 not1mm-23.5.7/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.5.7/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23934 2023-05-08 01:19:53.740575 not1mm-23.5.7/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23189 2023-05-08 01:13:10.000000 not1mm-23.5.7/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.486572 not1mm-23.5.7/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.7/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    78623 2023-05-07 16:55:25.000000 not1mm-23.5.7/not1mm/__main__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20323 2023-05-08 01:00:39.000000 not1mm-23.5.7/not1mm/bandmap.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.525573 not1mm-23.5.7/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16590 2023-02-15 20:52:35.000000 not1mm-23.5.7/not1mm/data/Combinear.qss
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.5.7/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   542666 2023-02-14 19:22:02.000000 not1mm-23.5.7/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2352 2023-04-10 21:02:17.000000 not1mm-23.5.7/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.5.7/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.5.7/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.5.7/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40156 2023-05-06 20:10:52.000000 not1mm-23.5.7/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.5.7/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4534539 2023-02-21 19:49:24.000000 not1mm-23.5.7/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.5.7/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.5.7/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.5.7/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.5.7/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.5.7/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.5.7/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.5.7/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.5.7/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.5.7/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43767 2023-05-05 23:13:09.000000 not1mm-23.5.7/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    17963 2023-05-05 12:59:56.000000 not1mm-23.5.7/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.5.7/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.686575 not1mm-23.5.7/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.5.7/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.5.7/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.5.7/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.5.7/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.5.7/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.5.7/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.5.7/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.5.7/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.5.7/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.5.7/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.5.7/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.5.7/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.5.7/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.5.7/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.5.7/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.5.7/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.5.7/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.5.7/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.5.7/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.5.7/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.5.7/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.5.7/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.5.7/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.5.7/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.5.7/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.5.7/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.5.7/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.5.7/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.5.7/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.5.7/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.5.7/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.5.7/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.5.7/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.5.7/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.5.7/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.5.7/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.5.7/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.5.7/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.5.7/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.5.7/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.5.7/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.5.7/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.5.7/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.5.7/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.5.7/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.5.7/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.5.7/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.5.7/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.5.7/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.5.7/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.5.7/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.5.7/not1mm/data/ssbmacros.txt
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.720575 not1mm-23.5.7/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.5.7/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.5.7/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13705 2023-05-07 16:50:54.000000 not1mm-23.5.7/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1772 2023-03-17 21:26:43.000000 not1mm-23.5.7/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    34193 2023-05-05 18:13:45.000000 not1mm-23.5.7/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.5.7/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.5.7/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.5.7/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.5.7/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.5.7/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.5.7/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1999 2023-04-12 19:58:03.000000 not1mm-23.5.7/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4434 2023-03-17 16:20:37.000000 not1mm-23.5.7/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.5.7/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.5.7/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6188 2023-05-06 20:36:00.000000 not1mm-23.5.7/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-05-08 01:15:23.000000 not1mm-23.5.7/not1mm/lib/version.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    30050 2023-05-05 15:32:10.000000 not1mm-23.5.7/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.738575 not1mm-23.5.7/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13746 2023-05-05 16:08:13.000000 not1mm-23.5.7/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13752 2023-05-05 16:08:31.000000 not1mm-23.5.7/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13759 2023-05-05 16:08:41.000000 not1mm-23.5.7/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13762 2023-05-05 16:08:51.000000 not1mm-23.5.7/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.5.7/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14549 2023-05-05 16:08:59.000000 not1mm-23.5.7/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14552 2023-05-05 16:09:07.000000 not1mm-23.5.7/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    12990 2023-05-05 16:10:17.000000 not1mm-23.5.7/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.5.7/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15941 2023-05-05 19:46:43.000000 not1mm-23.5.7/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15946 2023-05-05 19:54:23.000000 not1mm-23.5.7/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15022 2023-05-05 16:10:06.000000 not1mm-23.5.7/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15026 2023-05-05 16:10:01.000000 not1mm-23.5.7/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-05 16:09:55.000000 not1mm-23.5.7/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13899 2023-05-05 16:11:06.000000 not1mm-23.5.7/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14753 2023-05-05 16:11:03.000000 not1mm-23.5.7/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7453 2023-05-05 16:10:58.000000 not1mm-23.5.7/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13854 2023-05-05 16:10:55.000000 not1mm-23.5.7/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13855 2023-05-05 16:10:48.000000 not1mm-23.5.7/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3121 2023-05-05 16:11:15.000000 not1mm-23.5.7/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.739575 not1mm-23.5.7/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-05-05 15:04:14.000000 not1mm-23.5.7/not1mm/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.489572 not1mm-23.5.7/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23934 2023-05-08 01:19:53.000000 not1mm-23.5.7/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3443 2023-05-08 01:19:53.000000 not1mm-23.5.7/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-05-08 01:19:53.000000 not1mm-23.5.7/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-05-08 01:19:53.000000 not1mm-23.5.7/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       64 2023-05-08 01:19:53.000000 not1mm-23.5.7/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-05-08 01:19:53.000000 not1mm-23.5.7/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1217 2023-05-08 01:15:20.000000 not1mm-23.5.7/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-05-08 01:19:53.741575 not1mm-23.5.7/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-05-08 01:19:53.740575 not1mm-23.5.7/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2248 2023-03-07 22:04:42.000000 not1mm-23.5.7/testing/test.py
```

### Comparing `not1mm-23.5.6/LICENSE` & `not1mm-23.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/PKG-INFO` & `not1mm-23.5.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: not1mm
-Version: 23.5.6
-Summary: NOT1MM Logger
-Author-email: Michael Bridak <michael.bridak@gmail.com>
-Project-URL: Homepage, https://github.com/mbridak/not1mm
-Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Environment :: X11 Applications :: Qt
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: English
-Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Not1MM
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
@@ -119,15 +100,16 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-6] Added AR Cluster filter options for the bandmap.
+- [23-5-7] Added bandwidth marker to the bandmap.
+- [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
@@ -158,15 +140,15 @@
 - [23-3-31] Now saving station settings in the contest database.
 - [23-3-30] Added Open new and Open existing database
 - [23-3-29] Added a new contest dialog.
 - [23-3-27] Add menu item to recalculate mults.
 - [23-3-27] Fix cursor behaviour when editing text in callsign field.
 - [23-3-25] Fix minimum call length. Fix cabrillo tag. Add adif output.
 - [23-3-24] Added dupe checking. Added CAT check for flrig or rigctld. Added online flag for flrig.
-- [23-3-23] Added most of Cabrillo generation. Plan to test it this weekends CQ WPX SSB.
+- [23-3-23] Added json_data.get("cmd", "")most of Cabrillo generation. Plan to test it this weekends CQ WPX SSB.
 - [23-3-22] Add prefill of serial nr. set OP call on startup. Set IsMultiplier1 new unique wpx. Add OP and contest name to window title. and stuff.
 - [23-3-21] Worked on CQ WPX SSB plugin.
 - [23-3-20] Added a contact edit dialog. RightClick to edit contact. Changed placeholder text color in settings dialog. Hooked up CW speedchange widget. PgUp/PgDn to change speed.
 - [23-3-17] Added multicast UDP messages to update the log window when new contact made. You can now edit existing contacts in the log window. You can't delete them yet. Got rid of watchdog. Isolated common multicast code to it's own class.
 - [23-3-15] Added a rudimentary log view window.
 - [23-3-10] Started work on saving contacts to the DB. Added a claculate_wpx_prefix routine.
 - [23-3-9] Placed network call lookup in a thread. Display freq/mode for non CAT radios. Hooked up the CW macros to cwdaemon.
@@ -247,14 +229,16 @@
 
 ```bash
 not1mm
 ```
 
 ## Various data file locations
 
+json_data.get("cmd", "")
+
 ### Data
 
 If your system has an `XDG_DATA_HOME` environment variable set, the database and CW macro files can be found there. Otherwise they will be found at `yourhome/.local/share/not1mm`
 
 ### Config
 
 Configuration file(s) can be found at the location defined by `XDG_CONFIG_HOME`. Otherwise they will be found at `yourhome/.config/not1mm`
```

### Comparing `not1mm-23.5.6/README.md` & `not1mm-23.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: not1mm
+Version: 23.5.7
+Summary: NOT1MM Logger
+Author-email: Michael Bridak <michael.bridak@gmail.com>
+Project-URL: Homepage, https://github.com/mbridak/not1mm
+Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
+Classifier: Topic :: Communications :: Ham Radio
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Not1MM
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Python: 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
 [![Made With:PyQt5](https://img.shields.io/badge/Made%20with-PyQt5-red)](https://pypi.org/project/PyQt5/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/not1mm)](https://pypi.org/project/not1mm/)
 
@@ -100,15 +119,16 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-6] Added AR Cluster filter options for the bandmap.
+- [23-5-7] Added bandwidth marker to the bandmap.
+- [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
@@ -139,15 +159,15 @@
 - [23-3-31] Now saving station settings in the contest database.
 - [23-3-30] Added Open new and Open existing database
 - [23-3-29] Added a new contest dialog.
 - [23-3-27] Add menu item to recalculate mults.
 - [23-3-27] Fix cursor behaviour when editing text in callsign field.
 - [23-3-25] Fix minimum call length. Fix cabrillo tag. Add adif output.
 - [23-3-24] Added dupe checking. Added CAT check for flrig or rigctld. Added online flag for flrig.
-- [23-3-23] Added most of Cabrillo generation. Plan to test it this weekends CQ WPX SSB.
+- [23-3-23] Added json_data.get("cmd", "")most of Cabrillo generation. Plan to test it this weekends CQ WPX SSB.
 - [23-3-22] Add prefill of serial nr. set OP call on startup. Set IsMultiplier1 new unique wpx. Add OP and contest name to window title. and stuff.
 - [23-3-21] Worked on CQ WPX SSB plugin.
 - [23-3-20] Added a contact edit dialog. RightClick to edit contact. Changed placeholder text color in settings dialog. Hooked up CW speedchange widget. PgUp/PgDn to change speed.
 - [23-3-17] Added multicast UDP messages to update the log window when new contact made. You can now edit existing contacts in the log window. You can't delete them yet. Got rid of watchdog. Isolated common multicast code to it's own class.
 - [23-3-15] Added a rudimentary log view window.
 - [23-3-10] Started work on saving contacts to the DB. Added a claculate_wpx_prefix routine.
 - [23-3-9] Placed network call lookup in a thread. Display freq/mode for non CAT radios. Hooked up the CW macros to cwdaemon.
@@ -228,14 +248,16 @@
 
 ```bash
 not1mm
 ```
 
 ## Various data file locations
 
+json_data.get("cmd", "")
+
 ### Data
 
 If your system has an `XDG_DATA_HOME` environment variable set, the database and CW macro files can be found there. Otherwise they will be found at `yourhome/.local/share/not1mm`
 
 ### Config
 
 Configuration file(s) can be found at the location defined by `XDG_CONFIG_HOME`. Otherwise they will be found at `yourhome/.config/not1mm`
```

### Comparing `not1mm-23.5.6/not1mm/__main__.py` & `not1mm-23.5.7/not1mm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,4866 +8,4907 @@
 00000070: 696e 7661 6c69 642d 6e61 6d65 2c20 746f  invalid-name, to
 00000080: 6f2d 6d61 6e79 2d6c 696e 6573 2c20 6e6f  o-many-lines, no
 00000090: 2d6e 616d 652d 696e 2d6d 6f64 756c 650a  -name-in-module.
 000000a0: 0a69 6d70 6f72 7420 696d 706f 7274 6c69  .import importli
 000000b0: 620a 696d 706f 7274 206c 6f67 6769 6e67  b.import logging
 000000c0: 0a69 6d70 6f72 7420 6f73 0a69 6d70 6f72  .import os.impor
 000000d0: 7420 706b 6775 7469 6c0a 696d 706f 7274  t pkgutil.import
-000000e0: 2071 7565 7565 0a69 6d70 6f72 7420 7265   queue.import re
-000000f0: 0a69 6d70 6f72 7420 736f 636b 6574 0a69  .import socket.i
-00000100: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
-00000110: 0a69 6d70 6f72 7420 7379 730a 696d 706f  .import sys.impo
-00000120: 7274 2074 6872 6561 6469 6e67 0a69 6d70  rt threading.imp
-00000130: 6f72 7420 7469 6d65 0a69 6d70 6f72 7420  ort time.import 
-00000140: 7575 6964 0a0a 6672 6f6d 2064 6174 6574  uuid..from datet
-00000150: 696d 6520 696d 706f 7274 2064 6174 6574  ime import datet
-00000160: 696d 650a 6672 6f6d 206a 736f 6e20 696d  ime.from json im
-00000170: 706f 7274 2064 756d 7073 2c20 6c6f 6164  port dumps, load
-00000180: 732c 204a 534f 4e44 6563 6f64 6545 7272  s, JSONDecodeErr
-00000190: 6f72 0a66 726f 6d20 7061 7468 6c69 6220  or.from pathlib 
-000001a0: 696d 706f 7274 2050 6174 680a 6672 6f6d  import Path.from
-000001b0: 2073 6875 7469 6c20 696d 706f 7274 2063   shutil import c
-000001c0: 6f70 7966 696c 650a 6672 6f6d 2078 6d6c  opyfile.from xml
-000001d0: 7270 632e 636c 6965 6e74 2069 6d70 6f72  rpc.client impor
-000001e0: 7420 4572 726f 722c 2053 6572 7665 7250  t Error, ServerP
-000001f0: 726f 7879 0a0a 696d 706f 7274 2070 7375  roxy..import psu
-00000200: 7469 6c0a 6672 6f6d 2050 7951 7435 2069  til.from PyQt5 i
-00000210: 6d70 6f72 7420 5174 436f 7265 2c20 5174  mport QtCore, Qt
-00000220: 4775 692c 2051 7457 6964 6765 7473 2c20  Gui, QtWidgets, 
-00000230: 7569 630a 6672 6f6d 2050 7951 7435 2e51  uic.from PyQt5.Q
-00000240: 7457 6964 6765 7473 2069 6d70 6f72 7420  tWidgets import 
-00000250: 5146 696c 6544 6961 6c6f 670a 6672 6f6d  QFileDialog.from
-00000260: 2050 7951 7435 2e51 7443 6f72 6520 696d   PyQt5.QtCore im
-00000270: 706f 7274 2051 506f 696e 7420 2023 2070  port QPoint  # p
-00000280: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
-00000290: 6f2d 6e61 6d65 2d69 6e2d 6d6f 6475 6c65  o-name-in-module
-000002a0: 0a66 726f 6d20 5079 5174 352e 5174 436f  .from PyQt5.QtCo
-000002b0: 7265 2069 6d70 6f72 7420 5144 6972 2c20  re import QDir, 
-000002c0: 5152 6563 742c 2051 5369 7a65 2c20 5174  QRect, QSize, Qt
-000002d0: 0a66 726f 6d20 5079 5174 352e 5174 4775  .from PyQt5.QtGu
-000002e0: 6920 696d 706f 7274 2051 466f 6e74 4461  i import QFontDa
-000002f0: 7461 6261 7365 2020 2320 7079 6c69 6e74  tabase  # pylint
-00000300: 3a20 6469 7361 626c 653d 6e6f 2d6e 616d  : disable=no-nam
-00000310: 652d 696e 2d6d 6f64 756c 650a 696d 706f  e-in-module.impo
-00000320: 7274 2073 6f75 6e64 6465 7669 6365 2061  rt sounddevice a
-00000330: 7320 7364 0a69 6d70 6f72 7420 736f 756e  s sd.import soun
-00000340: 6466 696c 6520 6173 2073 660a 0a66 726f  dfile as sf..fro
-00000350: 6d20 6e6f 7431 6d6d 2e6c 6962 2e61 626f  m not1mm.lib.abo
-00000360: 7574 2069 6d70 6f72 7420 4162 6f75 740a  ut import About.
-00000370: 6672 6f6d 206e 6f74 316d 6d2e 6c69 622e  from not1mm.lib.
-00000380: 6361 745f 696e 7465 7266 6163 6520 696d  cat_interface im
-00000390: 706f 7274 2043 4154 0a66 726f 6d20 6e6f  port CAT.from no
-000003a0: 7431 6d6d 2e6c 6962 2e63 7769 6e74 6572  t1mm.lib.cwinter
-000003b0: 6661 6365 2069 6d70 6f72 7420 4357 0a66  face import CW.f
-000003c0: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e64  rom not1mm.lib.d
-000003d0: 6174 6162 6173 6520 696d 706f 7274 2044  atabase import D
-000003e0: 6174 6142 6173 650a 6672 6f6d 206e 6f74  ataBase.from not
-000003f0: 316d 6d2e 6c69 622e 6564 6974 5f6d 6163  1mm.lib.edit_mac
-00000400: 726f 2069 6d70 6f72 7420 4564 6974 4d61  ro import EditMa
-00000410: 6372 6f0a 6672 6f6d 206e 6f74 316d 6d2e  cro.from not1mm.
-00000420: 6c69 622e 6564 6974 5f6f 706f 6e20 696d  lib.edit_opon im
-00000430: 706f 7274 204f 704f 6e0a 6672 6f6d 206e  port OpOn.from n
-00000440: 6f74 316d 6d2e 6c69 622e 6564 6974 5f73  ot1mm.lib.edit_s
-00000450: 7461 7469 6f6e 2069 6d70 6f72 7420 4564  tation import Ed
-00000460: 6974 5374 6174 696f 6e0a 6672 6f6d 206e  itStation.from n
-00000470: 6f74 316d 6d2e 6c69 622e 7365 6c65 6374  ot1mm.lib.select
-00000480: 5f63 6f6e 7465 7374 2069 6d70 6f72 7420  _contest import 
-00000490: 5365 6c65 6374 436f 6e74 6573 740a 6672  SelectContest.fr
-000004a0: 6f6d 206e 6f74 316d 6d2e 6c69 622e 7365  om not1mm.lib.se
-000004b0: 7474 696e 6773 2069 6d70 6f72 7420 5365  ttings import Se
-000004c0: 7474 696e 6773 0a66 726f 6d20 6e6f 7431  ttings.from not1
-000004d0: 6d6d 2e6c 6962 2e68 616d 5f75 7469 6c69  mm.lib.ham_utili
-000004e0: 7479 2069 6d70 6f72 7420 280a 2020 2020  ty import (.    
-000004f0: 6265 6172 696e 672c 0a20 2020 2062 6561  bearing,.    bea
-00000500: 7269 6e67 5f77 6974 685f 6c61 746c 6f6e  ring_with_latlon
-00000510: 2c0a 2020 2020 6361 6c63 756c 6174 655f  ,.    calculate_
-00000520: 7770 785f 7072 6566 6978 2c0a 2020 2020  wpx_prefix,.    
-00000530: 6469 7374 616e 6365 2c0a 2020 2020 6469  distance,.    di
-00000540: 7374 616e 6365 5f77 6974 685f 6c61 746c  stance_with_latl
-00000550: 6f6e 2c0a 2020 2020 6765 745f 6c6f 6767  on,.    get_logg
-00000560: 6564 5f62 616e 642c 0a20 2020 2067 6574  ed_band,.    get
-00000570: 6261 6e64 2c0a 2020 2020 7265 6369 7072  band,.    recipr
-00000580: 6f63 6f6c 2c0a 290a 6672 6f6d 206e 6f74  ocol,.).from not
-00000590: 316d 6d2e 6c69 622e 6c6f 6f6b 7570 2069  1mm.lib.lookup i
-000005a0: 6d70 6f72 7420 5152 5a6c 6f6f 6b75 702c  mport QRZlookup,
-000005b0: 2048 616d 4442 6c6f 6f6b 7570 2c20 4861   HamDBlookup, Ha
-000005c0: 6d51 5448 0a66 726f 6d20 6e6f 7431 6d6d  mQTH.from not1mm
-000005d0: 2e6c 6962 2e6d 756c 7469 6361 7374 2069  .lib.multicast i
-000005e0: 6d70 6f72 7420 4d75 6c74 6963 6173 740a  mport Multicast.
-000005f0: 6672 6f6d 206e 6f74 316d 6d2e 6c69 622e  from not1mm.lib.
-00000600: 6e65 775f 636f 6e74 6573 7420 696d 706f  new_contest impo
-00000610: 7274 204e 6577 436f 6e74 6573 740a 6672  rt NewContest.fr
-00000620: 6f6d 206e 6f74 316d 6d2e 6c69 622e 6e31  om not1mm.lib.n1
-00000630: 6d6d 2069 6d70 6f72 7420 4e31 4d4d 0a66  mm import N1MM.f
-00000640: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e76  rom not1mm.lib.v
-00000650: 6572 7369 6f6e 2069 6d70 6f72 7420 5f5f  ersion import __
-00000660: 7665 7273 696f 6e5f 5f0a 0a6f 732e 656e  version__..os.en
-00000670: 7669 726f 6e5b 2251 545f 5150 415f 504c  viron["QT_QPA_PL
-00000680: 4154 464f 524d 5448 454d 4522 5d20 3d20  ATFORMTHEME"] = 
-00000690: 2267 6e6f 6d65 220a 2320 6f73 2e65 6e76  "gnome".# os.env
-000006a0: 6972 6f6e 5b22 5154 5f53 5459 4c45 5f4f  iron["QT_STYLE_O
-000006b0: 5645 5252 4944 4522 5d20 3d20 2261 6477  VERRIDE"] = "adw
-000006c0: 6169 7461 220a 0a6c 6f61 6465 7220 3d20  aita"..loader = 
-000006d0: 706b 6775 7469 6c2e 6765 745f 6c6f 6164  pkgutil.get_load
-000006e0: 6572 2822 6e6f 7431 6d6d 2229 0a57 4f52  er("not1mm").WOR
-000006f0: 4b49 4e47 5f50 4154 4820 3d20 6f73 2e70  KING_PATH = os.p
-00000700: 6174 682e 6469 726e 616d 6528 6c6f 6164  ath.dirname(load
-00000710: 6572 2e67 6574 5f66 696c 656e 616d 6528  er.get_filename(
-00000720: 2929 0a0a 6966 2022 5844 475f 4441 5441  ))..if "XDG_DATA
-00000730: 5f48 4f4d 4522 2069 6e20 6f73 2e65 6e76  _HOME" in os.env
-00000740: 6972 6f6e 3a0a 2020 2020 4441 5441 5f50  iron:.    DATA_P
-00000750: 4154 4820 3d20 6f73 2e65 6e76 6972 6f6e  ATH = os.environ
-00000760: 2e67 6574 2822 5844 475f 4441 5441 5f48  .get("XDG_DATA_H
-00000770: 4f4d 4522 290a 656c 7365 3a0a 2020 2020  OME").else:.    
-00000780: 4441 5441 5f50 4154 4820 3d20 7374 7228  DATA_PATH = str(
-00000790: 5061 7468 2e68 6f6d 6528 2920 2f20 222e  Path.home() / ".
-000007a0: 6c6f 6361 6c22 202f 2022 7368 6172 6522  local" / "share"
-000007b0: 290a 4441 5441 5f50 4154 4820 2b3d 2022  ).DATA_PATH += "
-000007c0: 2f6e 6f74 316d 6d22 0a74 7279 3a0a 2020  /not1mm".try:.  
-000007d0: 2020 6f73 2e6d 6b64 6972 2844 4154 415f    os.mkdir(DATA_
-000007e0: 5041 5448 290a 6578 6365 7074 2046 696c  PATH).except Fil
-000007f0: 6545 7869 7374 7345 7272 6f72 3a0a 2020  eExistsError:.  
-00000800: 2020 2e2e 2e0a 0a69 6620 2258 4447 5f43    .....if "XDG_C
-00000810: 4f4e 4649 475f 484f 4d45 2220 696e 206f  ONFIG_HOME" in o
-00000820: 732e 656e 7669 726f 6e3a 0a20 2020 2043  s.environ:.    C
-00000830: 4f4e 4649 475f 5041 5448 203d 206f 732e  ONFIG_PATH = os.
-00000840: 656e 7669 726f 6e2e 6765 7428 2258 4447  environ.get("XDG
-00000850: 5f43 4f4e 4649 475f 484f 4d45 2229 0a65  _CONFIG_HOME").e
-00000860: 6c73 653a 0a20 2020 2043 4f4e 4649 475f  lse:.    CONFIG_
-00000870: 5041 5448 203d 2073 7472 2850 6174 682e  PATH = str(Path.
-00000880: 686f 6d65 2829 202f 2022 2e63 6f6e 6669  home() / ".confi
-00000890: 6722 290a 434f 4e46 4947 5f50 4154 4820  g").CONFIG_PATH 
-000008a0: 2b3d 2022 2f6e 6f74 316d 6d22 0a74 7279  += "/not1mm".try
-000008b0: 3a0a 2020 2020 6f73 2e6d 6b64 6972 2843  :.    os.mkdir(C
-000008c0: 4f4e 4649 475f 5041 5448 290a 6578 6365  ONFIG_PATH).exce
-000008d0: 7074 2046 696c 6545 7869 7374 7345 7272  pt FileExistsErr
-000008e0: 6f72 3a0a 2020 2020 2e2e 2e0a 0a43 5459  or:.    .....CTY
-000008f0: 4649 4c45 203d 207b 7d0a 0a77 6974 6820  FILE = {}..with 
-00000900: 6f70 656e 2857 4f52 4b49 4e47 5f50 4154  open(WORKING_PAT
-00000910: 4820 2b20 222f 6461 7461 2f63 7479 2e6a  H + "/data/cty.j
-00000920: 736f 6e22 2c20 2272 7422 2c20 656e 636f  son", "rt", enco
-00000930: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
-00000940: 2063 5f66 696c 653a 0a20 2020 2043 5459   c_file:.    CTY
-00000950: 4649 4c45 203d 206c 6f61 6473 2863 5f66  FILE = loads(c_f
-00000960: 696c 652e 7265 6164 2829 290a 0a44 4152  ile.read())..DAR
-00000970: 4b5f 5354 594c 4553 4845 4554 203d 2022  K_STYLESHEET = "
-00000980: 220a 0a77 6974 6820 6f70 656e 2857 4f52  "..with open(WOR
-00000990: 4b49 4e47 5f50 4154 4820 2b20 222f 6461  KING_PATH + "/da
-000009a0: 7461 2f43 6f6d 6269 6e65 6172 2e71 7373  ta/Combinear.qss
-000009b0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-000009c0: 2d38 2229 2061 7320 7374 796c 6566 696c  -8") as stylefil
-000009d0: 653a 0a20 2020 2044 4152 4b5f 5354 594c  e:.    DARK_STYL
-000009e0: 4553 4845 4554 203d 2073 7479 6c65 6669  ESHEET = stylefi
-000009f0: 6c65 2e72 6561 6428 290a 0a0a 6465 6620  le.read()...def 
-00000a00: 6368 6563 6b5f 7072 6f63 6573 7328 6e61  check_process(na
-00000a10: 6d65 3a20 7374 7229 202d 3e20 626f 6f6c  me: str) -> bool
-00000a20: 3a0a 2020 2020 2222 2263 6865 636b 7320  :.    """checks 
-00000a30: 746f 2073 6565 2069 6620 7072 6f67 7261  to see if progra
-00000a40: 6d20 6f66 206e 616d 6520 6973 2069 6e20  m of name is in 
-00000a50: 7468 6520 6163 7469 7665 2070 726f 6365  the active proce
-00000a60: 7373 206c 6973 7422 2222 0a20 2020 2066  ss list""".    f
-00000a70: 6f72 2070 726f 6320 696e 2070 7375 7469  or proc in psuti
-00000a80: 6c2e 7072 6f63 6573 735f 6974 6572 2829  l.process_iter()
-00000a90: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
-00000aa0: 2870 726f 632e 636d 646c 696e 6528 2929  (proc.cmdline())
-00000ab0: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
-00000ac0: 2020 2069 6620 6e61 6d65 2069 6e20 7072     if name in pr
-00000ad0: 6f63 2e63 6d64 6c69 6e65 2829 5b31 5d3a  oc.cmdline()[1]:
-00000ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000af0: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00000b00: 2072 6574 7572 6e20 4661 6c73 650a 0a0a   return False...
-00000b10: 6465 6620 6374 795f 6c6f 6f6b 7570 2863  def cty_lookup(c
-00000b20: 616c 6c73 6967 6e3a 2073 7472 293a 0a20  allsign: str):. 
-00000b30: 2020 2022 2222 4c6f 6f6b 7570 2063 616c     """Lookup cal
-00000b40: 6c73 6967 6e20 696e 2063 7479 2e64 6174  lsign in cty.dat
-00000b50: 2066 696c 6522 2222 0a20 2020 2063 616c   file""".    cal
-00000b60: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
-00000b70: 2e75 7070 6572 2829 0a20 2020 2066 6f72  .upper().    for
-00000b80: 2063 6f75 6e74 2069 6e20 7265 7665 7273   count in revers
-00000b90: 6564 2872 616e 6765 286c 656e 2863 616c  ed(range(len(cal
-00000ba0: 6c73 6967 6e29 2929 3a0a 2020 2020 2020  lsign))):.      
-00000bb0: 2020 7365 6172 6368 6974 656d 203d 2063    searchitem = c
-00000bc0: 616c 6c73 6967 6e5b 3a20 636f 756e 7420  allsign[: count 
-00000bd0: 2b20 315d 0a20 2020 2020 2020 2072 6573  + 1].        res
-00000be0: 756c 7420 3d20 7b6b 6579 3a20 7661 6c20  ult = {key: val 
-00000bf0: 666f 7220 6b65 792c 2076 616c 2069 6e20  for key, val in 
-00000c00: 4354 5946 494c 452e 6974 656d 7328 2920  CTYFILE.items() 
-00000c10: 6966 206b 6579 203d 3d20 7365 6172 6368  if key == search
-00000c20: 6974 656d 7d0a 2020 2020 2020 2020 6966  item}.        if
-00000c30: 206e 6f74 2072 6573 756c 743a 0a20 2020   not result:.   
-00000c40: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00000c50: 650a 2020 2020 2020 2020 6966 2072 6573  e.        if res
-00000c60: 756c 742e 6765 7428 7365 6172 6368 6974  ult.get(searchit
-00000c70: 656d 292e 6765 7428 2265 7861 6374 5f6d  em).get("exact_m
-00000c80: 6174 6368 2229 3a0a 2020 2020 2020 2020  atch"):.        
-00000c90: 2020 2020 6966 2073 6561 7263 6869 7465      if searchite
-00000ca0: 6d20 3d3d 2063 616c 6c73 6967 6e3a 0a20  m == callsign:. 
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000cc0: 6574 7572 6e20 7265 7375 6c74 0a20 2020  eturn result.   
-00000cd0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00000ce0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00000cf0: 2072 6573 756c 740a 0a0a 636c 6173 7320   result...class 
-00000d00: 4d61 696e 5769 6e64 6f77 2851 7457 6964  MainWindow(QtWid
-00000d10: 6765 7473 2e51 4d61 696e 5769 6e64 6f77  gets.QMainWindow
-00000d20: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
-00000d30: 6865 206d 6169 6e20 7769 6e64 6f77 0a20  he main window. 
-00000d40: 2020 2022 2222 0a0a 2020 2020 7072 6566     """..    pref
-00000d50: 5f72 6566 203d 207b 0a20 2020 2020 2020  _ref = {.       
-00000d60: 2022 736f 756e 6464 6576 6963 6522 3a20   "sounddevice": 
-00000d70: 2264 6566 6175 6c74 222c 0a20 2020 2020  "default",.     
-00000d80: 2020 2022 7573 6571 727a 223a 2046 616c     "useqrz": Fal
-00000d90: 7365 2c0a 2020 2020 2020 2020 226c 6f6f  se,.        "loo
-00000da0: 6b75 7075 7365 726e 616d 6522 3a20 2275  kupusername": "u
-00000db0: 7365 726e 616d 6522 2c0a 2020 2020 2020  sername",.      
-00000dc0: 2020 226c 6f6f 6b75 7070 6173 7377 6f72    "lookuppasswor
-00000dd0: 6422 3a20 2270 6173 7377 6f72 6422 2c0a  d": "password",.
-00000de0: 2020 2020 2020 2020 2272 756e 5f73 7461          "run_sta
-00000df0: 7465 223a 2054 7275 652c 0a20 2020 2020  te": True,.     
-00000e00: 2020 2022 6461 726b 5f6d 6f64 6522 3a20     "dark_mode": 
-00000e10: 4661 6c73 652c 0a20 2020 2020 2020 2022  False,.        "
-00000e20: 636f 6d6d 616e 645f 6275 7474 6f6e 7322  command_buttons"
-00000e30: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-00000e40: 2022 6377 5f6d 6163 726f 7322 3a20 5472   "cw_macros": Tr
-00000e50: 7565 2c0a 2020 2020 2020 2020 2262 616e  ue,.        "ban
-00000e60: 6473 5f6d 6f64 6573 223a 2054 7275 652c  ds_modes": True,
-00000e70: 0a20 2020 2020 2020 2022 7769 6e64 6f77  .        "window
-00000e80: 5f68 6569 6768 7422 3a20 3230 302c 0a20  _height": 200,. 
-00000e90: 2020 2020 2020 2022 7769 6e64 6f77 5f77         "window_w
-00000ea0: 6964 7468 223a 2036 3030 2c0a 2020 2020  idth": 600,.    
-00000eb0: 2020 2020 2277 696e 646f 775f 7822 3a20      "window_x": 
-00000ec0: 3132 302c 0a20 2020 2020 2020 2022 7769  120,.        "wi
-00000ed0: 6e64 6f77 5f79 223a 2031 3230 2c0a 2020  ndow_y": 120,.  
-00000ee0: 2020 2020 2020 2263 7572 7265 6e74 5f64        "current_d
-00000ef0: 6174 6162 6173 6522 3a20 2268 616d 2e64  atabase": "ham.d
-00000f00: 6222 2c0a 2020 2020 2020 2020 2263 6f6e  b",.        "con
-00000f10: 7465 7374 223a 2022 222c 0a20 2020 2020  test": "",.     
-00000f20: 2020 2022 6d75 6c74 6963 6173 745f 6772     "multicast_gr
-00000f30: 6f75 7022 3a20 2232 3234 2e31 2e31 2e31  oup": "224.1.1.1
-00000f40: 222c 0a20 2020 2020 2020 2022 6d75 6c74  ",.        "mult
-00000f50: 6963 6173 745f 706f 7274 223a 2032 3233  icast_port": 223
-00000f60: 392c 0a20 2020 2020 2020 2022 696e 7465  9,.        "inte
-00000f70: 7266 6163 655f 6970 223a 2022 302e 302e  rface_ip": "0.0.
-00000f80: 302e 3022 2c0a 2020 2020 2020 2020 2273  0.0",.        "s
-00000f90: 656e 645f 6e31 6d6d 5f70 6163 6b65 7473  end_n1mm_packets
-00000fa0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-00000fb0: 2020 226e 316d 6d5f 7374 6174 696f 6e5f    "n1mm_station_
-00000fc0: 6e61 6d65 223a 2022 3230 4d20 4357 2054  name": "20M CW T
-00000fd0: 656e 7422 2c0a 2020 2020 2020 2020 226e  ent",.        "n
-00000fe0: 316d 6d5f 6f70 6572 6174 6f72 223a 2022  1mm_operator": "
-00000ff0: 4265 726e 6965 222c 0a20 2020 2020 2020  Bernie",.       
-00001000: 2022 6e31 6d6d 5f69 7022 3a20 2231 3237   "n1mm_ip": "127
-00001010: 2e30 2e30 2e31 222c 0a20 2020 2020 2020  .0.0.1",.       
-00001020: 2022 6e31 6d6d 5f72 6164 696f 706f 7274   "n1mm_radioport
-00001030: 223a 2031 3230 3630 2c0a 2020 2020 2020  ": 12060,.      
-00001040: 2020 226e 316d 6d5f 636f 6e74 6163 7470    "n1mm_contactp
-00001050: 6f72 7422 3a20 3132 3036 312c 0a20 2020  ort": 12061,.   
-00001060: 2020 2020 2022 6e31 6d6d 5f6c 6f6f 6b75       "n1mm_looku
-00001070: 7070 6f72 7422 3a20 3132 3036 302c 0a20  pport": 12060,. 
-00001080: 2020 2020 2020 2022 6e31 6d6d 5f73 636f         "n1mm_sco
-00001090: 7265 706f 7274 223a 2031 3230 3632 2c0a  report": 12062,.
-000010a0: 2020 2020 2020 2020 2275 7365 6861 6d64          "usehamd
-000010b0: 6222 3a20 4661 6c73 652c 0a20 2020 2020  b": False,.     
-000010c0: 2020 2022 7573 6568 616d 7174 6822 3a20     "usehamqth": 
-000010d0: 4661 6c73 652c 0a20 2020 2020 2020 2022  False,.        "
-000010e0: 636c 6f75 646c 6f67 223a 2046 616c 7365  cloudlog": False
-000010f0: 2c0a 2020 2020 2020 2020 2263 6c6f 7564  ,.        "cloud
-00001100: 6c6f 6761 7069 223a 2022 222c 0a20 2020  logapi": "",.   
-00001110: 2020 2020 2022 636c 6f75 646c 6f67 7572       "cloudlogur
-00001120: 6c22 3a20 2222 2c0a 2020 2020 2020 2020  l": "",.        
-00001130: 2243 4154 5f69 7022 3a20 2231 3237 2e30  "CAT_ip": "127.0
-00001140: 2e30 2e31 222c 0a20 2020 2020 2020 2022  .0.1",.        "
-00001150: 7573 6572 6967 6374 6c64 223a 2054 7275  userigctld": Tru
-00001160: 652c 0a20 2020 2020 2020 2022 7573 6566  e,.        "usef
-00001170: 6c72 6967 223a 2046 616c 7365 2c0a 2020  lrig": False,.  
-00001180: 2020 2020 2020 2263 7769 7022 3a20 2231        "cwip": "1
-00001190: 3237 2e30 2e30 2e31 222c 0a20 2020 2020  27.0.0.1",.     
-000011a0: 2020 2022 6377 706f 7274 223a 2036 3738     "cwport": 678
-000011b0: 392c 0a20 2020 2020 2020 2022 6377 7479  9,.        "cwty
-000011c0: 7065 223a 2031 2c0a 2020 2020 2020 2020  pe": 1,.        
-000011d0: 2275 7365 7365 7276 6572 223a 2046 616c  "useserver": Fal
-000011e0: 7365 2c0a 2020 2020 2020 2020 2243 4154  se,.        "CAT
-000011f0: 5f70 6f72 7422 3a20 3435 3332 2c0a 2020  _port": 4532,.  
-00001200: 2020 2020 2020 2263 6c75 7374 6572 5f73        "cluster_s
-00001210: 6572 7665 7222 3a20 2264 7863 2e6e 6337  erver": "dxc.nc7
-00001220: 6a2e 636f 6d22 2c0a 2020 2020 2020 2020  j.com",.        
-00001230: 2263 6c75 7374 6572 5f70 6f72 7422 3a20  "cluster_port": 
-00001240: 3733 3733 2c0a 2020 2020 2020 2020 2263  7373,.        "c
-00001250: 6c75 7374 6572 5f66 696c 7465 7222 3a20  luster_filter": 
-00001260: 2253 6574 2044 5820 4669 6c74 6572 2053  "Set DX Filter S
-00001270: 706f 7474 6572 436f 6e74 3d4e 4122 2c0a  potterCont=NA",.
-00001280: 2020 2020 2020 2020 2263 6c75 7374 6572          "cluster
-00001290: 5f6d 6f64 6522 3a20 224f 5045 4e22 2c0a  _mode": "OPEN",.
-000012a0: 2020 2020 7d0a 2020 2020 6170 7073 7461      }.    appsta
-000012b0: 7274 6564 203d 2046 616c 7365 0a20 2020  rted = False.   
-000012c0: 2063 6f6e 7461 6374 203d 207b 7d0a 2020   contact = {}.  
-000012d0: 2020 636f 6e74 6573 7420 3d20 4e6f 6e65    contest = None
-000012e0: 0a20 2020 2063 6f6e 7465 7374 5f73 6574  .    contest_set
-000012f0: 7469 6e67 7320 3d20 7b7d 0a20 2020 2070  tings = {}.    p
-00001300: 7265 6620 3d20 4e6f 6e65 0a20 2020 2073  ref = None.    s
-00001310: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
-00001320: 6375 7272 656e 745f 6f70 203d 2022 220a  current_op = "".
-00001330: 2020 2020 6375 7272 656e 745f 6d6f 6465      current_mode
-00001340: 203d 2022 220a 2020 2020 6375 7272 656e   = "".    curren
-00001350: 745f 6261 6e64 203d 2022 220a 2020 2020  t_band = "".    
-00001360: 6377 203d 204e 6f6e 650a 2020 2020 6c6f  cw = None.    lo
-00001370: 6f6b 5f75 7020 3d20 4e6f 6e65 0a20 2020  ok_up = None.   
-00001380: 2072 756e 5f73 7461 7465 203d 2046 616c   run_state = Fal
-00001390: 7365 0a20 2020 2066 6b65 7973 203d 207b  se.    fkeys = {
-000013a0: 7d0a 2020 2020 6162 6f75 745f 6469 616c  }.    about_dial
-000013b0: 6f67 203d 204e 6f6e 650a 2020 2020 7172  og = None.    qr
-000013c0: 7a5f 6469 616c 6f67 203d 204e 6f6e 650a  z_dialog = None.
-000013d0: 2020 2020 7365 7474 696e 6773 5f64 6961      settings_dia
-000013e0: 6c6f 6720 3d20 4e6f 6e65 0a20 2020 2065  log = None.    e
-000013f0: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
-00001400: 203d 204e 6f6e 650a 2020 2020 636f 6e74   = None.    cont
-00001410: 6573 745f 6469 616c 6f67 203d 204e 6f6e  est_dialog = Non
-00001420: 650a 2020 2020 636f 6e66 6967 7572 6174  e.    configurat
-00001430: 696f 6e5f 6469 616c 6f67 203d 204e 6f6e  ion_dialog = Non
-00001440: 650a 2020 2020 6f70 6f6e 5f64 6961 6c6f  e.    opon_dialo
-00001450: 6720 3d20 4e6f 6e65 0a20 2020 2064 626e  g = None.    dbn
-00001460: 616d 6520 3d20 4441 5441 5f50 4154 4820  ame = DATA_PATH 
-00001470: 2b20 222f 6861 6d2e 6462 220a 2020 2020  + "/ham.db".    
-00001480: 7261 6469 6f5f 7374 6174 6520 3d20 7b7d  radio_state = {}
-00001490: 0a20 2020 2072 6967 5f63 6f6e 7472 6f6c  .    rig_control
-000014a0: 203d 204e 6f6e 650a 2020 2020 7365 7276   = None.    serv
-000014b0: 6572 5f75 6470 203d 204e 6f6e 650a 2020  er_udp = None.  
-000014c0: 2020 6d75 6c74 6963 6173 745f 6772 6f75    multicast_grou
-000014d0: 7020 3d20 4e6f 6e65 0a20 2020 206d 756c  p = None.    mul
-000014e0: 7469 6361 7374 5f70 6f72 7420 3d20 4e6f  ticast_port = No
-000014f0: 6e65 0a20 2020 2069 6e74 6572 6661 6365  ne.    interface
-00001500: 5f69 7020 3d20 4e6f 6e65 0a20 2020 2072  _ip = None.    r
-00001510: 6967 5f63 6f6e 7472 6f6c 203d 204e 6f6e  ig_control = Non
-00001520: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
-00001530: 745f 5f28 7365 6c66 2c20 2a61 7267 732c  t__(self, *args,
-00001540: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00001550: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00001560: 6974 5f5f 282a 6172 6773 2c20 2a2a 6b77  it__(*args, **kw
-00001570: 6172 6773 290a 2020 2020 2020 2020 6c6f  args).        lo
-00001580: 6767 6572 2e69 6e66 6f28 224d 6169 6e57  gger.info("MainW
-00001590: 696e 646f 773a 205f 5f69 6e69 745f 5f22  indow: __init__"
-000015a0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-000015b0: 7564 7077 6174 6368 203d 204e 6f6e 650a  udpwatch = None.
-000015c0: 2020 2020 2020 2020 7365 6c66 2e75 6470          self.udp
-000015d0: 5f66 6966 6f20 3d20 7175 6575 652e 5175  _fifo = queue.Qu
-000015e0: 6575 6528 290a 2020 2020 2020 2020 6461  eue().        da
-000015f0: 7461 5f70 6174 6820 3d20 574f 524b 494e  ta_path = WORKIN
-00001600: 475f 5041 5448 202b 2022 2f64 6174 612f  G_PATH + "/data/
-00001610: 6d61 696e 2e75 6922 0a20 2020 2020 2020  main.ui".       
-00001620: 2075 6963 2e6c 6f61 6455 6928 6461 7461   uic.loadUi(data
-00001630: 5f70 6174 682c 2073 656c 6629 0a20 2020  _path, self).   
-00001640: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
-00001650: 742e 6869 6465 2829 0a20 2020 2020 2020  t.hide().       
-00001660: 2073 656c 662e 7269 6768 7464 6f74 2e68   self.rightdot.h
-00001670: 6964 6528 290a 2020 2020 2020 2020 7365  ide().        se
-00001680: 6c66 2e6e 316d 6d20 3d20 4e31 4d4d 2829  lf.n1mm = N1MM()
-00001690: 0a20 2020 2020 2020 2073 656c 662e 6e65  .        self.ne
-000016a0: 7874 5f66 6965 6c64 203d 2073 656c 662e  xt_field = self.
-000016b0: 6f74 6865 725f 320a 2020 2020 2020 2020  other_2.        
-000016c0: 7365 6c66 2e64 7570 655f 696e 6469 6361  self.dupe_indica
-000016d0: 746f 722e 6869 6465 2829 0a20 2020 2020  tor.hide().     
-000016e0: 2020 2073 656c 662e 6377 5f73 7065 6564     self.cw_speed
-000016f0: 2e76 616c 7565 4368 616e 6765 642e 636f  .valueChanged.co
-00001700: 6e6e 6563 7428 7365 6c66 2e63 7773 7065  nnect(self.cwspe
-00001710: 6564 5f73 7069 6e62 6f78 5f63 6861 6e67  ed_spinbox_chang
-00001720: 6564 290a 0a20 2020 2020 2020 2073 656c  ed)..        sel
-00001730: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
-00001740: 732e 7472 6967 6765 7265 642e 636f 6e6e  s.triggered.conn
-00001750: 6563 7428 7365 6c66 2e63 775f 6d61 6372  ect(self.cw_macr
-00001760: 6f73 5f73 7461 7465 5f63 6861 6e67 6564  os_state_changed
-00001770: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00001780: 6374 696f 6e43 6f6d 6d61 6e64 5f42 7574  ctionCommand_But
-00001790: 746f 6e73 2e74 7269 6767 6572 6564 2e63  tons.triggered.c
-000017a0: 6f6e 6e65 6374 2873 656c 662e 636f 6d6d  onnect(self.comm
-000017b0: 616e 645f 6275 7474 6f6e 735f 7374 6174  and_buttons_stat
-000017c0: 655f 6368 616e 6765 290a 2020 2020 2020  e_change).      
-000017d0: 2020 7365 6c66 2e61 6374 696f 6e44 6172    self.actionDar
-000017e0: 6b5f 4d6f 6465 2e74 7269 6767 6572 6564  k_Mode.triggered
-000017f0: 2e63 6f6e 6e65 6374 2873 656c 662e 6461  .connect(self.da
-00001800: 726b 5f6d 6f64 655f 7374 6174 655f 6368  rk_mode_state_ch
-00001810: 616e 6765 290a 2020 2020 2020 2020 7365  ange).        se
-00001820: 6c66 2e61 6374 696f 6e4c 6f67 5f57 696e  lf.actionLog_Win
-00001830: 646f 772e 7472 6967 6765 7265 642e 636f  dow.triggered.co
-00001840: 6e6e 6563 7428 7365 6c66 2e6c 6175 6e63  nnect(self.launc
-00001850: 685f 6c6f 675f 7769 6e64 6f77 290a 2020  h_log_window).  
-00001860: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001870: 6e42 616e 646d 6170 2e74 7269 6767 6572  nBandmap.trigger
-00001880: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00001890: 6c61 756e 6368 5f62 616e 646d 6170 5f77  launch_bandmap_w
-000018a0: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
-000018b0: 656c 662e 6163 7469 6f6e 5265 6361 6c63  elf.actionRecalc
-000018c0: 756c 6174 655f 4d75 6c74 732e 7472 6967  ulate_Mults.trig
-000018d0: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
-000018e0: 6c66 2e72 6563 616c 6375 6c61 7465 5f6d  lf.recalculate_m
-000018f0: 756c 7473 290a 0a20 2020 2020 2020 2073  ults)..        s
-00001900: 656c 662e 6163 7469 6f6e 4765 6e65 7261  elf.actionGenera
-00001910: 7465 5f43 6162 7269 6c6c 6f2e 7472 6967  te_Cabrillo.trig
-00001920: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
-00001930: 6c66 2e67 656e 6572 6174 655f 6361 6272  lf.generate_cabr
-00001940: 696c 6c6f 290a 2020 2020 2020 2020 7365  illo).        se
-00001950: 6c66 2e61 6374 696f 6e47 656e 6572 6174  lf.actionGenerat
-00001960: 655f 4144 4946 2e74 7269 6767 6572 6564  e_ADIF.triggered
-00001970: 2e63 6f6e 6e65 6374 2873 656c 662e 6765  .connect(self.ge
-00001980: 6e65 7261 7465 5f61 6469 6629 0a0a 2020  nerate_adif)..  
-00001990: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-000019a0: 6e43 6f6e 6669 6775 7261 7469 6f6e 5f53  nConfiguration_S
-000019b0: 6574 7469 6e67 732e 7472 6967 6765 7265  ettings.triggere
-000019c0: 642e 636f 6e6e 6563 7428 0a20 2020 2020  d.connect(.     
-000019d0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-000019e0: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f73  _configuration_s
-000019f0: 6574 7469 6e67 730a 2020 2020 2020 2020  ettings.        
-00001a00: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00001a10: 6374 696f 6e53 7461 7469 6f6e 5365 7474  ctionStationSett
-00001a20: 696e 6773 2e74 7269 6767 6572 6564 2e63  ings.triggered.c
-00001a30: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
-00001a40: 5f73 7461 7469 6f6e 5f73 6574 7469 6e67  _station_setting
-00001a50: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
-00001a60: 2e61 6374 696f 6e4e 6577 5f43 6f6e 7465  .actionNew_Conte
-00001a70: 7374 2e74 7269 6767 6572 6564 2e63 6f6e  st.triggered.con
-00001a80: 6e65 6374 2873 656c 662e 6e65 775f 636f  nect(self.new_co
-00001a90: 6e74 6573 745f 6469 616c 6f67 290a 2020  ntest_dialog).  
-00001aa0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001ab0: 6e4f 7065 6e5f 436f 6e74 6573 742e 7472  nOpen_Contest.tr
-00001ac0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001ad0: 7365 6c66 2e6f 7065 6e5f 636f 6e74 6573  self.open_contes
-00001ae0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-00001af0: 6163 7469 6f6e 4564 6974 5f43 7572 7265  actionEdit_Curre
-00001b00: 6e74 5f43 6f6e 7465 7374 2e74 7269 6767  nt_Contest.trigg
-00001b10: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
-00001b20: 662e 6564 6974 5f63 6f6e 7465 7374 290a  f.edit_contest).
-00001b30: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
-00001b40: 7469 6f6e 4e65 775f 4461 7461 6261 7365  tionNew_Database
-00001b50: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
-00001b60: 6374 2873 656c 662e 6e65 775f 6461 7461  ct(self.new_data
-00001b70: 6261 7365 290a 2020 2020 2020 2020 7365  base).        se
-00001b80: 6c66 2e61 6374 696f 6e4f 7065 6e5f 4461  lf.actionOpen_Da
-00001b90: 7461 6261 7365 2e74 7269 6767 6572 6564  tabase.triggered
-00001ba0: 2e63 6f6e 6e65 6374 2873 656c 662e 6f70  .connect(self.op
-00001bb0: 656e 5f64 6174 6162 6173 6529 0a0a 2020  en_database)..  
-00001bc0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001bd0: 6e45 6469 745f 4d61 6372 6f73 2e74 7269  nEdit_Macros.tri
-00001be0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-00001bf0: 656c 662e 6564 6974 5f63 775f 6d61 6372  elf.edit_cw_macr
-00001c00: 6f73 290a 0a20 2020 2020 2020 2073 656c  os)..        sel
-00001c10: 662e 6163 7469 6f6e 4162 6f75 742e 7472  f.actionAbout.tr
-00001c20: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001c30: 7365 6c66 2e73 686f 775f 6162 6f75 745f  self.show_about_
-00001c40: 6469 616c 6f67 290a 0a20 2020 2020 2020  dialog)..       
-00001c50: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
-00001c60: 6e5f 7275 6e2e 636c 6963 6b65 642e 636f  n_run.clicked.co
-00001c70: 6e6e 6563 7428 7365 6c66 2e72 756e 5f73  nnect(self.run_s
-00001c80: 705f 6275 7474 6f6e 735f 636c 6963 6b65  p_buttons_clicke
-00001c90: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00001ca0: 7261 6469 6f42 7574 746f 6e5f 7370 2e63  radioButton_sp.c
-00001cb0: 6c69 636b 6564 2e63 6f6e 6e65 6374 2873  licked.connect(s
-00001cc0: 656c 662e 7275 6e5f 7370 5f62 7574 746f  elf.run_sp_butto
-00001cd0: 6e73 5f63 6c69 636b 6564 290a 2020 2020  ns_clicked).    
-00001ce0: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
-00001cf0: 6574 5465 7874 2822 3022 290a 2020 2020  etText("0").    
-00001d00: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-00001d10: 6e2e 7465 7874 4564 6974 6564 2e63 6f6e  n.textEdited.con
-00001d20: 6e65 6374 2873 656c 662e 6361 6c6c 7369  nect(self.callsi
-00001d30: 676e 5f63 6861 6e67 6564 290a 2020 2020  gn_changed).    
-00001d40: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-00001d50: 6e2e 7265 7475 726e 5072 6573 7365 642e  n.returnPressed.
-00001d60: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
-00001d70: 655f 636f 6e74 6163 7429 0a20 2020 2020  e_contact).     
-00001d80: 2020 2073 656c 662e 7365 6e74 2e72 6574     self.sent.ret
-00001d90: 7572 6e50 7265 7373 6564 2e63 6f6e 6e65  urnPressed.conne
-00001da0: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
-00001db0: 7461 6374 290a 2020 2020 2020 2020 7365  tact).        se
-00001dc0: 6c66 2e72 6563 6569 7665 2e72 6574 7572  lf.receive.retur
-00001dd0: 6e50 7265 7373 6564 2e63 6f6e 6e65 6374  nPressed.connect
-00001de0: 2873 656c 662e 7361 7665 5f63 6f6e 7461  (self.save_conta
-00001df0: 6374 290a 2020 2020 2020 2020 7365 6c66  ct).        self
-00001e00: 2e6f 7468 6572 5f31 2e72 6574 7572 6e50  .other_1.returnP
-00001e10: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
-00001e20: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
-00001e30: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
-00001e40: 7468 6572 5f32 2e72 6574 7572 6e50 7265  ther_2.returnPre
-00001e50: 7373 6564 2e63 6f6e 6e65 6374 2873 656c  ssed.connect(sel
-00001e60: 662e 7361 7665 5f63 6f6e 7461 6374 290a  f.save_contact).
-00001e70: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
-00001e80: 6572 5f32 2e74 6578 7445 6469 7465 642e  er_2.textEdited.
-00001e90: 636f 6e6e 6563 7428 7365 6c66 2e6f 7468  connect(self.oth
-00001ea0: 6572 5f32 5f63 6861 6e67 6564 290a 2020  er_2_changed).  
-00001eb0: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
-00001ec0: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
-00001ed0: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
-00001ee0: 7665 2e73 6574 5465 7874 2822 3539 2229  ve.setText("59")
-00001ef0: 0a20 2020 2020 2020 2069 636f 6e5f 7061  .        icon_pa
-00001f00: 7468 203d 2057 4f52 4b49 4e47 5f50 4154  th = WORKING_PAT
-00001f10: 4820 2b20 222f 6461 7461 2f22 0a20 2020  H + "/data/".   
-00001f20: 2020 2020 2073 656c 662e 6772 6565 6e64       self.greend
-00001f30: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
-00001f40: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
-00001f50: 6772 6565 6e64 6f74 2e70 6e67 2229 0a20  greendot.png"). 
-00001f60: 2020 2020 2020 2073 656c 662e 7265 6464         self.redd
-00001f70: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
-00001f80: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
-00001f90: 7265 6464 6f74 2e70 6e67 2229 0a20 2020  reddot.png").   
-00001fa0: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
-00001fb0: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
-00001fc0: 2e67 7265 656e 646f 7429 0a20 2020 2020  .greendot).     
-00001fd0: 2020 2073 656c 662e 7269 6768 7464 6f74     self.rightdot
-00001fe0: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
-00001ff0: 7265 6464 6f74 290a 0a20 2020 2020 2020  reddot)..       
-00002000: 2073 656c 662e 4631 2e73 6574 436f 6e74   self.F1.setCont
-00002010: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002020: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002030: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002040: 2020 2073 656c 662e 4631 2e63 7573 746f     self.F1.custo
-00002050: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002060: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002070: 6c66 2e65 6469 745f 4631 290a 2020 2020  lf.edit_F1).    
-00002080: 2020 2020 7365 6c66 2e46 312e 636c 6963      self.F1.clic
-00002090: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-000020a0: 2e73 656e 6466 3129 0a20 2020 2020 2020  .sendf1).       
-000020b0: 2073 656c 662e 4632 2e73 6574 436f 6e74   self.F2.setCont
-000020c0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000020d0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000020e0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000020f0: 2020 2073 656c 662e 4632 2e63 7573 746f     self.F2.custo
-00002100: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002110: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002120: 6c66 2e65 6469 745f 4632 290a 2020 2020  lf.edit_F2).    
-00002130: 2020 2020 7365 6c66 2e46 322e 636c 6963      self.F2.clic
-00002140: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002150: 2e73 656e 6466 3229 0a20 2020 2020 2020  .sendf2).       
-00002160: 2073 656c 662e 4633 2e73 6574 436f 6e74   self.F3.setCont
-00002170: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002180: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002190: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000021a0: 2020 2073 656c 662e 4633 2e63 7573 746f     self.F3.custo
-000021b0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-000021c0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-000021d0: 6c66 2e65 6469 745f 4633 290a 2020 2020  lf.edit_F3).    
-000021e0: 2020 2020 7365 6c66 2e46 332e 636c 6963      self.F3.clic
-000021f0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002200: 2e73 656e 6466 3329 0a20 2020 2020 2020  .sendf3).       
-00002210: 2073 656c 662e 4634 2e73 6574 436f 6e74   self.F4.setCont
-00002220: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002230: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002240: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002250: 2020 2073 656c 662e 4634 2e63 7573 746f     self.F4.custo
-00002260: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002270: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002280: 6c66 2e65 6469 745f 4634 290a 2020 2020  lf.edit_F4).    
-00002290: 2020 2020 7365 6c66 2e46 342e 636c 6963      self.F4.clic
-000022a0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-000022b0: 2e73 656e 6466 3429 0a20 2020 2020 2020  .sendf4).       
-000022c0: 2073 656c 662e 4635 2e73 6574 436f 6e74   self.F5.setCont
-000022d0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000022e0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000022f0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002300: 2020 2073 656c 662e 4635 2e63 7573 746f     self.F5.custo
-00002310: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002320: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002330: 6c66 2e65 6469 745f 4635 290a 2020 2020  lf.edit_F5).    
-00002340: 2020 2020 7365 6c66 2e46 352e 636c 6963      self.F5.clic
-00002350: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002360: 2e73 656e 6466 3529 0a20 2020 2020 2020  .sendf5).       
-00002370: 2073 656c 662e 4636 2e73 6574 436f 6e74   self.F6.setCont
-00002380: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002390: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000023a0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000023b0: 2020 2073 656c 662e 4636 2e63 7573 746f     self.F6.custo
-000023c0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-000023d0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-000023e0: 6c66 2e65 6469 745f 4636 290a 2020 2020  lf.edit_F6).    
-000023f0: 2020 2020 7365 6c66 2e46 362e 636c 6963      self.F6.clic
-00002400: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002410: 2e73 656e 6466 3629 0a20 2020 2020 2020  .sendf6).       
-00002420: 2073 656c 662e 4637 2e73 6574 436f 6e74   self.F7.setCont
-00002430: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-00002440: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002450: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002460: 2020 2073 656c 662e 4637 2e63 7573 746f     self.F7.custo
-00002470: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002480: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002490: 6c66 2e65 6469 745f 4637 290a 2020 2020  lf.edit_F7).    
-000024a0: 2020 2020 7365 6c66 2e46 372e 636c 6963      self.F7.clic
-000024b0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-000024c0: 2e73 656e 6466 3729 0a20 2020 2020 2020  .sendf7).       
-000024d0: 2073 656c 662e 4638 2e73 6574 436f 6e74   self.F8.setCont
-000024e0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000024f0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-00002500: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-00002510: 2020 2073 656c 662e 4638 2e63 7573 746f     self.F8.custo
-00002520: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-00002530: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-00002540: 6c66 2e65 6469 745f 4638 290a 2020 2020  lf.edit_F8).    
-00002550: 2020 2020 7365 6c66 2e46 382e 636c 6963      self.F8.clic
-00002560: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002570: 2e73 656e 6466 3829 0a20 2020 2020 2020  .sendf8).       
-00002580: 2073 656c 662e 4639 2e73 6574 436f 6e74   self.F9.setCont
-00002590: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
-000025a0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
-000025b0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
-000025c0: 2020 2073 656c 662e 4639 2e63 7573 746f     self.F9.custo
-000025d0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
-000025e0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
-000025f0: 6c66 2e65 6469 745f 4639 290a 2020 2020  lf.edit_F9).    
-00002600: 2020 2020 7365 6c66 2e46 392e 636c 6963      self.F9.clic
-00002610: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
-00002620: 2e73 656e 6466 3929 0a20 2020 2020 2020  .sendf9).       
-00002630: 2073 656c 662e 4631 302e 7365 7443 6f6e   self.F10.setCon
-00002640: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002650: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002660: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002670: 2020 2020 7365 6c66 2e46 3130 2e63 7573      self.F10.cus
-00002680: 746f 6d43 6f6e 7465 7874 4d65 6e75 5265  tomContextMenuRe
-00002690: 7175 6573 7465 642e 636f 6e6e 6563 7428  quested.connect(
-000026a0: 7365 6c66 2e65 6469 745f 4631 3029 0a20  self.edit_F10). 
-000026b0: 2020 2020 2020 2073 656c 662e 4631 302e         self.F10.
-000026c0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
-000026d0: 7365 6c66 2e73 656e 6466 3130 290a 2020  self.sendf10).  
-000026e0: 2020 2020 2020 7365 6c66 2e46 3131 2e73        self.F11.s
-000026f0: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002700: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002710: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002720: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
-00002730: 312e 6375 7374 6f6d 436f 6e74 6578 744d  1.customContextM
-00002740: 656e 7552 6571 7565 7374 6564 2e63 6f6e  enuRequested.con
-00002750: 6e65 6374 2873 656c 662e 6564 6974 5f46  nect(self.edit_F
-00002760: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
-00002770: 2e46 3131 2e63 6c69 636b 6564 2e63 6f6e  .F11.clicked.con
-00002780: 6e65 6374 2873 656c 662e 7365 6e64 6631  nect(self.sendf1
-00002790: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
-000027a0: 4631 322e 7365 7443 6f6e 7465 7874 4d65  F12.setContextMe
-000027b0: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
-000027c0: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
-000027d0: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
-000027e0: 6c66 2e46 3132 2e63 7573 746f 6d43 6f6e  lf.F12.customCon
-000027f0: 7465 7874 4d65 6e75 5265 7175 6573 7465  textMenuRequeste
-00002800: 642e 636f 6e6e 6563 7428 7365 6c66 2e65  d.connect(self.e
-00002810: 6469 745f 4631 3229 0a20 2020 2020 2020  dit_F12).       
-00002820: 2073 656c 662e 4631 322e 636c 6963 6b65   self.F12.clicke
-00002830: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
-00002840: 656e 6466 3132 290a 0a20 2020 2020 2020  endf12)..       
-00002850: 2073 656c 662e 7265 6164 7072 6566 6572   self.readprefer
-00002860: 656e 6365 7328 290a 2020 2020 2020 2020  ences().        
-00002870: 7365 6c66 2e64 626e 616d 6520 3d20 4441  self.dbname = DA
-00002880: 5441 5f50 4154 4820 2b20 222f 2220 2b20  TA_PATH + "/" + 
-00002890: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
-000028a0: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
-000028b0: 2c20 2268 616d 2e64 6222 290a 2020 2020  , "ham.db").    
-000028c0: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
-000028d0: 6520 3d20 4461 7461 4261 7365 2873 656c  e = DataBase(sel
-000028e0: 662e 6462 6e61 6d65 2c20 574f 524b 494e  f.dbname, WORKIN
-000028f0: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
-00002900: 7365 6c66 2e73 7461 7469 6f6e 203d 2073  self.station = s
-00002910: 656c 662e 6461 7461 6261 7365 2e66 6574  elf.database.fet
-00002920: 6368 5f73 7461 7469 6f6e 2829 0a20 2020  ch_station().   
-00002930: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00002940: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00002950: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00002960: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
-00002970: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-00002980: 745f 7374 6174 696f 6e5f 7365 7474 696e  t_station_settin
-00002990: 6773 2829 0a20 2020 2020 2020 2020 2020  gs().           
-000029a0: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
-000029b0: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
-000029c0: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
-000029d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000029e0: 662e 7374 6174 696f 6e20 6973 204e 6f6e  f.station is Non
-000029f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00002a00: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
-00002a10: 3d20 7b7d 0a20 2020 2020 2020 2073 656c  = {}.        sel
-00002a20: 662e 636f 6e74 6163 7420 3d20 7365 6c66  f.contact = self
-00002a30: 2e64 6174 6162 6173 652e 656d 7074 795f  .database.empty_
-00002a40: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
-00002a50: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
-00002a60: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
-00002a70: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
-00002a80: 2020 2020 2020 2073 656c 662e 6d61 6b65         self.make
-00002a90: 5f6f 705f 6469 7228 290a 2020 2020 2020  _op_dir().      
-00002aa0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-00002ab0: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
-00002ac0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002ad0: 6c6f 6164 5f63 6f6e 7465 7374 2829 0a0a  load_contest()..
-00002ae0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00002af0: 645f 6377 5f6d 6163 726f 7328 290a 2020  d_cw_macros().  
-00002b00: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00002b10: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-00002b20: 2023 2073 656c 662e 6c61 756e 6368 5f6c   # self.launch_l
-00002b30: 6f67 5f77 696e 646f 7728 290a 0a20 2020  og_window()..   
-00002b40: 2020 2020 2073 656c 662e 6261 6e64 5f69       self.band_i
-00002b50: 6e64 6963 6174 6f72 735f 6377 203d 207b  ndicators_cw = {
-00002b60: 0a20 2020 2020 2020 2020 2020 2022 3136  .            "16
-00002b70: 3022 3a20 7365 6c66 2e63 775f 6261 6e64  0": self.cw_band
-00002b80: 5f31 3630 2c0a 2020 2020 2020 2020 2020  _160,.          
-00002b90: 2020 2238 3022 3a20 7365 6c66 2e63 775f    "80": self.cw_
-00002ba0: 6261 6e64 5f38 302c 0a20 2020 2020 2020  band_80,.       
-00002bb0: 2020 2020 2022 3430 223a 2073 656c 662e       "40": self.
-00002bc0: 6377 5f62 616e 645f 3430 2c0a 2020 2020  cw_band_40,.    
-00002bd0: 2020 2020 2020 2020 2232 3022 3a20 7365          "20": se
-00002be0: 6c66 2e63 775f 6261 6e64 5f32 302c 0a20  lf.cw_band_20,. 
-00002bf0: 2020 2020 2020 2020 2020 2022 3135 223a             "15":
-00002c00: 2073 656c 662e 6377 5f62 616e 645f 3135   self.cw_band_15
-00002c10: 2c0a 2020 2020 2020 2020 2020 2020 2231  ,.            "1
-00002c20: 3022 3a20 7365 6c66 2e63 775f 6261 6e64  0": self.cw_band
-00002c30: 5f31 302c 0a20 2020 2020 2020 207d 0a0a  _10,.        }..
-00002c40: 2020 2020 2020 2020 7365 6c66 2e62 616e          self.ban
-00002c50: 645f 696e 6469 6361 746f 7273 5f73 7362  d_indicators_ssb
-00002c60: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00002c70: 2022 3136 3022 3a20 7365 6c66 2e73 7362   "160": self.ssb
-00002c80: 5f62 616e 645f 3136 302c 0a20 2020 2020  _band_160,.     
-00002c90: 2020 2020 2020 2022 3830 223a 2073 656c         "80": sel
-00002ca0: 662e 7373 625f 6261 6e64 5f38 302c 0a20  f.ssb_band_80,. 
-00002cb0: 2020 2020 2020 2020 2020 2022 3430 223a             "40":
-00002cc0: 2073 656c 662e 7373 625f 6261 6e64 5f34   self.ssb_band_4
-00002cd0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-00002ce0: 3230 223a 2073 656c 662e 7373 625f 6261  20": self.ssb_ba
-00002cf0: 6e64 5f32 302c 0a20 2020 2020 2020 2020  nd_20,.         
-00002d00: 2020 2022 3135 223a 2073 656c 662e 7373     "15": self.ss
-00002d10: 625f 6261 6e64 5f31 352c 0a20 2020 2020  b_band_15,.     
-00002d20: 2020 2020 2020 2022 3130 223a 2073 656c         "10": sel
-00002d30: 662e 7373 625f 6261 6e64 5f31 302c 0a20  f.ssb_band_10,. 
-00002d40: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-00002d50: 2020 7365 6c66 2e62 616e 645f 696e 6469    self.band_indi
-00002d60: 6361 746f 7273 5f72 7474 7920 3d20 7b0a  cators_rtty = {.
-00002d70: 2020 2020 2020 2020 2020 2020 2231 3630              "160
-00002d80: 223a 2073 656c 662e 7274 7479 5f62 616e  ": self.rtty_ban
-00002d90: 645f 3136 302c 0a20 2020 2020 2020 2020  d_160,.         
-00002da0: 2020 2022 3830 223a 2073 656c 662e 7274     "80": self.rt
-00002db0: 7479 5f62 616e 645f 3830 2c0a 2020 2020  ty_band_80,.    
-00002dc0: 2020 2020 2020 2020 2234 3022 3a20 7365          "40": se
-00002dd0: 6c66 2e72 7474 795f 6261 6e64 5f34 302c  lf.rtty_band_40,
-00002de0: 0a20 2020 2020 2020 2020 2020 2022 3230  .            "20
-00002df0: 223a 2073 656c 662e 7274 7479 5f62 616e  ": self.rtty_ban
-00002e00: 645f 3230 2c0a 2020 2020 2020 2020 2020  d_20,.          
-00002e10: 2020 2231 3522 3a20 7365 6c66 2e72 7474    "15": self.rtt
-00002e20: 795f 6261 6e64 5f31 352c 0a20 2020 2020  y_band_15,.     
-00002e30: 2020 2020 2020 2022 3130 223a 2073 656c         "10": sel
-00002e40: 662e 7274 7479 5f62 616e 645f 3130 2c0a  f.rtty_band_10,.
-00002e50: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-00002e60: 2020 2073 656c 662e 616c 6c5f 6d6f 6465     self.all_mode
-00002e70: 5f69 6e64 6963 6174 6f72 7320 3d20 7b0a  _indicators = {.
-00002e80: 2020 2020 2020 2020 2020 2020 2243 5722              "CW"
-00002e90: 3a20 7365 6c66 2e62 616e 645f 696e 6469  : self.band_indi
-00002ea0: 6361 746f 7273 5f63 772c 0a20 2020 2020  cators_cw,.     
-00002eb0: 2020 2020 2020 2022 5353 4222 3a20 7365         "SSB": se
-00002ec0: 6c66 2e62 616e 645f 696e 6469 6361 746f  lf.band_indicato
-00002ed0: 7273 5f73 7362 2c0a 2020 2020 2020 2020  rs_ssb,.        
-00002ee0: 2020 2020 2252 5454 5922 3a20 7365 6c66      "RTTY": self
-00002ef0: 2e62 616e 645f 696e 6469 6361 746f 7273  .band_indicators
-00002f00: 5f72 7474 792c 0a20 2020 2020 2020 207d  _rtty,.        }
-00002f10: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00002f20: 2e5f 7564 7077 6174 6368 2069 7320 4e6f  ._udpwatch is No
-00002f30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002f40: 7365 6c66 2e5f 7564 7077 6174 6368 203d  self._udpwatch =
-00002f50: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
-00002f60: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-00002f70: 2020 2074 6172 6765 743d 7365 6c66 2e77     target=self.w
-00002f80: 6174 6368 5f75 6470 2c0a 2020 2020 2020  atch_udp,.      
-00002f90: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
-00002fa0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00002fb0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00002fc0: 2073 656c 662e 5f75 6470 7761 7463 682e   self._udpwatch.
-00002fd0: 7374 6172 7428 290a 0a20 2020 2040 7374  start()..    @st
-00002fe0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-00002ff0: 6566 2063 6865 636b 5f70 726f 6365 7373  ef check_process
-00003000: 286e 616d 653a 2073 7472 2920 2d3e 2062  (name: str) -> b
-00003010: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00003020: 6368 6563 6b73 2074 6f20 7365 6520 6966  checks to see if
-00003030: 2070 726f 6772 616d 206f 6620 6e61 6d65   program of name
-00003040: 2069 7320 696e 2074 6865 2061 6374 6976   is in the activ
-00003050: 6520 7072 6f63 6573 7320 6c69 7374 2222  e process list""
-00003060: 220a 2020 2020 2020 2020 666f 7220 7072  ".        for pr
-00003070: 6f63 2069 6e20 7073 7574 696c 2e70 726f  oc in psutil.pro
-00003080: 6365 7373 5f69 7465 7228 293a 0a20 2020  cess_iter():.   
-00003090: 2020 2020 2020 2020 2069 6620 626f 6f6c           if bool
-000030a0: 2872 652e 6d61 7463 6828 6e61 6d65 2c20  (re.match(name, 
-000030b0: 7072 6f63 2e6e 616d 6528 292e 6c6f 7765  proc.name().lowe
-000030c0: 7228 2929 293a 0a20 2020 2020 2020 2020  r())):.         
-000030d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000030e0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-000030f0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00003100: 2073 686f 775f 6d65 7373 6167 655f 626f   show_message_bo
-00003110: 7828 7365 6c66 2c20 6d65 7373 6167 653a  x(self, message:
-00003120: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
-00003130: 2020 2020 2020 2022 2222 646f 6322 2222         """doc"""
-00003140: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
-00003150: 5f62 6f78 203d 2051 7457 6964 6765 7473  _box = QtWidgets
-00003160: 2e51 4d65 7373 6167 6542 6f78 2829 0a20  .QMessageBox(). 
-00003170: 2020 2020 2020 206d 6573 7361 6765 5f62         message_b
-00003180: 6f78 2e73 6574 4963 6f6e 2851 7457 6964  ox.setIcon(QtWid
-00003190: 6765 7473 2e51 4d65 7373 6167 6542 6f78  gets.QMessageBox
-000031a0: 2e49 6e66 6f72 6d61 7469 6f6e 290a 2020  .Information).  
-000031b0: 2020 2020 2020 6d65 7373 6167 655f 626f        message_bo
-000031c0: 782e 7365 7454 6578 7428 6d65 7373 6167  x.setText(messag
-000031d0: 6529 0a20 2020 2020 2020 206d 6573 7361  e).        messa
-000031e0: 6765 5f62 6f78 2e73 6574 5769 6e64 6f77  ge_box.setWindow
-000031f0: 5469 746c 6528 2249 6e66 6f72 6d61 7469  Title("Informati
-00003200: 6f6e 2229 0a20 2020 2020 2020 206d 6573  on").        mes
-00003210: 7361 6765 5f62 6f78 2e73 6574 5374 616e  sage_box.setStan
-00003220: 6461 7264 4275 7474 6f6e 7328 5174 5769  dardButtons(QtWi
-00003230: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
-00003240: 782e 4f6b 290a 2020 2020 2020 2020 5f20  x.Ok).        _ 
-00003250: 3d20 6d65 7373 6167 655f 626f 782e 6578  = message_box.ex
-00003260: 6563 5f28 290a 0a20 2020 2064 6566 2073  ec_()..    def s
-00003270: 686f 775f 6162 6f75 745f 6469 616c 6f67  how_about_dialog
-00003280: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003290: 2222 2253 686f 7720 6162 6f75 7420 6469  """Show about di
-000032a0: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
-000032b0: 7365 6c66 2e61 626f 7574 5f64 6961 6c6f  self.about_dialo
-000032c0: 6720 3d20 4162 6f75 7428 574f 524b 494e  g = About(WORKIN
-000032d0: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
-000032e0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-000032f0: 2822 6461 726b 5f6d 6f64 6522 293a 0a20  ("dark_mode"):. 
-00003300: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003310: 6162 6f75 745f 6469 616c 6f67 2e73 6574  about_dialog.set
-00003320: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
-00003330: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
-00003340: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
-00003350: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-00003360: 2020 6465 6620 6564 6974 5f63 6f6e 6669    def edit_confi
-00003370: 6775 7261 7469 6f6e 5f73 6574 7469 6e67  guration_setting
-00003380: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00003390: 2022 2222 436f 6e66 6967 7572 6174 696f   """Configuratio
-000033a0: 6e20 5365 7474 696e 6773 2077 6173 2063  n Settings was c
-000033b0: 6c69 636b 6564 2222 220a 2020 2020 2020  licked""".      
-000033c0: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
-000033d0: 7469 6f6e 5f64 6961 6c6f 6720 3d20 5365  tion_dialog = Se
-000033e0: 7474 696e 6773 2857 4f52 4b49 4e47 5f50  ttings(WORKING_P
-000033f0: 4154 482c 2043 4f4e 4649 475f 5041 5448  ATH, CONFIG_PATH
-00003400: 2c20 7365 6c66 2e70 7265 6629 0a20 2020  , self.pref).   
-00003410: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-00003420: 7572 6174 696f 6e5f 6469 616c 6f67 2e75  uration_dialog.u
-00003430: 7365 6861 6d64 625f 7261 6469 6f42 7574  sehamdb_radioBut
-00003440: 746f 6e2e 6869 6465 2829 0a20 2020 2020  ton.hide().     
-00003450: 2020 2023 2073 656c 662e 636f 6e66 6967     # self.config
-00003460: 7572 6174 696f 6e5f 6469 616c 6f67 2e6e  uration_dialog.n
-00003470: 316d 6d5f 7461 622e 6869 6465 2829 0a20  1mm_tab.hide(). 
-00003480: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
-00003490: 6967 7572 6174 696f 6e5f 6469 616c 6f67  iguration_dialog
-000034a0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-000034b0: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
-000034c0: 6f6e 5f64 6961 6c6f 672e 6163 6365 7074  on_dialog.accept
-000034d0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-000034e0: 6564 6974 5f63 6f6e 6669 6775 7261 7469  edit_configurati
-000034f0: 6f6e 5f72 6574 7572 6e29 0a0a 2020 2020  on_return)..    
-00003500: 6465 6620 6564 6974 5f63 6f6e 6669 6775  def edit_configu
-00003510: 7261 7469 6f6e 5f72 6574 7572 6e28 7365  ration_return(se
-00003520: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003530: 5265 7475 726e 7320 6865 7265 2077 6865  Returns here whe
-00003540: 6e20 636f 6e66 6967 7572 6174 696f 6e20  n configuration 
-00003550: 6469 616c 6f67 2063 6c6f 7365 6420 7769  dialog closed wi
-00003560: 7468 206f 6b61 792e 2222 220a 2020 2020  th okay.""".    
-00003570: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
-00003580: 7261 7469 6f6e 5f64 6961 6c6f 672e 7361  ration_dialog.sa
-00003590: 7665 5f63 6861 6e67 6573 2829 0a20 2020  ve_changes().   
-000035a0: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
-000035b0: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
-000035c0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000035d0: 6728 2225 7322 2c20 6622 7b73 656c 662e  g("%s", f"{self.
-000035e0: 7072 6566 7d22 290a 2020 2020 2020 2020  pref}").        
-000035f0: 7365 6c66 2e72 6561 6470 7265 6665 7265  self.readprefere
-00003600: 6e63 6573 2829 0a0a 2020 2020 6465 6620  nces()..    def 
-00003610: 6e65 775f 6461 7461 6261 7365 2873 656c  new_database(sel
-00003620: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00003630: 7265 6174 6520 6e65 7720 6461 7461 6261  reate new databa
-00003640: 7365 2e22 2222 0a20 2020 2020 2020 2066  se.""".        f
-00003650: 696c 656e 616d 6520 3d20 7365 6c66 2e66  ilename = self.f
-00003660: 696c 6570 6963 6b65 7228 226e 6577 2229  ilepicker("new")
-00003670: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
-00003680: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-00003690: 2020 6966 2066 696c 656e 616d 655b 2d33    if filename[-3
-000036a0: 3a5d 2021 3d20 222e 6462 223a 0a20 2020  :] != ".db":.   
-000036b0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000036c0: 656e 616d 6520 2b3d 2022 2e64 6222 0a20  ename += ".db". 
-000036d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000036e0: 7072 6566 5b22 6375 7272 656e 745f 6461  pref["current_da
-000036f0: 7461 6261 7365 225d 203d 2066 696c 656e  tabase"] = filen
-00003700: 616d 652e 7370 6c69 7428 222f 2229 5b2d  ame.split("/")[-
-00003710: 313a 5d5b 305d 0a20 2020 2020 2020 2020  1:][0].         
-00003720: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
-00003730: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
-00003740: 2020 2020 2020 2073 656c 662e 6462 6e61         self.dbna
-00003750: 6d65 203d 2044 4154 415f 5041 5448 202b  me = DATA_PATH +
-00003760: 2022 2f22 202b 2073 656c 662e 7072 6566   "/" + self.pref
-00003770: 2e67 6574 2822 6375 7272 656e 745f 6461  .get("current_da
-00003780: 7461 6261 7365 222c 2022 6861 6d2e 6462  tabase", "ham.db
-00003790: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-000037a0: 656c 662e 6461 7461 6261 7365 203d 2044  elf.database = D
-000037b0: 6174 6142 6173 6528 7365 6c66 2e64 626e  ataBase(self.dbn
-000037c0: 616d 652c 2057 4f52 4b49 4e47 5f50 4154  ame, WORKING_PAT
-000037d0: 4829 0a20 2020 2020 2020 2020 2020 2073  H).            s
-000037e0: 656c 662e 636f 6e74 6163 7420 3d20 7365  elf.contact = se
-000037f0: 6c66 2e64 6174 6162 6173 652e 656d 7074  lf.database.empt
-00003800: 795f 636f 6e74 6163 740a 2020 2020 2020  y_contact.      
-00003810: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00003820: 6f6e 203d 2073 656c 662e 6461 7461 6261  on = self.databa
-00003830: 7365 2e66 6574 6368 5f73 7461 7469 6f6e  se.fetch_station
-00003840: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-00003850: 6620 7365 6c66 2e73 7461 7469 6f6e 2069  f self.station i
-00003860: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00003870: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00003880: 7469 6f6e 203d 207b 7d0a 2020 2020 2020  tion = {}.      
-00003890: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
-000038a0: 6e74 5f6f 7020 3d20 7365 6c66 2e73 7461  nt_op = self.sta
-000038b0: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
-000038c0: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
-000038d0: 2073 656c 662e 6d61 6b65 5f6f 705f 6469   self.make_op_di
-000038e0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
-000038f0: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
-00003900: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
-00003910: 3d20 224e 4557 4442 220a 2020 2020 2020  = "NEWDB".      
-00003920: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00003930: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-00003940: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-00003950: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003960: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
-00003970: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003980: 2e65 6469 745f 7374 6174 696f 6e5f 7365  .edit_station_se
-00003990: 7474 696e 6773 2829 0a0a 2020 2020 6465  ttings()..    de
-000039a0: 6620 6f70 656e 5f64 6174 6162 6173 6528  f open_database(
-000039b0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000039c0: 2222 4f70 656e 2065 7869 7374 696e 6720  ""Open existing 
-000039d0: 6461 7461 6261 7365 2e22 2222 0a20 2020  database.""".   
-000039e0: 2020 2020 2066 696c 656e 616d 6520 3d20       filename = 
-000039f0: 7365 6c66 2e66 696c 6570 6963 6b65 7228  self.filepicker(
-00003a00: 226f 7065 6e22 290a 2020 2020 2020 2020  "open").        
-00003a10: 6966 2066 696c 656e 616d 653a 0a20 2020  if filename:.   
-00003a20: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-00003a30: 6566 5b22 6375 7272 656e 745f 6461 7461  ef["current_data
-00003a40: 6261 7365 225d 203d 2066 696c 656e 616d  base"] = filenam
-00003a50: 652e 7370 6c69 7428 222f 2229 5b2d 313a  e.split("/")[-1:
-00003a60: 5d5b 305d 0a20 2020 2020 2020 2020 2020  ][0].           
-00003a70: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
-00003a80: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
-00003a90: 2020 2020 2073 656c 662e 6462 6e61 6d65       self.dbname
-00003aa0: 203d 2044 4154 415f 5041 5448 202b 2022   = DATA_PATH + "
-00003ab0: 2f22 202b 2073 656c 662e 7072 6566 2e67  /" + self.pref.g
-00003ac0: 6574 2822 6375 7272 656e 745f 6461 7461  et("current_data
-00003ad0: 6261 7365 222c 2022 6861 6d2e 6462 2229  base", "ham.db")
-00003ae0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003af0: 662e 6461 7461 6261 7365 203d 2044 6174  f.database = Dat
-00003b00: 6142 6173 6528 7365 6c66 2e64 626e 616d  aBase(self.dbnam
-00003b10: 652c 2057 4f52 4b49 4e47 5f50 4154 4829  e, WORKING_PATH)
-00003b20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003b30: 662e 636f 6e74 6163 7420 3d20 7365 6c66  f.contact = self
-00003b40: 2e64 6174 6162 6173 652e 656d 7074 795f  .database.empty_
-00003b50: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
-00003b60: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-00003b70: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
-00003b80: 2e66 6574 6368 5f73 7461 7469 6f6e 2829  .fetch_station()
-00003b90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003ba0: 7365 6c66 2e73 7461 7469 6f6e 2069 7320  self.station is 
-00003bb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003bc0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00003bd0: 6f6e 203d 207b 7d0a 2020 2020 2020 2020  on = {}.        
-00003be0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-00003bf0: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
-00003c00: 2222 2920 3d3d 2022 223a 0a20 2020 2020  "") == "":.     
-00003c10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003c20: 6564 6974 5f73 7461 7469 6f6e 5f73 6574  edit_station_set
-00003c30: 7469 6e67 7328 290a 2020 2020 2020 2020  tings().        
-00003c40: 2020 2020 7365 6c66 2e63 7572 7265 6e74      self.current
-00003c50: 5f6f 7020 3d20 7365 6c66 2e73 7461 7469  _op = self.stati
-00003c60: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
-00003c70: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00003c80: 656c 662e 6d61 6b65 5f6f 705f 6469 7228  elf.make_op_dir(
-00003c90: 290a 2020 2020 2020 2020 2020 2020 636d  ).            cm
-00003ca0: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
-00003cb0: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-00003cc0: 224e 4557 4442 220a 2020 2020 2020 2020  "NEWDB".        
-00003cd0: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
-00003ce0: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
-00003cf0: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
-00003d00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003d10: 636c 6561 7269 6e70 7574 7328 290a 0a20  clearinputs().. 
-00003d20: 2020 2064 6566 206e 6577 5f63 6f6e 7465     def new_conte
-00003d30: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
-00003d40: 2020 2222 2243 7265 6174 6520 6e65 7720    """Create new 
-00003d50: 636f 6e74 6573 7420 696e 2065 7869 7374  contest in exist
-00003d60: 696e 6720 6461 7461 6261 7365 2e22 2222  ing database."""
-00003d70: 0a0a 2020 2020 6465 6620 6f70 656e 5f63  ..    def open_c
-00003d80: 6f6e 7465 7374 2873 656c 6629 3a0a 2020  ontest(self):.  
-00003d90: 2020 2020 2020 2222 2253 7769 7463 6820        """Switch 
-00003da0: 746f 2061 2064 6966 6665 7265 6e74 2065  to a different e
-00003db0: 7869 7374 696e 6720 636f 6e74 6573 7420  xisting contest 
-00003dc0: 696e 2065 7869 7374 696e 6720 6461 7461  in existing data
-00003dd0: 6261 7365 2e22 2222 0a20 2020 2020 2020  base.""".       
-00003de0: 206c 6f67 6765 722e 6465 6275 6728 224f   logger.debug("O
-00003df0: 7065 6e20 436f 6e74 6573 7420 7365 6c65  pen Contest sele
-00003e00: 6374 6564 2229 0a20 2020 2020 2020 2063  cted").        c
-00003e10: 6f6e 7465 7374 7320 3d20 7365 6c66 2e64  ontests = self.d
-00003e20: 6174 6162 6173 652e 6665 7463 685f 616c  atabase.fetch_al
-00003e30: 6c5f 636f 6e74 6573 7473 2829 0a20 2020  l_contests().   
-00003e40: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00003e50: 6728 2225 7322 2c20 6622 7b63 6f6e 7465  g("%s", f"{conte
-00003e60: 7374 737d 2229 0a0a 2020 2020 2020 2020  sts}")..        
-00003e70: 6966 2063 6f6e 7465 7374 733a 0a20 2020  if contests:.   
-00003e80: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00003e90: 6e74 6573 745f 6469 616c 6f67 203d 2053  ntest_dialog = S
-00003ea0: 656c 6563 7443 6f6e 7465 7374 2857 4f52  electContest(WOR
-00003eb0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
-00003ec0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00003ed0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-00003ee0: 7374 5f6c 6973 742e 7365 7452 6f77 436f  st_list.setRowCo
-00003ef0: 756e 7428 3029 0a20 2020 2020 2020 2020  unt(0).         
-00003f00: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-00003f10: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
-00003f20: 6973 742e 7365 7443 6f6c 756d 6e43 6f75  ist.setColumnCou
-00003f30: 6e74 2834 290a 2020 2020 2020 2020 2020  nt(4).          
-00003f40: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00003f50: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00003f60: 7374 2e76 6572 7469 6361 6c48 6561 6465  st.verticalHeade
-00003f70: 7228 292e 7365 7456 6973 6962 6c65 2846  r().setVisible(F
-00003f80: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00003f90: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00003fa0: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00003fb0: 7374 2e73 6574 436f 6c75 6d6e 5769 6474  st.setColumnWidt
-00003fc0: 6828 312c 2032 3030 290a 2020 2020 2020  h(1, 200).      
-00003fd0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00003fe0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
-00003ff0: 745f 6c69 7374 2e73 6574 436f 6c75 6d6e  t_list.setColumn
-00004000: 5769 6474 6828 322c 2032 3030 290a 2020  Width(2, 200).  
-00004010: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00004020: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-00004030: 6e74 6573 745f 6c69 7374 2e73 6574 486f  ntest_list.setHo
-00004040: 7269 7a6f 6e74 616c 4865 6164 6572 4974  rizontalHeaderIt
-00004050: 656d 280a 2020 2020 2020 2020 2020 2020  em(.            
-00004060: 2020 2020 302c 2051 7457 6964 6765 7473      0, QtWidgets
-00004070: 2e51 5461 626c 6557 6964 6765 7449 7465  .QTableWidgetIte
-00004080: 6d28 2243 6f6e 7465 7374 204e 7222 290a  m("Contest Nr").
-00004090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000040a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000040b0: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-000040c0: 6e74 6573 745f 6c69 7374 2e73 6574 486f  ntest_list.setHo
-000040d0: 7269 7a6f 6e74 616c 4865 6164 6572 4974  rizontalHeaderIt
-000040e0: 656d 280a 2020 2020 2020 2020 2020 2020  em(.            
-000040f0: 2020 2020 312c 2051 7457 6964 6765 7473      1, QtWidgets
-00004100: 2e51 5461 626c 6557 6964 6765 7449 7465  .QTableWidgetIte
-00004110: 6d28 2243 6f6e 7465 7374 204e 616d 6522  m("Contest Name"
-00004120: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00004130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004140: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004150: 636f 6e74 6573 745f 6c69 7374 2e73 6574  contest_list.set
-00004160: 486f 7269 7a6f 6e74 616c 4865 6164 6572  HorizontalHeader
-00004170: 4974 656d 280a 2020 2020 2020 2020 2020  Item(.          
-00004180: 2020 2020 2020 322c 2051 7457 6964 6765        2, QtWidge
-00004190: 7473 2e51 5461 626c 6557 6964 6765 7449  ts.QTableWidgetI
-000041a0: 7465 6d28 2243 6f6e 7465 7374 2053 7461  tem("Contest Sta
-000041b0: 7274 2229 0a20 2020 2020 2020 2020 2020  rt").           
-000041c0: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-000041d0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000041e0: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-000041f0: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
-00004200: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
-00004210: 2020 2020 2020 2020 2033 2c20 5174 5769           3, QtWi
-00004220: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
-00004230: 6574 4974 656d 2822 4e6f 7420 5549 7365  etItem("Not UIse
-00004240: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
-00004250: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00004260: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004270: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
-00004280: 6574 436f 6c75 6d6e 4869 6464 656e 2830  etColumnHidden(0
-00004290: 2c20 5472 7565 290a 2020 2020 2020 2020  , True).        
-000042a0: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-000042b0: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-000042c0: 6c69 7374 2e73 6574 436f 6c75 6d6e 4869  list.setColumnHi
-000042d0: 6464 656e 2833 2c20 5472 7565 290a 2020  dden(3, True).  
-000042e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000042f0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6163  ontest_dialog.ac
-00004300: 6365 7074 6564 2e63 6f6e 6e65 6374 2873  cepted.connect(s
-00004310: 656c 662e 6f70 656e 5f63 6f6e 7465 7374  elf.open_contest
-00004320: 5f72 6574 7572 6e29 0a20 2020 2020 2020  _return).       
-00004330: 2020 2020 2066 6f72 2063 6f6e 7465 7374       for contest
-00004340: 2069 6e20 636f 6e74 6573 7473 3a0a 2020   in contests:.  
-00004350: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00004360: 6d62 6572 5f6f 665f 726f 7773 203d 2073  mber_of_rows = s
-00004370: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004380: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004390: 726f 7743 6f75 6e74 2829 0a20 2020 2020  rowCount().     
-000043a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000043b0: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-000043c0: 6f6e 7465 7374 5f6c 6973 742e 696e 7365  ontest_list.inse
-000043d0: 7274 526f 7728 6e75 6d62 6572 5f6f 665f  rtRow(number_of_
-000043e0: 726f 7773 290a 2020 2020 2020 2020 2020  rows).          
-000043f0: 2020 2020 2020 636f 6e74 6573 745f 6964        contest_id
-00004400: 203d 2073 7472 2863 6f6e 7465 7374 2e67   = str(contest.g
-00004410: 6574 2822 436f 6e74 6573 7449 4422 2c20  et("ContestID", 
-00004420: 3129 290a 2020 2020 2020 2020 2020 2020  1)).            
-00004430: 2020 2020 636f 6e74 6573 745f 6e61 6d65      contest_name
-00004440: 203d 2063 6f6e 7465 7374 2e67 6574 2822   = contest.get("
-00004450: 436f 6e74 6573 744e 616d 6522 2c20 3129  ContestName", 1)
-00004460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004470: 2073 7461 7274 5f64 6174 6520 3d20 636f   start_date = co
-00004480: 6e74 6573 742e 6765 7428 2253 7461 7274  ntest.get("Start
-00004490: 4461 7465 222c 2031 290a 2020 2020 2020  Date", 1).      
-000044a0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000044b0: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
-000044c0: 6e74 6573 745f 6c69 7374 2e73 6574 4974  ntest_list.setIt
-000044d0: 656d 280a 2020 2020 2020 2020 2020 2020  em(.            
-000044e0: 2020 2020 2020 2020 6e75 6d62 6572 5f6f          number_o
-000044f0: 665f 726f 7773 2c20 302c 2051 7457 6964  f_rows, 0, QtWid
-00004500: 6765 7473 2e51 5461 626c 6557 6964 6765  gets.QTableWidge
-00004510: 7449 7465 6d28 636f 6e74 6573 745f 6964  tItem(contest_id
-00004520: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004530: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00004540: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00004550: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-00004560: 6c69 7374 2e73 6574 4974 656d 280a 2020  list.setItem(.  
-00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004580: 2020 6e75 6d62 6572 5f6f 665f 726f 7773    number_of_rows
-00004590: 2c20 312c 2051 7457 6964 6765 7473 2e51  , 1, QtWidgets.Q
-000045a0: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
-000045b0: 636f 6e74 6573 745f 6e61 6d65 290a 2020  contest_name).  
-000045c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045e0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000045f0: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
-00004600: 2e73 6574 4974 656d 280a 2020 2020 2020  .setItem(.      
-00004610: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00004620: 6d62 6572 5f6f 665f 726f 7773 2c20 322c  mber_of_rows, 2,
-00004630: 2051 7457 6964 6765 7473 2e51 5461 626c   QtWidgets.QTabl
-00004640: 6557 6964 6765 7449 7465 6d28 7374 6172  eWidgetItem(star
-00004650: 745f 6461 7465 290a 2020 2020 2020 2020  t_date).        
-00004660: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00004670: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-00004680: 6961 6c6f 672e 7368 6f77 2829 0a0a 2020  ialog.show()..  
-00004690: 2020 6465 6620 6f70 656e 5f63 6f6e 7465    def open_conte
-000046a0: 7374 5f72 6574 7572 6e28 7365 6c66 293a  st_return(self):
-000046b0: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
-000046c0: 6564 2062 7920 6f70 656e 5f63 6f6e 7465  ed by open_conte
-000046d0: 7374 2222 220a 2020 2020 2020 2020 7365  st""".        se
-000046e0: 6c65 6374 6564 5f72 6f77 203d 2073 656c  lected_row = sel
-000046f0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00004700: 2e63 6f6e 7465 7374 5f6c 6973 742e 6375  .contest_list.cu
-00004710: 7272 656e 7452 6f77 2829 0a20 2020 2020  rrentRow().     
-00004720: 2020 2063 6f6e 7465 7374 203d 2073 656c     contest = sel
-00004730: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00004740: 2e63 6f6e 7465 7374 5f6c 6973 742e 6974  .contest_list.it
-00004750: 656d 2873 656c 6563 7465 645f 726f 772c  em(selected_row,
-00004760: 2030 292e 7465 7874 2829 0a20 2020 2020   0).text().     
-00004770: 2020 2073 656c 662e 7072 6566 5b22 636f     self.pref["co
-00004780: 6e74 6573 7422 5d20 3d20 636f 6e74 6573  ntest"] = contes
-00004790: 740a 2020 2020 2020 2020 7365 6c66 2e77  t.        self.w
-000047a0: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
-000047b0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-000047c0: 2e64 6562 7567 2822 5365 6c65 6374 6564  .debug("Selected
-000047d0: 2063 6f6e 7465 7374 3a20 2573 222c 2066   contest: %s", f
-000047e0: 227b 636f 6e74 6573 747d 2229 0a20 2020  "{contest}").   
-000047f0: 2020 2020 2073 656c 662e 6c6f 6164 5f63       self.load_c
-00004800: 6f6e 7465 7374 2829 0a0a 2020 2020 6465  ontest()..    de
-00004810: 6620 7265 6669 6c6c 5f64 726f 7064 6f77  f refill_dropdow
-00004820: 6e28 7365 6c66 2c20 7461 7267 6574 2c20  n(self, target, 
-00004830: 736f 7572 6365 293a 0a20 2020 2020 2020  source):.       
-00004840: 2022 2222 5265 6669 6c6c 2051 436f 6d62   """Refill QComb
-00004850: 6f62 6f78 2077 6964 6765 7420 7769 7468  obox widget with
-00004860: 2076 616c 7565 2e22 2222 0a20 2020 2020   value.""".     
-00004870: 2020 2069 6e64 6578 203d 2074 6172 6765     index = targe
-00004880: 742e 6669 6e64 5465 7874 2873 6f75 7263  t.findText(sourc
-00004890: 6529 0a20 2020 2020 2020 2074 6172 6765  e).        targe
-000048a0: 742e 7365 7443 7572 7265 6e74 496e 6465  t.setCurrentInde
-000048b0: 7828 696e 6465 7829 0a0a 2020 2020 6465  x(index)..    de
-000048c0: 6620 6564 6974 5f63 6f6e 7465 7374 2873  f edit_contest(s
-000048d0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000048e0: 2245 6469 7420 7468 6520 6375 7272 656e  "Edit the curren
-000048f0: 7420 636f 6e74 6573 7422 2222 0a20 2020  t contest""".   
-00004900: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00004910: 6728 2245 6469 7420 636f 6e74 6573 7420  g("Edit contest 
-00004920: 4469 616c 6f67 2229 0a20 2020 2020 2020  Dialog").       
-00004930: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-00004940: 5f73 6574 7469 6e67 7320 6973 204e 6f6e  _settings is Non
-00004950: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00004960: 6574 7572 6e0a 2020 2020 2020 2020 7365  eturn.        se
-00004970: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004980: 6720 3d20 4e65 7743 6f6e 7465 7374 2857  g = NewContest(W
-00004990: 4f52 4b49 4e47 5f50 4154 4829 0a20 2020  ORKING_PATH).   
-000049a0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-000049b0: 745f 6469 616c 6f67 2e73 6574 5769 6e64  t_dialog.setWind
-000049c0: 6f77 5469 746c 6528 2245 6469 7420 436f  owTitle("Edit Co
-000049d0: 6e74 6573 7422 290a 2020 2020 2020 2020  ntest").        
-000049e0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000049f0: 6c6f 672e 7469 746c 652e 7365 7454 6578  log.title.setTex
-00004a00: 7428 2222 290a 2020 2020 2020 2020 7365  t("").        se
-00004a10: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004a20: 672e 6163 6365 7074 6564 2e63 6f6e 6e65  g.accepted.conne
-00004a30: 6374 2873 656c 662e 7361 7665 5f65 6469  ct(self.save_edi
-00004a40: 7465 645f 636f 6e74 6573 7429 0a20 2020  ted_contest).   
-00004a50: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-00004a60: 662e 6765 7428 2264 6172 6b5f 6d6f 6465  f.get("dark_mode
-00004a70: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00004a80: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004a90: 6c6f 672e 7365 7453 7479 6c65 5368 6565  log.setStyleShee
-00004aa0: 7428 4441 524b 5f53 5459 4c45 5348 4545  t(DARK_STYLESHEE
-00004ab0: 5429 0a0a 2020 2020 2020 2020 7661 6c75  T)..        valu
-00004ac0: 6520 3d20 7365 6c66 2e63 6f6e 7465 7374  e = self.contest
-00004ad0: 5f73 6574 7469 6e67 732e 6765 7428 2243  _settings.get("C
-00004ae0: 6f6e 7465 7374 4e61 6d65 2229 2e75 7070  ontestName").upp
-00004af0: 6572 2829 2e72 6570 6c61 6365 2822 5f22  er().replace("_"
-00004b00: 2c20 2220 2229 0a20 2020 2020 2020 2069  , " ").        i
-00004b10: 6620 7661 6c75 6520 3d3d 2022 4745 4e45  f value == "GENE
-00004b20: 5241 4c20 4c4f 4747 494e 4722 3a0a 2020  RAL LOGGING":.  
-00004b30: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-00004b40: 3d20 2247 656e 6572 616c 204c 6f67 6769  = "General Loggi
-00004b50: 6e67 220a 2020 2020 2020 2020 7365 6c66  ng".        self
-00004b60: 2e72 6566 696c 6c5f 6472 6f70 646f 776e  .refill_dropdown
-00004b70: 2873 656c 662e 636f 6e74 6573 745f 6469  (self.contest_di
-00004b80: 616c 6f67 2e63 6f6e 7465 7374 2c20 7661  alog.contest, va
-00004b90: 6c75 6529 0a20 2020 2020 2020 2076 616c  lue).        val
-00004ba0: 7565 203d 2073 656c 662e 636f 6e74 6573  ue = self.contes
-00004bb0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00004bc0: 4f70 6572 6174 6f72 4361 7465 676f 7279  OperatorCategory
-00004bd0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00004be0: 7265 6669 6c6c 5f64 726f 7064 6f77 6e28  refill_dropdown(
-00004bf0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004c00: 6c6f 672e 6f70 6572 6174 6f72 5f63 6c61  log.operator_cla
-00004c10: 7373 2c20 7661 6c75 6529 0a20 2020 2020  ss, value).     
-00004c20: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
-00004c30: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-00004c40: 2e67 6574 2822 4261 6e64 4361 7465 676f  .get("BandCatego
-00004c50: 7279 2229 0a20 2020 2020 2020 2073 656c  ry").        sel
-00004c60: 662e 7265 6669 6c6c 5f64 726f 7064 6f77  f.refill_dropdow
-00004c70: 6e28 7365 6c66 2e63 6f6e 7465 7374 5f64  n(self.contest_d
-00004c80: 6961 6c6f 672e 6261 6e64 2c20 7661 6c75  ialog.band, valu
-00004c90: 6529 0a20 2020 2020 2020 2076 616c 7565  e).        value
-00004ca0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00004cb0: 7365 7474 696e 6773 2e67 6574 2822 506f  settings.get("Po
-00004cc0: 7765 7243 6174 6567 6f72 7922 290a 2020  werCategory").  
-00004cd0: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
-00004ce0: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
-00004cf0: 636f 6e74 6573 745f 6469 616c 6f67 2e70  contest_dialog.p
-00004d00: 6f77 6572 2c20 7661 6c75 6529 0a20 2020  ower, value).   
-00004d10: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
-00004d20: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00004d30: 6773 2e67 6574 2822 4d6f 6465 4361 7465  gs.get("ModeCate
-00004d40: 676f 7279 2229 0a20 2020 2020 2020 2073  gory").        s
-00004d50: 656c 662e 7265 6669 6c6c 5f64 726f 7064  elf.refill_dropd
-00004d60: 6f77 6e28 7365 6c66 2e63 6f6e 7465 7374  own(self.contest
-00004d70: 5f64 6961 6c6f 672e 6d6f 6465 2c20 7661  _dialog.mode, va
-00004d80: 6c75 6529 0a20 2020 2020 2020 2076 616c  lue).        val
-00004d90: 7565 203d 2073 656c 662e 636f 6e74 6573  ue = self.contes
-00004da0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00004db0: 4f76 6572 6c61 7943 6174 6567 6f72 7922  OverlayCategory"
-00004dc0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
-00004dd0: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
-00004de0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004df0: 6f67 2e6f 7665 726c 6179 2c20 7661 6c75  og.overlay, valu
-00004e00: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-00004e10: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
-00004e20: 7065 7261 746f 7273 2e73 6574 5465 7874  perators.setText
-00004e30: 2873 656c 662e 636f 6e74 6573 745f 7365  (self.contest_se
-00004e40: 7474 696e 6773 2e67 6574 2822 4f70 6572  ttings.get("Oper
-00004e50: 6174 6f72 7322 2929 0a20 2020 2020 2020  ators")).       
-00004e60: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00004e70: 616c 6f67 2e73 6f61 7062 6f78 2e73 6574  alog.soapbox.set
-00004e80: 506c 6169 6e54 6578 7428 7365 6c66 2e63  PlainText(self.c
-00004e90: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
-00004ea0: 6765 7428 2253 6f61 7062 6f78 2229 290a  get("Soapbox")).
-00004eb0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00004ec0: 7465 7374 5f64 6961 6c6f 672e 6578 6368  test_dialog.exch
-00004ed0: 616e 6765 2e73 6574 5465 7874 2873 656c  ange.setText(sel
-00004ee0: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00004ef0: 6773 2e67 6574 2822 5365 6e74 4578 6368  gs.get("SentExch
-00004f00: 616e 6765 2229 290a 2020 2020 2020 2020  ange")).        
-00004f10: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
-00004f20: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-00004f30: 7428 2253 7461 7469 6f6e 4361 7465 676f  t("StationCatego
-00004f40: 7279 2229 0a20 2020 2020 2020 2073 656c  ry").        sel
-00004f50: 662e 7265 6669 6c6c 5f64 726f 7064 6f77  f.refill_dropdow
-00004f60: 6e28 7365 6c66 2e63 6f6e 7465 7374 5f64  n(self.contest_d
-00004f70: 6961 6c6f 672e 7374 6174 696f 6e2c 2076  ialog.station, v
-00004f80: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
-00004f90: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
-00004fa0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-00004fb0: 2241 7373 6973 7465 6443 6174 6567 6f72  "AssistedCategor
-00004fc0: 7922 290a 2020 2020 2020 2020 7365 6c66  y").        self
-00004fd0: 2e72 6566 696c 6c5f 6472 6f70 646f 776e  .refill_dropdown
-00004fe0: 2873 656c 662e 636f 6e74 6573 745f 6469  (self.contest_di
-00004ff0: 616c 6f67 2e61 7373 6973 7465 642c 2076  alog.assisted, v
-00005000: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
-00005010: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
-00005020: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-00005030: 2254 7261 6e73 6d69 7474 6572 4361 7465  "TransmitterCate
-00005040: 676f 7279 2229 0a20 2020 2020 2020 2073  gory").        s
-00005050: 656c 662e 7265 6669 6c6c 5f64 726f 7064  elf.refill_dropd
-00005060: 6f77 6e28 7365 6c66 2e63 6f6e 7465 7374  own(self.contest
-00005070: 5f64 6961 6c6f 672e 7472 616e 736d 6974  _dialog.transmit
-00005080: 7465 722c 2076 616c 7565 290a 2020 2020  ter, value).    
-00005090: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
-000050a0: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
-000050b0: 732e 6765 7428 2253 7461 7274 4461 7465  s.get("StartDate
-000050c0: 2229 0a20 2020 2020 2020 2074 6865 5f64  ").        the_d
-000050d0: 6174 652c 2074 6865 5f74 696d 6520 3d20  ate, the_time = 
-000050e0: 7661 6c75 652e 7370 6c69 7428 290a 2020  value.split().  
-000050f0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00005100: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
-00005110: 6d65 4564 6974 2e73 6574 4461 7465 280a  meEdit.setDate(.
-00005120: 2020 2020 2020 2020 2020 2020 5174 436f              QtCo
-00005130: 7265 2e51 4461 7465 2e66 726f 6d53 7472  re.QDate.fromStr
-00005140: 696e 6728 7468 655f 6461 7465 2c20 2279  ing(the_date, "y
-00005150: 7979 792d 4d4d 2d64 6422 290a 2020 2020  yyy-MM-dd").    
-00005160: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-00005170: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005180: 672e 6461 7465 5469 6d65 4564 6974 2e73  g.dateTimeEdit.s
-00005190: 6574 4361 6c65 6e64 6172 506f 7075 7028  etCalendarPopup(
-000051a0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
-000051b0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-000051c0: 672e 6461 7465 5469 6d65 4564 6974 2e73  g.dateTimeEdit.s
-000051d0: 6574 5469 6d65 280a 2020 2020 2020 2020  etTime(.        
-000051e0: 2020 2020 5174 436f 7265 2e51 5469 6d65      QtCore.QTime
-000051f0: 2e66 726f 6d53 7472 696e 6728 7468 655f  .fromString(the_
-00005200: 7469 6d65 2c20 2268 683a 6d6d 3a73 7322  time, "hh:mm:ss"
-00005210: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-00005220: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00005230: 5f64 6961 6c6f 672e 6f70 656e 2829 0a0a  _dialog.open()..
-00005240: 2020 2020 6465 6620 7361 7665 5f65 6469      def save_edi
-00005250: 7465 645f 636f 6e74 6573 7428 7365 6c66  ted_contest(self
-00005260: 293a 0a20 2020 2020 2020 2022 2222 5361  ):.        """Sa
-00005270: 7665 2074 6865 2065 6469 7465 6420 636f  ve the edited co
-00005280: 6e74 6573 7422 2222 0a20 2020 2020 2020  ntest""".       
-00005290: 2063 6f6e 7465 7374 203d 207b 7d0a 2020   contest = {}.  
-000052a0: 2020 2020 2020 636f 6e74 6573 745b 2243        contest["C
-000052b0: 6f6e 7465 7374 4e61 6d65 225d 203d 2028  ontestName"] = (
-000052c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000052d0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-000052e0: 2e63 6f6e 7465 7374 2e63 7572 7265 6e74  .contest.current
-000052f0: 5465 7874 2829 2e6c 6f77 6572 2829 2e72  Text().lower().r
-00005300: 6570 6c61 6365 2822 2022 2c20 225f 2229  eplace(" ", "_")
-00005310: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00005320: 2020 2063 6f6e 7465 7374 5b22 5374 6172     contest["Star
-00005330: 7444 6174 6522 5d20 3d20 7365 6c66 2e63  tDate"] = self.c
-00005340: 6f6e 7465 7374 5f64 6961 6c6f 672e 6461  ontest_dialog.da
-00005350: 7465 5469 6d65 4564 6974 2e64 6174 6554  teTimeEdit.dateT
-00005360: 696d 6528 292e 746f 5374 7269 6e67 280a  ime().toString(.
-00005370: 2020 2020 2020 2020 2020 2020 2279 7979              "yyy
-00005380: 792d 4d4d 2d64 6420 6868 3a6d 6d3a 7373  y-MM-dd hh:mm:ss
-00005390: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
-000053a0: 2020 2020 636f 6e74 6573 745b 224f 7065      contest["Ope
-000053b0: 7261 746f 7243 6174 6567 6f72 7922 5d20  ratorCategory"] 
-000053c0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-000053d0: 6961 6c6f 672e 6f70 6572 6174 6f72 5f63  ialog.operator_c
-000053e0: 6c61 7373 2e63 7572 7265 6e74 5465 7874  lass.currentText
-000053f0: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-00005400: 7374 5b22 4261 6e64 4361 7465 676f 7279  st["BandCategory
-00005410: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00005420: 745f 6469 616c 6f67 2e62 616e 642e 6375  t_dialog.band.cu
-00005430: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
-00005440: 2020 2020 636f 6e74 6573 745b 2250 6f77      contest["Pow
-00005450: 6572 4361 7465 676f 7279 225d 203d 2073  erCategory"] = s
-00005460: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005470: 6f67 2e70 6f77 6572 2e63 7572 7265 6e74  og.power.current
-00005480: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
-00005490: 6f6e 7465 7374 5b22 4d6f 6465 4361 7465  ontest["ModeCate
-000054a0: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
-000054b0: 6e74 6573 745f 6469 616c 6f67 2e6d 6f64  ntest_dialog.mod
-000054c0: 652e 6375 7272 656e 7454 6578 7428 290a  e.currentText().
-000054d0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
-000054e0: 224f 7665 726c 6179 4361 7465 676f 7279  "OverlayCategory
-000054f0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00005500: 745f 6469 616c 6f67 2e6f 7665 726c 6179  t_dialog.overlay
-00005510: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
-00005520: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-00005530: 4f70 6572 6174 6f72 7322 5d20 3d20 7365  Operators"] = se
-00005540: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005550: 672e 6f70 6572 6174 6f72 732e 7465 7874  g.operators.text
-00005560: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-00005570: 7374 5b22 536f 6170 626f 7822 5d20 3d20  st["Soapbox"] = 
-00005580: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00005590: 6c6f 672e 736f 6170 626f 782e 746f 506c  log.soapbox.toPl
-000055a0: 6169 6e54 6578 7428 290a 2020 2020 2020  ainText().      
-000055b0: 2020 636f 6e74 6573 745b 2253 656e 7445    contest["SentE
-000055c0: 7863 6861 6e67 6522 5d20 3d20 7365 6c66  xchange"] = self
-000055d0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-000055e0: 6578 6368 616e 6765 2e74 6578 7428 290a  exchange.text().
-000055f0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
-00005600: 2243 6f6e 7465 7374 4e52 225d 203d 2073  "ContestNR"] = s
-00005610: 656c 662e 7072 6566 2e67 6574 2822 636f  elf.pref.get("co
-00005620: 6e74 6573 7422 2c20 3129 0a20 2020 2020  ntest", 1).     
-00005630: 2020 2063 6f6e 7465 7374 5b22 5374 6174     contest["Stat
-00005640: 696f 6e43 6174 6567 6f72 7922 5d20 3d20  ionCategory"] = 
-00005650: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00005660: 6c6f 672e 7374 6174 696f 6e2e 6375 7272  log.station.curr
-00005670: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-00005680: 2020 636f 6e74 6573 745b 2241 7373 6973    contest["Assis
-00005690: 7465 6443 6174 6567 6f72 7922 5d20 3d20  tedCategory"] = 
-000056a0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000056b0: 6c6f 672e 6173 7369 7374 6564 2e63 7572  log.assisted.cur
-000056c0: 7265 6e74 5465 7874 2829 0a20 2020 2020  rentText().     
-000056d0: 2020 2063 6f6e 7465 7374 5b22 5472 616e     contest["Tran
-000056e0: 736d 6974 7465 7243 6174 6567 6f72 7922  smitterCategory"
-000056f0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-00005700: 5f64 6961 6c6f 672e 7472 616e 736d 6974  _dialog.transmit
-00005710: 7465 722e 6375 7272 656e 7454 6578 7428  ter.currentText(
-00005720: 290a 0a20 2020 2020 2020 206c 6f67 6765  )..        logge
-00005730: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-00005740: 7b63 6f6e 7465 7374 7d22 290a 2020 2020  {contest}").    
-00005750: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
-00005760: 652e 7570 6461 7465 5f63 6f6e 7465 7374  e.update_contest
-00005770: 2863 6f6e 7465 7374 290a 2020 2020 2020  (contest).      
-00005780: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
-00005790: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
-000057a0: 2020 7365 6c66 2e6c 6f61 645f 636f 6e74    self.load_cont
-000057b0: 6573 7428 290a 0a20 2020 2064 6566 206c  est()..    def l
-000057c0: 6f61 645f 636f 6e74 6573 7428 7365 6c66  oad_contest(self
-000057d0: 293a 0a20 2020 2020 2020 2022 2222 6c6f  ):.        """lo
-000057e0: 6164 2061 2063 6f6e 7465 7374 2222 220a  ad a contest""".
-000057f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00005800: 7072 6566 2e67 6574 2822 636f 6e74 6573  pref.get("contes
-00005810: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
-00005820: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
-00005830: 7474 696e 6773 203d 2073 656c 662e 6461  ttings = self.da
-00005840: 7461 6261 7365 2e66 6574 6368 5f63 6f6e  tabase.fetch_con
-00005850: 7465 7374 5f62 795f 6964 280a 2020 2020  test_by_id(.    
-00005860: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005870: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
-00005880: 7374 2229 0a20 2020 2020 2020 2020 2020  st").           
-00005890: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-000058a0: 6620 7365 6c66 2e63 6f6e 7465 7374 5f73  f self.contest_s
-000058b0: 6574 7469 6e67 733a 0a20 2020 2020 2020  ettings:.       
-000058c0: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
-000058d0: 7461 6261 7365 2e63 7572 7265 6e74 5f63  tabase.current_c
-000058e0: 6f6e 7465 7374 203d 2073 656c 662e 7072  ontest = self.pr
-000058f0: 6566 2e67 6574 2822 636f 6e74 6573 7422  ef.get("contest"
-00005900: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005910: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-00005920: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
-00005930: 436f 6e74 6573 744e 616d 6522 293a 0a20  ContestName"):. 
-00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005950: 2020 2073 656c 662e 636f 6e74 6573 7420     self.contest 
-00005960: 3d20 646f 696d 7028 7365 6c66 2e63 6f6e  = doimp(self.con
-00005970: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-00005980: 7428 2243 6f6e 7465 7374 4e61 6d65 2229  t("ContestName")
-00005990: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000059a0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000059b0: 7567 2822 4c6f 6164 6564 2043 6f6e 7465  ug("Loaded Conte
-000059c0: 7374 204e 616d 6520 3d20 2573 222c 2073  st Name = %s", s
-000059d0: 656c 662e 636f 6e74 6573 742e 6e61 6d65  elf.contest.name
-000059e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000059f0: 2020 2020 2020 7365 6c66 2e73 6574 5f77        self.set_w
-00005a00: 696e 646f 775f 7469 746c 6528 290a 2020  indow_title().  
-00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a20: 2020 7365 6c66 2e63 6f6e 7465 7374 2e69    self.contest.i
-00005a30: 6e69 745f 636f 6e74 6573 7428 7365 6c66  nit_contest(self
-00005a40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005a50: 2020 2020 2020 7365 6c66 2e68 6964 655f        self.hide_
-00005a60: 6261 6e64 5f6d 6f64 6528 7365 6c66 2e63  band_mode(self.c
-00005a70: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
-00005a80: 6765 7428 224d 6f64 6543 6174 6567 6f72  get("ModeCategor
-00005a90: 7922 2c20 2222 2929 0a0a 2020 2020 2020  y", ""))..      
-00005aa0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-00005ab0: 6174 7472 2873 656c 662e 636f 6e74 6573  attr(self.contes
-00005ac0: 742c 2022 6d6f 6465 2229 3a0a 2020 2020  t, "mode"):.    
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ae0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
-00005af0: 6d6f 6465 2069 6e20 5b22 4357 222c 2022  mode in ["CW", "
-00005b00: 424f 5448 225d 3a0a 2020 2020 2020 2020  BOTH"]:.        
-00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 7365 6c66 2e63 775f 7370 6565 642e 7368  self.cw_speed.sh
-00005b30: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
-00005b40: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 2020 2073 656c 662e 6377 5f73         self.cw_s
-00005b70: 7065 6564 2e68 6964 6528 290a 0a20 2020  peed.hide()..   
-00005b80: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00005b90: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-00005ba0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
-00005bb0: 203d 2022 4e45 5744 4222 0a20 2020 2020   = "NEWDB".     
-00005bc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005bd0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-00005be0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-00005bf0: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
-00005c00: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-00005c10: 2873 656c 662e 636f 6e74 6573 742c 2022  (self.contest, "
-00005c20: 636f 6c75 6d6e 7322 293a 0a20 2020 2020  columns"):.     
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00005c40: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
-00005c50: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00005c60: 2263 6d64 225d 203d 2022 5348 4f57 434f  "cmd"] = "SHOWCO
-00005c70: 4c55 4d4e 5322 0a20 2020 2020 2020 2020  LUMNS".         
-00005c80: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00005c90: 434f 4c55 4d4e 5322 5d20 3d20 7365 6c66  COLUMNS"] = self
-00005ca0: 2e63 6f6e 7465 7374 2e63 6f6c 756d 6e73  .contest.columns
-00005cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cc0: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
-00005cd0: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
-00005ce0: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
-00005cf0: 0a20 2020 2064 6566 2068 6964 655f 6261  .    def hide_ba
-00005d00: 6e64 5f6d 6f64 6528 7365 6c66 2c20 7468  nd_mode(self, th
-00005d10: 655f 6d6f 6465 3a20 7374 7229 202d 3e20  e_mode: str) -> 
-00005d20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00005d30: 2268 6964 6522 2222 0a20 2020 2020 2020  "hide""".       
-00005d40: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-00005d50: 7322 2c20 6622 7b74 6865 5f6d 6f64 657d  s", f"{the_mode}
-00005d60: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00005d70: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
-00005d80: 4357 2e68 6964 6528 290a 2020 2020 2020  CW.hide().      
-00005d90: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
-00005da0: 5f46 7261 6d65 5f53 5342 2e68 6964 6528  _Frame_SSB.hide(
-00005db0: 290a 2020 2020 2020 2020 7365 6c66 2e42  ).        self.B
-00005dc0: 616e 645f 4d6f 6465 5f46 7261 6d65 5f52  and_Mode_Frame_R
-00005dd0: 5454 592e 6869 6465 2829 0a20 2020 2020  TTY.hide().     
-00005de0: 2020 206d 6f64 6573 203d 207b 0a20 2020     modes = {.   
-00005df0: 2020 2020 2020 2020 2022 4357 223a 2028           "CW": (
-00005e00: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
-00005e10: 7261 6d65 5f43 572c 292c 0a20 2020 2020  rame_CW,),.     
-00005e20: 2020 2020 2020 2022 5353 4222 3a20 2873         "SSB": (s
-00005e30: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
-00005e40: 616d 655f 5353 422c 292c 0a20 2020 2020  ame_SSB,),.     
-00005e50: 2020 2020 2020 2022 5254 5459 223a 2028         "RTTY": (
-00005e60: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
-00005e70: 7261 6d65 5f52 5454 592c 292c 0a20 2020  rame_RTTY,),.   
-00005e80: 2020 2020 2020 2020 2022 5053 4b22 3a20           "PSK": 
-00005e90: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-00005ea0: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
-00005eb0: 2020 2020 2020 2020 2020 2253 5342 2b43            "SSB+C
-00005ec0: 5722 3a20 2873 656c 662e 4261 6e64 5f4d  W": (self.Band_M
-00005ed0: 6f64 655f 4672 616d 655f 4357 2c20 7365  ode_Frame_CW, se
-00005ee0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00005ef0: 6d65 5f53 5342 292c 0a20 2020 2020 2020  me_SSB),.       
-00005f00: 2020 2020 2022 4449 4749 5441 4c22 3a20       "DIGITAL": 
-00005f10: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-00005f20: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
-00005f30: 2020 2020 2020 2020 2020 2253 5342 2b43            "SSB+C
-00005f40: 572b 4449 4749 5441 4c22 3a20 280a 2020  W+DIGITAL": (.  
-00005f50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005f60: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00005f70: 6d65 5f52 5454 592c 0a20 2020 2020 2020  me_RTTY,.       
-00005f80: 2020 2020 2020 2020 2073 656c 662e 4261           self.Ba
-00005f90: 6e64 5f4d 6f64 655f 4672 616d 655f 4357  nd_Mode_Frame_CW
-00005fa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005fb0: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
-00005fc0: 5f46 7261 6d65 5f53 5342 2c0a 2020 2020  _Frame_SSB,.    
-00005fd0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00005fe0: 2020 2020 2020 2022 464d 223a 2028 7365         "FM": (se
-00005ff0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00006000: 6d65 5f53 5342 2c29 2c0a 2020 2020 2020  me_SSB,),.      
-00006010: 2020 7d0a 2020 2020 2020 2020 6672 616d    }.        fram
-00006020: 6573 203d 206d 6f64 6573 2e67 6574 2874  es = modes.get(t
-00006030: 6865 5f6d 6f64 6529 0a20 2020 2020 2020  he_mode).       
-00006040: 2069 6620 6672 616d 6573 3a0a 2020 2020   if frames:.    
-00006050: 2020 2020 2020 2020 666f 7220 6672 616d          for fram
-00006060: 6520 696e 2066 7261 6d65 733a 0a20 2020  e in frames:.   
-00006070: 2020 2020 2020 2020 2020 2020 2066 7261               fra
-00006080: 6d65 2e73 686f 7728 290a 0a20 2020 2064  me.show()..    d
-00006090: 6566 2066 696c 6570 6963 6b65 7228 7365  ef filepicker(se
-000060a0: 6c66 2c20 6163 7469 6f6e 3a20 7374 7229  lf, action: str)
-000060b0: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-000060c0: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
-000060d0: 2061 2066 696c 656e 616d 650a 2020 2020   a filename.    
-000060e0: 2020 2020 6163 7469 6f6e 3a20 226e 6577      action: "new
-000060f0: 2220 6f72 2022 6f70 656e 220a 2020 2020  " or "open".    
-00006100: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006110: 6f70 7469 6f6e 7320 3d20 5146 696c 6544  options = QFileD
-00006120: 6961 6c6f 672e 4f70 7469 6f6e 7328 290a  ialog.Options().
-00006130: 2020 2020 2020 2020 6f70 7469 6f6e 7320          options 
-00006140: 7c3d 2051 4669 6c65 4469 616c 6f67 2e44  |= QFileDialog.D
-00006150: 6f6e 7455 7365 4e61 7469 7665 4469 616c  ontUseNativeDial
-00006160: 6f67 0a20 2020 2020 2020 206f 7074 696f  og.        optio
-00006170: 6e73 207c 3d20 5146 696c 6544 6961 6c6f  ns |= QFileDialo
-00006180: 672e 446f 6e74 436f 6e66 6972 6d4f 7665  g.DontConfirmOve
-00006190: 7277 7269 7465 0a20 2020 2020 2020 2023  rwrite.        #
-000061a0: 2070 6963 6b65 7220 3d20 5146 696c 6544   picker = QFileD
-000061b0: 6961 6c6f 6728 7365 6c66 290a 2020 2020  ialog(self).    
-000061c0: 2020 2020 6966 2061 6374 696f 6e20 3d3d      if action ==
-000061d0: 2022 6e65 7722 3a0a 2020 2020 2020 2020   "new":.        
-000061e0: 2020 2020 6669 6c65 2c20 5f20 3d20 5146      file, _ = QF
-000061f0: 696c 6544 6961 6c6f 672e 6765 7453 6176  ileDialog.getSav
-00006200: 6546 696c 654e 616d 6528 0a20 2020 2020  eFileName(.     
-00006210: 2020 2020 2020 2020 2020 2073 656c 662c             self,
-00006220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006230: 2022 4368 6f6f 7365 2061 2044 6174 6162   "Choose a Datab
-00006240: 6173 6522 2c0a 2020 2020 2020 2020 2020  ase",.          
-00006250: 2020 2020 2020 4441 5441 5f50 4154 482c        DATA_PATH,
-00006260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006270: 2022 4461 7461 6261 7365 2028 2a2e 6462   "Database (*.db
-00006280: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-00006290: 2020 2020 6f70 7469 6f6e 733d 6f70 7469      options=opti
-000062a0: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-000062b0: 2029 0a20 2020 2020 2020 2069 6620 6163   ).        if ac
-000062c0: 7469 6f6e 203d 3d20 226f 7065 6e22 3a0a  tion == "open":.
-000062d0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-000062e0: 2c20 5f20 3d20 5146 696c 6544 6961 6c6f  , _ = QFileDialo
-000062f0: 672e 6765 744f 7065 6e46 696c 654e 616d  g.getOpenFileNam
-00006300: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00006310: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00006320: 2020 2020 2020 2020 2022 4368 6f6f 7365           "Choose
-00006330: 2061 2044 6174 6162 6173 6522 2c0a 2020   a Database",.  
-00006340: 2020 2020 2020 2020 2020 2020 2020 4441                DA
-00006350: 5441 5f50 4154 482c 0a20 2020 2020 2020  TA_PATH,.       
-00006360: 2020 2020 2020 2020 2022 4461 7461 6261           "Databa
-00006370: 7365 2028 2a2e 6462 2922 2c0a 2020 2020  se (*.db)",.    
-00006380: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00006390: 6f6e 733d 6f70 7469 6f6e 732c 0a20 2020  ons=options,.   
-000063a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000063b0: 2020 2072 6574 7572 6e20 6669 6c65 0a0a     return file..
-000063c0: 2020 2020 6465 6620 7265 6361 6c63 756c      def recalcul
-000063d0: 6174 655f 6d75 6c74 7328 7365 6c66 293a  ate_mults(self):
-000063e0: 0a20 2020 2020 2020 2022 2222 5265 6361  .        """Reca
-000063f0: 6c63 756c 6174 6520 4d75 6c74 6970 6c69  lculate Multipli
-00006400: 6572 7322 2222 0a20 2020 2020 2020 2073  ers""".        s
-00006410: 656c 662e 636f 6e74 6573 742e 7265 6361  elf.contest.reca
-00006420: 6c63 756c 6174 655f 6d75 6c74 7328 7365  lculate_mults(se
-00006430: 6c66 290a 0a20 2020 2064 6566 206c 6175  lf)..    def lau
-00006440: 6e63 685f 6c6f 675f 7769 6e64 6f77 2873  nch_log_window(s
-00006450: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00006460: 226c 6175 6e63 6820 7468 6520 4c6f 6720  "launch the Log 
-00006470: 5769 6e64 6f77 2222 220a 2020 2020 2020  Window""".      
-00006480: 2020 6966 206e 6f74 2063 6865 636b 5f70    if not check_p
-00006490: 726f 6365 7373 2822 6c6f 6777 696e 646f  rocess("logwindo
-000064a0: 772e 7079 2229 3a0a 2020 2020 2020 2020  w.py"):.        
-000064b0: 2020 2020 5f20 3d20 7375 6270 726f 6365      _ = subproce
-000064c0: 7373 2e50 6f70 656e 285b 7379 732e 6578  ss.Popen([sys.ex
-000064d0: 6563 7574 6162 6c65 2c20 574f 524b 494e  ecutable, WORKIN
-000064e0: 475f 5041 5448 202b 2022 2f6c 6f67 7769  G_PATH + "/logwi
-000064f0: 6e64 6f77 2e70 7922 5d29 0a0a 2020 2020  ndow.py"])..    
-00006500: 6465 6620 6c61 756e 6368 5f62 616e 646d  def launch_bandm
-00006510: 6170 5f77 696e 646f 7728 7365 6c66 293a  ap_window(self):
-00006520: 0a20 2020 2020 2020 2022 2222 6c61 756e  .        """laun
-00006530: 6368 2074 6865 204c 6f67 2057 696e 646f  ch the Log Windo
-00006540: 7722 2222 0a20 2020 2020 2020 2069 6620  w""".        if 
-00006550: 6e6f 7420 6368 6563 6b5f 7072 6f63 6573  not check_proces
-00006560: 7328 2262 616e 646d 6170 2e70 7922 293a  s("bandmap.py"):
-00006570: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
-00006580: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
-00006590: 6e28 5b73 7973 2e65 7865 6375 7461 626c  n([sys.executabl
-000065a0: 652c 2057 4f52 4b49 4e47 5f50 4154 4820  e, WORKING_PATH 
-000065b0: 2b20 222f 6261 6e64 6d61 702e 7079 225d  + "/bandmap.py"]
-000065c0: 290a 0a20 2020 2064 6566 2063 6c65 6172  )..    def clear
-000065d0: 5f62 616e 645f 696e 6469 6361 746f 7273  _band_indicators
-000065e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000065f0: 2222 2243 6c65 6172 2074 6865 2069 6e64  """Clear the ind
-00006600: 6963 6174 6f72 7322 2222 0a20 2020 2020  icators""".     
-00006610: 2020 2066 6f72 205f 2c20 696e 6469 6361     for _, indica
-00006620: 746f 7273 2069 6e20 7365 6c66 2e61 6c6c  tors in self.all
-00006630: 5f6d 6f64 655f 696e 6469 6361 746f 7273  _mode_indicators
-00006640: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00006650: 2020 2020 2020 666f 7220 5f2c 2069 6e64        for _, ind
-00006660: 6963 6174 6f72 2069 6e20 696e 6469 6361  icator in indica
-00006670: 746f 7273 2e69 7465 6d73 2829 3a0a 2020  tors.items():.  
-00006680: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00006690: 6469 6361 746f 722e 7365 7446 7261 6d65  dicator.setFrame
-000066a0: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
-000066b0: 5146 7261 6d65 2e4e 6f46 7261 6d65 290a  QFrame.NoFrame).
-000066c0: 0a20 2020 2064 6566 2073 6574 5f62 616e  .    def set_ban
-000066d0: 645f 696e 6469 6361 746f 7228 7365 6c66  d_indicator(self
-000066e0: 2c20 6261 6e64 3a20 7374 7229 202d 3e20  , band: str) -> 
-000066f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00006700: 2253 6574 2074 6865 2062 616e 6420 696e  "Set the band in
-00006710: 6469 6361 746f 7222 2222 0a20 2020 2020  dicator""".     
-00006720: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00006730: 2225 7322 2c20 6622 6261 6e64 3a7b 6261  "%s", f"band:{ba
-00006740: 6e64 7d20 6d6f 6465 3a20 7b73 656c 662e  nd} mode: {self.
-00006750: 6375 7272 656e 745f 6d6f 6465 7d22 290a  current_mode}").
-00006760: 2020 2020 2020 2020 6966 2062 616e 6420          if band 
-00006770: 616e 6420 7365 6c66 2e63 7572 7265 6e74  and self.current
-00006780: 5f6d 6f64 653a 0a20 2020 2020 2020 2020  _mode:.         
-00006790: 2020 2073 656c 662e 636c 6561 725f 6261     self.clear_ba
-000067a0: 6e64 5f69 6e64 6963 6174 6f72 7328 290a  nd_indicators().
-000067b0: 2020 2020 2020 2020 2020 2020 696e 6469              indi
-000067c0: 6361 746f 7220 3d20 7365 6c66 2e61 6c6c  cator = self.all
-000067d0: 5f6d 6f64 655f 696e 6469 6361 746f 7273  _mode_indicators
-000067e0: 5b73 656c 662e 6375 7272 656e 745f 6d6f  [self.current_mo
-000067f0: 6465 5d2e 6765 7428 6261 6e64 2c20 4e6f  de].get(band, No
-00006800: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
-00006810: 6966 2069 6e64 6963 6174 6f72 3a0a 2020  if indicator:.  
-00006820: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00006830: 6469 6361 746f 722e 7365 7446 7261 6d65  dicator.setFrame
-00006840: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
-00006850: 5146 7261 6d65 2e42 6f78 290a 0a20 2020  QFrame.Box)..   
-00006860: 2064 6566 2063 6c6f 7365 4576 656e 7428   def closeEvent(
-00006870: 7365 6c66 2c20 5f65 7665 6e74 293a 0a20  self, _event):. 
-00006880: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00006890: 2020 2057 7269 7465 2077 696e 646f 7720     Write window 
-000068a0: 7369 7a65 2061 6e64 2070 6f73 6974 696f  size and positio
-000068b0: 6e20 746f 2063 6f6e 6669 6720 6669 6c65  n to config file
-000068c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000068d0: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
-000068e0: 7769 6e64 6f77 5f77 6964 7468 225d 203d  window_width"] =
-000068f0: 2073 656c 662e 7369 7a65 2829 2e77 6964   self.size().wid
-00006900: 7468 2829 0a20 2020 2020 2020 2073 656c  th().        sel
-00006910: 662e 7072 6566 5b22 7769 6e64 6f77 5f68  f.pref["window_h
-00006920: 6569 6768 7422 5d20 3d20 7365 6c66 2e73  eight"] = self.s
-00006930: 697a 6528 292e 6865 6967 6874 2829 0a20  ize().height(). 
-00006940: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00006950: 5b22 7769 6e64 6f77 5f78 225d 203d 2073  ["window_x"] = s
-00006960: 656c 662e 706f 7328 292e 7828 290a 2020  elf.pos().x().  
-00006970: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
-00006980: 2277 696e 646f 775f 7922 5d20 3d20 7365  "window_y"] = se
-00006990: 6c66 2e70 6f73 2829 2e79 2829 0a20 2020  lf.pos().y().   
-000069a0: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
-000069b0: 7072 6566 6572 656e 6365 2829 0a0a 2020  preference()..  
-000069c0: 2020 6465 6620 6374 795f 6c6f 6f6b 7570    def cty_lookup
-000069d0: 2873 656c 662c 2063 616c 6c73 6967 6e3a  (self, callsign:
-000069e0: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
-000069f0: 2222 4c6f 6f6b 7570 2063 616c 6c73 6967  ""Lookup callsig
-00006a00: 6e20 696e 2063 7479 2e64 6174 2066 696c  n in cty.dat fil
-00006a10: 6522 2222 0a20 2020 2020 2020 2063 616c  e""".        cal
-00006a20: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
-00006a30: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-00006a40: 2066 6f72 2063 6f75 6e74 2069 6e20 7265   for count in re
-00006a50: 7665 7273 6564 2872 616e 6765 286c 656e  versed(range(len
-00006a60: 2863 616c 6c73 6967 6e29 2929 3a0a 2020  (callsign))):.  
-00006a70: 2020 2020 2020 2020 2020 7365 6172 6368            search
-00006a80: 6974 656d 203d 2063 616c 6c73 6967 6e5b  item = callsign[
-00006a90: 3a20 636f 756e 7420 2b20 315d 0a20 2020  : count + 1].   
-00006aa0: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00006ab0: 3d20 7b6b 6579 3a20 7661 6c20 666f 7220  = {key: val for 
-00006ac0: 6b65 792c 2076 616c 2069 6e20 4354 5946  key, val in CTYF
-00006ad0: 494c 452e 6974 656d 7328 2920 6966 206b  ILE.items() if k
-00006ae0: 6579 203d 3d20 7365 6172 6368 6974 656d  ey == searchitem
-00006af0: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
-00006b00: 206e 6f74 2072 6573 756c 743a 0a20 2020   not result:.   
-00006b10: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00006b20: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00006b30: 2020 6966 2072 6573 756c 742e 6765 7428    if result.get(
-00006b40: 7365 6172 6368 6974 656d 292e 6765 7428  searchitem).get(
-00006b50: 2265 7861 6374 5f6d 6174 6368 2229 3a0a  "exact_match"):.
-00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b70: 6966 2073 6561 7263 6869 7465 6d20 3d3d  if searchitem ==
-00006b80: 2063 616c 6c73 6967 6e3a 0a20 2020 2020   callsign:.     
-00006b90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00006ba0: 6574 7572 6e20 7265 7375 6c74 0a20 2020  eturn result.   
-00006bb0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00006bc0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-00006bd0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-00006be0: 0a20 2020 2064 6566 2063 7773 7065 6564  .    def cwspeed
-00006bf0: 5f73 7069 6e62 6f78 5f63 6861 6e67 6564  _spinbox_changed
-00006c00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00006c10: 2222 2274 7269 6767 6572 6564 2077 6865  """triggered whe
-00006c20: 6e20 7661 6c75 6520 6f66 2043 5720 7370  n value of CW sp
-00006c30: 6565 6420 696e 2074 6865 2073 7069 6e62  eed in the spinb
-00006c40: 6f78 2063 6861 6e67 6573 2e22 2222 0a20  ox changes.""". 
-00006c50: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00006c60: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
-00006c70: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-00006c80: 656c 662e 6377 2e73 7065 6564 203d 2073  elf.cw.speed = s
-00006c90: 656c 662e 6377 5f73 7065 6564 2e76 616c  elf.cw_speed.val
-00006ca0: 7565 2829 0a20 2020 2020 2020 2020 2020  ue().           
-00006cb0: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
-00006cc0: 6622 5c78 3162 327b 7365 6c66 2e63 772e  f"\x1b2{self.cw.
-00006cd0: 7370 6565 647d 2229 0a0a 2020 2020 6465  speed}")..    de
-00006ce0: 6620 6b65 7950 7265 7373 4576 656e 7428  f keyPressEvent(
-00006cf0: 7365 6c66 2c20 6576 656e 7429 3a20 2023  self, event):  #
-00006d00: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-00006d10: 3d69 6e76 616c 6964 2d6e 616d 650a 2020  =invalid-name.  
-00006d20: 2020 2020 2020 2222 2254 6869 7320 6f76        """This ov
-00006d30: 6572 7269 6465 7320 5174 206b 6579 2065  errides Qt key e
-00006d40: 7665 6e74 2e22 2222 0a20 2020 2020 2020  vent.""".       
-00006d50: 206d 6f64 6966 6965 7220 3d20 6576 656e   modifier = even
-00006d60: 742e 6d6f 6469 6669 6572 7328 290a 2020  t.modifiers().  
-00006d70: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-00006d80: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
-00006d90: 6579 5f45 7363 6170 653a 2020 2320 7079  ey_Escape:  # py
-00006da0: 6c69 6e74 3a20 6469 7361 626c 653d 6e6f  lint: disable=no
-00006db0: 2d6d 656d 6265 720a 2020 2020 2020 2020  -member.        
-00006dc0: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
-00006dd0: 7075 7473 2829 0a20 2020 2020 2020 2069  puts().        i
-00006de0: 6620 7365 6c66 2e63 7720 6973 206e 6f74  f self.cw is not
-00006df0: 204e 6f6e 6520 616e 6420 6d6f 6469 6669   None and modifi
-00006e00: 6572 203d 3d20 5174 2e43 6f6e 7472 6f6c  er == Qt.Control
-00006e10: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
-00006e20: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-00006e30: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
-00006e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006e50: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-00006e60: 2822 5c78 3162 3422 290a 2020 2020 2020  ("\x1b4").      
-00006e70: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-00006e80: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f50   == Qt.Key.Key_P
-00006e90: 6167 6555 703a 0a20 2020 2020 2020 2020  ageUp:.         
-00006ea0: 2020 2069 6620 7365 6c66 2e63 7720 6973     if self.cw is
-00006eb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00006ec0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00006ed0: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
-00006ee0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-00006ef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006f00: 6377 2e73 7065 6564 202b 3d20 310a 2020  cw.speed += 1.  
-00006f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f20: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
-00006f30: 7365 7456 616c 7565 2873 656c 662e 6377  setValue(self.cw
-00006f40: 2e73 7065 6564 290a 2020 2020 2020 2020  .speed).        
-00006f50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006f60: 2e63 772e 7365 6e64 6377 2866 225c 7831  .cw.sendcw(f"\x1
-00006f70: 6232 7b73 656c 662e 6377 2e73 7065 6564  b2{self.cw.speed
-00006f80: 7d22 290a 2020 2020 2020 2020 6966 2065  }").        if e
-00006f90: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-00006fa0: 2e4b 6579 2e4b 6579 5f50 6167 6544 6f77  .Key.Key_PageDow
-00006fb0: 6e3a 0a20 2020 2020 2020 2020 2020 2069  n:.            i
-00006fc0: 6620 7365 6c66 2e63 7720 6973 206e 6f74  f self.cw is not
-00006fd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006fe0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00006ff0: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
-00007000: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00007010: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-00007020: 7065 6564 202d 3d20 310a 2020 2020 2020  peed -= 1.      
-00007030: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007040: 6c66 2e63 775f 7370 6565 642e 7365 7456  lf.cw_speed.setV
-00007050: 616c 7565 2873 656c 662e 6377 2e73 7065  alue(self.cw.spe
-00007060: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
-00007070: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-00007080: 7365 6e64 6377 2866 225c 7831 6232 7b73  sendcw(f"\x1b2{s
-00007090: 656c 662e 6377 2e73 7065 6564 7d22 290a  elf.cw.speed}").
-000070a0: 2020 2020 2020 2020 2320 6966 2065 7665          # if eve
-000070b0: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-000070c0: 6579 2e4b 6579 5f45 6e74 6572 3a0a 2020  ey.Key_Enter:.  
-000070d0: 2020 2020 2020 2320 2020 2020 7365 6c66        #     self
-000070e0: 2e73 6176 655f 636f 6e74 6163 7428 290a  .save_contact().
-000070f0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-00007100: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-00007110: 2e4b 6579 5f54 6162 206f 7220 6576 656e  .Key_Tab or even
-00007120: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
-00007130: 792e 4b65 795f 4261 636b 7461 623a 0a20  y.Key_Backtab:. 
-00007140: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007150: 6c66 2e73 656e 742e 6861 7346 6f63 7573  lf.sent.hasFocus
-00007160: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00007170: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00007180: 2822 4672 6f6d 2073 656e 7422 290a 2020  ("From sent").  
-00007190: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000071a0: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
-000071b0: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
-000071e0: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
-000071f0: 7365 6c66 2e73 656e 7429 0a20 2020 2020  self.sent).     
-00007200: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007210: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
-00007220: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00007230: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-00007240: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-00007250: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007260: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
-00007270: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00007280: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00007290: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-000072a0: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
-000072b0: 5f6e 6578 742e 6765 7428 7365 6c66 2e73  _next.get(self.s
-000072c0: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-000072d0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-000072e0: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007300: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
-00007310: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00007320: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00007330: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-00007340: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00007350: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
-00007360: 6966 2073 656c 662e 7265 6365 6976 652e  if self.receive.
-00007370: 6861 7346 6f63 7573 2829 3a0a 2020 2020  hasFocus():.    
-00007380: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00007390: 6572 2e64 6562 7567 2822 4672 6f6d 2072  er.debug("From r
-000073a0: 6563 6569 7665 2229 0a20 2020 2020 2020  eceive").       
-000073b0: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
-000073c0: 6669 6572 203d 3d20 5174 2e53 6869 6674  fier == Qt.Shift
-000073d0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
-000073e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000073f0: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
-00007400: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
-00007410: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
-00007420: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00007430: 765f 7461 622e 7365 7446 6f63 7573 2829  v_tab.setFocus()
-00007440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007450: 2020 2020 2070 7265 765f 7461 622e 6465       prev_tab.de
-00007460: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
-00007470: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00007480: 765f 7461 622e 656e 6428 4661 6c73 6529  v_tab.end(False)
-00007490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000074a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000074b0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-000074c0: 7461 6220 3d20 7365 6c66 2e74 6162 5f6e  tab = self.tab_n
-000074d0: 6578 742e 6765 7428 7365 6c66 2e72 6563  ext.get(self.rec
-000074e0: 6569 7665 290a 2020 2020 2020 2020 2020  eive).          
-000074f0: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00007500: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 6e65 7874 5f74 6162 2e64 6573 656c    next_tab.desel
-00007530: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
-00007540: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00007550: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
-00007560: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00007570: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00007580: 2069 6620 7365 6c66 2e6f 7468 6572 5f31   if self.other_1
-00007590: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
-000075a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000075b0: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
-000075c0: 6f74 6865 725f 3122 290a 2020 2020 2020  other_1").      
-000075d0: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-000075e0: 6966 6965 7220 3d3d 2051 742e 5368 6966  ifier == Qt.Shif
-000075f0: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
-00007600: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007610: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
-00007620: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
-00007630: 2e6f 7468 6572 5f31 290a 2020 2020 2020  .other_1).      
-00007640: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00007650: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
-00007660: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007670: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
-00007680: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-00007690: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-000076a0: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
-000076b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000076c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000076d0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-000076e0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
-000076f0: 6e65 7874 2e67 6574 2873 656c 662e 6f74  next.get(self.ot
-00007700: 6865 725f 3129 0a20 2020 2020 2020 2020  her_1).         
-00007710: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00007720: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 206e 6578 745f 7461 622e 6465 7365     next_tab.dese
-00007750: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
-00007760: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00007770: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
-00007780: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007790: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-000077a0: 2020 6966 2073 656c 662e 6f74 6865 725f    if self.other_
-000077b0: 322e 6861 7346 6f63 7573 2829 3a0a 2020  2.hasFocus():.  
-000077c0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000077d0: 6767 6572 2e64 6562 7567 2822 4672 6f6d  gger.debug("From
-000077e0: 206f 7468 6572 5f32 2229 0a20 2020 2020   other_2").     
-000077f0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-00007800: 6469 6669 6572 203d 3d20 5174 2e53 6869  difier == Qt.Shi
-00007810: 6674 4d6f 6469 6669 6572 3a0a 2020 2020  ftModifier:.    
-00007820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007830: 7072 6576 5f74 6162 203d 2073 656c 662e  prev_tab = self.
-00007840: 7461 625f 7072 6576 2e67 6574 2873 656c  tab_prev.get(sel
-00007850: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
-00007860: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00007870: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
-00007880: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00007890: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
-000078a0: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-000078b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000078c0: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
-000078d0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-000078e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000078f0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00007900: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
-00007910: 5f6e 6578 742e 6765 7428 7365 6c66 2e6f  _next.get(self.o
-00007920: 7468 6572 5f32 290a 2020 2020 2020 2020  ther_2).        
-00007930: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00007940: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
-00007970: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
-00007980: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00007990: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
-000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079b0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-000079c0: 2020 2069 6620 7365 6c66 2e63 616c 6c73     if self.calls
-000079d0: 6967 6e2e 6861 7346 6f63 7573 2829 3a0a  ign.hasFocus():.
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
-00007a00: 6f6d 2063 616c 6c73 6967 6e22 290a 2020  om callsign").  
-00007a10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00007a20: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
-00007a30: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a50: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
-00007a60: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
-00007a70: 7365 6c66 2e63 616c 6c73 6967 6e29 0a20  self.callsign). 
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a90: 2020 2070 7265 765f 7461 622e 7365 7446     prev_tab.setF
-00007aa0: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
-00007ab0: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
-00007ac0: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
-00007ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ae0: 2020 2070 7265 765f 7461 622e 656e 6428     prev_tab.end(
-00007af0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00007b00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000000e0: 2070 6c61 7466 6f72 6d0a 696d 706f 7274   platform.import
+000000f0: 2071 7565 7565 0a69 6d70 6f72 7420 7265   queue.import re
+00000100: 0a69 6d70 6f72 7420 736f 636b 6574 0a69  .import socket.i
+00000110: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
+00000120: 0a69 6d70 6f72 7420 7379 730a 696d 706f  .import sys.impo
+00000130: 7274 2074 6872 6561 6469 6e67 0a69 6d70  rt threading.imp
+00000140: 6f72 7420 7469 6d65 0a69 6d70 6f72 7420  ort time.import 
+00000150: 7575 6964 0a0a 6672 6f6d 2064 6174 6574  uuid..from datet
+00000160: 696d 6520 696d 706f 7274 2064 6174 6574  ime import datet
+00000170: 696d 650a 6672 6f6d 206a 736f 6e20 696d  ime.from json im
+00000180: 706f 7274 2064 756d 7073 2c20 6c6f 6164  port dumps, load
+00000190: 732c 204a 534f 4e44 6563 6f64 6545 7272  s, JSONDecodeErr
+000001a0: 6f72 0a66 726f 6d20 7061 7468 6c69 6220  or.from pathlib 
+000001b0: 696d 706f 7274 2050 6174 680a 6672 6f6d  import Path.from
+000001c0: 2073 6875 7469 6c20 696d 706f 7274 2063   shutil import c
+000001d0: 6f70 7966 696c 650a 6672 6f6d 2078 6d6c  opyfile.from xml
+000001e0: 7270 632e 636c 6965 6e74 2069 6d70 6f72  rpc.client impor
+000001f0: 7420 4572 726f 722c 2053 6572 7665 7250  t Error, ServerP
+00000200: 726f 7879 0a0a 696d 706f 7274 2070 7375  roxy..import psu
+00000210: 7469 6c0a 6672 6f6d 2050 7951 7435 2069  til.from PyQt5 i
+00000220: 6d70 6f72 7420 5174 436f 7265 2c20 5174  mport QtCore, Qt
+00000230: 4775 692c 2051 7457 6964 6765 7473 2c20  Gui, QtWidgets, 
+00000240: 7569 630a 6672 6f6d 2050 7951 7435 2e51  uic.from PyQt5.Q
+00000250: 7457 6964 6765 7473 2069 6d70 6f72 7420  tWidgets import 
+00000260: 5146 696c 6544 6961 6c6f 670a 6672 6f6d  QFileDialog.from
+00000270: 2050 7951 7435 2e51 7443 6f72 6520 696d   PyQt5.QtCore im
+00000280: 706f 7274 2051 506f 696e 7420 2023 2070  port QPoint  # p
+00000290: 796c 696e 743a 2064 6973 6162 6c65 3d6e  ylint: disable=n
+000002a0: 6f2d 6e61 6d65 2d69 6e2d 6d6f 6475 6c65  o-name-in-module
+000002b0: 0a66 726f 6d20 5079 5174 352e 5174 436f  .from PyQt5.QtCo
+000002c0: 7265 2069 6d70 6f72 7420 5144 6972 2c20  re import QDir, 
+000002d0: 5152 6563 742c 2051 5369 7a65 2c20 5174  QRect, QSize, Qt
+000002e0: 0a66 726f 6d20 5079 5174 352e 5174 4775  .from PyQt5.QtGu
+000002f0: 6920 696d 706f 7274 2051 466f 6e74 4461  i import QFontDa
+00000300: 7461 6261 7365 2020 2320 7079 6c69 6e74  tabase  # pylint
+00000310: 3a20 6469 7361 626c 653d 6e6f 2d6e 616d  : disable=no-nam
+00000320: 652d 696e 2d6d 6f64 756c 650a 696d 706f  e-in-module.impo
+00000330: 7274 2073 6f75 6e64 6465 7669 6365 2061  rt sounddevice a
+00000340: 7320 7364 0a69 6d70 6f72 7420 736f 756e  s sd.import soun
+00000350: 6466 696c 6520 6173 2073 660a 0a66 726f  dfile as sf..fro
+00000360: 6d20 6e6f 7431 6d6d 2e6c 6962 2e61 626f  m not1mm.lib.abo
+00000370: 7574 2069 6d70 6f72 7420 4162 6f75 740a  ut import About.
+00000380: 6672 6f6d 206e 6f74 316d 6d2e 6c69 622e  from not1mm.lib.
+00000390: 6361 745f 696e 7465 7266 6163 6520 696d  cat_interface im
+000003a0: 706f 7274 2043 4154 0a66 726f 6d20 6e6f  port CAT.from no
+000003b0: 7431 6d6d 2e6c 6962 2e63 7769 6e74 6572  t1mm.lib.cwinter
+000003c0: 6661 6365 2069 6d70 6f72 7420 4357 0a66  face import CW.f
+000003d0: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e64  rom not1mm.lib.d
+000003e0: 6174 6162 6173 6520 696d 706f 7274 2044  atabase import D
+000003f0: 6174 6142 6173 650a 6672 6f6d 206e 6f74  ataBase.from not
+00000400: 316d 6d2e 6c69 622e 6564 6974 5f6d 6163  1mm.lib.edit_mac
+00000410: 726f 2069 6d70 6f72 7420 4564 6974 4d61  ro import EditMa
+00000420: 6372 6f0a 6672 6f6d 206e 6f74 316d 6d2e  cro.from not1mm.
+00000430: 6c69 622e 6564 6974 5f6f 706f 6e20 696d  lib.edit_opon im
+00000440: 706f 7274 204f 704f 6e0a 6672 6f6d 206e  port OpOn.from n
+00000450: 6f74 316d 6d2e 6c69 622e 6564 6974 5f73  ot1mm.lib.edit_s
+00000460: 7461 7469 6f6e 2069 6d70 6f72 7420 4564  tation import Ed
+00000470: 6974 5374 6174 696f 6e0a 6672 6f6d 206e  itStation.from n
+00000480: 6f74 316d 6d2e 6c69 622e 7365 6c65 6374  ot1mm.lib.select
+00000490: 5f63 6f6e 7465 7374 2069 6d70 6f72 7420  _contest import 
+000004a0: 5365 6c65 6374 436f 6e74 6573 740a 6672  SelectContest.fr
+000004b0: 6f6d 206e 6f74 316d 6d2e 6c69 622e 7365  om not1mm.lib.se
+000004c0: 7474 696e 6773 2069 6d70 6f72 7420 5365  ttings import Se
+000004d0: 7474 696e 6773 0a66 726f 6d20 6e6f 7431  ttings.from not1
+000004e0: 6d6d 2e6c 6962 2e68 616d 5f75 7469 6c69  mm.lib.ham_utili
+000004f0: 7479 2069 6d70 6f72 7420 280a 2020 2020  ty import (.    
+00000500: 6265 6172 696e 672c 0a20 2020 2062 6561  bearing,.    bea
+00000510: 7269 6e67 5f77 6974 685f 6c61 746c 6f6e  ring_with_latlon
+00000520: 2c0a 2020 2020 6361 6c63 756c 6174 655f  ,.    calculate_
+00000530: 7770 785f 7072 6566 6978 2c0a 2020 2020  wpx_prefix,.    
+00000540: 6469 7374 616e 6365 2c0a 2020 2020 6469  distance,.    di
+00000550: 7374 616e 6365 5f77 6974 685f 6c61 746c  stance_with_latl
+00000560: 6f6e 2c0a 2020 2020 6765 745f 6c6f 6767  on,.    get_logg
+00000570: 6564 5f62 616e 642c 0a20 2020 2067 6574  ed_band,.    get
+00000580: 6261 6e64 2c0a 2020 2020 7265 6369 7072  band,.    recipr
+00000590: 6f63 6f6c 2c0a 290a 6672 6f6d 206e 6f74  ocol,.).from not
+000005a0: 316d 6d2e 6c69 622e 6c6f 6f6b 7570 2069  1mm.lib.lookup i
+000005b0: 6d70 6f72 7420 5152 5a6c 6f6f 6b75 702c  mport QRZlookup,
+000005c0: 2048 616d 4442 6c6f 6f6b 7570 2c20 4861   HamDBlookup, Ha
+000005d0: 6d51 5448 0a66 726f 6d20 6e6f 7431 6d6d  mQTH.from not1mm
+000005e0: 2e6c 6962 2e6d 756c 7469 6361 7374 2069  .lib.multicast i
+000005f0: 6d70 6f72 7420 4d75 6c74 6963 6173 740a  mport Multicast.
+00000600: 6672 6f6d 206e 6f74 316d 6d2e 6c69 622e  from not1mm.lib.
+00000610: 6e65 775f 636f 6e74 6573 7420 696d 706f  new_contest impo
+00000620: 7274 204e 6577 436f 6e74 6573 740a 6672  rt NewContest.fr
+00000630: 6f6d 206e 6f74 316d 6d2e 6c69 622e 6e31  om not1mm.lib.n1
+00000640: 6d6d 2069 6d70 6f72 7420 4e31 4d4d 0a66  mm import N1MM.f
+00000650: 726f 6d20 6e6f 7431 6d6d 2e6c 6962 2e76  rom not1mm.lib.v
+00000660: 6572 7369 6f6e 2069 6d70 6f72 7420 5f5f  ersion import __
+00000670: 7665 7273 696f 6e5f 5f0a 0a6f 732e 656e  version__..os.en
+00000680: 7669 726f 6e5b 2251 545f 5150 415f 504c  viron["QT_QPA_PL
+00000690: 4154 464f 524d 5448 454d 4522 5d20 3d20  ATFORMTHEME"] = 
+000006a0: 2267 6e6f 6d65 220a 2320 6f73 2e65 6e76  "gnome".# os.env
+000006b0: 6972 6f6e 5b22 5154 5f53 5459 4c45 5f4f  iron["QT_STYLE_O
+000006c0: 5645 5252 4944 4522 5d20 3d20 2261 6477  VERRIDE"] = "adw
+000006d0: 6169 7461 220a 0a6c 6f61 6465 7220 3d20  aita"..loader = 
+000006e0: 706b 6775 7469 6c2e 6765 745f 6c6f 6164  pkgutil.get_load
+000006f0: 6572 2822 6e6f 7431 6d6d 2229 0a57 4f52  er("not1mm").WOR
+00000700: 4b49 4e47 5f50 4154 4820 3d20 6f73 2e70  KING_PATH = os.p
+00000710: 6174 682e 6469 726e 616d 6528 6c6f 6164  ath.dirname(load
+00000720: 6572 2e67 6574 5f66 696c 656e 616d 6528  er.get_filename(
+00000730: 2929 0a0a 6966 2022 5844 475f 4441 5441  ))..if "XDG_DATA
+00000740: 5f48 4f4d 4522 2069 6e20 6f73 2e65 6e76  _HOME" in os.env
+00000750: 6972 6f6e 3a0a 2020 2020 4441 5441 5f50  iron:.    DATA_P
+00000760: 4154 4820 3d20 6f73 2e65 6e76 6972 6f6e  ATH = os.environ
+00000770: 2e67 6574 2822 5844 475f 4441 5441 5f48  .get("XDG_DATA_H
+00000780: 4f4d 4522 290a 656c 7365 3a0a 2020 2020  OME").else:.    
+00000790: 4441 5441 5f50 4154 4820 3d20 7374 7228  DATA_PATH = str(
+000007a0: 5061 7468 2e68 6f6d 6528 2920 2f20 222e  Path.home() / ".
+000007b0: 6c6f 6361 6c22 202f 2022 7368 6172 6522  local" / "share"
+000007c0: 290a 4441 5441 5f50 4154 4820 2b3d 2022  ).DATA_PATH += "
+000007d0: 2f6e 6f74 316d 6d22 0a74 7279 3a0a 2020  /not1mm".try:.  
+000007e0: 2020 6f73 2e6d 6b64 6972 2844 4154 415f    os.mkdir(DATA_
+000007f0: 5041 5448 290a 6578 6365 7074 2046 696c  PATH).except Fil
+00000800: 6545 7869 7374 7345 7272 6f72 3a0a 2020  eExistsError:.  
+00000810: 2020 2e2e 2e0a 0a69 6620 2258 4447 5f43    .....if "XDG_C
+00000820: 4f4e 4649 475f 484f 4d45 2220 696e 206f  ONFIG_HOME" in o
+00000830: 732e 656e 7669 726f 6e3a 0a20 2020 2043  s.environ:.    C
+00000840: 4f4e 4649 475f 5041 5448 203d 206f 732e  ONFIG_PATH = os.
+00000850: 656e 7669 726f 6e2e 6765 7428 2258 4447  environ.get("XDG
+00000860: 5f43 4f4e 4649 475f 484f 4d45 2229 0a65  _CONFIG_HOME").e
+00000870: 6c73 653a 0a20 2020 2043 4f4e 4649 475f  lse:.    CONFIG_
+00000880: 5041 5448 203d 2073 7472 2850 6174 682e  PATH = str(Path.
+00000890: 686f 6d65 2829 202f 2022 2e63 6f6e 6669  home() / ".confi
+000008a0: 6722 290a 434f 4e46 4947 5f50 4154 4820  g").CONFIG_PATH 
+000008b0: 2b3d 2022 2f6e 6f74 316d 6d22 0a74 7279  += "/not1mm".try
+000008c0: 3a0a 2020 2020 6f73 2e6d 6b64 6972 2843  :.    os.mkdir(C
+000008d0: 4f4e 4649 475f 5041 5448 290a 6578 6365  ONFIG_PATH).exce
+000008e0: 7074 2046 696c 6545 7869 7374 7345 7272  pt FileExistsErr
+000008f0: 6f72 3a0a 2020 2020 2e2e 2e0a 0a43 5459  or:.    .....CTY
+00000900: 4649 4c45 203d 207b 7d0a 0a77 6974 6820  FILE = {}..with 
+00000910: 6f70 656e 2857 4f52 4b49 4e47 5f50 4154  open(WORKING_PAT
+00000920: 4820 2b20 222f 6461 7461 2f63 7479 2e6a  H + "/data/cty.j
+00000930: 736f 6e22 2c20 2272 7422 2c20 656e 636f  son", "rt", enco
+00000940: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
+00000950: 2063 5f66 696c 653a 0a20 2020 2043 5459   c_file:.    CTY
+00000960: 4649 4c45 203d 206c 6f61 6473 2863 5f66  FILE = loads(c_f
+00000970: 696c 652e 7265 6164 2829 290a 0a44 4152  ile.read())..DAR
+00000980: 4b5f 5354 594c 4553 4845 4554 203d 2022  K_STYLESHEET = "
+00000990: 220a 0a77 6974 6820 6f70 656e 2857 4f52  "..with open(WOR
+000009a0: 4b49 4e47 5f50 4154 4820 2b20 222f 6461  KING_PATH + "/da
+000009b0: 7461 2f43 6f6d 6269 6e65 6172 2e71 7373  ta/Combinear.qss
+000009c0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+000009d0: 2d38 2229 2061 7320 7374 796c 6566 696c  -8") as stylefil
+000009e0: 653a 0a20 2020 2044 4152 4b5f 5354 594c  e:.    DARK_STYL
+000009f0: 4553 4845 4554 203d 2073 7479 6c65 6669  ESHEET = stylefi
+00000a00: 6c65 2e72 6561 6428 290a 0a0a 6465 6620  le.read()...def 
+00000a10: 6368 6563 6b5f 7072 6f63 6573 7328 6e61  check_process(na
+00000a20: 6d65 3a20 7374 7229 202d 3e20 626f 6f6c  me: str) -> bool
+00000a30: 3a0a 2020 2020 2222 2263 6865 636b 7320  :.    """checks 
+00000a40: 746f 2073 6565 2069 6620 7072 6f67 7261  to see if progra
+00000a50: 6d20 6f66 206e 616d 6520 6973 2069 6e20  m of name is in 
+00000a60: 7468 6520 6163 7469 7665 2070 726f 6365  the active proce
+00000a70: 7373 206c 6973 7422 2222 0a20 2020 2066  ss list""".    f
+00000a80: 6f72 2070 726f 6320 696e 2070 7375 7469  or proc in psuti
+00000a90: 6c2e 7072 6f63 6573 735f 6974 6572 2829  l.process_iter()
+00000aa0: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
+00000ab0: 2870 726f 632e 636d 646c 696e 6528 2929  (proc.cmdline())
+00000ac0: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
+00000ad0: 2020 2069 6620 6e61 6d65 2069 6e20 7072     if name in pr
+00000ae0: 6f63 2e63 6d64 6c69 6e65 2829 5b31 5d3a  oc.cmdline()[1]:
+00000af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b00: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00000b10: 2072 6574 7572 6e20 4661 6c73 650a 0a0a   return False...
+00000b20: 6465 6620 6374 795f 6c6f 6f6b 7570 2863  def cty_lookup(c
+00000b30: 616c 6c73 6967 6e3a 2073 7472 293a 0a20  allsign: str):. 
+00000b40: 2020 2022 2222 4c6f 6f6b 7570 2063 616c     """Lookup cal
+00000b50: 6c73 6967 6e20 696e 2063 7479 2e64 6174  lsign in cty.dat
+00000b60: 2066 696c 6522 2222 0a20 2020 2063 616c   file""".    cal
+00000b70: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
+00000b80: 2e75 7070 6572 2829 0a20 2020 2066 6f72  .upper().    for
+00000b90: 2063 6f75 6e74 2069 6e20 7265 7665 7273   count in revers
+00000ba0: 6564 2872 616e 6765 286c 656e 2863 616c  ed(range(len(cal
+00000bb0: 6c73 6967 6e29 2929 3a0a 2020 2020 2020  lsign))):.      
+00000bc0: 2020 7365 6172 6368 6974 656d 203d 2063    searchitem = c
+00000bd0: 616c 6c73 6967 6e5b 3a20 636f 756e 7420  allsign[: count 
+00000be0: 2b20 315d 0a20 2020 2020 2020 2072 6573  + 1].        res
+00000bf0: 756c 7420 3d20 7b6b 6579 3a20 7661 6c20  ult = {key: val 
+00000c00: 666f 7220 6b65 792c 2076 616c 2069 6e20  for key, val in 
+00000c10: 4354 5946 494c 452e 6974 656d 7328 2920  CTYFILE.items() 
+00000c20: 6966 206b 6579 203d 3d20 7365 6172 6368  if key == search
+00000c30: 6974 656d 7d0a 2020 2020 2020 2020 6966  item}.        if
+00000c40: 206e 6f74 2072 6573 756c 743a 0a20 2020   not result:.   
+00000c50: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00000c60: 650a 2020 2020 2020 2020 6966 2072 6573  e.        if res
+00000c70: 756c 742e 6765 7428 7365 6172 6368 6974  ult.get(searchit
+00000c80: 656d 292e 6765 7428 2265 7861 6374 5f6d  em).get("exact_m
+00000c90: 6174 6368 2229 3a0a 2020 2020 2020 2020  atch"):.        
+00000ca0: 2020 2020 6966 2073 6561 7263 6869 7465      if searchite
+00000cb0: 6d20 3d3d 2063 616c 6c73 6967 6e3a 0a20  m == callsign:. 
+00000cc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00000cd0: 6574 7572 6e20 7265 7375 6c74 0a20 2020  eturn result.   
+00000ce0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00000cf0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00000d00: 2072 6573 756c 740a 0a0a 636c 6173 7320   result...class 
+00000d10: 4d61 696e 5769 6e64 6f77 2851 7457 6964  MainWindow(QtWid
+00000d20: 6765 7473 2e51 4d61 696e 5769 6e64 6f77  gets.QMainWindow
+00000d30: 293a 0a20 2020 2022 2222 0a20 2020 2054  ):.    """.    T
+00000d40: 6865 206d 6169 6e20 7769 6e64 6f77 0a20  he main window. 
+00000d50: 2020 2022 2222 0a0a 2020 2020 7072 6566     """..    pref
+00000d60: 5f72 6566 203d 207b 0a20 2020 2020 2020  _ref = {.       
+00000d70: 2022 736f 756e 6464 6576 6963 6522 3a20   "sounddevice": 
+00000d80: 2264 6566 6175 6c74 222c 0a20 2020 2020  "default",.     
+00000d90: 2020 2022 7573 6571 727a 223a 2046 616c     "useqrz": Fal
+00000da0: 7365 2c0a 2020 2020 2020 2020 226c 6f6f  se,.        "loo
+00000db0: 6b75 7075 7365 726e 616d 6522 3a20 2275  kupusername": "u
+00000dc0: 7365 726e 616d 6522 2c0a 2020 2020 2020  sername",.      
+00000dd0: 2020 226c 6f6f 6b75 7070 6173 7377 6f72    "lookuppasswor
+00000de0: 6422 3a20 2270 6173 7377 6f72 6422 2c0a  d": "password",.
+00000df0: 2020 2020 2020 2020 2272 756e 5f73 7461          "run_sta
+00000e00: 7465 223a 2054 7275 652c 0a20 2020 2020  te": True,.     
+00000e10: 2020 2022 6461 726b 5f6d 6f64 6522 3a20     "dark_mode": 
+00000e20: 4661 6c73 652c 0a20 2020 2020 2020 2022  False,.        "
+00000e30: 636f 6d6d 616e 645f 6275 7474 6f6e 7322  command_buttons"
+00000e40: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00000e50: 2022 6377 5f6d 6163 726f 7322 3a20 5472   "cw_macros": Tr
+00000e60: 7565 2c0a 2020 2020 2020 2020 2262 616e  ue,.        "ban
+00000e70: 6473 5f6d 6f64 6573 223a 2054 7275 652c  ds_modes": True,
+00000e80: 0a20 2020 2020 2020 2022 7769 6e64 6f77  .        "window
+00000e90: 5f68 6569 6768 7422 3a20 3230 302c 0a20  _height": 200,. 
+00000ea0: 2020 2020 2020 2022 7769 6e64 6f77 5f77         "window_w
+00000eb0: 6964 7468 223a 2036 3030 2c0a 2020 2020  idth": 600,.    
+00000ec0: 2020 2020 2277 696e 646f 775f 7822 3a20      "window_x": 
+00000ed0: 3132 302c 0a20 2020 2020 2020 2022 7769  120,.        "wi
+00000ee0: 6e64 6f77 5f79 223a 2031 3230 2c0a 2020  ndow_y": 120,.  
+00000ef0: 2020 2020 2020 2263 7572 7265 6e74 5f64        "current_d
+00000f00: 6174 6162 6173 6522 3a20 2268 616d 2e64  atabase": "ham.d
+00000f10: 6222 2c0a 2020 2020 2020 2020 2263 6f6e  b",.        "con
+00000f20: 7465 7374 223a 2022 222c 0a20 2020 2020  test": "",.     
+00000f30: 2020 2022 6d75 6c74 6963 6173 745f 6772     "multicast_gr
+00000f40: 6f75 7022 3a20 2232 3234 2e31 2e31 2e31  oup": "224.1.1.1
+00000f50: 222c 0a20 2020 2020 2020 2022 6d75 6c74  ",.        "mult
+00000f60: 6963 6173 745f 706f 7274 223a 2032 3233  icast_port": 223
+00000f70: 392c 0a20 2020 2020 2020 2022 696e 7465  9,.        "inte
+00000f80: 7266 6163 655f 6970 223a 2022 302e 302e  rface_ip": "0.0.
+00000f90: 302e 3022 2c0a 2020 2020 2020 2020 2273  0.0",.        "s
+00000fa0: 656e 645f 6e31 6d6d 5f70 6163 6b65 7473  end_n1mm_packets
+00000fb0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
+00000fc0: 2020 226e 316d 6d5f 7374 6174 696f 6e5f    "n1mm_station_
+00000fd0: 6e61 6d65 223a 2022 3230 4d20 4357 2054  name": "20M CW T
+00000fe0: 656e 7422 2c0a 2020 2020 2020 2020 226e  ent",.        "n
+00000ff0: 316d 6d5f 6f70 6572 6174 6f72 223a 2022  1mm_operator": "
+00001000: 4265 726e 6965 222c 0a20 2020 2020 2020  Bernie",.       
+00001010: 2022 6e31 6d6d 5f69 7022 3a20 2231 3237   "n1mm_ip": "127
+00001020: 2e30 2e30 2e31 222c 0a20 2020 2020 2020  .0.0.1",.       
+00001030: 2022 6e31 6d6d 5f72 6164 696f 706f 7274   "n1mm_radioport
+00001040: 223a 2031 3230 3630 2c0a 2020 2020 2020  ": 12060,.      
+00001050: 2020 226e 316d 6d5f 636f 6e74 6163 7470    "n1mm_contactp
+00001060: 6f72 7422 3a20 3132 3036 312c 0a20 2020  ort": 12061,.   
+00001070: 2020 2020 2022 6e31 6d6d 5f6c 6f6f 6b75       "n1mm_looku
+00001080: 7070 6f72 7422 3a20 3132 3036 302c 0a20  pport": 12060,. 
+00001090: 2020 2020 2020 2022 6e31 6d6d 5f73 636f         "n1mm_sco
+000010a0: 7265 706f 7274 223a 2031 3230 3632 2c0a  report": 12062,.
+000010b0: 2020 2020 2020 2020 2275 7365 6861 6d64          "usehamd
+000010c0: 6222 3a20 4661 6c73 652c 0a20 2020 2020  b": False,.     
+000010d0: 2020 2022 7573 6568 616d 7174 6822 3a20     "usehamqth": 
+000010e0: 4661 6c73 652c 0a20 2020 2020 2020 2022  False,.        "
+000010f0: 636c 6f75 646c 6f67 223a 2046 616c 7365  cloudlog": False
+00001100: 2c0a 2020 2020 2020 2020 2263 6c6f 7564  ,.        "cloud
+00001110: 6c6f 6761 7069 223a 2022 222c 0a20 2020  logapi": "",.   
+00001120: 2020 2020 2022 636c 6f75 646c 6f67 7572       "cloudlogur
+00001130: 6c22 3a20 2222 2c0a 2020 2020 2020 2020  l": "",.        
+00001140: 2243 4154 5f69 7022 3a20 2231 3237 2e30  "CAT_ip": "127.0
+00001150: 2e30 2e31 222c 0a20 2020 2020 2020 2022  .0.1",.        "
+00001160: 7573 6572 6967 6374 6c64 223a 2054 7275  userigctld": Tru
+00001170: 652c 0a20 2020 2020 2020 2022 7573 6566  e,.        "usef
+00001180: 6c72 6967 223a 2046 616c 7365 2c0a 2020  lrig": False,.  
+00001190: 2020 2020 2020 2263 7769 7022 3a20 2231        "cwip": "1
+000011a0: 3237 2e30 2e30 2e31 222c 0a20 2020 2020  27.0.0.1",.     
+000011b0: 2020 2022 6377 706f 7274 223a 2036 3738     "cwport": 678
+000011c0: 392c 0a20 2020 2020 2020 2022 6377 7479  9,.        "cwty
+000011d0: 7065 223a 2031 2c0a 2020 2020 2020 2020  pe": 1,.        
+000011e0: 2275 7365 7365 7276 6572 223a 2046 616c  "useserver": Fal
+000011f0: 7365 2c0a 2020 2020 2020 2020 2243 4154  se,.        "CAT
+00001200: 5f70 6f72 7422 3a20 3435 3332 2c0a 2020  _port": 4532,.  
+00001210: 2020 2020 2020 2263 6c75 7374 6572 5f73        "cluster_s
+00001220: 6572 7665 7222 3a20 2264 7863 2e6e 6337  erver": "dxc.nc7
+00001230: 6a2e 636f 6d22 2c0a 2020 2020 2020 2020  j.com",.        
+00001240: 2263 6c75 7374 6572 5f70 6f72 7422 3a20  "cluster_port": 
+00001250: 3733 3733 2c0a 2020 2020 2020 2020 2263  7373,.        "c
+00001260: 6c75 7374 6572 5f66 696c 7465 7222 3a20  luster_filter": 
+00001270: 2253 6574 2044 5820 4669 6c74 6572 2053  "Set DX Filter S
+00001280: 706f 7474 6572 436f 6e74 3d4e 4122 2c0a  potterCont=NA",.
+00001290: 2020 2020 2020 2020 2263 6c75 7374 6572          "cluster
+000012a0: 5f6d 6f64 6522 3a20 224f 5045 4e22 2c0a  _mode": "OPEN",.
+000012b0: 2020 2020 7d0a 2020 2020 6170 7073 7461      }.    appsta
+000012c0: 7274 6564 203d 2046 616c 7365 0a20 2020  rted = False.   
+000012d0: 2063 6f6e 7461 6374 203d 207b 7d0a 2020   contact = {}.  
+000012e0: 2020 636f 6e74 6573 7420 3d20 4e6f 6e65    contest = None
+000012f0: 0a20 2020 2063 6f6e 7465 7374 5f73 6574  .    contest_set
+00001300: 7469 6e67 7320 3d20 7b7d 0a20 2020 2070  tings = {}.    p
+00001310: 7265 6620 3d20 4e6f 6e65 0a20 2020 2073  ref = None.    s
+00001320: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
+00001330: 6375 7272 656e 745f 6f70 203d 2022 220a  current_op = "".
+00001340: 2020 2020 6375 7272 656e 745f 6d6f 6465      current_mode
+00001350: 203d 2022 220a 2020 2020 6375 7272 656e   = "".    curren
+00001360: 745f 6261 6e64 203d 2022 220a 2020 2020  t_band = "".    
+00001370: 6377 203d 204e 6f6e 650a 2020 2020 6c6f  cw = None.    lo
+00001380: 6f6b 5f75 7020 3d20 4e6f 6e65 0a20 2020  ok_up = None.   
+00001390: 2072 756e 5f73 7461 7465 203d 2046 616c   run_state = Fal
+000013a0: 7365 0a20 2020 2066 6b65 7973 203d 207b  se.    fkeys = {
+000013b0: 7d0a 2020 2020 6162 6f75 745f 6469 616c  }.    about_dial
+000013c0: 6f67 203d 204e 6f6e 650a 2020 2020 7172  og = None.    qr
+000013d0: 7a5f 6469 616c 6f67 203d 204e 6f6e 650a  z_dialog = None.
+000013e0: 2020 2020 7365 7474 696e 6773 5f64 6961      settings_dia
+000013f0: 6c6f 6720 3d20 4e6f 6e65 0a20 2020 2065  log = None.    e
+00001400: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
+00001410: 203d 204e 6f6e 650a 2020 2020 636f 6e74   = None.    cont
+00001420: 6573 745f 6469 616c 6f67 203d 204e 6f6e  est_dialog = Non
+00001430: 650a 2020 2020 636f 6e66 6967 7572 6174  e.    configurat
+00001440: 696f 6e5f 6469 616c 6f67 203d 204e 6f6e  ion_dialog = Non
+00001450: 650a 2020 2020 6f70 6f6e 5f64 6961 6c6f  e.    opon_dialo
+00001460: 6720 3d20 4e6f 6e65 0a20 2020 2064 626e  g = None.    dbn
+00001470: 616d 6520 3d20 4441 5441 5f50 4154 4820  ame = DATA_PATH 
+00001480: 2b20 222f 6861 6d2e 6462 220a 2020 2020  + "/ham.db".    
+00001490: 7261 6469 6f5f 7374 6174 6520 3d20 7b7d  radio_state = {}
+000014a0: 0a20 2020 2072 6967 5f63 6f6e 7472 6f6c  .    rig_control
+000014b0: 203d 204e 6f6e 650a 2020 2020 7365 7276   = None.    serv
+000014c0: 6572 5f75 6470 203d 204e 6f6e 650a 2020  er_udp = None.  
+000014d0: 2020 6d75 6c74 6963 6173 745f 6772 6f75    multicast_grou
+000014e0: 7020 3d20 4e6f 6e65 0a20 2020 206d 756c  p = None.    mul
+000014f0: 7469 6361 7374 5f70 6f72 7420 3d20 4e6f  ticast_port = No
+00001500: 6e65 0a20 2020 2069 6e74 6572 6661 6365  ne.    interface
+00001510: 5f69 7020 3d20 4e6f 6e65 0a20 2020 2072  _ip = None.    r
+00001520: 6967 5f63 6f6e 7472 6f6c 203d 204e 6f6e  ig_control = Non
+00001530: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
+00001540: 745f 5f28 7365 6c66 2c20 2a61 7267 732c  t__(self, *args,
+00001550: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+00001560: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+00001570: 6974 5f5f 282a 6172 6773 2c20 2a2a 6b77  it__(*args, **kw
+00001580: 6172 6773 290a 2020 2020 2020 2020 6c6f  args).        lo
+00001590: 6767 6572 2e69 6e66 6f28 224d 6169 6e57  gger.info("MainW
+000015a0: 696e 646f 773a 205f 5f69 6e69 745f 5f22  indow: __init__"
+000015b0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+000015c0: 7564 7077 6174 6368 203d 204e 6f6e 650a  udpwatch = None.
+000015d0: 2020 2020 2020 2020 7365 6c66 2e75 6470          self.udp
+000015e0: 5f66 6966 6f20 3d20 7175 6575 652e 5175  _fifo = queue.Qu
+000015f0: 6575 6528 290a 2020 2020 2020 2020 6461  eue().        da
+00001600: 7461 5f70 6174 6820 3d20 574f 524b 494e  ta_path = WORKIN
+00001610: 475f 5041 5448 202b 2022 2f64 6174 612f  G_PATH + "/data/
+00001620: 6d61 696e 2e75 6922 0a20 2020 2020 2020  main.ui".       
+00001630: 2075 6963 2e6c 6f61 6455 6928 6461 7461   uic.loadUi(data
+00001640: 5f70 6174 682c 2073 656c 6629 0a20 2020  _path, self).   
+00001650: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
+00001660: 742e 6869 6465 2829 0a20 2020 2020 2020  t.hide().       
+00001670: 2073 656c 662e 7269 6768 7464 6f74 2e68   self.rightdot.h
+00001680: 6964 6528 290a 2020 2020 2020 2020 7365  ide().        se
+00001690: 6c66 2e6e 316d 6d20 3d20 4e31 4d4d 2829  lf.n1mm = N1MM()
+000016a0: 0a20 2020 2020 2020 2073 656c 662e 6e65  .        self.ne
+000016b0: 7874 5f66 6965 6c64 203d 2073 656c 662e  xt_field = self.
+000016c0: 6f74 6865 725f 320a 2020 2020 2020 2020  other_2.        
+000016d0: 7365 6c66 2e64 7570 655f 696e 6469 6361  self.dupe_indica
+000016e0: 746f 722e 6869 6465 2829 0a20 2020 2020  tor.hide().     
+000016f0: 2020 2073 656c 662e 6377 5f73 7065 6564     self.cw_speed
+00001700: 2e76 616c 7565 4368 616e 6765 642e 636f  .valueChanged.co
+00001710: 6e6e 6563 7428 7365 6c66 2e63 7773 7065  nnect(self.cwspe
+00001720: 6564 5f73 7069 6e62 6f78 5f63 6861 6e67  ed_spinbox_chang
+00001730: 6564 290a 0a20 2020 2020 2020 2073 656c  ed)..        sel
+00001740: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
+00001750: 732e 7472 6967 6765 7265 642e 636f 6e6e  s.triggered.conn
+00001760: 6563 7428 7365 6c66 2e63 775f 6d61 6372  ect(self.cw_macr
+00001770: 6f73 5f73 7461 7465 5f63 6861 6e67 6564  os_state_changed
+00001780: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00001790: 6374 696f 6e43 6f6d 6d61 6e64 5f42 7574  ctionCommand_But
+000017a0: 746f 6e73 2e74 7269 6767 6572 6564 2e63  tons.triggered.c
+000017b0: 6f6e 6e65 6374 2873 656c 662e 636f 6d6d  onnect(self.comm
+000017c0: 616e 645f 6275 7474 6f6e 735f 7374 6174  and_buttons_stat
+000017d0: 655f 6368 616e 6765 290a 2020 2020 2020  e_change).      
+000017e0: 2020 7365 6c66 2e61 6374 696f 6e44 6172    self.actionDar
+000017f0: 6b5f 4d6f 6465 2e74 7269 6767 6572 6564  k_Mode.triggered
+00001800: 2e63 6f6e 6e65 6374 2873 656c 662e 6461  .connect(self.da
+00001810: 726b 5f6d 6f64 655f 7374 6174 655f 6368  rk_mode_state_ch
+00001820: 616e 6765 290a 2020 2020 2020 2020 7365  ange).        se
+00001830: 6c66 2e61 6374 696f 6e4c 6f67 5f57 696e  lf.actionLog_Win
+00001840: 646f 772e 7472 6967 6765 7265 642e 636f  dow.triggered.co
+00001850: 6e6e 6563 7428 7365 6c66 2e6c 6175 6e63  nnect(self.launc
+00001860: 685f 6c6f 675f 7769 6e64 6f77 290a 2020  h_log_window).  
+00001870: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001880: 6e42 616e 646d 6170 2e74 7269 6767 6572  nBandmap.trigger
+00001890: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+000018a0: 6c61 756e 6368 5f62 616e 646d 6170 5f77  launch_bandmap_w
+000018b0: 696e 646f 7729 0a20 2020 2020 2020 2073  indow).        s
+000018c0: 656c 662e 6163 7469 6f6e 5265 6361 6c63  elf.actionRecalc
+000018d0: 756c 6174 655f 4d75 6c74 732e 7472 6967  ulate_Mults.trig
+000018e0: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
+000018f0: 6c66 2e72 6563 616c 6375 6c61 7465 5f6d  lf.recalculate_m
+00001900: 756c 7473 290a 0a20 2020 2020 2020 2073  ults)..        s
+00001910: 656c 662e 6163 7469 6f6e 4765 6e65 7261  elf.actionGenera
+00001920: 7465 5f43 6162 7269 6c6c 6f2e 7472 6967  te_Cabrillo.trig
+00001930: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
+00001940: 6c66 2e67 656e 6572 6174 655f 6361 6272  lf.generate_cabr
+00001950: 696c 6c6f 290a 2020 2020 2020 2020 7365  illo).        se
+00001960: 6c66 2e61 6374 696f 6e47 656e 6572 6174  lf.actionGenerat
+00001970: 655f 4144 4946 2e74 7269 6767 6572 6564  e_ADIF.triggered
+00001980: 2e63 6f6e 6e65 6374 2873 656c 662e 6765  .connect(self.ge
+00001990: 6e65 7261 7465 5f61 6469 6629 0a0a 2020  nerate_adif)..  
+000019a0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+000019b0: 6e43 6f6e 6669 6775 7261 7469 6f6e 5f53  nConfiguration_S
+000019c0: 6574 7469 6e67 732e 7472 6967 6765 7265  ettings.triggere
+000019d0: 642e 636f 6e6e 6563 7428 0a20 2020 2020  d.connect(.     
+000019e0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+000019f0: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f73  _configuration_s
+00001a00: 6574 7469 6e67 730a 2020 2020 2020 2020  ettings.        
+00001a10: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00001a20: 6374 696f 6e53 7461 7469 6f6e 5365 7474  ctionStationSett
+00001a30: 696e 6773 2e74 7269 6767 6572 6564 2e63  ings.triggered.c
+00001a40: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
+00001a50: 5f73 7461 7469 6f6e 5f73 6574 7469 6e67  _station_setting
+00001a60: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
+00001a70: 2e61 6374 696f 6e4e 6577 5f43 6f6e 7465  .actionNew_Conte
+00001a80: 7374 2e74 7269 6767 6572 6564 2e63 6f6e  st.triggered.con
+00001a90: 6e65 6374 2873 656c 662e 6e65 775f 636f  nect(self.new_co
+00001aa0: 6e74 6573 745f 6469 616c 6f67 290a 2020  ntest_dialog).  
+00001ab0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001ac0: 6e4f 7065 6e5f 436f 6e74 6573 742e 7472  nOpen_Contest.tr
+00001ad0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001ae0: 7365 6c66 2e6f 7065 6e5f 636f 6e74 6573  self.open_contes
+00001af0: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00001b00: 6163 7469 6f6e 4564 6974 5f43 7572 7265  actionEdit_Curre
+00001b10: 6e74 5f43 6f6e 7465 7374 2e74 7269 6767  nt_Contest.trigg
+00001b20: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
+00001b30: 662e 6564 6974 5f63 6f6e 7465 7374 290a  f.edit_contest).
+00001b40: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+00001b50: 7469 6f6e 4e65 775f 4461 7461 6261 7365  tionNew_Database
+00001b60: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
+00001b70: 6374 2873 656c 662e 6e65 775f 6461 7461  ct(self.new_data
+00001b80: 6261 7365 290a 2020 2020 2020 2020 7365  base).        se
+00001b90: 6c66 2e61 6374 696f 6e4f 7065 6e5f 4461  lf.actionOpen_Da
+00001ba0: 7461 6261 7365 2e74 7269 6767 6572 6564  tabase.triggered
+00001bb0: 2e63 6f6e 6e65 6374 2873 656c 662e 6f70  .connect(self.op
+00001bc0: 656e 5f64 6174 6162 6173 6529 0a0a 2020  en_database)..  
+00001bd0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001be0: 6e45 6469 745f 4d61 6372 6f73 2e74 7269  nEdit_Macros.tri
+00001bf0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+00001c00: 656c 662e 6564 6974 5f63 775f 6d61 6372  elf.edit_cw_macr
+00001c10: 6f73 290a 0a20 2020 2020 2020 2073 656c  os)..        sel
+00001c20: 662e 6163 7469 6f6e 4162 6f75 742e 7472  f.actionAbout.tr
+00001c30: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001c40: 7365 6c66 2e73 686f 775f 6162 6f75 745f  self.show_about_
+00001c50: 6469 616c 6f67 290a 0a20 2020 2020 2020  dialog)..       
+00001c60: 2073 656c 662e 7261 6469 6f42 7574 746f   self.radioButto
+00001c70: 6e5f 7275 6e2e 636c 6963 6b65 642e 636f  n_run.clicked.co
+00001c80: 6e6e 6563 7428 7365 6c66 2e72 756e 5f73  nnect(self.run_s
+00001c90: 705f 6275 7474 6f6e 735f 636c 6963 6b65  p_buttons_clicke
+00001ca0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00001cb0: 7261 6469 6f42 7574 746f 6e5f 7370 2e63  radioButton_sp.c
+00001cc0: 6c69 636b 6564 2e63 6f6e 6e65 6374 2873  licked.connect(s
+00001cd0: 656c 662e 7275 6e5f 7370 5f62 7574 746f  elf.run_sp_butto
+00001ce0: 6e73 5f63 6c69 636b 6564 290a 2020 2020  ns_clicked).    
+00001cf0: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
+00001d00: 6574 5465 7874 2822 3022 290a 2020 2020  etText("0").    
+00001d10: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00001d20: 6e2e 7465 7874 4564 6974 6564 2e63 6f6e  n.textEdited.con
+00001d30: 6e65 6374 2873 656c 662e 6361 6c6c 7369  nect(self.callsi
+00001d40: 676e 5f63 6861 6e67 6564 290a 2020 2020  gn_changed).    
+00001d50: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00001d60: 6e2e 7265 7475 726e 5072 6573 7365 642e  n.returnPressed.
+00001d70: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+00001d80: 655f 636f 6e74 6163 7429 0a20 2020 2020  e_contact).     
+00001d90: 2020 2073 656c 662e 7365 6e74 2e72 6574     self.sent.ret
+00001da0: 7572 6e50 7265 7373 6564 2e63 6f6e 6e65  urnPressed.conne
+00001db0: 6374 2873 656c 662e 7361 7665 5f63 6f6e  ct(self.save_con
+00001dc0: 7461 6374 290a 2020 2020 2020 2020 7365  tact).        se
+00001dd0: 6c66 2e72 6563 6569 7665 2e72 6574 7572  lf.receive.retur
+00001de0: 6e50 7265 7373 6564 2e63 6f6e 6e65 6374  nPressed.connect
+00001df0: 2873 656c 662e 7361 7665 5f63 6f6e 7461  (self.save_conta
+00001e00: 6374 290a 2020 2020 2020 2020 7365 6c66  ct).        self
+00001e10: 2e6f 7468 6572 5f31 2e72 6574 7572 6e50  .other_1.returnP
+00001e20: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
+00001e30: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
+00001e40: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
+00001e50: 7468 6572 5f32 2e72 6574 7572 6e50 7265  ther_2.returnPre
+00001e60: 7373 6564 2e63 6f6e 6e65 6374 2873 656c  ssed.connect(sel
+00001e70: 662e 7361 7665 5f63 6f6e 7461 6374 290a  f.save_contact).
+00001e80: 2020 2020 2020 2020 7365 6c66 2e6f 7468          self.oth
+00001e90: 6572 5f32 2e74 6578 7445 6469 7465 642e  er_2.textEdited.
+00001ea0: 636f 6e6e 6563 7428 7365 6c66 2e6f 7468  connect(self.oth
+00001eb0: 6572 5f32 5f63 6861 6e67 6564 290a 2020  er_2_changed).  
+00001ec0: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
+00001ed0: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
+00001ee0: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
+00001ef0: 7665 2e73 6574 5465 7874 2822 3539 2229  ve.setText("59")
+00001f00: 0a20 2020 2020 2020 2069 636f 6e5f 7061  .        icon_pa
+00001f10: 7468 203d 2057 4f52 4b49 4e47 5f50 4154  th = WORKING_PAT
+00001f20: 4820 2b20 222f 6461 7461 2f22 0a20 2020  H + "/data/".   
+00001f30: 2020 2020 2073 656c 662e 6772 6565 6e64       self.greend
+00001f40: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
+00001f50: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
+00001f60: 6772 6565 6e64 6f74 2e70 6e67 2229 0a20  greendot.png"). 
+00001f70: 2020 2020 2020 2073 656c 662e 7265 6464         self.redd
+00001f80: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
+00001f90: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
+00001fa0: 7265 6464 6f74 2e70 6e67 2229 0a20 2020  reddot.png").   
+00001fb0: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
+00001fc0: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
+00001fd0: 2e67 7265 656e 646f 7429 0a20 2020 2020  .greendot).     
+00001fe0: 2020 2073 656c 662e 7269 6768 7464 6f74     self.rightdot
+00001ff0: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
+00002000: 7265 6464 6f74 290a 0a20 2020 2020 2020  reddot)..       
+00002010: 2073 656c 662e 4631 2e73 6574 436f 6e74   self.F1.setCont
+00002020: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002030: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002040: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002050: 2020 2073 656c 662e 4631 2e63 7573 746f     self.F1.custo
+00002060: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002070: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002080: 6c66 2e65 6469 745f 4631 290a 2020 2020  lf.edit_F1).    
+00002090: 2020 2020 7365 6c66 2e46 312e 636c 6963      self.F1.clic
+000020a0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+000020b0: 2e73 656e 6466 3129 0a20 2020 2020 2020  .sendf1).       
+000020c0: 2073 656c 662e 4632 2e73 6574 436f 6e74   self.F2.setCont
+000020d0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+000020e0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+000020f0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002100: 2020 2073 656c 662e 4632 2e63 7573 746f     self.F2.custo
+00002110: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002120: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002130: 6c66 2e65 6469 745f 4632 290a 2020 2020  lf.edit_F2).    
+00002140: 2020 2020 7365 6c66 2e46 322e 636c 6963      self.F2.clic
+00002150: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002160: 2e73 656e 6466 3229 0a20 2020 2020 2020  .sendf2).       
+00002170: 2073 656c 662e 4633 2e73 6574 436f 6e74   self.F3.setCont
+00002180: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002190: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+000021a0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+000021b0: 2020 2073 656c 662e 4633 2e63 7573 746f     self.F3.custo
+000021c0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+000021d0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+000021e0: 6c66 2e65 6469 745f 4633 290a 2020 2020  lf.edit_F3).    
+000021f0: 2020 2020 7365 6c66 2e46 332e 636c 6963      self.F3.clic
+00002200: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002210: 2e73 656e 6466 3329 0a20 2020 2020 2020  .sendf3).       
+00002220: 2073 656c 662e 4634 2e73 6574 436f 6e74   self.F4.setCont
+00002230: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002240: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002250: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002260: 2020 2073 656c 662e 4634 2e63 7573 746f     self.F4.custo
+00002270: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002280: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002290: 6c66 2e65 6469 745f 4634 290a 2020 2020  lf.edit_F4).    
+000022a0: 2020 2020 7365 6c66 2e46 342e 636c 6963      self.F4.clic
+000022b0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+000022c0: 2e73 656e 6466 3429 0a20 2020 2020 2020  .sendf4).       
+000022d0: 2073 656c 662e 4635 2e73 6574 436f 6e74   self.F5.setCont
+000022e0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+000022f0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002300: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002310: 2020 2073 656c 662e 4635 2e63 7573 746f     self.F5.custo
+00002320: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002330: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002340: 6c66 2e65 6469 745f 4635 290a 2020 2020  lf.edit_F5).    
+00002350: 2020 2020 7365 6c66 2e46 352e 636c 6963      self.F5.clic
+00002360: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002370: 2e73 656e 6466 3529 0a20 2020 2020 2020  .sendf5).       
+00002380: 2073 656c 662e 4636 2e73 6574 436f 6e74   self.F6.setCont
+00002390: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+000023a0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+000023b0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+000023c0: 2020 2073 656c 662e 4636 2e63 7573 746f     self.F6.custo
+000023d0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+000023e0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+000023f0: 6c66 2e65 6469 745f 4636 290a 2020 2020  lf.edit_F6).    
+00002400: 2020 2020 7365 6c66 2e46 362e 636c 6963      self.F6.clic
+00002410: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002420: 2e73 656e 6466 3629 0a20 2020 2020 2020  .sendf6).       
+00002430: 2073 656c 662e 4637 2e73 6574 436f 6e74   self.F7.setCont
+00002440: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002450: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002460: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002470: 2020 2073 656c 662e 4637 2e63 7573 746f     self.F7.custo
+00002480: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002490: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+000024a0: 6c66 2e65 6469 745f 4637 290a 2020 2020  lf.edit_F7).    
+000024b0: 2020 2020 7365 6c66 2e46 372e 636c 6963      self.F7.clic
+000024c0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+000024d0: 2e73 656e 6466 3729 0a20 2020 2020 2020  .sendf7).       
+000024e0: 2073 656c 662e 4638 2e73 6574 436f 6e74   self.F8.setCont
+000024f0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002500: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002510: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002520: 2020 2073 656c 662e 4638 2e63 7573 746f     self.F8.custo
+00002530: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002540: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002550: 6c66 2e65 6469 745f 4638 290a 2020 2020  lf.edit_F8).    
+00002560: 2020 2020 7365 6c66 2e46 382e 636c 6963      self.F8.clic
+00002570: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002580: 2e73 656e 6466 3829 0a20 2020 2020 2020  .sendf8).       
+00002590: 2073 656c 662e 4639 2e73 6574 436f 6e74   self.F9.setCont
+000025a0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+000025b0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+000025c0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+000025d0: 2020 2073 656c 662e 4639 2e63 7573 746f     self.F9.custo
+000025e0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+000025f0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002600: 6c66 2e65 6469 745f 4639 290a 2020 2020  lf.edit_F9).    
+00002610: 2020 2020 7365 6c66 2e46 392e 636c 6963      self.F9.clic
+00002620: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002630: 2e73 656e 6466 3929 0a20 2020 2020 2020  .sendf9).       
+00002640: 2073 656c 662e 4631 302e 7365 7443 6f6e   self.F10.setCon
+00002650: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002660: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+00002670: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+00002680: 2020 2020 7365 6c66 2e46 3130 2e63 7573      self.F10.cus
+00002690: 746f 6d43 6f6e 7465 7874 4d65 6e75 5265  tomContextMenuRe
+000026a0: 7175 6573 7465 642e 636f 6e6e 6563 7428  quested.connect(
+000026b0: 7365 6c66 2e65 6469 745f 4631 3029 0a20  self.edit_F10). 
+000026c0: 2020 2020 2020 2073 656c 662e 4631 302e         self.F10.
+000026d0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
+000026e0: 7365 6c66 2e73 656e 6466 3130 290a 2020  self.sendf10).  
+000026f0: 2020 2020 2020 7365 6c66 2e46 3131 2e73        self.F11.s
+00002700: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
+00002710: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
+00002720: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
+00002730: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
+00002740: 312e 6375 7374 6f6d 436f 6e74 6578 744d  1.customContextM
+00002750: 656e 7552 6571 7565 7374 6564 2e63 6f6e  enuRequested.con
+00002760: 6e65 6374 2873 656c 662e 6564 6974 5f46  nect(self.edit_F
+00002770: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
+00002780: 2e46 3131 2e63 6c69 636b 6564 2e63 6f6e  .F11.clicked.con
+00002790: 6e65 6374 2873 656c 662e 7365 6e64 6631  nect(self.sendf1
+000027a0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+000027b0: 4631 322e 7365 7443 6f6e 7465 7874 4d65  F12.setContextMe
+000027c0: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
+000027d0: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
+000027e0: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
+000027f0: 6c66 2e46 3132 2e63 7573 746f 6d43 6f6e  lf.F12.customCon
+00002800: 7465 7874 4d65 6e75 5265 7175 6573 7465  textMenuRequeste
+00002810: 642e 636f 6e6e 6563 7428 7365 6c66 2e65  d.connect(self.e
+00002820: 6469 745f 4631 3229 0a20 2020 2020 2020  dit_F12).       
+00002830: 2073 656c 662e 4631 322e 636c 6963 6b65   self.F12.clicke
+00002840: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
+00002850: 656e 6466 3132 290a 0a20 2020 2020 2020  endf12)..       
+00002860: 2073 656c 662e 7265 6164 7072 6566 6572   self.readprefer
+00002870: 656e 6365 7328 290a 2020 2020 2020 2020  ences().        
+00002880: 7365 6c66 2e64 626e 616d 6520 3d20 4441  self.dbname = DA
+00002890: 5441 5f50 4154 4820 2b20 222f 2220 2b20  TA_PATH + "/" + 
+000028a0: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+000028b0: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
+000028c0: 2c20 2268 616d 2e64 6222 290a 2020 2020  , "ham.db").    
+000028d0: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+000028e0: 6520 3d20 4461 7461 4261 7365 2873 656c  e = DataBase(sel
+000028f0: 662e 6462 6e61 6d65 2c20 574f 524b 494e  f.dbname, WORKIN
+00002900: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
+00002910: 7365 6c66 2e73 7461 7469 6f6e 203d 2073  self.station = s
+00002920: 656c 662e 6461 7461 6261 7365 2e66 6574  elf.database.fet
+00002930: 6368 5f73 7461 7469 6f6e 2829 0a20 2020  ch_station().   
+00002940: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+00002950: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+00002960: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00002970: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
+00002980: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+00002990: 745f 7374 6174 696f 6e5f 7365 7474 696e  t_station_settin
+000029a0: 6773 2829 0a20 2020 2020 2020 2020 2020  gs().           
+000029b0: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+000029c0: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
+000029d0: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
+000029e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000029f0: 662e 7374 6174 696f 6e20 6973 204e 6f6e  f.station is Non
+00002a00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00002a10: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
+00002a20: 3d20 7b7d 0a20 2020 2020 2020 2073 656c  = {}.        sel
+00002a30: 662e 636f 6e74 6163 7420 3d20 7365 6c66  f.contact = self
+00002a40: 2e64 6174 6162 6173 652e 656d 7074 795f  .database.empty_
+00002a50: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
+00002a60: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
+00002a70: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
+00002a80: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
+00002a90: 2020 2020 2020 2073 656c 662e 6d61 6b65         self.make
+00002aa0: 5f6f 705f 6469 7228 290a 2020 2020 2020  _op_dir().      
+00002ab0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+00002ac0: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
+00002ad0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002ae0: 6c6f 6164 5f63 6f6e 7465 7374 2829 0a0a  load_contest()..
+00002af0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
+00002b00: 645f 6377 5f6d 6163 726f 7328 290a 2020  d_cw_macros().  
+00002b10: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
+00002b20: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
+00002b30: 2023 2073 656c 662e 6c61 756e 6368 5f6c   # self.launch_l
+00002b40: 6f67 5f77 696e 646f 7728 290a 0a20 2020  og_window()..   
+00002b50: 2020 2020 2073 656c 662e 6261 6e64 5f69       self.band_i
+00002b60: 6e64 6963 6174 6f72 735f 6377 203d 207b  ndicators_cw = {
+00002b70: 0a20 2020 2020 2020 2020 2020 2022 3136  .            "16
+00002b80: 3022 3a20 7365 6c66 2e63 775f 6261 6e64  0": self.cw_band
+00002b90: 5f31 3630 2c0a 2020 2020 2020 2020 2020  _160,.          
+00002ba0: 2020 2238 3022 3a20 7365 6c66 2e63 775f    "80": self.cw_
+00002bb0: 6261 6e64 5f38 302c 0a20 2020 2020 2020  band_80,.       
+00002bc0: 2020 2020 2022 3430 223a 2073 656c 662e       "40": self.
+00002bd0: 6377 5f62 616e 645f 3430 2c0a 2020 2020  cw_band_40,.    
+00002be0: 2020 2020 2020 2020 2232 3022 3a20 7365          "20": se
+00002bf0: 6c66 2e63 775f 6261 6e64 5f32 302c 0a20  lf.cw_band_20,. 
+00002c00: 2020 2020 2020 2020 2020 2022 3135 223a             "15":
+00002c10: 2073 656c 662e 6377 5f62 616e 645f 3135   self.cw_band_15
+00002c20: 2c0a 2020 2020 2020 2020 2020 2020 2231  ,.            "1
+00002c30: 3022 3a20 7365 6c66 2e63 775f 6261 6e64  0": self.cw_band
+00002c40: 5f31 302c 0a20 2020 2020 2020 207d 0a0a  _10,.        }..
+00002c50: 2020 2020 2020 2020 7365 6c66 2e62 616e          self.ban
+00002c60: 645f 696e 6469 6361 746f 7273 5f73 7362  d_indicators_ssb
+00002c70: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+00002c80: 2022 3136 3022 3a20 7365 6c66 2e73 7362   "160": self.ssb
+00002c90: 5f62 616e 645f 3136 302c 0a20 2020 2020  _band_160,.     
+00002ca0: 2020 2020 2020 2022 3830 223a 2073 656c         "80": sel
+00002cb0: 662e 7373 625f 6261 6e64 5f38 302c 0a20  f.ssb_band_80,. 
+00002cc0: 2020 2020 2020 2020 2020 2022 3430 223a             "40":
+00002cd0: 2073 656c 662e 7373 625f 6261 6e64 5f34   self.ssb_band_4
+00002ce0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00002cf0: 3230 223a 2073 656c 662e 7373 625f 6261  20": self.ssb_ba
+00002d00: 6e64 5f32 302c 0a20 2020 2020 2020 2020  nd_20,.         
+00002d10: 2020 2022 3135 223a 2073 656c 662e 7373     "15": self.ss
+00002d20: 625f 6261 6e64 5f31 352c 0a20 2020 2020  b_band_15,.     
+00002d30: 2020 2020 2020 2022 3130 223a 2073 656c         "10": sel
+00002d40: 662e 7373 625f 6261 6e64 5f31 302c 0a20  f.ssb_band_10,. 
+00002d50: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+00002d60: 2020 7365 6c66 2e62 616e 645f 696e 6469    self.band_indi
+00002d70: 6361 746f 7273 5f72 7474 7920 3d20 7b0a  cators_rtty = {.
+00002d80: 2020 2020 2020 2020 2020 2020 2231 3630              "160
+00002d90: 223a 2073 656c 662e 7274 7479 5f62 616e  ": self.rtty_ban
+00002da0: 645f 3136 302c 0a20 2020 2020 2020 2020  d_160,.         
+00002db0: 2020 2022 3830 223a 2073 656c 662e 7274     "80": self.rt
+00002dc0: 7479 5f62 616e 645f 3830 2c0a 2020 2020  ty_band_80,.    
+00002dd0: 2020 2020 2020 2020 2234 3022 3a20 7365          "40": se
+00002de0: 6c66 2e72 7474 795f 6261 6e64 5f34 302c  lf.rtty_band_40,
+00002df0: 0a20 2020 2020 2020 2020 2020 2022 3230  .            "20
+00002e00: 223a 2073 656c 662e 7274 7479 5f62 616e  ": self.rtty_ban
+00002e10: 645f 3230 2c0a 2020 2020 2020 2020 2020  d_20,.          
+00002e20: 2020 2231 3522 3a20 7365 6c66 2e72 7474    "15": self.rtt
+00002e30: 795f 6261 6e64 5f31 352c 0a20 2020 2020  y_band_15,.     
+00002e40: 2020 2020 2020 2022 3130 223a 2073 656c         "10": sel
+00002e50: 662e 7274 7479 5f62 616e 645f 3130 2c0a  f.rtty_band_10,.
+00002e60: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00002e70: 2020 2073 656c 662e 616c 6c5f 6d6f 6465     self.all_mode
+00002e80: 5f69 6e64 6963 6174 6f72 7320 3d20 7b0a  _indicators = {.
+00002e90: 2020 2020 2020 2020 2020 2020 2243 5722              "CW"
+00002ea0: 3a20 7365 6c66 2e62 616e 645f 696e 6469  : self.band_indi
+00002eb0: 6361 746f 7273 5f63 772c 0a20 2020 2020  cators_cw,.     
+00002ec0: 2020 2020 2020 2022 5353 4222 3a20 7365         "SSB": se
+00002ed0: 6c66 2e62 616e 645f 696e 6469 6361 746f  lf.band_indicato
+00002ee0: 7273 5f73 7362 2c0a 2020 2020 2020 2020  rs_ssb,.        
+00002ef0: 2020 2020 2252 5454 5922 3a20 7365 6c66      "RTTY": self
+00002f00: 2e62 616e 645f 696e 6469 6361 746f 7273  .band_indicators
+00002f10: 5f72 7474 792c 0a20 2020 2020 2020 207d  _rtty,.        }
+00002f20: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00002f30: 2e5f 7564 7077 6174 6368 2069 7320 4e6f  ._udpwatch is No
+00002f40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00002f50: 7365 6c66 2e5f 7564 7077 6174 6368 203d  self._udpwatch =
+00002f60: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
+00002f70: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00002f80: 2020 2074 6172 6765 743d 7365 6c66 2e77     target=self.w
+00002f90: 6174 6368 5f75 6470 2c0a 2020 2020 2020  atch_udp,.      
+00002fa0: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
+00002fb0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00002fc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00002fd0: 2073 656c 662e 5f75 6470 7761 7463 682e   self._udpwatch.
+00002fe0: 7374 6172 7428 290a 0a20 2020 2040 7374  start()..    @st
+00002ff0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00003000: 6566 2063 6865 636b 5f70 726f 6365 7373  ef check_process
+00003010: 286e 616d 653a 2073 7472 2920 2d3e 2062  (name: str) -> b
+00003020: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+00003030: 6368 6563 6b73 2074 6f20 7365 6520 6966  checks to see if
+00003040: 2070 726f 6772 616d 206f 6620 6e61 6d65   program of name
+00003050: 2069 7320 696e 2074 6865 2061 6374 6976   is in the activ
+00003060: 6520 7072 6f63 6573 7320 6c69 7374 2222  e process list""
+00003070: 220a 2020 2020 2020 2020 666f 7220 7072  ".        for pr
+00003080: 6f63 2069 6e20 7073 7574 696c 2e70 726f  oc in psutil.pro
+00003090: 6365 7373 5f69 7465 7228 293a 0a20 2020  cess_iter():.   
+000030a0: 2020 2020 2020 2020 2069 6620 626f 6f6c           if bool
+000030b0: 2872 652e 6d61 7463 6828 6e61 6d65 2c20  (re.match(name, 
+000030c0: 7072 6f63 2e6e 616d 6528 292e 6c6f 7765  proc.name().lowe
+000030d0: 7228 2929 293a 0a20 2020 2020 2020 2020  r())):.         
+000030e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000030f0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00003100: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00003110: 2073 686f 775f 6d65 7373 6167 655f 626f   show_message_bo
+00003120: 7828 7365 6c66 2c20 6d65 7373 6167 653a  x(self, message:
+00003130: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
+00003140: 2020 2020 2020 2022 2222 646f 6322 2222         """doc"""
+00003150: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+00003160: 5f62 6f78 203d 2051 7457 6964 6765 7473  _box = QtWidgets
+00003170: 2e51 4d65 7373 6167 6542 6f78 2829 0a20  .QMessageBox(). 
+00003180: 2020 2020 2020 206d 6573 7361 6765 5f62         message_b
+00003190: 6f78 2e73 6574 4963 6f6e 2851 7457 6964  ox.setIcon(QtWid
+000031a0: 6765 7473 2e51 4d65 7373 6167 6542 6f78  gets.QMessageBox
+000031b0: 2e49 6e66 6f72 6d61 7469 6f6e 290a 2020  .Information).  
+000031c0: 2020 2020 2020 6d65 7373 6167 655f 626f        message_bo
+000031d0: 782e 7365 7454 6578 7428 6d65 7373 6167  x.setText(messag
+000031e0: 6529 0a20 2020 2020 2020 206d 6573 7361  e).        messa
+000031f0: 6765 5f62 6f78 2e73 6574 5769 6e64 6f77  ge_box.setWindow
+00003200: 5469 746c 6528 2249 6e66 6f72 6d61 7469  Title("Informati
+00003210: 6f6e 2229 0a20 2020 2020 2020 206d 6573  on").        mes
+00003220: 7361 6765 5f62 6f78 2e73 6574 5374 616e  sage_box.setStan
+00003230: 6461 7264 4275 7474 6f6e 7328 5174 5769  dardButtons(QtWi
+00003240: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
+00003250: 782e 4f6b 290a 2020 2020 2020 2020 5f20  x.Ok).        _ 
+00003260: 3d20 6d65 7373 6167 655f 626f 782e 6578  = message_box.ex
+00003270: 6563 5f28 290a 0a20 2020 2064 6566 2073  ec_()..    def s
+00003280: 686f 775f 6162 6f75 745f 6469 616c 6f67  how_about_dialog
+00003290: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000032a0: 2222 2253 686f 7720 6162 6f75 7420 6469  """Show about di
+000032b0: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
+000032c0: 7365 6c66 2e61 626f 7574 5f64 6961 6c6f  self.about_dialo
+000032d0: 6720 3d20 4162 6f75 7428 574f 524b 494e  g = About(WORKIN
+000032e0: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
+000032f0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+00003300: 2822 6461 726b 5f6d 6f64 6522 293a 0a20  ("dark_mode"):. 
+00003310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003320: 6162 6f75 745f 6469 616c 6f67 2e73 6574  about_dialog.set
+00003330: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
+00003340: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
+00003350: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
+00003360: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
+00003370: 2020 6465 6620 6564 6974 5f63 6f6e 6669    def edit_confi
+00003380: 6775 7261 7469 6f6e 5f73 6574 7469 6e67  guration_setting
+00003390: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+000033a0: 2022 2222 436f 6e66 6967 7572 6174 696f   """Configuratio
+000033b0: 6e20 5365 7474 696e 6773 2077 6173 2063  n Settings was c
+000033c0: 6c69 636b 6564 2222 220a 2020 2020 2020  licked""".      
+000033d0: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
+000033e0: 7469 6f6e 5f64 6961 6c6f 6720 3d20 5365  tion_dialog = Se
+000033f0: 7474 696e 6773 2857 4f52 4b49 4e47 5f50  ttings(WORKING_P
+00003400: 4154 482c 2043 4f4e 4649 475f 5041 5448  ATH, CONFIG_PATH
+00003410: 2c20 7365 6c66 2e70 7265 6629 0a20 2020  , self.pref).   
+00003420: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
+00003430: 7572 6174 696f 6e5f 6469 616c 6f67 2e75  uration_dialog.u
+00003440: 7365 6861 6d64 625f 7261 6469 6f42 7574  sehamdb_radioBut
+00003450: 746f 6e2e 6869 6465 2829 0a20 2020 2020  ton.hide().     
+00003460: 2020 2023 2073 656c 662e 636f 6e66 6967     # self.config
+00003470: 7572 6174 696f 6e5f 6469 616c 6f67 2e6e  uration_dialog.n
+00003480: 316d 6d5f 7461 622e 6869 6465 2829 0a20  1mm_tab.hide(). 
+00003490: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
+000034a0: 6967 7572 6174 696f 6e5f 6469 616c 6f67  iguration_dialog
+000034b0: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+000034c0: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
+000034d0: 6f6e 5f64 6961 6c6f 672e 6163 6365 7074  on_dialog.accept
+000034e0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+000034f0: 6564 6974 5f63 6f6e 6669 6775 7261 7469  edit_configurati
+00003500: 6f6e 5f72 6574 7572 6e29 0a0a 2020 2020  on_return)..    
+00003510: 6465 6620 6564 6974 5f63 6f6e 6669 6775  def edit_configu
+00003520: 7261 7469 6f6e 5f72 6574 7572 6e28 7365  ration_return(se
+00003530: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00003540: 5265 7475 726e 7320 6865 7265 2077 6865  Returns here whe
+00003550: 6e20 636f 6e66 6967 7572 6174 696f 6e20  n configuration 
+00003560: 6469 616c 6f67 2063 6c6f 7365 6420 7769  dialog closed wi
+00003570: 7468 206f 6b61 792e 2222 220a 2020 2020  th okay.""".    
+00003580: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
+00003590: 7261 7469 6f6e 5f64 6961 6c6f 672e 7361  ration_dialog.sa
+000035a0: 7665 5f63 6861 6e67 6573 2829 0a20 2020  ve_changes().   
+000035b0: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
+000035c0: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
+000035d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+000035e0: 6728 2225 7322 2c20 6622 7b73 656c 662e  g("%s", f"{self.
+000035f0: 7072 6566 7d22 290a 2020 2020 2020 2020  pref}").        
+00003600: 7365 6c66 2e72 6561 6470 7265 6665 7265  self.readprefere
+00003610: 6e63 6573 2829 0a0a 2020 2020 6465 6620  nces()..    def 
+00003620: 6e65 775f 6461 7461 6261 7365 2873 656c  new_database(sel
+00003630: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+00003640: 7265 6174 6520 6e65 7720 6461 7461 6261  reate new databa
+00003650: 7365 2e22 2222 0a20 2020 2020 2020 2066  se.""".        f
+00003660: 696c 656e 616d 6520 3d20 7365 6c66 2e66  ilename = self.f
+00003670: 696c 6570 6963 6b65 7228 226e 6577 2229  ilepicker("new")
+00003680: 0a20 2020 2020 2020 2069 6620 6669 6c65  .        if file
+00003690: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
+000036a0: 2020 6966 2066 696c 656e 616d 655b 2d33    if filename[-3
+000036b0: 3a5d 2021 3d20 222e 6462 223a 0a20 2020  :] != ".db":.   
+000036c0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+000036d0: 656e 616d 6520 2b3d 2022 2e64 6222 0a20  ename += ".db". 
+000036e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000036f0: 7072 6566 5b22 6375 7272 656e 745f 6461  pref["current_da
+00003700: 7461 6261 7365 225d 203d 2066 696c 656e  tabase"] = filen
+00003710: 616d 652e 7370 6c69 7428 222f 2229 5b2d  ame.split("/")[-
+00003720: 313a 5d5b 305d 0a20 2020 2020 2020 2020  1:][0].         
+00003730: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
+00003740: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
+00003750: 2020 2020 2020 2073 656c 662e 6462 6e61         self.dbna
+00003760: 6d65 203d 2044 4154 415f 5041 5448 202b  me = DATA_PATH +
+00003770: 2022 2f22 202b 2073 656c 662e 7072 6566   "/" + self.pref
+00003780: 2e67 6574 2822 6375 7272 656e 745f 6461  .get("current_da
+00003790: 7461 6261 7365 222c 2022 6861 6d2e 6462  tabase", "ham.db
+000037a0: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+000037b0: 656c 662e 6461 7461 6261 7365 203d 2044  elf.database = D
+000037c0: 6174 6142 6173 6528 7365 6c66 2e64 626e  ataBase(self.dbn
+000037d0: 616d 652c 2057 4f52 4b49 4e47 5f50 4154  ame, WORKING_PAT
+000037e0: 4829 0a20 2020 2020 2020 2020 2020 2073  H).            s
+000037f0: 656c 662e 636f 6e74 6163 7420 3d20 7365  elf.contact = se
+00003800: 6c66 2e64 6174 6162 6173 652e 656d 7074  lf.database.empt
+00003810: 795f 636f 6e74 6163 740a 2020 2020 2020  y_contact.      
+00003820: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+00003830: 6f6e 203d 2073 656c 662e 6461 7461 6261  on = self.databa
+00003840: 7365 2e66 6574 6368 5f73 7461 7469 6f6e  se.fetch_station
+00003850: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+00003860: 6620 7365 6c66 2e73 7461 7469 6f6e 2069  f self.station i
+00003870: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00003880: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00003890: 7469 6f6e 203d 207b 7d0a 2020 2020 2020  tion = {}.      
+000038a0: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
+000038b0: 6e74 5f6f 7020 3d20 7365 6c66 2e73 7461  nt_op = self.sta
+000038c0: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
+000038d0: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+000038e0: 2073 656c 662e 6d61 6b65 5f6f 705f 6469   self.make_op_di
+000038f0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+00003900: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00003910: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00003920: 3d20 224e 4557 4442 220a 2020 2020 2020  = "NEWDB".      
+00003930: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
+00003940: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
+00003950: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+00003960: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
+00003970: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
+00003980: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
+00003990: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000039a0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+000039b0: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
+000039c0: 6974 5f73 7461 7469 6f6e 5f73 6574 7469  it_station_setti
+000039d0: 6e67 7328 290a 0a20 2020 2064 6566 206f  ngs()..    def o
+000039e0: 7065 6e5f 6461 7461 6261 7365 2873 656c  pen_database(sel
+000039f0: 6629 3a0a 2020 2020 2020 2020 2222 224f  f):.        """O
+00003a00: 7065 6e20 6578 6973 7469 6e67 2064 6174  pen existing dat
+00003a10: 6162 6173 652e 2222 220a 2020 2020 2020  abase.""".      
+00003a20: 2020 6669 6c65 6e61 6d65 203d 2073 656c    filename = sel
+00003a30: 662e 6669 6c65 7069 636b 6572 2822 6f70  f.filepicker("op
+00003a40: 656e 2229 0a20 2020 2020 2020 2069 6620  en").        if 
+00003a50: 6669 6c65 6e61 6d65 3a0a 2020 2020 2020  filename:.      
+00003a60: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+00003a70: 2263 7572 7265 6e74 5f64 6174 6162 6173  "current_databas
+00003a80: 6522 5d20 3d20 6669 6c65 6e61 6d65 2e73  e"] = filename.s
+00003a90: 706c 6974 2822 2f22 295b 2d31 3a5d 5b30  plit("/")[-1:][0
+00003aa0: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
+00003ab0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+00003ac0: 6e63 6528 290a 2020 2020 2020 2020 2020  nce().          
+00003ad0: 2020 7365 6c66 2e64 626e 616d 6520 3d20    self.dbname = 
+00003ae0: 4441 5441 5f50 4154 4820 2b20 222f 2220  DATA_PATH + "/" 
+00003af0: 2b20 7365 6c66 2e70 7265 662e 6765 7428  + self.pref.get(
+00003b00: 2263 7572 7265 6e74 5f64 6174 6162 6173  "current_databas
+00003b10: 6522 2c20 2268 616d 2e64 6222 290a 2020  e", "ham.db").  
+00003b20: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00003b30: 6174 6162 6173 6520 3d20 4461 7461 4261  atabase = DataBa
+00003b40: 7365 2873 656c 662e 6462 6e61 6d65 2c20  se(self.dbname, 
+00003b50: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
+00003b60: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003b70: 6f6e 7461 6374 203d 2073 656c 662e 6461  ontact = self.da
+00003b80: 7461 6261 7365 2e65 6d70 7479 5f63 6f6e  tabase.empty_con
+00003b90: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
+00003ba0: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+00003bb0: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
+00003bc0: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
+00003bd0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003be0: 662e 7374 6174 696f 6e20 6973 204e 6f6e  f.station is Non
+00003bf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00003c00: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
+00003c10: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+00003c20: 2069 6620 7365 6c66 2e73 7461 7469 6f6e   if self.station
+00003c30: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
+00003c40: 203d 3d20 2222 3a0a 2020 2020 2020 2020   == "":.        
+00003c50: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+00003c60: 745f 7374 6174 696f 6e5f 7365 7474 696e  t_station_settin
+00003c70: 6773 2829 0a20 2020 2020 2020 2020 2020  gs().           
+00003c80: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+00003c90: 203d 2073 656c 662e 7374 6174 696f 6e2e   = self.station.
+00003ca0: 6765 7428 2243 616c 6c22 2c20 2222 290a  get("Call", "").
+00003cb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003cc0: 2e6d 616b 655f 6f70 5f64 6972 2829 0a20  .make_op_dir(). 
+00003cd0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00003ce0: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00003cf0: 636d 645b 2263 6d64 225d 203d 2022 4e45  cmd["cmd"] = "NE
+00003d00: 5744 4222 0a20 2020 2020 2020 2020 2020  WDB".           
+00003d10: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
+00003d20: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
+00003d30: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00003d40: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+00003d50: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
+00003d60: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
+00003d70: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
+00003d80: 6e70 7574 7328 290a 0a20 2020 2064 6566  nputs()..    def
+00003d90: 206e 6577 5f63 6f6e 7465 7374 2873 656c   new_contest(sel
+00003da0: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
+00003db0: 7265 6174 6520 6e65 7720 636f 6e74 6573  reate new contes
+00003dc0: 7420 696e 2065 7869 7374 696e 6720 6461  t in existing da
+00003dd0: 7461 6261 7365 2e22 2222 0a0a 2020 2020  tabase."""..    
+00003de0: 6465 6620 6f70 656e 5f63 6f6e 7465 7374  def open_contest
+00003df0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00003e00: 2222 2253 7769 7463 6820 746f 2061 2064  """Switch to a d
+00003e10: 6966 6665 7265 6e74 2065 7869 7374 696e  ifferent existin
+00003e20: 6720 636f 6e74 6573 7420 696e 2065 7869  g contest in exi
+00003e30: 7374 696e 6720 6461 7461 6261 7365 2e22  sting database."
+00003e40: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+00003e50: 722e 6465 6275 6728 224f 7065 6e20 436f  r.debug("Open Co
+00003e60: 6e74 6573 7420 7365 6c65 6374 6564 2229  ntest selected")
+00003e70: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00003e80: 7320 3d20 7365 6c66 2e64 6174 6162 6173  s = self.databas
+00003e90: 652e 6665 7463 685f 616c 6c5f 636f 6e74  e.fetch_all_cont
+00003ea0: 6573 7473 2829 0a20 2020 2020 2020 206c  ests().        l
+00003eb0: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
+00003ec0: 2c20 6622 7b63 6f6e 7465 7374 737d 2229  , f"{contests}")
+00003ed0: 0a0a 2020 2020 2020 2020 6966 2063 6f6e  ..        if con
+00003ee0: 7465 7374 733a 0a20 2020 2020 2020 2020  tests:.         
+00003ef0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00003f00: 6469 616c 6f67 203d 2053 656c 6563 7443  dialog = SelectC
+00003f10: 6f6e 7465 7374 2857 4f52 4b49 4e47 5f50  ontest(WORKING_P
+00003f20: 4154 4829 0a20 2020 2020 2020 2020 2020  ATH).           
+00003f30: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00003f40: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+00003f50: 742e 7365 7452 6f77 436f 756e 7428 3029  t.setRowCount(0)
+00003f60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00003f70: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00003f80: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00003f90: 7443 6f6c 756d 6e43 6f75 6e74 2834 290a  tColumnCount(4).
+00003fa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003fb0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00003fc0: 636f 6e74 6573 745f 6c69 7374 2e76 6572  contest_list.ver
+00003fd0: 7469 6361 6c48 6561 6465 7228 292e 7365  ticalHeader().se
+00003fe0: 7456 6973 6962 6c65 2846 616c 7365 290a  tVisible(False).
+00003ff0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004000: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004010: 636f 6e74 6573 745f 6c69 7374 2e73 6574  contest_list.set
+00004020: 436f 6c75 6d6e 5769 6474 6828 312c 2032  ColumnWidth(1, 2
+00004030: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+00004040: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00004050: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
+00004060: 2e73 6574 436f 6c75 6d6e 5769 6474 6828  .setColumnWidth(
+00004070: 322c 2032 3030 290a 2020 2020 2020 2020  2, 200).        
+00004080: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00004090: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
+000040a0: 6c69 7374 2e73 6574 486f 7269 7a6f 6e74  list.setHorizont
+000040b0: 616c 4865 6164 6572 4974 656d 280a 2020  alHeaderItem(.  
+000040c0: 2020 2020 2020 2020 2020 2020 2020 302c                0,
+000040d0: 2051 7457 6964 6765 7473 2e51 5461 626c   QtWidgets.QTabl
+000040e0: 6557 6964 6765 7449 7465 6d28 2243 6f6e  eWidgetItem("Con
+000040f0: 7465 7374 204e 7222 290a 2020 2020 2020  test Nr").      
+00004100: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004110: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00004120: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
+00004130: 6c69 7374 2e73 6574 486f 7269 7a6f 6e74  list.setHorizont
+00004140: 616c 4865 6164 6572 4974 656d 280a 2020  alHeaderItem(.  
+00004150: 2020 2020 2020 2020 2020 2020 2020 312c                1,
+00004160: 2051 7457 6964 6765 7473 2e51 5461 626c   QtWidgets.QTabl
+00004170: 6557 6964 6765 7449 7465 6d28 2243 6f6e  eWidgetItem("Con
+00004180: 7465 7374 204e 616d 6522 290a 2020 2020  test Name").    
+00004190: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000041a0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+000041b0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
+000041c0: 745f 6c69 7374 2e73 6574 486f 7269 7a6f  t_list.setHorizo
+000041d0: 6e74 616c 4865 6164 6572 4974 656d 280a  ntalHeaderItem(.
+000041e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000041f0: 322c 2051 7457 6964 6765 7473 2e51 5461  2, QtWidgets.QTa
+00004200: 626c 6557 6964 6765 7449 7465 6d28 2243  bleWidgetItem("C
+00004210: 6f6e 7465 7374 2053 7461 7274 2229 0a20  ontest Start"). 
+00004220: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00004230: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004240: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00004250: 7465 7374 5f6c 6973 742e 7365 7448 6f72  test_list.setHor
+00004260: 697a 6f6e 7461 6c48 6561 6465 7249 7465  izontalHeaderIte
+00004270: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
+00004280: 2020 2033 2c20 5174 5769 6467 6574 732e     3, QtWidgets.
+00004290: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
+000042a0: 2822 4e6f 7420 5549 7365 6422 290a 2020  ("Not UIsed").  
+000042b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000042c0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000042d0: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
+000042e0: 6573 745f 6c69 7374 2e73 6574 436f 6c75  est_list.setColu
+000042f0: 6d6e 4869 6464 656e 2830 2c20 5472 7565  mnHidden(0, True
+00004300: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00004310: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004320: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
+00004330: 6574 436f 6c75 6d6e 4869 6464 656e 2833  etColumnHidden(3
+00004340: 2c20 5472 7565 290a 2020 2020 2020 2020  , True).        
+00004350: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00004360: 5f64 6961 6c6f 672e 6163 6365 7074 6564  _dialog.accepted
+00004370: 2e63 6f6e 6e65 6374 2873 656c 662e 6f70  .connect(self.op
+00004380: 656e 5f63 6f6e 7465 7374 5f72 6574 7572  en_contest_retur
+00004390: 6e29 0a20 2020 2020 2020 2020 2020 2066  n).            f
+000043a0: 6f72 2063 6f6e 7465 7374 2069 6e20 636f  or contest in co
+000043b0: 6e74 6573 7473 3a0a 2020 2020 2020 2020  ntests:.        
+000043c0: 2020 2020 2020 2020 6e75 6d62 6572 5f6f          number_o
+000043d0: 665f 726f 7773 203d 2073 656c 662e 636f  f_rows = self.co
+000043e0: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+000043f0: 7465 7374 5f6c 6973 742e 726f 7743 6f75  test_list.rowCou
+00004400: 6e74 2829 0a20 2020 2020 2020 2020 2020  nt().           
+00004410: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00004420: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+00004430: 5f6c 6973 742e 696e 7365 7274 526f 7728  _list.insertRow(
+00004440: 6e75 6d62 6572 5f6f 665f 726f 7773 290a  number_of_rows).
+00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004460: 636f 6e74 6573 745f 6964 203d 2073 7472  contest_id = str
+00004470: 2863 6f6e 7465 7374 2e67 6574 2822 436f  (contest.get("Co
+00004480: 6e74 6573 7449 4422 2c20 3129 290a 2020  ntestID", 1)).  
+00004490: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000044a0: 6e74 6573 745f 6e61 6d65 203d 2063 6f6e  ntest_name = con
+000044b0: 7465 7374 2e67 6574 2822 436f 6e74 6573  test.get("Contes
+000044c0: 744e 616d 6522 2c20 3129 0a20 2020 2020  tName", 1).     
+000044d0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+000044e0: 5f64 6174 6520 3d20 636f 6e74 6573 742e  _date = contest.
+000044f0: 6765 7428 2253 7461 7274 4461 7465 222c  get("StartDate",
+00004500: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+00004510: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00004520: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
+00004530: 6c69 7374 2e73 6574 4974 656d 280a 2020  list.setItem(.  
+00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004550: 2020 6e75 6d62 6572 5f6f 665f 726f 7773    number_of_rows
+00004560: 2c20 302c 2051 7457 6964 6765 7473 2e51  , 0, QtWidgets.Q
+00004570: 5461 626c 6557 6964 6765 7449 7465 6d28  TableWidgetItem(
+00004580: 636f 6e74 6573 745f 6964 290a 2020 2020  contest_id).    
+00004590: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000045a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000045b0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000045c0: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
+000045d0: 6574 4974 656d 280a 2020 2020 2020 2020  etItem(.        
+000045e0: 2020 2020 2020 2020 2020 2020 6e75 6d62              numb
+000045f0: 6572 5f6f 665f 726f 7773 2c20 312c 2051  er_of_rows, 1, Q
+00004600: 7457 6964 6765 7473 2e51 5461 626c 6557  tWidgets.QTableW
+00004610: 6964 6765 7449 7465 6d28 636f 6e74 6573  idgetItem(contes
+00004620: 745f 6e61 6d65 290a 2020 2020 2020 2020  t_name).        
+00004630: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00004640: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00004650: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+00004660: 6e74 6573 745f 6c69 7374 2e73 6574 4974  ntest_list.setIt
+00004670: 656d 280a 2020 2020 2020 2020 2020 2020  em(.            
+00004680: 2020 2020 2020 2020 6e75 6d62 6572 5f6f          number_o
+00004690: 665f 726f 7773 2c20 322c 2051 7457 6964  f_rows, 2, QtWid
+000046a0: 6765 7473 2e51 5461 626c 6557 6964 6765  gets.QTableWidge
+000046b0: 7449 7465 6d28 7374 6172 745f 6461 7465  tItem(start_date
+000046c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000046d0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+000046e0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+000046f0: 7368 6f77 2829 0a0a 2020 2020 6465 6620  show()..    def 
+00004700: 6f70 656e 5f63 6f6e 7465 7374 5f72 6574  open_contest_ret
+00004710: 7572 6e28 7365 6c66 293a 0a20 2020 2020  urn(self):.     
+00004720: 2020 2022 2222 4361 6c6c 6564 2062 7920     """Called by 
+00004730: 6f70 656e 5f63 6f6e 7465 7374 2222 220a  open_contest""".
+00004740: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
+00004750: 5f72 6f77 203d 2073 656c 662e 636f 6e74  _row = self.cont
+00004760: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00004770: 7374 5f6c 6973 742e 6375 7272 656e 7452  st_list.currentR
+00004780: 6f77 2829 0a20 2020 2020 2020 2063 6f6e  ow().        con
+00004790: 7465 7374 203d 2073 656c 662e 636f 6e74  test = self.cont
+000047a0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+000047b0: 7374 5f6c 6973 742e 6974 656d 2873 656c  st_list.item(sel
+000047c0: 6563 7465 645f 726f 772c 2030 292e 7465  ected_row, 0).te
+000047d0: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
+000047e0: 662e 7072 6566 5b22 636f 6e74 6573 7422  f.pref["contest"
+000047f0: 5d20 3d20 636f 6e74 6573 740a 2020 2020  ] = contest.    
+00004800: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
+00004810: 7265 6665 7265 6e63 6528 290a 2020 2020  reference().    
+00004820: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00004830: 2822 5365 6c65 6374 6564 2063 6f6e 7465  ("Selected conte
+00004840: 7374 3a20 2573 222c 2066 227b 636f 6e74  st: %s", f"{cont
+00004850: 6573 747d 2229 0a20 2020 2020 2020 2073  est}").        s
+00004860: 656c 662e 6c6f 6164 5f63 6f6e 7465 7374  elf.load_contest
+00004870: 2829 0a0a 2020 2020 6465 6620 7265 6669  ()..    def refi
+00004880: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00004890: 2c20 7461 7267 6574 2c20 736f 7572 6365  , target, source
+000048a0: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+000048b0: 6669 6c6c 2051 436f 6d62 6f62 6f78 2077  fill QCombobox w
+000048c0: 6964 6765 7420 7769 7468 2076 616c 7565  idget with value
+000048d0: 2e22 2222 0a20 2020 2020 2020 2069 6e64  .""".        ind
+000048e0: 6578 203d 2074 6172 6765 742e 6669 6e64  ex = target.find
+000048f0: 5465 7874 2873 6f75 7263 6529 0a20 2020  Text(source).   
+00004900: 2020 2020 2074 6172 6765 742e 7365 7443       target.setC
+00004910: 7572 7265 6e74 496e 6465 7828 696e 6465  urrentIndex(inde
+00004920: 7829 0a0a 2020 2020 6465 6620 6564 6974  x)..    def edit
+00004930: 5f63 6f6e 7465 7374 2873 656c 6629 3a0a  _contest(self):.
+00004940: 2020 2020 2020 2020 2222 2245 6469 7420          """Edit 
+00004950: 7468 6520 6375 7272 656e 7420 636f 6e74  the current cont
+00004960: 6573 7422 2222 0a20 2020 2020 2020 206c  est""".        l
+00004970: 6f67 6765 722e 6465 6275 6728 2245 6469  ogger.debug("Edi
+00004980: 7420 636f 6e74 6573 7420 4469 616c 6f67  t contest Dialog
+00004990: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+000049a0: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+000049b0: 6e67 7320 6973 204e 6f6e 653a 0a20 2020  ngs is None:.   
+000049c0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000049d0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000049e0: 7465 7374 5f64 6961 6c6f 6720 3d20 4e65  test_dialog = Ne
+000049f0: 7743 6f6e 7465 7374 2857 4f52 4b49 4e47  wContest(WORKING
+00004a00: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
+00004a10: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00004a20: 6f67 2e73 6574 5769 6e64 6f77 5469 746c  og.setWindowTitl
+00004a30: 6528 2245 6469 7420 436f 6e74 6573 7422  e("Edit Contest"
+00004a40: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00004a50: 6f6e 7465 7374 5f64 6961 6c6f 672e 7469  ontest_dialog.ti
+00004a60: 746c 652e 7365 7454 6578 7428 2222 290a  tle.setText("").
+00004a70: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00004a80: 7465 7374 5f64 6961 6c6f 672e 6163 6365  test_dialog.acce
+00004a90: 7074 6564 2e63 6f6e 6e65 6374 2873 656c  pted.connect(sel
+00004aa0: 662e 7361 7665 5f65 6469 7465 645f 636f  f.save_edited_co
+00004ab0: 6e74 6573 7429 0a20 2020 2020 2020 2069  ntest).        i
+00004ac0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+00004ad0: 2264 6172 6b5f 6d6f 6465 2229 3a0a 2020  "dark_mode"):.  
+00004ae0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00004af0: 6f6e 7465 7374 5f64 6961 6c6f 672e 7365  ontest_dialog.se
+00004b00: 7453 7479 6c65 5368 6565 7428 4441 524b  tStyleSheet(DARK
+00004b10: 5f53 5459 4c45 5348 4545 5429 0a0a 2020  _STYLESHEET)..  
+00004b20: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
+00004b30: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+00004b40: 6e67 732e 6765 7428 2243 6f6e 7465 7374  ngs.get("Contest
+00004b50: 4e61 6d65 2229 2e75 7070 6572 2829 2e72  Name").upper().r
+00004b60: 6570 6c61 6365 2822 5f22 2c20 2220 2229  eplace("_", " ")
+00004b70: 0a20 2020 2020 2020 2069 6620 7661 6c75  .        if valu
+00004b80: 6520 3d3d 2022 4745 4e45 5241 4c20 4c4f  e == "GENERAL LO
+00004b90: 4747 494e 4722 3a0a 2020 2020 2020 2020  GGING":.        
+00004ba0: 2020 2020 7661 6c75 6520 3d20 2247 656e      value = "Gen
+00004bb0: 6572 616c 204c 6f67 6769 6e67 220a 2020  eral Logging".  
+00004bc0: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
+00004bd0: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
+00004be0: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
+00004bf0: 6f6e 7465 7374 2c20 7661 6c75 6529 0a20  ontest, value). 
+00004c00: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+00004c10: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00004c20: 696e 6773 2e67 6574 2822 4f70 6572 6174  ings.get("Operat
+00004c30: 6f72 4361 7465 676f 7279 2229 0a20 2020  orCategory").   
+00004c40: 2020 2020 2073 656c 662e 7265 6669 6c6c       self.refill
+00004c50: 5f64 726f 7064 6f77 6e28 7365 6c66 2e63  _dropdown(self.c
+00004c60: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
+00004c70: 6572 6174 6f72 5f63 6c61 7373 2c20 7661  erator_class, va
+00004c80: 6c75 6529 0a20 2020 2020 2020 2076 616c  lue).        val
+00004c90: 7565 203d 2073 656c 662e 636f 6e74 6573  ue = self.contes
+00004ca0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
+00004cb0: 4261 6e64 4361 7465 676f 7279 2229 0a20  BandCategory"). 
+00004cc0: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
+00004cd0: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00004ce0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004cf0: 6261 6e64 2c20 7661 6c75 6529 0a20 2020  band, value).   
+00004d00: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
+00004d10: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
+00004d20: 6773 2e67 6574 2822 506f 7765 7243 6174  gs.get("PowerCat
+00004d30: 6567 6f72 7922 290a 2020 2020 2020 2020  egory").        
+00004d40: 7365 6c66 2e72 6566 696c 6c5f 6472 6f70  self.refill_drop
+00004d50: 646f 776e 2873 656c 662e 636f 6e74 6573  down(self.contes
+00004d60: 745f 6469 616c 6f67 2e70 6f77 6572 2c20  t_dialog.power, 
+00004d70: 7661 6c75 6529 0a20 2020 2020 2020 2076  value).        v
+00004d80: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
+00004d90: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+00004da0: 2822 4d6f 6465 4361 7465 676f 7279 2229  ("ModeCategory")
+00004db0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00004dc0: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+00004dd0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004de0: 672e 6d6f 6465 2c20 7661 6c75 6529 0a20  g.mode, value). 
+00004df0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+00004e00: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00004e10: 696e 6773 2e67 6574 2822 4f76 6572 6c61  ings.get("Overla
+00004e20: 7943 6174 6567 6f72 7922 290a 2020 2020  yCategory").    
+00004e30: 2020 2020 7365 6c66 2e72 6566 696c 6c5f      self.refill_
+00004e40: 6472 6f70 646f 776e 2873 656c 662e 636f  dropdown(self.co
+00004e50: 6e74 6573 745f 6469 616c 6f67 2e6f 7665  ntest_dialog.ove
+00004e60: 726c 6179 2c20 7661 6c75 6529 0a20 2020  rlay, value).   
+00004e70: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00004e80: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
+00004e90: 7273 2e73 6574 5465 7874 2873 656c 662e  rs.setText(self.
+00004ea0: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
+00004eb0: 2e67 6574 2822 4f70 6572 6174 6f72 7322  .get("Operators"
+00004ec0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00004ed0: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
+00004ee0: 6f61 7062 6f78 2e73 6574 506c 6169 6e54  oapbox.setPlainT
+00004ef0: 6578 7428 7365 6c66 2e63 6f6e 7465 7374  ext(self.contest
+00004f00: 5f73 6574 7469 6e67 732e 6765 7428 2253  _settings.get("S
+00004f10: 6f61 7062 6f78 2229 290a 2020 2020 2020  oapbox")).      
+00004f20: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00004f30: 6961 6c6f 672e 6578 6368 616e 6765 2e73  ialog.exchange.s
+00004f40: 6574 5465 7874 2873 656c 662e 636f 6e74  etText(self.cont
+00004f50: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+00004f60: 2822 5365 6e74 4578 6368 616e 6765 2229  ("SentExchange")
+00004f70: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+00004f80: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+00004f90: 6574 7469 6e67 732e 6765 7428 2253 7461  ettings.get("Sta
+00004fa0: 7469 6f6e 4361 7465 676f 7279 2229 0a20  tionCategory"). 
+00004fb0: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
+00004fc0: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00004fd0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004fe0: 7374 6174 696f 6e2c 2076 616c 7565 290a  station, value).
+00004ff0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00005000: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00005010: 7469 6e67 732e 6765 7428 2241 7373 6973  tings.get("Assis
+00005020: 7465 6443 6174 6567 6f72 7922 290a 2020  tedCategory").  
+00005030: 2020 2020 2020 7365 6c66 2e72 6566 696c        self.refil
+00005040: 6c5f 6472 6f70 646f 776e 2873 656c 662e  l_dropdown(self.
+00005050: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
+00005060: 7373 6973 7465 642c 2076 616c 7565 290a  ssisted, value).
+00005070: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00005080: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00005090: 7469 6e67 732e 6765 7428 2254 7261 6e73  tings.get("Trans
+000050a0: 6d69 7474 6572 4361 7465 676f 7279 2229  mitterCategory")
+000050b0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+000050c0: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+000050d0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000050e0: 672e 7472 616e 736d 6974 7465 722c 2076  g.transmitter, v
+000050f0: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
+00005100: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
+00005110: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+00005120: 2253 7461 7274 4461 7465 2229 0a20 2020  "StartDate").   
+00005130: 2020 2020 2074 6865 5f64 6174 652c 2074       the_date, t
+00005140: 6865 5f74 696d 6520 3d20 7661 6c75 652e  he_time = value.
+00005150: 7370 6c69 7428 290a 2020 2020 2020 2020  split().        
+00005160: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00005170: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
+00005180: 2e73 6574 4461 7465 280a 2020 2020 2020  .setDate(.      
+00005190: 2020 2020 2020 5174 436f 7265 2e51 4461        QtCore.QDa
+000051a0: 7465 2e66 726f 6d53 7472 696e 6728 7468  te.fromString(th
+000051b0: 655f 6461 7465 2c20 2279 7979 792d 4d4d  e_date, "yyyy-MM
+000051c0: 2d64 6422 290a 2020 2020 2020 2020 290a  -dd").        ).
+000051d0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000051e0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
+000051f0: 5469 6d65 4564 6974 2e73 6574 4361 6c65  TimeEdit.setCale
+00005200: 6e64 6172 506f 7075 7028 5472 7565 290a  ndarPopup(True).
+00005210: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00005220: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
+00005230: 5469 6d65 4564 6974 2e73 6574 5469 6d65  TimeEdit.setTime
+00005240: 280a 2020 2020 2020 2020 2020 2020 5174  (.            Qt
+00005250: 436f 7265 2e51 5469 6d65 2e66 726f 6d53  Core.QTime.fromS
+00005260: 7472 696e 6728 7468 655f 7469 6d65 2c20  tring(the_time, 
+00005270: 2268 683a 6d6d 3a73 7322 290a 2020 2020  "hh:mm:ss").    
+00005280: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+00005290: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000052a0: 672e 6f70 656e 2829 0a0a 2020 2020 6465  g.open()..    de
+000052b0: 6620 7361 7665 5f65 6469 7465 645f 636f  f save_edited_co
+000052c0: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
+000052d0: 2020 2020 2022 2222 5361 7665 2074 6865       """Save the
+000052e0: 2065 6469 7465 6420 636f 6e74 6573 7422   edited contest"
+000052f0: 2222 0a20 2020 2020 2020 2063 6f6e 7465  "".        conte
+00005300: 7374 203d 207b 7d0a 2020 2020 2020 2020  st = {}.        
+00005310: 636f 6e74 6573 745b 2243 6f6e 7465 7374  contest["Contest
+00005320: 4e61 6d65 225d 203d 2028 0a20 2020 2020  Name"] = (.     
+00005330: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+00005340: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
+00005350: 7374 2e63 7572 7265 6e74 5465 7874 2829  st.currentText()
+00005360: 2e6c 6f77 6572 2829 2e72 6570 6c61 6365  .lower().replace
+00005370: 2822 2022 2c20 225f 2229 0a20 2020 2020  (" ", "_").     
+00005380: 2020 2029 0a20 2020 2020 2020 2063 6f6e     ).        con
+00005390: 7465 7374 5b22 5374 6172 7444 6174 6522  test["StartDate"
+000053a0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+000053b0: 5f64 6961 6c6f 672e 6461 7465 5469 6d65  _dialog.dateTime
+000053c0: 4564 6974 2e64 6174 6554 696d 6528 292e  Edit.dateTime().
+000053d0: 746f 5374 7269 6e67 280a 2020 2020 2020  toString(.      
+000053e0: 2020 2020 2020 2279 7979 792d 4d4d 2d64        "yyyy-MM-d
+000053f0: 6420 6868 3a6d 6d3a 7373 220a 2020 2020  d hh:mm:ss".    
+00005400: 2020 2020 290a 2020 2020 2020 2020 636f      ).        co
+00005410: 6e74 6573 745b 224f 7065 7261 746f 7243  ntest["OperatorC
+00005420: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+00005430: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00005440: 6f70 6572 6174 6f72 5f63 6c61 7373 2e63  operator_class.c
+00005450: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+00005460: 2020 2020 2063 6f6e 7465 7374 5b22 4261       contest["Ba
+00005470: 6e64 4361 7465 676f 7279 225d 203d 2073  ndCategory"] = s
+00005480: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00005490: 6f67 2e62 616e 642e 6375 7272 656e 7454  og.band.currentT
+000054a0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+000054b0: 6e74 6573 745b 2250 6f77 6572 4361 7465  ntest["PowerCate
+000054c0: 676f 7279 225d 203d 2073 656c 662e 636f  gory"] = self.co
+000054d0: 6e74 6573 745f 6469 616c 6f67 2e70 6f77  ntest_dialog.pow
+000054e0: 6572 2e63 7572 7265 6e74 5465 7874 2829  er.currentText()
+000054f0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00005500: 5b22 4d6f 6465 4361 7465 676f 7279 225d  ["ModeCategory"]
+00005510: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00005520: 6469 616c 6f67 2e6d 6f64 652e 6375 7272  dialog.mode.curr
+00005530: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
+00005540: 2020 636f 6e74 6573 745b 224f 7665 726c    contest["Overl
+00005550: 6179 4361 7465 676f 7279 225d 203d 2073  ayCategory"] = s
+00005560: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00005570: 6f67 2e6f 7665 726c 6179 2e63 7572 7265  og.overlay.curre
+00005580: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
+00005590: 2063 6f6e 7465 7374 5b22 4f70 6572 6174   contest["Operat
+000055a0: 6f72 7322 5d20 3d20 7365 6c66 2e63 6f6e  ors"] = self.con
+000055b0: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
+000055c0: 6174 6f72 732e 7465 7874 2829 0a20 2020  ators.text().   
+000055d0: 2020 2020 2063 6f6e 7465 7374 5b22 536f       contest["So
+000055e0: 6170 626f 7822 5d20 3d20 7365 6c66 2e63  apbox"] = self.c
+000055f0: 6f6e 7465 7374 5f64 6961 6c6f 672e 736f  ontest_dialog.so
+00005600: 6170 626f 782e 746f 506c 6169 6e54 6578  apbox.toPlainTex
+00005610: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
+00005620: 6573 745b 2253 656e 7445 7863 6861 6e67  est["SentExchang
+00005630: 6522 5d20 3d20 7365 6c66 2e63 6f6e 7465  e"] = self.conte
+00005640: 7374 5f64 6961 6c6f 672e 6578 6368 616e  st_dialog.exchan
+00005650: 6765 2e74 6578 7428 290a 2020 2020 2020  ge.text().      
+00005660: 2020 636f 6e74 6573 745b 2243 6f6e 7465    contest["Conte
+00005670: 7374 4e52 225d 203d 2073 656c 662e 7072  stNR"] = self.pr
+00005680: 6566 2e67 6574 2822 636f 6e74 6573 7422  ef.get("contest"
+00005690: 2c20 3129 0a20 2020 2020 2020 2063 6f6e  , 1).        con
+000056a0: 7465 7374 5b22 5374 6174 696f 6e43 6174  test["StationCat
+000056b0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+000056c0: 6f6e 7465 7374 5f64 6961 6c6f 672e 7374  ontest_dialog.st
+000056d0: 6174 696f 6e2e 6375 7272 656e 7454 6578  ation.currentTex
+000056e0: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
+000056f0: 6573 745b 2241 7373 6973 7465 6443 6174  est["AssistedCat
+00005700: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+00005710: 6f6e 7465 7374 5f64 6961 6c6f 672e 6173  ontest_dialog.as
+00005720: 7369 7374 6564 2e63 7572 7265 6e74 5465  sisted.currentTe
+00005730: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+00005740: 7465 7374 5b22 5472 616e 736d 6974 7465  test["Transmitte
+00005750: 7243 6174 6567 6f72 7922 5d20 3d20 7365  rCategory"] = se
+00005760: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00005770: 672e 7472 616e 736d 6974 7465 722e 6375  g.transmitter.cu
+00005780: 7272 656e 7454 6578 7428 290a 0a20 2020  rrentText()..   
+00005790: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+000057a0: 6728 2225 7322 2c20 6622 7b63 6f6e 7465  g("%s", f"{conte
+000057b0: 7374 7d22 290a 2020 2020 2020 2020 7365  st}").        se
+000057c0: 6c66 2e64 6174 6162 6173 652e 7570 6461  lf.database.upda
+000057d0: 7465 5f63 6f6e 7465 7374 2863 6f6e 7465  te_contest(conte
+000057e0: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
+000057f0: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+00005800: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00005810: 2e6c 6f61 645f 636f 6e74 6573 7428 290a  .load_contest().
+00005820: 0a20 2020 2064 6566 206c 6f61 645f 636f  .    def load_co
+00005830: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
+00005840: 2020 2020 2022 2222 6c6f 6164 2061 2063       """load a c
+00005850: 6f6e 7465 7374 2222 220a 2020 2020 2020  ontest""".      
+00005860: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+00005870: 6574 2822 636f 6e74 6573 7422 293a 0a20  et("contest"):. 
+00005880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00005890: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
+000058a0: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
+000058b0: 2e66 6574 6368 5f63 6f6e 7465 7374 5f62  .fetch_contest_b
+000058c0: 795f 6964 280a 2020 2020 2020 2020 2020  y_id(.          
+000058d0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+000058e0: 6765 7428 2263 6f6e 7465 7374 2229 0a20  get("contest"). 
+000058f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00005900: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00005910: 2e63 6f6e 7465 7374 5f73 6574 7469 6e67  .contest_setting
+00005920: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00005930: 2020 2073 656c 662e 6461 7461 6261 7365     self.database
+00005940: 2e63 7572 7265 6e74 5f63 6f6e 7465 7374  .current_contest
+00005950: 203d 2073 656c 662e 7072 6566 2e67 6574   = self.pref.get
+00005960: 2822 636f 6e74 6573 7422 290a 2020 2020  ("contest").    
+00005970: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00005980: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00005990: 696e 6773 2e67 6574 2822 436f 6e74 6573  ings.get("Contes
+000059a0: 744e 616d 6522 293a 0a20 2020 2020 2020  tName"):.       
+000059b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000059c0: 662e 636f 6e74 6573 7420 3d20 646f 696d  f.contest = doim
+000059d0: 7028 7365 6c66 2e63 6f6e 7465 7374 5f73  p(self.contest_s
+000059e0: 6574 7469 6e67 732e 6765 7428 2243 6f6e  ettings.get("Con
+000059f0: 7465 7374 4e61 6d65 2229 290a 2020 2020  testName")).    
+00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a10: 6c6f 6767 6572 2e64 6562 7567 2822 4c6f  logger.debug("Lo
+00005a20: 6164 6564 2043 6f6e 7465 7374 204e 616d  aded Contest Nam
+00005a30: 6520 3d20 2573 222c 2073 656c 662e 636f  e = %s", self.co
+00005a40: 6e74 6573 742e 6e61 6d65 290a 2020 2020  ntest.name).    
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a60: 7365 6c66 2e73 6574 5f77 696e 646f 775f  self.set_window_
+00005a70: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
+00005a80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00005a90: 2e63 6f6e 7465 7374 2e69 6e69 745f 636f  .contest.init_co
+00005aa0: 6e74 6573 7428 7365 6c66 290a 2020 2020  ntest(self).    
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 7365 6c66 2e68 6964 655f 6261 6e64 5f6d  self.hide_band_m
+00005ad0: 6f64 6528 7365 6c66 2e63 6f6e 7465 7374  ode(self.contest
+00005ae0: 5f73 6574 7469 6e67 732e 6765 7428 224d  _settings.get("M
+00005af0: 6f64 6543 6174 6567 6f72 7922 2c20 2222  odeCategory", ""
+00005b00: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00005b10: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
+00005b20: 656c 662e 636f 6e74 6573 742c 2022 6d6f  elf.contest, "mo
+00005b30: 6465 2229 3a0a 2020 2020 2020 2020 2020  de"):.          
+00005b40: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005b50: 662e 636f 6e74 6573 742e 6d6f 6465 2069  f.contest.mode i
+00005b60: 6e20 5b22 4357 222c 2022 424f 5448 225d  n ["CW", "BOTH"]
+00005b70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005b80: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00005b90: 775f 7370 6565 642e 7368 6f77 2829 0a20  w_speed.show(). 
+00005ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bb0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bd0: 2073 656c 662e 6377 5f73 7065 6564 2e68   self.cw_speed.h
+00005be0: 6964 6528 290a 0a20 2020 2020 2020 2020  ide()..         
+00005bf0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
+00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c10: 636d 645b 2263 6d64 225d 203d 2022 4e45  cmd["cmd"] = "NE
+00005c20: 5744 4222 0a20 2020 2020 2020 2020 2020  WDB".           
+00005c30: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
+00005c40: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
+00005c50: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+00005c60: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+00005c70: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+00005c80: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+00005c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005ca0: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
+00005cb0: 2e63 6f6e 7465 7374 2c20 2263 6f6c 756d  .contest, "colum
+00005cc0: 6e73 2229 3a0a 2020 2020 2020 2020 2020  ns"):.          
+00005cd0: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
+00005ce0: 7b7d 0a20 2020 2020 2020 2020 2020 2020  {}.             
+00005cf0: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+00005d00: 5d20 3d20 2253 484f 5743 4f4c 554d 4e53  ] = "SHOWCOLUMNS
+00005d10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00005d20: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
+00005d30: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
+00005d40: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+00005d50: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00005d60: 434f 4c55 4d4e 5322 5d20 3d20 7365 6c66  COLUMNS"] = self
+00005d70: 2e63 6f6e 7465 7374 2e63 6f6c 756d 6e73  .contest.columns
+00005d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d90: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+00005da0: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+00005db0: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+00005dc0: 0a20 2020 2064 6566 2068 6964 655f 6261  .    def hide_ba
+00005dd0: 6e64 5f6d 6f64 6528 7365 6c66 2c20 7468  nd_mode(self, th
+00005de0: 655f 6d6f 6465 3a20 7374 7229 202d 3e20  e_mode: str) -> 
+00005df0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00005e00: 2268 6964 6522 2222 0a20 2020 2020 2020  "hide""".       
+00005e10: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
+00005e20: 7322 2c20 6622 7b74 6865 5f6d 6f64 657d  s", f"{the_mode}
+00005e30: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00005e40: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
+00005e50: 4357 2e68 6964 6528 290a 2020 2020 2020  CW.hide().      
+00005e60: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
+00005e70: 5f46 7261 6d65 5f53 5342 2e68 6964 6528  _Frame_SSB.hide(
+00005e80: 290a 2020 2020 2020 2020 7365 6c66 2e42  ).        self.B
+00005e90: 616e 645f 4d6f 6465 5f46 7261 6d65 5f52  and_Mode_Frame_R
+00005ea0: 5454 592e 6869 6465 2829 0a20 2020 2020  TTY.hide().     
+00005eb0: 2020 206d 6f64 6573 203d 207b 0a20 2020     modes = {.   
+00005ec0: 2020 2020 2020 2020 2022 4357 223a 2028           "CW": (
+00005ed0: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+00005ee0: 7261 6d65 5f43 572c 292c 0a20 2020 2020  rame_CW,),.     
+00005ef0: 2020 2020 2020 2022 5353 4222 3a20 2873         "SSB": (s
+00005f00: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
+00005f10: 616d 655f 5353 422c 292c 0a20 2020 2020  ame_SSB,),.     
+00005f20: 2020 2020 2020 2022 5254 5459 223a 2028         "RTTY": (
+00005f30: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+00005f40: 7261 6d65 5f52 5454 592c 292c 0a20 2020  rame_RTTY,),.   
+00005f50: 2020 2020 2020 2020 2022 5053 4b22 3a20           "PSK": 
+00005f60: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
+00005f70: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
+00005f80: 2020 2020 2020 2020 2020 2253 5342 2b43            "SSB+C
+00005f90: 5722 3a20 2873 656c 662e 4261 6e64 5f4d  W": (self.Band_M
+00005fa0: 6f64 655f 4672 616d 655f 4357 2c20 7365  ode_Frame_CW, se
+00005fb0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
+00005fc0: 6d65 5f53 5342 292c 0a20 2020 2020 2020  me_SSB),.       
+00005fd0: 2020 2020 2022 4449 4749 5441 4c22 3a20       "DIGITAL": 
+00005fe0: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
+00005ff0: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
+00006000: 2020 2020 2020 2020 2020 2253 5342 2b43            "SSB+C
+00006010: 572b 4449 4749 5441 4c22 3a20 280a 2020  W+DIGITAL": (.  
+00006020: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006030: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
+00006040: 6d65 5f52 5454 592c 0a20 2020 2020 2020  me_RTTY,.       
+00006050: 2020 2020 2020 2020 2073 656c 662e 4261           self.Ba
+00006060: 6e64 5f4d 6f64 655f 4672 616d 655f 4357  nd_Mode_Frame_CW
+00006070: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006080: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
+00006090: 5f46 7261 6d65 5f53 5342 2c0a 2020 2020  _Frame_SSB,.    
+000060a0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+000060b0: 2020 2020 2020 2022 464d 223a 2028 7365         "FM": (se
+000060c0: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
+000060d0: 6d65 5f53 5342 2c29 2c0a 2020 2020 2020  me_SSB,),.      
+000060e0: 2020 7d0a 2020 2020 2020 2020 6672 616d    }.        fram
+000060f0: 6573 203d 206d 6f64 6573 2e67 6574 2874  es = modes.get(t
+00006100: 6865 5f6d 6f64 6529 0a20 2020 2020 2020  he_mode).       
+00006110: 2069 6620 6672 616d 6573 3a0a 2020 2020   if frames:.    
+00006120: 2020 2020 2020 2020 666f 7220 6672 616d          for fram
+00006130: 6520 696e 2066 7261 6d65 733a 0a20 2020  e in frames:.   
+00006140: 2020 2020 2020 2020 2020 2020 2066 7261               fra
+00006150: 6d65 2e73 686f 7728 290a 0a20 2020 2064  me.show()..    d
+00006160: 6566 2066 696c 6570 6963 6b65 7228 7365  ef filepicker(se
+00006170: 6c66 2c20 6163 7469 6f6e 3a20 7374 7229  lf, action: str)
+00006180: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00006190: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
+000061a0: 2061 2066 696c 656e 616d 650a 2020 2020   a filename.    
+000061b0: 2020 2020 6163 7469 6f6e 3a20 226e 6577      action: "new
+000061c0: 2220 6f72 2022 6f70 656e 220a 2020 2020  " or "open".    
+000061d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000061e0: 6f70 7469 6f6e 7320 3d20 5146 696c 6544  options = QFileD
+000061f0: 6961 6c6f 672e 4f70 7469 6f6e 7328 290a  ialog.Options().
+00006200: 2020 2020 2020 2020 6f70 7469 6f6e 7320          options 
+00006210: 7c3d 2051 4669 6c65 4469 616c 6f67 2e44  |= QFileDialog.D
+00006220: 6f6e 7455 7365 4e61 7469 7665 4469 616c  ontUseNativeDial
+00006230: 6f67 0a20 2020 2020 2020 206f 7074 696f  og.        optio
+00006240: 6e73 207c 3d20 5146 696c 6544 6961 6c6f  ns |= QFileDialo
+00006250: 672e 446f 6e74 436f 6e66 6972 6d4f 7665  g.DontConfirmOve
+00006260: 7277 7269 7465 0a20 2020 2020 2020 2023  rwrite.        #
+00006270: 2070 6963 6b65 7220 3d20 5146 696c 6544   picker = QFileD
+00006280: 6961 6c6f 6728 7365 6c66 290a 2020 2020  ialog(self).    
+00006290: 2020 2020 6966 2061 6374 696f 6e20 3d3d      if action ==
+000062a0: 2022 6e65 7722 3a0a 2020 2020 2020 2020   "new":.        
+000062b0: 2020 2020 6669 6c65 2c20 5f20 3d20 5146      file, _ = QF
+000062c0: 696c 6544 6961 6c6f 672e 6765 7453 6176  ileDialog.getSav
+000062d0: 6546 696c 654e 616d 6528 0a20 2020 2020  eFileName(.     
+000062e0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+000062f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006300: 2022 4368 6f6f 7365 2061 2044 6174 6162   "Choose a Datab
+00006310: 6173 6522 2c0a 2020 2020 2020 2020 2020  ase",.          
+00006320: 2020 2020 2020 4441 5441 5f50 4154 482c        DATA_PATH,
+00006330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006340: 2022 4461 7461 6261 7365 2028 2a2e 6462   "Database (*.db
+00006350: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
+00006360: 2020 2020 6f70 7469 6f6e 733d 6f70 7469      options=opti
+00006370: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
+00006380: 2029 0a20 2020 2020 2020 2069 6620 6163   ).        if ac
+00006390: 7469 6f6e 203d 3d20 226f 7065 6e22 3a0a  tion == "open":.
+000063a0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+000063b0: 2c20 5f20 3d20 5146 696c 6544 6961 6c6f  , _ = QFileDialo
+000063c0: 672e 6765 744f 7065 6e46 696c 654e 616d  g.getOpenFileNam
+000063d0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+000063e0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000063f0: 2020 2020 2020 2020 2022 4368 6f6f 7365           "Choose
+00006400: 2061 2044 6174 6162 6173 6522 2c0a 2020   a Database",.  
+00006410: 2020 2020 2020 2020 2020 2020 2020 4441                DA
+00006420: 5441 5f50 4154 482c 0a20 2020 2020 2020  TA_PATH,.       
+00006430: 2020 2020 2020 2020 2022 4461 7461 6261           "Databa
+00006440: 7365 2028 2a2e 6462 2922 2c0a 2020 2020  se (*.db)",.    
+00006450: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+00006460: 6f6e 733d 6f70 7469 6f6e 732c 0a20 2020  ons=options,.   
+00006470: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00006480: 2020 2072 6574 7572 6e20 6669 6c65 0a0a     return file..
+00006490: 2020 2020 6465 6620 7265 6361 6c63 756c      def recalcul
+000064a0: 6174 655f 6d75 6c74 7328 7365 6c66 293a  ate_mults(self):
+000064b0: 0a20 2020 2020 2020 2022 2222 5265 6361  .        """Reca
+000064c0: 6c63 756c 6174 6520 4d75 6c74 6970 6c69  lculate Multipli
+000064d0: 6572 7322 2222 0a20 2020 2020 2020 2073  ers""".        s
+000064e0: 656c 662e 636f 6e74 6573 742e 7265 6361  elf.contest.reca
+000064f0: 6c63 756c 6174 655f 6d75 6c74 7328 7365  lculate_mults(se
+00006500: 6c66 290a 0a20 2020 2064 6566 206c 6175  lf)..    def lau
+00006510: 6e63 685f 6c6f 675f 7769 6e64 6f77 2873  nch_log_window(s
+00006520: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00006530: 226c 6175 6e63 6820 7468 6520 4c6f 6720  "launch the Log 
+00006540: 5769 6e64 6f77 2222 220a 2020 2020 2020  Window""".      
+00006550: 2020 6966 206e 6f74 2063 6865 636b 5f70    if not check_p
+00006560: 726f 6365 7373 2822 6c6f 6777 696e 646f  rocess("logwindo
+00006570: 772e 7079 2229 3a0a 2020 2020 2020 2020  w.py"):.        
+00006580: 2020 2020 5f20 3d20 7375 6270 726f 6365      _ = subproce
+00006590: 7373 2e50 6f70 656e 285b 7379 732e 6578  ss.Popen([sys.ex
+000065a0: 6563 7574 6162 6c65 2c20 574f 524b 494e  ecutable, WORKIN
+000065b0: 475f 5041 5448 202b 2022 2f6c 6f67 7769  G_PATH + "/logwi
+000065c0: 6e64 6f77 2e70 7922 5d29 0a0a 2020 2020  ndow.py"])..    
+000065d0: 6465 6620 6c61 756e 6368 5f62 616e 646d  def launch_bandm
+000065e0: 6170 5f77 696e 646f 7728 7365 6c66 293a  ap_window(self):
+000065f0: 0a20 2020 2020 2020 2022 2222 6c61 756e  .        """laun
+00006600: 6368 2074 6865 204c 6f67 2057 696e 646f  ch the Log Windo
+00006610: 7722 2222 0a20 2020 2020 2020 2069 6620  w""".        if 
+00006620: 6e6f 7420 6368 6563 6b5f 7072 6f63 6573  not check_proces
+00006630: 7328 2262 616e 646d 6170 2e70 7922 293a  s("bandmap.py"):
+00006640: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
+00006650: 2073 7562 7072 6f63 6573 732e 506f 7065   subprocess.Pope
+00006660: 6e28 5b73 7973 2e65 7865 6375 7461 626c  n([sys.executabl
+00006670: 652c 2057 4f52 4b49 4e47 5f50 4154 4820  e, WORKING_PATH 
+00006680: 2b20 222f 6261 6e64 6d61 702e 7079 225d  + "/bandmap.py"]
+00006690: 290a 0a20 2020 2064 6566 2063 6c65 6172  )..    def clear
+000066a0: 5f62 616e 645f 696e 6469 6361 746f 7273  _band_indicators
+000066b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000066c0: 2222 2243 6c65 6172 2074 6865 2069 6e64  """Clear the ind
+000066d0: 6963 6174 6f72 7322 2222 0a20 2020 2020  icators""".     
+000066e0: 2020 2066 6f72 205f 2c20 696e 6469 6361     for _, indica
+000066f0: 746f 7273 2069 6e20 7365 6c66 2e61 6c6c  tors in self.all
+00006700: 5f6d 6f64 655f 696e 6469 6361 746f 7273  _mode_indicators
+00006710: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00006720: 2020 2020 2020 666f 7220 5f2c 2069 6e64        for _, ind
+00006730: 6963 6174 6f72 2069 6e20 696e 6469 6361  icator in indica
+00006740: 746f 7273 2e69 7465 6d73 2829 3a0a 2020  tors.items():.  
+00006750: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00006760: 6469 6361 746f 722e 7365 7446 7261 6d65  dicator.setFrame
+00006770: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
+00006780: 5146 7261 6d65 2e4e 6f46 7261 6d65 290a  QFrame.NoFrame).
+00006790: 0a20 2020 2064 6566 2073 6574 5f62 616e  .    def set_ban
+000067a0: 645f 696e 6469 6361 746f 7228 7365 6c66  d_indicator(self
+000067b0: 2c20 6261 6e64 3a20 7374 7229 202d 3e20  , band: str) -> 
+000067c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+000067d0: 2253 6574 2074 6865 2062 616e 6420 696e  "Set the band in
+000067e0: 6469 6361 746f 7222 2222 0a20 2020 2020  dicator""".     
+000067f0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00006800: 2225 7322 2c20 6622 6261 6e64 3a7b 6261  "%s", f"band:{ba
+00006810: 6e64 7d20 6d6f 6465 3a20 7b73 656c 662e  nd} mode: {self.
+00006820: 6375 7272 656e 745f 6d6f 6465 7d22 290a  current_mode}").
+00006830: 2020 2020 2020 2020 6966 2062 616e 6420          if band 
+00006840: 616e 6420 7365 6c66 2e63 7572 7265 6e74  and self.current
+00006850: 5f6d 6f64 653a 0a20 2020 2020 2020 2020  _mode:.         
+00006860: 2020 2073 656c 662e 636c 6561 725f 6261     self.clear_ba
+00006870: 6e64 5f69 6e64 6963 6174 6f72 7328 290a  nd_indicators().
+00006880: 2020 2020 2020 2020 2020 2020 696e 6469              indi
+00006890: 6361 746f 7220 3d20 7365 6c66 2e61 6c6c  cator = self.all
+000068a0: 5f6d 6f64 655f 696e 6469 6361 746f 7273  _mode_indicators
+000068b0: 5b73 656c 662e 6375 7272 656e 745f 6d6f  [self.current_mo
+000068c0: 6465 5d2e 6765 7428 6261 6e64 2c20 4e6f  de].get(band, No
+000068d0: 6e65 290a 2020 2020 2020 2020 2020 2020  ne).            
+000068e0: 6966 2069 6e64 6963 6174 6f72 3a0a 2020  if indicator:.  
+000068f0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00006900: 6469 6361 746f 722e 7365 7446 7261 6d65  dicator.setFrame
+00006910: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
+00006920: 5146 7261 6d65 2e42 6f78 290a 0a20 2020  QFrame.Box)..   
+00006930: 2064 6566 2063 6c6f 7365 4576 656e 7428   def closeEvent(
+00006940: 7365 6c66 2c20 5f65 7665 6e74 293a 0a20  self, _event):. 
+00006950: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006960: 2020 2057 7269 7465 2077 696e 646f 7720     Write window 
+00006970: 7369 7a65 2061 6e64 2070 6f73 6974 696f  size and positio
+00006980: 6e20 746f 2063 6f6e 6669 6720 6669 6c65  n to config file
+00006990: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000069a0: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
+000069b0: 7769 6e64 6f77 5f77 6964 7468 225d 203d  window_width"] =
+000069c0: 2073 656c 662e 7369 7a65 2829 2e77 6964   self.size().wid
+000069d0: 7468 2829 0a20 2020 2020 2020 2073 656c  th().        sel
+000069e0: 662e 7072 6566 5b22 7769 6e64 6f77 5f68  f.pref["window_h
+000069f0: 6569 6768 7422 5d20 3d20 7365 6c66 2e73  eight"] = self.s
+00006a00: 697a 6528 292e 6865 6967 6874 2829 0a20  ize().height(). 
+00006a10: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00006a20: 5b22 7769 6e64 6f77 5f78 225d 203d 2073  ["window_x"] = s
+00006a30: 656c 662e 706f 7328 292e 7828 290a 2020  elf.pos().x().  
+00006a40: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+00006a50: 2277 696e 646f 775f 7922 5d20 3d20 7365  "window_y"] = se
+00006a60: 6c66 2e70 6f73 2829 2e79 2829 0a20 2020  lf.pos().y().   
+00006a70: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
+00006a80: 7072 6566 6572 656e 6365 2829 0a0a 2020  preference()..  
+00006a90: 2020 6465 6620 6374 795f 6c6f 6f6b 7570    def cty_lookup
+00006aa0: 2873 656c 662c 2063 616c 6c73 6967 6e3a  (self, callsign:
+00006ab0: 2073 7472 293a 0a20 2020 2020 2020 2022   str):.        "
+00006ac0: 2222 4c6f 6f6b 7570 2063 616c 6c73 6967  ""Lookup callsig
+00006ad0: 6e20 696e 2063 7479 2e64 6174 2066 696c  n in cty.dat fil
+00006ae0: 6522 2222 0a20 2020 2020 2020 2063 616c  e""".        cal
+00006af0: 6c73 6967 6e20 3d20 6361 6c6c 7369 676e  lsign = callsign
+00006b00: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
+00006b10: 2066 6f72 2063 6f75 6e74 2069 6e20 7265   for count in re
+00006b20: 7665 7273 6564 2872 616e 6765 286c 656e  versed(range(len
+00006b30: 2863 616c 6c73 6967 6e29 2929 3a0a 2020  (callsign))):.  
+00006b40: 2020 2020 2020 2020 2020 7365 6172 6368            search
+00006b50: 6974 656d 203d 2063 616c 6c73 6967 6e5b  item = callsign[
+00006b60: 3a20 636f 756e 7420 2b20 315d 0a20 2020  : count + 1].   
+00006b70: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+00006b80: 3d20 7b6b 6579 3a20 7661 6c20 666f 7220  = {key: val for 
+00006b90: 6b65 792c 2076 616c 2069 6e20 4354 5946  key, val in CTYF
+00006ba0: 494c 452e 6974 656d 7328 2920 6966 206b  ILE.items() if k
+00006bb0: 6579 203d 3d20 7365 6172 6368 6974 656d  ey == searchitem
+00006bc0: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
+00006bd0: 206e 6f74 2072 6573 756c 743a 0a20 2020   not result:.   
+00006be0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00006bf0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+00006c00: 2020 6966 2072 6573 756c 742e 6765 7428    if result.get(
+00006c10: 7365 6172 6368 6974 656d 292e 6765 7428  searchitem).get(
+00006c20: 2265 7861 6374 5f6d 6174 6368 2229 3a0a  "exact_match"):.
+00006c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c40: 6966 2073 6561 7263 6869 7465 6d20 3d3d  if searchitem ==
+00006c50: 2063 616c 6c73 6967 6e3a 0a20 2020 2020   callsign:.     
+00006c60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00006c70: 6574 7572 6e20 7265 7375 6c74 0a20 2020  eturn result.   
+00006c80: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00006c90: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+00006ca0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00006cb0: 0a20 2020 2064 6566 2063 7773 7065 6564  .    def cwspeed
+00006cc0: 5f73 7069 6e62 6f78 5f63 6861 6e67 6564  _spinbox_changed
+00006cd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006ce0: 2222 2274 7269 6767 6572 6564 2077 6865  """triggered whe
+00006cf0: 6e20 7661 6c75 6520 6f66 2043 5720 7370  n value of CW sp
+00006d00: 6565 6420 696e 2074 6865 2073 7069 6e62  eed in the spinb
+00006d10: 6f78 2063 6861 6e67 6573 2e22 2222 0a20  ox changes.""". 
+00006d20: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00006d30: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
+00006d40: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+00006d50: 656c 662e 6377 2e73 7065 6564 203d 2073  elf.cw.speed = s
+00006d60: 656c 662e 6377 5f73 7065 6564 2e76 616c  elf.cw_speed.val
+00006d70: 7565 2829 0a20 2020 2020 2020 2020 2020  ue().           
+00006d80: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
+00006d90: 6622 5c78 3162 327b 7365 6c66 2e63 772e  f"\x1b2{self.cw.
+00006da0: 7370 6565 647d 2229 0a0a 2020 2020 6465  speed}")..    de
+00006db0: 6620 6b65 7950 7265 7373 4576 656e 7428  f keyPressEvent(
+00006dc0: 7365 6c66 2c20 6576 656e 7429 3a20 2023  self, event):  #
+00006dd0: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+00006de0: 3d69 6e76 616c 6964 2d6e 616d 650a 2020  =invalid-name.  
+00006df0: 2020 2020 2020 2222 2254 6869 7320 6f76        """This ov
+00006e00: 6572 7269 6465 7320 5174 206b 6579 2065  errides Qt key e
+00006e10: 7665 6e74 2e22 2222 0a20 2020 2020 2020  vent.""".       
+00006e20: 206d 6f64 6966 6965 7220 3d20 6576 656e   modifier = even
+00006e30: 742e 6d6f 6469 6669 6572 7328 290a 2020  t.modifiers().  
+00006e40: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00006e50: 6579 2829 203d 3d20 5174 2e4b 6579 2e4b  ey() == Qt.Key.K
+00006e60: 6579 5f45 7363 6170 653a 2020 2320 7079  ey_Escape:  # py
+00006e70: 6c69 6e74 3a20 6469 7361 626c 653d 6e6f  lint: disable=no
+00006e80: 2d6d 656d 6265 720a 2020 2020 2020 2020  -member.        
+00006e90: 2020 2020 7365 6c66 2e63 6c65 6172 696e      self.clearin
+00006ea0: 7075 7473 2829 0a20 2020 2020 2020 2069  puts().        i
+00006eb0: 6620 7365 6c66 2e63 7720 6973 206e 6f74  f self.cw is not
+00006ec0: 204e 6f6e 6520 616e 6420 6d6f 6469 6669   None and modifi
+00006ed0: 6572 203d 3d20 5174 2e43 6f6e 7472 6f6c  er == Qt.Control
+00006ee0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+00006ef0: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+00006f00: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
+00006f10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006f20: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+00006f30: 2822 5c78 3162 3422 290a 2020 2020 2020  ("\x1b4").      
+00006f40: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+00006f50: 203d 3d20 5174 2e4b 6579 2e4b 6579 5f50   == Qt.Key.Key_P
+00006f60: 6167 6555 703a 0a20 2020 2020 2020 2020  ageUp:.         
+00006f70: 2020 2069 6620 7365 6c66 2e63 7720 6973     if self.cw is
+00006f80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00006f90: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00006fa0: 6c66 2e63 772e 7365 7276 6572 7479 7065  lf.cw.servertype
+00006fb0: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+00006fc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006fd0: 6377 2e73 7065 6564 202b 3d20 310a 2020  cw.speed += 1.  
+00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ff0: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
+00007000: 7365 7456 616c 7565 2873 656c 662e 6377  setValue(self.cw
+00007010: 2e73 7065 6564 290a 2020 2020 2020 2020  .speed).        
+00007020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007030: 2e63 772e 7365 6e64 6377 2866 225c 7831  .cw.sendcw(f"\x1
+00007040: 6232 7b73 656c 662e 6377 2e73 7065 6564  b2{self.cw.speed
+00007050: 7d22 290a 2020 2020 2020 2020 6966 2065  }").        if e
+00007060: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+00007070: 2e4b 6579 2e4b 6579 5f50 6167 6544 6f77  .Key.Key_PageDow
+00007080: 6e3a 0a20 2020 2020 2020 2020 2020 2069  n:.            i
+00007090: 6620 7365 6c66 2e63 7720 6973 206e 6f74  f self.cw is not
+000070a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000070b0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000070c0: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
+000070d0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+000070e0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+000070f0: 7065 6564 202d 3d20 310a 2020 2020 2020  peed -= 1.      
+00007100: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00007110: 6c66 2e63 775f 7370 6565 642e 7365 7456  lf.cw_speed.setV
+00007120: 616c 7565 2873 656c 662e 6377 2e73 7065  alue(self.cw.spe
+00007130: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
+00007140: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+00007150: 7365 6e64 6377 2866 225c 7831 6232 7b73  sendcw(f"\x1b2{s
+00007160: 656c 662e 6377 2e73 7065 6564 7d22 290a  elf.cw.speed}").
+00007170: 2020 2020 2020 2020 2320 6966 2065 7665          # if eve
+00007180: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+00007190: 6579 2e4b 6579 5f45 6e74 6572 3a0a 2020  ey.Key_Enter:.  
+000071a0: 2020 2020 2020 2320 2020 2020 7365 6c66        #     self
+000071b0: 2e73 6176 655f 636f 6e74 6163 7428 290a  .save_contact().
+000071c0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+000071d0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+000071e0: 2e4b 6579 5f54 6162 206f 7220 6576 656e  .Key_Tab or even
+000071f0: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
+00007200: 792e 4b65 795f 4261 636b 7461 623a 0a20  y.Key_Backtab:. 
+00007210: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00007220: 6c66 2e73 656e 742e 6861 7346 6f63 7573  lf.sent.hasFocus
+00007230: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00007240: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00007250: 2822 4672 6f6d 2073 656e 7422 290a 2020  ("From sent").  
+00007260: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007270: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
+00007280: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
+00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072a0: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
+000072b0: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
+000072c0: 7365 6c66 2e73 656e 7429 0a20 2020 2020  self.sent).     
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000072e0: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
+000072f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00007300: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+00007310: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+00007320: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007330: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
+00007340: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00007350: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007360: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00007370: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
+00007380: 5f6e 6578 742e 6765 7428 7365 6c66 2e73  _next.get(self.s
+00007390: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+000073a0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+000073b0: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
+000073e0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+000073f0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+00007400: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
+00007410: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007420: 7572 6e0a 2020 2020 2020 2020 2020 2020  urn.            
+00007430: 6966 2073 656c 662e 7265 6365 6976 652e  if self.receive.
+00007440: 6861 7346 6f63 7573 2829 3a0a 2020 2020  hasFocus():.    
+00007450: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00007460: 6572 2e64 6562 7567 2822 4672 6f6d 2072  er.debug("From r
+00007470: 6563 6569 7665 2229 0a20 2020 2020 2020  eceive").       
+00007480: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
+00007490: 6669 6572 203d 3d20 5174 2e53 6869 6674  fier == Qt.Shift
+000074a0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
+000074b0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000074c0: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
+000074d0: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
+000074e0: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
+000074f0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00007500: 765f 7461 622e 7365 7446 6f63 7573 2829  v_tab.setFocus()
+00007510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007520: 2020 2020 2070 7265 765f 7461 622e 6465       prev_tab.de
+00007530: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+00007540: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00007550: 765f 7461 622e 656e 6428 4661 6c73 6529  v_tab.end(False)
+00007560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007570: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00007580: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00007590: 7461 6220 3d20 7365 6c66 2e74 6162 5f6e  tab = self.tab_n
+000075a0: 6578 742e 6765 7428 7365 6c66 2e72 6563  ext.get(self.rec
+000075b0: 6569 7665 290a 2020 2020 2020 2020 2020  eive).          
+000075c0: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+000075d0: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
+000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075f0: 2020 6e65 7874 5f74 6162 2e64 6573 656c    next_tab.desel
+00007600: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
+00007610: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+00007620: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
+00007630: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00007640: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+00007650: 2069 6620 7365 6c66 2e6f 7468 6572 5f31   if self.other_1
+00007660: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
+00007670: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00007680: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
+00007690: 6f74 6865 725f 3122 290a 2020 2020 2020  other_1").      
+000076a0: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+000076b0: 6966 6965 7220 3d3d 2051 742e 5368 6966  ifier == Qt.Shif
+000076c0: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
+000076d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000076e0: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
+000076f0: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
+00007700: 2e6f 7468 6572 5f31 290a 2020 2020 2020  .other_1).      
+00007710: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00007720: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+00007730: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007740: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
+00007750: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+00007760: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00007770: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
+00007780: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007790: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000077a0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+000077b0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
+000077c0: 6e65 7874 2e67 6574 2873 656c 662e 6f74  next.get(self.ot
+000077d0: 6865 725f 3129 0a20 2020 2020 2020 2020  her_1).         
+000077e0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+000077f0: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
+00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007810: 2020 206e 6578 745f 7461 622e 6465 7365     next_tab.dese
+00007820: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
+00007830: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00007840: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
+00007850: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007860: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
+00007870: 2020 6966 2073 656c 662e 6f74 6865 725f    if self.other_
+00007880: 322e 6861 7346 6f63 7573 2829 3a0a 2020  2.hasFocus():.  
+00007890: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000078a0: 6767 6572 2e64 6562 7567 2822 4672 6f6d  gger.debug("From
+000078b0: 206f 7468 6572 5f32 2229 0a20 2020 2020   other_2").     
+000078c0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+000078d0: 6469 6669 6572 203d 3d20 5174 2e53 6869  difier == Qt.Shi
+000078e0: 6674 4d6f 6469 6669 6572 3a0a 2020 2020  ftModifier:.    
+000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007900: 7072 6576 5f74 6162 203d 2073 656c 662e  prev_tab = self.
+00007910: 7461 625f 7072 6576 2e67 6574 2873 656c  tab_prev.get(sel
+00007920: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
+00007930: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007940: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
+00007950: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00007960: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+00007970: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+00007980: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007990: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
+000079a0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000079b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000079c0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+000079d0: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
+000079e0: 5f6e 6578 742e 6765 7428 7365 6c66 2e6f  _next.get(self.o
+000079f0: 7468 6572 5f32 290a 2020 2020 2020 2020  ther_2).        
+00007a00: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00007a10: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a30: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
+00007a40: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+00007a50: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00007a60: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+00007a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a80: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00007a90: 2020 2069 6620 7365 6c66 2e63 616c 6c73     if self.calls
+00007aa0: 6967 6e2e 6861 7346 6f63 7573 2829 3a0a  ign.hasFocus():.
+00007ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ac0: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
+00007ad0: 6f6d 2063 616c 6c73 6967 6e22 290a 2020  om callsign").  
+00007ae0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007af0: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
+00007b00: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
 00007b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b20: 2074 6578 7420 3d20 7365 6c66 2e63 616c   text = self.cal
-00007b30: 6c73 6967 6e2e 7465 7874 2829 0a20 2020  lsign.text().   
-00007b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b50: 2074 6578 7420 3d20 7465 7874 2e75 7070   text = text.upp
-00007b60: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-00007b70: 2020 2020 2020 2020 205f 7468 6574 6872           _thethr
-00007b80: 6561 6420 3d20 7468 7265 6164 696e 672e  ead = threading.
-00007b90: 5468 7265 6164 280a 2020 2020 2020 2020  Thread(.        
+00007b20: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
+00007b30: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
+00007b40: 7365 6c66 2e63 616c 6c73 6967 6e29 0a20  self.callsign). 
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 2020 2070 7265 765f 7461 622e 7365 7446     prev_tab.setF
+00007b70: 6f63 7573 2829 0a20 2020 2020 2020 2020  ocus().         
+00007b80: 2020 2020 2020 2020 2020 2070 7265 765f             prev_
+00007b90: 7461 622e 6465 7365 6c65 6374 2829 0a20  tab.deselect(). 
 00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bb0: 7461 7267 6574 3d73 656c 662e 6368 6563  target=self.chec
-00007bc0: 6b5f 6361 6c6c 7369 676e 322c 0a20 2020  k_callsign2,.   
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 2020 2061 7267 733d 2874 6578 742c       args=(text,
-00007bf0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00007c00: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
-00007c10: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
-00007c20: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 2020 5f74 6865 7468 7265 6164 2e73 7461    _thethread.sta
-00007c50: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
-00007c60: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00007c70: 6220 3d20 7365 6c66 2e74 6162 5f6e 6578  b = self.tab_nex
-00007c80: 742e 6765 7428 7365 6c66 2e63 616c 6c73  t.get(self.calls
-00007c90: 6967 6e29 0a20 2020 2020 2020 2020 2020  ign).           
-00007ca0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00007cb0: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
-00007ce0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
-00007cf0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00007d00: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
-00007d10: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00007d20: 7572 6e0a 2020 2020 2020 2020 6966 2065  urn.        if e
-00007d30: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-00007d40: 2e4b 6579 5f46 313a 0a20 2020 2020 2020  .Key_F1:.       
-00007d50: 2020 2020 2073 656c 662e 7365 6e64 6631       self.sendf1
-00007d60: 2829 0a20 2020 2020 2020 2069 6620 6576  ().        if ev
-00007d70: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-00007d80: 4b65 795f 4632 3a0a 2020 2020 2020 2020  Key_F2:.        
-00007d90: 2020 2020 7365 6c66 2e73 656e 6466 3228      self.sendf2(
-00007da0: 290a 2020 2020 2020 2020 6966 2065 7665  ).        if eve
-00007db0: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-00007dc0: 6579 5f46 333a 0a20 2020 2020 2020 2020  ey_F3:.         
-00007dd0: 2020 2073 656c 662e 7365 6e64 6633 2829     self.sendf3()
-00007de0: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
-00007df0: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
-00007e00: 795f 4634 3a0a 2020 2020 2020 2020 2020  y_F4:.          
-00007e10: 2020 7365 6c66 2e73 656e 6466 3428 290a    self.sendf4().
-00007e20: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
-00007e30: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
-00007e40: 5f46 353a 0a20 2020 2020 2020 2020 2020  _F5:.           
-00007e50: 2073 656c 662e 7365 6e64 6635 2829 0a20   self.sendf5(). 
-00007e60: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-00007e70: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
-00007e80: 4636 3a0a 2020 2020 2020 2020 2020 2020  F6:.            
-00007e90: 7365 6c66 2e73 656e 6466 3628 290a 2020  self.sendf6().  
-00007ea0: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-00007eb0: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
-00007ec0: 373a 0a20 2020 2020 2020 2020 2020 2073  7:.            s
-00007ed0: 656c 662e 7365 6e64 6637 2829 0a20 2020  elf.sendf7().   
-00007ee0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-00007ef0: 7928 2920 3d3d 2051 742e 4b65 795f 4638  y() == Qt.Key_F8
-00007f00: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007f10: 6c66 2e73 656e 6466 3828 290a 2020 2020  lf.sendf8().    
-00007f20: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-00007f30: 2829 203d 3d20 5174 2e4b 6579 5f46 393a  () == Qt.Key_F9:
-00007f40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007f50: 662e 7365 6e64 6639 2829 0a20 2020 2020  f.sendf9().     
-00007f60: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-00007f70: 2920 3d3d 2051 742e 4b65 795f 4631 303a  ) == Qt.Key_F10:
-00007f80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00007f90: 662e 7365 6e64 6631 3028 290a 2020 2020  f.sendf10().    
-00007fa0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-00007fb0: 2829 203d 3d20 5174 2e4b 6579 5f46 3131  () == Qt.Key_F11
-00007fc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007fd0: 6c66 2e73 656e 6466 3131 2829 0a20 2020  lf.sendf11().   
-00007fe0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-00007ff0: 7928 2920 3d3d 2051 742e 4b65 795f 4631  y() == Qt.Key_F1
-00008000: 323a 0a20 2020 2020 2020 2020 2020 2073  2:.            s
-00008010: 656c 662e 7365 6e64 6631 3228 290a 0a20  elf.sendf12().. 
-00008020: 2020 2064 6566 2073 6574 5f77 696e 646f     def set_windo
-00008030: 775f 7469 746c 6528 7365 6c66 293a 0a20  w_title(self):. 
-00008040: 2020 2020 2020 2022 2222 5365 7420 7769         """Set wi
-00008050: 6e64 6f77 2074 6974 6c65 2222 220a 2020  ndow title""".  
-00008060: 2020 2020 2020 7666 6f61 203d 2073 656c        vfoa = sel
-00008070: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-00008080: 7428 2276 666f 6122 2c20 2222 290a 2020  t("vfoa", "").  
-00008090: 2020 2020 2020 6966 2076 666f 613a 0a20        if vfoa:. 
-000080a0: 2020 2020 2020 2020 2020 2076 666f 6120             vfoa 
-000080b0: 3d20 696e 7428 7666 6f61 2920 2f20 3130  = int(vfoa) / 10
-000080c0: 3030 0a20 2020 2020 2020 2065 6c73 653a  00.        else:
-000080d0: 0a20 2020 2020 2020 2020 2020 2076 666f  .            vfo
-000080e0: 6120 3d20 302e 300a 2020 2020 2020 2020  a = 0.0.        
-000080f0: 636f 6e74 6573 745f 6e61 6d65 203d 2022  contest_name = "
-00008100: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00008110: 662e 636f 6e74 6573 743a 0a20 2020 2020  f.contest:.     
-00008120: 2020 2020 2020 2063 6f6e 7465 7374 5f6e         contest_n
-00008130: 616d 6520 3d20 7365 6c66 2e63 6f6e 7465  ame = self.conte
-00008140: 7374 2e6e 616d 650a 2020 2020 2020 2020  st.name.        
-00008150: 6c69 6e65 203d 2028 0a20 2020 2020 2020  line = (.       
-00008160: 2020 2020 2066 2276 666f 613a 7b72 6f75       f"vfoa:{rou
-00008170: 6e64 2876 666f 612c 3229 7d20 220a 2020  nd(vfoa,2)} ".  
-00008180: 2020 2020 2020 2020 2020 6622 6d6f 6465            f"mode
-00008190: 3a7b 7365 6c66 2e72 6164 696f 5f73 7461  :{self.radio_sta
-000081a0: 7465 2e67 6574 2827 6d6f 6465 272c 2027  te.get('mode', '
-000081b0: 2729 7d20 220a 2020 2020 2020 2020 2020  ')} ".          
-000081c0: 2020 6622 4f50 3a7b 7365 6c66 2e63 7572    f"OP:{self.cur
-000081d0: 7265 6e74 5f6f 707d 207b 636f 6e74 6573  rent_op} {contes
-000081e0: 745f 6e61 6d65 7d20 220a 2020 2020 2020  t_name} ".      
-000081f0: 2020 2020 2020 6622 2d20 4e6f 7431 4d4d        f"- Not1MM
-00008200: 2076 7b5f 5f76 6572 7369 6f6e 5f5f 7d22   v{__version__}"
-00008210: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00008220: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00008230: 2225 7322 2c20 6c69 6e65 290a 2020 2020  "%s", line).    
-00008240: 2020 2020 7365 6c66 2e73 6574 5769 6e64      self.setWind
-00008250: 6f77 5469 746c 6528 6c69 6e65 290a 0a20  owTitle(line).. 
-00008260: 2020 2064 6566 2063 6c65 6172 696e 7075     def clearinpu
-00008270: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
-00008280: 2020 2222 2243 6c65 6172 7320 7468 6520    """Clears the 
-00008290: 7465 7874 2069 6e70 7574 2066 6965 6c64  text input field
-000082a0: 7320 616e 6420 7365 7473 2066 6f63 7573  s and sets focus
-000082b0: 2074 6f20 6361 6c6c 7369 676e 2066 6965   to callsign fie
-000082c0: 6c64 2e22 2222 0a20 2020 2020 2020 2073  ld.""".        s
-000082d0: 656c 662e 6475 7065 5f69 6e64 6963 6174  elf.dupe_indicat
-000082e0: 6f72 2e68 6964 6528 290a 2020 2020 2020  or.hide().      
-000082f0: 2020 7365 6c66 2e63 6f6e 7461 6374 203d    self.contact =
-00008300: 2073 656c 662e 6461 7461 6261 7365 2e65   self.database.e
-00008310: 6d70 7479 5f63 6f6e 7461 6374 0a20 2020  mpty_contact.   
-00008320: 2020 2020 2073 656c 662e 6865 6164 696e       self.headin
-00008330: 675f 6469 7374 616e 6365 2e73 6574 5465  g_distance.setTe
-00008340: 7874 2822 2229 0a20 2020 2020 2020 2073  xt("").        s
-00008350: 656c 662e 6478 5f65 6e74 6974 792e 7365  elf.dx_entity.se
-00008360: 7454 6578 7428 2222 290a 2020 2020 2020  tText("").      
-00008370: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-00008380: 743a 0a20 2020 2020 2020 2020 2020 206d  t:.            m
-00008390: 756c 7473 203d 2073 656c 662e 636f 6e74  ults = self.cont
-000083a0: 6573 742e 7368 6f77 5f6d 756c 7473 2873  est.show_mults(s
-000083b0: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-000083c0: 2071 736f 7320 3d20 7365 6c66 2e63 6f6e   qsos = self.con
-000083d0: 7465 7374 2e73 686f 775f 7173 6f28 7365  test.show_qso(se
-000083e0: 6c66 290a 2020 2020 2020 2020 2020 2020  lf).            
-000083f0: 6d75 6c74 7374 7269 6e67 203d 2066 227b  multstring = f"{
-00008400: 7173 6f73 7d2f 7b6d 756c 7473 7d22 0a20  qsos}/{mults}". 
-00008410: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008420: 6d75 6c74 732e 7365 7454 6578 7428 6d75  mults.setText(mu
-00008430: 6c74 7374 7269 6e67 290a 2020 2020 2020  ltstring).      
-00008440: 2020 2020 2020 7363 6f72 6520 3d20 7365        score = se
-00008450: 6c66 2e63 6f6e 7465 7374 2e63 616c 635f  lf.contest.calc_
-00008460: 7363 6f72 6528 7365 6c66 290a 2020 2020  score(self).    
-00008470: 2020 2020 2020 2020 7365 6c66 2e73 636f          self.sco
-00008480: 7265 2e73 6574 5465 7874 2873 7472 2873  re.setText(str(s
-00008490: 636f 7265 2929 0a20 2020 2020 2020 2020  core)).         
-000084a0: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
-000084b0: 7265 7365 745f 6c61 6265 6c28 7365 6c66  reset_label(self
-000084c0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-000084d0: 616c 6c73 6967 6e2e 636c 6561 7228 290a  allsign.clear().
-000084e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000084f0: 6375 7272 656e 745f 6d6f 6465 203d 3d20  current_mode == 
-00008500: 2243 5722 3a0a 2020 2020 2020 2020 2020  "CW":.          
-00008510: 2020 7365 6c66 2e73 656e 742e 7365 7454    self.sent.setT
-00008520: 6578 7428 2235 3939 2229 0a20 2020 2020  ext("599").     
-00008530: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
-00008540: 6976 652e 7365 7454 6578 7428 2235 3939  ive.setText("599
-00008550: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
-00008560: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00008570: 662e 7365 6e74 2e73 6574 5465 7874 2822  f.sent.setText("
-00008580: 3539 2229 0a20 2020 2020 2020 2020 2020  59").           
-00008590: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
-000085a0: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
-000085b0: 2020 2020 7365 6c66 2e6f 7468 6572 5f31      self.other_1
-000085c0: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
-000085d0: 2073 656c 662e 6f74 6865 725f 322e 636c   self.other_2.cl
-000085e0: 6561 7228 290a 2020 2020 2020 2020 7365  ear().        se
-000085f0: 6c66 2e63 616c 6c73 6967 6e2e 7365 7446  lf.callsign.setF
-00008600: 6f63 7573 2829 0a20 2020 2020 2020 2063  ocus().        c
-00008610: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
-00008620: 636d 645b 2263 6d64 225d 203d 2022 4341  cmd["cmd"] = "CA
-00008630: 4c4c 4348 414e 4745 4422 0a20 2020 2020  LLCHANGED".     
-00008640: 2020 2063 6d64 5b22 6361 6c6c 225d 203d     cmd["call"] =
-00008650: 2022 220a 2020 2020 2020 2020 7365 6c66   "".        self
-00008660: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-00008670: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-00008680: 6e28 636d 6429 0a0a 2020 2020 6465 6620  n(cmd)..    def 
-00008690: 7361 7665 5f63 6f6e 7461 6374 2873 656c  save_contact(sel
-000086a0: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-000086b0: 6176 6520 746f 2064 6222 2222 0a20 2020  ave to db""".   
-000086c0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-000086d0: 6728 2273 6176 696e 6720 636f 6e74 6163  g("saving contac
-000086e0: 7422 290a 2020 2020 2020 2020 6966 206c  t").        if l
-000086f0: 656e 2873 656c 662e 6361 6c6c 7369 676e  en(self.callsign
-00008700: 2e74 6578 7428 2929 203c 2033 3a0a 2020  .text()) < 3:.  
-00008710: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008720: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00008730: 616e 7928 6368 6172 2e69 7364 6967 6974  any(char.isdigit
-00008740: 2829 2066 6f72 2063 6861 7220 696e 2073  () for char in s
-00008750: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
-00008760: 7428 2929 3a0a 2020 2020 2020 2020 2020  t()):.          
-00008770: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00008780: 2069 6620 6e6f 7420 616e 7928 6368 6172   if not any(char
-00008790: 2e69 7361 6c70 6861 2829 2066 6f72 2063  .isalpha() for c
-000087a0: 6861 7220 696e 2073 656c 662e 6361 6c6c  har in self.call
-000087b0: 7369 676e 2e74 6578 7428 2929 3a0a 2020  sign.text()):.  
-000087c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000087d0: 0a0a 2020 2020 2020 2020 7365 6c66 2e63  ..        self.c
-000087e0: 6f6e 7461 6374 5b22 5453 225d 203d 2064  ontact["TS"] = d
-000087f0: 6174 6574 696d 652e 7574 636e 6f77 2829  atetime.utcnow()
-00008800: 2e69 736f 666f 726d 6174 2822 2022 295b  .isoformat(" ")[
-00008810: 3a31 395d 0a20 2020 2020 2020 2073 656c  :19].        sel
-00008820: 662e 636f 6e74 6163 745b 2243 616c 6c22  f.contact["Call"
-00008830: 5d20 3d20 7365 6c66 2e63 616c 6c73 6967  ] = self.callsig
-00008840: 6e2e 7465 7874 2829 0a20 2020 2020 2020  n.text().       
-00008850: 2073 656c 662e 636f 6e74 6163 745b 2246   self.contact["F
-00008860: 7265 7122 5d20 3d20 726f 756e 6428 666c  req"] = round(fl
-00008870: 6f61 7428 7365 6c66 2e72 6164 696f 5f73  oat(self.radio_s
-00008880: 7461 7465 2e67 6574 2822 7666 6f61 222c  tate.get("vfoa",
-00008890: 2030 2e30 2929 202f 2031 3030 302c 2032   0.0)) / 1000, 2
-000088a0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-000088b0: 6f6e 7461 6374 5b22 5153 5846 7265 7122  ontact["QSXFreq"
-000088c0: 5d20 3d20 726f 756e 6428 0a20 2020 2020  ] = round(.     
-000088d0: 2020 2020 2020 2066 6c6f 6174 2873 656c         float(sel
-000088e0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-000088f0: 7428 2276 666f 6122 2c20 302e 3029 2920  t("vfoa", 0.0)) 
-00008900: 2f20 3130 3030 2c20 320a 2020 2020 2020  / 1000, 2.      
-00008910: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-00008920: 2e63 6f6e 7461 6374 5b22 4d6f 6465 225d  .contact["Mode"]
-00008930: 203d 2073 656c 662e 7261 6469 6f5f 7374   = self.radio_st
-00008940: 6174 652e 6765 7428 226d 6f64 6522 2c20  ate.get("mode", 
-00008950: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
-00008960: 2e63 6f6e 7461 6374 5b22 436f 6e74 6573  .contact["Contes
-00008970: 744e 616d 6522 5d20 3d20 7365 6c66 2e63  tName"] = self.c
-00008980: 6f6e 7465 7374 2e63 6162 7269 6c6c 6f5f  ontest.cabrillo_
-00008990: 6e61 6d65 0a20 2020 2020 2020 2073 656c  name.        sel
-000089a0: 662e 636f 6e74 6163 745b 2243 6f6e 7465  f.contact["Conte
-000089b0: 7374 4e52 225d 203d 2073 656c 662e 7072  stNR"] = self.pr
-000089c0: 6566 2e67 6574 2822 636f 6e74 6573 7422  ef.get("contest"
-000089d0: 2c20 2230 2229 0a20 2020 2020 2020 2073  , "0").        s
-000089e0: 656c 662e 636f 6e74 6163 745b 2253 7461  elf.contact["Sta
-000089f0: 7469 6f6e 5072 6566 6978 225d 203d 2073  tionPrefix"] = s
-00008a00: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00008a10: 2243 616c 6c22 2c20 2222 290a 2020 2020  "Call", "").    
-00008a20: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00008a30: 5b22 5750 5850 7265 6669 7822 5d20 3d20  ["WPXPrefix"] = 
-00008a40: 6361 6c63 756c 6174 655f 7770 785f 7072  calculate_wpx_pr
-00008a50: 6566 6978 2873 656c 662e 6361 6c6c 7369  efix(self.callsi
-00008a60: 676e 2e74 6578 7428 2929 0a20 2020 2020  gn.text()).     
-00008a70: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
-00008a80: 2249 7352 756e 5153 4f22 5d20 3d20 7365  "IsRunQSO"] = se
-00008a90: 6c66 2e72 6164 696f 4275 7474 6f6e 5f72  lf.radioButton_r
-00008aa0: 756e 2e69 7343 6865 636b 6564 2829 0a20  un.isChecked(). 
-00008ab0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00008ac0: 6163 745b 224f 7065 7261 746f 7222 5d20  act["Operator"] 
-00008ad0: 3d20 7365 6c66 2e63 7572 7265 6e74 5f6f  = self.current_o
-00008ae0: 700a 2020 2020 2020 2020 7365 6c66 2e63  p.        self.c
-00008af0: 6f6e 7461 6374 5b22 4e65 7442 696f 734e  ontact["NetBiosN
-00008b00: 616d 6522 5d20 3d20 736f 636b 6574 2e67  ame"] = socket.g
-00008b10: 6574 686f 7374 6e61 6d65 2829 0a20 2020  ethostname().   
-00008b20: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-00008b30: 745b 2249 734f 7269 6769 6e61 6c22 5d20  t["IsOriginal"] 
-00008b40: 3d20 310a 2020 2020 2020 2020 7365 6c66  = 1.        self
-00008b50: 2e63 6f6e 7461 6374 5b22 4944 225d 203d  .contact["ID"] =
-00008b60: 2075 7569 642e 7575 6964 3428 292e 6865   uuid.uuid4().he
-00008b70: 780a 2020 2020 2020 2020 7365 6c66 2e63  x.        self.c
-00008b80: 6f6e 7465 7374 2e73 6574 5f63 6f6e 7461  ontest.set_conta
-00008b90: 6374 5f76 6172 7328 7365 6c66 290a 2020  ct_vars(self).  
-00008ba0: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
-00008bb0: 6374 5b22 506f 696e 7473 225d 203d 2073  ct["Points"] = s
-00008bc0: 656c 662e 636f 6e74 6573 742e 706f 696e  elf.contest.poin
-00008bd0: 7473 2873 656c 6629 0a20 2020 2020 2020  ts(self).       
-00008be0: 2064 6562 7567 5f6f 7574 7075 7420 3d20   debug_output = 
-00008bf0: 6622 7b73 656c 662e 636f 6e74 6163 747d  f"{self.contact}
-00008c00: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-00008c10: 2e64 6562 7567 2864 6562 7567 5f6f 7574  .debug(debug_out
-00008c20: 7075 7429 0a20 2020 2020 2020 2073 656c  put).        sel
-00008c30: 662e 6461 7461 6261 7365 2e6c 6f67 5f63  f.database.log_c
-00008c40: 6f6e 7461 6374 2873 656c 662e 636f 6e74  ontact(self.cont
-00008c50: 6163 7429 0a20 2020 2020 2020 2073 656c  act).        sel
-00008c60: 662e 6e31 6d6d 2e73 656e 645f 636f 6e74  f.n1mm.send_cont
-00008c70: 6163 745f 696e 666f 2829 0a20 2020 2020  act_info().     
-00008c80: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
-00008c90: 7574 7328 290a 2020 2020 2020 2020 636d  uts().        cm
-00008ca0: 6420 3d20 7b7d 0a20 2020 2020 2020 2063  d = {}.        c
-00008cb0: 6d64 5b22 636d 6422 5d20 3d20 2255 5044  md["cmd"] = "UPD
-00008cc0: 4154 454c 4f47 220a 2020 2020 2020 2020  ATELOG".        
-00008cd0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-00008ce0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
-00008cf0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
-00008d00: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00008d10: 745b 2243 6f6e 7465 7374 4e61 6d65 225d  t["ContestName"]
-00008d20: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
-00008d30: 6e61 6d65 0a20 2020 2020 2020 2023 2073  name.        # s
-00008d40: 656c 662e 636f 6e74 6163 745b 2253 4e54  elf.contact["SNT
-00008d50: 225d 203d 2073 656c 662e 7365 6e74 2e74  "] = self.sent.t
-00008d60: 6578 7428 290a 2020 2020 2020 2020 2320  ext().        # 
-00008d70: 7365 6c66 2e63 6f6e 7461 6374 5b22 5243  self.contact["RC
-00008d80: 5622 5d20 3d20 7365 6c66 2e72 6563 6569  V"] = self.recei
-00008d90: 7665 2e74 6578 7428 290a 2020 2020 2020  ve.text().      
-00008da0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-00008db0: 5b22 436f 756e 7472 7950 7265 6669 7822  ["CountryPrefix"
-00008dc0: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-00008dd0: 2e63 6f6e 7461 6374 5b22 5374 6174 696f  .contact["Statio
-00008de0: 6e50 7265 6669 7822 5d20 3d20 7365 6c66  nPrefix"] = self
-00008df0: 2e70 7265 662e 6765 7428 2263 616c 6c73  .pref.get("calls
-00008e00: 6967 6e22 2c20 2222 290a 2020 2020 2020  ign", "").      
-00008e10: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-00008e20: 5b22 5154 4822 5d0a 2020 2020 2020 2020  ["QTH"].        
-00008e30: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-00008e40: 4e61 6d65 225d 203d 2073 656c 662e 6f74  Name"] = self.ot
-00008e50: 6865 725f 312e 7465 7874 2829 0a20 2020  her_1.text().   
-00008e60: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-00008e70: 6163 745b 2243 6f6d 6d65 6e74 225d 203d  act["Comment"] =
-00008e80: 2073 656c 662e 6f74 6865 725f 322e 7465   self.other_2.te
-00008e90: 7874 2829 0a20 2020 2020 2020 2023 2073  xt().        # s
-00008ea0: 656c 662e 636f 6e74 6163 745b 224e 5222  elf.contact["NR"
-00008eb0: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-00008ec0: 2e63 6f6e 7461 6374 5b22 5365 6374 225d  .contact["Sect"]
-00008ed0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-00008ee0: 636f 6e74 6163 745b 2250 7265 6322 5d0a  contact["Prec"].
-00008ef0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-00008f00: 6f6e 7461 6374 5b22 434b 225d 0a20 2020  ontact["CK"].   
-00008f10: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-00008f20: 6163 745b 225a 4e22 5d0a 2020 2020 2020  act["ZN"].      
-00008f30: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-00008f40: 5b22 5365 6e74 4e72 225d 0a20 2020 2020  ["SentNr"].     
-00008f50: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00008f60: 745b 2250 6f69 6e74 7322 5d0a 2020 2020  t["Points"].    
-00008f70: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-00008f80: 6374 5b22 4973 4d75 6c74 6970 6c69 6572  ct["IsMultiplier
-00008f90: 3122 5d0a 2020 2020 2020 2020 2320 7365  1"].        # se
-00008fa0: 6c66 2e63 6f6e 7461 6374 5b22 4973 4d75  lf.contact["IsMu
-00008fb0: 6c74 6970 6c69 6572 3222 5d0a 2020 2020  ltiplier2"].    
-00008fc0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-00008fd0: 6374 5b22 506f 7765 7222 5d0a 2020 2020  ct["Power"].    
-00008fe0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-00008ff0: 6374 5b22 4261 6e64 225d 0a20 2020 2020  ct["Band"].     
-00009000: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00009010: 745b 2257 5058 5072 6566 6978 225d 203d  t["WPXPrefix"] =
-00009020: 2063 616c 6375 6c61 7465 5f77 7078 5f70   calculate_wpx_p
-00009030: 7265 6669 7828 7365 6c66 2e63 616c 6c73  refix(self.calls
-00009040: 6967 6e2e 7465 7874 2829 290a 2020 2020  ign.text()).    
+00007bb0: 2020 2070 7265 765f 7461 622e 656e 6428     prev_tab.end(
+00007bc0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+00007bd0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bf0: 2074 6578 7420 3d20 7365 6c66 2e63 616c   text = self.cal
+00007c00: 6c73 6967 6e2e 7465 7874 2829 0a20 2020  lsign.text().   
+00007c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c20: 2074 6578 7420 3d20 7465 7874 2e75 7070   text = text.upp
+00007c30: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+00007c40: 2020 2020 2020 2020 205f 7468 6574 6872           _thethr
+00007c50: 6561 6420 3d20 7468 7265 6164 696e 672e  ead = threading.
+00007c60: 5468 7265 6164 280a 2020 2020 2020 2020  Thread(.        
+00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 7461 7267 6574 3d73 656c 662e 6368 6563  target=self.chec
+00007c90: 6b5f 6361 6c6c 7369 676e 322c 0a20 2020  k_callsign2,.   
+00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007cb0: 2020 2020 2061 7267 733d 2874 6578 742c       args=(text,
+00007cc0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00007cd0: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
+00007ce0: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
+00007cf0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d10: 2020 5f74 6865 7468 7265 6164 2e73 7461    _thethread.sta
+00007d20: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
+00007d30: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+00007d40: 6220 3d20 7365 6c66 2e74 6162 5f6e 6578  b = self.tab_nex
+00007d50: 742e 6765 7428 7365 6c66 2e63 616c 6c73  t.get(self.calls
+00007d60: 6967 6e29 0a20 2020 2020 2020 2020 2020  ign).           
+00007d70: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+00007d80: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
+00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007da0: 206e 6578 745f 7461 622e 6465 7365 6c65   next_tab.desele
+00007db0: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+00007dc0: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
+00007dd0: 622e 656e 6428 4661 6c73 6529 0a20 2020  b.end(False).   
+00007de0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007df0: 7572 6e0a 2020 2020 2020 2020 6966 2065  urn.        if e
+00007e00: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+00007e10: 2e4b 6579 5f46 313a 0a20 2020 2020 2020  .Key_F1:.       
+00007e20: 2020 2020 2073 656c 662e 7365 6e64 6631       self.sendf1
+00007e30: 2829 0a20 2020 2020 2020 2069 6620 6576  ().        if ev
+00007e40: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+00007e50: 4b65 795f 4632 3a0a 2020 2020 2020 2020  Key_F2:.        
+00007e60: 2020 2020 7365 6c66 2e73 656e 6466 3228      self.sendf2(
+00007e70: 290a 2020 2020 2020 2020 6966 2065 7665  ).        if eve
+00007e80: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+00007e90: 6579 5f46 333a 0a20 2020 2020 2020 2020  ey_F3:.         
+00007ea0: 2020 2073 656c 662e 7365 6e64 6633 2829     self.sendf3()
+00007eb0: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
+00007ec0: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
+00007ed0: 795f 4634 3a0a 2020 2020 2020 2020 2020  y_F4:.          
+00007ee0: 2020 7365 6c66 2e73 656e 6466 3428 290a    self.sendf4().
+00007ef0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+00007f00: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+00007f10: 5f46 353a 0a20 2020 2020 2020 2020 2020  _F5:.           
+00007f20: 2073 656c 662e 7365 6e64 6635 2829 0a20   self.sendf5(). 
+00007f30: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
+00007f40: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
+00007f50: 4636 3a0a 2020 2020 2020 2020 2020 2020  F6:.            
+00007f60: 7365 6c66 2e73 656e 6466 3628 290a 2020  self.sendf6().  
+00007f70: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
+00007f80: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
+00007f90: 373a 0a20 2020 2020 2020 2020 2020 2073  7:.            s
+00007fa0: 656c 662e 7365 6e64 6637 2829 0a20 2020  elf.sendf7().   
+00007fb0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+00007fc0: 7928 2920 3d3d 2051 742e 4b65 795f 4638  y() == Qt.Key_F8
+00007fd0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00007fe0: 6c66 2e73 656e 6466 3828 290a 2020 2020  lf.sendf8().    
+00007ff0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+00008000: 2829 203d 3d20 5174 2e4b 6579 5f46 393a  () == Qt.Key_F9:
+00008010: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008020: 662e 7365 6e64 6639 2829 0a20 2020 2020  f.sendf9().     
+00008030: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+00008040: 2920 3d3d 2051 742e 4b65 795f 4631 303a  ) == Qt.Key_F10:
+00008050: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008060: 662e 7365 6e64 6631 3028 290a 2020 2020  f.sendf10().    
+00008070: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+00008080: 2829 203d 3d20 5174 2e4b 6579 5f46 3131  () == Qt.Key_F11
+00008090: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000080a0: 6c66 2e73 656e 6466 3131 2829 0a20 2020  lf.sendf11().   
+000080b0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+000080c0: 7928 2920 3d3d 2051 742e 4b65 795f 4631  y() == Qt.Key_F1
+000080d0: 323a 0a20 2020 2020 2020 2020 2020 2073  2:.            s
+000080e0: 656c 662e 7365 6e64 6631 3228 290a 0a20  elf.sendf12().. 
+000080f0: 2020 2064 6566 2073 6574 5f77 696e 646f     def set_windo
+00008100: 775f 7469 746c 6528 7365 6c66 293a 0a20  w_title(self):. 
+00008110: 2020 2020 2020 2022 2222 5365 7420 7769         """Set wi
+00008120: 6e64 6f77 2074 6974 6c65 2222 220a 2020  ndow title""".  
+00008130: 2020 2020 2020 7666 6f61 203d 2073 656c        vfoa = sel
+00008140: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00008150: 7428 2276 666f 6122 2c20 2222 290a 2020  t("vfoa", "").  
+00008160: 2020 2020 2020 6966 2076 666f 613a 0a20        if vfoa:. 
+00008170: 2020 2020 2020 2020 2020 2076 666f 6120             vfoa 
+00008180: 3d20 696e 7428 7666 6f61 2920 2f20 3130  = int(vfoa) / 10
+00008190: 3030 0a20 2020 2020 2020 2065 6c73 653a  00.        else:
+000081a0: 0a20 2020 2020 2020 2020 2020 2076 666f  .            vfo
+000081b0: 6120 3d20 302e 300a 2020 2020 2020 2020  a = 0.0.        
+000081c0: 636f 6e74 6573 745f 6e61 6d65 203d 2022  contest_name = "
+000081d0: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+000081e0: 662e 636f 6e74 6573 743a 0a20 2020 2020  f.contest:.     
+000081f0: 2020 2020 2020 2063 6f6e 7465 7374 5f6e         contest_n
+00008200: 616d 6520 3d20 7365 6c66 2e63 6f6e 7465  ame = self.conte
+00008210: 7374 2e6e 616d 650a 2020 2020 2020 2020  st.name.        
+00008220: 6c69 6e65 203d 2028 0a20 2020 2020 2020  line = (.       
+00008230: 2020 2020 2066 2276 666f 613a 7b72 6f75       f"vfoa:{rou
+00008240: 6e64 2876 666f 612c 3229 7d20 220a 2020  nd(vfoa,2)} ".  
+00008250: 2020 2020 2020 2020 2020 6622 6d6f 6465            f"mode
+00008260: 3a7b 7365 6c66 2e72 6164 696f 5f73 7461  :{self.radio_sta
+00008270: 7465 2e67 6574 2827 6d6f 6465 272c 2027  te.get('mode', '
+00008280: 2729 7d20 220a 2020 2020 2020 2020 2020  ')} ".          
+00008290: 2020 6622 4f50 3a7b 7365 6c66 2e63 7572    f"OP:{self.cur
+000082a0: 7265 6e74 5f6f 707d 207b 636f 6e74 6573  rent_op} {contes
+000082b0: 745f 6e61 6d65 7d20 220a 2020 2020 2020  t_name} ".      
+000082c0: 2020 2020 2020 6622 2d20 4e6f 7431 4d4d        f"- Not1MM
+000082d0: 2076 7b5f 5f76 6572 7369 6f6e 5f5f 7d22   v{__version__}"
+000082e0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000082f0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00008300: 2225 7322 2c20 6c69 6e65 290a 2020 2020  "%s", line).    
+00008310: 2020 2020 7365 6c66 2e73 6574 5769 6e64      self.setWind
+00008320: 6f77 5469 746c 6528 6c69 6e65 290a 0a20  owTitle(line).. 
+00008330: 2020 2064 6566 2063 6c65 6172 696e 7075     def clearinpu
+00008340: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+00008350: 2020 2222 2243 6c65 6172 7320 7468 6520    """Clears the 
+00008360: 7465 7874 2069 6e70 7574 2066 6965 6c64  text input field
+00008370: 7320 616e 6420 7365 7473 2066 6f63 7573  s and sets focus
+00008380: 2074 6f20 6361 6c6c 7369 676e 2066 6965   to callsign fie
+00008390: 6c64 2e22 2222 0a20 2020 2020 2020 2073  ld.""".        s
+000083a0: 656c 662e 6475 7065 5f69 6e64 6963 6174  elf.dupe_indicat
+000083b0: 6f72 2e68 6964 6528 290a 2020 2020 2020  or.hide().      
+000083c0: 2020 7365 6c66 2e63 6f6e 7461 6374 203d    self.contact =
+000083d0: 2073 656c 662e 6461 7461 6261 7365 2e65   self.database.e
+000083e0: 6d70 7479 5f63 6f6e 7461 6374 0a20 2020  mpty_contact.   
+000083f0: 2020 2020 2073 656c 662e 6865 6164 696e       self.headin
+00008400: 675f 6469 7374 616e 6365 2e73 6574 5465  g_distance.setTe
+00008410: 7874 2822 2229 0a20 2020 2020 2020 2073  xt("").        s
+00008420: 656c 662e 6478 5f65 6e74 6974 792e 7365  elf.dx_entity.se
+00008430: 7454 6578 7428 2222 290a 2020 2020 2020  tText("").      
+00008440: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
+00008450: 743a 0a20 2020 2020 2020 2020 2020 206d  t:.            m
+00008460: 756c 7473 203d 2073 656c 662e 636f 6e74  ults = self.cont
+00008470: 6573 742e 7368 6f77 5f6d 756c 7473 2873  est.show_mults(s
+00008480: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
+00008490: 2071 736f 7320 3d20 7365 6c66 2e63 6f6e   qsos = self.con
+000084a0: 7465 7374 2e73 686f 775f 7173 6f28 7365  test.show_qso(se
+000084b0: 6c66 290a 2020 2020 2020 2020 2020 2020  lf).            
+000084c0: 6d75 6c74 7374 7269 6e67 203d 2066 227b  multstring = f"{
+000084d0: 7173 6f73 7d2f 7b6d 756c 7473 7d22 0a20  qsos}/{mults}". 
+000084e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000084f0: 6d75 6c74 732e 7365 7454 6578 7428 6d75  mults.setText(mu
+00008500: 6c74 7374 7269 6e67 290a 2020 2020 2020  ltstring).      
+00008510: 2020 2020 2020 7363 6f72 6520 3d20 7365        score = se
+00008520: 6c66 2e63 6f6e 7465 7374 2e63 616c 635f  lf.contest.calc_
+00008530: 7363 6f72 6528 7365 6c66 290a 2020 2020  score(self).    
+00008540: 2020 2020 2020 2020 7365 6c66 2e73 636f          self.sco
+00008550: 7265 2e73 6574 5465 7874 2873 7472 2873  re.setText(str(s
+00008560: 636f 7265 2929 0a20 2020 2020 2020 2020  core)).         
+00008570: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
+00008580: 7265 7365 745f 6c61 6265 6c28 7365 6c66  reset_label(self
+00008590: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+000085a0: 616c 6c73 6967 6e2e 636c 6561 7228 290a  allsign.clear().
+000085b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000085c0: 6375 7272 656e 745f 6d6f 6465 203d 3d20  current_mode == 
+000085d0: 2243 5722 3a0a 2020 2020 2020 2020 2020  "CW":.          
+000085e0: 2020 7365 6c66 2e73 656e 742e 7365 7454    self.sent.setT
+000085f0: 6578 7428 2235 3939 2229 0a20 2020 2020  ext("599").     
+00008600: 2020 2020 2020 2073 656c 662e 7265 6365         self.rece
+00008610: 6976 652e 7365 7454 6578 7428 2235 3939  ive.setText("599
+00008620: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00008630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008640: 662e 7365 6e74 2e73 6574 5465 7874 2822  f.sent.setText("
+00008650: 3539 2229 0a20 2020 2020 2020 2020 2020  59").           
+00008660: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
+00008670: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
+00008680: 2020 2020 7365 6c66 2e6f 7468 6572 5f31      self.other_1
+00008690: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
+000086a0: 2073 656c 662e 6f74 6865 725f 322e 636c   self.other_2.cl
+000086b0: 6561 7228 290a 2020 2020 2020 2020 7365  ear().        se
+000086c0: 6c66 2e63 616c 6c73 6967 6e2e 7365 7446  lf.callsign.setF
+000086d0: 6f63 7573 2829 0a20 2020 2020 2020 2063  ocus().        c
+000086e0: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
+000086f0: 636d 645b 2263 6d64 225d 203d 2022 4341  cmd["cmd"] = "CA
+00008700: 4c4c 4348 414e 4745 4422 0a20 2020 2020  LLCHANGED".     
+00008710: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
+00008720: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
+00008730: 6528 290a 2020 2020 2020 2020 636d 645b  e().        cmd[
+00008740: 2263 616c 6c22 5d20 3d20 2222 0a20 2020  "call"] = "".   
+00008750: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+00008760: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+00008770: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+00008780: 0a20 2020 2064 6566 2073 6176 655f 636f  .    def save_co
+00008790: 6e74 6163 7428 7365 6c66 293a 0a20 2020  ntact(self):.   
+000087a0: 2020 2020 2022 2222 5361 7665 2074 6f20       """Save to 
+000087b0: 6462 2222 220a 2020 2020 2020 2020 6c6f  db""".        lo
+000087c0: 6767 6572 2e64 6562 7567 2822 7361 7669  gger.debug("savi
+000087d0: 6e67 2063 6f6e 7461 6374 2229 0a20 2020  ng contact").   
+000087e0: 2020 2020 2069 6620 6c65 6e28 7365 6c66       if len(self
+000087f0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+00008800: 2920 3c20 333a 0a20 2020 2020 2020 2020  ) < 3:.         
+00008810: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00008820: 2020 6966 206e 6f74 2061 6e79 2863 6861    if not any(cha
+00008830: 722e 6973 6469 6769 7428 2920 666f 7220  r.isdigit() for 
+00008840: 6368 6172 2069 6e20 7365 6c66 2e63 616c  char in self.cal
+00008850: 6c73 6967 6e2e 7465 7874 2829 293a 0a20  lsign.text()):. 
+00008860: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00008870: 6e0a 2020 2020 2020 2020 6966 206e 6f74  n.        if not
+00008880: 2061 6e79 2863 6861 722e 6973 616c 7068   any(char.isalph
+00008890: 6128 2920 666f 7220 6368 6172 2069 6e20  a() for char in 
+000088a0: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
+000088b0: 7874 2829 293a 0a20 2020 2020 2020 2020  xt()):.         
+000088c0: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+000088d0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+000088e0: 2254 5322 5d20 3d20 6461 7465 7469 6d65  "TS"] = datetime
+000088f0: 2e75 7463 6e6f 7728 292e 6973 6f66 6f72  .utcnow().isofor
+00008900: 6d61 7428 2220 2229 5b3a 3139 5d0a 2020  mat(" ")[:19].  
+00008910: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00008920: 6374 5b22 4361 6c6c 225d 203d 2073 656c  ct["Call"] = sel
+00008930: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
+00008940: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+00008950: 6f6e 7461 6374 5b22 4672 6571 225d 203d  ontact["Freq"] =
+00008960: 2072 6f75 6e64 2866 6c6f 6174 2873 656c   round(float(sel
+00008970: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00008980: 7428 2276 666f 6122 2c20 302e 3029 2920  t("vfoa", 0.0)) 
+00008990: 2f20 3130 3030 2c20 3229 0a20 2020 2020  / 1000, 2).     
+000089a0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+000089b0: 2251 5358 4672 6571 225d 203d 2072 6f75  "QSXFreq"] = rou
+000089c0: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+000089d0: 666c 6f61 7428 7365 6c66 2e72 6164 696f  float(self.radio
+000089e0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+000089f0: 222c 2030 2e30 2929 202f 2031 3030 302c  ", 0.0)) / 1000,
+00008a00: 2032 0a20 2020 2020 2020 2029 0a20 2020   2.        ).   
+00008a10: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00008a20: 745b 224d 6f64 6522 5d20 3d20 7365 6c66  t["Mode"] = self
+00008a30: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+00008a40: 2822 6d6f 6465 222c 2022 2229 0a20 2020  ("mode", "").   
+00008a50: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00008a60: 745b 2243 6f6e 7465 7374 4e61 6d65 225d  t["ContestName"]
+00008a70: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
+00008a80: 6361 6272 696c 6c6f 5f6e 616d 650a 2020  cabrillo_name.  
+00008a90: 2020 2020 2020 7365 6c66 2e63 6f6e 7461        self.conta
+00008aa0: 6374 5b22 436f 6e74 6573 744e 5222 5d20  ct["ContestNR"] 
+00008ab0: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
+00008ac0: 2263 6f6e 7465 7374 222c 2022 3022 290a  "contest", "0").
+00008ad0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00008ae0: 7461 6374 5b22 5374 6174 696f 6e50 7265  tact["StationPre
+00008af0: 6669 7822 5d20 3d20 7365 6c66 2e73 7461  fix"] = self.sta
+00008b00: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
+00008b10: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
+00008b20: 662e 636f 6e74 6163 745b 2257 5058 5072  f.contact["WPXPr
+00008b30: 6566 6978 225d 203d 2063 616c 6375 6c61  efix"] = calcula
+00008b40: 7465 5f77 7078 5f70 7265 6669 7828 7365  te_wpx_prefix(se
+00008b50: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
+00008b60: 2829 290a 2020 2020 2020 2020 7365 6c66  ()).        self
+00008b70: 2e63 6f6e 7461 6374 5b22 4973 5275 6e51  .contact["IsRunQ
+00008b80: 534f 225d 203d 2073 656c 662e 7261 6469  SO"] = self.radi
+00008b90: 6f42 7574 746f 6e5f 7275 6e2e 6973 4368  oButton_run.isCh
+00008ba0: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
+00008bb0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4f70  self.contact["Op
+00008bc0: 6572 6174 6f72 225d 203d 2073 656c 662e  erator"] = self.
+00008bd0: 6375 7272 656e 745f 6f70 0a20 2020 2020  current_op.     
+00008be0: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00008bf0: 224e 6574 4269 6f73 4e61 6d65 225d 203d  "NetBiosName"] =
+00008c00: 2073 6f63 6b65 742e 6765 7468 6f73 746e   socket.gethostn
+00008c10: 616d 6528 290a 2020 2020 2020 2020 7365  ame().        se
+00008c20: 6c66 2e63 6f6e 7461 6374 5b22 4973 4f72  lf.contact["IsOr
+00008c30: 6967 696e 616c 225d 203d 2031 0a20 2020  iginal"] = 1.   
+00008c40: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+00008c50: 745b 2249 4422 5d20 3d20 7575 6964 2e75  t["ID"] = uuid.u
+00008c60: 7569 6434 2829 2e68 6578 0a20 2020 2020  uid4().hex.     
+00008c70: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
+00008c80: 7365 745f 636f 6e74 6163 745f 7661 7273  set_contact_vars
+00008c90: 2873 656c 6629 0a20 2020 2020 2020 2073  (self).        s
+00008ca0: 656c 662e 636f 6e74 6163 745b 2250 6f69  elf.contact["Poi
+00008cb0: 6e74 7322 5d20 3d20 7365 6c66 2e63 6f6e  nts"] = self.con
+00008cc0: 7465 7374 2e70 6f69 6e74 7328 7365 6c66  test.points(self
+00008cd0: 290a 2020 2020 2020 2020 6465 6275 675f  ).        debug_
+00008ce0: 6f75 7470 7574 203d 2066 227b 7365 6c66  output = f"{self
+00008cf0: 2e63 6f6e 7461 6374 7d22 0a20 2020 2020  .contact}".     
+00008d00: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00008d10: 6465 6275 675f 6f75 7470 7574 290a 2020  debug_output).  
+00008d20: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
+00008d30: 6173 652e 6c6f 675f 636f 6e74 6163 7428  ase.log_contact(
+00008d40: 7365 6c66 2e63 6f6e 7461 6374 290a 2020  self.contact).  
+00008d50: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00008d60: 7365 6e64 5f63 6f6e 7461 6374 5f69 6e66  send_contact_inf
+00008d70: 6f28 290a 2020 2020 2020 2020 7365 6c66  o().        self
+00008d80: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
+00008d90: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
+00008da0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+00008db0: 225d 203d 2022 5550 4441 5445 4c4f 4722  "] = "UPDATELOG"
+00008dc0: 0a20 2020 2020 2020 2063 6d64 5b22 7374  .        cmd["st
+00008dd0: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
+00008de0: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
+00008df0: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+00008e00: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
+00008e10: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
+00008e20: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+00008e30: 6163 745b 2243 6f6e 7465 7374 4e61 6d65  act["ContestName
+00008e40: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+00008e50: 742e 6e61 6d65 0a20 2020 2020 2020 2023  t.name.        #
+00008e60: 2073 656c 662e 636f 6e74 6163 745b 2253   self.contact["S
+00008e70: 4e54 225d 203d 2073 656c 662e 7365 6e74  NT"] = self.sent
+00008e80: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00008e90: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+00008ea0: 5243 5622 5d20 3d20 7365 6c66 2e72 6563  RCV"] = self.rec
+00008eb0: 6569 7665 2e74 6578 7428 290a 2020 2020  eive.text().    
+00008ec0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+00008ed0: 6374 5b22 436f 756e 7472 7950 7265 6669  ct["CountryPrefi
+00008ee0: 7822 5d0a 2020 2020 2020 2020 2320 7365  x"].        # se
+00008ef0: 6c66 2e63 6f6e 7461 6374 5b22 5374 6174  lf.contact["Stat
+00008f00: 696f 6e50 7265 6669 7822 5d20 3d20 7365  ionPrefix"] = se
+00008f10: 6c66 2e70 7265 662e 6765 7428 2263 616c  lf.pref.get("cal
+00008f20: 6c73 6967 6e22 2c20 2222 290a 2020 2020  lsign", "").    
+00008f30: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+00008f40: 6374 5b22 5154 4822 5d0a 2020 2020 2020  ct["QTH"].      
+00008f50: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+00008f60: 5b22 4e61 6d65 225d 203d 2073 656c 662e  ["Name"] = self.
+00008f70: 6f74 6865 725f 312e 7465 7874 2829 0a20  other_1.text(). 
+00008f80: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
+00008f90: 6e74 6163 745b 2243 6f6d 6d65 6e74 225d  ntact["Comment"]
+00008fa0: 203d 2073 656c 662e 6f74 6865 725f 322e   = self.other_2.
+00008fb0: 7465 7874 2829 0a20 2020 2020 2020 2023  text().        #
+00008fc0: 2073 656c 662e 636f 6e74 6163 745b 224e   self.contact["N
+00008fd0: 5222 5d0a 2020 2020 2020 2020 2320 7365  R"].        # se
+00008fe0: 6c66 2e63 6f6e 7461 6374 5b22 5365 6374  lf.contact["Sect
+00008ff0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+00009000: 662e 636f 6e74 6163 745b 2250 7265 6322  f.contact["Prec"
+00009010: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+00009020: 2e63 6f6e 7461 6374 5b22 434b 225d 0a20  .contact["CK"]. 
+00009030: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
+00009040: 6e74 6163 745b 225a 4e22 5d0a 2020 2020  ntact["ZN"].    
 00009050: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-00009060: 6374 5b22 4578 6368 616e 6765 3122 5d0a  ct["Exchange1"].
-00009070: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-00009080: 6f6e 7461 6374 5b22 5261 6469 6f4e 5222  ontact["RadioNR"
-00009090: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
-000090a0: 2e63 6f6e 7461 6374 5b22 6973 4d75 6c74  .contact["isMult
-000090b0: 6970 6c69 6572 3322 5d0a 2020 2020 2020  iplier3"].      
-000090c0: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-000090d0: 5b22 4d69 7363 5465 7874 225d 0a20 2020  ["MiscText"].   
-000090e0: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-000090f0: 6163 745b 2243 6f6e 7461 6374 5479 7065  act["ContactType
-00009100: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-00009110: 662e 636f 6e74 6163 745b 2252 756e 3152  f.contact["Run1R
-00009120: 756e 3222 5d0a 2020 2020 2020 2020 2320  un2"].        # 
-00009130: 7365 6c66 2e63 6f6e 7461 6374 5b22 4772  self.contact["Gr
-00009140: 6964 5371 7561 7265 225d 0a20 2020 2020  idSquare"].     
-00009150: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00009160: 745b 2243 6f6e 7469 6e65 6e74 225d 0a20  t["Continent"]. 
-00009170: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-00009180: 6e74 6163 745b 2252 6f76 6572 4c6f 6361  ntact["RoverLoca
-00009190: 7469 6f6e 225d 0a20 2020 2020 2020 2023  tion"].        #
-000091a0: 2073 656c 662e 636f 6e74 6163 745b 2252   self.contact["R
-000091b0: 6164 696f 496e 7465 7266 6163 6564 225d  adioInterfaced"]
-000091c0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-000091d0: 636f 6e74 6163 745b 224e 6574 776f 726b  contact["Network
-000091e0: 6564 436f 6d70 4e72 225d 0a20 2020 2020  edCompNr"].     
-000091f0: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-00009200: 745b 2243 4c41 494d 4544 5153 4f22 5d0a  t["CLAIMEDQSO"].
-00009210: 0a20 2020 2064 6566 206e 6577 5f63 6f6e  .    def new_con
-00009220: 7465 7374 5f64 6961 6c6f 6728 7365 6c66  test_dialog(self
-00009230: 293a 0a20 2020 2020 2020 2022 2222 5368  ):.        """Sh
-00009240: 6f77 206e 6577 2063 6f6e 7465 7374 2064  ow new contest d
-00009250: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
-00009260: 206c 6f67 6765 722e 6465 6275 6728 224e   logger.debug("N
-00009270: 6577 2063 6f6e 7465 7374 2044 6961 6c6f  ew contest Dialo
-00009280: 6722 290a 2020 2020 2020 2020 7365 6c66  g").        self
-00009290: 2e63 6f6e 7465 7374 5f64 6961 6c6f 6720  .contest_dialog 
-000092a0: 3d20 4e65 7743 6f6e 7465 7374 2857 4f52  = NewContest(WOR
-000092b0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
-000092c0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-000092d0: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
-000092e0: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
-000092f0: 655f 636f 6e74 6573 7429 0a20 2020 2020  e_contest).     
-00009300: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-00009310: 6765 7428 2264 6172 6b5f 6d6f 6465 2229  get("dark_mode")
-00009320: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00009330: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00009340: 672e 7365 7453 7479 6c65 5368 6565 7428  g.setStyleSheet(
-00009350: 4441 524b 5f53 5459 4c45 5348 4545 5429  DARK_STYLESHEET)
-00009360: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00009370: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
-00009380: 6554 696d 6545 6469 742e 7365 7444 6174  eTimeEdit.setDat
-00009390: 6528 5174 436f 7265 2e51 4461 7465 2e63  e(QtCore.QDate.c
-000093a0: 7572 7265 6e74 4461 7465 2829 290a 2020  urrentDate()).  
-000093b0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-000093c0: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
-000093d0: 6d65 4564 6974 2e73 6574 4361 6c65 6e64  meEdit.setCalend
-000093e0: 6172 506f 7075 7028 5472 7565 290a 2020  arPopup(True).  
-000093f0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00009400: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
-00009410: 6d65 4564 6974 2e73 6574 5469 6d65 2851  meEdit.setTime(Q
-00009420: 7443 6f72 652e 5154 696d 6528 302c 2030  tCore.QTime(0, 0
-00009430: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00009440: 636f 6e74 6573 745f 6469 616c 6f67 2e70  contest_dialog.p
-00009450: 6f77 6572 2e73 6574 4375 7272 656e 7454  ower.setCurrentT
-00009460: 6578 7428 224c 4f57 2229 0a20 2020 2020  ext("LOW").     
-00009470: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-00009480: 6469 616c 6f67 2e73 7461 7469 6f6e 2e73  dialog.station.s
-00009490: 6574 4375 7272 656e 7454 6578 7428 2246  etCurrentText("F
-000094a0: 4958 4544 2229 0a20 2020 2020 2020 2073  IXED").        s
-000094b0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000094c0: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
-000094d0: 6566 2073 6176 655f 636f 6e74 6573 7428  ef save_contest(
-000094e0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-000094f0: 2222 5361 7665 2043 6f6e 7465 7374 2222  ""Save Contest""
-00009500: 220a 2020 2020 2020 2020 6e65 7874 5f6e  ".        next_n
-00009510: 756d 6265 7220 3d20 7365 6c66 2e64 6174  umber = self.dat
-00009520: 6162 6173 652e 6765 745f 6e65 7874 5f63  abase.get_next_c
-00009530: 6f6e 7465 7374 5f6e 7228 290a 2020 2020  ontest_nr().    
-00009540: 2020 2020 636f 6e74 6573 7420 3d20 7b7d      contest = {}
-00009550: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-00009560: 5b22 436f 6e74 6573 744e 616d 6522 5d20  ["ContestName"] 
-00009570: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00009580: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00009590: 6c6f 672e 636f 6e74 6573 742e 6375 7272  log.contest.curr
-000095a0: 656e 7454 6578 7428 292e 6c6f 7765 7228  entText().lower(
-000095b0: 292e 7265 706c 6163 6528 2220 222c 2022  ).replace(" ", "
-000095c0: 5f22 290a 2020 2020 2020 2020 290a 2020  _").        ).  
-000095d0: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
-000095e0: 7461 7274 4461 7465 225d 203d 2073 656c  tartDate"] = sel
-000095f0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00009600: 2e64 6174 6554 696d 6545 6469 742e 6461  .dateTimeEdit.da
-00009610: 7465 5469 6d65 2829 2e74 6f53 7472 696e  teTime().toStrin
-00009620: 6728 0a20 2020 2020 2020 2020 2020 2022  g(.            "
-00009630: 7979 7979 2d4d 4d2d 6464 2068 683a 6d6d  yyyy-MM-dd hh:mm
-00009640: 3a73 7322 0a20 2020 2020 2020 2029 0a20  :ss".        ). 
-00009650: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-00009660: 4f70 6572 6174 6f72 4361 7465 676f 7279  OperatorCategory
-00009670: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00009680: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
-00009690: 725f 636c 6173 732e 6375 7272 656e 7454  r_class.currentT
-000096a0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-000096b0: 6e74 6573 745b 2242 616e 6443 6174 6567  ntest["BandCateg
-000096c0: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-000096d0: 7465 7374 5f64 6961 6c6f 672e 6261 6e64  test_dialog.band
-000096e0: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
-000096f0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-00009700: 506f 7765 7243 6174 6567 6f72 7922 5d20  PowerCategory"] 
-00009710: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00009720: 6961 6c6f 672e 706f 7765 722e 6375 7272  ialog.power.curr
-00009730: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-00009740: 2020 636f 6e74 6573 745b 224d 6f64 6543    contest["ModeC
-00009750: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
-00009760: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00009770: 6d6f 6465 2e63 7572 7265 6e74 5465 7874  mode.currentText
-00009780: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-00009790: 7374 5b22 4f76 6572 6c61 7943 6174 6567  st["OverlayCateg
-000097a0: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-000097b0: 7465 7374 5f64 6961 6c6f 672e 6f76 6572  test_dialog.over
-000097c0: 6c61 792e 6375 7272 656e 7454 6578 7428  lay.currentText(
-000097d0: 290a 2020 2020 2020 2020 2320 636f 6e74  ).        # cont
-000097e0: 6573 745b 2743 6c61 696d 6564 5363 6f72  est['ClaimedScor
-000097f0: 6527 5d20 3d20 7365 6c66 2e63 6f6e 7465  e'] = self.conte
-00009800: 7374 5f64 6961 6c6f 672e 0a20 2020 2020  st_dialog..     
-00009810: 2020 2063 6f6e 7465 7374 5b22 4f70 6572     contest["Oper
-00009820: 6174 6f72 7322 5d20 3d20 7365 6c66 2e63  ators"] = self.c
-00009830: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
-00009840: 6572 6174 6f72 732e 7465 7874 2829 0a20  erators.text(). 
-00009850: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-00009860: 536f 6170 626f 7822 5d20 3d20 7365 6c66  Soapbox"] = self
-00009870: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00009880: 736f 6170 626f 782e 746f 506c 6169 6e54  soapbox.toPlainT
-00009890: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-000098a0: 6e74 6573 745b 2253 656e 7445 7863 6861  ntest["SentExcha
-000098b0: 6e67 6522 5d20 3d20 7365 6c66 2e63 6f6e  nge"] = self.con
-000098c0: 7465 7374 5f64 6961 6c6f 672e 6578 6368  test_dialog.exch
-000098d0: 616e 6765 2e74 6578 7428 290a 2020 2020  ange.text().    
-000098e0: 2020 2020 636f 6e74 6573 745b 2243 6f6e      contest["Con
-000098f0: 7465 7374 4e52 225d 203d 206e 6578 745f  testNR"] = next_
-00009900: 6e75 6d62 6572 2e67 6574 2822 636f 756e  number.get("coun
-00009910: 7422 2c20 3129 0a20 2020 2020 2020 2073  t", 1).        s
-00009920: 656c 662e 7072 6566 5b22 636f 6e74 6573  elf.pref["contes
-00009930: 7422 5d20 3d20 6e65 7874 5f6e 756d 6265  t"] = next_numbe
-00009940: 722e 6765 7428 2263 6f75 6e74 222c 2031  r.get("count", 1
-00009950: 290a 2020 2020 2020 2020 2320 636f 6e74  ).        # cont
-00009960: 6573 745b 2753 7562 5479 7065 275d 203d  est['SubType'] =
-00009970: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00009980: 616c 6f67 2e0a 2020 2020 2020 2020 636f  alog..        co
-00009990: 6e74 6573 745b 2253 7461 7469 6f6e 4361  ntest["StationCa
-000099a0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-000099b0: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
-000099c0: 7461 7469 6f6e 2e63 7572 7265 6e74 5465  tation.currentTe
-000099d0: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
-000099e0: 7465 7374 5b22 4173 7369 7374 6564 4361  test["AssistedCa
-000099f0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-00009a00: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
-00009a10: 7373 6973 7465 642e 6375 7272 656e 7454  ssisted.currentT
-00009a20: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-00009a30: 6e74 6573 745b 2254 7261 6e73 6d69 7474  ntest["Transmitt
-00009a40: 6572 4361 7465 676f 7279 225d 203d 2073  erCategory"] = s
-00009a50: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00009a60: 6f67 2e74 7261 6e73 6d69 7474 6572 2e63  og.transmitter.c
-00009a70: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-00009a80: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
-00009a90: 5469 6d65 4361 7465 676f 7279 275d 203d  TimeCategory'] =
-00009aa0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00009ab0: 616c 6f67 2e0a 2020 2020 2020 2020 6c6f  alog..        lo
-00009ac0: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-00009ad0: 2066 227b 636f 6e74 6573 747d 2229 0a20   f"{contest}"). 
-00009ae0: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00009af0: 6261 7365 2e61 6464 5f63 6f6e 7465 7374  base.add_contest
-00009b00: 2863 6f6e 7465 7374 290a 2020 2020 2020  (contest).      
-00009b10: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
-00009b20: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
-00009b30: 2020 7365 6c66 2e6c 6f61 645f 636f 6e74    self.load_cont
-00009b40: 6573 7428 290a 0a20 2020 2064 6566 2065  est()..    def e
-00009b50: 6469 745f 7374 6174 696f 6e5f 7365 7474  dit_station_sett
-00009b60: 696e 6773 2873 656c 6629 3a0a 2020 2020  ings(self):.    
-00009b70: 2020 2020 2222 2253 686f 7720 7365 7474      """Show sett
-00009b80: 696e 6773 2064 6961 6c6f 6722 2222 0a20  ings dialog""". 
-00009b90: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00009ba0: 6275 6728 2253 7461 7469 6f6e 2053 6574  bug("Station Set
-00009bb0: 7469 6e67 7320 7365 6c65 6374 6564 2229  tings selected")
-00009bc0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00009bd0: 7474 696e 6773 5f64 6961 6c6f 6720 3d20  ttings_dialog = 
-00009be0: 4564 6974 5374 6174 696f 6e28 574f 524b  EditStation(WORK
-00009bf0: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
-00009c00: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-00009c10: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
-00009c20: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
-00009c30: 655f 7365 7474 696e 6773 290a 2020 2020  e_settings).    
-00009c40: 2020 2020 2320 6966 2073 656c 662e 7072      # if self.pr
-00009c50: 6566 2e67 6574 2822 6461 726b 5f6d 6f64  ef.get("dark_mod
-00009c60: 6522 293a 0a20 2020 2020 2020 2023 2020  e"):.        #  
-00009c70: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-00009c80: 5f64 6961 6c6f 672e 7365 7453 7479 6c65  _dialog.setStyle
-00009c90: 5368 6565 7428 4441 524b 5f53 5459 4c45  Sheet(DARK_STYLE
-00009ca0: 5348 4545 5429 0a0a 2020 2020 2020 2020  SHEET)..        
-00009cb0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-00009cc0: 616c 6f67 2e43 616c 6c2e 7365 7454 6578  alog.Call.setTex
-00009cd0: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-00009ce0: 6574 2822 4361 6c6c 222c 2022 2229 290a  et("Call", "")).
-00009cf0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00009d00: 7469 6e67 735f 6469 616c 6f67 2e4e 616d  tings_dialog.Nam
-00009d10: 652e 7365 7454 6578 7428 7365 6c66 2e73  e.setText(self.s
-00009d20: 7461 7469 6f6e 2e67 6574 2822 4e61 6d65  tation.get("Name
-00009d30: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-00009d40: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-00009d50: 616c 6f67 2e41 6464 7265 7373 312e 7365  alog.Address1.se
-00009d60: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-00009d70: 6f6e 2e67 6574 2822 5374 7265 6574 3122  on.get("Street1"
-00009d80: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-00009d90: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-00009da0: 6c6f 672e 4164 6472 6573 7332 2e73 6574  log.Address2.set
-00009db0: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-00009dc0: 6e2e 6765 7428 2253 7472 6565 7432 222c  n.get("Street2",
-00009dd0: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
-00009de0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-00009df0: 6f67 2e43 6974 792e 7365 7454 6578 7428  og.City.setText(
-00009e00: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00009e10: 2822 4369 7479 222c 2022 2229 290a 2020  ("City", "")).  
-00009e20: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-00009e30: 6e67 735f 6469 616c 6f67 2e53 7461 7465  ngs_dialog.State
-00009e40: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-00009e50: 6174 696f 6e2e 6765 7428 2253 7461 7465  ation.get("State
-00009e60: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-00009e70: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-00009e80: 616c 6f67 2e5a 6970 2e73 6574 5465 7874  alog.Zip.setText
-00009e90: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-00009ea0: 7428 225a 6970 222c 2022 2229 290a 2020  t("Zip", "")).  
-00009eb0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-00009ec0: 6e67 735f 6469 616c 6f67 2e43 6f75 6e74  ngs_dialog.Count
-00009ed0: 7279 2e73 6574 5465 7874 2873 656c 662e  ry.setText(self.
-00009ee0: 7374 6174 696f 6e2e 6765 7428 2243 6f75  station.get("Cou
-00009ef0: 6e74 7279 222c 2022 2229 290a 2020 2020  ntry", "")).    
-00009f00: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-00009f10: 735f 6469 616c 6f67 2e47 7269 6453 7175  s_dialog.GridSqu
-00009f20: 6172 652e 7365 7454 6578 7428 7365 6c66  are.setText(self
-00009f30: 2e73 7461 7469 6f6e 2e67 6574 2822 4772  .station.get("Gr
-00009f40: 6964 5371 7561 7265 222c 2022 2229 290a  idSquare", "")).
-00009f50: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-00009f60: 7469 6e67 735f 6469 616c 6f67 2e43 515a  tings_dialog.CQZ
-00009f70: 6f6e 652e 7365 7454 6578 7428 7374 7228  one.setText(str(
-00009f80: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-00009f90: 2822 4351 5a6f 6e65 222c 2022 2229 2929  ("CQZone", "")))
-00009fa0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00009fb0: 7474 696e 6773 5f64 6961 6c6f 672e 4954  ttings_dialog.IT
-00009fc0: 555a 6f6e 652e 7365 7454 6578 7428 7374  UZone.setText(st
-00009fd0: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
-00009fe0: 6574 2822 4941 5255 5a6f 6e65 222c 2022  et("IARUZone", "
-00009ff0: 2229 2929 0a20 2020 2020 2020 2073 656c  "))).        sel
-0000a000: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000a010: 672e 4c69 6365 6e73 652e 7365 7454 6578  g.License.setTex
-0000a020: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000a030: 6574 2822 4c69 6365 6e73 6543 6c61 7373  et("LicenseClass
-0000a040: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-0000a050: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a060: 616c 6f67 2e4c 6174 6974 7564 652e 7365  alog.Latitude.se
-0000a070: 7454 6578 7428 7374 7228 7365 6c66 2e73  tText(str(self.s
-0000a080: 7461 7469 6f6e 2e67 6574 2822 4c61 7469  tation.get("Lati
-0000a090: 7475 6465 222c 2022 2229 2929 0a20 2020  tude", ""))).   
-0000a0a0: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000a0b0: 6773 5f64 6961 6c6f 672e 4c6f 6e67 6974  gs_dialog.Longit
-0000a0c0: 7564 652e 7365 7454 6578 7428 7374 7228  ude.setText(str(
-0000a0d0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-0000a0e0: 2822 4c6f 6e67 6974 7564 6522 2c20 2222  ("Longitude", ""
-0000a0f0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-0000a100: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000a110: 2e53 7461 7469 6f6e 5458 5258 2e73 6574  .StationTXRX.set
-0000a120: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-0000a130: 6e2e 6765 7428 2273 7461 7469 6f6e 7478  n.get("stationtx
-0000a140: 7278 222c 2022 2229 290a 2020 2020 2020  rx", "")).      
-0000a150: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
-0000a160: 6469 616c 6f67 2e50 6f77 6572 2e73 6574  dialog.Power.set
-0000a170: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
-0000a180: 6e2e 6765 7428 2253 506f 7765 222c 2022  n.get("SPowe", "
-0000a190: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
-0000a1a0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000a1b0: 2e41 6e74 656e 6e61 2e73 6574 5465 7874  .Antenna.setText
-0000a1c0: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000a1d0: 7428 2253 416e 7465 222c 2022 2229 290a  t("SAnte", "")).
-0000a1e0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a1f0: 7469 6e67 735f 6469 616c 6f67 2e41 6e74  tings_dialog.Ant
-0000a200: 4865 6967 6874 2e73 6574 5465 7874 2873  Height.setText(s
-0000a210: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000a220: 2253 416e 7448 3122 2c20 2222 2929 0a20  "SAntH1", "")). 
-0000a230: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000a240: 696e 6773 5f64 6961 6c6f 672e 4153 4c2e  ings_dialog.ASL.
-0000a250: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000a260: 7469 6f6e 2e67 6574 2822 5341 6e74 4832  tion.get("SAntH2
-0000a270: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
-0000a280: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a290: 616c 6f67 2e41 5252 4c53 6563 7469 6f6e  alog.ARRLSection
-0000a2a0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000a2b0: 6174 696f 6e2e 6765 7428 2241 5252 4c53  ation.get("ARRLS
-0000a2c0: 6563 7469 6f6e 222c 2022 2229 290a 2020  ection", "")).  
-0000a2d0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000a2e0: 6e67 735f 6469 616c 6f67 2e52 6f76 6572  ngs_dialog.Rover
-0000a2f0: 5154 482e 7365 7454 6578 7428 7365 6c66  QTH.setText(self
-0000a300: 2e73 7461 7469 6f6e 2e67 6574 2822 526f  .station.get("Ro
-0000a310: 7665 7251 5448 222c 2022 2229 290a 2020  verQTH", "")).  
-0000a320: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000a330: 6e67 735f 6469 616c 6f67 2e43 6c75 622e  ngs_dialog.Club.
-0000a340: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000a350: 7469 6f6e 2e67 6574 2822 436c 7562 222c  tion.get("Club",
-0000a360: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
-0000a370: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000a380: 6f67 2e45 6d61 696c 2e73 6574 5465 7874  og.Email.setText
-0000a390: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000a3a0: 7428 2245 6d61 696c 222c 2022 2229 290a  t("Email", "")).
-0000a3b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000a3c0: 7469 6e67 735f 6469 616c 6f67 2e6f 7065  tings_dialog.ope
-0000a3d0: 6e28 290a 0a20 2020 2064 6566 2073 6176  n()..    def sav
-0000a3e0: 655f 7365 7474 696e 6773 2873 656c 6629  e_settings(self)
-0000a3f0: 3a0a 2020 2020 2020 2020 2222 2253 6176  :.        """Sav
-0000a400: 6520 7365 7474 696e 6773 2222 220a 2020  e settings""".  
-0000a410: 2020 2020 2020 6373 203d 2073 656c 662e        cs = self.
-0000a420: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000a430: 4361 6c6c 2e74 6578 7428 290a 2020 2020  Call.text().    
-0000a440: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-0000a450: 203d 207b 7d0a 2020 2020 2020 2020 7365   = {}.        se
-0000a460: 6c66 2e73 7461 7469 6f6e 5b22 4361 6c6c  lf.station["Call
-0000a470: 225d 203d 2063 732e 7570 7065 7228 290a  "] = cs.upper().
-0000a480: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000a490: 7469 6f6e 5b22 4e61 6d65 225d 203d 2073  tion["Name"] = s
-0000a4a0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000a4b0: 6c6f 672e 4e61 6d65 2e74 6578 7428 292e  log.Name.text().
-0000a4c0: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-0000a4d0: 7365 6c66 2e73 7461 7469 6f6e 5b22 5374  self.station["St
-0000a4e0: 7265 6574 3122 5d20 3d20 7365 6c66 2e73  reet1"] = self.s
-0000a4f0: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
-0000a500: 6464 7265 7373 312e 7465 7874 2829 2e74  ddress1.text().t
-0000a510: 6974 6c65 2829 0a20 2020 2020 2020 2073  itle().        s
-0000a520: 656c 662e 7374 6174 696f 6e5b 2253 7472  elf.station["Str
-0000a530: 6565 7432 225d 203d 2073 656c 662e 7365  eet2"] = self.se
-0000a540: 7474 696e 6773 5f64 6961 6c6f 672e 4164  ttings_dialog.Ad
-0000a550: 6472 6573 7332 2e74 6578 7428 292e 7469  dress2.text().ti
-0000a560: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
-0000a570: 6c66 2e73 7461 7469 6f6e 5b22 4369 7479  lf.station["City
-0000a580: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-0000a590: 6773 5f64 6961 6c6f 672e 4369 7479 2e74  gs_dialog.City.t
-0000a5a0: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
-0000a5b0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000a5c0: 6f6e 5b22 5374 6174 6522 5d20 3d20 7365  on["State"] = se
-0000a5d0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000a5e0: 6f67 2e53 7461 7465 2e74 6578 7428 292e  og.State.text().
-0000a5f0: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
-0000a600: 7365 6c66 2e73 7461 7469 6f6e 5b22 5a69  self.station["Zi
-0000a610: 7022 5d20 3d20 7365 6c66 2e73 6574 7469  p"] = self.setti
-0000a620: 6e67 735f 6469 616c 6f67 2e5a 6970 2e74  ngs_dialog.Zip.t
-0000a630: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000a640: 6c66 2e73 7461 7469 6f6e 5b22 436f 756e  lf.station["Coun
-0000a650: 7472 7922 5d20 3d20 7365 6c66 2e73 6574  try"] = self.set
-0000a660: 7469 6e67 735f 6469 616c 6f67 2e43 6f75  tings_dialog.Cou
-0000a670: 6e74 7279 2e74 6578 7428 292e 7469 746c  ntry.text().titl
-0000a680: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
-0000a690: 2e73 7461 7469 6f6e 5b22 4772 6964 5371  .station["GridSq
-0000a6a0: 7561 7265 225d 203d 2073 656c 662e 7365  uare"] = self.se
-0000a6b0: 7474 696e 6773 5f64 6961 6c6f 672e 4772  ttings_dialog.Gr
-0000a6c0: 6964 5371 7561 7265 2e74 6578 7428 290a  idSquare.text().
+00009060: 6374 5b22 5365 6e74 4e72 225d 0a20 2020  ct["SentNr"].   
+00009070: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+00009080: 6163 745b 2250 6f69 6e74 7322 5d0a 2020  act["Points"].  
+00009090: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+000090a0: 7461 6374 5b22 4973 4d75 6c74 6970 6c69  tact["IsMultipli
+000090b0: 6572 3122 5d0a 2020 2020 2020 2020 2320  er1"].        # 
+000090c0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4973  self.contact["Is
+000090d0: 4d75 6c74 6970 6c69 6572 3222 5d0a 2020  Multiplier2"].  
+000090e0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+000090f0: 7461 6374 5b22 506f 7765 7222 5d0a 2020  tact["Power"].  
+00009100: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+00009110: 7461 6374 5b22 4261 6e64 225d 0a20 2020  tact["Band"].   
+00009120: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+00009130: 6163 745b 2257 5058 5072 6566 6978 225d  act["WPXPrefix"]
+00009140: 203d 2063 616c 6375 6c61 7465 5f77 7078   = calculate_wpx
+00009150: 5f70 7265 6669 7828 7365 6c66 2e63 616c  _prefix(self.cal
+00009160: 6c73 6967 6e2e 7465 7874 2829 290a 2020  lsign.text()).  
+00009170: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+00009180: 7461 6374 5b22 4578 6368 616e 6765 3122  tact["Exchange1"
+00009190: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+000091a0: 2e63 6f6e 7461 6374 5b22 5261 6469 6f4e  .contact["RadioN
+000091b0: 5222 5d0a 2020 2020 2020 2020 2320 7365  R"].        # se
+000091c0: 6c66 2e63 6f6e 7461 6374 5b22 6973 4d75  lf.contact["isMu
+000091d0: 6c74 6970 6c69 6572 3322 5d0a 2020 2020  ltiplier3"].    
+000091e0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+000091f0: 6374 5b22 4d69 7363 5465 7874 225d 0a20  ct["MiscText"]. 
+00009200: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
+00009210: 6e74 6163 745b 2243 6f6e 7461 6374 5479  ntact["ContactTy
+00009220: 7065 225d 0a20 2020 2020 2020 2023 2073  pe"].        # s
+00009230: 656c 662e 636f 6e74 6163 745b 2252 756e  elf.contact["Run
+00009240: 3152 756e 3222 5d0a 2020 2020 2020 2020  1Run2"].        
+00009250: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+00009260: 4772 6964 5371 7561 7265 225d 0a20 2020  GridSquare"].   
+00009270: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+00009280: 6163 745b 2243 6f6e 7469 6e65 6e74 225d  act["Continent"]
+00009290: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+000092a0: 636f 6e74 6163 745b 2252 6f76 6572 4c6f  contact["RoverLo
+000092b0: 6361 7469 6f6e 225d 0a20 2020 2020 2020  cation"].       
+000092c0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+000092d0: 2252 6164 696f 496e 7465 7266 6163 6564  "RadioInterfaced
+000092e0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+000092f0: 662e 636f 6e74 6163 745b 224e 6574 776f  f.contact["Netwo
+00009300: 726b 6564 436f 6d70 4e72 225d 0a20 2020  rkedCompNr"].   
+00009310: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+00009320: 6163 745b 2243 4c41 494d 4544 5153 4f22  act["CLAIMEDQSO"
+00009330: 5d0a 0a20 2020 2064 6566 206e 6577 5f63  ]..    def new_c
+00009340: 6f6e 7465 7374 5f64 6961 6c6f 6728 7365  ontest_dialog(se
+00009350: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00009360: 5368 6f77 206e 6577 2063 6f6e 7465 7374  Show new contest
+00009370: 2064 6961 6c6f 6722 2222 0a20 2020 2020   dialog""".     
+00009380: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00009390: 224e 6577 2063 6f6e 7465 7374 2044 6961  "New contest Dia
+000093a0: 6c6f 6722 290a 2020 2020 2020 2020 7365  log").        se
+000093b0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000093c0: 6720 3d20 4e65 7743 6f6e 7465 7374 2857  g = NewContest(W
+000093d0: 4f52 4b49 4e47 5f50 4154 4829 0a20 2020  ORKING_PATH).   
+000093e0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+000093f0: 745f 6469 616c 6f67 2e61 6363 6570 7465  t_dialog.accepte
+00009400: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
+00009410: 6176 655f 636f 6e74 6573 7429 0a20 2020  ave_contest).   
+00009420: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+00009430: 662e 6765 7428 2264 6172 6b5f 6d6f 6465  f.get("dark_mode
+00009440: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00009450: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+00009460: 6c6f 672e 7365 7453 7479 6c65 5368 6565  log.setStyleShee
+00009470: 7428 4441 524b 5f53 5459 4c45 5348 4545  t(DARK_STYLESHEE
+00009480: 5429 0a20 2020 2020 2020 2073 656c 662e  T).        self.
+00009490: 636f 6e74 6573 745f 6469 616c 6f67 2e64  contest_dialog.d
+000094a0: 6174 6554 696d 6545 6469 742e 7365 7444  ateTimeEdit.setD
+000094b0: 6174 6528 5174 436f 7265 2e51 4461 7465  ate(QtCore.QDate
+000094c0: 2e63 7572 7265 6e74 4461 7465 2829 290a  .currentDate()).
+000094d0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000094e0: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
+000094f0: 5469 6d65 4564 6974 2e73 6574 4361 6c65  TimeEdit.setCale
+00009500: 6e64 6172 506f 7075 7028 5472 7565 290a  ndarPopup(True).
+00009510: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00009520: 7465 7374 5f64 6961 6c6f 672e 6461 7465  test_dialog.date
+00009530: 5469 6d65 4564 6974 2e73 6574 5469 6d65  TimeEdit.setTime
+00009540: 2851 7443 6f72 652e 5154 696d 6528 302c  (QtCore.QTime(0,
+00009550: 2030 2929 0a20 2020 2020 2020 2073 656c   0)).        sel
+00009560: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00009570: 2e70 6f77 6572 2e73 6574 4375 7272 656e  .power.setCurren
+00009580: 7454 6578 7428 224c 4f57 2229 0a20 2020  tText("LOW").   
+00009590: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+000095a0: 745f 6469 616c 6f67 2e73 7461 7469 6f6e  t_dialog.station
+000095b0: 2e73 6574 4375 7272 656e 7454 6578 7428  .setCurrentText(
+000095c0: 2246 4958 4544 2229 0a20 2020 2020 2020  "FIXED").       
+000095d0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+000095e0: 616c 6f67 2e6f 7065 6e28 290a 0a20 2020  alog.open()..   
+000095f0: 2064 6566 2073 6176 655f 636f 6e74 6573   def save_contes
+00009600: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00009610: 2022 2222 5361 7665 2043 6f6e 7465 7374   """Save Contest
+00009620: 2222 220a 2020 2020 2020 2020 6e65 7874  """.        next
+00009630: 5f6e 756d 6265 7220 3d20 7365 6c66 2e64  _number = self.d
+00009640: 6174 6162 6173 652e 6765 745f 6e65 7874  atabase.get_next
+00009650: 5f63 6f6e 7465 7374 5f6e 7228 290a 2020  _contest_nr().  
+00009660: 2020 2020 2020 636f 6e74 6573 7420 3d20        contest = 
+00009670: 7b7d 0a20 2020 2020 2020 2063 6f6e 7465  {}.        conte
+00009680: 7374 5b22 436f 6e74 6573 744e 616d 6522  st["ContestName"
+00009690: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+000096a0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+000096b0: 6961 6c6f 672e 636f 6e74 6573 742e 6375  ialog.contest.cu
+000096c0: 7272 656e 7454 6578 7428 292e 6c6f 7765  rrentText().lowe
+000096d0: 7228 292e 7265 706c 6163 6528 2220 222c  r().replace(" ",
+000096e0: 2022 5f22 290a 2020 2020 2020 2020 290a   "_").        ).
+000096f0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+00009700: 2253 7461 7274 4461 7465 225d 203d 2073  "StartDate"] = s
+00009710: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00009720: 6f67 2e64 6174 6554 696d 6545 6469 742e  og.dateTimeEdit.
+00009730: 6461 7465 5469 6d65 2829 2e74 6f53 7472  dateTime().toStr
+00009740: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00009750: 2022 7979 7979 2d4d 4d2d 6464 2068 683a   "yyyy-MM-dd hh:
+00009760: 6d6d 3a73 7322 0a20 2020 2020 2020 2029  mm:ss".        )
+00009770: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00009780: 5b22 4f70 6572 6174 6f72 4361 7465 676f  ["OperatorCatego
+00009790: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
+000097a0: 6573 745f 6469 616c 6f67 2e6f 7065 7261  est_dialog.opera
+000097b0: 746f 725f 636c 6173 732e 6375 7272 656e  tor_class.curren
+000097c0: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
+000097d0: 636f 6e74 6573 745b 2242 616e 6443 6174  contest["BandCat
+000097e0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+000097f0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6261  ontest_dialog.ba
+00009800: 6e64 2e63 7572 7265 6e74 5465 7874 2829  nd.currentText()
+00009810: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00009820: 5b22 506f 7765 7243 6174 6567 6f72 7922  ["PowerCategory"
+00009830: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
+00009840: 5f64 6961 6c6f 672e 706f 7765 722e 6375  _dialog.power.cu
+00009850: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
+00009860: 2020 2020 636f 6e74 6573 745b 224d 6f64      contest["Mod
+00009870: 6543 6174 6567 6f72 7922 5d20 3d20 7365  eCategory"] = se
+00009880: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00009890: 672e 6d6f 6465 2e63 7572 7265 6e74 5465  g.mode.currentTe
+000098a0: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+000098b0: 7465 7374 5b22 4f76 6572 6c61 7943 6174  test["OverlayCat
+000098c0: 6567 6f72 7922 5d20 3d20 7365 6c66 2e63  egory"] = self.c
+000098d0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f76  ontest_dialog.ov
+000098e0: 6572 6c61 792e 6375 7272 656e 7454 6578  erlay.currentTex
+000098f0: 7428 290a 2020 2020 2020 2020 2320 636f  t().        # co
+00009900: 6e74 6573 745b 2743 6c61 696d 6564 5363  ntest['ClaimedSc
+00009910: 6f72 6527 5d20 3d20 7365 6c66 2e63 6f6e  ore'] = self.con
+00009920: 7465 7374 5f64 6961 6c6f 672e 0a20 2020  test_dialog..   
+00009930: 2020 2020 2063 6f6e 7465 7374 5b22 4f70       contest["Op
+00009940: 6572 6174 6f72 7322 5d20 3d20 7365 6c66  erators"] = self
+00009950: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00009960: 6f70 6572 6174 6f72 732e 7465 7874 2829  operators.text()
+00009970: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+00009980: 5b22 536f 6170 626f 7822 5d20 3d20 7365  ["Soapbox"] = se
+00009990: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000099a0: 672e 736f 6170 626f 782e 746f 506c 6169  g.soapbox.toPlai
+000099b0: 6e54 6578 7428 290a 2020 2020 2020 2020  nText().        
+000099c0: 636f 6e74 6573 745b 2253 656e 7445 7863  contest["SentExc
+000099d0: 6861 6e67 6522 5d20 3d20 7365 6c66 2e63  hange"] = self.c
+000099e0: 6f6e 7465 7374 5f64 6961 6c6f 672e 6578  ontest_dialog.ex
+000099f0: 6368 616e 6765 2e74 6578 7428 290a 2020  change.text().  
+00009a00: 2020 2020 2020 636f 6e74 6573 745b 2243        contest["C
+00009a10: 6f6e 7465 7374 4e52 225d 203d 206e 6578  ontestNR"] = nex
+00009a20: 745f 6e75 6d62 6572 2e67 6574 2822 636f  t_number.get("co
+00009a30: 756e 7422 2c20 3129 0a20 2020 2020 2020  unt", 1).       
+00009a40: 2073 656c 662e 7072 6566 5b22 636f 6e74   self.pref["cont
+00009a50: 6573 7422 5d20 3d20 6e65 7874 5f6e 756d  est"] = next_num
+00009a60: 6265 722e 6765 7428 2263 6f75 6e74 222c  ber.get("count",
+00009a70: 2031 290a 2020 2020 2020 2020 2320 636f   1).        # co
+00009a80: 6e74 6573 745b 2753 7562 5479 7065 275d  ntest['SubType']
+00009a90: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00009aa0: 6469 616c 6f67 2e0a 2020 2020 2020 2020  dialog..        
+00009ab0: 636f 6e74 6573 745b 2253 7461 7469 6f6e  contest["Station
+00009ac0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+00009ad0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00009ae0: 2e73 7461 7469 6f6e 2e63 7572 7265 6e74  .station.current
+00009af0: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+00009b00: 6f6e 7465 7374 5b22 4173 7369 7374 6564  ontest["Assisted
+00009b10: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+00009b20: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00009b30: 2e61 7373 6973 7465 642e 6375 7272 656e  .assisted.curren
+00009b40: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
+00009b50: 636f 6e74 6573 745b 2254 7261 6e73 6d69  contest["Transmi
+00009b60: 7474 6572 4361 7465 676f 7279 225d 203d  tterCategory"] =
+00009b70: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00009b80: 616c 6f67 2e74 7261 6e73 6d69 7474 6572  alog.transmitter
+00009b90: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+00009ba0: 2020 2020 2020 2023 2063 6f6e 7465 7374         # contest
+00009bb0: 5b27 5469 6d65 4361 7465 676f 7279 275d  ['TimeCategory']
+00009bc0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00009bd0: 6469 616c 6f67 2e0a 2020 2020 2020 2020  dialog..        
+00009be0: 6c6f 6767 6572 2e64 6562 7567 2822 2573  logger.debug("%s
+00009bf0: 222c 2066 227b 636f 6e74 6573 747d 2229  ", f"{contest}")
+00009c00: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
+00009c10: 7461 6261 7365 2e61 6464 5f63 6f6e 7465  tabase.add_conte
+00009c20: 7374 2863 6f6e 7465 7374 290a 2020 2020  st(contest).    
+00009c30: 2020 2020 7365 6c66 2e77 7269 7465 5f70      self.write_p
+00009c40: 7265 6665 7265 6e63 6528 290a 2020 2020  reference().    
+00009c50: 2020 2020 7365 6c66 2e6c 6f61 645f 636f      self.load_co
+00009c60: 6e74 6573 7428 290a 0a20 2020 2064 6566  ntest()..    def
+00009c70: 2065 6469 745f 7374 6174 696f 6e5f 7365   edit_station_se
+00009c80: 7474 696e 6773 2873 656c 6629 3a0a 2020  ttings(self):.  
+00009c90: 2020 2020 2020 2222 2253 686f 7720 7365        """Show se
+00009ca0: 7474 696e 6773 2064 6961 6c6f 6722 2222  ttings dialog"""
+00009cb0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00009cc0: 6465 6275 6728 2253 7461 7469 6f6e 2053  debug("Station S
+00009cd0: 6574 7469 6e67 7320 7365 6c65 6374 6564  ettings selected
+00009ce0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00009cf0: 7365 7474 696e 6773 5f64 6961 6c6f 6720  settings_dialog 
+00009d00: 3d20 4564 6974 5374 6174 696f 6e28 574f  = EditStation(WO
+00009d10: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
+00009d20: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+00009d30: 735f 6469 616c 6f67 2e61 6363 6570 7465  s_dialog.accepte
+00009d40: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
+00009d50: 6176 655f 7365 7474 696e 6773 290a 2020  ave_settings).  
+00009d60: 2020 2020 2020 2320 6966 2073 656c 662e        # if self.
+00009d70: 7072 6566 2e67 6574 2822 6461 726b 5f6d  pref.get("dark_m
+00009d80: 6f64 6522 293a 0a20 2020 2020 2020 2023  ode"):.        #
+00009d90: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
+00009da0: 6773 5f64 6961 6c6f 672e 7365 7453 7479  gs_dialog.setSty
+00009db0: 6c65 5368 6565 7428 4441 524b 5f53 5459  leSheet(DARK_STY
+00009dc0: 4c45 5348 4545 5429 0a0a 2020 2020 2020  LESHEET)..      
+00009dd0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+00009de0: 6469 616c 6f67 2e43 616c 6c2e 7365 7454  dialog.Call.setT
+00009df0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+00009e00: 2e67 6574 2822 4361 6c6c 222c 2022 2229  .get("Call", "")
+00009e10: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00009e20: 6574 7469 6e67 735f 6469 616c 6f67 2e4e  ettings_dialog.N
+00009e30: 616d 652e 7365 7454 6578 7428 7365 6c66  ame.setText(self
+00009e40: 2e73 7461 7469 6f6e 2e67 6574 2822 4e61  .station.get("Na
+00009e50: 6d65 222c 2022 2229 290a 2020 2020 2020  me", "")).      
+00009e60: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+00009e70: 6469 616c 6f67 2e41 6464 7265 7373 312e  dialog.Address1.
+00009e80: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
+00009e90: 7469 6f6e 2e67 6574 2822 5374 7265 6574  tion.get("Street
+00009ea0: 3122 2c20 2222 2929 0a20 2020 2020 2020  1", "")).       
+00009eb0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+00009ec0: 6961 6c6f 672e 4164 6472 6573 7332 2e73  ialog.Address2.s
+00009ed0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+00009ee0: 696f 6e2e 6765 7428 2253 7472 6565 7432  ion.get("Street2
+00009ef0: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+00009f00: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+00009f10: 616c 6f67 2e43 6974 792e 7365 7454 6578  alog.City.setTex
+00009f20: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
+00009f30: 6574 2822 4369 7479 222c 2022 2229 290a  et("City", "")).
+00009f40: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00009f50: 7469 6e67 735f 6469 616c 6f67 2e53 7461  tings_dialog.Sta
+00009f60: 7465 2e73 6574 5465 7874 2873 656c 662e  te.setText(self.
+00009f70: 7374 6174 696f 6e2e 6765 7428 2253 7461  station.get("Sta
+00009f80: 7465 222c 2022 2229 290a 2020 2020 2020  te", "")).      
+00009f90: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+00009fa0: 6469 616c 6f67 2e5a 6970 2e73 6574 5465  dialog.Zip.setTe
+00009fb0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+00009fc0: 6765 7428 225a 6970 222c 2022 2229 290a  get("Zip", "")).
+00009fd0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00009fe0: 7469 6e67 735f 6469 616c 6f67 2e43 6f75  tings_dialog.Cou
+00009ff0: 6e74 7279 2e73 6574 5465 7874 2873 656c  ntry.setText(sel
+0000a000: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
+0000a010: 6f75 6e74 7279 222c 2022 2229 290a 2020  ountry", "")).  
+0000a020: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000a030: 6e67 735f 6469 616c 6f67 2e47 7269 6453  ngs_dialog.GridS
+0000a040: 7175 6172 652e 7365 7454 6578 7428 7365  quare.setText(se
+0000a050: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000a060: 4772 6964 5371 7561 7265 222c 2022 2229  GridSquare", "")
+0000a070: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a080: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+0000a090: 515a 6f6e 652e 7365 7454 6578 7428 7374  QZone.setText(st
+0000a0a0: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
+0000a0b0: 6574 2822 4351 5a6f 6e65 222c 2022 2229  et("CQZone", "")
+0000a0c0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000a0d0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000a0e0: 4954 555a 6f6e 652e 7365 7454 6578 7428  ITUZone.setText(
+0000a0f0: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
+0000a100: 2e67 6574 2822 4941 5255 5a6f 6e65 222c  .get("IARUZone",
+0000a110: 2022 2229 2929 0a20 2020 2020 2020 2073   ""))).        s
+0000a120: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000a130: 6c6f 672e 4c69 6365 6e73 652e 7365 7454  log.License.setT
+0000a140: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000a150: 2e67 6574 2822 4c69 6365 6e73 6543 6c61  .get("LicenseCla
+0000a160: 7373 222c 2022 2229 290a 2020 2020 2020  ss", "")).      
+0000a170: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a180: 6469 616c 6f67 2e4c 6174 6974 7564 652e  dialog.Latitude.
+0000a190: 7365 7454 6578 7428 7374 7228 7365 6c66  setText(str(self
+0000a1a0: 2e73 7461 7469 6f6e 2e67 6574 2822 4c61  .station.get("La
+0000a1b0: 7469 7475 6465 222c 2022 2229 2929 0a20  titude", ""))). 
+0000a1c0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
+0000a1d0: 696e 6773 5f64 6961 6c6f 672e 4c6f 6e67  ings_dialog.Long
+0000a1e0: 6974 7564 652e 7365 7454 6578 7428 7374  itude.setText(st
+0000a1f0: 7228 7365 6c66 2e73 7461 7469 6f6e 2e67  r(self.station.g
+0000a200: 6574 2822 4c6f 6e67 6974 7564 6522 2c20  et("Longitude", 
+0000a210: 2222 2929 290a 2020 2020 2020 2020 7365  ""))).        se
+0000a220: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000a230: 6f67 2e53 7461 7469 6f6e 5458 5258 2e73  og.StationTXRX.s
+0000a240: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000a250: 696f 6e2e 6765 7428 2273 7461 7469 6f6e  ion.get("station
+0000a260: 7478 7278 222c 2022 2229 290a 2020 2020  txrx", "")).    
+0000a270: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000a280: 735f 6469 616c 6f67 2e50 6f77 6572 2e73  s_dialog.Power.s
+0000a290: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
+0000a2a0: 696f 6e2e 6765 7428 2253 506f 7765 222c  ion.get("SPowe",
+0000a2b0: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
+0000a2c0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000a2d0: 6f67 2e41 6e74 656e 6e61 2e73 6574 5465  og.Antenna.setTe
+0000a2e0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000a2f0: 6765 7428 2253 416e 7465 222c 2022 2229  get("SAnte", "")
+0000a300: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a310: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000a320: 6e74 4865 6967 6874 2e73 6574 5465 7874  ntHeight.setText
+0000a330: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
+0000a340: 7428 2253 416e 7448 3122 2c20 2222 2929  t("SAntH1", ""))
+0000a350: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000a360: 7474 696e 6773 5f64 6961 6c6f 672e 4153  ttings_dialog.AS
+0000a370: 4c2e 7365 7454 6578 7428 7365 6c66 2e73  L.setText(self.s
+0000a380: 7461 7469 6f6e 2e67 6574 2822 5341 6e74  tation.get("SAnt
+0000a390: 4832 222c 2022 2229 290a 2020 2020 2020  H2", "")).      
+0000a3a0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000a3b0: 6469 616c 6f67 2e41 5252 4c53 6563 7469  dialog.ARRLSecti
+0000a3c0: 6f6e 2e73 6574 5465 7874 2873 656c 662e  on.setText(self.
+0000a3d0: 7374 6174 696f 6e2e 6765 7428 2241 5252  station.get("ARR
+0000a3e0: 4c53 6563 7469 6f6e 222c 2022 2229 290a  LSection", "")).
+0000a3f0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a400: 7469 6e67 735f 6469 616c 6f67 2e52 6f76  tings_dialog.Rov
+0000a410: 6572 5154 482e 7365 7454 6578 7428 7365  erQTH.setText(se
+0000a420: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000a430: 526f 7665 7251 5448 222c 2022 2229 290a  RoverQTH", "")).
+0000a440: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000a450: 7469 6e67 735f 6469 616c 6f67 2e43 6c75  tings_dialog.Clu
+0000a460: 622e 7365 7454 6578 7428 7365 6c66 2e73  b.setText(self.s
+0000a470: 7461 7469 6f6e 2e67 6574 2822 436c 7562  tation.get("Club
+0000a480: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000a490: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000a4a0: 616c 6f67 2e45 6d61 696c 2e73 6574 5465  alog.Email.setTe
+0000a4b0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000a4c0: 6765 7428 2245 6d61 696c 222c 2022 2229  get("Email", "")
+0000a4d0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a4e0: 6574 7469 6e67 735f 6469 616c 6f67 2e6f  ettings_dialog.o
+0000a4f0: 7065 6e28 290a 0a20 2020 2064 6566 2073  pen()..    def s
+0000a500: 6176 655f 7365 7474 696e 6773 2873 656c  ave_settings(sel
+0000a510: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
+0000a520: 6176 6520 7365 7474 696e 6773 2222 220a  ave settings""".
+0000a530: 2020 2020 2020 2020 6373 203d 2073 656c          cs = sel
+0000a540: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000a550: 672e 4361 6c6c 2e74 6578 7428 290a 2020  g.Call.text().  
+0000a560: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000a570: 6f6e 203d 207b 7d0a 2020 2020 2020 2020  on = {}.        
+0000a580: 7365 6c66 2e73 7461 7469 6f6e 5b22 4361  self.station["Ca
+0000a590: 6c6c 225d 203d 2063 732e 7570 7065 7228  ll"] = cs.upper(
+0000a5a0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a5b0: 7461 7469 6f6e 5b22 4e61 6d65 225d 203d  tation["Name"] =
+0000a5c0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000a5d0: 6961 6c6f 672e 4e61 6d65 2e74 6578 7428  ialog.Name.text(
+0000a5e0: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+0000a5f0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000a600: 5374 7265 6574 3122 5d20 3d20 7365 6c66  Street1"] = self
+0000a610: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000a620: 2e41 6464 7265 7373 312e 7465 7874 2829  .Address1.text()
+0000a630: 2e74 6974 6c65 2829 0a20 2020 2020 2020  .title().       
+0000a640: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
+0000a650: 7472 6565 7432 225d 203d 2073 656c 662e  treet2"] = self.
+0000a660: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000a670: 4164 6472 6573 7332 2e74 6578 7428 292e  Address2.text().
+0000a680: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
+0000a690: 7365 6c66 2e73 7461 7469 6f6e 5b22 4369  self.station["Ci
+0000a6a0: 7479 225d 203d 2073 656c 662e 7365 7474  ty"] = self.sett
+0000a6b0: 696e 6773 5f64 6961 6c6f 672e 4369 7479  ings_dialog.City
+0000a6c0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
 0000a6d0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000a6e0: 7469 6f6e 5b22 4351 5a6f 6e65 225d 203d  tion["CQZone"] =
-0000a6f0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000a700: 6961 6c6f 672e 4351 5a6f 6e65 2e74 6578  ialog.CQZone.tex
-0000a710: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-0000a720: 2e73 7461 7469 6f6e 5b22 4941 5255 5a6f  .station["IARUZo
-0000a730: 6e65 225d 203d 2073 656c 662e 7365 7474  ne"] = self.sett
-0000a740: 696e 6773 5f64 6961 6c6f 672e 4954 555a  ings_dialog.ITUZ
-0000a750: 6f6e 652e 7465 7874 2829 0a20 2020 2020  one.text().     
-0000a760: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000a770: 224c 6963 656e 7365 436c 6173 7322 5d20  "LicenseClass"] 
-0000a780: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000a790: 6469 616c 6f67 2e4c 6963 656e 7365 2e74  dialog.License.t
-0000a7a0: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
-0000a7b0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000a7c0: 6f6e 5b22 4c61 7469 7475 6465 225d 203d  on["Latitude"] =
-0000a7d0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000a7e0: 6961 6c6f 672e 4c61 7469 7475 6465 2e74  ialog.Latitude.t
-0000a7f0: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000a800: 6c66 2e73 7461 7469 6f6e 5b22 4c6f 6e67  lf.station["Long
-0000a810: 6974 7564 6522 5d20 3d20 7365 6c66 2e73  itude"] = self.s
-0000a820: 6574 7469 6e67 735f 6469 616c 6f67 2e4c  ettings_dialog.L
-0000a830: 6f6e 6769 7475 6465 2e74 6578 7428 290a  ongitude.text().
-0000a840: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0000a850: 7469 6f6e 5b22 5354 5865 7122 5d20 3d20  tion["STXeq"] = 
-0000a860: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000a870: 616c 6f67 2e53 7461 7469 6f6e 5458 5258  alog.StationTXRX
-0000a880: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000a890: 7365 6c66 2e73 7461 7469 6f6e 5b22 5350  self.station["SP
-0000a8a0: 6f77 6522 5d20 3d20 7365 6c66 2e73 6574  owe"] = self.set
-0000a8b0: 7469 6e67 735f 6469 616c 6f67 2e50 6f77  tings_dialog.Pow
-0000a8c0: 6572 2e74 6578 7428 290a 2020 2020 2020  er.text().      
-0000a8d0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
-0000a8e0: 5341 6e74 6522 5d20 3d20 7365 6c66 2e73  SAnte"] = self.s
-0000a8f0: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
-0000a900: 6e74 656e 6e61 2e74 6578 7428 290a 2020  ntenna.text().  
-0000a910: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000a920: 6f6e 5b22 5341 6e74 4831 225d 203d 2073  on["SAntH1"] = s
-0000a930: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000a940: 6c6f 672e 416e 7448 6569 6768 742e 7465  log.AntHeight.te
-0000a950: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
-0000a960: 662e 7374 6174 696f 6e5b 2253 416e 7448  f.station["SAntH
-0000a970: 3222 5d20 3d20 7365 6c66 2e73 6574 7469  2"] = self.setti
-0000a980: 6e67 735f 6469 616c 6f67 2e41 534c 2e74  ngs_dialog.ASL.t
-0000a990: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
-0000a9a0: 6c66 2e73 7461 7469 6f6e 5b22 4152 524c  lf.station["ARRL
-0000a9b0: 5365 6374 696f 6e22 5d20 3d20 7365 6c66  Section"] = self
-0000a9c0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000a9d0: 2e41 5252 4c53 6563 7469 6f6e 2e74 6578  .ARRLSection.tex
-0000a9e0: 7428 292e 7570 7065 7228 290a 2020 2020  t().upper().    
+0000a6e0: 7469 6f6e 5b22 5374 6174 6522 5d20 3d20  tion["State"] = 
+0000a6f0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000a700: 616c 6f67 2e53 7461 7465 2e74 6578 7428  alog.State.text(
+0000a710: 292e 7570 7065 7228 290a 2020 2020 2020  ).upper().      
+0000a720: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000a730: 5a69 7022 5d20 3d20 7365 6c66 2e73 6574  Zip"] = self.set
+0000a740: 7469 6e67 735f 6469 616c 6f67 2e5a 6970  tings_dialog.Zip
+0000a750: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000a760: 7365 6c66 2e73 7461 7469 6f6e 5b22 436f  self.station["Co
+0000a770: 756e 7472 7922 5d20 3d20 7365 6c66 2e73  untry"] = self.s
+0000a780: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+0000a790: 6f75 6e74 7279 2e74 6578 7428 292e 7469  ountry.text().ti
+0000a7a0: 746c 6528 290a 2020 2020 2020 2020 7365  tle().        se
+0000a7b0: 6c66 2e73 7461 7469 6f6e 5b22 4772 6964  lf.station["Grid
+0000a7c0: 5371 7561 7265 225d 203d 2073 656c 662e  Square"] = self.
+0000a7d0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000a7e0: 4772 6964 5371 7561 7265 2e74 6578 7428  GridSquare.text(
+0000a7f0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a800: 7461 7469 6f6e 5b22 4351 5a6f 6e65 225d  tation["CQZone"]
+0000a810: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000a820: 5f64 6961 6c6f 672e 4351 5a6f 6e65 2e74  _dialog.CQZone.t
+0000a830: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+0000a840: 6c66 2e73 7461 7469 6f6e 5b22 4941 5255  lf.station["IARU
+0000a850: 5a6f 6e65 225d 203d 2073 656c 662e 7365  Zone"] = self.se
+0000a860: 7474 696e 6773 5f64 6961 6c6f 672e 4954  ttings_dialog.IT
+0000a870: 555a 6f6e 652e 7465 7874 2829 0a20 2020  UZone.text().   
+0000a880: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
+0000a890: 6e5b 224c 6963 656e 7365 436c 6173 7322  n["LicenseClass"
+0000a8a0: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000a8b0: 735f 6469 616c 6f67 2e4c 6963 656e 7365  s_dialog.License
+0000a8c0: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
+0000a8d0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000a8e0: 7469 6f6e 5b22 4c61 7469 7475 6465 225d  tion["Latitude"]
+0000a8f0: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000a900: 5f64 6961 6c6f 672e 4c61 7469 7475 6465  _dialog.Latitude
+0000a910: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000a920: 7365 6c66 2e73 7461 7469 6f6e 5b22 4c6f  self.station["Lo
+0000a930: 6e67 6974 7564 6522 5d20 3d20 7365 6c66  ngitude"] = self
+0000a940: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000a950: 2e4c 6f6e 6769 7475 6465 2e74 6578 7428  .Longitude.text(
+0000a960: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000a970: 7461 7469 6f6e 5b22 5354 5865 7122 5d20  tation["STXeq"] 
+0000a980: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000a990: 6469 616c 6f67 2e53 7461 7469 6f6e 5458  dialog.StationTX
+0000a9a0: 5258 2e74 6578 7428 290a 2020 2020 2020  RX.text().      
+0000a9b0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000a9c0: 5350 6f77 6522 5d20 3d20 7365 6c66 2e73  SPowe"] = self.s
+0000a9d0: 6574 7469 6e67 735f 6469 616c 6f67 2e50  ettings_dialog.P
+0000a9e0: 6f77 6572 2e74 6578 7428 290a 2020 2020  ower.text().    
 0000a9f0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-0000aa00: 5b22 526f 7665 7251 5448 225d 203d 2073  ["RoverQTH"] = s
-0000aa10: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000aa20: 6c6f 672e 526f 7665 7251 5448 2e74 6578  log.RoverQTH.tex
-0000aa30: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-0000aa40: 2e73 7461 7469 6f6e 5b22 436c 7562 225d  .station["Club"]
-0000aa50: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000aa60: 5f64 6961 6c6f 672e 436c 7562 2e74 6578  _dialog.Club.tex
-0000aa70: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
-0000aa80: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-0000aa90: 5b22 456d 6169 6c22 5d20 3d20 7365 6c66  ["Email"] = self
-0000aaa0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000aab0: 2e45 6d61 696c 2e74 6578 7428 290a 2020  .Email.text().  
-0000aac0: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
-0000aad0: 6173 652e 6164 645f 7374 6174 696f 6e28  ase.add_station(
-0000aae0: 7365 6c66 2e73 7461 7469 6f6e 290a 2020  self.station).  
-0000aaf0: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000ab00: 6e67 735f 6469 616c 6f67 2e63 6c6f 7365  ngs_dialog.close
-0000ab10: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000ab20: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d3d  lf.current_op ==
-0000ab30: 2022 223a 0a20 2020 2020 2020 2020 2020   "":.           
-0000ab40: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-0000ab50: 203d 2073 656c 662e 7374 6174 696f 6e2e   = self.station.
-0000ab60: 6765 7428 2243 616c 6c22 2c20 2222 290a  get("Call", "").
-0000ab70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ab80: 2e6d 616b 655f 6f70 5f64 6972 2829 0a20  .make_op_dir(). 
-0000ab90: 2020 2020 2020 2063 6f6e 7465 7374 5f63         contest_c
-0000aba0: 6f75 6e74 203d 2073 656c 662e 6461 7461  ount = self.data
-0000abb0: 6261 7365 2e66 6574 6368 5f61 6c6c 5f63  base.fetch_all_c
-0000abc0: 6f6e 7465 7374 7328 290a 2020 2020 2020  ontests().      
-0000abd0: 2020 6966 206c 656e 2863 6f6e 7465 7374    if len(contest
-0000abe0: 5f63 6f75 6e74 2920 3d3d 2030 3a0a 2020  _count) == 0:.  
-0000abf0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000ac00: 6577 5f63 6f6e 7465 7374 5f64 6961 6c6f  ew_contest_dialo
-0000ac10: 6728 290a 0a20 2020 2064 6566 2065 6469  g()..    def edi
-0000ac20: 745f 6d61 6372 6f28 7365 6c66 2c20 6675  t_macro(self, fu
-0000ac30: 6e63 7469 6f6e 5f6b 6579 293a 0a20 2020  nction_key):.   
-0000ac40: 2020 2020 2022 2222 5368 6f77 2065 6469       """Show edi
-0000ac50: 7420 6d61 6372 6f20 6469 616c 6f67 2222  t macro dialog""
-0000ac60: 220a 2020 2020 2020 2020 7365 6c66 2e65  ".        self.e
-0000ac70: 6469 745f 6d61 6372 6f5f 6469 616c 6f67  dit_macro_dialog
-0000ac80: 203d 2045 6469 744d 6163 726f 2866 756e   = EditMacro(fun
-0000ac90: 6374 696f 6e5f 6b65 792c 2057 4f52 4b49  ction_key, WORKI
-0000aca0: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
-0000acb0: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000acc0: 5f64 6961 6c6f 672e 6163 6365 7074 6564  _dialog.accepted
-0000acd0: 2e63 6f6e 6e65 6374 2873 656c 662e 6564  .connect(self.ed
-0000ace0: 6974 6564 5f6d 6163 726f 290a 2020 2020  ited_macro).    
-0000acf0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-0000ad00: 2e67 6574 2822 6461 726b 5f6d 6f64 6522  .get("dark_mode"
-0000ad10: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000ad20: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
-0000ad30: 6961 6c6f 672e 7365 7453 7479 6c65 5368  ialog.setStyleSh
-0000ad40: 6565 7428 4441 524b 5f53 5459 4c45 5348  eet(DARK_STYLESH
-0000ad50: 4545 5429 0a20 2020 2020 2020 2073 656c  EET).        sel
-0000ad60: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
-0000ad70: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
-0000ad80: 6465 6620 6564 6974 6564 5f6d 6163 726f  def edited_macro
-0000ad90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000ada0: 2222 2253 6176 6520 6564 6974 6564 206d  """Save edited m
-0000adb0: 6163 726f 2222 220a 2020 2020 2020 2020  acro""".        
-0000adc0: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
-0000add0: 6469 616c 6f67 2e66 756e 6374 696f 6e5f  dialog.function_
-0000ade0: 6b65 792e 7365 7454 6578 7428 0a20 2020  key.setText(.   
-0000adf0: 2020 2020 2020 2020 2073 656c 662e 6564           self.ed
-0000ae00: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
-0000ae10: 6d61 6372 6f5f 6c61 6265 6c2e 7465 7874  macro_label.text
-0000ae20: 2829 0a20 2020 2020 2020 2029 0a20 2020  ().        ).   
-0000ae30: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000ae40: 6163 726f 5f64 6961 6c6f 672e 6675 6e63  acro_dialog.func
-0000ae50: 7469 6f6e 5f6b 6579 2e73 6574 546f 6f6c  tion_key.setTool
-0000ae60: 5469 7028 0a20 2020 2020 2020 2020 2020  Tip(.           
-0000ae70: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000ae80: 5f64 6961 6c6f 672e 7468 655f 6d61 6372  _dialog.the_macr
-0000ae90: 6f2e 7465 7874 2829 0a20 2020 2020 2020  o.text().       
-0000aea0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-0000aeb0: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
-0000aec0: 672e 636c 6f73 6528 290a 0a20 2020 2064  g.close()..    d
-0000aed0: 6566 2065 6469 745f 4631 2873 656c 6629  ef edit_F1(self)
-0000aee0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000aef0: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000af00: 6765 722e 6465 6275 6728 2246 3120 5269  ger.debug("F1 Ri
-0000af10: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000af20: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000af30: 5f6d 6163 726f 2873 656c 662e 4631 290a  _macro(self.F1).
-0000af40: 0a20 2020 2064 6566 2065 6469 745f 4632  .    def edit_F2
-0000af50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000af60: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000af70: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000af80: 2246 3220 5269 6768 7420 436c 6963 6b65  "F2 Right Clicke
-0000af90: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
-0000afa0: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
-0000afb0: 662e 4632 290a 0a20 2020 2064 6566 2065  f.F2)..    def e
-0000afc0: 6469 745f 4633 2873 656c 6629 3a0a 2020  dit_F3(self):.  
-0000afd0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000afe0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000aff0: 6465 6275 6728 2246 3320 5269 6768 7420  debug("F3 Right 
-0000b000: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000b010: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000b020: 726f 2873 656c 662e 4633 290a 0a20 2020  ro(self.F3)..   
-0000b030: 2064 6566 2065 6469 745f 4634 2873 656c   def edit_F4(sel
-0000b040: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000b050: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000b060: 6f67 6765 722e 6465 6275 6728 2246 3420  ogger.debug("F4 
-0000b070: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000b080: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000b090: 6974 5f6d 6163 726f 2873 656c 662e 4634  it_macro(self.F4
-0000b0a0: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000b0b0: 4635 2873 656c 6629 3a0a 2020 2020 2020  F5(self):.      
-0000b0c0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000b0d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000b0e0: 6728 2246 3520 5269 6768 7420 436c 6963  g("F5 Right Clic
-0000b0f0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000b100: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000b110: 656c 662e 4635 290a 0a20 2020 2064 6566  elf.F5)..    def
-0000b120: 2065 6469 745f 4636 2873 656c 6629 3a0a   edit_F6(self):.
-0000b130: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000b140: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000b150: 722e 6465 6275 6728 2246 3620 5269 6768  r.debug("F6 Righ
-0000b160: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000b170: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000b180: 6163 726f 2873 656c 662e 4636 290a 0a20  acro(self.F6).. 
-0000b190: 2020 2064 6566 2065 6469 745f 4637 2873     def edit_F7(s
-0000b1a0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000b1b0: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000b1c0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000b1d0: 3720 5269 6768 7420 436c 6963 6b65 642e  7 Right Clicked.
-0000b1e0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000b1f0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000b200: 4637 290a 0a20 2020 2064 6566 2065 6469  F7)..    def edi
-0000b210: 745f 4638 2873 656c 6629 3a0a 2020 2020  t_F8(self):.    
-0000b220: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000b230: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000b240: 6275 6728 2246 3820 5269 6768 7420 436c  bug("F8 Right Cl
-0000b250: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000b260: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b270: 2873 656c 662e 4638 290a 0a20 2020 2064  (self.F8)..    d
-0000b280: 6566 2065 6469 745f 4639 2873 656c 6629  ef edit_F9(self)
-0000b290: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000b2a0: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000b2b0: 6765 722e 6465 6275 6728 2246 3920 5269  ger.debug("F9 Ri
-0000b2c0: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000b2d0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000b2e0: 5f6d 6163 726f 2873 656c 662e 4639 290a  _macro(self.F9).
-0000b2f0: 0a20 2020 2064 6566 2065 6469 745f 4631  .    def edit_F1
-0000b300: 3028 7365 6c66 293a 0a20 2020 2020 2020  0(self):.       
-0000b310: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000b320: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000b330: 2822 4631 3020 5269 6768 7420 436c 6963  ("F10 Right Clic
-0000b340: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000b350: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000b360: 656c 662e 4631 3029 0a0a 2020 2020 6465  elf.F10)..    de
-0000b370: 6620 6564 6974 5f46 3131 2873 656c 6629  f edit_F11(self)
-0000b380: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000b390: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000b3a0: 6765 722e 6465 6275 6728 2246 3131 2052  ger.debug("F11 R
-0000b3b0: 6967 6874 2043 6c69 636b 6564 2e22 290a  ight Clicked.").
-0000b3c0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-0000b3d0: 745f 6d61 6372 6f28 7365 6c66 2e46 3131  t_macro(self.F11
-0000b3e0: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000b3f0: 4631 3228 7365 6c66 293a 0a20 2020 2020  F12(self):.     
-0000b400: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
-0000b410: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000b420: 7567 2822 4631 3220 5269 6768 7420 436c  ug("F12 Right Cl
-0000b430: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000b440: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000b450: 2873 656c 662e 4631 3229 0a0a 2020 2020  (self.F12)..    
-0000b460: 6465 6620 7072 6f63 6573 735f 6d61 6372  def process_macr
-0000b470: 6f28 7365 6c66 2c20 6d61 6372 6f3a 2073  o(self, macro: s
-0000b480: 7472 2920 2d3e 2073 7472 3a0a 2020 2020  tr) -> str:.    
-0000b490: 2020 2020 2222 2250 726f 6365 7373 2043      """Process C
-0000b4a0: 5720 6d61 6372 6f20 7375 6273 7469 7475  W macro substitu
-0000b4b0: 7469 6f6e 7322 2222 0a20 2020 2020 2020  tions""".       
-0000b4c0: 2072 6573 756c 7420 3d20 7365 6c66 2e64   result = self.d
-0000b4d0: 6174 6162 6173 652e 6765 745f 7365 7269  atabase.get_seri
-0000b4e0: 616c 2829 0a20 2020 2020 2020 2070 7269  al().        pri
-0000b4f0: 6e74 2872 6573 756c 7429 0a20 2020 2020  nt(result).     
-0000b500: 2020 206e 6578 745f 7365 7269 616c 203d     next_serial =
-0000b510: 2073 7472 2872 6573 756c 742e 6765 7428   str(result.get(
-0000b520: 2273 6572 6961 6c5f 6e72 222c 2022 3122  "serial_nr", "1"
-0000b530: 2929 0a20 2020 2020 2020 2069 6620 6e65  )).        if ne
-0000b540: 7874 5f73 6572 6961 6c20 3d3d 2022 4e6f  xt_serial == "No
-0000b550: 6e65 223a 0a20 2020 2020 2020 2020 2020  ne":.           
-0000b560: 206e 6578 745f 7365 7269 616c 203d 2022   next_serial = "
-0000b570: 3122 0a20 2020 2020 2020 2070 7269 6e74  1".        print
-0000b580: 286e 6578 745f 7365 7269 616c 290a 2020  (next_serial).  
-0000b590: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
-0000b5a0: 6372 6f2e 7570 7065 7228 290a 2020 2020  cro.upper().    
-0000b5b0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
-0000b5c0: 6f2e 7265 706c 6163 6528 2223 222c 206e  o.replace("#", n
-0000b5d0: 6578 745f 7365 7269 616c 290a 2020 2020  ext_serial).    
-0000b5e0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
-0000b5f0: 6f2e 7265 706c 6163 6528 227b 4d59 4341  o.replace("{MYCA
-0000b600: 4c4c 7d22 2c20 7365 6c66 2e73 7461 7469  LL}", self.stati
-0000b610: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
-0000b620: 2229 290a 2020 2020 2020 2020 6d61 6372  ")).        macr
-0000b630: 6f20 3d20 6d61 6372 6f2e 7265 706c 6163  o = macro.replac
-0000b640: 6528 227b 4849 5343 414c 4c7d 222c 2073  e("{HISCALL}", s
-0000b650: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
-0000b660: 7428 2929 0a20 2020 2020 2020 2069 6620  t()).        if 
-0000b670: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000b680: 2e67 6574 2822 6d6f 6465 2229 203d 3d20  .get("mode") == 
-0000b690: 2243 5722 3a0a 2020 2020 2020 2020 2020  "CW":.          
-0000b6a0: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
-0000b6b0: 7265 706c 6163 6528 227b 534e 547d 222c  replace("{SNT}",
-0000b6c0: 2073 656c 662e 7365 6e74 2e74 6578 7428   self.sent.text(
-0000b6d0: 292e 7265 706c 6163 6528 2239 222c 2022  ).replace("9", "
-0000b6e0: 6e22 2929 0a20 2020 2020 2020 2065 6c73  n")).        els
-0000b6f0: 653a 0a20 2020 2020 2020 2020 2020 206d  e:.            m
-0000b700: 6163 726f 203d 206d 6163 726f 2e72 6570  acro = macro.rep
-0000b710: 6c61 6365 2822 7b53 4e54 7d22 2c20 7365  lace("{SNT}", se
-0000b720: 6c66 2e73 656e 742e 7465 7874 2829 290a  lf.sent.text()).
-0000b730: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
-0000b740: 6d61 6372 6f2e 7265 706c 6163 6528 227b  macro.replace("{
-0000b750: 5345 4e54 4e52 7d22 2c20 7365 6c66 2e6f  SENTNR}", self.o
-0000b760: 7468 6572 5f31 2e74 6578 7428 2929 0a20  ther_1.text()). 
-0000b770: 2020 2020 2020 206d 6163 726f 203d 206d         macro = m
-0000b780: 6163 726f 2e72 6570 6c61 6365 280a 2020  acro.replace(.  
-0000b790: 2020 2020 2020 2020 2020 227b 4558 4348            "{EXCH
-0000b7a0: 7d22 2c20 7365 6c66 2e63 6f6e 7465 7374  }", self.contest
-0000b7b0: 5f73 6574 7469 6e67 732e 6765 7428 2253  _settings.get("S
-0000b7c0: 656e 7445 7863 6861 6e67 6522 2c20 2278  entExchange", "x
-0000b7d0: 7878 2229 0a20 2020 2020 2020 2029 0a20  xx").        ). 
-0000b7e0: 2020 2020 2020 2072 6574 7572 6e20 6d61         return ma
-0000b7f0: 6372 6f0a 0a20 2020 2064 6566 2076 6f69  cro..    def voi
-0000b800: 6365 5f73 7472 696e 6728 7365 6c66 2c20  ce_string(self, 
-0000b810: 7468 655f 7374 7269 6e67 3a20 7374 7229  the_string: str)
-0000b820: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-0000b830: 2020 2222 2276 6f69 6365 7320 7374 7269    """voices stri
-0000b840: 6e67 2075 7369 6e67 206e 6174 6f20 7068  ng using nato ph
-0000b850: 6f6e 6574 6963 7322 2222 0a20 2020 2020  onetics""".     
-0000b860: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000b870: 2256 6f69 6369 6e67 3a20 2573 222c 2074  "Voicing: %s", t
-0000b880: 6865 5f73 7472 696e 6729 0a20 2020 2020  he_string).     
-0000b890: 2020 206f 705f 7061 7468 203d 2050 6174     op_path = Pat
-0000b8a0: 6828 4441 5441 5f50 4154 4829 202f 2073  h(DATA_PATH) / s
-0000b8b0: 656c 662e 6375 7272 656e 745f 6f70 0a20  elf.current_op. 
-0000b8c0: 2020 2020 2020 2069 6620 225b 2220 696e         if "[" in
-0000b8d0: 2074 6865 5f73 7472 696e 673a 0a20 2020   the_string:.   
-0000b8e0: 2020 2020 2020 2020 2073 7562 5f73 7472           sub_str
-0000b8f0: 696e 6720 3d20 7468 655f 7374 7269 6e67  ing = the_string
-0000b900: 2e73 7472 6970 2822 5b5d 2229 2e6c 6f77  .strip("[]").low
-0000b910: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-0000b920: 2066 696c 656e 616d 6520 3d20 6622 7b73   filename = f"{s
-0000b930: 7472 286f 705f 7061 7468 297d 2f7b 7375  tr(op_path)}/{su
-0000b940: 625f 7374 7269 6e67 7d2e 7761 7622 0a20  b_string}.wav". 
-0000b950: 2020 2020 2020 2020 2020 2069 6620 5061             if Pa
-0000b960: 7468 2866 696c 656e 616d 6529 2e69 735f  th(filename).is_
-0000b970: 6669 6c65 2829 3a0a 2020 2020 2020 2020  file():.        
-0000b980: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000b990: 6562 7567 2822 566f 6963 696e 673a 2025  ebug("Voicing: %
-0000b9a0: 7322 2c20 6669 6c65 6e61 6d65 290a 2020  s", filename).  
-0000b9b0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000b9c0: 7461 2c20 5f66 7320 3d20 7366 2e72 6561  ta, _fs = sf.rea
-0000b9d0: 6428 6669 6c65 6e61 6d65 2c20 6474 7970  d(filename, dtyp
-0000b9e0: 653d 2266 6c6f 6174 3332 2229 0a20 2020  e="float32").   
-0000b9f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ba00: 662e 7074 745f 6f6e 2829 0a20 2020 2020  f.ptt_on().     
-0000ba10: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2020 2020 7364 2e64 6566 6175 6c74 2e64      sd.default.d
-0000ba40: 6576 6963 6520 3d20 7365 6c66 2e70 7265  evice = self.pre
-0000ba50: 662e 6765 7428 2273 6f75 6e64 6465 7669  f.get("sounddevi
-0000ba60: 6365 222c 2022 6465 6661 756c 7422 290a  ce", "default").
-0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba80: 2020 2020 7364 2e64 6566 6175 6c74 2e73      sd.default.s
-0000ba90: 616d 706c 6572 6174 6520 3d20 3434 3130  amplerate = 4410
-0000baa0: 302e 300a 2020 2020 2020 2020 2020 2020  0.0.            
-0000bab0: 2020 2020 2020 2020 7364 2e70 6c61 7928          sd.play(
-0000bac0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-0000bad0: 2020 2020 2020 2020 2020 5f73 7461 7475            _statu
-0000bae0: 7320 3d20 7364 2e77 6169 7428 290a 2020  s = sd.wait().  
-0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb00: 2020 2320 6874 7470 733a 2f2f 736e 796b    # https://snyk
-0000bb10: 2e69 6f2f 6164 7669 736f 722f 7079 7468  .io/advisor/pyth
-0000bb20: 6f6e 2f73 6f75 6e64 6465 7669 6365 2f66  on/sounddevice/f
-0000bb30: 756e 6374 696f 6e73 2f73 6f75 6e64 6465  unctions/soundde
-0000bb40: 7669 6365 2e50 6f72 7441 7564 696f 4572  vice.PortAudioEr
-0000bb50: 726f 720a 2020 2020 2020 2020 2020 2020  ror.            
-0000bb60: 2020 2020 6578 6365 7074 2073 642e 506f      except sd.Po
-0000bb70: 7274 4175 6469 6f45 7272 6f72 2061 7320  rtAudioError as 
-0000bb80: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
-0000bb90: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000bba0: 6465 6275 6728 2225 7322 2c20 6622 7b65  debug("%s", f"{e
-0000bbb0: 7272 7d22 290a 0a20 2020 2020 2020 2020  rr}")..         
-0000bbc0: 2020 2020 2020 2073 656c 662e 7074 745f         self.ptt_
-0000bbd0: 6f66 6628 290a 2020 2020 2020 2020 2020  off().          
-0000bbe0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000bbf0: 2073 656c 662e 7074 745f 6f6e 2829 0a20   self.ptt_on(). 
-0000bc00: 2020 2020 2020 2066 6f72 206c 6574 7465         for lette
-0000bc10: 7220 696e 2074 6865 5f73 7472 696e 672e  r in the_string.
-0000bc20: 6c6f 7765 7228 293a 0a20 2020 2020 2020  lower():.       
-0000bc30: 2020 2020 2069 6620 6c65 7474 6572 2069       if letter i
-0000bc40: 6e20 2261 6263 6465 6667 6869 6a6b 6c6d  n "abcdefghijklm
-0000bc50: 6e6f 7071 7273 7475 7677 7879 7a20 3132  nopqrstuvwxyz 12
-0000bc60: 3334 3536 3738 3930 223a 0a20 2020 2020  34567890":.     
-0000bc70: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-0000bc80: 7474 6572 203d 3d20 2220 223a 0a20 2020  tter == " ":.   
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 206c 6574 7465 7220 3d20 2273 7061 6365   letter = "space
-0000bcb0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000bcc0: 2020 6669 6c65 6e61 6d65 203d 2066 227b    filename = f"{
-0000bcd0: 7374 7228 6f70 5f70 6174 6829 7d2f 7b6c  str(op_path)}/{l
-0000bce0: 6574 7465 727d 2e77 6176 220a 2020 2020  etter}.wav".    
-0000bcf0: 2020 2020 2020 2020 2020 2020 6966 2050              if P
-0000bd00: 6174 6828 6669 6c65 6e61 6d65 292e 6973  ath(filename).is
-0000bd10: 5f66 696c 6528 293a 0a20 2020 2020 2020  _file():.       
-0000bd20: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000bd30: 6765 722e 6465 6275 6728 2256 6f69 6369  ger.debug("Voici
-0000bd40: 6e67 3a20 2573 222c 2066 696c 656e 616d  ng: %s", filenam
-0000bd50: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000bd60: 2020 2020 2020 2064 6174 612c 205f 6673         data, _fs
-0000bd70: 203d 2073 662e 7265 6164 2866 696c 656e   = sf.read(filen
-0000bd80: 616d 652c 2064 7479 7065 3d22 666c 6f61  ame, dtype="floa
-0000bd90: 7433 3222 290a 2020 2020 2020 2020 2020  t32").          
-0000bda0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0000aa00: 5b22 5341 6e74 6522 5d20 3d20 7365 6c66  ["SAnte"] = self
+0000aa10: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000aa20: 2e41 6e74 656e 6e61 2e74 6578 7428 290a  .Antenna.text().
+0000aa30: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000aa40: 7469 6f6e 5b22 5341 6e74 4831 225d 203d  tion["SAntH1"] =
+0000aa50: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000aa60: 6961 6c6f 672e 416e 7448 6569 6768 742e  ialog.AntHeight.
+0000aa70: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
+0000aa80: 656c 662e 7374 6174 696f 6e5b 2253 416e  elf.station["SAn
+0000aa90: 7448 3222 5d20 3d20 7365 6c66 2e73 6574  tH2"] = self.set
+0000aaa0: 7469 6e67 735f 6469 616c 6f67 2e41 534c  tings_dialog.ASL
+0000aab0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000aac0: 7365 6c66 2e73 7461 7469 6f6e 5b22 4152  self.station["AR
+0000aad0: 524c 5365 6374 696f 6e22 5d20 3d20 7365  RLSection"] = se
+0000aae0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000aaf0: 6f67 2e41 5252 4c53 6563 7469 6f6e 2e74  og.ARRLSection.t
+0000ab00: 6578 7428 292e 7570 7065 7228 290a 2020  ext().upper().  
+0000ab10: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000ab20: 6f6e 5b22 526f 7665 7251 5448 225d 203d  on["RoverQTH"] =
+0000ab30: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000ab40: 6961 6c6f 672e 526f 7665 7251 5448 2e74  ialog.RoverQTH.t
+0000ab50: 6578 7428 290a 2020 2020 2020 2020 7365  ext().        se
+0000ab60: 6c66 2e73 7461 7469 6f6e 5b22 436c 7562  lf.station["Club
+0000ab70: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000ab80: 6773 5f64 6961 6c6f 672e 436c 7562 2e74  gs_dialog.Club.t
+0000ab90: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
+0000aba0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000abb0: 6f6e 5b22 456d 6169 6c22 5d20 3d20 7365  on["Email"] = se
+0000abc0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000abd0: 6f67 2e45 6d61 696c 2e74 6578 7428 290a  og.Email.text().
+0000abe0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+0000abf0: 6162 6173 652e 6164 645f 7374 6174 696f  abase.add_statio
+0000ac00: 6e28 7365 6c66 2e73 7461 7469 6f6e 290a  n(self.station).
+0000ac10: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000ac20: 7469 6e67 735f 6469 616c 6f67 2e63 6c6f  tings_dialog.clo
+0000ac30: 7365 2829 0a20 2020 2020 2020 2069 6620  se().        if 
+0000ac40: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
+0000ac50: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
+0000ac60: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
+0000ac70: 6f70 203d 2073 656c 662e 7374 6174 696f  op = self.statio
+0000ac80: 6e2e 6765 7428 2243 616c 6c22 2c20 2222  n.get("Call", ""
+0000ac90: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+0000aca0: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
+0000acb0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+0000acc0: 5f63 6f75 6e74 203d 2073 656c 662e 6461  _count = self.da
+0000acd0: 7461 6261 7365 2e66 6574 6368 5f61 6c6c  tabase.fetch_all
+0000ace0: 5f63 6f6e 7465 7374 7328 290a 2020 2020  _contests().    
+0000acf0: 2020 2020 6966 206c 656e 2863 6f6e 7465      if len(conte
+0000ad00: 7374 5f63 6f75 6e74 2920 3d3d 2030 3a0a  st_count) == 0:.
+0000ad10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ad20: 2e6e 6577 5f63 6f6e 7465 7374 5f64 6961  .new_contest_dia
+0000ad30: 6c6f 6728 290a 0a20 2020 2064 6566 2065  log()..    def e
+0000ad40: 6469 745f 6d61 6372 6f28 7365 6c66 2c20  dit_macro(self, 
+0000ad50: 6675 6e63 7469 6f6e 5f6b 6579 293a 0a20  function_key):. 
+0000ad60: 2020 2020 2020 2022 2222 5368 6f77 2065         """Show e
+0000ad70: 6469 7420 6d61 6372 6f20 6469 616c 6f67  dit macro dialog
+0000ad80: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+0000ad90: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
+0000ada0: 6f67 203d 2045 6469 744d 6163 726f 2866  og = EditMacro(f
+0000adb0: 756e 6374 696f 6e5f 6b65 792c 2057 4f52  unction_key, WOR
+0000adc0: 4b49 4e47 5f50 4154 4829 0a20 2020 2020  KING_PATH).     
+0000add0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000ade0: 726f 5f64 6961 6c6f 672e 6163 6365 7074  ro_dialog.accept
+0000adf0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+0000ae00: 6564 6974 6564 5f6d 6163 726f 290a 2020  edited_macro).  
+0000ae10: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000ae20: 6566 2e67 6574 2822 6461 726b 5f6d 6f64  ef.get("dark_mod
+0000ae30: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
+0000ae40: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
+0000ae50: 5f64 6961 6c6f 672e 7365 7453 7479 6c65  _dialog.setStyle
+0000ae60: 5368 6565 7428 4441 524b 5f53 5459 4c45  Sheet(DARK_STYLE
+0000ae70: 5348 4545 5429 0a20 2020 2020 2020 2073  SHEET).        s
+0000ae80: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
+0000ae90: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
+0000aea0: 2020 6465 6620 6564 6974 6564 5f6d 6163    def edited_mac
+0000aeb0: 726f 2873 656c 6629 3a0a 2020 2020 2020  ro(self):.      
+0000aec0: 2020 2222 2253 6176 6520 6564 6974 6564    """Save edited
+0000aed0: 206d 6163 726f 2222 220a 2020 2020 2020   macro""".      
+0000aee0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000aef0: 6f5f 6469 616c 6f67 2e66 756e 6374 696f  o_dialog.functio
+0000af00: 6e5f 6b65 792e 7365 7454 6578 7428 0a20  n_key.setText(. 
+0000af10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000af20: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
+0000af30: 672e 6d61 6372 6f5f 6c61 6265 6c2e 7465  g.macro_label.te
+0000af40: 7874 2829 0a20 2020 2020 2020 2029 0a20  xt().        ). 
+0000af50: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+0000af60: 5f6d 6163 726f 5f64 6961 6c6f 672e 6675  _macro_dialog.fu
+0000af70: 6e63 7469 6f6e 5f6b 6579 2e73 6574 546f  nction_key.setTo
+0000af80: 6f6c 5469 7028 0a20 2020 2020 2020 2020  olTip(.         
+0000af90: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000afa0: 726f 5f64 6961 6c6f 672e 7468 655f 6d61  ro_dialog.the_ma
+0000afb0: 6372 6f2e 7465 7874 2829 0a20 2020 2020  cro.text().     
+0000afc0: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+0000afd0: 662e 6564 6974 5f6d 6163 726f 5f64 6961  f.edit_macro_dia
+0000afe0: 6c6f 672e 636c 6f73 6528 290a 0a20 2020  log.close()..   
+0000aff0: 2064 6566 2065 6469 745f 4631 2873 656c   def edit_F1(sel
+0000b000: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000b010: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000b020: 6f67 6765 722e 6465 6275 6728 2246 3120  ogger.debug("F1 
+0000b030: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
+0000b040: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+0000b050: 6974 5f6d 6163 726f 2873 656c 662e 4631  it_macro(self.F1
+0000b060: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+0000b070: 4632 2873 656c 6629 3a0a 2020 2020 2020  F2(self):.      
+0000b080: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000b090: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000b0a0: 6728 2246 3220 5269 6768 7420 436c 6963  g("F2 Right Clic
+0000b0b0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
+0000b0c0: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
+0000b0d0: 656c 662e 4632 290a 0a20 2020 2064 6566  elf.F2)..    def
+0000b0e0: 2065 6469 745f 4633 2873 656c 6629 3a0a   edit_F3(self):.
+0000b0f0: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
+0000b100: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+0000b110: 722e 6465 6275 6728 2246 3320 5269 6768  r.debug("F3 Righ
+0000b120: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
+0000b130: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
+0000b140: 6163 726f 2873 656c 662e 4633 290a 0a20  acro(self.F3).. 
+0000b150: 2020 2064 6566 2065 6469 745f 4634 2873     def edit_F4(s
+0000b160: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000b170: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
+0000b180: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000b190: 3420 5269 6768 7420 436c 6963 6b65 642e  4 Right Clicked.
+0000b1a0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000b1b0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
+0000b1c0: 4634 290a 0a20 2020 2064 6566 2065 6469  F4)..    def edi
+0000b1d0: 745f 4635 2873 656c 6629 3a0a 2020 2020  t_F5(self):.    
+0000b1e0: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
+0000b1f0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000b200: 6275 6728 2246 3520 5269 6768 7420 436c  bug("F5 Right Cl
+0000b210: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
+0000b220: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
+0000b230: 2873 656c 662e 4635 290a 0a20 2020 2064  (self.F5)..    d
+0000b240: 6566 2065 6469 745f 4636 2873 656c 6629  ef edit_F6(self)
+0000b250: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
+0000b260: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
+0000b270: 6765 722e 6465 6275 6728 2246 3620 5269  ger.debug("F6 Ri
+0000b280: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
+0000b290: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+0000b2a0: 5f6d 6163 726f 2873 656c 662e 4636 290a  _macro(self.F6).
+0000b2b0: 0a20 2020 2064 6566 2065 6469 745f 4637  .    def edit_F7
+0000b2c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000b2d0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
+0000b2e0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000b2f0: 2246 3720 5269 6768 7420 436c 6963 6b65  "F7 Right Clicke
+0000b300: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
+0000b310: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
+0000b320: 662e 4637 290a 0a20 2020 2064 6566 2065  f.F7)..    def e
+0000b330: 6469 745f 4638 2873 656c 6629 3a0a 2020  dit_F8(self):.  
+0000b340: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000b350: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000b360: 6465 6275 6728 2246 3820 5269 6768 7420  debug("F8 Right 
+0000b370: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
+0000b380: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000b390: 726f 2873 656c 662e 4638 290a 0a20 2020  ro(self.F8)..   
+0000b3a0: 2064 6566 2065 6469 745f 4639 2873 656c   def edit_F9(sel
+0000b3b0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000b3c0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000b3d0: 6f67 6765 722e 6465 6275 6728 2246 3920  ogger.debug("F9 
+0000b3e0: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
+0000b3f0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
+0000b400: 6974 5f6d 6163 726f 2873 656c 662e 4639  it_macro(self.F9
+0000b410: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
+0000b420: 4631 3028 7365 6c66 293a 0a20 2020 2020  F10(self):.     
+0000b430: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000b440: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000b450: 7567 2822 4631 3020 5269 6768 7420 436c  ug("F10 Right Cl
+0000b460: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
+0000b470: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
+0000b480: 2873 656c 662e 4631 3029 0a0a 2020 2020  (self.F10)..    
+0000b490: 6465 6620 6564 6974 5f46 3131 2873 656c  def edit_F11(sel
+0000b4a0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000b4b0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000b4c0: 6f67 6765 722e 6465 6275 6728 2246 3131  ogger.debug("F11
+0000b4d0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000b4e0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000b4f0: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000b500: 3131 290a 0a20 2020 2064 6566 2065 6469  11)..    def edi
+0000b510: 745f 4631 3228 7365 6c66 293a 0a20 2020  t_F12(self):.   
+0000b520: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000b530: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000b540: 6562 7567 2822 4631 3220 5269 6768 7420  ebug("F12 Right 
+0000b550: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
+0000b560: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000b570: 726f 2873 656c 662e 4631 3229 0a0a 2020  ro(self.F12)..  
+0000b580: 2020 6465 6620 7072 6f63 6573 735f 6d61    def process_ma
+0000b590: 6372 6f28 7365 6c66 2c20 6d61 6372 6f3a  cro(self, macro:
+0000b5a0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
+0000b5b0: 2020 2020 2020 2222 2250 726f 6365 7373        """Process
+0000b5c0: 2043 5720 6d61 6372 6f20 7375 6273 7469   CW macro substi
+0000b5d0: 7475 7469 6f6e 7322 2222 0a20 2020 2020  tutions""".     
+0000b5e0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+0000b5f0: 2e64 6174 6162 6173 652e 6765 745f 7365  .database.get_se
+0000b600: 7269 616c 2829 0a20 2020 2020 2020 2070  rial().        p
+0000b610: 7269 6e74 2872 6573 756c 7429 0a20 2020  rint(result).   
+0000b620: 2020 2020 206e 6578 745f 7365 7269 616c       next_serial
+0000b630: 203d 2073 7472 2872 6573 756c 742e 6765   = str(result.ge
+0000b640: 7428 2273 6572 6961 6c5f 6e72 222c 2022  t("serial_nr", "
+0000b650: 3122 2929 0a20 2020 2020 2020 2069 6620  1")).        if 
+0000b660: 6e65 7874 5f73 6572 6961 6c20 3d3d 2022  next_serial == "
+0000b670: 4e6f 6e65 223a 0a20 2020 2020 2020 2020  None":.         
+0000b680: 2020 206e 6578 745f 7365 7269 616c 203d     next_serial =
+0000b690: 2022 3122 0a20 2020 2020 2020 2070 7269   "1".        pri
+0000b6a0: 6e74 286e 6578 745f 7365 7269 616c 290a  nt(next_serial).
+0000b6b0: 2020 2020 2020 2020 6d61 6372 6f20 3d20          macro = 
+0000b6c0: 6d61 6372 6f2e 7570 7065 7228 290a 2020  macro.upper().  
+0000b6d0: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+0000b6e0: 6372 6f2e 7265 706c 6163 6528 2223 222c  cro.replace("#",
+0000b6f0: 206e 6578 745f 7365 7269 616c 290a 2020   next_serial).  
+0000b700: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+0000b710: 6372 6f2e 7265 706c 6163 6528 227b 4d59  cro.replace("{MY
+0000b720: 4341 4c4c 7d22 2c20 7365 6c66 2e73 7461  CALL}", self.sta
+0000b730: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
+0000b740: 2022 2229 290a 2020 2020 2020 2020 6d61   "")).        ma
+0000b750: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
+0000b760: 6163 6528 227b 4849 5343 414c 4c7d 222c  ace("{HISCALL}",
+0000b770: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+0000b780: 6578 7428 2929 0a20 2020 2020 2020 2069  ext()).        i
+0000b790: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+0000b7a0: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
+0000b7b0: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+0000b7c0: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
+0000b7d0: 6f2e 7265 706c 6163 6528 227b 534e 547d  o.replace("{SNT}
+0000b7e0: 222c 2073 656c 662e 7365 6e74 2e74 6578  ", self.sent.tex
+0000b7f0: 7428 292e 7265 706c 6163 6528 2239 222c  t().replace("9",
+0000b800: 2022 6e22 2929 0a20 2020 2020 2020 2065   "n")).        e
+0000b810: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000b820: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
+0000b830: 6570 6c61 6365 2822 7b53 4e54 7d22 2c20  eplace("{SNT}", 
+0000b840: 7365 6c66 2e73 656e 742e 7465 7874 2829  self.sent.text()
+0000b850: 290a 2020 2020 2020 2020 6d61 6372 6f20  ).        macro 
+0000b860: 3d20 6d61 6372 6f2e 7265 706c 6163 6528  = macro.replace(
+0000b870: 227b 5345 4e54 4e52 7d22 2c20 7365 6c66  "{SENTNR}", self
+0000b880: 2e6f 7468 6572 5f31 2e74 6578 7428 2929  .other_1.text())
+0000b890: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
+0000b8a0: 206d 6163 726f 2e72 6570 6c61 6365 280a   macro.replace(.
+0000b8b0: 2020 2020 2020 2020 2020 2020 227b 4558              "{EX
+0000b8c0: 4348 7d22 2c20 7365 6c66 2e63 6f6e 7465  CH}", self.conte
+0000b8d0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
+0000b8e0: 2253 656e 7445 7863 6861 6e67 6522 2c20  "SentExchange", 
+0000b8f0: 2278 7878 2229 0a20 2020 2020 2020 2029  "xxx").        )
+0000b900: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b910: 6d61 6372 6f0a 0a20 2020 2064 6566 2076  macro..    def v
+0000b920: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000b930: 2c20 7468 655f 7374 7269 6e67 3a20 7374  , the_string: st
+0000b940: 7229 202d 3e20 4e6f 6e65 3a0a 2020 2020  r) -> None:.    
+0000b950: 2020 2020 2222 2276 6f69 6365 7320 7374      """voices st
+0000b960: 7269 6e67 2075 7369 6e67 206e 6174 6f20  ring using nato 
+0000b970: 7068 6f6e 6574 6963 7322 2222 0a20 2020  phonetics""".   
+0000b980: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000b990: 6728 2256 6f69 6369 6e67 3a20 2573 222c  g("Voicing: %s",
+0000b9a0: 2074 6865 5f73 7472 696e 6729 0a20 2020   the_string).   
+0000b9b0: 2020 2020 206f 705f 7061 7468 203d 2050       op_path = P
+0000b9c0: 6174 6828 4441 5441 5f50 4154 4829 202f  ath(DATA_PATH) /
+0000b9d0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
+0000b9e0: 0a20 2020 2020 2020 2069 6620 225b 2220  .        if "[" 
+0000b9f0: 696e 2074 6865 5f73 7472 696e 673a 0a20  in the_string:. 
+0000ba00: 2020 2020 2020 2020 2020 2073 7562 5f73             sub_s
+0000ba10: 7472 696e 6720 3d20 7468 655f 7374 7269  tring = the_stri
+0000ba20: 6e67 2e73 7472 6970 2822 5b5d 2229 2e6c  ng.strip("[]").l
+0000ba30: 6f77 6572 2829 0a20 2020 2020 2020 2020  ower().         
+0000ba40: 2020 2066 696c 656e 616d 6520 3d20 6622     filename = f"
+0000ba50: 7b73 7472 286f 705f 7061 7468 297d 2f7b  {str(op_path)}/{
+0000ba60: 7375 625f 7374 7269 6e67 7d2e 7761 7622  sub_string}.wav"
+0000ba70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000ba80: 5061 7468 2866 696c 656e 616d 6529 2e69  Path(filename).i
+0000ba90: 735f 6669 6c65 2829 3a0a 2020 2020 2020  s_file():.      
+0000baa0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000bab0: 2e64 6562 7567 2822 566f 6963 696e 673a  .debug("Voicing:
+0000bac0: 2025 7322 2c20 6669 6c65 6e61 6d65 290a   %s", filename).
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 6461 7461 2c20 5f66 7320 3d20 7366 2e72  data, _fs = sf.r
+0000baf0: 6561 6428 6669 6c65 6e61 6d65 2c20 6474  ead(filename, dt
+0000bb00: 7970 653d 2266 6c6f 6174 3332 2229 0a20  ype="float32"). 
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000bb20: 656c 662e 7074 745f 6f6e 2829 0a20 2020  elf.ptt_on().   
+0000bb30: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0000bb40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bb50: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
+0000bb60: 2e64 6576 6963 6520 3d20 7365 6c66 2e70  .device = self.p
+0000bb70: 7265 662e 6765 7428 2273 6f75 6e64 6465  ref.get("soundde
+0000bb80: 7669 6365 222c 2022 6465 6661 756c 7422  vice", "default"
+0000bb90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000bba0: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
+0000bbb0: 2e73 616d 706c 6572 6174 6520 3d20 3434  .samplerate = 44
+0000bbc0: 3130 302e 300a 2020 2020 2020 2020 2020  100.0.          
+0000bbd0: 2020 2020 2020 2020 2020 7364 2e70 6c61            sd.pla
+0000bbe0: 7928 6461 7461 290a 2020 2020 2020 2020  y(data).        
+0000bbf0: 2020 2020 2020 2020 2020 2020 5f73 7461              _sta
+0000bc00: 7475 7320 3d20 7364 2e77 6169 7428 290a  tus = sd.wait().
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc20: 2020 2020 2320 6874 7470 733a 2f2f 736e      # https://sn
+0000bc30: 796b 2e69 6f2f 6164 7669 736f 722f 7079  yk.io/advisor/py
+0000bc40: 7468 6f6e 2f73 6f75 6e64 6465 7669 6365  thon/sounddevice
+0000bc50: 2f66 756e 6374 696f 6e73 2f73 6f75 6e64  /functions/sound
+0000bc60: 6465 7669 6365 2e50 6f72 7441 7564 696f  device.PortAudio
+0000bc70: 4572 726f 720a 2020 2020 2020 2020 2020  Error.          
+0000bc80: 2020 2020 2020 6578 6365 7074 2073 642e        except sd.
+0000bc90: 506f 7274 4175 6469 6f45 7272 6f72 2061  PortAudioError a
+0000bca0: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
+0000bcb0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000bcc0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+0000bcd0: 7b65 7272 7d22 290a 0a20 2020 2020 2020  {err}")..       
+0000bce0: 2020 2020 2020 2020 2073 656c 662e 7074           self.pt
+0000bcf0: 745f 6f66 6628 290a 2020 2020 2020 2020  t_off().        
+0000bd00: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000bd10: 2020 2073 656c 662e 7074 745f 6f6e 2829     self.ptt_on()
+0000bd20: 0a20 2020 2020 2020 2066 6f72 206c 6574  .        for let
+0000bd30: 7465 7220 696e 2074 6865 5f73 7472 696e  ter in the_strin
+0000bd40: 672e 6c6f 7765 7228 293a 0a20 2020 2020  g.lower():.     
+0000bd50: 2020 2020 2020 2069 6620 6c65 7474 6572         if letter
+0000bd60: 2069 6e20 2261 6263 6465 6667 6869 6a6b   in "abcdefghijk
+0000bd70: 6c6d 6e6f 7071 7273 7475 7677 7879 7a20  lmnopqrstuvwxyz 
+0000bd80: 3132 3334 3536 3738 3930 223a 0a20 2020  1234567890":.   
+0000bd90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000bda0: 6c65 7474 6572 203d 3d20 2220 223a 0a20  letter == " ":. 
 0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdc0: 2020 2020 2020 2073 642e 6465 6661 756c         sd.defaul
-0000bdd0: 742e 6465 7669 6365 203d 2073 656c 662e  t.device = self.
-0000bde0: 7072 6566 2e67 6574 2822 736f 756e 6464  pref.get("soundd
-0000bdf0: 6576 6963 6522 2c20 2264 6566 6175 6c74  evice", "default
-0000be00: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000be10: 2020 2020 2020 2020 2020 2073 642e 6465             sd.de
-0000be20: 6661 756c 742e 7361 6d70 6c65 7261 7465  fault.samplerate
-0000be30: 203d 2034 3431 3030 2e30 0a20 2020 2020   = 44100.0.     
-0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be50: 2020 2073 642e 706c 6179 2864 6174 6129     sd.play(data)
-0000be60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000be70: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000be80: 6465 6275 6728 2225 7322 2c20 6622 7b73  debug("%s", f"{s
-0000be90: 642e 7761 6974 2829 7d22 290a 2020 2020  d.wait()}").    
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 6578 6365 7074 2073 642e 506f 7274 4175  except sd.PortAu
-0000bec0: 6469 6f45 7272 6f72 2061 7320 6572 723a  dioError as err:
+0000bdc0: 2020 206c 6574 7465 7220 3d20 2273 7061     letter = "spa
+0000bdd0: 6365 220a 2020 2020 2020 2020 2020 2020  ce".            
+0000bde0: 2020 2020 6669 6c65 6e61 6d65 203d 2066      filename = f
+0000bdf0: 227b 7374 7228 6f70 5f70 6174 6829 7d2f  "{str(op_path)}/
+0000be00: 7b6c 6574 7465 727d 2e77 6176 220a 2020  {letter}.wav".  
+0000be10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000be20: 2050 6174 6828 6669 6c65 6e61 6d65 292e   Path(filename).
+0000be30: 6973 5f66 696c 6528 293a 0a20 2020 2020  is_file():.     
+0000be40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000be50: 6f67 6765 722e 6465 6275 6728 2256 6f69  ogger.debug("Voi
+0000be60: 6369 6e67 3a20 2573 222c 2066 696c 656e  cing: %s", filen
+0000be70: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+0000be80: 2020 2020 2020 2020 2064 6174 612c 205f           data, _
+0000be90: 6673 203d 2073 662e 7265 6164 2866 696c  fs = sf.read(fil
+0000bea0: 656e 616d 652c 2064 7479 7065 3d22 666c  ename, dtype="fl
+0000beb0: 6f61 7433 3222 290a 2020 2020 2020 2020  oat32").        
+0000bec0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
 0000bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bee0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-0000bef0: 6465 6275 6728 2225 7322 2c20 6622 7b65  debug("%s", f"{e
-0000bf00: 7272 7d22 290a 2020 2020 2020 2020 7365  rr}").        se
-0000bf10: 6c66 2e70 7474 5f6f 6666 2829 0a0a 2020  lf.ptt_off()..  
-0000bf20: 2020 6465 6620 7074 745f 6f6e 2873 656c    def ptt_on(sel
-0000bf30: 6629 3a0a 2020 2020 2020 2020 2222 2274  f):.        """t
-0000bf40: 7572 6e20 6f6e 2070 7474 2222 220a 2020  urn on ptt""".  
-0000bf50: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
-0000bf60: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
-0000bf70: 2020 2020 2020 2073 656c 662e 6c65 6674         self.left
-0000bf80: 646f 742e 7365 7450 6978 6d61 7028 7365  dot.setPixmap(se
-0000bf90: 6c66 2e67 7265 656e 646f 7429 0a20 2020  lf.greendot).   
-0000bfa0: 2020 2020 2020 2020 2061 7070 2e70 726f           app.pro
-0000bfb0: 6365 7373 4576 656e 7473 2829 0a20 2020  cessEvents().   
-0000bfc0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
-0000bfd0: 675f 636f 6e74 726f 6c2e 7074 745f 6f6e  g_control.ptt_on
-0000bfe0: 2829 0a0a 2020 2020 6465 6620 7074 745f  ()..    def ptt_
-0000bff0: 6f66 6628 7365 6c66 293a 0a20 2020 2020  off(self):.     
-0000c000: 2020 2022 2222 7475 726e 206f 6666 2070     """turn off p
-0000c010: 7474 2222 220a 2020 2020 2020 2020 7365  tt""".        se
-0000c020: 6c66 2e6c 6566 7464 6f74 2e73 6574 5069  lf.leftdot.setPi
-0000c030: 786d 6170 2873 656c 662e 7265 6464 6f74  xmap(self.reddot
-0000c040: 290a 2020 2020 2020 2020 6170 702e 7072  ).        app.pr
-0000c050: 6f63 6573 7345 7665 6e74 7328 290a 2020  ocessEvents().  
-0000c060: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-0000c070: 6f6e 7472 6f6c 2e70 7474 5f6f 6666 2829  ontrol.ptt_off()
-0000c080: 0a0a 2020 2020 6465 6620 7365 6e64 6631  ..    def sendf1
-0000c090: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000c0a0: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000c0b0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000c0c0: 2246 3120 436c 6963 6b65 6422 290a 2020  "F1 Clicked").  
-0000c0d0: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-0000c0e0: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
-0000c0f0: 6f64 6522 2920 696e 205b 2255 5342 222c  ode") in ["USB",
-0000c100: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
-0000c110: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
-0000c120: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
-0000c130: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000c140: 312e 746f 6f6c 5469 7028 2929 290a 2020  1.toolTip())).  
-0000c150: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000c160: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000c170: 2e63 773a 0a20 2020 2020 2020 2020 2020  .cw:.           
-0000c180: 2023 2069 6620 7365 6c66 2e70 7265 6665   # if self.prefe
-0000c190: 7265 6e63 652e 6765 7428 2273 656e 645f  rence.get("send_
-0000c1a0: 6e31 6d6d 5f70 6163 6b65 7473 2229 3a0a  n1mm_packets"):.
-0000c1b0: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000c1c0: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
-0000c1d0: 6f5f 696e 666f 5b22 4675 6e63 7469 6f6e  o_info["Function
-0000c1e0: 4b65 7943 6170 7469 6f6e 225d 203d 2073  KeyCaption"] = s
-0000c1f0: 656c 662e 4631 2e74 6578 7428 290a 2020  elf.F1.text().  
-0000c200: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000c210: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
-0000c220: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000c230: 2e46 312e 746f 6f6c 5469 7028 2929 290a  .F1.toolTip())).
-0000c240: 0a20 2020 2064 6566 2073 656e 6466 3228  .    def sendf2(
-0000c250: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000c260: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
-0000c270: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000c280: 4632 2043 6c69 636b 6564 2229 0a20 2020  F2 Clicked").   
-0000c290: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
-0000c2a0: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0000c2b0: 6465 2229 2069 6e20 5b22 5553 4222 2c20  de") in ["USB", 
-0000c2c0: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
-0000c2d0: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
-0000c2e0: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
-0000c2f0: 7373 5f6d 6163 726f 2873 656c 662e 4632  ss_macro(self.F2
-0000c300: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
-0000c310: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000c320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000c330: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
-0000c340: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
-0000c350: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000c360: 6f28 7365 6c66 2e46 322e 746f 6f6c 5469  o(self.F2.toolTi
-0000c370: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
-0000c380: 656e 6466 3328 7365 6c66 293a 0a20 2020  endf3(self):.   
-0000c390: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000c3a0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000c3b0: 6562 7567 2822 4633 2043 6c69 636b 6564  ebug("F3 Clicked
-0000c3c0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000c3d0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000c3e0: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000c3f0: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000c400: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000c410: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000c420: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000c430: 656c 662e 4633 2e74 6f6f 6c54 6970 2829  elf.F3.toolTip()
-0000c440: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-0000c450: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000c460: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
-0000c470: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000c480: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
-0000c490: 735f 6d61 6372 6f28 7365 6c66 2e46 332e  s_macro(self.F3.
-0000c4a0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000c4b0: 2064 6566 2073 656e 6466 3428 7365 6c66   def sendf4(self
-0000c4c0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000c4d0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000c4e0: 6767 6572 2e64 6562 7567 2822 4634 2043  gger.debug("F4 C
-0000c4f0: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000c500: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000c510: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000c520: 2069 6e20 5b22 5553 4222 2c20 2253 5342   in ["USB", "SSB
-0000c530: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000c540: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000c550: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000c560: 6163 726f 2873 656c 662e 4634 2e74 6f6f  acro(self.F4.too
-0000c570: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
-0000c580: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000c590: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
-0000c5a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c5b0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000c5c0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000c5d0: 6c66 2e46 342e 746f 6f6c 5469 7028 2929  lf.F4.toolTip())
-0000c5e0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000c5f0: 3528 7365 6c66 293a 0a20 2020 2020 2020  5(self):.       
-0000c600: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000c610: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000c620: 2822 4635 2043 6c69 636b 6564 2229 0a20  ("F5 Clicked"). 
-0000c630: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000c640: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000c650: 6d6f 6465 2229 2069 6e20 5b22 5553 4222  mode") in ["USB"
-0000c660: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
-0000c670: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
-0000c680: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
-0000c690: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000c6a0: 4635 2e74 6f6f 6c54 6970 2829 2929 0a20  F5.toolTip())). 
-0000c6b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000c6c0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0000c6d0: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
-0000c6e0: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000c6f0: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000c700: 6372 6f28 7365 6c66 2e46 352e 746f 6f6c  cro(self.F5.tool
-0000c710: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
-0000c720: 2073 656e 6466 3628 7365 6c66 293a 0a20   sendf6(self):. 
-0000c730: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
-0000c740: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000c750: 2e64 6562 7567 2822 4636 2043 6c69 636b  .debug("F6 Click
-0000c760: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
-0000c770: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000c780: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
-0000c790: 5b22 5553 4222 2c20 2253 5342 225d 3a0a  ["USB", "SSB"]:.
-0000c7a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000c7b0: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
-0000c7c0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000c7d0: 2873 656c 662e 4636 2e74 6f6f 6c54 6970  (self.F6.toolTip
-0000c7e0: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
-0000c7f0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000c800: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
-0000c810: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-0000c820: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
-0000c830: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000c840: 362e 746f 6f6c 5469 7028 2929 290a 0a20  6.toolTip())).. 
-0000c850: 2020 2064 6566 2073 656e 6466 3728 7365     def sendf7(se
-0000c860: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000c870: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
-0000c880: 6c6f 6767 6572 2e64 6562 7567 2822 4637  logger.debug("F7
-0000c890: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
-0000c8a0: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-0000c8b0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
-0000c8c0: 2229 2069 6e20 5b22 5553 4222 2c20 2253  ") in ["USB", "S
-0000c8d0: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
-0000c8e0: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
-0000c8f0: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
-0000c900: 5f6d 6163 726f 2873 656c 662e 4637 2e74  _macro(self.F7.t
-0000c910: 6f6f 6c54 6970 2829 2929 0a20 2020 2020  oolTip())).     
-0000c920: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000c930: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-0000c940: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000c950: 6c66 2e63 772e 7365 6e64 6377 2873 656c  lf.cw.sendcw(sel
-0000c960: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
-0000c970: 7365 6c66 2e46 372e 746f 6f6c 5469 7028  self.F7.toolTip(
-0000c980: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
-0000c990: 6466 3828 7365 6c66 293a 0a20 2020 2020  df8(self):.     
-0000c9a0: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
-0000c9b0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000c9c0: 7567 2822 4638 2043 6c69 636b 6564 2229  ug("F8 Clicked")
-0000c9d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000c9e0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000c9f0: 2822 6d6f 6465 2229 2069 6e20 5b22 5553  ("mode") in ["US
-0000ca00: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
-0000ca10: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
-0000ca20: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
-0000ca30: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000ca40: 662e 4638 2e74 6f6f 6c54 6970 2829 2929  f.F8.toolTip()))
-0000ca50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000ca60: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
-0000ca70: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
-0000ca80: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
-0000ca90: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
-0000caa0: 6d61 6372 6f28 7365 6c66 2e46 382e 746f  macro(self.F8.to
-0000cab0: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
-0000cac0: 6566 2073 656e 6466 3928 7365 6c66 293a  ef sendf9(self):
-0000cad0: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
-0000cae0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
-0000caf0: 6572 2e64 6562 7567 2822 4639 2043 6c69  er.debug("F9 Cli
-0000cb00: 636b 6564 2229 0a20 2020 2020 2020 2069  cked").        i
-0000cb10: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000cb20: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
-0000cb30: 6e20 5b22 5553 4222 2c20 2253 5342 225d  n ["USB", "SSB"]
-0000cb40: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000cb50: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
-0000cb60: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000cb70: 726f 2873 656c 662e 4639 2e74 6f6f 6c54  ro(self.F9.toolT
-0000cb80: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
-0000cb90: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000cba0: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
-0000cbb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000cbc0: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
-0000cbd0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
-0000cbe0: 2e46 392e 746f 6f6c 5469 7028 2929 290a  .F9.toolTip())).
-0000cbf0: 0a20 2020 2064 6566 2073 656e 6466 3130  .    def sendf10
-0000cc00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000cc10: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000cc20: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000cc30: 2246 3130 2043 6c69 636b 6564 2229 0a20  "F10 Clicked"). 
-0000cc40: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000cc50: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-0000cc60: 6d6f 6465 2229 2069 6e20 5b22 5553 4222  mode") in ["USB"
-0000cc70: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
-0000cc80: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
-0000cc90: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
-0000cca0: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000ccb0: 4631 302e 746f 6f6c 5469 7028 2929 290a  F10.toolTip())).
-0000ccc0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000ccd0: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-0000cce0: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
-0000ccf0: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-0000cd00: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
-0000cd10: 6163 726f 2873 656c 662e 4631 302e 746f  acro(self.F10.to
-0000cd20: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
-0000cd30: 6566 2073 656e 6466 3131 2873 656c 6629  ef sendf11(self)
-0000cd40: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000cd50: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000cd60: 6765 722e 6465 6275 6728 2246 3131 2043  ger.debug("F11 C
-0000cd70: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000cd80: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-0000cd90: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
-0000cda0: 2069 6e20 5b22 5553 4222 2c20 2253 5342   in ["USB", "SSB
-0000cdb0: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000cdc0: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000cdd0: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000cde0: 6163 726f 2873 656c 662e 4631 312e 746f  acro(self.F11.to
-0000cdf0: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000ce00: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000ce10: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000ce20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ce30: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000ce40: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ce50: 656c 662e 4631 312e 746f 6f6c 5469 7028  elf.F11.toolTip(
-0000ce60: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
-0000ce70: 6466 3132 2873 656c 6629 3a0a 2020 2020  df12(self):.    
-0000ce80: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000ce90: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000cea0: 6275 6728 2246 3132 2043 6c69 636b 6564  bug("F12 Clicked
-0000ceb0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000cec0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000ced0: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000cee0: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000cef0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000cf00: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000cf10: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000cf20: 656c 662e 4631 322e 746f 6f6c 5469 7028  elf.F12.toolTip(
-0000cf30: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0000cf40: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000cf50: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-0000cf60: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-0000cf70: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-0000cf80: 7373 5f6d 6163 726f 2873 656c 662e 4631  ss_macro(self.F1
-0000cf90: 322e 746f 6f6c 5469 7028 2929 290a 0a20  2.toolTip())).. 
-0000cfa0: 2020 2064 6566 2072 756e 5f73 705f 6275     def run_sp_bu
-0000cfb0: 7474 6f6e 735f 636c 6963 6b65 6428 7365  ttons_clicked(se
-0000cfc0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000cfd0: 4861 6e64 6c65 2072 756e 2f73 2670 206d  Handle run/s&p m
-0000cfe0: 6f64 6522 2222 0a20 2020 2020 2020 2073  ode""".        s
-0000cff0: 656c 662e 7072 6566 5b22 7275 6e5f 7374  elf.pref["run_st
-0000d000: 6174 6522 5d20 3d20 7365 6c66 2e72 6164  ate"] = self.rad
-0000d010: 696f 4275 7474 6f6e 5f72 756e 2e69 7343  ioButton_run.isC
-0000d020: 6865 636b 6564 2829 0a20 2020 2020 2020  hecked().       
-0000d030: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
-0000d040: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
-0000d050: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
-0000d060: 6372 6f73 2829 0a0a 2020 2020 6465 6620  cros()..    def 
-0000d070: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
-0000d080: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000d090: 2222 220a 2020 2020 2020 2020 5772 6974  """.        Writ
-0000d0a0: 6520 7072 6566 6572 656e 6365 7320 746f  e preferences to
-0000d0b0: 206a 736f 6e20 6669 6c65 2e0a 2020 2020   json file..    
-0000d0c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000d0d0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0000d0e0: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-0000d0f0: 2020 2020 2020 2020 2020 2020 434f 4e46              CONF
-0000d100: 4947 5f50 4154 4820 2b20 222f 6e6f 7431  IG_PATH + "/not1
-0000d110: 6d6d 2e6a 736f 6e22 2c20 2277 7422 2c20  mm.json", "wt", 
-0000d120: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-0000d130: 0a20 2020 2020 2020 2020 2020 2029 2061  .            ) a
-0000d140: 7320 6669 6c65 5f64 6573 6372 6970 746f  s file_descripto
-0000d150: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000d160: 2020 2066 696c 655f 6465 7363 7269 7074     file_descript
-0000d170: 6f72 2e77 7269 7465 2864 756d 7073 2873  or.write(dumps(s
-0000d180: 656c 662e 7072 6566 2c20 696e 6465 6e74  elf.pref, indent
-0000d190: 3d34 2929 0a20 2020 2020 2020 2020 2020  =4)).           
-0000d1a0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000d1b0: 2822 7772 6974 696e 673a 2025 7322 2c20  ("writing: %s", 
-0000d1c0: 7365 6c66 2e70 7265 6629 0a20 2020 2020  self.pref).     
-0000d1d0: 2020 2065 7863 6570 7420 494f 4572 726f     except IOErro
-0000d1e0: 7220 6173 2065 7863 6570 7469 6f6e 3a0a  r as exception:.
-0000d1f0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000d200: 6572 2e63 7269 7469 6361 6c28 2277 7269  er.critical("wri
-0000d210: 7465 7072 6566 6572 656e 6365 733a 2025  tepreferences: %
-0000d220: 7322 2c20 6578 6365 7074 696f 6e29 0a0a  s", exception)..
-0000d230: 2020 2020 6465 6620 7265 6164 7072 6566      def readpref
-0000d240: 6572 656e 6365 7328 7365 6c66 293a 0a20  erences(self):. 
-0000d250: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d260: 2020 2052 6573 746f 7265 2070 7265 6665     Restore prefe
-0000d270: 7265 6e63 6573 2069 6620 7468 6579 2065  rences if they e
-0000d280: 7869 7374 2c20 6f74 6865 7277 6973 6520  xist, otherwise 
-0000d290: 6372 6561 7465 2073 6f6d 6520 7361 6e65  create some sane
-0000d2a0: 2064 6566 6175 6c74 732e 0a20 2020 2020   defaults..     
-0000d2b0: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-0000d2c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000d2d0: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
-0000d2e0: 7328 434f 4e46 4947 5f50 4154 4820 2b20  s(CONFIG_PATH + 
-0000d2f0: 222f 6e6f 7431 6d6d 2e6a 736f 6e22 293a  "/not1mm.json"):
-0000d300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d310: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d330: 434f 4e46 4947 5f50 4154 4820 2b20 222f  CONFIG_PATH + "/
-0000d340: 6e6f 7431 6d6d 2e6a 736f 6e22 2c20 2272  not1mm.json", "r
-0000d350: 7422 2c20 656e 636f 6469 6e67 3d22 7574  t", encoding="ut
-0000d360: 662d 3822 0a20 2020 2020 2020 2020 2020  f-8".           
-0000d370: 2020 2020 2029 2061 7320 6669 6c65 5f64       ) as file_d
-0000d380: 6573 6372 6970 746f 723a 0a20 2020 2020  escriptor:.     
-0000d390: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d3a0: 656c 662e 7072 6566 203d 206c 6f61 6473  elf.pref = loads
-0000d3b0: 2866 696c 655f 6465 7363 7269 7074 6f72  (file_descriptor
-0000d3c0: 2e72 6561 6428 2929 0a20 2020 2020 2020  .read()).       
-0000d3d0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-0000d3e0: 6765 722e 696e 666f 2822 2573 222c 2073  ger.info("%s", s
-0000d3f0: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
-0000d400: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000d410: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000d420: 6572 2e69 6e66 6f28 224e 6f20 7072 6566  er.info("No pref
-0000d430: 6572 656e 6365 2066 696c 652e 2057 7269  erence file. Wri
-0000d440: 7469 6e67 2070 7265 6665 7265 6e63 652e  ting preference.
-0000d450: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000d460: 2020 2077 6974 6820 6f70 656e 280a 2020     with open(.  
-0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d480: 2020 434f 4e46 4947 5f50 4154 4820 2b20    CONFIG_PATH + 
-0000d490: 222f 6e6f 7431 6d6d 2e6a 736f 6e22 2c20  "/not1mm.json", 
-0000d4a0: 2277 7422 2c20 656e 636f 6469 6e67 3d22  "wt", encoding="
-0000d4b0: 7574 662d 3822 0a20 2020 2020 2020 2020  utf-8".         
-0000d4c0: 2020 2020 2020 2029 2061 7320 6669 6c65         ) as file
-0000d4d0: 5f64 6573 6372 6970 746f 723a 0a20 2020  _descriptor:.   
-0000d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4f0: 2073 656c 662e 7072 6566 203d 2073 656c   self.pref = sel
-0000d500: 662e 7072 6566 5f72 6566 2e63 6f70 7928  f.pref_ref.copy(
-0000d510: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000d520: 2020 2020 2020 6669 6c65 5f64 6573 6372        file_descr
-0000d530: 6970 746f 722e 7772 6974 6528 6475 6d70  iptor.write(dump
-0000d540: 7328 7365 6c66 2e70 7265 662c 2069 6e64  s(self.pref, ind
-0000d550: 656e 743d 3429 290a 2020 2020 2020 2020  ent=4)).        
-0000d560: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000d570: 6572 2e69 6e66 6f28 2225 7322 2c20 7365  er.info("%s", se
-0000d580: 6c66 2e70 7265 6629 0a20 2020 2020 2020  lf.pref).       
-0000d590: 2065 7863 6570 7420 494f 4572 726f 7220   except IOError 
-0000d5a0: 6173 2065 7863 6570 7469 6f6e 3a0a 2020  as exception:.  
-0000d5b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000d5c0: 2e63 7269 7469 6361 6c28 2245 7272 6f72  .critical("Error
-0000d5d0: 3a20 2573 222c 2065 7863 6570 7469 6f6e  : %s", exception
-0000d5e0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000d5f0: 6c6f 6f6b 5f75 7020 3d20 4e6f 6e65 0a20  look_up = None. 
-0000d600: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000d610: 7265 662e 6765 7428 2275 7365 7172 7a22  ref.get("useqrz"
-0000d620: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000d630: 656c 662e 6c6f 6f6b 5f75 7020 3d20 5152  elf.look_up = QR
-0000d640: 5a6c 6f6f 6b75 7028 0a20 2020 2020 2020  Zlookup(.       
-0000d650: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-0000d660: 6566 2e67 6574 2822 6c6f 6f6b 7570 7573  ef.get("lookupus
-0000d670: 6572 6e61 6d65 2229 2c0a 2020 2020 2020  ername"),.      
-0000d680: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000d690: 7265 662e 6765 7428 226c 6f6f 6b75 7070  ref.get("lookupp
-0000d6a0: 6173 7377 6f72 6422 292c 0a20 2020 2020  assword"),.     
-0000d6b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d6c0: 2023 2069 6620 7365 6c66 2e70 7265 662e   # if self.pref.
-0000d6d0: 6765 7428 2275 7365 6861 6d64 6222 293a  get("usehamdb"):
-0000d6e0: 0a20 2020 2020 2020 2023 2020 2020 2073  .        #     s
-0000d6f0: 656c 662e 6c6f 6f6b 5f75 7020 3d20 4861  elf.look_up = Ha
-0000d700: 6d44 426c 6f6f 6b75 7028 290a 2020 2020  mDBlookup().    
-0000d710: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-0000d720: 2e67 6574 2822 7573 6568 616d 7174 6822  .get("usehamqth"
-0000d730: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0000d740: 656c 662e 6c6f 6f6b 5f75 7020 3d20 4861  elf.look_up = Ha
-0000d750: 6d51 5448 280a 2020 2020 2020 2020 2020  mQTH(.          
-0000d760: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-0000d770: 6765 7428 226c 6f6f 6b75 7075 7365 726e  get("lookupusern
-0000d780: 616d 6522 292c 0a20 2020 2020 2020 2020  ame"),.         
-0000d790: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-0000d7a0: 2e67 6574 2822 6c6f 6f6b 7570 7061 7373  .get("lookuppass
-0000d7b0: 776f 7264 2229 2c0a 2020 2020 2020 2020  word"),.        
-0000d7c0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-0000d7d0: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-0000d7e0: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
-0000d7f0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000d800: 6164 696f 4275 7474 6f6e 5f72 756e 2e73  adioButton_run.s
-0000d810: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
-0000d820: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000d830: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000d840: 6164 696f 4275 7474 6f6e 5f73 702e 7365  adioButton_sp.se
-0000d850: 7443 6865 636b 6564 2854 7275 6529 0a0a  tChecked(True)..
-0000d860: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000d870: 7072 6566 2e67 6574 2822 6461 726b 5f6d  pref.get("dark_m
-0000d880: 6f64 6522 293a 0a20 2020 2020 2020 2020  ode"):.         
-0000d890: 2020 2073 656c 662e 6163 7469 6f6e 4461     self.actionDa
-0000d8a0: 726b 5f4d 6f64 652e 7365 7443 6865 636b  rk_Mode.setCheck
-0000d8b0: 6564 2854 7275 6529 0a20 2020 2020 2020  ed(True).       
-0000d8c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d8d0: 2020 2073 656c 662e 6163 7469 6f6e 4461     self.actionDa
-0000d8e0: 726b 5f4d 6f64 652e 7365 7443 6865 636b  rk_Mode.setCheck
-0000d8f0: 6564 2846 616c 7365 290a 0a20 2020 2020  ed(False)..     
-0000d900: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
-0000d910: 6765 7428 2263 6f6d 6d61 6e64 5f62 7574  get("command_but
-0000d920: 746f 6e73 2229 3a0a 2020 2020 2020 2020  tons"):.        
-0000d930: 2020 2020 7365 6c66 2e61 6374 696f 6e43      self.actionC
-0000d940: 6f6d 6d61 6e64 5f42 7574 746f 6e73 2e73  ommand_Buttons.s
-0000d950: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
-0000d960: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000d970: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000d980: 6374 696f 6e43 6f6d 6d61 6e64 5f42 7574  ctionCommand_But
-0000d990: 746f 6e73 2e73 6574 4368 6563 6b65 6428  tons.setChecked(
-0000d9a0: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
-0000d9b0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-0000d9c0: 2822 6377 5f6d 6163 726f 7322 293a 0a20  ("cw_macros"):. 
-0000d9d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d9e0: 6163 7469 6f6e 4357 5f4d 6163 726f 732e  actionCW_Macros.
-0000d9f0: 7365 7443 6865 636b 6564 2854 7275 6529  setChecked(True)
-0000da00: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000da10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000da20: 6163 7469 6f6e 4357 5f4d 6163 726f 732e  actionCW_Macros.
-0000da30: 7365 7443 6865 636b 6564 2846 616c 7365  setChecked(False
-0000da40: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-0000da50: 6c66 2e70 7265 662e 6765 7428 2262 616e  lf.pref.get("ban
-0000da60: 6473 5f6d 6f64 6573 2229 3a0a 2020 2020  ds_modes"):.    
-0000da70: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-0000da80: 696f 6e4d 6f64 655f 616e 645f 4261 6e64  ionMode_and_Band
-0000da90: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
-0000daa0: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
-0000dab0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000dac0: 662e 6163 7469 6f6e 4d6f 6465 5f61 6e64  f.actionMode_and
-0000dad0: 5f42 616e 6473 2e73 6574 4368 6563 6b65  _Bands.setChecke
-0000dae0: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
-0000daf0: 2020 6d75 6c74 6963 6173 745f 6772 6f75    multicast_grou
-0000db00: 7020 3d20 7365 6c66 2e70 7265 662e 6765  p = self.pref.ge
-0000db10: 7428 226d 756c 7469 6361 7374 5f67 726f  t("multicast_gro
-0000db20: 7570 222c 2022 3232 342e 312e 312e 3122  up", "224.1.1.1"
-0000db30: 290a 2020 2020 2020 2020 6d75 6c74 6963  ).        multic
-0000db40: 6173 745f 706f 7274 203d 2073 656c 662e  ast_port = self.
-0000db50: 7072 6566 2e67 6574 2822 6d75 6c74 6963  pref.get("multic
-0000db60: 6173 745f 706f 7274 222c 2032 3233 3929  ast_port", 2239)
-0000db70: 0a20 2020 2020 2020 2069 6e74 6572 6661  .        interfa
-0000db80: 6365 5f69 7020 3d20 7365 6c66 2e70 7265  ce_ip = self.pre
-0000db90: 662e 6765 7428 2269 6e74 6572 6661 6365  f.get("interface
-0000dba0: 5f69 7022 2c20 2230 2e30 2e30 2e30 2229  _ip", "0.0.0.0")
-0000dbb0: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
-0000dbc0: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-0000dbd0: 6520 3d20 4d75 6c74 6963 6173 7428 0a20  e = Multicast(. 
-0000dbe0: 2020 2020 2020 2020 2020 206d 756c 7469             multi
-0000dbf0: 6361 7374 5f67 726f 7570 2c20 6d75 6c74  cast_group, mult
-0000dc00: 6963 6173 745f 706f 7274 2c20 696e 7465  icast_port, inte
-0000dc10: 7266 6163 655f 6970 0a20 2020 2020 2020  rface_ip.       
-0000dc20: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
-0000dc30: 2e72 6967 5f63 6f6e 7472 6f6c 203d 204e  .rig_control = N
-0000dc40: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-0000dc50: 7365 6c66 2e70 7265 662e 6765 7428 2275  self.pref.get("u
-0000dc60: 7365 666c 7269 6722 2c20 4661 6c73 6529  seflrig", False)
-0000dc70: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-0000dc80: 6767 6572 2e64 6562 7567 280a 2020 2020  gger.debug(.    
-0000dc90: 2020 2020 2020 2020 2020 2020 2255 7369              "Usi
-0000dca0: 6e67 2066 6c72 6967 3a20 2573 222c 0a20  ng flrig: %s",. 
-0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000dcc0: 227b 7365 6c66 2e70 7265 662e 6765 7428  "{self.pref.get(
-0000dcd0: 2743 4154 5f69 7027 297d 207b 7365 6c66  'CAT_ip')} {self
-0000dce0: 2e70 7265 662e 6765 7428 2743 4154 5f70  .pref.get('CAT_p
-0000dcf0: 6f72 7427 297d 222c 0a20 2020 2020 2020  ort')}",.       
-0000dd00: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000dd10: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-0000dd20: 726f 6c20 3d20 4341 5428 0a20 2020 2020  rol = CAT(.     
-0000dd30: 2020 2020 2020 2020 2020 2022 666c 7269             "flri
-0000dd40: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
-0000dd50: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
-0000dd60: 7428 2243 4154 5f69 7022 2c20 2231 3237  t("CAT_ip", "127
-0000dd70: 2e30 2e30 2e31 2229 2c0a 2020 2020 2020  .0.0.1"),.      
-0000dd80: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
-0000dd90: 6c66 2e70 7265 662e 6765 7428 2243 4154  lf.pref.get("CAT
-0000dda0: 5f70 6f72 7422 2c20 3132 3334 3529 292c  _port", 12345)),
-0000ddb0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000ddc0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000ddd0: 7265 662e 6765 7428 2275 7365 7269 6763  ref.get("userigc
-0000dde0: 746c 6422 2c20 4661 6c73 6529 3a0a 2020  tld", False):.  
-0000ddf0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000de00: 2e64 6562 7567 280a 2020 2020 2020 2020  .debug(.        
-0000de10: 2020 2020 2020 2020 2255 7369 6e67 2072          "Using r
-0000de20: 6967 6374 6c64 3a20 2573 222c 0a20 2020  igctld: %s",.   
-0000de30: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-0000de40: 7365 6c66 2e70 7265 662e 6765 7428 2743  self.pref.get('C
-0000de50: 4154 5f69 7027 297d 207b 7365 6c66 2e70  AT_ip')} {self.p
-0000de60: 7265 662e 6765 7428 2743 4154 5f70 6f72  ref.get('CAT_por
-0000de70: 7427 297d 222c 0a20 2020 2020 2020 2020  t')}",.         
-0000de80: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000de90: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-0000dea0: 6c20 3d20 4341 5428 0a20 2020 2020 2020  l = CAT(.       
-0000deb0: 2020 2020 2020 2020 2022 7269 6763 746c           "rigctl
-0000dec0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-0000ded0: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
-0000dee0: 7428 2243 4154 5f69 7022 2c20 2231 3237  t("CAT_ip", "127
-0000def0: 2e30 2e30 2e31 2229 2c0a 2020 2020 2020  .0.0.1"),.      
-0000df00: 2020 2020 2020 2020 2020 696e 7428 7365            int(se
-0000df10: 6c66 2e70 7265 662e 6765 7428 2243 4154  lf.pref.get("CAT
-0000df20: 5f70 6f72 7422 2c20 3435 3332 2929 2c0a  _port", 4532)),.
-0000df30: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000df40: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0000df50: 7265 662e 6765 7428 2263 7774 7970 6522  ref.get("cwtype"
-0000df60: 2c20 3029 203d 3d20 303a 0a20 2020 2020  , 0) == 0:.     
-0000df70: 2020 2020 2020 2073 656c 662e 6377 203d         self.cw =
-0000df80: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
-0000df90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000dfa0: 7365 6c66 2e63 7720 3d20 4357 280a 2020  self.cw = CW(.  
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000dfc0: 7428 7365 6c66 2e70 7265 662e 6765 7428  t(self.pref.get(
-0000dfd0: 2263 7774 7970 6522 2929 2c0a 2020 2020  "cwtype")),.    
-0000dfe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000dff0: 2e70 7265 662e 6765 7428 2263 7769 7022  .pref.get("cwip"
-0000e000: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000e010: 2020 2069 6e74 2873 656c 662e 7072 6566     int(self.pref
-0000e020: 2e67 6574 2822 6377 706f 7274 222c 2036  .get("cwport", 6
-0000e030: 3738 3929 292c 0a20 2020 2020 2020 2020  789)),.         
-0000e040: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000e050: 2073 656c 662e 6377 2e73 7065 6564 203d   self.cw.speed =
-0000e060: 2032 300a 0a20 2020 2020 2020 2073 656c   20..        sel
-0000e070: 662e 6461 726b 5f6d 6f64 6528 290a 2020  f.dark_mode().  
-0000e080: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-0000e090: 636f 6d6d 616e 645f 6275 7474 6f6e 7328  command_buttons(
-0000e0a0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000e0b0: 686f 775f 4357 5f6d 6163 726f 7328 290a  how_CW_macros().
-0000e0c0: 2020 2020 2020 2020 2320 7365 6c66 2e73          # self.s
-0000e0d0: 686f 775f 6261 6e64 5f6d 6f64 6528 290a  how_band_mode().
-0000e0e0: 0a20 2020 2064 6566 2077 6174 6368 5f75  .    def watch_u
-0000e0f0: 6470 2873 656c 6629 3a0a 2020 2020 2020  dp(self):.      
-0000e100: 2020 2222 2250 7574 7320 5544 5020 6461    """Puts UDP da
-0000e110: 7461 6772 616d 7320 696e 2061 2046 4946  tagrams in a FIF
-0000e120: 4f20 7175 6575 6522 2222 0a20 2020 2020  O queue""".     
-0000e130: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
-0000e140: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e160: 6461 7461 6772 616d 203d 2073 656c 662e  datagram = self.
-0000e170: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-0000e180: 6163 652e 7365 7276 6572 5f75 6470 2e72  ace.server_udp.r
-0000e190: 6563 7628 3135 3030 290a 2020 2020 2020  ecv(1500).      
-0000e1a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000e1b0: 2e64 6562 7567 2864 6174 6167 7261 6d2e  .debug(datagram.
-0000e1c0: 6465 636f 6465 2829 290a 2020 2020 2020  decode()).      
-0000e1d0: 2020 2020 2020 6578 6365 7074 2073 6f63        except soc
-0000e1e0: 6b65 742e 7469 6d65 6f75 743a 0a20 2020  ket.timeout:.   
-0000e1f0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-0000e200: 652e 736c 6565 7028 302e 3129 0a20 2020  e.sleep(0.1).   
-0000e210: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000e220: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-0000e230: 2020 6966 2064 6174 6167 7261 6d3a 0a20    if datagram:. 
-0000e240: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e250: 656c 662e 7564 705f 6669 666f 2e70 7574  elf.udp_fifo.put
-0000e260: 2864 6174 6167 7261 6d29 0a0a 2020 2020  (datagram)..    
-0000e270: 6465 6620 6368 6563 6b5f 7564 705f 7472  def check_udp_tr
-0000e280: 6166 6669 6328 7365 6c66 293a 0a20 2020  affic(self):.   
-0000e290: 2020 2020 2022 2222 4368 6563 6b73 2055       """Checks U
-0000e2a0: 4450 2054 7261 6666 6963 2222 220a 2020  DP Traffic""".  
-0000e2b0: 2020 2020 2020 7768 696c 6520 6e6f 7420        while not 
-0000e2c0: 7365 6c66 2e75 6470 5f66 6966 6f2e 656d  self.udp_fifo.em
-0000e2d0: 7074 7928 293a 0a20 2020 2020 2020 2020  pty():.         
-0000e2e0: 2020 2064 6174 6167 7261 6d20 3d20 7365     datagram = se
-0000e2f0: 6c66 2e75 6470 5f66 6966 6f2e 6765 7428  lf.udp_fifo.get(
-0000e300: 290a 2020 2020 2020 2020 2020 2020 7472  ).            tr
-0000e310: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000e320: 2020 2064 6562 7567 5f69 6e66 6f20 3d20     debug_info = 
-0000e330: 6622 7b64 6174 6167 7261 6d2e 6465 636f  f"{datagram.deco
-0000e340: 6465 2829 7d22 0a20 2020 2020 2020 2020  de()}".         
-0000e350: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000e360: 6275 6728 6465 6275 675f 696e 666f 290a  bug(debug_info).
-0000e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e380: 6a73 6f6e 5f64 6174 6120 3d20 6c6f 6164  json_data = load
-0000e390: 7328 6461 7461 6772 616d 2e64 6563 6f64  s(datagram.decod
-0000e3a0: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
-0000e3b0: 2065 7863 6570 7420 556e 6963 6f64 6544   except UnicodeD
-0000e3c0: 6563 6f64 6545 7272 6f72 2061 7320 6572  ecodeError as er
-0000e3d0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-0000e3e0: 2020 2074 6865 5f65 7272 6f72 203d 2066     the_error = f
-0000e3f0: 224e 6f74 2055 6e69 636f 6465 3a20 7b65  "Not Unicode: {e
-0000e400: 7272 7d5c 6e7b 6461 7461 6772 616d 7d22  rr}\n{datagram}"
-0000e410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e420: 206c 6f67 6765 722e 6465 6275 6728 7468   logger.debug(th
-0000e430: 655f 6572 726f 7229 0a20 2020 2020 2020  e_error).       
-0000e440: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0000e450: 650a 2020 2020 2020 2020 2020 2020 6578  e.            ex
-0000e460: 6365 7074 204a 534f 4e44 6563 6f64 6545  cept JSONDecodeE
-0000e470: 7272 6f72 2061 7320 6572 723a 0a20 2020  rror as err:.   
-0000e480: 2020 2020 2020 2020 2020 2020 2074 6865               the
-0000e490: 5f65 7272 6f72 203d 2066 224e 6f74 204a  _error = f"Not J
-0000e4a0: 534f 4e3a 207b 6572 727d 5c6e 7b64 6174  SON: {err}\n{dat
-0000e4b0: 6167 7261 6d7d 220a 2020 2020 2020 2020  agram}".        
-0000e4c0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000e4d0: 6562 7567 2874 6865 5f65 7272 6f72 290a  ebug(the_error).
-0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4f0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0000e500: 2020 2020 2069 6620 6a73 6f6e 5f64 6174       if json_dat
-0000e510: 612e 6765 7428 2263 6d64 222c 2022 2229  a.get("cmd", "")
-0000e520: 203d 3d20 2247 4554 434f 4c55 4d4e 5322   == "GETCOLUMNS"
-0000e530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e540: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
-0000e550: 662e 636f 6e74 6573 742c 2022 636f 6c75  f.contest, "colu
-0000e560: 6d6e 7322 293a 0a20 2020 2020 2020 2020  mns"):.         
-0000e570: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-0000e580: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-0000e590: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-0000e5a0: 225d 203d 2022 5348 4f57 434f 4c55 4d4e  "] = "SHOWCOLUMN
-0000e5b0: 5322 0a20 2020 2020 2020 2020 2020 2020  S".             
-0000e5c0: 2020 2020 2020 2063 6d64 5b22 434f 4c55         cmd["COLU
-0000e5d0: 4d4e 5322 5d20 3d20 7365 6c66 2e63 6f6e  MNS"] = self.con
-0000e5e0: 7465 7374 2e63 6f6c 756d 6e73 0a20 2020  test.columns.   
-0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e600: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-0000e610: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-0000e620: 735f 6a73 6f6e 2863 6d64 290a 2020 2020  s_json(cmd).    
-0000e630: 2020 2020 2020 2020 6966 206a 736f 6e5f          if json_
-0000e640: 6461 7461 2e67 6574 2822 636d 6422 2c20  data.get("cmd", 
-0000e650: 2222 2920 3d3d 2022 5455 4e45 223a 0a20  "") == "TUNE":. 
-0000e660: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000e670: 2062 277b 2263 6d64 223a 2022 5455 4e45   b'{"cmd": "TUNE
-0000e680: 222c 2022 6672 6571 223a 2037 2e30 3233  ", "freq": 7.023
-0000e690: 352c 2022 7370 6f74 223a 2022 4d4d 3044  5, "spot": "MM0D
-0000e6a0: 4749 227d 270a 2020 2020 2020 2020 2020  GI"}'.          
-0000e6b0: 2020 2020 2020 7666 6f20 3d20 6a73 6f6e        vfo = json
-0000e6c0: 5f64 6174 612e 6765 7428 2266 7265 7122  _data.get("freq"
-0000e6d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e6e0: 2020 7666 6f20 3d20 666c 6f61 7428 7666    vfo = float(vf
-0000e6f0: 6f29 202a 2031 3030 3030 3030 0a20 2020  o) * 1000000.   
-0000e700: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e710: 662e 7261 6469 6f5f 7374 6174 655b 2276  f.radio_state["v
-0000e720: 666f 6122 5d20 3d20 696e 7428 7666 6f29  foa"] = int(vfo)
-0000e730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e740: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
-0000e750: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
-0000e760: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000e770: 6967 5f63 6f6e 7472 6f6c 2e73 6574 5f76  ig_control.set_v
-0000e780: 666f 2869 6e74 2876 666f 2929 0a20 2020  fo(int(vfo)).   
-0000e790: 2020 2020 2020 2020 2020 2020 2073 706f               spo
-0000e7a0: 7420 3d20 6a73 6f6e 5f64 6174 612e 6765  t = json_data.ge
-0000e7b0: 7428 2273 706f 7422 2c20 2222 290a 2020  t("spot", "").  
-0000e7c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e7d0: 6c66 2e63 616c 6c73 6967 6e2e 7365 7454  lf.callsign.setT
-0000e7e0: 6578 7428 7370 6f74 290a 2020 2020 2020  ext(spot).      
-0000e7f0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000e800: 616c 6c73 6967 6e5f 6368 616e 6765 6428  allsign_changed(
-0000e810: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e820: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
-0000e830: 7365 7446 6f63 7573 2829 0a20 2020 2020  setFocus().     
-0000e840: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e850: 6361 6c6c 7369 676e 2e61 6374 6976 6174  callsign.activat
-0000e860: 6557 696e 646f 7728 290a 2020 2020 2020  eWindow().      
-0000e870: 2020 2020 2020 2020 2020 7769 6e64 6f77            window
-0000e880: 2e72 6169 7365 5f28 290a 0a20 2020 2064  .raise_()..    d
-0000e890: 6566 2064 6172 6b5f 6d6f 6465 5f73 7461  ef dark_mode_sta
-0000e8a0: 7465 5f63 6861 6e67 6528 7365 6c66 293a  te_change(self):
-0000e8b0: 0a20 2020 2020 2020 2022 2222 6461 726b  .        """dark
-0000e8c0: 6d6f 6465 2064 726f 7064 6f77 6e20 6368  mode dropdown ch
-0000e8d0: 6563 6b6d 6172 6b20 6368 616e 6765 6422  eckmark changed"
-0000e8e0: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-0000e8f0: 7072 6566 5b22 6461 726b 5f6d 6f64 6522  pref["dark_mode"
-0000e900: 5d20 3d20 7365 6c66 2e61 6374 696f 6e44  ] = self.actionD
-0000e910: 6172 6b5f 4d6f 6465 2e69 7343 6865 636b  ark_Mode.isCheck
-0000e920: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
-0000e930: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-0000e940: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-0000e950: 662e 6461 726b 5f6d 6f64 6528 290a 0a20  f.dark_mode().. 
-0000e960: 2020 2064 6566 2064 6172 6b5f 6d6f 6465     def dark_mode
-0000e970: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000e980: 2222 2263 6861 6e67 6520 6469 7370 6c61  """change displa
-0000e990: 7920 6d6f 6465 2222 220a 2020 2020 2020  y mode""".      
-0000e9a0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
-0000e9b0: 6574 2822 6461 726b 5f6d 6f64 6522 293a  et("dark_mode"):
-0000e9c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000e9d0: 662e 7365 7453 7479 6c65 5368 6565 7428  f.setStyleSheet(
-0000e9e0: 4441 524b 5f53 5459 4c45 5348 4545 5429  DARK_STYLESHEET)
-0000e9f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000ea00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000ea10: 7365 7453 7479 6c65 5368 6565 7428 2222  setStyleSheet(""
-0000ea20: 290a 0a20 2020 2064 6566 2063 775f 6d61  )..    def cw_ma
-0000ea30: 6372 6f73 5f73 7461 7465 5f63 6861 6e67  cros_state_chang
-0000ea40: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
-0000ea50: 2020 2222 224d 656e 7520 6974 656d 2074    """Menu item t
-0000ea60: 6f20 7368 6f77 2f68 6964 6520 6d61 6372  o show/hide macr
-0000ea70: 6f20 6275 7474 6f6e 7322 2222 0a20 2020  o buttons""".   
-0000ea80: 2020 2020 2073 656c 662e 7072 6566 5b22       self.pref["
-0000ea90: 6377 5f6d 6163 726f 7322 5d20 3d20 7365  cw_macros"] = se
-0000eaa0: 6c66 2e61 6374 696f 6e43 575f 4d61 6372  lf.actionCW_Macr
-0000eab0: 6f73 2e69 7343 6865 636b 6564 2829 0a20  os.isChecked(). 
-0000eac0: 2020 2020 2020 2073 656c 662e 7772 6974         self.writ
-0000ead0: 655f 7072 6566 6572 656e 6365 2829 0a20  e_preference(). 
-0000eae0: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
-0000eaf0: 5f43 575f 6d61 6372 6f73 2829 0a0a 2020  _CW_macros()..  
-0000eb00: 2020 6465 6620 7368 6f77 5f43 575f 6d61    def show_CW_ma
-0000eb10: 6372 6f73 2873 656c 6629 3a0a 2020 2020  cros(self):.    
-0000eb20: 2020 2020 2222 226d 6163 726f 2062 7574      """macro but
-0000eb30: 746f 6e20 7374 6174 6520 6368 616e 6765  ton state change
-0000eb40: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-0000eb50: 656c 662e 7072 6566 2e67 6574 2822 6377  elf.pref.get("cw
-0000eb60: 5f6d 6163 726f 7322 293a 0a20 2020 2020  _macros"):.     
-0000eb70: 2020 2020 2020 2073 656c 662e 4275 7474         self.Butt
-0000eb80: 6f6e 5f52 6f77 312e 7368 6f77 2829 0a20  on_Row1.show(). 
-0000eb90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000eba0: 4275 7474 6f6e 5f52 6f77 322e 7368 6f77  Button_Row2.show
-0000ebb0: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
-0000ebc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000ebd0: 662e 4275 7474 6f6e 5f52 6f77 312e 6869  f.Button_Row1.hi
-0000ebe0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-0000ebf0: 2073 656c 662e 4275 7474 6f6e 5f52 6f77   self.Button_Row
-0000ec00: 322e 6869 6465 2829 0a0a 2020 2020 6465  2.hide()..    de
-0000ec10: 6620 636f 6d6d 616e 645f 6275 7474 6f6e  f command_button
-0000ec20: 735f 7374 6174 655f 6368 616e 6765 2873  s_state_change(s
-0000ec30: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000ec40: 224d 656e 7520 6974 656d 2074 6f20 7368  "Menu item to sh
-0000ec50: 6f77 2f68 6964 6520 636f 6d6d 616e 6420  ow/hide command 
-0000ec60: 6275 7474 6f6e 7322 2222 0a20 2020 2020  buttons""".     
-0000ec70: 2020 2073 656c 662e 7072 6566 5b22 636f     self.pref["co
-0000ec80: 6d6d 616e 645f 6275 7474 6f6e 7322 5d20  mmand_buttons"] 
-0000ec90: 3d20 7365 6c66 2e61 6374 696f 6e43 6f6d  = self.actionCom
-0000eca0: 6d61 6e64 5f42 7574 746f 6e73 2e69 7343  mand_Buttons.isC
-0000ecb0: 6865 636b 6564 2829 0a20 2020 2020 2020  hecked().       
-0000ecc0: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
-0000ecd0: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
-0000ece0: 2073 656c 662e 7368 6f77 5f63 6f6d 6d61   self.show_comma
-0000ecf0: 6e64 5f62 7574 746f 6e73 2829 0a0a 2020  nd_buttons()..  
-0000ed00: 2020 6465 6620 7368 6f77 5f63 6f6d 6d61    def show_comma
-0000ed10: 6e64 5f62 7574 746f 6e73 2873 656c 6629  nd_buttons(self)
-0000ed20: 3a0a 2020 2020 2020 2020 2222 2263 6f6d  :.        """com
-0000ed30: 6d61 6e64 2062 7574 746f 6e20 7374 6174  mand button stat
-0000ed40: 6520 6368 616e 6765 2222 220a 2020 2020  e change""".    
-0000ed50: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-0000ed60: 2e67 6574 2822 636f 6d6d 616e 645f 6275  .get("command_bu
-0000ed70: 7474 6f6e 7322 293a 0a20 2020 2020 2020  ttons"):.       
-0000ed80: 2020 2020 2073 656c 662e 436f 6d6d 616e       self.Comman
-0000ed90: 645f 4275 7474 6f6e 732e 7368 6f77 2829  d_Buttons.show()
-0000eda0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000edb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000edc0: 436f 6d6d 616e 645f 4275 7474 6f6e 732e  Command_Buttons.
-0000edd0: 6869 6465 2829 0a0a 2020 2020 6465 6620  hide()..    def 
-0000ede0: 6973 5f66 6c6f 6174 6162 6c65 2873 656c  is_floatable(sel
-0000edf0: 662c 2069 7465 6d3a 2073 7472 2920 2d3e  f, item: str) ->
-0000ee00: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-0000ee10: 2222 6368 6563 6b20 746f 2073 6565 2069  ""check to see i
-0000ee20: 6620 7374 7269 6e67 2063 616e 2062 6520  f string can be 
-0000ee30: 6120 666c 6f61 7422 2222 0a20 2020 2020  a float""".     
-0000ee40: 2020 2069 6620 6974 656d 2e69 736e 756d     if item.isnum
-0000ee50: 6572 6963 2829 3a0a 2020 2020 2020 2020  eric():.        
-0000ee60: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0000ee70: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000ee80: 2020 2020 2020 2020 205f 7465 7374 203d           _test =
-0000ee90: 2066 6c6f 6174 2869 7465 6d29 0a20 2020   float(item).   
-0000eea0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-0000eeb0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-0000eec0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-0000eed0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000eee0: 5472 7565 0a0a 2020 2020 6465 6620 6f74  True..    def ot
-0000eef0: 6865 725f 325f 6368 616e 6765 6428 7365  her_2_changed(se
-0000ef00: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000ef10: 4361 6c6c 6564 2077 6865 6e20 7765 206e  Called when we n
-0000ef20: 6565 6420 746f 2070 6172 7365 2053 5320  eed to parse SS 
-0000ef30: 6578 6368 616e 6765 2e22 2222 0a20 2020  exchange.""".   
-0000ef40: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-0000ef50: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
-0000ef60: 2020 6966 2022 4152 524c 2053 7765 6570    if "ARRL Sweep
-0000ef70: 7374 616b 6573 2220 696e 2073 656c 662e  stakes" in self.
-0000ef80: 636f 6e74 6573 742e 6e61 6d65 3a0a 2020  contest.name:.  
-0000ef90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000efa0: 6c66 2e63 6f6e 7465 7374 2e70 6172 7365  lf.contest.parse
-0000efb0: 5f65 7863 6861 6e67 6528 7365 6c66 290a  _exchange(self).
-0000efc0: 0a20 2020 2064 6566 2063 616c 6c73 6967  .    def callsig
-0000efd0: 6e5f 6368 616e 6765 6428 7365 6c66 293a  n_changed(self):
-0000efe0: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
-0000eff0: 6564 2077 6865 6e20 7465 7874 2069 6e20  ed when text in 
-0000f000: 7468 6520 6361 6c6c 7369 676e 2066 6965  the callsign fie
-0000f010: 6c64 2068 6173 2063 6861 6e67 6564 2222  ld has changed""
-0000f020: 220a 2020 2020 2020 2020 7465 7874 203d  ".        text =
-0000f030: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
-0000f040: 6578 7428 290a 2020 2020 2020 2020 7465  ext().        te
-0000f050: 7874 203d 2074 6578 742e 7570 7065 7228  xt = text.upper(
-0000f060: 290a 2020 2020 2020 2020 706f 7369 7469  ).        positi
-0000f070: 6f6e 203d 2073 656c 662e 6361 6c6c 7369  on = self.callsi
-0000f080: 676e 2e63 7572 736f 7250 6f73 6974 696f  gn.cursorPositio
-0000f090: 6e28 290a 2020 2020 2020 2020 7374 7269  n().        stri
-0000f0a0: 7070 6564 5f74 6578 7420 3d20 7465 7874  pped_text = text
-0000f0b0: 2e73 7472 6970 2829 2e72 6570 6c61 6365  .strip().replace
-0000f0c0: 2822 2022 2c20 2222 290a 2020 2020 2020  (" ", "").      
-0000f0d0: 2020 7365 6c66 2e63 616c 6c73 6967 6e2e    self.callsign.
-0000f0e0: 7365 7454 6578 7428 7374 7269 7070 6564  setText(stripped
-0000f0f0: 5f74 6578 7429 0a20 2020 2020 2020 2073  _text).        s
-0000f100: 656c 662e 6361 6c6c 7369 676e 2e73 6574  elf.callsign.set
-0000f110: 4375 7273 6f72 506f 7369 7469 6f6e 2870  CursorPosition(p
-0000f120: 6f73 6974 696f 6e29 0a0a 2020 2020 2020  osition)..      
-0000f130: 2020 6966 2022 2022 2069 6e20 7465 7874    if " " in text
-0000f140: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000f150: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
-0000f160: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
-0000f170: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000f180: 6d6f 6465 2822 4357 2229 0a20 2020 2020  mode("CW").     
-0000f190: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f1a0: 7261 6469 6f5f 7374 6174 655b 226d 6f64  radio_state["mod
-0000f1b0: 6522 5d20 3d20 2243 5722 0a20 2020 2020  e"] = "CW".     
-0000f1c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000f1d0: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 3a0a  lf.rig_control:.
-0000f1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1f0: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
-0000f200: 636f 6e74 726f 6c2e 6f6e 6c69 6e65 3a0a  control.online:.
-0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
-0000f230: 5f63 6f6e 7472 6f6c 2e73 6574 5f6d 6f64  _control.set_mod
-0000f240: 6528 2243 5722 290a 2020 2020 2020 2020  e("CW").        
-0000f250: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000f260: 5f77 696e 646f 775f 7469 746c 6528 290a  _window_title().
-0000f270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f280: 7365 6c66 2e63 6c65 6172 696e 7075 7473  self.clearinputs
-0000f290: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000f2a0: 2020 2073 656c 662e 7265 6164 5f63 775f     self.read_cw_
-0000f2b0: 6d61 6372 6f73 2829 0a20 2020 2020 2020  macros().       
-0000f2c0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000f2d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000f2e0: 7472 6970 7065 645f 7465 7874 203d 3d20  tripped_text == 
-0000f2f0: 2252 5454 5922 3a0a 2020 2020 2020 2020  "RTTY":.        
-0000f300: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-0000f310: 6d6f 6465 2822 5254 5459 2229 0a20 2020  mode("RTTY").   
-0000f320: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f330: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-0000f340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f350: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
-0000f360: 675f 636f 6e74 726f 6c2e 6f6e 6c69 6e65  g_control.online
-0000f370: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f380: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000f390: 6967 5f63 6f6e 7472 6f6c 2e73 6574 5f6d  ig_control.set_m
-0000f3a0: 6f64 6528 2252 5454 5922 290a 2020 2020  ode("RTTY").    
-0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000f3d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000f3e0: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
-0000f3f0: 6d6f 6465 225d 203d 2022 5254 5459 220a  mode"] = "RTTY".
-0000f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f410: 7365 6c66 2e73 6574 5f77 696e 646f 775f  self.set_window_
-0000f420: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
-0000f430: 2020 2020 2020 2020 7365 6c66 2e63 6c65          self.cle
-0000f440: 6172 696e 7075 7473 2829 0a20 2020 2020  arinputs().     
-0000f450: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000f460: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
-0000f470: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
-0000f480: 3d20 2253 5342 223a 0a20 2020 2020 2020  = "SSB":.       
-0000f490: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000f4a0: 746d 6f64 6528 2253 5342 2229 0a20 2020  tmode("SSB").   
-0000f4b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000f4c0: 696e 7428 7365 6c66 2e72 6164 696f 5f73  int(self.radio_s
-0000f4d0: 7461 7465 2e67 6574 2822 7666 6f61 222c  tate.get("vfoa",
-0000f4e0: 2030 2929 203e 2031 3030 3030 3030 303a   0)) > 10000000:
-0000f4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f500: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
-0000f510: 7374 6174 655b 226d 6f64 6522 5d20 3d20  state["mode"] = 
-0000f520: 2255 5342 220a 2020 2020 2020 2020 2020  "USB".          
-0000f530: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f550: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000f560: 5b22 6d6f 6465 225d 203d 2022 4c53 4222  ["mode"] = "LSB"
-0000f570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f580: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
-0000f590: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
-0000f5a0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000f5b0: 2e72 6967 5f63 6f6e 7472 6f6c 3a0a 2020  .rig_control:.  
-0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5d0: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
-0000f5e0: 6f6c 2e73 6574 5f6d 6f64 6528 7365 6c66  ol.set_mode(self
-0000f5f0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000f600: 2822 6d6f 6465 2229 290a 2020 2020 2020  ("mode")).      
-0000f610: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0000f620: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
-0000f630: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000f640: 662e 7265 6164 5f63 775f 6d61 6372 6f73  f.read_cw_macros
-0000f650: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000f660: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-0000f670: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
-0000f680: 645f 7465 7874 203d 3d20 224f 504f 4e22  d_text == "OPON"
-0000f690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f6a0: 2020 7365 6c66 2e67 6574 5f6f 706f 6e28    self.get_opon(
-0000f6b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f6c0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
-0000f6d0: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
-0000f6e0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000f6f0: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
-0000f700: 7065 645f 7465 7874 203d 3d20 2254 4553  ped_text == "TES
-0000f710: 5422 3a0a 2020 2020 2020 2020 2020 2020  T":.            
-0000f720: 2020 2020 7365 6c66 2e73 686f 775f 6d65      self.show_me
-0000f730: 7373 6167 655f 626f 7828 2254 6869 7320  ssage_box("This 
-0000f740: 6973 2061 2074 6573 7422 290a 2020 2020  is a test").    
-0000f750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f760: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
-0000f770: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f780: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-0000f790: 2020 6966 2073 656c 662e 6973 5f66 6c6f    if self.is_flo
-0000f7a0: 6174 6162 6c65 2873 7472 6970 7065 645f  atable(stripped_
-0000f7b0: 7465 7874 293a 0a20 2020 2020 2020 2020  text):.         
-0000f7c0: 2020 2020 2020 2076 666f 203d 2066 6c6f         vfo = flo
-0000f7d0: 6174 2873 7472 6970 7065 645f 7465 7874  at(stripped_text
-0000f7e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f7f0: 2020 7666 6f20 3d20 696e 7428 7666 6f20    vfo = int(vfo 
-0000f800: 2a20 3130 3030 290a 2020 2020 2020 2020  * 1000).        
-0000f810: 2020 2020 2020 2020 6261 6e64 203d 2067          band = g
-0000f820: 6574 6261 6e64 2873 7472 2876 666f 2929  etband(str(vfo))
-0000f830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f840: 2073 656c 662e 7365 745f 6261 6e64 5f69   self.set_band_i
-0000f850: 6e64 6963 6174 6f72 2862 616e 6429 0a20  ndicator(band). 
-0000f860: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f870: 2073 656c 662e 636f 6e74 6163 745b 2242   self.contact["B
-0000f880: 616e 6422 5d20 3d20 6765 745f 6c6f 6767  and"] = get_logg
-0000f890: 6564 5f62 616e 6428 7374 7228 7365 6c66  ed_band(str(self
-0000f8a0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000f8b0: 2822 7666 6f61 222c 2030 2e30 2929 290a  ("vfoa", 0.0))).
-0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8d0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-0000f8e0: 5b22 7666 6f61 225d 203d 2076 666f 0a20  ["vfoa"] = vfo. 
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f900: 656c 662e 7365 745f 7769 6e64 6f77 5f74  elf.set_window_t
-0000f910: 6974 6c65 2829 0a20 2020 2020 2020 2020  itle().         
-0000f920: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
-0000f930: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
-0000f940: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000f950: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
-0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f970: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-0000f980: 726f 6c2e 7365 745f 7666 6f28 7666 6f29  rol.set_vfo(vfo)
-0000f990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f9a0: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-0000f9b0: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
-0000f9c0: 6361 6c6c 7369 676e 2873 7472 6970 7065  callsign(strippe
-0000f9d0: 645f 7465 7874 290a 2020 2020 2020 2020  d_text).        
-0000f9e0: 2020 2020 6966 2073 656c 662e 6368 6563      if self.chec
-0000f9f0: 6b5f 6475 7065 2873 7472 6970 7065 645f  k_dupe(stripped_
-0000fa00: 7465 7874 293a 0a20 2020 2020 2020 2020  text):.         
-0000fa10: 2020 2020 2020 2073 656c 662e 6475 7065         self.dupe
-0000fa20: 5f69 6e64 6963 6174 6f72 2e73 686f 7728  _indicator.show(
-0000fa30: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0000fa40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000fa50: 2020 2020 7365 6c66 2e64 7570 655f 696e      self.dupe_in
-0000fa60: 6469 6361 746f 722e 6869 6465 2829 0a20  dicator.hide(). 
-0000fa70: 2020 2020 2020 2020 2020 205f 7468 6574             _thet
-0000fa80: 6872 6561 6420 3d20 7468 7265 6164 696e  hread = threadin
-0000fa90: 672e 5468 7265 6164 280a 2020 2020 2020  g.Thread(.      
-0000faa0: 2020 2020 2020 2020 2020 7461 7267 6574            target
-0000fab0: 3d73 656c 662e 6368 6563 6b5f 6361 6c6c  =self.check_call
-0000fac0: 7369 676e 322c 0a20 2020 2020 2020 2020  sign2,.         
-0000fad0: 2020 2020 2020 2061 7267 733d 2874 6578         args=(tex
-0000fae0: 742c 292c 0a20 2020 2020 2020 2020 2020  t,),.           
-0000faf0: 2020 2020 2064 6165 6d6f 6e3d 5472 7565       daemon=True
-0000fb00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000fb10: 2020 2020 2020 2020 2020 2020 5f74 6865              _the
-0000fb20: 7468 7265 6164 2e73 7461 7274 2829 0a20  thread.start(). 
-0000fb30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fb40: 6e65 7874 5f66 6965 6c64 2e73 6574 466f  next_field.setFo
-0000fb50: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-0000fb60: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-0000fb70: 2063 6d64 203d 207b 7d0a 2020 2020 2020   cmd = {}.      
-0000fb80: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
-0000fb90: 4341 4c4c 4348 414e 4745 4422 0a20 2020  CALLCHANGED".   
-0000fba0: 2020 2020 2063 6d64 5b22 6361 6c6c 225d       cmd["call"]
-0000fbb0: 203d 2073 7472 6970 7065 645f 7465 7874   = stripped_text
-0000fbc0: 0a20 2020 2020 2020 2073 656c 662e 6d75  .        self.mu
-0000fbd0: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-0000fbe0: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-0000fbf0: 6d64 290a 2020 2020 2020 2020 7365 6c66  md).        self
-0000fc00: 2e63 6865 636b 5f63 616c 6c73 6967 6e28  .check_callsign(
-0000fc10: 7374 7269 7070 6564 5f74 6578 7429 0a0a  stripped_text)..
-0000fc20: 2020 2020 6465 6620 6368 6563 6b5f 6361      def check_ca
-0000fc30: 6c6c 7369 676e 2873 656c 662c 2063 616c  llsign(self, cal
-0000fc40: 6c73 6967 6e29 3a0a 2020 2020 2020 2020  lsign):.        
-0000fc50: 2222 2243 6865 636b 2063 616c 6c20 6173  """Check call as
-0000fc60: 2065 6e74 6572 6564 2222 220a 2020 2020   entered""".    
-0000fc70: 2020 2020 7265 7375 6c74 203d 2063 7479      result = cty
-0000fc80: 5f6c 6f6f 6b75 7028 6361 6c6c 7369 676e  _lookup(callsign
-0000fc90: 290a 2020 2020 2020 2020 6465 6275 675f  ).        debug_
-0000fca0: 7265 7375 6c74 203d 2066 227b 7265 7375  result = f"{resu
-0000fcb0: 6c74 7d22 0a20 2020 2020 2020 206c 6f67  lt}".        log
-0000fcc0: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
-0000fcd0: 6465 6275 675f 7265 7375 6c74 290a 2020  debug_result).  
-0000fce0: 2020 2020 2020 6966 2072 6573 756c 743a        if result:
-0000fcf0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000fd00: 2061 2069 6e20 7265 7375 6c74 2e69 7465   a in result.ite
-0000fd10: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000fd20: 2020 2020 2020 656e 7469 7479 203d 2061        entity = a
-0000fd30: 5b31 5d2e 6765 7428 2265 6e74 6974 7922  [1].get("entity"
-0000fd40: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-0000fd50: 2020 2020 2020 6371 203d 2061 5b31 5d2e        cq = a[1].
-0000fd60: 6765 7428 2263 7122 2c20 2222 290a 2020  get("cq", "").  
-0000fd70: 2020 2020 2020 2020 2020 2020 2020 6974                it
-0000fd80: 7520 3d20 615b 315d 2e67 6574 2822 6974  u = a[1].get("it
-0000fd90: 7522 2c20 2222 290a 2020 2020 2020 2020  u", "").        
-0000fda0: 2020 2020 2020 2020 636f 6e74 696e 656e          continen
-0000fdb0: 7420 3d20 615b 315d 2e67 6574 2822 636f  t = a[1].get("co
-0000fdc0: 6e74 696e 656e 7422 290a 2020 2020 2020  ntinent").      
-0000fdd0: 2020 2020 2020 2020 2020 6c61 7420 3d20            lat = 
-0000fde0: 666c 6f61 7428 615b 315d 2e67 6574 2822  float(a[1].get("
-0000fdf0: 6c61 7422 2c20 2230 2e30 2229 290a 2020  lat", "0.0")).  
-0000fe00: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-0000fe10: 6e20 3d20 666c 6f61 7428 615b 315d 2e67  n = float(a[1].g
-0000fe20: 6574 2822 6c6f 6e67 222c 2022 302e 3022  et("long", "0.0"
-0000fe30: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000fe40: 2020 206c 6f6e 203d 206c 6f6e 202a 202d     lon = lon * -
-0000fe50: 3120 2023 2063 7479 2e64 6174 2066 696c  1  # cty.dat fil
-0000fe60: 6520 696e 7665 7274 7320 6c6f 6e67 6974  e inverts longit
-0000fe70: 7564 6573 0a20 2020 2020 2020 2020 2020  udes.           
-0000fe80: 2020 2020 2070 7269 6d61 7279 5f70 6678       primary_pfx
-0000fe90: 203d 2061 5b31 5d2e 6765 7428 2270 7269   = a[1].get("pri
-0000fea0: 6d61 7279 5f70 6678 222c 2022 2229 0a20  mary_pfx", ""). 
-0000feb0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000fec0: 6561 6469 6e67 203d 2062 6561 7269 6e67  eading = bearing
-0000fed0: 5f77 6974 685f 6c61 746c 6f6e 2873 656c  _with_latlon(sel
-0000fee0: 662e 7374 6174 696f 6e2e 6765 7428 2247  f.station.get("G
-0000fef0: 7269 6453 7175 6172 6522 292c 206c 6174  ridSquare"), lat
-0000ff00: 2c20 6c6f 6e29 0a20 2020 2020 2020 2020  , lon).         
-0000ff10: 2020 2020 2020 206b 696c 6f6d 6574 6572         kilometer
-0000ff20: 7320 3d20 6469 7374 616e 6365 5f77 6974  s = distance_wit
-0000ff30: 685f 6c61 746c 6f6e 280a 2020 2020 2020  h_latlon(.      
-0000ff40: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ff50: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-0000ff60: 4772 6964 5371 7561 7265 2229 2c20 6c61  GridSquare"), la
-0000ff70: 742c 206c 6f6e 0a20 2020 2020 2020 2020  t, lon.         
-0000ff80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000ff90: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-0000ffa0: 6164 696e 675f 6469 7374 616e 6365 2e73  ading_distance.s
-0000ffb0: 6574 5465 7874 280a 2020 2020 2020 2020  etText(.        
-0000ffc0: 2020 2020 2020 2020 2020 2020 6622 5265              f"Re
-0000ffd0: 6769 6f6e 616c 2048 6467 207b 6865 6164  gional Hdg {head
-0000ffe0: 696e 677d c2b0 204c 5020 7b72 6563 6970  ing}.. LP {recip
-0000fff0: 726f 636f 6c28 6865 6164 696e 6729 7dc2  rocol(heading)}.
-00010000: b020 2f20 220a 2020 2020 2020 2020 2020  . / ".          
-00010010: 2020 2020 2020 2020 2020 6622 6469 7374            f"dist
-00010020: 616e 6365 207b 696e 7428 6b69 6c6f 6d65  ance {int(kilome
-00010030: 7465 7273 2a30 2e36 3231 3337 3129 7d6d  ters*0.621371)}m
-00010040: 6920 7b6b 696c 6f6d 6574 6572 737d 6b6d  i {kilometers}km
-00010050: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00010060: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00010070: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00010080: 5b22 436f 756e 7472 7950 7265 6669 7822  ["CountryPrefix"
-00010090: 5d20 3d20 7072 696d 6172 795f 7066 780a  ] = primary_pfx.
-000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100b0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5a4e  self.contact["ZN
-000100c0: 225d 203d 2069 6e74 2863 7129 0a20 2020  "] = int(cq).   
-000100d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000100e0: 662e 636f 6e74 6163 745b 2243 6f6e 7469  f.contact["Conti
-000100f0: 6e65 6e74 225d 203d 2063 6f6e 7469 6e65  nent"] = contine
-00010100: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00010110: 2020 2073 656c 662e 6478 5f65 6e74 6974     self.dx_entit
-00010120: 792e 7365 7454 6578 7428 0a20 2020 2020  y.setText(.     
-00010130: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00010140: 227b 7072 696d 6172 795f 7066 787d 3a20  "{primary_pfx}: 
-00010150: 7b63 6f6e 7469 6e65 6e74 7d2f 7b65 6e74  {continent}/{ent
-00010160: 6974 797d 2063 713a 7b63 717d 2069 7475  ity} cq:{cq} itu
-00010170: 3a7b 6974 757d 220a 2020 2020 2020 2020  :{itu}".        
-00010180: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010190: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000101a0: 2863 616c 6c73 6967 6e29 203e 2032 3a0a  (callsign) > 2:.
-000101b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101c0: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
-000101d0: 6573 743a 0a20 2020 2020 2020 2020 2020  est:.           
-000101e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000101f0: 662e 636f 6e74 6573 742e 7072 6566 696c  f.contest.prefil
-00010200: 6c28 7365 6c66 290a 0a20 2020 2064 6566  l(self)..    def
-00010210: 2063 6865 636b 5f63 616c 6c73 6967 6e32   check_callsign2
-00010220: 2873 656c 662c 2063 616c 6c73 6967 6e29  (self, callsign)
-00010230: 3a0a 2020 2020 2020 2020 2222 2243 6865  :.        """Che
-00010240: 636b 2063 616c 6c20 6f6e 6365 2065 6e74  ck call once ent
-00010250: 6572 6564 2222 220a 2020 2020 2020 2020  ered""".        
-00010260: 6361 6c6c 7369 676e 203d 2063 616c 6c73  callsign = calls
-00010270: 6967 6e2e 7374 7269 7028 290a 2020 2020  ign.strip().    
-00010280: 2020 2020 6465 6275 675f 6c6f 6f6b 7570      debug_lookup
-00010290: 203d 2066 227b 7365 6c66 2e6c 6f6f 6b5f   = f"{self.look_
-000102a0: 7570 7d22 0a20 2020 2020 2020 206c 6f67  up}".        log
-000102b0: 6765 722e 6465 6275 6728 2225 732c 2025  ger.debug("%s, %
-000102c0: 7322 2c20 6361 6c6c 7369 676e 2c20 6465  s", callsign, de
-000102d0: 6275 675f 6c6f 6f6b 7570 290a 2020 2020  bug_lookup).    
-000102e0: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
-000102f0: 656c 662e 6c6f 6f6b 5f75 702c 2022 7365  elf.look_up, "se
-00010300: 7373 696f 6e22 293a 0a20 2020 2020 2020  ssion"):.       
-00010310: 2020 2020 2069 6620 7365 6c66 2e6c 6f6f       if self.loo
-00010320: 6b5f 7570 2e73 6573 7369 6f6e 3a0a 2020  k_up.session:.  
-00010330: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00010340: 7370 6f6e 7365 203d 2073 656c 662e 6c6f  sponse = self.lo
-00010350: 6f6b 5f75 702e 6c6f 6f6b 7570 2863 616c  ok_up.lookup(cal
-00010360: 6c73 6967 6e29 0a20 2020 2020 2020 2020  lsign).         
-00010370: 2020 2020 2020 2064 6562 7567 5f72 6573         debug_res
-00010380: 706f 6e73 6520 3d20 6622 7b72 6573 706f  ponse = f"{respo
-00010390: 6e73 657d 220a 2020 2020 2020 2020 2020  nse}".          
-000103a0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000103b0: 7567 2822 5468 6520 5265 7370 6f6e 7365  ug("The Response
-000103c0: 3a20 2573 5c6e 222c 2064 6562 7567 5f72  : %s\n", debug_r
-000103d0: 6573 706f 6e73 6529 0a20 2020 2020 2020  esponse).       
-000103e0: 2020 2020 2020 2020 2069 6620 7265 7370           if resp
-000103f0: 6f6e 7365 3a0a 2020 2020 2020 2020 2020  onse:.          
-00010400: 2020 2020 2020 2020 2020 7468 6569 7267            theirg
-00010410: 7269 6420 3d20 7265 7370 6f6e 7365 2e67  rid = response.g
-00010420: 6574 2822 6772 6964 2229 0a20 2020 2020  et("grid").     
-00010430: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010440: 656c 662e 636f 6e74 6163 745b 2247 7269  elf.contact["Gri
-00010450: 6453 7175 6172 6522 5d20 3d20 7468 6569  dSquare"] = thei
-00010460: 7267 7269 640a 2020 2020 2020 2020 2020  rgrid.          
-00010470: 2020 2020 2020 2020 2020 5f74 6865 6972            _their
-00010480: 636f 756e 7472 7920 3d20 7265 7370 6f6e  country = respon
-00010490: 7365 2e67 6574 2822 636f 756e 7472 7922  se.get("country"
-000104a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000104b0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-000104c0: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
-000104d0: 7175 6172 6522 2c20 2222 293a 0a20 2020  quare", ""):.   
-000104e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000104f0: 2020 2020 2068 6561 6469 6e67 203d 2062       heading = b
-00010500: 6561 7269 6e67 2873 656c 662e 7374 6174  earing(self.stat
-00010510: 696f 6e2e 6765 7428 2247 7269 6453 7175  ion.get("GridSqu
-00010520: 6172 6522 2c20 2222 292c 2074 6865 6972  are", ""), their
-00010530: 6772 6964 290a 2020 2020 2020 2020 2020  grid).          
-00010540: 2020 2020 2020 2020 2020 2020 2020 6b69                ki
-00010550: 6c6f 6d65 7465 7273 203d 2064 6973 7461  lometers = dista
-00010560: 6e63 6528 7365 6c66 2e73 7461 7469 6f6e  nce(self.station
-00010570: 2e67 6574 2822 4772 6964 5371 7561 7265  .get("GridSquare
-00010580: 2229 2c20 7468 6569 7267 7269 6429 0a20  "), theirgrid). 
-00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-000105b0: 696e 675f 6469 7374 616e 6365 2e73 6574  ing_distance.set
-000105c0: 5465 7874 280a 2020 2020 2020 2020 2020  Text(.          
-000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105e0: 2020 6622 7b74 6865 6972 6772 6964 7d20    f"{theirgrid} 
-000105f0: 4864 6720 7b68 6561 6469 6e67 7dc2 b020  Hdg {heading}.. 
-00010600: 4c50 207b 7265 6369 7072 6f63 6f6c 2868  LP {reciprocol(h
-00010610: 6561 6469 6e67 297d c2b0 202f 2022 0a20  eading)}.. / ". 
-00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2020 2020 2020 2020 2020 2066 2264 6973             f"dis
-00010640: 7461 6e63 6520 7b69 6e74 286b 696c 6f6d  tance {int(kilom
-00010650: 6574 6572 732a 302e 3632 3133 3731 297d  eters*0.621371)}
-00010660: 6d69 207b 6b69 6c6f 6d65 7465 7273 7d6b  mi {kilometers}k
-00010670: 6d22 0a20 2020 2020 2020 2020 2020 2020  m".             
-00010680: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106a0: 2023 2073 656c 662e 6478 5f65 6e74 6974   # self.dx_entit
-000106b0: 792e 7365 7454 6578 7428 6622 7b74 6865  y.setText(f"{the
-000106c0: 6972 636f 756e 7472 797d 2229 0a20 2020  ircountry}").   
-000106d0: 2020 2020 2020 2020 2020 2020 2023 2065               # e
-000106e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000106f0: 2020 2020 2023 2073 656c 662e 6865 6164       # self.head
-00010700: 696e 675f 6469 7374 616e 6365 2e73 6574  ing_distance.set
-00010710: 5465 7874 2822 4c6f 6f6b 7570 2066 6169  Text("Lookup fai
-00010720: 6c65 642e 2229 0a0a 2020 2020 6465 6620  led.")..    def 
-00010730: 6368 6563 6b5f 6475 7065 2873 656c 662c  check_dupe(self,
-00010740: 2063 616c 6c3a 2073 7472 2920 2d3e 2062   call: str) -> b
-00010750: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00010760: 4368 6563 6b73 2069 6620 6120 6361 6c6c  Checks if a call
-00010770: 7369 676e 2069 7320 6120 6475 7065 206f  sign is a dupe o
-00010780: 6e20 6375 7272 656e 7420 6261 6e64 2f6d  n current band/m
-00010790: 6f64 652e 2222 220a 2020 2020 2020 2020  ode.""".        
-000107a0: 7365 6c66 2e63 6f6e 7465 7374 2e70 7265  self.contest.pre
-000107b0: 6475 7065 2873 656c 6629 0a20 2020 2020  dupe(self).     
-000107c0: 2020 2062 616e 6420 3d20 666c 6f61 7428     band = float(
-000107d0: 6765 745f 6c6f 6767 6564 5f62 616e 6428  get_logged_band(
-000107e0: 7374 7228 7365 6c66 2e72 6164 696f 5f73  str(self.radio_s
-000107f0: 7461 7465 2e67 6574 2822 7666 6f61 222c  tate.get("vfoa",
-00010800: 2030 2e30 2929 2929 0a20 2020 2020 2020   0.0)))).       
-00010810: 206d 6f64 6520 3d20 7365 6c66 2e72 6164   mode = self.rad
-00010820: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-00010830: 6465 222c 2022 2229 0a20 2020 2020 2020  de", "").       
-00010840: 2064 6562 7567 6c69 6e65 203d 2028 0a20   debugline = (. 
-00010850: 2020 2020 2020 2020 2020 2066 2243 616c             f"Cal
-00010860: 6c3a 207b 6361 6c6c 7d20 4261 6e64 3a20  l: {call} Band: 
-00010870: 7b62 616e 647d 204d 6f64 653a 207b 6d6f  {band} Mode: {mo
-00010880: 6465 7d20 4475 7065 7479 7065 3a20 7b73  de} Dupetype: {s
-00010890: 656c 662e 636f 6e74 6573 742e 6475 7065  elf.contest.dupe
-000108a0: 5f74 7970 657d 220a 2020 2020 2020 2020  _type}".        
-000108b0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-000108c0: 2e64 6562 7567 2822 2573 222c 2064 6562  .debug("%s", deb
-000108d0: 7567 6c69 6e65 290a 2020 2020 2020 2020  ugline).        
-000108e0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
-000108f0: 6475 7065 5f74 7970 6520 3d3d 2031 3a0a  dupe_type == 1:.
-00010900: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00010910: 6c74 203d 2073 656c 662e 6461 7461 6261  lt = self.databa
-00010920: 7365 2e63 6865 636b 5f64 7570 6528 6361  se.check_dupe(ca
-00010930: 6c6c 290a 2020 2020 2020 2020 6966 2073  ll).        if s
-00010940: 656c 662e 636f 6e74 6573 742e 6475 7065  elf.contest.dupe
-00010950: 5f74 7970 6520 3d3d 2032 3a0a 2020 2020  _type == 2:.    
-00010960: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00010970: 2073 656c 662e 6461 7461 6261 7365 2e63   self.database.c
-00010980: 6865 636b 5f64 7570 655f 6f6e 5f62 616e  heck_dupe_on_ban
-00010990: 6428 6361 6c6c 2c20 6261 6e64 290a 2020  d(call, band).  
-000109a0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-000109b0: 6e74 6573 742e 6475 7065 5f74 7970 6520  ntest.dupe_type 
-000109c0: 3d3d 2033 3a0a 2020 2020 2020 2020 2020  == 3:.          
-000109d0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-000109e0: 6461 7461 6261 7365 2e63 6865 636b 5f64  database.check_d
-000109f0: 7570 655f 6f6e 5f62 616e 645f 6d6f 6465  upe_on_band_mode
-00010a00: 2863 616c 6c2c 2062 616e 642c 206d 6f64  (call, band, mod
-00010a10: 6529 0a20 2020 2020 2020 2069 6620 7365  e).        if se
-00010a20: 6c66 2e63 6f6e 7465 7374 2e64 7570 655f  lf.contest.dupe_
-00010a30: 7479 7065 203d 3d20 343a 0a20 2020 2020  type == 4:.     
-00010a40: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00010a50: 7b22 6973 6475 7065 223a 2046 616c 7365  {"isdupe": False
-00010a60: 7d0a 2020 2020 2020 2020 6465 6275 676c  }.        debugl
-00010a70: 696e 6520 3d20 6622 7b72 6573 756c 747d  ine = f"{result}
-00010a80: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-00010a90: 2e64 6562 7567 2822 2573 222c 2064 6562  .debug("%s", deb
-00010aa0: 7567 6c69 6e65 290a 2020 2020 2020 2020  ugline).        
-00010ab0: 7265 7475 726e 2072 6573 756c 742e 6765  return result.ge
-00010ac0: 7428 2269 7364 7570 6522 2c20 4661 6c73  t("isdupe", Fals
-00010ad0: 6529 0a0a 2020 2020 6465 6620 7365 746d  e)..    def setm
-00010ae0: 6f64 6528 7365 6c66 2c20 6d6f 6465 3a20  ode(self, mode: 
-00010af0: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
-00010b00: 2020 2020 2020 2222 2273 7475 6220 666f        """stub fo
-00010b10: 7220 7768 656e 2074 6865 206d 6f64 6520  r when the mode 
-00010b20: 6368 616e 6765 732e 2222 220a 2020 2020  changes.""".    
-00010b30: 2020 2020 6966 206d 6f64 6520 3d3d 2022      if mode == "
-00010b40: 4357 223a 0a20 2020 2020 2020 2020 2020  CW":.           
-00010b50: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
-00010b60: 6465 203d 2022 4357 220a 2020 2020 2020  de = "CW".      
-00010b70: 2020 2020 2020 2320 7365 6c66 2e6d 6f64        # self.mod
-00010b80: 652e 7365 7454 6578 7428 2243 5722 290a  e.setText("CW").
-00010b90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010ba0: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
-00010bb0: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
-00010bc0: 2073 656c 662e 7265 6365 6976 652e 7365   self.receive.se
-00010bd0: 7454 6578 7428 2235 3939 2229 0a20 2020  tText("599").   
-00010be0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00010bf0: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
-00010c00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010c10: 6e0a 2020 2020 2020 2020 6966 206d 6f64  n.        if mod
-00010c20: 6520 3d3d 2022 5353 4222 3a0a 2020 2020  e == "SSB":.    
-00010c30: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
-00010c40: 7265 6e74 5f6d 6f64 6520 3d20 2253 5342  rent_mode = "SSB
-00010c50: 220a 2020 2020 2020 2020 2020 2020 2320  ".            # 
-00010c60: 7365 6c66 2e6d 6f64 652e 7365 7454 6578  self.mode.setTex
-00010c70: 7428 2253 5342 2229 0a20 2020 2020 2020  t("SSB").       
-00010c80: 2020 2020 2073 656c 662e 7365 6e74 2e73       self.sent.s
-00010c90: 6574 5465 7874 2822 3539 2229 0a20 2020  etText("59").   
-00010ca0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00010cb0: 6365 6976 652e 7365 7454 6578 7428 2235  ceive.setText("5
-00010cc0: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
-00010cd0: 7365 6c66 2e72 6561 645f 6377 5f6d 6163  self.read_cw_mac
-00010ce0: 726f 7328 290a 2020 2020 2020 2020 6966  ros().        if
-00010cf0: 206d 6f64 6520 3d3d 2022 5254 5459 223a   mode == "RTTY":
-00010d00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010d10: 662e 6375 7272 656e 745f 6d6f 6465 203d  f.current_mode =
-00010d20: 2022 5254 5459 220a 2020 2020 2020 2020   "RTTY".        
-00010d30: 2020 2020 2320 7365 6c66 2e6d 6f64 652e      # self.mode.
-00010d40: 7365 7454 6578 7428 2252 5454 5922 290a  setText("RTTY").
-00010d50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010d60: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
-00010d70: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
-00010d80: 7365 6c66 2e72 6563 6569 7665 2e73 6574  self.receive.set
-00010d90: 5465 7874 2822 3539 2229 0a0a 2020 2020  Text("59")..    
-00010da0: 6465 6620 6765 745f 6f70 6f6e 2873 656c  def get_opon(sel
-00010db0: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00010dc0: 7472 6c2b 4f20 6f72 204f 504f 4e20 6469  trl+O or OPON di
-00010dd0: 616c 6f67 2222 220a 2020 2020 2020 2020  alog""".        
-00010de0: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
-00010df0: 203d 204f 704f 6e28 574f 524b 494e 475f   = OpOn(WORKING_
-00010e00: 5041 5448 290a 2020 2020 2020 2020 7365  PATH).        se
-00010e10: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e61  lf.opon_dialog.a
-00010e20: 6363 6570 7465 642e 636f 6e6e 6563 7428  ccepted.connect(
-00010e30: 7365 6c66 2e6e 6577 5f6f 7029 0a20 2020  self.new_op).   
-00010e40: 2020 2020 2073 656c 662e 6f70 6f6e 5f64       self.opon_d
-00010e50: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-00010e60: 2020 6465 6620 6e65 775f 6f70 2873 656c    def new_op(sel
-00010e70: 6629 3a0a 2020 2020 2020 2020 2222 2253  f):.        """S
-00010e80: 6176 6520 6e65 7720 4f50 2222 220a 2020  ave new OP""".  
-00010e90: 2020 2020 2020 6966 2073 656c 662e 6f70        if self.op
-00010ea0: 6f6e 5f64 6961 6c6f 672e 4e65 774f 7065  on_dialog.NewOpe
-00010eb0: 7261 746f 722e 7465 7874 2829 3a0a 2020  rator.text():.  
-00010ec0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00010ed0: 7572 7265 6e74 5f6f 7020 3d20 7365 6c66  urrent_op = self
-00010ee0: 2e6f 706f 6e5f 6469 616c 6f67 2e4e 6577  .opon_dialog.New
-00010ef0: 4f70 6572 6174 6f72 2e74 6578 7428 292e  Operator.text().
-00010f00: 7570 7065 7228 290a 2020 2020 2020 2020  upper().        
-00010f10: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
-00010f20: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-00010f30: 206c 6f67 6765 722e 6465 6275 6728 224e   logger.debug("N
-00010f40: 6577 204f 703a 2025 7322 2c20 7365 6c66  ew Op: %s", self
-00010f50: 2e63 7572 7265 6e74 5f6f 7029 0a20 2020  .current_op).   
-00010f60: 2020 2020 2073 656c 662e 6d61 6b65 5f6f       self.make_o
-00010f70: 705f 6469 7228 290a 0a20 2020 2064 6566  p_dir()..    def
-00010f80: 206d 616b 655f 6f70 5f64 6972 2873 656c   make_op_dir(sel
-00010f90: 6629 3a0a 2020 2020 2020 2020 2222 2243  f):.        """C
-00010fa0: 7265 6174 6520 4f50 2064 6972 6563 746f  reate OP directo
-00010fb0: 7279 2069 6620 6974 2064 6f65 7320 6e6f  ry if it does no
-00010fc0: 7420 6578 6973 742e 2222 220a 2020 2020  t exist.""".    
-00010fd0: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
-00010fe0: 656e 745f 6f70 3a0a 2020 2020 2020 2020  ent_op:.        
-00010ff0: 2020 2020 6f70 5f70 6174 6820 3d20 5061      op_path = Pa
-00011000: 7468 2844 4154 415f 5041 5448 2920 2f20  th(DATA_PATH) / 
-00011010: 7365 6c66 2e63 7572 7265 6e74 5f6f 700a  self.current_op.
-00011020: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00011030: 6572 2e64 6562 7567 2822 6f70 5f70 6174  er.debug("op_pat
-00011040: 683a 2025 7322 2c20 7374 7228 6f70 5f70  h: %s", str(op_p
-00011050: 6174 6829 290a 2020 2020 2020 2020 2020  ath)).          
-00011060: 2020 6966 206f 705f 7061 7468 2e69 735f    if op_path.is_
-00011070: 6469 7228 2920 6973 2046 616c 7365 3a0a  dir() is False:.
-00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011090: 6c6f 6767 6572 2e64 6562 7567 2822 4372  logger.debug("Cr
-000110a0: 6561 7469 6e67 204f 7020 4469 7265 6374  eating Op Direct
-000110b0: 6f72 793a 2025 7322 2c20 7374 7228 6f70  ory: %s", str(op
-000110c0: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
-000110d0: 2020 2020 2020 2020 6f73 2e6d 6b64 6972          os.mkdir
-000110e0: 2873 7472 286f 705f 7061 7468 2929 0a20  (str(op_path)). 
-000110f0: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
-00011100: 5f70 6174 682e 6973 5f64 6972 2829 3a0a  _path.is_dir():.
-00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 736f 7572 6365 5f70 6174 6820 3d20 5061  source_path = Pa
-00011130: 7468 2857 4f52 4b49 4e47 5f50 4154 4829  th(WORKING_PATH)
-00011140: 202f 2022 6461 7461 2220 2f20 2270 686f   / "data" / "pho
-00011150: 6e65 7469 6373 220a 2020 2020 2020 2020  netics".        
-00011160: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00011170: 6562 7567 2822 736f 7572 6365 5f70 6174  ebug("source_pat
-00011180: 683a 2025 7322 2c20 7374 7228 736f 7572  h: %s", str(sour
-00011190: 6365 5f70 6174 6829 290a 2020 2020 2020  ce_path)).      
-000111a0: 2020 2020 2020 2020 2020 666f 7220 6368            for ch
-000111b0: 696c 6420 696e 2073 6f75 7263 655f 7061  ild in source_pa
-000111c0: 7468 2e69 7465 7264 6972 2829 3a0a 2020  th.iterdir():.  
-000111d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111e0: 2020 6465 7374 696e 6174 696f 6e5f 6669    destination_fi
-000111f0: 6c65 203d 206f 705f 7061 7468 202f 2063  le = op_path / c
-00011200: 6869 6c64 2e6e 616d 650a 2020 2020 2020  hild.name.      
-00011210: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00011220: 2064 6573 7469 6e61 7469 6f6e 5f66 696c   destination_fil
-00011230: 652e 6973 5f66 696c 6528 2920 6973 2046  e.is_file() is F
-00011240: 616c 7365 3a0a 2020 2020 2020 2020 2020  alse:.          
-00011250: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00011260: 6767 6572 2e64 6562 7567 2822 4465 7374  gger.debug("Dest
-00011270: 696e 6174 696f 6e3a 2025 7322 2c20 7374  ination: %s", st
-00011280: 7228 6465 7374 696e 6174 696f 6e5f 6669  r(destination_fi
-00011290: 6c65 2929 0a20 2020 2020 2020 2020 2020  le)).           
-000112a0: 2020 2020 2020 2020 2020 2020 2064 6573               des
-000112b0: 7469 6e61 7469 6f6e 5f66 696c 652e 7772  tination_file.wr
-000112c0: 6974 655f 6279 7465 7328 6368 696c 642e  ite_bytes(child.
-000112d0: 7265 6164 5f62 7974 6573 2829 290a 0a20  read_bytes()).. 
-000112e0: 2020 2064 6566 2070 6f6c 6c5f 7261 6469     def poll_radi
-000112f0: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
-00011300: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-00011310: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
-00011320: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
-00011330: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
-00011340: 5f63 6f6e 7472 6f6c 2e6f 6e6c 696e 653a  _control.online:
-00011350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011360: 2076 666f 203d 2073 656c 662e 7269 675f   vfo = self.rig_
-00011370: 636f 6e74 726f 6c2e 6765 745f 7666 6f28  control.get_vfo(
-00011380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011390: 2020 6d6f 6465 203d 2073 656c 662e 7269    mode = self.ri
-000113a0: 675f 636f 6e74 726f 6c2e 6765 745f 6d6f  g_control.get_mo
-000113b0: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-000113c0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
-000113d0: 7374 6174 655b 2270 7474 225d 203d 2073  state["ptt"] = s
-000113e0: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-000113f0: 6765 745f 7074 7428 290a 2020 2020 2020  get_ptt().      
-00011400: 2020 2020 2020 2020 2020 2320 6966 2073            # if s
-00011410: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-00011420: 6765 7428 2270 7474 222c 2030 2920 3d3d  get("ptt", 0) ==
-00011430: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00011440: 2020 2020 2320 2020 2020 7365 6c66 2e6c      #     self.l
-00011450: 6566 7464 6f74 2e73 6574 5069 786d 6170  eftdot.setPixmap
-00011460: 2873 656c 662e 6772 6565 6e64 6f74 290a  (self.greendot).
-00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011480: 2320 656c 7365 3a0a 2020 2020 2020 2020  # else:.        
-00011490: 2020 2020 2020 2020 2320 2020 2020 7365          #     se
-000114a0: 6c66 2e6c 6566 7464 6f74 2e73 6574 5069  lf.leftdot.setPi
-000114b0: 786d 6170 2873 656c 662e 7265 6464 6f74  xmap(self.reddot
-000114c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000114d0: 2020 6966 206d 6f64 6520 3d3d 2022 4357    if mode == "CW
-000114e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000114f0: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-00011500: 6f64 6528 6d6f 6465 290a 2020 2020 2020  ode(mode).      
-00011510: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00011520: 6520 3d3d 2022 4c53 4222 206f 7220 6d6f  e == "LSB" or mo
-00011530: 6465 203d 3d20 2255 5342 223a 0a20 2020  de == "USB":.   
-00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011550: 2073 656c 662e 7365 746d 6f64 6528 2253   self.setmode("S
-00011560: 5342 2229 0a20 2020 2020 2020 2020 2020  SB").           
-00011570: 2020 2020 2069 6620 6d6f 6465 203d 3d20       if mode == 
-00011580: 2252 5454 5922 3a0a 2020 2020 2020 2020  "RTTY":.        
-00011590: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000115a0: 2e73 6574 6d6f 6465 2822 5254 5459 2229  .setmode("RTTY")
-000115b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000115c0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-000115d0: 655b 2276 666f 6122 5d20 3d20 7666 6f0a  e["vfoa"] = vfo.
-000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115f0: 6261 6e64 203d 2067 6574 6261 6e64 2873  band = getband(s
-00011600: 7472 2876 666f 2929 0a20 2020 2020 2020  tr(vfo)).       
-00011610: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-00011620: 6469 6f5f 7374 6174 655b 2262 616e 6422  dio_state["band"
-00011630: 5d20 3d20 6261 6e64 0a20 2020 2020 2020  ] = band.       
-00011640: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00011650: 6e74 6163 745b 2242 616e 6422 5d20 3d20  ntact["Band"] = 
-00011660: 6765 745f 6c6f 6767 6564 5f62 616e 6428  get_logged_band(
-00011670: 7374 7228 7666 6f29 290a 2020 2020 2020  str(vfo)).      
-00011680: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00011690: 6574 5f62 616e 645f 696e 6469 6361 746f  et_band_indicato
-000116a0: 7228 6261 6e64 290a 2020 2020 2020 2020  r(band).        
-000116b0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-000116c0: 696f 5f73 7461 7465 5b22 6d6f 6465 225d  io_state["mode"]
-000116d0: 203d 206d 6f64 650a 2020 2020 2020 2020   = mode.        
-000116e0: 2020 2020 2020 2020 2320 6c6f 6767 6572          # logger
-000116f0: 2e64 6562 7567 2822 5646 4f3a 2025 7320  .debug("VFO: %s 
-00011700: 204d 4f44 453a 2025 7322 2c20 7666 6f2c   MODE: %s", vfo,
-00011710: 206d 6f64 6529 0a20 2020 2020 2020 2020   mode).         
-00011720: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-00011730: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
-00011740: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011750: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
-00011760: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00011770: 225d 203d 2022 5241 4449 4f5f 5354 4154  "] = "RADIO_STAT
-00011780: 4522 0a20 2020 2020 2020 2020 2020 2020  E".             
-00011790: 2020 2063 6d64 5b22 6261 6e64 225d 203d     cmd["band"] =
-000117a0: 2062 616e 640a 2020 2020 2020 2020 2020   band.          
-000117b0: 2020 2020 2020 636d 645b 2276 666f 6122        cmd["vfoa"
-000117c0: 5d20 3d20 7666 6f0a 2020 2020 2020 2020  ] = vfo.        
-000117d0: 2020 2020 2020 2020 636d 645b 226d 6f64          cmd["mod
-000117e0: 6522 5d20 3d20 6d6f 6465 0a20 2020 2020  e"] = mode.     
-000117f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011800: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-00011810: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-00011820: 2863 6d64 290a 0a20 2020 2064 6566 2065  (cmd)..    def e
-00011830: 6469 745f 6377 5f6d 6163 726f 7328 7365  dit_cw_macros(se
-00011840: 6c66 2920 2d3e 204e 6f6e 653a 0a20 2020  lf) -> None:.   
-00011850: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011860: 2043 616c 6c73 2074 6865 2064 6566 6175   Calls the defau
-00011870: 6c74 2074 6578 7420 6564 6974 6f72 2074  lt text editor t
-00011880: 6f20 6564 6974 2074 6865 2043 5720 6d61  o edit the CW ma
-00011890: 6372 6f20 6669 6c65 2e0a 2020 2020 2020  cro file..      
-000118a0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000118b0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-000118c0: 652e 6765 7428 226d 6f64 6522 2920 3d3d  e.get("mode") ==
-000118d0: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
-000118e0: 2020 206d 6163 726f 5f66 696c 6520 3d20     macro_file = 
-000118f0: 222f 6377 6d61 6372 6f73 2e74 7874 220a  "/cwmacros.txt".
-00011900: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00011910: 2020 2020 2020 2020 2020 6d61 6372 6f5f            macro_
-00011920: 6669 6c65 203d 2022 2f73 7362 6d61 6372  file = "/ssbmacr
-00011930: 6f73 2e74 7874 220a 2020 2020 2020 2020  os.txt".        
-00011940: 6966 206e 6f74 2050 6174 6828 4441 5441  if not Path(DATA
-00011950: 5f50 4154 4820 2b20 6d61 6372 6f5f 6669  _PATH + macro_fi
-00011960: 6c65 292e 6578 6973 7473 2829 3a0a 2020  le).exists():.  
-00011970: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00011980: 2e64 6562 7567 2822 7265 6164 5f63 775f  .debug("read_cw_
-00011990: 6d61 6372 6f73 3a20 636f 7079 696e 6720  macros: copying 
-000119a0: 6465 6661 756c 7420 6d61 6372 6f20 6669  default macro fi
-000119b0: 6c65 2e22 290a 2020 2020 2020 2020 2020  le.").          
-000119c0: 2020 636f 7079 6669 6c65 2857 4f52 4b49    copyfile(WORKI
-000119d0: 4e47 5f50 4154 4820 2b20 222f 6461 7461  NG_PATH + "/data
-000119e0: 2220 2b20 6d61 6372 6f5f 6669 6c65 2c20  " + macro_file, 
-000119f0: 4441 5441 5f50 4154 4820 2b20 6d61 6372  DATA_PATH + macr
-00011a00: 6f5f 6669 6c65 290a 2020 2020 2020 2020  o_file).        
-00011a10: 6f73 2e73 7973 7465 6d28 6622 7864 672d  os.system(f"xdg-
-00011a20: 6f70 656e 207b 4441 5441 5f50 4154 487d  open {DATA_PATH}
-00011a30: 7b6d 6163 726f 5f66 696c 657d 2229 0a0a  {macro_file}")..
-00011a40: 2020 2020 6465 6620 7265 6164 5f63 775f      def read_cw_
-00011a50: 6d61 6372 6f73 2873 656c 6629 202d 3e20  macros(self) -> 
-00011a60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00011a70: 220a 2020 2020 2020 2020 5265 6164 7320  ".        Reads 
-00011a80: 696e 2074 6865 2043 5720 6d61 6372 6f73  in the CW macros
-00011a90: 2c20 6669 7273 7473 2069 7420 6368 6563  , firsts it chec
-00011aa0: 6b73 2074 6f20 7365 6520 6966 2074 6865  ks to see if the
-00011ab0: 2066 696c 6520 6578 6973 7473 2e20 4966   file exists. If
-00011ac0: 2069 7420 646f 6573 206e 6f74 2c0a 2020   it does not,.  
-00011ad0: 2020 2020 2020 616e 6420 7468 6973 2068        and this h
-00011ae0: 6173 2062 6565 6e20 7061 636b 6167 6564  as been packaged
-00011af0: 2077 6974 6820 7079 696e 7374 616c 6c65   with pyinstalle
-00011b00: 7220 6974 2077 696c 6c20 636f 7079 2074  r it will copy t
-00011b10: 6865 2064 6566 6175 6c74 2066 696c 6520  he default file 
-00011b20: 6672 6f6d 2074 6865 0a20 2020 2020 2020  from the.       
-00011b30: 2074 656d 7020 6469 7265 6374 6f72 7920   temp directory 
-00011b40: 7468 6973 2069 7320 7275 6e6e 696e 6720  this is running 
-00011b50: 6672 6f6d 2e2e 2e20 496e 2074 6865 6f72  from... In theor
-00011b60: 792e 0a20 2020 2020 2020 2022 2222 0a0a  y..        """..
-00011b70: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011b80: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
-00011b90: 226d 6f64 6522 2920 3d3d 2022 4357 223a  "mode") == "CW":
-00011ba0: 0a20 2020 2020 2020 2020 2020 206d 6163  .            mac
-00011bb0: 726f 5f66 696c 6520 3d20 222f 6377 6d61  ro_file = "/cwma
-00011bc0: 6372 6f73 2e74 7874 220a 2020 2020 2020  cros.txt".      
-00011bd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00011be0: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
-00011bf0: 2022 2f73 7362 6d61 6372 6f73 2e74 7874   "/ssbmacros.txt
-00011c00: 220a 0a20 2020 2020 2020 2069 6620 6e6f  "..        if no
-00011c10: 7420 5061 7468 2844 4154 415f 5041 5448  t Path(DATA_PATH
-00011c20: 202b 206d 6163 726f 5f66 696c 6529 2e65   + macro_file).e
-00011c30: 7869 7374 7328 293a 0a20 2020 2020 2020  xists():.       
-00011c40: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00011c50: 6728 2272 6561 645f 6377 5f6d 6163 726f  g("read_cw_macro
-00011c60: 733a 2063 6f70 7969 6e67 2064 6566 6175  s: copying defau
-00011c70: 6c74 206d 6163 726f 2066 696c 652e 2229  lt macro file.")
-00011c80: 0a20 2020 2020 2020 2020 2020 2063 6f70  .            cop
-00011c90: 7966 696c 6528 574f 524b 494e 475f 5041  yfile(WORKING_PA
-00011ca0: 5448 202b 2022 2f64 6174 6122 202b 206d  TH + "/data" + m
-00011cb0: 6163 726f 5f66 696c 652c 2044 4154 415f  acro_file, DATA_
-00011cc0: 5041 5448 202b 206d 6163 726f 5f66 696c  PATH + macro_fil
-00011cd0: 6529 0a20 2020 2020 2020 2077 6974 6820  e).        with 
-00011ce0: 6f70 656e 2844 4154 415f 5041 5448 202b  open(DATA_PATH +
-00011cf0: 206d 6163 726f 5f66 696c 652c 2022 7222   macro_file, "r"
-00011d00: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00011d10: 3822 2920 6173 2066 696c 655f 6465 7363  8") as file_desc
-00011d20: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
-00011d30: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-00011d40: 6669 6c65 5f64 6573 6372 6970 746f 723a  file_descriptor:
-00011d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d60: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00011d70: 2020 2020 2020 2020 2020 6d6f 6465 2c20            mode, 
-00011d80: 666b 6579 2c20 6275 7474 6f6e 6e61 6d65  fkey, buttonname
-00011d90: 2c20 6377 7465 7874 203d 206c 696e 652e  , cwtext = line.
-00011da0: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
-00011db0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00011dc0: 6620 6d6f 6465 2e73 7472 6970 2829 2e75  f mode.strip().u
-00011dd0: 7070 6572 2829 203d 3d20 2252 2220 616e  pper() == "R" an
-00011de0: 6420 7365 6c66 2e70 7265 662e 6765 7428  d self.pref.get(
-00011df0: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2020 2020 7365 6c66 2e66 6b65 7973        self.fkeys
-00011e20: 5b66 6b65 792e 7374 7269 7028 295d 203d  [fkey.strip()] =
-00011e30: 2028 6275 7474 6f6e 6e61 6d65 2e73 7472   (buttonname.str
-00011e40: 6970 2829 2c20 6377 7465 7874 2e73 7472  ip(), cwtext.str
-00011e50: 6970 2829 290a 2020 2020 2020 2020 2020  ip()).          
-00011e60: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00011e70: 652e 7374 7269 7028 292e 7570 7065 7228  e.strip().upper(
-00011e80: 2920 213d 2022 5222 2061 6e64 206e 6f74  ) != "R" and not
-00011e90: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00011ea0: 7275 6e5f 7374 6174 6522 293a 0a20 2020  run_state"):.   
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 2020 2020 2073 656c 662e 666b 6579 735b       self.fkeys[
-00011ed0: 666b 6579 2e73 7472 6970 2829 5d20 3d20  fkey.strip()] = 
-00011ee0: 2862 7574 746f 6e6e 616d 652e 7374 7269  (buttonname.stri
-00011ef0: 7028 292c 2063 7774 6578 742e 7374 7269  p(), cwtext.stri
-00011f00: 7028 2929 0a20 2020 2020 2020 2020 2020  p()).           
-00011f10: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-00011f20: 6545 7272 6f72 2061 7320 6572 723a 0a20  eError as err:. 
-00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f40: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-00011f50: 7265 6164 5f63 775f 6d61 6372 6f73 3a20  read_cw_macros: 
-00011f60: 2573 222c 2065 7272 290a 2020 2020 2020  %s", err).      
-00011f70: 2020 6b65 7973 203d 2073 656c 662e 666b    keys = self.fk
-00011f80: 6579 732e 6b65 7973 2829 0a20 2020 2020  eys.keys().     
-00011f90: 2020 2069 6620 2246 3122 2069 6e20 6b65     if "F1" in ke
-00011fa0: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-00011fb0: 7365 6c66 2e46 312e 7365 7454 6578 7428  self.F1.setText(
-00011fc0: 6622 4631 3a20 7b73 656c 662e 666b 6579  f"F1: {self.fkey
-00011fd0: 735b 2746 3127 5d5b 305d 7d22 290a 2020  s['F1'][0]}").  
-00011fe0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-00011ff0: 312e 7365 7454 6f6f 6c54 6970 2873 656c  1.setToolTip(sel
-00012000: 662e 666b 6579 735b 2246 3122 5d5b 315d  f.fkeys["F1"][1]
-00012010: 290a 2020 2020 2020 2020 6966 2022 4632  ).        if "F2
-00012020: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
-00012030: 2020 2020 2020 2073 656c 662e 4632 2e73         self.F2.s
-00012040: 6574 5465 7874 2866 2246 323a 207b 7365  etText(f"F2: {se
-00012050: 6c66 2e66 6b65 7973 5b27 4632 275d 5b30  lf.fkeys['F2'][0
-00012060: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
-00012070: 2073 656c 662e 4632 2e73 6574 546f 6f6c   self.F2.setTool
-00012080: 5469 7028 7365 6c66 2e66 6b65 7973 5b22  Tip(self.fkeys["
-00012090: 4632 225d 5b31 5d29 0a20 2020 2020 2020  F2"][1]).       
-000120a0: 2069 6620 2246 3322 2069 6e20 6b65 7973   if "F3" in keys
-000120b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000120c0: 6c66 2e46 332e 7365 7454 6578 7428 6622  lf.F3.setText(f"
-000120d0: 4633 3a20 7b73 656c 662e 666b 6579 735b  F3: {self.fkeys[
-000120e0: 2746 3327 5d5b 305d 7d22 290a 2020 2020  'F3'][0]}").    
-000120f0: 2020 2020 2020 2020 7365 6c66 2e46 332e          self.F3.
-00012100: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-00012110: 666b 6579 735b 2246 3322 5d5b 315d 290a  fkeys["F3"][1]).
-00012120: 2020 2020 2020 2020 6966 2022 4634 2220          if "F4" 
-00012130: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
-00012140: 2020 2020 2073 656c 662e 4634 2e73 6574       self.F4.set
-00012150: 5465 7874 2866 2246 343a 207b 7365 6c66  Text(f"F4: {self
-00012160: 2e66 6b65 7973 5b27 4634 275d 5b30 5d7d  .fkeys['F4'][0]}
-00012170: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-00012180: 656c 662e 4634 2e73 6574 546f 6f6c 5469  elf.F4.setToolTi
-00012190: 7028 7365 6c66 2e66 6b65 7973 5b22 4634  p(self.fkeys["F4
-000121a0: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-000121b0: 6620 2246 3522 2069 6e20 6b65 7973 3a0a  f "F5" in keys:.
-000121c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000121d0: 2e46 352e 7365 7454 6578 7428 6622 4635  .F5.setText(f"F5
-000121e0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-000121f0: 3527 5d5b 305d 7d22 290a 2020 2020 2020  5'][0]}").      
-00012200: 2020 2020 2020 7365 6c66 2e46 352e 7365        self.F5.se
-00012210: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
-00012220: 6579 735b 2246 3522 5d5b 315d 290a 2020  eys["F5"][1]).  
-00012230: 2020 2020 2020 6966 2022 4636 2220 696e        if "F6" in
-00012240: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
-00012250: 2020 2073 656c 662e 4636 2e73 6574 5465     self.F6.setTe
-00012260: 7874 2866 2246 363a 207b 7365 6c66 2e66  xt(f"F6: {self.f
-00012270: 6b65 7973 5b27 4636 275d 5b30 5d7d 2229  keys['F6'][0]}")
-00012280: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012290: 662e 4636 2e73 6574 546f 6f6c 5469 7028  f.F6.setToolTip(
-000122a0: 7365 6c66 2e66 6b65 7973 5b22 4636 225d  self.fkeys["F6"]
-000122b0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
-000122c0: 2246 3722 2069 6e20 6b65 7973 3a0a 2020  "F7" in keys:.  
-000122d0: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-000122e0: 372e 7365 7454 6578 7428 6622 4637 3a20  7.setText(f"F7: 
-000122f0: 7b73 656c 662e 666b 6579 735b 2746 3727  {self.fkeys['F7'
-00012300: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
-00012310: 2020 2020 7365 6c66 2e46 372e 7365 7454      self.F7.setT
-00012320: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
-00012330: 735b 2246 3722 5d5b 315d 290a 2020 2020  s["F7"][1]).    
-00012340: 2020 2020 6966 2022 4638 2220 696e 206b      if "F8" in k
-00012350: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-00012360: 2073 656c 662e 4638 2e73 6574 5465 7874   self.F8.setText
-00012370: 2866 2246 383a 207b 7365 6c66 2e66 6b65  (f"F8: {self.fke
-00012380: 7973 5b27 4638 275d 5b30 5d7d 2229 0a20  ys['F8'][0]}"). 
-00012390: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000123a0: 4638 2e73 6574 546f 6f6c 5469 7028 7365  F8.setToolTip(se
-000123b0: 6c66 2e66 6b65 7973 5b22 4638 225d 5b31  lf.fkeys["F8"][1
-000123c0: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
-000123d0: 3922 2069 6e20 6b65 7973 3a0a 2020 2020  9" in keys:.    
-000123e0: 2020 2020 2020 2020 7365 6c66 2e46 392e          self.F9.
-000123f0: 7365 7454 6578 7428 6622 4639 3a20 7b73  setText(f"F9: {s
-00012400: 656c 662e 666b 6579 735b 2746 3927 5d5b  elf.fkeys['F9'][
-00012410: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-00012420: 2020 7365 6c66 2e46 392e 7365 7454 6f6f    self.F9.setToo
-00012430: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-00012440: 2246 3922 5d5b 315d 290a 2020 2020 2020  "F9"][1]).      
-00012450: 2020 6966 2022 4631 3022 2069 6e20 6b65    if "F10" in ke
-00012460: 7973 3a0a 2020 2020 2020 2020 2020 2020  ys:.            
-00012470: 7365 6c66 2e46 3130 2e73 6574 5465 7874  self.F10.setText
-00012480: 2866 2246 3130 3a20 7b73 656c 662e 666b  (f"F10: {self.fk
-00012490: 6579 735b 2746 3130 275d 5b30 5d7d 2229  eys['F10'][0]}")
-000124a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000124b0: 662e 4631 302e 7365 7454 6f6f 6c54 6970  f.F10.setToolTip
-000124c0: 2873 656c 662e 666b 6579 735b 2246 3130  (self.fkeys["F10
-000124d0: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
-000124e0: 6620 2246 3131 2220 696e 206b 6579 733a  f "F11" in keys:
-000124f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012500: 662e 4631 312e 7365 7454 6578 7428 6622  f.F11.setText(f"
-00012510: 4631 313a 207b 7365 6c66 2e66 6b65 7973  F11: {self.fkeys
-00012520: 5b27 4631 3127 5d5b 305d 7d22 290a 2020  ['F11'][0]}").  
-00012530: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-00012540: 3131 2e73 6574 546f 6f6c 5469 7028 7365  11.setToolTip(se
-00012550: 6c66 2e66 6b65 7973 5b22 4631 3122 5d5b  lf.fkeys["F11"][
-00012560: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-00012570: 4631 3222 2069 6e20 6b65 7973 3a0a 2020  F12" in keys:.  
-00012580: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
-00012590: 3132 2e73 6574 5465 7874 2866 2246 3132  12.setText(f"F12
-000125a0: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
-000125b0: 3132 275d 5b30 5d7d 2229 0a20 2020 2020  12'][0]}").     
-000125c0: 2020 2020 2020 2073 656c 662e 4631 322e         self.F12.
-000125d0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
-000125e0: 666b 6579 735b 2246 3132 225d 5b31 5d29  fkeys["F12"][1])
-000125f0: 0a0a 2020 2020 6465 6620 6765 6e65 7261  ..    def genera
-00012600: 7465 5f61 6469 6628 7365 6c66 293a 0a20  te_adif(self):. 
-00012610: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
-00012620: 7465 2041 4449 4622 2222 0a20 2020 2020  te ADIF""".     
-00012630: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00012640: 222a 2a2a 2a2a 2a41 4449 462a 2a2a 2a2a  "******ADIF*****
-00012650: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00012660: 636f 6e74 6573 742e 6164 6966 2873 656c  contest.adif(sel
-00012670: 6629 0a0a 2020 2020 6465 6620 6765 6e65  f)..    def gene
-00012680: 7261 7465 5f63 6162 7269 6c6c 6f28 7365  rate_cabrillo(se
-00012690: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-000126a0: 4765 6e65 7261 7465 7320 4361 6272 696c  Generates Cabril
-000126b0: 6c6f 2066 696c 652e 204d 6179 6265 2e22  lo file. Maybe."
-000126c0: 2222 0a20 2020 2020 2020 2023 2068 7474  "".        # htt
-000126d0: 7073 3a2f 2f77 7777 2e63 7177 7078 2e63  ps://www.cqwpx.c
-000126e0: 6f6d 2f63 6162 7269 6c6c 6f2e 6874 6d0a  om/cabrillo.htm.
-000126f0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00012700: 6562 7567 2822 2a2a 2a2a 2a2a 4361 6272  ebug("******Cabr
-00012710: 696c 6c6f 2a2a 2a2a 2a22 290a 2020 2020  illo*****").    
-00012720: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00012730: 2e63 6162 7269 6c6c 6f28 7365 6c66 290a  .cabrillo(self).
-00012740: 0a0a 6465 6620 6c6f 6164 5f66 6f6e 7473  ..def load_fonts
-00012750: 5f66 726f 6d5f 6469 7228 6469 7265 6374  _from_dir(direct
-00012760: 6f72 793a 2073 7472 2920 2d3e 2073 6574  ory: str) -> set
-00012770: 3a0a 2020 2020 2222 220a 2020 2020 5765  :.    """.    We
-00012780: 6c6c 2069 7420 6c6f 6164 7320 666f 6e74  ll it loads font
-00012790: 7320 6672 6f6d 2061 2064 6972 6563 746f  s from a directo
-000127a0: 7279 2e2e 2e0a 2020 2020 2222 220a 2020  ry....    """.  
-000127b0: 2020 666f 6e74 5f66 616d 696c 6965 7320    font_families 
-000127c0: 3d20 7365 7428 290a 2020 2020 666f 7220  = set().    for 
-000127d0: 5f66 6920 696e 2051 4469 7228 6469 7265  _fi in QDir(dire
-000127e0: 6374 6f72 7929 2e65 6e74 7279 496e 666f  ctory).entryInfo
-000127f0: 4c69 7374 285b 222a 2e74 7466 222c 2022  List(["*.ttf", "
-00012800: 2a2e 776f 6666 222c 2022 2a2e 776f 6666  *.woff", "*.woff
-00012810: 3222 5d29 3a0a 2020 2020 2020 2020 5f69  2"]):.        _i
-00012820: 6420 3d20 5146 6f6e 7444 6174 6162 6173  d = QFontDatabas
-00012830: 652e 6164 6441 7070 6c69 6361 7469 6f6e  e.addApplication
-00012840: 466f 6e74 285f 6669 2e61 6273 6f6c 7574  Font(_fi.absolut
-00012850: 6546 696c 6550 6174 6828 2929 0a20 2020  eFilePath()).   
-00012860: 2020 2020 2066 6f6e 745f 6661 6d69 6c69       font_famili
-00012870: 6573 207c 3d20 7365 7428 5146 6f6e 7444  es |= set(QFontD
-00012880: 6174 6162 6173 652e 6170 706c 6963 6174  atabase.applicat
-00012890: 696f 6e46 6f6e 7446 616d 696c 6965 7328  ionFontFamilies(
-000128a0: 5f69 6429 290a 2020 2020 7265 7475 726e  _id)).    return
-000128b0: 2066 6f6e 745f 6661 6d69 6c69 6573 0a0a   font_families..
-000128c0: 0a64 6566 2069 6e73 7461 6c6c 5f69 636f  .def install_ico
-000128d0: 6e73 2829 3a0a 2020 2020 2222 2249 6e73  ns():.    """Ins
-000128e0: 7461 6c6c 2069 636f 6e73 2222 220a 2020  tall icons""".  
-000128f0: 2020 6f73 2e73 7973 7465 6d28 0a20 2020    os.system(.   
-00012900: 2020 2020 2022 7864 672d 6963 6f6e 2d72       "xdg-icon-r
-00012910: 6573 6f75 7263 6520 696e 7374 616c 6c20  esource install 
-00012920: 2d2d 7369 7a65 2033 3220 2d2d 636f 6e74  --size 32 --cont
-00012930: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
-00012940: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
-00012950: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
-00012960: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
-00012970: 6d2d 3332 2e70 6e67 206b 3667 7465 2d6e  m-32.png k6gte-n
-00012980: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
-00012990: 206f 732e 7379 7374 656d 280a 2020 2020   os.system(.    
-000129a0: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
-000129b0: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
-000129c0: 2d73 697a 6520 3634 202d 2d63 6f6e 7465  -size 64 --conte
-000129d0: 7874 2061 7070 7320 2d2d 6d6f 6465 2075  xt apps --mode u
-000129e0: 7365 7220 220a 2020 2020 2020 2020 6622  ser ".        f"
-000129f0: 7b57 4f52 4b49 4e47 5f50 4154 487d 2f64  {WORKING_PATH}/d
-00012a00: 6174 612f 6b36 6774 652e 6e6f 7431 6d6d  ata/k6gte.not1mm
-00012a10: 2d36 342e 706e 6720 6b36 6774 652d 6e6f  -64.png k6gte-no
-00012a20: 7431 6d6d 220a 2020 2020 290a 2020 2020  t1mm".    ).    
-00012a30: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
-00012a40: 2020 2022 7864 672d 6963 6f6e 2d72 6573     "xdg-icon-res
-00012a50: 6f75 7263 6520 696e 7374 616c 6c20 2d2d  ource install --
-00012a60: 7369 7a65 2031 3238 202d 2d63 6f6e 7465  size 128 --conte
-00012a70: 7874 2061 7070 7320 2d2d 6d6f 6465 2075  xt apps --mode u
-00012a80: 7365 7220 220a 2020 2020 2020 2020 6622  ser ".        f"
-00012a90: 7b57 4f52 4b49 4e47 5f50 4154 487d 2f64  {WORKING_PATH}/d
-00012aa0: 6174 612f 6b36 6774 652e 6e6f 7431 6d6d  ata/k6gte.not1mm
-00012ab0: 2d31 3238 2e70 6e67 206b 3667 7465 2d6e  -128.png k6gte-n
-00012ac0: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
-00012ad0: 206f 732e 7379 7374 656d 2866 2278 6467   os.system(f"xdg
-00012ae0: 2d64 6573 6b74 6f70 2d6d 656e 7520 696e  -desktop-menu in
-00012af0: 7374 616c 6c20 7b57 4f52 4b49 4e47 5f50  stall {WORKING_P
-00012b00: 4154 487d 2f64 6174 612f 6b36 6774 652d  ATH}/data/k6gte-
-00012b10: 6e6f 7431 6d6d 2e64 6573 6b74 6f70 2229  not1mm.desktop")
-00012b20: 0a0a 0a64 6566 2064 6f69 6d70 286d 6f64  ...def doimp(mod
-00012b30: 6e61 6d65 293a 0a20 2020 2022 2222 7265  name):.    """re
-00012b40: 7475 726e 206d 6f64 756c 6520 7061 7468  turn module path
-00012b50: 2222 220a 2020 2020 7265 7475 726e 2069  """.    return i
-00012b60: 6d70 6f72 746c 6962 2e69 6d70 6f72 745f  mportlib.import_
-00012b70: 6d6f 6475 6c65 2866 226e 6f74 316d 6d2e  module(f"not1mm.
-00012b80: 706c 7567 696e 732e 7b6d 6f64 6e61 6d65  plugins.{modname
-00012b90: 7d22 290a 0a0a 6465 6620 7275 6e28 293a  }")...def run():
-00012ba0: 0a20 2020 2022 2222 0a20 2020 204d 6169  .    """.    Mai
-00012bb0: 6e20 456e 7472 790a 2020 2020 2222 220a  n Entry.    """.
-00012bc0: 0a20 2020 2069 6e73 7461 6c6c 5f69 636f  .    install_ico
-00012bd0: 6e73 2829 0a20 2020 2074 696d 6572 2e73  ns().    timer.s
-00012be0: 7461 7274 2831 3030 3029 0a20 2020 2074  tart(1000).    t
-00012bf0: 696d 6572 322e 7374 6172 7428 3130 3030  imer2.start(1000
-00012c00: 290a 0a20 2020 2073 7973 2e65 7869 7428  )..    sys.exit(
-00012c10: 6170 702e 6578 6563 2829 290a 0a0a 6c6f  app.exec())...lo
-00012c20: 6767 6572 203d 206c 6f67 6769 6e67 2e67  gger = logging.g
-00012c30: 6574 4c6f 6767 6572 2822 5f5f 6d61 696e  etLogger("__main
-00012c40: 5f5f 2229 0a68 616e 646c 6572 203d 206c  __").handler = l
-00012c50: 6f67 6769 6e67 2e53 7472 6561 6d48 616e  ogging.StreamHan
-00012c60: 646c 6572 2829 0a66 6f72 6d61 7474 6572  dler().formatter
-00012c70: 203d 206c 6f67 6769 6e67 2e46 6f72 6d61   = logging.Forma
-00012c80: 7474 6572 280a 2020 2020 6461 7465 666d  tter(.    datefm
-00012c90: 743d 2225 483a 254d 3a25 5322 2c0a 2020  t="%H:%M:%S",.  
-00012ca0: 2020 666d 743d 225b 2528 6173 6374 696d    fmt="[%(asctim
-00012cb0: 6529 735d 2025 286c 6576 656c 6e61 6d65  e)s] %(levelname
-00012cc0: 2973 2025 286d 6f64 756c 6529 7320 2d20  )s %(module)s - 
-00012cd0: 2528 6675 6e63 4e61 6d65 2973 204c 696e  %(funcName)s Lin
-00012ce0: 6520 2528 6c69 6e65 6e6f 2964 3a20 2528  e %(lineno)d: %(
-00012cf0: 6d65 7373 6167 6529 7322 2c0a 290a 6861  message)s",.).ha
-00012d00: 6e64 6c65 722e 7365 7446 6f72 6d61 7474  ndler.setFormatt
-00012d10: 6572 2866 6f72 6d61 7474 6572 290a 6c6f  er(formatter).lo
-00012d20: 6767 6572 2e61 6464 4861 6e64 6c65 7228  gger.addHandler(
-00012d30: 6861 6e64 6c65 7229 0a0a 6966 2050 6174  handler)..if Pat
-00012d40: 6828 222e 2f64 6562 7567 2229 2e65 7869  h("./debug").exi
-00012d50: 7374 7328 293a 0a20 2020 206c 6f67 6765  sts():.    logge
-00012d60: 722e 7365 744c 6576 656c 286c 6f67 6769  r.setLevel(loggi
-00012d70: 6e67 2e44 4542 5547 290a 2020 2020 6c6f  ng.DEBUG).    lo
-00012d80: 6767 6572 2e64 6562 7567 2822 6465 6275  gger.debug("debu
-00012d90: 6767 696e 6720 6f6e 2229 0a65 6c73 653a  gging on").else:
-00012da0: 0a20 2020 206c 6f67 6765 722e 7365 744c  .    logger.setL
-00012db0: 6576 656c 286c 6f67 6769 6e67 2e57 4152  evel(logging.WAR
-00012dc0: 4e49 4e47 290a 2020 2020 6c6f 6767 6572  NING).    logger
-00012dd0: 2e77 6172 6e69 6e67 2822 6465 6275 6767  .warning("debugg
-00012de0: 696e 6720 6f66 6622 290a 0a61 7070 203d  ing off")..app =
-00012df0: 2051 7457 6964 6765 7473 2e51 4170 706c   QtWidgets.QAppl
-00012e00: 6963 6174 696f 6e28 7379 732e 6172 6776  ication(sys.argv
-00012e10: 290a 6170 702e 7365 7453 7479 6c65 2822  ).app.setStyle("
-00012e20: 4675 7369 6f6e 2229 0a66 6f6e 745f 7061  Fusion").font_pa
-00012e30: 7468 203d 2057 4f52 4b49 4e47 5f50 4154  th = WORKING_PAT
-00012e40: 4820 2b20 222f 6461 7461 220a 6661 6d69  H + "/data".fami
-00012e50: 6c69 6573 203d 206c 6f61 645f 666f 6e74  lies = load_font
-00012e60: 735f 6672 6f6d 5f64 6972 286f 732e 6673  s_from_dir(os.fs
-00012e70: 7061 7468 2866 6f6e 745f 7061 7468 2929  path(font_path))
-00012e80: 0a6c 6f67 6765 722e 696e 666f 2866 616d  .logger.info(fam
-00012e90: 696c 6965 7329 0a77 696e 646f 7720 3d20  ilies).window = 
-00012ea0: 4d61 696e 5769 6e64 6f77 2829 0a68 6569  MainWindow().hei
-00012eb0: 6768 7420 3d20 7769 6e64 6f77 2e70 7265  ght = window.pre
-00012ec0: 662e 6765 7428 2277 696e 646f 775f 6865  f.get("window_he
-00012ed0: 6967 6874 222c 2033 3030 290a 7769 6474  ight", 300).widt
-00012ee0: 6820 3d20 7769 6e64 6f77 2e70 7265 662e  h = window.pref.
-00012ef0: 6765 7428 2277 696e 646f 775f 7769 6474  get("window_widt
-00012f00: 6822 2c20 3730 3029 0a78 203d 2077 696e  h", 700).x = win
-00012f10: 646f 772e 7072 6566 2e67 6574 2822 7769  dow.pref.get("wi
-00012f20: 6e64 6f77 5f78 222c 202d 3129 0a79 203d  ndow_x", -1).y =
-00012f30: 2077 696e 646f 772e 7072 6566 2e67 6574   window.pref.get
-00012f40: 2822 7769 6e64 6f77 5f79 222c 202d 3129  ("window_y", -1)
-00012f50: 0a77 696e 646f 772e 7365 7447 656f 6d65  .window.setGeome
-00012f60: 7472 7928 782c 2079 2c20 7769 6474 682c  try(x, y, width,
-00012f70: 2068 6569 6768 7429 0a23 2077 696e 646f   height).# windo
-00012f80: 772e 7365 7457 696e 646f 7754 6974 6c65  w.setWindowTitle
-00012f90: 2866 224e 6f74 314d 4d20 767b 5f5f 7665  (f"Not1MM v{__ve
-00012fa0: 7273 696f 6e5f 5f7d 2229 0a77 696e 646f  rsion__}").windo
-00012fb0: 772e 6361 6c6c 7369 676e 2e73 6574 466f  w.callsign.setFo
-00012fc0: 6375 7328 290a 7769 6e64 6f77 2e73 686f  cus().window.sho
-00012fd0: 7728 290a 7469 6d65 7220 3d20 5174 436f  w().timer = QtCo
-00012fe0: 7265 2e51 5469 6d65 7228 290a 7469 6d65  re.QTimer().time
-00012ff0: 722e 7469 6d65 6f75 742e 636f 6e6e 6563  r.timeout.connec
-00013000: 7428 7769 6e64 6f77 2e70 6f6c 6c5f 7261  t(window.poll_ra
-00013010: 6469 6f29 0a74 696d 6572 3220 3d20 5174  dio).timer2 = Qt
-00013020: 436f 7265 2e51 5469 6d65 7228 290a 7469  Core.QTimer().ti
-00013030: 6d65 7232 2e74 696d 656f 7574 2e63 6f6e  mer2.timeout.con
-00013040: 6e65 6374 2877 696e 646f 772e 6368 6563  nect(window.chec
-00013050: 6b5f 7564 705f 7472 6166 6669 6329 0a0a  k_udp_traffic)..
-00013060: 6966 205f 5f6e 616d 655f 5f20 3d3d 2022  if __name__ == "
-00013070: 5f5f 6d61 696e 5f5f 223a 0a20 2020 2072  __main__":.    r
-00013080: 756e 2829 0a                             un().
+0000bee0: 2020 2020 2020 2020 2073 642e 6465 6661           sd.defa
+0000bef0: 756c 742e 6465 7669 6365 203d 2073 656c  ult.device = sel
+0000bf00: 662e 7072 6566 2e67 6574 2822 736f 756e  f.pref.get("soun
+0000bf10: 6464 6576 6963 6522 2c20 2264 6566 6175  ddevice", "defau
+0000bf20: 6c74 2229 0a20 2020 2020 2020 2020 2020  lt").           
+0000bf30: 2020 2020 2020 2020 2020 2020 2073 642e               sd.
+0000bf40: 6465 6661 756c 742e 7361 6d70 6c65 7261  default.samplera
+0000bf50: 7465 203d 2034 3431 3030 2e30 0a20 2020  te = 44100.0.   
+0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf70: 2020 2020 2073 642e 706c 6179 2864 6174       sd.play(dat
+0000bf80: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+0000bf90: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000bfa0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+0000bfb0: 7b73 642e 7761 6974 2829 7d22 290a 2020  {sd.wait()}").  
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfd0: 2020 6578 6365 7074 2073 642e 506f 7274    except sd.Port
+0000bfe0: 4175 6469 6f45 7272 6f72 2061 7320 6572  AudioError as er
+0000bff0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+0000c000: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000c010: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
+0000c020: 7b65 7272 7d22 290a 2020 2020 2020 2020  {err}").        
+0000c030: 7365 6c66 2e70 7474 5f6f 6666 2829 0a0a  self.ptt_off()..
+0000c040: 2020 2020 6465 6620 7074 745f 6f6e 2873      def ptt_on(s
+0000c050: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000c060: 2274 7572 6e20 6f6e 2070 7474 2222 220a  "turn on ptt""".
+0000c070: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000c080: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
+0000c090: 2020 2020 2020 2020 2073 656c 662e 6c65           self.le
+0000c0a0: 6674 646f 742e 7365 7450 6978 6d61 7028  ftdot.setPixmap(
+0000c0b0: 7365 6c66 2e67 7265 656e 646f 7429 0a20  self.greendot). 
+0000c0c0: 2020 2020 2020 2020 2020 2061 7070 2e70             app.p
+0000c0d0: 726f 6365 7373 4576 656e 7473 2829 0a20  rocessEvents(). 
+0000c0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c0f0: 7269 675f 636f 6e74 726f 6c2e 7074 745f  rig_control.ptt_
+0000c100: 6f6e 2829 0a0a 2020 2020 6465 6620 7074  on()..    def pt
+0000c110: 745f 6f66 6628 7365 6c66 293a 0a20 2020  t_off(self):.   
+0000c120: 2020 2020 2022 2222 7475 726e 206f 6666       """turn off
+0000c130: 2070 7474 2222 220a 2020 2020 2020 2020   ptt""".        
+0000c140: 7365 6c66 2e6c 6566 7464 6f74 2e73 6574  self.leftdot.set
+0000c150: 5069 786d 6170 2873 656c 662e 7265 6464  Pixmap(self.redd
+0000c160: 6f74 290a 2020 2020 2020 2020 6170 702e  ot).        app.
+0000c170: 7072 6f63 6573 7345 7665 6e74 7328 290a  processEvents().
+0000c180: 2020 2020 2020 2020 7365 6c66 2e72 6967          self.rig
+0000c190: 5f63 6f6e 7472 6f6c 2e70 7474 5f6f 6666  _control.ptt_off
+0000c1a0: 2829 0a0a 2020 2020 6465 6620 7365 6e64  ()..    def send
+0000c1b0: 6631 2873 656c 6629 3a0a 2020 2020 2020  f1(self):.      
+0000c1c0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000c1d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000c1e0: 6728 2246 3120 436c 6963 6b65 6422 290a  g("F1 Clicked").
+0000c1f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000c200: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000c210: 226d 6f64 6522 2920 696e 205b 2255 5342  "mode") in ["USB
+0000c220: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+0000c230: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+0000c240: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+0000c250: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000c260: 2e46 312e 746f 6f6c 5469 7028 2929 290a  .F1.toolTip())).
+0000c270: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c280: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
+0000c290: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
+0000c2a0: 2020 2023 2069 6620 7365 6c66 2e70 7265     # if self.pre
+0000c2b0: 6665 7265 6e63 652e 6765 7428 2273 656e  ference.get("sen
+0000c2c0: 645f 6e31 6d6d 5f70 6163 6b65 7473 2229  d_n1mm_packets")
+0000c2d0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000c2e0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+0000c2f0: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
+0000c300: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
+0000c310: 2073 656c 662e 4631 2e74 6578 7428 290a   self.F1.text().
+0000c320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c330: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000c340: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000c350: 6c66 2e46 312e 746f 6f6c 5469 7028 2929  lf.F1.toolTip())
+0000c360: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000c370: 3228 7365 6c66 293a 0a20 2020 2020 2020  2(self):.       
+0000c380: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000c390: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000c3a0: 2822 4632 2043 6c69 636b 6564 2229 0a20  ("F2 Clicked"). 
+0000c3b0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000c3c0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000c3d0: 6d6f 6465 2229 2069 6e20 5b22 5553 4222  mode") in ["USB"
+0000c3e0: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
+0000c3f0: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
+0000c400: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
+0000c410: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
+0000c420: 4632 2e74 6f6f 6c54 6970 2829 2929 0a20  F2.toolTip())). 
+0000c430: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c440: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
+0000c450: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
+0000c460: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
+0000c470: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
+0000c480: 6372 6f28 7365 6c66 2e46 322e 746f 6f6c  cro(self.F2.tool
+0000c490: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
+0000c4a0: 2073 656e 6466 3328 7365 6c66 293a 0a20   sendf3(self):. 
+0000c4b0: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000c4c0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000c4d0: 2e64 6562 7567 2822 4633 2043 6c69 636b  .debug("F3 Click
+0000c4e0: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000c4f0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000c500: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
+0000c510: 5b22 5553 4222 2c20 2253 5342 225d 3a0a  ["USB", "SSB"]:.
+0000c520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000c530: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
+0000c540: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000c550: 2873 656c 662e 4633 2e74 6f6f 6c54 6970  (self.F3.toolTip
+0000c560: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
+0000c570: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000c580: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
+0000c590: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+0000c5a0: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
+0000c5b0: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
+0000c5c0: 332e 746f 6f6c 5469 7028 2929 290a 0a20  3.toolTip())).. 
+0000c5d0: 2020 2064 6566 2073 656e 6466 3428 7365     def sendf4(se
+0000c5e0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000c5f0: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000c600: 6c6f 6767 6572 2e64 6562 7567 2822 4634  logger.debug("F4
+0000c610: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
+0000c620: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000c630: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000c640: 2229 2069 6e20 5b22 5553 4222 2c20 2253  ") in ["USB", "S
+0000c650: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
+0000c660: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
+0000c670: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
+0000c680: 5f6d 6163 726f 2873 656c 662e 4634 2e74  _macro(self.F4.t
+0000c690: 6f6f 6c54 6970 2829 2929 0a20 2020 2020  oolTip())).     
+0000c6a0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000c6b0: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+0000c6c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000c6d0: 6c66 2e63 772e 7365 6e64 6377 2873 656c  lf.cw.sendcw(sel
+0000c6e0: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
+0000c6f0: 7365 6c66 2e46 342e 746f 6f6c 5469 7028  self.F4.toolTip(
+0000c700: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
+0000c710: 6466 3528 7365 6c66 293a 0a20 2020 2020  df5(self):.     
+0000c720: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000c730: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000c740: 7567 2822 4635 2043 6c69 636b 6564 2229  ug("F5 Clicked")
+0000c750: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000c760: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000c770: 2822 6d6f 6465 2229 2069 6e20 5b22 5553  ("mode") in ["US
+0000c780: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
+0000c790: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
+0000c7a0: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
+0000c7b0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000c7c0: 662e 4635 2e74 6f6f 6c54 6970 2829 2929  f.F5.toolTip()))
+0000c7d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c7e0: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+0000c7f0: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+0000c800: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+0000c810: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+0000c820: 6d61 6372 6f28 7365 6c66 2e46 352e 746f  macro(self.F5.to
+0000c830: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
+0000c840: 6566 2073 656e 6466 3628 7365 6c66 293a  ef sendf6(self):
+0000c850: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000c860: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000c870: 6572 2e64 6562 7567 2822 4636 2043 6c69  er.debug("F6 Cli
+0000c880: 636b 6564 2229 0a20 2020 2020 2020 2069  cked").        i
+0000c890: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
+0000c8a0: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
+0000c8b0: 6e20 5b22 5553 4222 2c20 2253 5342 225d  n ["USB", "SSB"]
+0000c8c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000c8d0: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000c8e0: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000c8f0: 726f 2873 656c 662e 4636 2e74 6f6f 6c54  ro(self.F6.toolT
+0000c900: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000c910: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000c920: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000c930: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000c940: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000c950: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000c960: 2e46 362e 746f 6f6c 5469 7028 2929 290a  .F6.toolTip())).
+0000c970: 0a20 2020 2064 6566 2073 656e 6466 3728  .    def sendf7(
+0000c980: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000c990: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000c9a0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000c9b0: 4637 2043 6c69 636b 6564 2229 0a20 2020  F7 Clicked").   
+0000c9c0: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
+0000c9d0: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
+0000c9e0: 6465 2229 2069 6e20 5b22 5553 4222 2c20  de") in ["USB", 
+0000c9f0: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
+0000ca00: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
+0000ca10: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
+0000ca20: 7373 5f6d 6163 726f 2873 656c 662e 4637  ss_macro(self.F7
+0000ca30: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
+0000ca40: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0000ca50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ca60: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
+0000ca70: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
+0000ca80: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000ca90: 6f28 7365 6c66 2e46 372e 746f 6f6c 5469  o(self.F7.toolTi
+0000caa0: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000cab0: 656e 6466 3828 7365 6c66 293a 0a20 2020  endf8(self):.   
+0000cac0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000cad0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000cae0: 6562 7567 2822 4638 2043 6c69 636b 6564  ebug("F8 Clicked
+0000caf0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+0000cb00: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+0000cb10: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
+0000cb20: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
+0000cb30: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
+0000cb40: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
+0000cb50: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000cb60: 656c 662e 4638 2e74 6f6f 6c54 6970 2829  elf.F8.toolTip()
+0000cb70: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+0000cb80: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+0000cb90: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
+0000cba0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
+0000cbb0: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
+0000cbc0: 735f 6d61 6372 6f28 7365 6c66 2e46 382e  s_macro(self.F8.
+0000cbd0: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000cbe0: 2064 6566 2073 656e 6466 3928 7365 6c66   def sendf9(self
+0000cbf0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000cc00: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000cc10: 6767 6572 2e64 6562 7567 2822 4639 2043  gger.debug("F9 C
+0000cc20: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
+0000cc30: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000cc40: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000cc50: 2069 6e20 5b22 5553 4222 2c20 2253 5342   in ["USB", "SSB
+0000cc60: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
+0000cc70: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
+0000cc80: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
+0000cc90: 6163 726f 2873 656c 662e 4639 2e74 6f6f  acro(self.F9.too
+0000cca0: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
+0000ccb0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000ccc0: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
+0000ccd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cce0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
+0000ccf0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000cd00: 6c66 2e46 392e 746f 6f6c 5469 7028 2929  lf.F9.toolTip())
+0000cd10: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
+0000cd20: 3130 2873 656c 6629 3a0a 2020 2020 2020  10(self):.      
+0000cd30: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000cd40: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000cd50: 6728 2246 3130 2043 6c69 636b 6564 2229  g("F10 Clicked")
+0000cd60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000cd70: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000cd80: 2822 6d6f 6465 2229 2069 6e20 5b22 5553  ("mode") in ["US
+0000cd90: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
+0000cda0: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
+0000cdb0: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
+0000cdc0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000cdd0: 662e 4631 302e 746f 6f6c 5469 7028 2929  f.F10.toolTip())
+0000cde0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000cdf0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+0000ce00: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
+0000ce10: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
+0000ce20: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
+0000ce30: 5f6d 6163 726f 2873 656c 662e 4631 302e  _macro(self.F10.
+0000ce40: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
+0000ce50: 2064 6566 2073 656e 6466 3131 2873 656c   def sendf11(sel
+0000ce60: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000ce70: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000ce80: 6f67 6765 722e 6465 6275 6728 2246 3131  ogger.debug("F11
+0000ce90: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
+0000cea0: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000ceb0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000cec0: 2229 2069 6e20 5b22 5553 4222 2c20 2253  ") in ["USB", "S
+0000ced0: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
+0000cee0: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
+0000cef0: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
+0000cf00: 5f6d 6163 726f 2873 656c 662e 4631 312e  _macro(self.F11.
+0000cf10: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
+0000cf20: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000cf30: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000cf40: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
+0000cf50: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
+0000cf60: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000cf70: 2873 656c 662e 4631 312e 746f 6f6c 5469  (self.F11.toolTi
+0000cf80: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
+0000cf90: 656e 6466 3132 2873 656c 6629 3a0a 2020  endf12(self):.  
+0000cfa0: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
+0000cfb0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000cfc0: 6465 6275 6728 2246 3132 2043 6c69 636b  debug("F12 Click
+0000cfd0: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000cfe0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000cff0: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
+0000d000: 5b22 5553 4222 2c20 2253 5342 225d 3a0a  ["USB", "SSB"]:.
+0000d010: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d020: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
+0000d030: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000d040: 2873 656c 662e 4631 322e 746f 6f6c 5469  (self.F12.toolTi
+0000d050: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
+0000d060: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000d070: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
+0000d080: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+0000d090: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
+0000d0a0: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
+0000d0b0: 4631 322e 746f 6f6c 5469 7028 2929 290a  F12.toolTip())).
+0000d0c0: 0a20 2020 2064 6566 2072 756e 5f73 705f  .    def run_sp_
+0000d0d0: 6275 7474 6f6e 735f 636c 6963 6b65 6428  buttons_clicked(
+0000d0e0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000d0f0: 2222 4861 6e64 6c65 2072 756e 2f73 2670  ""Handle run/s&p
+0000d100: 206d 6f64 6522 2222 0a20 2020 2020 2020   mode""".       
+0000d110: 2073 656c 662e 7072 6566 5b22 7275 6e5f   self.pref["run_
+0000d120: 7374 6174 6522 5d20 3d20 7365 6c66 2e72  state"] = self.r
+0000d130: 6164 696f 4275 7474 6f6e 5f72 756e 2e69  adioButton_run.i
+0000d140: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
+0000d150: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
+0000d160: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
+0000d170: 2020 2073 656c 662e 7265 6164 5f63 775f     self.read_cw_
+0000d180: 6d61 6372 6f73 2829 0a0a 2020 2020 6465  macros()..    de
+0000d190: 6620 7772 6974 655f 7072 6566 6572 656e  f write_preferen
+0000d1a0: 6365 2873 656c 6629 3a0a 2020 2020 2020  ce(self):.      
+0000d1b0: 2020 2222 220a 2020 2020 2020 2020 5772    """.        Wr
+0000d1c0: 6974 6520 7072 6566 6572 656e 6365 7320  ite preferences 
+0000d1d0: 746f 206a 736f 6e20 6669 6c65 2e0a 2020  to json file..  
+0000d1e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d1f0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000d200: 2020 2077 6974 6820 6f70 656e 280a 2020     with open(.  
+0000d210: 2020 2020 2020 2020 2020 2020 2020 434f                CO
+0000d220: 4e46 4947 5f50 4154 4820 2b20 222f 6e6f  NFIG_PATH + "/no
+0000d230: 7431 6d6d 2e6a 736f 6e22 2c20 2277 7422  t1mm.json", "wt"
+0000d240: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
+0000d250: 3822 0a20 2020 2020 2020 2020 2020 2029  8".            )
+0000d260: 2061 7320 6669 6c65 5f64 6573 6372 6970   as file_descrip
+0000d270: 746f 723a 0a20 2020 2020 2020 2020 2020  tor:.           
+0000d280: 2020 2020 2066 696c 655f 6465 7363 7269       file_descri
+0000d290: 7074 6f72 2e77 7269 7465 2864 756d 7073  ptor.write(dumps
+0000d2a0: 2873 656c 662e 7072 6566 2c20 696e 6465  (self.pref, inde
+0000d2b0: 6e74 3d34 2929 0a20 2020 2020 2020 2020  nt=4)).         
+0000d2c0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000d2d0: 666f 2822 7772 6974 696e 673a 2025 7322  fo("writing: %s"
+0000d2e0: 2c20 7365 6c66 2e70 7265 6629 0a20 2020  , self.pref).   
+0000d2f0: 2020 2020 2065 7863 6570 7420 494f 4572       except IOEr
+0000d300: 726f 7220 6173 2065 7863 6570 7469 6f6e  ror as exception
+0000d310: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+0000d320: 6767 6572 2e63 7269 7469 6361 6c28 2277  gger.critical("w
+0000d330: 7269 7465 7072 6566 6572 656e 6365 733a  ritepreferences:
+0000d340: 2025 7322 2c20 6578 6365 7074 696f 6e29   %s", exception)
+0000d350: 0a0a 2020 2020 6465 6620 7265 6164 7072  ..    def readpr
+0000d360: 6566 6572 656e 6365 7328 7365 6c66 293a  eferences(self):
+0000d370: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d380: 2020 2020 2052 6573 746f 7265 2070 7265       Restore pre
+0000d390: 6665 7265 6e63 6573 2069 6620 7468 6579  ferences if they
+0000d3a0: 2065 7869 7374 2c20 6f74 6865 7277 6973   exist, otherwis
+0000d3b0: 6520 6372 6561 7465 2073 6f6d 6520 7361  e create some sa
+0000d3c0: 6e65 2064 6566 6175 6c74 732e 0a20 2020  ne defaults..   
+0000d3d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d3e0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000d3f0: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
+0000d400: 7374 7328 434f 4e46 4947 5f50 4154 4820  sts(CONFIG_PATH 
+0000d410: 2b20 222f 6e6f 7431 6d6d 2e6a 736f 6e22  + "/not1mm.json"
+0000d420: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000d430: 2020 2077 6974 6820 6f70 656e 280a 2020     with open(.  
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 2020 434f 4e46 4947 5f50 4154 4820 2b20    CONFIG_PATH + 
+0000d460: 222f 6e6f 7431 6d6d 2e6a 736f 6e22 2c20  "/not1mm.json", 
+0000d470: 2272 7422 2c20 656e 636f 6469 6e67 3d22  "rt", encoding="
+0000d480: 7574 662d 3822 0a20 2020 2020 2020 2020  utf-8".         
+0000d490: 2020 2020 2020 2029 2061 7320 6669 6c65         ) as file
+0000d4a0: 5f64 6573 6372 6970 746f 723a 0a20 2020  _descriptor:.   
+0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4c0: 2073 656c 662e 7072 6566 203d 206c 6f61   self.pref = loa
+0000d4d0: 6473 2866 696c 655f 6465 7363 7269 7074  ds(file_descript
+0000d4e0: 6f72 2e72 6561 6428 2929 0a20 2020 2020  or.read()).     
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000d500: 6f67 6765 722e 696e 666f 2822 2573 222c  ogger.info("%s",
+0000d510: 2073 656c 662e 7072 6566 290a 2020 2020   self.pref).    
+0000d520: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000d530: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000d540: 6767 6572 2e69 6e66 6f28 224e 6f20 7072  gger.info("No pr
+0000d550: 6566 6572 656e 6365 2066 696c 652e 2057  eference file. W
+0000d560: 7269 7469 6e67 2070 7265 6665 7265 6e63  riting preferenc
+0000d570: 652e 2229 0a20 2020 2020 2020 2020 2020  e.").           
+0000d580: 2020 2020 2077 6974 6820 6f70 656e 280a       with open(.
+0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5a0: 2020 2020 434f 4e46 4947 5f50 4154 4820      CONFIG_PATH 
+0000d5b0: 2b20 222f 6e6f 7431 6d6d 2e6a 736f 6e22  + "/not1mm.json"
+0000d5c0: 2c20 2277 7422 2c20 656e 636f 6469 6e67  , "wt", encoding
+0000d5d0: 3d22 7574 662d 3822 0a20 2020 2020 2020  ="utf-8".       
+0000d5e0: 2020 2020 2020 2020 2029 2061 7320 6669           ) as fi
+0000d5f0: 6c65 5f64 6573 6372 6970 746f 723a 0a20  le_descriptor:. 
+0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d610: 2020 2073 656c 662e 7072 6566 203d 2073     self.pref = s
+0000d620: 656c 662e 7072 6566 5f72 6566 2e63 6f70  elf.pref_ref.cop
+0000d630: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+0000d640: 2020 2020 2020 2020 6669 6c65 5f64 6573          file_des
+0000d650: 6372 6970 746f 722e 7772 6974 6528 6475  criptor.write(du
+0000d660: 6d70 7328 7365 6c66 2e70 7265 662c 2069  mps(self.pref, i
+0000d670: 6e64 656e 743d 3429 290a 2020 2020 2020  ndent=4)).      
+0000d680: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000d690: 6767 6572 2e69 6e66 6f28 2225 7322 2c20  gger.info("%s", 
+0000d6a0: 7365 6c66 2e70 7265 6629 0a20 2020 2020  self.pref).     
+0000d6b0: 2020 2065 7863 6570 7420 494f 4572 726f     except IOErro
+0000d6c0: 7220 6173 2065 7863 6570 7469 6f6e 3a0a  r as exception:.
+0000d6d0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000d6e0: 6572 2e63 7269 7469 6361 6c28 2245 7272  er.critical("Err
+0000d6f0: 6f72 3a20 2573 222c 2065 7863 6570 7469  or: %s", excepti
+0000d700: 6f6e 290a 0a20 2020 2020 2020 2073 656c  on)..        sel
+0000d710: 662e 6c6f 6f6b 5f75 7020 3d20 4e6f 6e65  f.look_up = None
+0000d720: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000d730: 2e70 7265 662e 6765 7428 2275 7365 7172  .pref.get("useqr
+0000d740: 7a22 293a 0a20 2020 2020 2020 2020 2020  z"):.           
+0000d750: 2073 656c 662e 6c6f 6f6b 5f75 7020 3d20   self.look_up = 
+0000d760: 5152 5a6c 6f6f 6b75 7028 0a20 2020 2020  QRZlookup(.     
+0000d770: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d780: 7072 6566 2e67 6574 2822 6c6f 6f6b 7570  pref.get("lookup
+0000d790: 7573 6572 6e61 6d65 2229 2c0a 2020 2020  username"),.    
+0000d7a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d7b0: 2e70 7265 662e 6765 7428 226c 6f6f 6b75  .pref.get("looku
+0000d7c0: 7070 6173 7377 6f72 6422 292c 0a20 2020  ppassword"),.   
+0000d7d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d7e0: 2020 2023 2069 6620 7365 6c66 2e70 7265     # if self.pre
+0000d7f0: 662e 6765 7428 2275 7365 6861 6d64 6222  f.get("usehamdb"
+0000d800: 293a 0a20 2020 2020 2020 2023 2020 2020  ):.        #    
+0000d810: 2073 656c 662e 6c6f 6f6b 5f75 7020 3d20   self.look_up = 
+0000d820: 4861 6d44 426c 6f6f 6b75 7028 290a 2020  HamDBlookup().  
+0000d830: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+0000d840: 6566 2e67 6574 2822 7573 6568 616d 7174  ef.get("usehamqt
+0000d850: 6822 293a 0a20 2020 2020 2020 2020 2020  h"):.           
+0000d860: 2073 656c 662e 6c6f 6f6b 5f75 7020 3d20   self.look_up = 
+0000d870: 4861 6d51 5448 280a 2020 2020 2020 2020  HamQTH(.        
+0000d880: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+0000d890: 662e 6765 7428 226c 6f6f 6b75 7075 7365  f.get("lookupuse
+0000d8a0: 726e 616d 6522 292c 0a20 2020 2020 2020  rname"),.       
+0000d8b0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0000d8c0: 6566 2e67 6574 2822 6c6f 6f6b 7570 7061  ef.get("lookuppa
+0000d8d0: 7373 776f 7264 2229 2c0a 2020 2020 2020  ssword"),.      
+0000d8e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000d8f0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+0000d900: 7428 2272 756e 5f73 7461 7465 2229 3a0a  t("run_state"):.
+0000d910: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d920: 2e72 6164 696f 4275 7474 6f6e 5f72 756e  .radioButton_run
+0000d930: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
+0000d940: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000d950: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000d960: 2e72 6164 696f 4275 7474 6f6e 5f73 702e  .radioButton_sp.
+0000d970: 7365 7443 6865 636b 6564 2854 7275 6529  setChecked(True)
+0000d980: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000d990: 662e 7072 6566 2e67 6574 2822 6461 726b  f.pref.get("dark
+0000d9a0: 5f6d 6f64 6522 293a 0a20 2020 2020 2020  _mode"):.       
+0000d9b0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+0000d9c0: 4461 726b 5f4d 6f64 652e 7365 7443 6865  Dark_Mode.setChe
+0000d9d0: 636b 6564 2854 7275 6529 0a20 2020 2020  cked(True).     
+0000d9e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000d9f0: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
+0000da00: 4461 726b 5f4d 6f64 652e 7365 7443 6865  Dark_Mode.setChe
+0000da10: 636b 6564 2846 616c 7365 290a 0a20 2020  cked(False)..   
+0000da20: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+0000da30: 662e 6765 7428 2263 6f6d 6d61 6e64 5f62  f.get("command_b
+0000da40: 7574 746f 6e73 2229 3a0a 2020 2020 2020  uttons"):.      
+0000da50: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+0000da60: 6e43 6f6d 6d61 6e64 5f42 7574 746f 6e73  nCommand_Buttons
+0000da70: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
+0000da80: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000da90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000daa0: 2e61 6374 696f 6e43 6f6d 6d61 6e64 5f42  .actionCommand_B
+0000dab0: 7574 746f 6e73 2e73 6574 4368 6563 6b65  uttons.setChecke
+0000dac0: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
+0000dad0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+0000dae0: 6574 2822 6377 5f6d 6163 726f 7322 293a  et("cw_macros"):
+0000daf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000db00: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
+0000db10: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
+0000db20: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+0000db30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000db40: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
+0000db50: 732e 7365 7443 6865 636b 6564 2846 616c  s.setChecked(Fal
+0000db60: 7365 290a 0a20 2020 2020 2020 2069 6620  se)..        if 
+0000db70: 7365 6c66 2e70 7265 662e 6765 7428 2262  self.pref.get("b
+0000db80: 616e 6473 5f6d 6f64 6573 2229 3a0a 2020  ands_modes"):.  
+0000db90: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000dba0: 6374 696f 6e4d 6f64 655f 616e 645f 4261  ctionMode_and_Ba
+0000dbb0: 6e64 732e 7365 7443 6865 636b 6564 2854  nds.setChecked(T
+0000dbc0: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
+0000dbd0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000dbe0: 656c 662e 6163 7469 6f6e 4d6f 6465 5f61  elf.actionMode_a
+0000dbf0: 6e64 5f42 616e 6473 2e73 6574 4368 6563  nd_Bands.setChec
+0000dc00: 6b65 6428 4661 6c73 6529 0a0a 2020 2020  ked(False)..    
+0000dc10: 2020 2020 6d75 6c74 6963 6173 745f 6772      multicast_gr
+0000dc20: 6f75 7020 3d20 7365 6c66 2e70 7265 662e  oup = self.pref.
+0000dc30: 6765 7428 226d 756c 7469 6361 7374 5f67  get("multicast_g
+0000dc40: 726f 7570 222c 2022 3232 342e 312e 312e  roup", "224.1.1.
+0000dc50: 3122 290a 2020 2020 2020 2020 6d75 6c74  1").        mult
+0000dc60: 6963 6173 745f 706f 7274 203d 2073 656c  icast_port = sel
+0000dc70: 662e 7072 6566 2e67 6574 2822 6d75 6c74  f.pref.get("mult
+0000dc80: 6963 6173 745f 706f 7274 222c 2032 3233  icast_port", 223
+0000dc90: 3929 0a20 2020 2020 2020 2069 6e74 6572  9).        inter
+0000dca0: 6661 6365 5f69 7020 3d20 7365 6c66 2e70  face_ip = self.p
+0000dcb0: 7265 662e 6765 7428 2269 6e74 6572 6661  ref.get("interfa
+0000dcc0: 6365 5f69 7022 2c20 2230 2e30 2e30 2e30  ce_ip", "0.0.0.0
+0000dcd0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0000dce0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+0000dcf0: 6163 6520 3d20 4d75 6c74 6963 6173 7428  ace = Multicast(
+0000dd00: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
+0000dd10: 7469 6361 7374 5f67 726f 7570 2c20 6d75  ticast_group, mu
+0000dd20: 6c74 6963 6173 745f 706f 7274 2c20 696e  lticast_port, in
+0000dd30: 7465 7266 6163 655f 6970 0a20 2020 2020  terface_ip.     
+0000dd40: 2020 2029 0a0a 2020 2020 2020 2020 7365     )..        se
+0000dd50: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 203d  lf.rig_control =
+0000dd60: 204e 6f6e 650a 0a20 2020 2020 2020 2069   None..        i
+0000dd70: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+0000dd80: 2275 7365 666c 7269 6722 2c20 4661 6c73  "useflrig", Fals
+0000dd90: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+0000dda0: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
+0000ddb0: 2020 2020 2020 2020 2020 2020 2020 2255                "U
+0000ddc0: 7369 6e67 2066 6c72 6967 3a20 2573 222c  sing flrig: %s",
+0000ddd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dde0: 2066 227b 7365 6c66 2e70 7265 662e 6765   f"{self.pref.ge
+0000ddf0: 7428 2743 4154 5f69 7027 297d 207b 7365  t('CAT_ip')} {se
+0000de00: 6c66 2e70 7265 662e 6765 7428 2743 4154  lf.pref.get('CAT
+0000de10: 5f70 6f72 7427 297d 222c 0a20 2020 2020  _port')}",.     
+0000de20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000de30: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+0000de40: 6e74 726f 6c20 3d20 4341 5428 0a20 2020  ntrol = CAT(.   
+0000de50: 2020 2020 2020 2020 2020 2020 2022 666c               "fl
+0000de60: 7269 6722 2c0a 2020 2020 2020 2020 2020  rig",.          
+0000de70: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+0000de80: 6765 7428 2243 4154 5f69 7022 2c20 2231  get("CAT_ip", "1
+0000de90: 3237 2e30 2e30 2e31 2229 2c0a 2020 2020  27.0.0.1"),.    
+0000dea0: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+0000deb0: 7365 6c66 2e70 7265 662e 6765 7428 2243  self.pref.get("C
+0000dec0: 4154 5f70 6f72 7422 2c20 3132 3334 3529  AT_port", 12345)
+0000ded0: 292c 0a20 2020 2020 2020 2020 2020 2029  ),.            )
+0000dee0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000def0: 2e70 7265 662e 6765 7428 2275 7365 7269  .pref.get("useri
+0000df00: 6763 746c 6422 2c20 4661 6c73 6529 3a0a  gctld", False):.
+0000df10: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000df20: 6572 2e64 6562 7567 280a 2020 2020 2020  er.debug(.      
+0000df30: 2020 2020 2020 2020 2020 2255 7369 6e67            "Using
+0000df40: 2072 6967 6374 6c64 3a20 2573 222c 0a20   rigctld: %s",. 
+0000df50: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000df60: 227b 7365 6c66 2e70 7265 662e 6765 7428  "{self.pref.get(
+0000df70: 2743 4154 5f69 7027 297d 207b 7365 6c66  'CAT_ip')} {self
+0000df80: 2e70 7265 662e 6765 7428 2743 4154 5f70  .pref.get('CAT_p
+0000df90: 6f72 7427 297d 222c 0a20 2020 2020 2020  ort')}",.       
+0000dfa0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000dfb0: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
+0000dfc0: 726f 6c20 3d20 4341 5428 0a20 2020 2020  rol = CAT(.     
+0000dfd0: 2020 2020 2020 2020 2020 2022 7269 6763             "rigc
+0000dfe0: 746c 6422 2c0a 2020 2020 2020 2020 2020  tld",.          
+0000dff0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+0000e000: 6765 7428 2243 4154 5f69 7022 2c20 2231  get("CAT_ip", "1
+0000e010: 3237 2e30 2e30 2e31 2229 2c0a 2020 2020  27.0.0.1"),.    
+0000e020: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+0000e030: 7365 6c66 2e70 7265 662e 6765 7428 2243  self.pref.get("C
+0000e040: 4154 5f70 6f72 7422 2c20 3435 3332 2929  AT_port", 4532))
+0000e050: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000e060: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000e070: 2e70 7265 662e 6765 7428 2263 7774 7970  .pref.get("cwtyp
+0000e080: 6522 2c20 3029 203d 3d20 303a 0a20 2020  e", 0) == 0:.   
+0000e090: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+0000e0a0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000e0b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000e0c0: 2020 7365 6c66 2e63 7720 3d20 4357 280a    self.cw = CW(.
+0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 696e 7428 7365 6c66 2e70 7265 662e 6765  int(self.pref.ge
+0000e0f0: 7428 2263 7774 7970 6522 2929 2c0a 2020  t("cwtype")),.  
+0000e100: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e110: 6c66 2e70 7265 662e 6765 7428 2263 7769  lf.pref.get("cwi
+0000e120: 7022 292c 0a20 2020 2020 2020 2020 2020  p"),.           
+0000e130: 2020 2020 2069 6e74 2873 656c 662e 7072       int(self.pr
+0000e140: 6566 2e67 6574 2822 6377 706f 7274 222c  ef.get("cwport",
+0000e150: 2036 3738 3929 292c 0a20 2020 2020 2020   6789)),.       
+0000e160: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000e170: 2020 2073 656c 662e 6377 2e73 7065 6564     self.cw.speed
+0000e180: 203d 2032 300a 0a20 2020 2020 2020 2073   = 20..        s
+0000e190: 656c 662e 6461 726b 5f6d 6f64 6528 290a  elf.dark_mode().
+0000e1a0: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
+0000e1b0: 775f 636f 6d6d 616e 645f 6275 7474 6f6e  w_command_button
+0000e1c0: 7328 290a 2020 2020 2020 2020 7365 6c66  s().        self
+0000e1d0: 2e73 686f 775f 4357 5f6d 6163 726f 7328  .show_CW_macros(
+0000e1e0: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
+0000e1f0: 2e73 686f 775f 6261 6e64 5f6d 6f64 6528  .show_band_mode(
+0000e200: 290a 0a20 2020 2064 6566 2077 6174 6368  )..    def watch
+0000e210: 5f75 6470 2873 656c 6629 3a0a 2020 2020  _udp(self):.    
+0000e220: 2020 2020 2222 2250 7574 7320 5544 5020      """Puts UDP 
+0000e230: 6461 7461 6772 616d 7320 696e 2061 2046  datagrams in a F
+0000e240: 4946 4f20 7175 6575 6522 2222 0a20 2020  IFO queue""".   
+0000e250: 2020 2020 2077 6869 6c65 2054 7275 653a       while True:
+0000e260: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+0000e270: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e280: 2020 6461 7461 6772 616d 203d 2073 656c    datagram = sel
+0000e290: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+0000e2a0: 7266 6163 652e 7365 7276 6572 5f75 6470  rface.server_udp
+0000e2b0: 2e72 6563 7628 3135 3030 290a 2020 2020  .recv(1500).    
+0000e2c0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000e2d0: 6572 2e64 6562 7567 2864 6174 6167 7261  er.debug(datagra
+0000e2e0: 6d2e 6465 636f 6465 2829 290a 2020 2020  m.decode()).    
+0000e2f0: 2020 2020 2020 2020 6578 6365 7074 2073          except s
+0000e300: 6f63 6b65 742e 7469 6d65 6f75 743a 0a20  ocket.timeout:. 
+0000e310: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e320: 696d 652e 736c 6565 7028 302e 3129 0a20  ime.sleep(0.1). 
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000e340: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+0000e350: 2020 2020 6966 2064 6174 6167 7261 6d3a      if datagram:
+0000e360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e370: 2073 656c 662e 7564 705f 6669 666f 2e70   self.udp_fifo.p
+0000e380: 7574 2864 6174 6167 7261 6d29 0a0a 2020  ut(datagram)..  
+0000e390: 2020 6465 6620 6368 6563 6b5f 7564 705f    def check_udp_
+0000e3a0: 7472 6166 6669 6328 7365 6c66 293a 0a20  traffic(self):. 
+0000e3b0: 2020 2020 2020 2022 2222 4368 6563 6b73         """Checks
+0000e3c0: 2055 4450 2054 7261 6666 6963 2222 220a   UDP Traffic""".
+0000e3d0: 2020 2020 2020 2020 7768 696c 6520 6e6f          while no
+0000e3e0: 7420 7365 6c66 2e75 6470 5f66 6966 6f2e  t self.udp_fifo.
+0000e3f0: 656d 7074 7928 293a 0a20 2020 2020 2020  empty():.       
+0000e400: 2020 2020 2064 6174 6167 7261 6d20 3d20       datagram = 
+0000e410: 7365 6c66 2e75 6470 5f66 6966 6f2e 6765  self.udp_fifo.ge
+0000e420: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+0000e430: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000e440: 2020 2020 2064 6562 7567 5f69 6e66 6f20       debug_info 
+0000e450: 3d20 6622 7b64 6174 6167 7261 6d2e 6465  = f"{datagram.de
+0000e460: 636f 6465 2829 7d22 0a20 2020 2020 2020  code()}".       
+0000e470: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000e480: 6465 6275 6728 6465 6275 675f 696e 666f  debug(debug_info
+0000e490: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e4a0: 2020 6a73 6f6e 5f64 6174 6120 3d20 6c6f    json_data = lo
+0000e4b0: 6164 7328 6461 7461 6772 616d 2e64 6563  ads(datagram.dec
+0000e4c0: 6f64 6528 2929 0a20 2020 2020 2020 2020  ode()).         
+0000e4d0: 2020 2065 7863 6570 7420 556e 6963 6f64     except Unicod
+0000e4e0: 6544 6563 6f64 6545 7272 6f72 2061 7320  eDecodeError as 
+0000e4f0: 6572 723a 0a20 2020 2020 2020 2020 2020  err:.           
+0000e500: 2020 2020 2074 6865 5f65 7272 6f72 203d       the_error =
+0000e510: 2066 224e 6f74 2055 6e69 636f 6465 3a20   f"Not Unicode: 
+0000e520: 7b65 7272 7d5c 6e7b 6461 7461 6772 616d  {err}\n{datagram
+0000e530: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0000e540: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000e550: 7468 655f 6572 726f 7229 0a20 2020 2020  the_error).     
+0000e560: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000e570: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+0000e580: 6578 6365 7074 204a 534f 4e44 6563 6f64  except JSONDecod
+0000e590: 6545 7272 6f72 2061 7320 6572 723a 0a20  eError as err:. 
+0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e5b0: 6865 5f65 7272 6f72 203d 2066 224e 6f74  he_error = f"Not
+0000e5c0: 204a 534f 4e3a 207b 6572 727d 5c6e 7b64   JSON: {err}\n{d
+0000e5d0: 6174 6167 7261 6d7d 220a 2020 2020 2020  atagram}".      
+0000e5e0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000e5f0: 2e64 6562 7567 2874 6865 5f65 7272 6f72  .debug(the_error
+0000e600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e610: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+0000e620: 2020 2020 2020 2069 6620 6a73 6f6e 5f64         if json_d
+0000e630: 6174 612e 6765 7428 2263 6d64 222c 2022  ata.get("cmd", "
+0000e640: 2229 203d 3d20 2247 4554 434f 4c55 4d4e  ") == "GETCOLUMN
+0000e650: 5322 3a0a 2020 2020 2020 2020 2020 2020  S":.            
+0000e660: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
+0000e670: 656c 662e 636f 6e74 6573 742c 2022 636f  elf.contest, "co
+0000e680: 6c75 6d6e 7322 293a 0a20 2020 2020 2020  lumns"):.       
+0000e690: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+0000e6a0: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+0000e6b0: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
+0000e6c0: 6d64 225d 203d 2022 5348 4f57 434f 4c55  md"] = "SHOWCOLU
+0000e6d0: 4d4e 5322 0a20 2020 2020 2020 2020 2020  MNS".           
+0000e6e0: 2020 2020 2020 2020 2063 6d64 5b22 7374           cmd["st
+0000e6f0: 6174 696f 6e22 5d20 3d20 706c 6174 666f  ation"] = platfo
+0000e700: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
+0000e710: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+0000e720: 645b 2243 4f4c 554d 4e53 225d 203d 2073  d["COLUMNS"] = s
+0000e730: 656c 662e 636f 6e74 6573 742e 636f 6c75  elf.contest.colu
+0000e740: 6d6e 730a 2020 2020 2020 2020 2020 2020  mns.            
+0000e750: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+0000e760: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+0000e770: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
+0000e780: 6429 0a20 2020 2020 2020 2020 2020 2069  d).            i
+0000e790: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+0000e7a0: 2020 2020 6a73 6f6e 5f64 6174 612e 6765      json_data.ge
+0000e7b0: 7428 2263 6d64 222c 2022 2229 203d 3d20  t("cmd", "") == 
+0000e7c0: 2254 554e 4522 0a20 2020 2020 2020 2020  "TUNE".         
+0000e7d0: 2020 2020 2020 2061 6e64 206a 736f 6e5f         and json_
+0000e7e0: 6461 7461 2e67 6574 2822 7374 6174 696f  data.get("statio
+0000e7f0: 6e22 2c20 2222 2920 3d3d 2070 6c61 7466  n", "") == platf
+0000e800: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
+0000e810: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+0000e820: 2020 2020 2020 2020 2020 2320 6227 7b22            # b'{"
+0000e830: 636d 6422 3a20 2254 554e 4522 2c20 2266  cmd": "TUNE", "f
+0000e840: 7265 7122 3a20 372e 3032 3335 2c20 2273  req": 7.0235, "s
+0000e850: 706f 7422 3a20 224d 4d30 4447 4922 7d27  pot": "MM0DGI"}'
+0000e860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e870: 2076 666f 203d 206a 736f 6e5f 6461 7461   vfo = json_data
+0000e880: 2e67 6574 2822 6672 6571 2229 0a20 2020  .get("freq").   
+0000e890: 2020 2020 2020 2020 2020 2020 2076 666f               vfo
+0000e8a0: 203d 2066 6c6f 6174 2876 666f 2920 2a20   = float(vfo) * 
+0000e8b0: 3130 3030 3030 300a 2020 2020 2020 2020  1000000.        
+0000e8c0: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
+0000e8d0: 696f 5f73 7461 7465 5b22 7666 6f61 225d  io_state["vfoa"]
+0000e8e0: 203d 2069 6e74 2876 666f 290a 2020 2020   = int(vfo).    
+0000e8f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000e900: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
+0000e910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e920: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+0000e930: 6e74 726f 6c2e 7365 745f 7666 6f28 696e  ntrol.set_vfo(in
+0000e940: 7428 7666 6f29 290a 2020 2020 2020 2020  t(vfo)).        
+0000e950: 2020 2020 2020 2020 7370 6f74 203d 206a          spot = j
+0000e960: 736f 6e5f 6461 7461 2e67 6574 2822 7370  son_data.get("sp
+0000e970: 6f74 222c 2022 2229 0a20 2020 2020 2020  ot", "").       
+0000e980: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+0000e990: 6c6c 7369 676e 2e73 6574 5465 7874 2873  llsign.setText(s
+0000e9a0: 706f 7429 0a20 2020 2020 2020 2020 2020  pot).           
+0000e9b0: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+0000e9c0: 676e 5f63 6861 6e67 6564 2829 0a20 2020  gn_changed().   
+0000e9d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000e9e0: 662e 6361 6c6c 7369 676e 2e73 6574 466f  f.callsign.setFo
+0000e9f0: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+0000ea00: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
+0000ea10: 6967 6e2e 6163 7469 7661 7465 5769 6e64  ign.activateWind
+0000ea20: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
+0000ea30: 2020 2020 2077 696e 646f 772e 7261 6973       window.rais
+0000ea40: 655f 2829 0a0a 2020 2020 6465 6620 6461  e_()..    def da
+0000ea50: 726b 5f6d 6f64 655f 7374 6174 655f 6368  rk_mode_state_ch
+0000ea60: 616e 6765 2873 656c 6629 3a0a 2020 2020  ange(self):.    
+0000ea70: 2020 2020 2222 2264 6172 6b6d 6f64 6520      """darkmode 
+0000ea80: 6472 6f70 646f 776e 2063 6865 636b 6d61  dropdown checkma
+0000ea90: 726b 2063 6861 6e67 6564 2222 220a 2020  rk changed""".  
+0000eaa0: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+0000eab0: 2264 6172 6b5f 6d6f 6465 225d 203d 2073  "dark_mode"] = s
+0000eac0: 656c 662e 6163 7469 6f6e 4461 726b 5f4d  elf.actionDark_M
+0000ead0: 6f64 652e 6973 4368 6563 6b65 6428 290a  ode.isChecked().
+0000eae0: 2020 2020 2020 2020 7365 6c66 2e77 7269          self.wri
+0000eaf0: 7465 5f70 7265 6665 7265 6e63 6528 290a  te_preference().
+0000eb00: 2020 2020 2020 2020 7365 6c66 2e64 6172          self.dar
+0000eb10: 6b5f 6d6f 6465 2829 0a0a 2020 2020 6465  k_mode()..    de
+0000eb20: 6620 6461 726b 5f6d 6f64 6528 7365 6c66  f dark_mode(self
+0000eb30: 293a 0a20 2020 2020 2020 2022 2222 6368  ):.        """ch
+0000eb40: 616e 6765 2064 6973 706c 6179 206d 6f64  ange display mod
+0000eb50: 6522 2222 0a20 2020 2020 2020 2069 6620  e""".        if 
+0000eb60: 7365 6c66 2e70 7265 662e 6765 7428 2264  self.pref.get("d
+0000eb70: 6172 6b5f 6d6f 6465 2229 3a0a 2020 2020  ark_mode"):.    
+0000eb80: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000eb90: 5374 796c 6553 6865 6574 2844 4152 4b5f  StyleSheet(DARK_
+0000eba0: 5354 594c 4553 4845 4554 290a 2020 2020  STYLESHEET).    
+0000ebb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ebc0: 2020 2020 2020 7365 6c66 2e73 6574 5374        self.setSt
+0000ebd0: 796c 6553 6865 6574 2822 2229 0a0a 2020  yleSheet("")..  
+0000ebe0: 2020 6465 6620 6377 5f6d 6163 726f 735f    def cw_macros_
+0000ebf0: 7374 6174 655f 6368 616e 6765 6428 7365  state_changed(se
+0000ec00: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000ec10: 4d65 6e75 2069 7465 6d20 746f 2073 686f  Menu item to sho
+0000ec20: 772f 6869 6465 206d 6163 726f 2062 7574  w/hide macro but
+0000ec30: 746f 6e73 2222 220a 2020 2020 2020 2020  tons""".        
+0000ec40: 7365 6c66 2e70 7265 665b 2263 775f 6d61  self.pref["cw_ma
+0000ec50: 6372 6f73 225d 203d 2073 656c 662e 6163  cros"] = self.ac
+0000ec60: 7469 6f6e 4357 5f4d 6163 726f 732e 6973  tionCW_Macros.is
+0000ec70: 4368 6563 6b65 6428 290a 2020 2020 2020  Checked().      
+0000ec80: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
+0000ec90: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
+0000eca0: 2020 7365 6c66 2e73 686f 775f 4357 5f6d    self.show_CW_m
+0000ecb0: 6163 726f 7328 290a 0a20 2020 2064 6566  acros()..    def
+0000ecc0: 2073 686f 775f 4357 5f6d 6163 726f 7328   show_CW_macros(
+0000ecd0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000ece0: 2222 6d61 6372 6f20 6275 7474 6f6e 2073  ""macro button s
+0000ecf0: 7461 7465 2063 6861 6e67 6522 2222 0a20  tate change""". 
+0000ed00: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+0000ed10: 7265 662e 6765 7428 2263 775f 6d61 6372  ref.get("cw_macr
+0000ed20: 6f73 2229 3a0a 2020 2020 2020 2020 2020  os"):.          
+0000ed30: 2020 7365 6c66 2e42 7574 746f 6e5f 526f    self.Button_Ro
+0000ed40: 7731 2e73 686f 7728 290a 2020 2020 2020  w1.show().      
+0000ed50: 2020 2020 2020 7365 6c66 2e42 7574 746f        self.Butto
+0000ed60: 6e5f 526f 7732 2e73 686f 7728 290a 2020  n_Row2.show().  
+0000ed70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000ed80: 2020 2020 2020 2020 7365 6c66 2e42 7574          self.But
+0000ed90: 746f 6e5f 526f 7731 2e68 6964 6528 290a  ton_Row1.hide().
+0000eda0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000edb0: 2e42 7574 746f 6e5f 526f 7732 2e68 6964  .Button_Row2.hid
+0000edc0: 6528 290a 0a20 2020 2064 6566 2063 6f6d  e()..    def com
+0000edd0: 6d61 6e64 5f62 7574 746f 6e73 5f73 7461  mand_buttons_sta
+0000ede0: 7465 5f63 6861 6e67 6528 7365 6c66 293a  te_change(self):
+0000edf0: 0a20 2020 2020 2020 2022 2222 4d65 6e75  .        """Menu
+0000ee00: 2069 7465 6d20 746f 2073 686f 772f 6869   item to show/hi
+0000ee10: 6465 2063 6f6d 6d61 6e64 2062 7574 746f  de command butto
+0000ee20: 6e73 2222 220a 2020 2020 2020 2020 7365  ns""".        se
+0000ee30: 6c66 2e70 7265 665b 2263 6f6d 6d61 6e64  lf.pref["command
+0000ee40: 5f62 7574 746f 6e73 225d 203d 2073 656c  _buttons"] = sel
+0000ee50: 662e 6163 7469 6f6e 436f 6d6d 616e 645f  f.actionCommand_
+0000ee60: 4275 7474 6f6e 732e 6973 4368 6563 6b65  Buttons.isChecke
+0000ee70: 6428 290a 2020 2020 2020 2020 7365 6c66  d().        self
+0000ee80: 2e77 7269 7465 5f70 7265 6665 7265 6e63  .write_preferenc
+0000ee90: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+0000eea0: 2e73 686f 775f 636f 6d6d 616e 645f 6275  .show_command_bu
+0000eeb0: 7474 6f6e 7328 290a 0a20 2020 2064 6566  ttons()..    def
+0000eec0: 2073 686f 775f 636f 6d6d 616e 645f 6275   show_command_bu
+0000eed0: 7474 6f6e 7328 7365 6c66 293a 0a20 2020  ttons(self):.   
+0000eee0: 2020 2020 2022 2222 636f 6d6d 616e 6420       """command 
+0000eef0: 6275 7474 6f6e 2073 7461 7465 2063 6861  button state cha
+0000ef00: 6e67 6522 2222 0a20 2020 2020 2020 2069  nge""".        i
+0000ef10: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
+0000ef20: 2263 6f6d 6d61 6e64 5f62 7574 746f 6e73  "command_buttons
+0000ef30: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0000ef40: 7365 6c66 2e43 6f6d 6d61 6e64 5f42 7574  self.Command_But
+0000ef50: 746f 6e73 2e73 686f 7728 290a 2020 2020  tons.show().    
+0000ef60: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ef70: 2020 2020 2020 7365 6c66 2e43 6f6d 6d61        self.Comma
+0000ef80: 6e64 5f42 7574 746f 6e73 2e68 6964 6528  nd_Buttons.hide(
+0000ef90: 290a 0a20 2020 2064 6566 2069 735f 666c  )..    def is_fl
+0000efa0: 6f61 7461 626c 6528 7365 6c66 2c20 6974  oatable(self, it
+0000efb0: 656d 3a20 7374 7229 202d 3e20 626f 6f6c  em: str) -> bool
+0000efc0: 3a0a 2020 2020 2020 2020 2222 2263 6865  :.        """che
+0000efd0: 636b 2074 6f20 7365 6520 6966 2073 7472  ck to see if str
+0000efe0: 696e 6720 6361 6e20 6265 2061 2066 6c6f  ing can be a flo
+0000eff0: 6174 2222 220a 2020 2020 2020 2020 6966  at""".        if
+0000f000: 2069 7465 6d2e 6973 6e75 6d65 7269 6328   item.isnumeric(
+0000f010: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+0000f020: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+0000f030: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000f040: 2020 2020 5f74 6573 7420 3d20 666c 6f61      _test = floa
+0000f050: 7428 6974 656d 290a 2020 2020 2020 2020  t(item).        
+0000f060: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+0000f070: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+0000f080: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+0000f090: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000f0a0: 0a20 2020 2064 6566 206f 7468 6572 5f32  .    def other_2
+0000f0b0: 5f63 6861 6e67 6564 2873 656c 6629 3a0a  _changed(self):.
+0000f0c0: 2020 2020 2020 2020 2222 2243 616c 6c65          """Calle
+0000f0d0: 6420 7768 656e 2077 6520 6e65 6564 2074  d when we need t
+0000f0e0: 6f20 7061 7273 6520 5353 2065 7863 6861  o parse SS excha
+0000f0f0: 6e67 652e 2222 220a 2020 2020 2020 2020  nge.""".        
+0000f100: 6966 2073 656c 662e 636f 6e74 6573 743a  if self.contest:
+0000f110: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000f120: 2241 5252 4c20 5377 6565 7073 7461 6b65  "ARRL Sweepstake
+0000f130: 7322 2069 6e20 7365 6c66 2e63 6f6e 7465  s" in self.conte
+0000f140: 7374 2e6e 616d 653a 0a20 2020 2020 2020  st.name:.       
+0000f150: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0000f160: 6e74 6573 742e 7061 7273 655f 6578 6368  ntest.parse_exch
+0000f170: 616e 6765 2873 656c 6629 0a0a 2020 2020  ange(self)..    
+0000f180: 6465 6620 6361 6c6c 7369 676e 5f63 6861  def callsign_cha
+0000f190: 6e67 6564 2873 656c 6629 3a0a 2020 2020  nged(self):.    
+0000f1a0: 2020 2020 2222 2243 616c 6c65 6420 7768      """Called wh
+0000f1b0: 656e 2074 6578 7420 696e 2074 6865 2063  en text in the c
+0000f1c0: 616c 6c73 6967 6e20 6669 656c 6420 6861  allsign field ha
+0000f1d0: 7320 6368 616e 6765 6422 2222 0a20 2020  s changed""".   
+0000f1e0: 2020 2020 2074 6578 7420 3d20 7365 6c66       text = self
+0000f1f0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+0000f200: 0a20 2020 2020 2020 2074 6578 7420 3d20  .        text = 
+0000f210: 7465 7874 2e75 7070 6572 2829 0a20 2020  text.upper().   
+0000f220: 2020 2020 2070 6f73 6974 696f 6e20 3d20       position = 
+0000f230: 7365 6c66 2e63 616c 6c73 6967 6e2e 6375  self.callsign.cu
+0000f240: 7273 6f72 506f 7369 7469 6f6e 2829 0a20  rsorPosition(). 
+0000f250: 2020 2020 2020 2073 7472 6970 7065 645f         stripped_
+0000f260: 7465 7874 203d 2074 6578 742e 7374 7269  text = text.stri
+0000f270: 7028 292e 7265 706c 6163 6528 2220 222c  p().replace(" ",
+0000f280: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
+0000f290: 662e 6361 6c6c 7369 676e 2e73 6574 5465  f.callsign.setTe
+0000f2a0: 7874 2873 7472 6970 7065 645f 7465 7874  xt(stripped_text
+0000f2b0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
+0000f2c0: 616c 6c73 6967 6e2e 7365 7443 7572 736f  allsign.setCurso
+0000f2d0: 7250 6f73 6974 696f 6e28 706f 7369 7469  rPosition(positi
+0000f2e0: 6f6e 290a 0a20 2020 2020 2020 2069 6620  on)..        if 
+0000f2f0: 2220 2220 696e 2074 6578 743a 0a20 2020  " " in text:.   
+0000f300: 2020 2020 2020 2020 2069 6620 7374 7269           if stri
+0000f310: 7070 6564 5f74 6578 7420 3d3d 2022 4357  pped_text == "CW
+0000f320: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000f330: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
+0000f340: 2243 5722 290a 2020 2020 2020 2020 2020  "CW").          
+0000f350: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
+0000f360: 5f73 7461 7465 5b22 6d6f 6465 225d 203d  _state["mode"] =
+0000f370: 2022 4357 220a 2020 2020 2020 2020 2020   "CW".          
+0000f380: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
+0000f390: 675f 636f 6e74 726f 6c3a 0a20 2020 2020  g_control:.     
+0000f3a0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f3b0: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
+0000f3c0: 6f6c 2e6f 6e6c 696e 653a 0a20 2020 2020  ol.online:.     
+0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3e0: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
+0000f3f0: 726f 6c2e 7365 745f 6d6f 6465 2822 4357  rol.set_mode("CW
+0000f400: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000f410: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+0000f420: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
+0000f430: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f440: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
+0000f450: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f460: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
+0000f470: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+0000f480: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+0000f490: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
+0000f4a0: 6564 5f74 6578 7420 3d3d 2022 5254 5459  ed_text == "RTTY
+0000f4b0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000f4c0: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
+0000f4d0: 2252 5454 5922 290a 2020 2020 2020 2020  "RTTY").        
+0000f4e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f4f0: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
+0000f500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f510: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
+0000f520: 7472 6f6c 2e6f 6e6c 696e 653a 0a20 2020  trol.online:.   
+0000f530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f540: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+0000f550: 6e74 726f 6c2e 7365 745f 6d6f 6465 2822  ntrol.set_mode("
+0000f560: 5254 5459 2229 0a20 2020 2020 2020 2020  RTTY").         
+0000f570: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000f580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f590: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+0000f5a0: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
+0000f5b0: 5d20 3d20 2252 5454 5922 0a20 2020 2020  ] = "RTTY".     
+0000f5c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f5d0: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
+0000f5e0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000f5f0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+0000f600: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
+0000f610: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000f620: 2020 2020 2020 2020 2069 6620 7374 7269           if stri
+0000f630: 7070 6564 5f74 6578 7420 3d3d 2022 5353  pped_text == "SS
+0000f640: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
+0000f650: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
+0000f660: 2822 5353 4222 290a 2020 2020 2020 2020  ("SSB").        
+0000f670: 2020 2020 2020 2020 6966 2069 6e74 2873          if int(s
+0000f680: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000f690: 6765 7428 2276 666f 6122 2c20 3029 2920  get("vfoa", 0)) 
+0000f6a0: 3e20 3130 3030 3030 3030 3a0a 2020 2020  > 10000000:.    
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000f6d0: 5b22 6d6f 6465 225d 203d 2022 5553 4222  ["mode"] = "USB"
+0000f6e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f6f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f710: 7261 6469 6f5f 7374 6174 655b 226d 6f64  radio_state["mod
+0000f720: 6522 5d20 3d20 224c 5342 220a 2020 2020  e"] = "LSB".    
+0000f730: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f740: 2e73 6574 5f77 696e 646f 775f 7469 746c  .set_window_titl
+0000f750: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000f760: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+0000f770: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
+0000f780: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f790: 662e 7269 675f 636f 6e74 726f 6c2e 7365  f.rig_control.se
+0000f7a0: 745f 6d6f 6465 2873 656c 662e 7261 6469  t_mode(self.radi
+0000f7b0: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
+0000f7c0: 6522 2929 0a20 2020 2020 2020 2020 2020  e")).           
+0000f7d0: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
+0000f7e0: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
+0000f7f0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
+0000f800: 645f 6377 5f6d 6163 726f 7328 290a 2020  d_cw_macros().  
+0000f810: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000f820: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+0000f830: 2069 6620 7374 7269 7070 6564 5f74 6578   if stripped_tex
+0000f840: 7420 3d3d 2022 4f50 4f4e 223a 0a20 2020  t == "OPON":.   
+0000f850: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f860: 662e 6765 745f 6f70 6f6e 2829 0a20 2020  f.get_opon().   
+0000f870: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f880: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8a0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+0000f8b0: 2020 2069 6620 7374 7269 7070 6564 5f74     if stripped_t
+0000f8c0: 6578 7420 3d3d 2022 5445 5354 223a 0a20  ext == "TEST":. 
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000f8e0: 656c 662e 7368 6f77 5f6d 6573 7361 6765  elf.show_message
+0000f8f0: 5f62 6f78 2822 5468 6973 2069 7320 6120  _box("This is a 
+0000f900: 7465 7374 2229 0a20 2020 2020 2020 2020  test").         
+0000f910: 2020 2020 2020 2073 656c 662e 636c 6561         self.clea
+0000f920: 7269 6e70 7574 7328 290a 2020 2020 2020  rinputs().      
+0000f930: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000f940: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000f950: 7365 6c66 2e69 735f 666c 6f61 7461 626c  self.is_floatabl
+0000f960: 6528 7374 7269 7070 6564 5f74 6578 7429  e(stripped_text)
+0000f970: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f980: 2020 7666 6f20 3d20 666c 6f61 7428 7374    vfo = float(st
+0000f990: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
+0000f9a0: 2020 2020 2020 2020 2020 2020 2076 666f               vfo
+0000f9b0: 203d 2069 6e74 2876 666f 202a 2031 3030   = int(vfo * 100
+0000f9c0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+0000f9d0: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
+0000f9e0: 6428 7374 7228 7666 6f29 290a 2020 2020  d(str(vfo)).    
+0000f9f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fa00: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
+0000fa10: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
+0000fa20: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+0000fa30: 2e63 6f6e 7461 6374 5b22 4261 6e64 225d  .contact["Band"]
+0000fa40: 203d 2067 6574 5f6c 6f67 6765 645f 6261   = get_logged_ba
+0000fa50: 6e64 2873 7472 2873 656c 662e 7261 6469  nd(str(self.radi
+0000fa60: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+0000fa70: 6122 2c20 302e 3029 2929 0a20 2020 2020  a", 0.0))).     
+0000fa80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000fa90: 7261 6469 6f5f 7374 6174 655b 2276 666f  radio_state["vfo
+0000faa0: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
+0000fab0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000fac0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
+0000fad0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000fae0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+0000faf0: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+0000fb00: 2020 2020 2069 6620 7365 6c66 2e72 6967       if self.rig
+0000fb10: 5f63 6f6e 7472 6f6c 3a0a 2020 2020 2020  _control:.      
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fb30: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
+0000fb40: 6574 5f76 666f 2876 666f 290a 2020 2020  et_vfo(vfo).    
+0000fb50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000fb60: 726e 0a0a 2020 2020 2020 2020 2020 2020  rn..            
+0000fb70: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
+0000fb80: 6967 6e28 7374 7269 7070 6564 5f74 6578  ign(stripped_tex
+0000fb90: 7429 0a20 2020 2020 2020 2020 2020 2069  t).            i
+0000fba0: 6620 7365 6c66 2e63 6865 636b 5f64 7570  f self.check_dup
+0000fbb0: 6528 7374 7269 7070 6564 5f74 6578 7429  e(stripped_text)
+0000fbc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fbd0: 2020 7365 6c66 2e64 7570 655f 696e 6469    self.dupe_indi
+0000fbe0: 6361 746f 722e 7368 6f77 2829 0a20 2020  cator.show().   
+0000fbf0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000fc00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fc10: 656c 662e 6475 7065 5f69 6e64 6963 6174  elf.dupe_indicat
+0000fc20: 6f72 2e68 6964 6528 290a 2020 2020 2020  or.hide().      
+0000fc30: 2020 2020 2020 5f74 6865 7468 7265 6164        _thethread
+0000fc40: 203d 2074 6872 6561 6469 6e67 2e54 6872   = threading.Thr
+0000fc50: 6561 6428 0a20 2020 2020 2020 2020 2020  ead(.           
+0000fc60: 2020 2020 2074 6172 6765 743d 7365 6c66       target=self
+0000fc70: 2e63 6865 636b 5f63 616c 6c73 6967 6e32  .check_callsign2
+0000fc80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000fc90: 2020 6172 6773 3d28 7465 7874 2c29 2c0a    args=(text,),.
+0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcb0: 6461 656d 6f6e 3d54 7275 652c 0a20 2020  daemon=True,.   
+0000fcc0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000fcd0: 2020 2020 2020 205f 7468 6574 6872 6561         _thethrea
+0000fce0: 642e 7374 6172 7428 290a 2020 2020 2020  d.start().      
+0000fcf0: 2020 2020 2020 7365 6c66 2e6e 6578 745f        self.next_
+0000fd00: 6669 656c 642e 7365 7446 6f63 7573 2829  field.setFocus()
+0000fd10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000fd20: 7572 6e0a 2020 2020 2020 2020 636d 6420  urn.        cmd 
+0000fd30: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
+0000fd40: 5b22 636d 6422 5d20 3d20 2243 414c 4c43  ["cmd"] = "CALLC
+0000fd50: 4841 4e47 4544 220a 2020 2020 2020 2020  HANGED".        
+0000fd60: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+0000fd70: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+0000fd80: 0a20 2020 2020 2020 2063 6d64 5b22 6361  .        cmd["ca
+0000fd90: 6c6c 225d 203d 2073 7472 6970 7065 645f  ll"] = stripped_
+0000fda0: 7465 7874 0a20 2020 2020 2020 2073 656c  text.        sel
+0000fdb0: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+0000fdc0: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
+0000fdd0: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
+0000fde0: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
+0000fdf0: 6967 6e28 7374 7269 7070 6564 5f74 6578  ign(stripped_tex
+0000fe00: 7429 0a0a 2020 2020 6465 6620 6368 6563  t)..    def chec
+0000fe10: 6b5f 6361 6c6c 7369 676e 2873 656c 662c  k_callsign(self,
+0000fe20: 2063 616c 6c73 6967 6e29 3a0a 2020 2020   callsign):.    
+0000fe30: 2020 2020 2222 2243 6865 636b 2063 616c      """Check cal
+0000fe40: 6c20 6173 2065 6e74 6572 6564 2222 220a  l as entered""".
+0000fe50: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0000fe60: 2063 7479 5f6c 6f6f 6b75 7028 6361 6c6c   cty_lookup(call
+0000fe70: 7369 676e 290a 2020 2020 2020 2020 6465  sign).        de
+0000fe80: 6275 675f 7265 7375 6c74 203d 2066 227b  bug_result = f"{
+0000fe90: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
+0000fea0: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
+0000feb0: 7322 2c20 6465 6275 675f 7265 7375 6c74  s", debug_result
+0000fec0: 290a 2020 2020 2020 2020 6966 2072 6573  ).        if res
+0000fed0: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
+0000fee0: 2066 6f72 2061 2069 6e20 7265 7375 6c74   for a in result
+0000fef0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+0000ff00: 2020 2020 2020 2020 2020 656e 7469 7479            entity
+0000ff10: 203d 2061 5b31 5d2e 6765 7428 2265 6e74   = a[1].get("ent
+0000ff20: 6974 7922 2c20 2222 290a 2020 2020 2020  ity", "").      
+0000ff30: 2020 2020 2020 2020 2020 6371 203d 2061            cq = a
+0000ff40: 5b31 5d2e 6765 7428 2263 7122 2c20 2222  [1].get("cq", ""
+0000ff50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ff60: 2020 6974 7520 3d20 615b 315d 2e67 6574    itu = a[1].get
+0000ff70: 2822 6974 7522 2c20 2222 290a 2020 2020  ("itu", "").    
+0000ff80: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000ff90: 696e 656e 7420 3d20 615b 315d 2e67 6574  inent = a[1].get
+0000ffa0: 2822 636f 6e74 696e 656e 7422 290a 2020  ("continent").  
+0000ffb0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
+0000ffc0: 7420 3d20 666c 6f61 7428 615b 315d 2e67  t = float(a[1].g
+0000ffd0: 6574 2822 6c61 7422 2c20 2230 2e30 2229  et("lat", "0.0")
+0000ffe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000fff0: 2020 6c6f 6e20 3d20 666c 6f61 7428 615b    lon = float(a[
+00010000: 315d 2e67 6574 2822 6c6f 6e67 222c 2022  1].get("long", "
+00010010: 302e 3022 2929 0a20 2020 2020 2020 2020  0.0")).         
+00010020: 2020 2020 2020 206c 6f6e 203d 206c 6f6e         lon = lon
+00010030: 202a 202d 3120 2023 2063 7479 2e64 6174   * -1  # cty.dat
+00010040: 2066 696c 6520 696e 7665 7274 7320 6c6f   file inverts lo
+00010050: 6e67 6974 7564 6573 0a20 2020 2020 2020  ngitudes.       
+00010060: 2020 2020 2020 2020 2070 7269 6d61 7279           primary
+00010070: 5f70 6678 203d 2061 5b31 5d2e 6765 7428  _pfx = a[1].get(
+00010080: 2270 7269 6d61 7279 5f70 6678 222c 2022  "primary_pfx", "
+00010090: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+000100a0: 2020 2068 6561 6469 6e67 203d 2062 6561     heading = bea
+000100b0: 7269 6e67 5f77 6974 685f 6c61 746c 6f6e  ring_with_latlon
+000100c0: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
+000100d0: 7428 2247 7269 6453 7175 6172 6522 292c  t("GridSquare"),
+000100e0: 206c 6174 2c20 6c6f 6e29 0a20 2020 2020   lat, lon).     
+000100f0: 2020 2020 2020 2020 2020 206b 696c 6f6d             kilom
+00010100: 6574 6572 7320 3d20 6469 7374 616e 6365  eters = distance
+00010110: 5f77 6974 685f 6c61 746c 6f6e 280a 2020  _with_latlon(.  
+00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010130: 2020 7365 6c66 2e73 7461 7469 6f6e 2e67    self.station.g
+00010140: 6574 2822 4772 6964 5371 7561 7265 2229  et("GridSquare")
+00010150: 2c20 6c61 742c 206c 6f6e 0a20 2020 2020  , lat, lon.     
+00010160: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00010180: 662e 6865 6164 696e 675f 6469 7374 616e  f.heading_distan
+00010190: 6365 2e73 6574 5465 7874 280a 2020 2020  ce.setText(.    
+000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101b0: 6622 5265 6769 6f6e 616c 2048 6467 207b  f"Regional Hdg {
+000101c0: 6865 6164 696e 677d c2b0 204c 5020 7b72  heading}.. LP {r
+000101d0: 6563 6970 726f 636f 6c28 6865 6164 696e  eciprocol(headin
+000101e0: 6729 7dc2 b020 2f20 220a 2020 2020 2020  g)}.. / ".      
+000101f0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00010200: 6469 7374 616e 6365 207b 696e 7428 6b69  distance {int(ki
+00010210: 6c6f 6d65 7465 7273 2a30 2e36 3231 3337  lometers*0.62137
+00010220: 3129 7d6d 6920 7b6b 696c 6f6d 6574 6572  1)}mi {kilometer
+00010230: 737d 6b6d 220a 2020 2020 2020 2020 2020  s}km".          
+00010240: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010250: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00010260: 7461 6374 5b22 436f 756e 7472 7950 7265  tact["CountryPre
+00010270: 6669 7822 5d20 3d20 7072 696d 6172 795f  fix"] = primary_
+00010280: 7066 780a 2020 2020 2020 2020 2020 2020  pfx.            
+00010290: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+000102a0: 5b22 5a4e 225d 203d 2069 6e74 2863 7129  ["ZN"] = int(cq)
+000102b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000102c0: 2073 656c 662e 636f 6e74 6163 745b 2243   self.contact["C
+000102d0: 6f6e 7469 6e65 6e74 225d 203d 2063 6f6e  ontinent"] = con
+000102e0: 7469 6e65 6e74 0a20 2020 2020 2020 2020  tinent.         
+000102f0: 2020 2020 2020 2073 656c 662e 6478 5f65         self.dx_e
+00010300: 6e74 6974 792e 7365 7454 6578 7428 0a20  ntity.setText(. 
+00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010320: 2020 2066 227b 7072 696d 6172 795f 7066     f"{primary_pf
+00010330: 787d 3a20 7b63 6f6e 7469 6e65 6e74 7d2f  x}: {continent}/
+00010340: 7b65 6e74 6974 797d 2063 713a 7b63 717d  {entity} cq:{cq}
+00010350: 2069 7475 3a7b 6974 757d 220a 2020 2020   itu:{itu}".    
+00010360: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010370: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00010380: 206c 656e 2863 616c 6c73 6967 6e29 203e   len(callsign) >
+00010390: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+000103a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000103b0: 636f 6e74 6573 743a 0a20 2020 2020 2020  contest:.       
+000103c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000103d0: 2073 656c 662e 636f 6e74 6573 742e 7072   self.contest.pr
+000103e0: 6566 696c 6c28 7365 6c66 290a 0a20 2020  efill(self)..   
+000103f0: 2064 6566 2063 6865 636b 5f63 616c 6c73   def check_calls
+00010400: 6967 6e32 2873 656c 662c 2063 616c 6c73  ign2(self, calls
+00010410: 6967 6e29 3a0a 2020 2020 2020 2020 2222  ign):.        ""
+00010420: 2243 6865 636b 2063 616c 6c20 6f6e 6365  "Check call once
+00010430: 2065 6e74 6572 6564 2222 220a 2020 2020   entered""".    
+00010440: 2020 2020 6361 6c6c 7369 676e 203d 2063      callsign = c
+00010450: 616c 6c73 6967 6e2e 7374 7269 7028 290a  allsign.strip().
+00010460: 2020 2020 2020 2020 6465 6275 675f 6c6f          debug_lo
+00010470: 6f6b 7570 203d 2066 227b 7365 6c66 2e6c  okup = f"{self.l
+00010480: 6f6f 6b5f 7570 7d22 0a20 2020 2020 2020  ook_up}".       
+00010490: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
+000104a0: 732c 2025 7322 2c20 6361 6c6c 7369 676e  s, %s", callsign
+000104b0: 2c20 6465 6275 675f 6c6f 6f6b 7570 290a  , debug_lookup).
+000104c0: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+000104d0: 7472 2873 656c 662e 6c6f 6f6b 5f75 702c  tr(self.look_up,
+000104e0: 2022 7365 7373 696f 6e22 293a 0a20 2020   "session"):.   
+000104f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00010500: 2e6c 6f6f 6b5f 7570 2e73 6573 7369 6f6e  .look_up.session
+00010510: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010520: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+00010530: 662e 6c6f 6f6b 5f75 702e 6c6f 6f6b 7570  f.look_up.lookup
+00010540: 2863 616c 6c73 6967 6e29 0a20 2020 2020  (callsign).     
+00010550: 2020 2020 2020 2020 2020 2064 6562 7567             debug
+00010560: 5f72 6573 706f 6e73 6520 3d20 6622 7b72  _response = f"{r
+00010570: 6573 706f 6e73 657d 220a 2020 2020 2020  esponse}".      
+00010580: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00010590: 2e64 6562 7567 2822 5468 6520 5265 7370  .debug("The Resp
+000105a0: 6f6e 7365 3a20 2573 5c6e 222c 2064 6562  onse: %s\n", deb
+000105b0: 7567 5f72 6573 706f 6e73 6529 0a20 2020  ug_response).   
+000105c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000105d0: 7265 7370 6f6e 7365 3a0a 2020 2020 2020  response:.      
+000105e0: 2020 2020 2020 2020 2020 2020 2020 7468                th
+000105f0: 6569 7267 7269 6420 3d20 7265 7370 6f6e  eirgrid = respon
+00010600: 7365 2e67 6574 2822 6772 6964 2229 0a20  se.get("grid"). 
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 2020 2073 656c 662e 636f 6e74 6163 745b     self.contact[
+00010630: 2247 7269 6453 7175 6172 6522 5d20 3d20  "GridSquare"] = 
+00010640: 7468 6569 7267 7269 640a 2020 2020 2020  theirgrid.      
+00010650: 2020 2020 2020 2020 2020 2020 2020 5f74                _t
+00010660: 6865 6972 636f 756e 7472 7920 3d20 7265  heircountry = re
+00010670: 7370 6f6e 7365 2e67 6574 2822 636f 756e  sponse.get("coun
+00010680: 7472 7922 290a 2020 2020 2020 2020 2020  try").          
+00010690: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000106a0: 662e 7374 6174 696f 6e2e 6765 7428 2247  f.station.get("G
+000106b0: 7269 6453 7175 6172 6522 2c20 2222 293a  ridSquare", ""):
+000106c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000106d0: 2020 2020 2020 2020 2068 6561 6469 6e67           heading
+000106e0: 203d 2062 6561 7269 6e67 2873 656c 662e   = bearing(self.
+000106f0: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
+00010700: 6453 7175 6172 6522 2c20 2222 292c 2074  dSquare", ""), t
+00010710: 6865 6972 6772 6964 290a 2020 2020 2020  heirgrid).      
+00010720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010730: 2020 6b69 6c6f 6d65 7465 7273 203d 2064    kilometers = d
+00010740: 6973 7461 6e63 6528 7365 6c66 2e73 7461  istance(self.sta
+00010750: 7469 6f6e 2e67 6574 2822 4772 6964 5371  tion.get("GridSq
+00010760: 7561 7265 2229 2c20 7468 6569 7267 7269  uare"), theirgri
+00010770: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00010780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010790: 6865 6164 696e 675f 6469 7374 616e 6365  heading_distance
+000107a0: 2e73 6574 5465 7874 280a 2020 2020 2020  .setText(.      
+000107b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107c0: 2020 2020 2020 6622 7b74 6865 6972 6772        f"{theirgr
+000107d0: 6964 7d20 4864 6720 7b68 6561 6469 6e67  id} Hdg {heading
+000107e0: 7dc2 b020 4c50 207b 7265 6369 7072 6f63  }.. LP {reciproc
+000107f0: 6f6c 2868 6561 6469 6e67 297d c2b0 202f  ol(heading)}.. /
+00010800: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00010810: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010820: 2264 6973 7461 6e63 6520 7b69 6e74 286b  "distance {int(k
+00010830: 696c 6f6d 6574 6572 732a 302e 3632 3133  ilometers*0.6213
+00010840: 3731 297d 6d69 207b 6b69 6c6f 6d65 7465  71)}mi {kilomete
+00010850: 7273 7d6b 6d22 0a20 2020 2020 2020 2020  rs}km".         
+00010860: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010880: 2020 2020 2023 2073 656c 662e 6478 5f65       # self.dx_e
+00010890: 6e74 6974 792e 7365 7454 6578 7428 6622  ntity.setText(f"
+000108a0: 7b74 6865 6972 636f 756e 7472 797d 2229  {theircountry}")
+000108b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000108c0: 2023 2065 6c73 653a 0a20 2020 2020 2020   # else:.       
+000108d0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+000108e0: 6865 6164 696e 675f 6469 7374 616e 6365  heading_distance
+000108f0: 2e73 6574 5465 7874 2822 4c6f 6f6b 7570  .setText("Lookup
+00010900: 2066 6169 6c65 642e 2229 0a0a 2020 2020   failed.")..    
+00010910: 6465 6620 6368 6563 6b5f 6475 7065 2873  def check_dupe(s
+00010920: 656c 662c 2063 616c 6c3a 2073 7472 2920  elf, call: str) 
+00010930: 2d3e 2062 6f6f 6c3a 0a20 2020 2020 2020  -> bool:.       
+00010940: 2022 2222 4368 6563 6b73 2069 6620 6120   """Checks if a 
+00010950: 6361 6c6c 7369 676e 2069 7320 6120 6475  callsign is a du
+00010960: 7065 206f 6e20 6375 7272 656e 7420 6261  pe on current ba
+00010970: 6e64 2f6d 6f64 652e 2222 220a 2020 2020  nd/mode.""".    
+00010980: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+00010990: 2e70 7265 6475 7065 2873 656c 6629 0a20  .predupe(self). 
+000109a0: 2020 2020 2020 2062 616e 6420 3d20 666c         band = fl
+000109b0: 6f61 7428 6765 745f 6c6f 6767 6564 5f62  oat(get_logged_b
+000109c0: 616e 6428 7374 7228 7365 6c66 2e72 6164  and(str(self.rad
+000109d0: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
+000109e0: 6f61 222c 2030 2e30 2929 2929 0a20 2020  oa", 0.0)))).   
+000109f0: 2020 2020 206d 6f64 6520 3d20 7365 6c66       mode = self
+00010a00: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+00010a10: 2822 6d6f 6465 222c 2022 2229 0a20 2020  ("mode", "").   
+00010a20: 2020 2020 2064 6562 7567 6c69 6e65 203d       debugline =
+00010a30: 2028 0a20 2020 2020 2020 2020 2020 2066   (.            f
+00010a40: 2243 616c 6c3a 207b 6361 6c6c 7d20 4261  "Call: {call} Ba
+00010a50: 6e64 3a20 7b62 616e 647d 204d 6f64 653a  nd: {band} Mode:
+00010a60: 207b 6d6f 6465 7d20 4475 7065 7479 7065   {mode} Dupetype
+00010a70: 3a20 7b73 656c 662e 636f 6e74 6573 742e  : {self.contest.
+00010a80: 6475 7065 5f74 7970 657d 220a 2020 2020  dupe_type}".    
+00010a90: 2020 2020 290a 2020 2020 2020 2020 6c6f      ).        lo
+00010aa0: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+00010ab0: 2064 6562 7567 6c69 6e65 290a 2020 2020   debugline).    
+00010ac0: 2020 2020 6966 2073 656c 662e 636f 6e74      if self.cont
+00010ad0: 6573 742e 6475 7065 5f74 7970 6520 3d3d  est.dupe_type ==
+00010ae0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00010af0: 7265 7375 6c74 203d 2073 656c 662e 6461  result = self.da
+00010b00: 7461 6261 7365 2e63 6865 636b 5f64 7570  tabase.check_dup
+00010b10: 6528 6361 6c6c 290a 2020 2020 2020 2020  e(call).        
+00010b20: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
+00010b30: 6475 7065 5f74 7970 6520 3d3d 2032 3a0a  dupe_type == 2:.
+00010b40: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00010b50: 6c74 203d 2073 656c 662e 6461 7461 6261  lt = self.databa
+00010b60: 7365 2e63 6865 636b 5f64 7570 655f 6f6e  se.check_dupe_on
+00010b70: 5f62 616e 6428 6361 6c6c 2c20 6261 6e64  _band(call, band
+00010b80: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00010b90: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
+00010ba0: 7970 6520 3d3d 2033 3a0a 2020 2020 2020  ype == 3:.      
+00010bb0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00010bc0: 656c 662e 6461 7461 6261 7365 2e63 6865  elf.database.che
+00010bd0: 636b 5f64 7570 655f 6f6e 5f62 616e 645f  ck_dupe_on_band_
+00010be0: 6d6f 6465 2863 616c 6c2c 2062 616e 642c  mode(call, band,
+00010bf0: 206d 6f64 6529 0a20 2020 2020 2020 2069   mode).        i
+00010c00: 6620 7365 6c66 2e63 6f6e 7465 7374 2e64  f self.contest.d
+00010c10: 7570 655f 7479 7065 203d 3d20 343a 0a20  upe_type == 4:. 
+00010c20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00010c30: 7420 3d20 7b22 6973 6475 7065 223a 2046  t = {"isdupe": F
+00010c40: 616c 7365 7d0a 2020 2020 2020 2020 6465  alse}.        de
+00010c50: 6275 676c 696e 6520 3d20 6622 7b72 6573  bugline = f"{res
+00010c60: 756c 747d 220a 2020 2020 2020 2020 6c6f  ult}".        lo
+00010c70: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+00010c80: 2064 6562 7567 6c69 6e65 290a 2020 2020   debugline).    
+00010c90: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00010ca0: 742e 6765 7428 2269 7364 7570 6522 2c20  t.get("isdupe", 
+00010cb0: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
+00010cc0: 7365 746d 6f64 6528 7365 6c66 2c20 6d6f  setmode(self, mo
+00010cd0: 6465 3a20 7374 7229 202d 3e20 4e6f 6e65  de: str) -> None
+00010ce0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
+00010cf0: 6220 666f 7220 7768 656e 2074 6865 206d  b for when the m
+00010d00: 6f64 6520 6368 616e 6765 732e 2222 220a  ode changes.""".
+00010d10: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00010d20: 3d3d 2022 4357 223a 0a20 2020 2020 2020  == "CW":.       
+00010d30: 2020 2020 2073 656c 662e 6375 7272 656e       self.curren
+00010d40: 745f 6d6f 6465 203d 2022 4357 220a 2020  t_mode = "CW".  
+00010d50: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+00010d60: 2e6d 6f64 652e 7365 7454 6578 7428 2243  .mode.setText("C
+00010d70: 5722 290a 2020 2020 2020 2020 2020 2020  W").            
+00010d80: 7365 6c66 2e73 656e 742e 7365 7454 6578  self.sent.setTex
+00010d90: 7428 2235 3939 2229 0a20 2020 2020 2020  t("599").       
+00010da0: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
+00010db0: 652e 7365 7454 6578 7428 2235 3939 2229  e.setText("599")
+00010dc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010dd0: 662e 7265 6164 5f63 775f 6d61 6372 6f73  f.read_cw_macros
+00010de0: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+00010df0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+00010e00: 206d 6f64 6520 3d3d 2022 5353 4222 3a0a   mode == "SSB":.
+00010e10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010e20: 2e63 7572 7265 6e74 5f6d 6f64 6520 3d20  .current_mode = 
+00010e30: 2253 5342 220a 2020 2020 2020 2020 2020  "SSB".          
+00010e40: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
+00010e50: 7454 6578 7428 2253 5342 2229 0a20 2020  tText("SSB").   
+00010e60: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00010e70: 6e74 2e73 6574 5465 7874 2822 3539 2229  nt.setText("59")
+00010e80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010e90: 662e 7265 6365 6976 652e 7365 7454 6578  f.receive.setTex
+00010ea0: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
+00010eb0: 2020 2020 7365 6c66 2e72 6561 645f 6377      self.read_cw
+00010ec0: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
+00010ed0: 2020 6966 206d 6f64 6520 3d3d 2022 5254    if mode == "RT
+00010ee0: 5459 223a 0a20 2020 2020 2020 2020 2020  TY":.           
+00010ef0: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
+00010f00: 6465 203d 2022 5254 5459 220a 2020 2020  de = "RTTY".    
+00010f10: 2020 2020 2020 2020 2320 7365 6c66 2e6d          # self.m
+00010f20: 6f64 652e 7365 7454 6578 7428 2252 5454  ode.setText("RTT
+00010f30: 5922 290a 2020 2020 2020 2020 2020 2020  Y").            
+00010f40: 7365 6c66 2e73 656e 742e 7365 7454 6578  self.sent.setTex
+00010f50: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
+00010f60: 2020 2020 7365 6c66 2e72 6563 6569 7665      self.receive
+00010f70: 2e73 6574 5465 7874 2822 3539 2229 0a0a  .setText("59")..
+00010f80: 2020 2020 6465 6620 6765 745f 6f70 6f6e      def get_opon
+00010f90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00010fa0: 2222 2243 7472 6c2b 4f20 6f72 204f 504f  """Ctrl+O or OPO
+00010fb0: 4e20 6469 616c 6f67 2222 220a 2020 2020  N dialog""".    
+00010fc0: 2020 2020 7365 6c66 2e6f 706f 6e5f 6469      self.opon_di
+00010fd0: 616c 6f67 203d 204f 704f 6e28 574f 524b  alog = OpOn(WORK
+00010fe0: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
+00010ff0: 2020 7365 6c66 2e6f 706f 6e5f 6469 616c    self.opon_dial
+00011000: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
+00011010: 6563 7428 7365 6c66 2e6e 6577 5f6f 7029  ect(self.new_op)
+00011020: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
+00011030: 6f6e 5f64 6961 6c6f 672e 6f70 656e 2829  on_dialog.open()
+00011040: 0a0a 2020 2020 6465 6620 6e65 775f 6f70  ..    def new_op
+00011050: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00011060: 2222 2253 6176 6520 6e65 7720 4f50 2222  """Save new OP""
+00011070: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00011080: 662e 6f70 6f6e 5f64 6961 6c6f 672e 4e65  f.opon_dialog.Ne
+00011090: 774f 7065 7261 746f 722e 7465 7874 2829  wOperator.text()
+000110a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000110b0: 6c66 2e63 7572 7265 6e74 5f6f 7020 3d20  lf.current_op = 
+000110c0: 7365 6c66 2e6f 706f 6e5f 6469 616c 6f67  self.opon_dialog
+000110d0: 2e4e 6577 4f70 6572 6174 6f72 2e74 6578  .NewOperator.tex
+000110e0: 7428 292e 7570 7065 7228 290a 2020 2020  t().upper().    
+000110f0: 2020 2020 7365 6c66 2e6f 706f 6e5f 6469      self.opon_di
+00011100: 616c 6f67 2e63 6c6f 7365 2829 0a20 2020  alog.close().   
+00011110: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00011120: 6728 224e 6577 204f 703a 2025 7322 2c20  g("New Op: %s", 
+00011130: 7365 6c66 2e63 7572 7265 6e74 5f6f 7029  self.current_op)
+00011140: 0a20 2020 2020 2020 2073 656c 662e 6d61  .        self.ma
+00011150: 6b65 5f6f 705f 6469 7228 290a 0a20 2020  ke_op_dir()..   
+00011160: 2064 6566 206d 616b 655f 6f70 5f64 6972   def make_op_dir
+00011170: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00011180: 2222 2243 7265 6174 6520 4f50 2064 6972  """Create OP dir
+00011190: 6563 746f 7279 2069 6620 6974 2064 6f65  ectory if it doe
+000111a0: 7320 6e6f 7420 6578 6973 742e 2222 220a  s not exist.""".
+000111b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000111c0: 6375 7272 656e 745f 6f70 3a0a 2020 2020  current_op:.    
+000111d0: 2020 2020 2020 2020 6f70 5f70 6174 6820          op_path 
+000111e0: 3d20 5061 7468 2844 4154 415f 5041 5448  = Path(DATA_PATH
+000111f0: 2920 2f20 7365 6c66 2e63 7572 7265 6e74  ) / self.current
+00011200: 5f6f 700a 2020 2020 2020 2020 2020 2020  _op.            
+00011210: 6c6f 6767 6572 2e64 6562 7567 2822 6f70  logger.debug("op
+00011220: 5f70 6174 683a 2025 7322 2c20 7374 7228  _path: %s", str(
+00011230: 6f70 5f70 6174 6829 290a 2020 2020 2020  op_path)).      
+00011240: 2020 2020 2020 6966 206f 705f 7061 7468        if op_path
+00011250: 2e69 735f 6469 7228 2920 6973 2046 616c  .is_dir() is Fal
+00011260: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00011270: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00011280: 2822 4372 6561 7469 6e67 204f 7020 4469  ("Creating Op Di
+00011290: 7265 6374 6f72 793a 2025 7322 2c20 7374  rectory: %s", st
+000112a0: 7228 6f70 5f70 6174 6829 290a 2020 2020  r(op_path)).    
+000112b0: 2020 2020 2020 2020 2020 2020 6f73 2e6d              os.m
+000112c0: 6b64 6972 2873 7472 286f 705f 7061 7468  kdir(str(op_path
+000112d0: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+000112e0: 6620 6f70 5f70 6174 682e 6973 5f64 6972  f op_path.is_dir
+000112f0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00011300: 2020 2020 736f 7572 6365 5f70 6174 6820      source_path 
+00011310: 3d20 5061 7468 2857 4f52 4b49 4e47 5f50  = Path(WORKING_P
+00011320: 4154 4829 202f 2022 6461 7461 2220 2f20  ATH) / "data" / 
+00011330: 2270 686f 6e65 7469 6373 220a 2020 2020  "phonetics".    
+00011340: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00011350: 6572 2e64 6562 7567 2822 736f 7572 6365  er.debug("source
+00011360: 5f70 6174 683a 2025 7322 2c20 7374 7228  _path: %s", str(
+00011370: 736f 7572 6365 5f70 6174 6829 290a 2020  source_path)).  
+00011380: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011390: 7220 6368 696c 6420 696e 2073 6f75 7263  r child in sourc
+000113a0: 655f 7061 7468 2e69 7465 7264 6972 2829  e_path.iterdir()
+000113b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000113c0: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
+000113d0: 6e5f 6669 6c65 203d 206f 705f 7061 7468  n_file = op_path
+000113e0: 202f 2063 6869 6c64 2e6e 616d 650a 2020   / child.name.  
+000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011400: 2020 6966 2064 6573 7469 6e61 7469 6f6e    if destination
+00011410: 5f66 696c 652e 6973 5f66 696c 6528 2920  _file.is_file() 
+00011420: 6973 2046 616c 7365 3a0a 2020 2020 2020  is False:.      
+00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011440: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00011450: 4465 7374 696e 6174 696f 6e3a 2025 7322  Destination: %s"
+00011460: 2c20 7374 7228 6465 7374 696e 6174 696f  , str(destinatio
+00011470: 6e5f 6669 6c65 2929 0a20 2020 2020 2020  n_file)).       
+00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011490: 2064 6573 7469 6e61 7469 6f6e 5f66 696c   destination_fil
+000114a0: 652e 7772 6974 655f 6279 7465 7328 6368  e.write_bytes(ch
+000114b0: 696c 642e 7265 6164 5f62 7974 6573 2829  ild.read_bytes()
+000114c0: 290a 0a20 2020 2064 6566 2070 6f6c 6c5f  )..    def poll_
+000114d0: 7261 6469 6f28 7365 6c66 293a 0a20 2020  radio(self):.   
+000114e0: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+000114f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011500: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
+00011510: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00011520: 2e72 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c  .rig_control.onl
+00011530: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
+00011540: 2020 2020 2076 666f 203d 2073 656c 662e       vfo = self.
+00011550: 7269 675f 636f 6e74 726f 6c2e 6765 745f  rig_control.get_
+00011560: 7666 6f28 290a 2020 2020 2020 2020 2020  vfo().          
+00011570: 2020 2020 2020 6d6f 6465 203d 2073 656c        mode = sel
+00011580: 662e 7269 675f 636f 6e74 726f 6c2e 6765  f.rig_control.ge
+00011590: 745f 6d6f 6465 2829 0a20 2020 2020 2020  t_mode().       
+000115a0: 2020 2020 2020 2020 2062 7720 3d20 7365           bw = se
+000115b0: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
+000115c0: 6574 5f62 7728 290a 2020 2020 2020 2020  et_bw().        
+000115d0: 2020 2020 2020 2020 2320 7365 6c66 2e72          # self.r
+000115e0: 6164 696f 5f73 7461 7465 5b22 7074 7422  adio_state["ptt"
+000115f0: 5d20 3d20 7365 6c66 2e72 6967 5f63 6f6e  ] = self.rig_con
+00011600: 7472 6f6c 2e67 6574 5f70 7474 2829 0a20  trol.get_ptt(). 
+00011610: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00011620: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+00011630: 7461 7465 2e67 6574 2822 7074 7422 2c20  tate.get("ptt", 
+00011640: 3029 203d 3d20 313a 0a20 2020 2020 2020  0) == 1:.       
+00011650: 2020 2020 2020 2020 2023 2020 2020 2073           #     s
+00011660: 656c 662e 6c65 6674 646f 742e 7365 7450  elf.leftdot.setP
+00011670: 6978 6d61 7028 7365 6c66 2e67 7265 656e  ixmap(self.green
+00011680: 646f 7429 0a20 2020 2020 2020 2020 2020  dot).           
+00011690: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+000116a0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
+000116b0: 2020 2073 656c 662e 6c65 6674 646f 742e     self.leftdot.
+000116c0: 7365 7450 6978 6d61 7028 7365 6c66 2e72  setPixmap(self.r
+000116d0: 6564 646f 7429 0a20 2020 2020 2020 2020  eddot).         
+000116e0: 2020 2020 2020 2069 6620 6d6f 6465 203d         if mode =
+000116f0: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
+00011700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011710: 2e73 6574 6d6f 6465 286d 6f64 6529 0a20  .setmode(mode). 
+00011720: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011730: 6620 6d6f 6465 203d 3d20 224c 5342 2220  f mode == "LSB" 
+00011740: 6f72 206d 6f64 6520 3d3d 2022 5553 4222  or mode == "USB"
+00011750: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011760: 2020 2020 2020 7365 6c66 2e73 6574 6d6f        self.setmo
+00011770: 6465 2822 5353 4222 290a 2020 2020 2020  de("SSB").      
+00011780: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+00011790: 6520 3d3d 2022 5254 5459 223a 0a20 2020  e == "RTTY":.   
+000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117b0: 2073 656c 662e 7365 746d 6f64 6528 2252   self.setmode("R
+000117c0: 5454 5922 290a 2020 2020 2020 2020 2020  TTY").          
+000117d0: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
+000117e0: 5f73 7461 7465 5b22 7666 6f61 225d 203d  _state["vfoa"] =
+000117f0: 2076 666f 0a20 2020 2020 2020 2020 2020   vfo.           
+00011800: 2020 2020 2062 616e 6420 3d20 6765 7462       band = getb
+00011810: 616e 6428 7374 7228 7666 6f29 290a 2020  and(str(vfo)).  
+00011820: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011830: 6c66 2e72 6164 696f 5f73 7461 7465 5b22  lf.radio_state["
+00011840: 6261 6e64 225d 203d 2062 616e 640a 2020  band"] = band.  
+00011850: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00011860: 6c66 2e63 6f6e 7461 6374 5b22 4261 6e64  lf.contact["Band
+00011870: 225d 203d 2067 6574 5f6c 6f67 6765 645f  "] = get_logged_
+00011880: 6261 6e64 2873 7472 2876 666f 2929 0a20  band(str(vfo)). 
+00011890: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000118a0: 656c 662e 7365 745f 6261 6e64 5f69 6e64  elf.set_band_ind
+000118b0: 6963 6174 6f72 2862 616e 6429 0a20 2020  icator(band).   
+000118c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000118d0: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
+000118e0: 6f64 6522 5d20 3d20 6d6f 6465 0a20 2020  ode"] = mode.   
+000118f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00011900: 662e 7261 6469 6f5f 7374 6174 655b 2262  f.radio_state["b
+00011910: 7722 5d20 3d20 6277 0a20 2020 2020 2020  w"] = bw.       
+00011920: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00011930: 6465 6275 6728 2256 464f 3a20 2573 2020  debug("VFO: %s  
+00011940: 4d4f 4445 3a20 2573 2042 573a 2025 7322  MODE: %s BW: %s"
+00011950: 2c20 7666 6f2c 206d 6f64 652c 2062 7729  , vfo, mode, bw)
+00011960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011970: 2073 656c 662e 7365 745f 7769 6e64 6f77   self.set_window
+00011980: 5f74 6974 6c65 2829 0a20 2020 2020 2020  _title().       
+00011990: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+000119a0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000119b0: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+000119c0: 5241 4449 4f5f 5354 4154 4522 0a20 2020  RADIO_STATE".   
+000119d0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+000119e0: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
+000119f0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
+00011a00: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00011a10: 645b 2262 616e 6422 5d20 3d20 6261 6e64  d["band"] = band
+00011a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011a30: 2063 6d64 5b22 7666 6f61 225d 203d 2076   cmd["vfoa"] = v
+00011a40: 666f 0a20 2020 2020 2020 2020 2020 2020  fo.             
+00011a50: 2020 2063 6d64 5b22 6d6f 6465 225d 203d     cmd["mode"] =
+00011a60: 206d 6f64 650a 2020 2020 2020 2020 2020   mode.          
+00011a70: 2020 2020 2020 636d 645b 2262 7722 5d20        cmd["bw"] 
+00011a80: 3d20 6277 0a20 2020 2020 2020 2020 2020  = bw.           
+00011a90: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+00011aa0: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+00011ab0: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+00011ac0: 0a20 2020 2064 6566 2065 6469 745f 6377  .    def edit_cw
+00011ad0: 5f6d 6163 726f 7328 7365 6c66 2920 2d3e  _macros(self) ->
+00011ae0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00011af0: 2222 0a20 2020 2020 2020 2043 616c 6c73  "".        Calls
+00011b00: 2074 6865 2064 6566 6175 6c74 2074 6578   the default tex
+00011b10: 7420 6564 6974 6f72 2074 6f20 6564 6974  t editor to edit
+00011b20: 2074 6865 2043 5720 6d61 6372 6f20 6669   the CW macro fi
+00011b30: 6c65 2e0a 2020 2020 2020 2020 2222 220a  le..        """.
+00011b40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011b50: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+00011b60: 226d 6f64 6522 2920 3d3d 2022 4357 223a  "mode") == "CW":
+00011b70: 0a20 2020 2020 2020 2020 2020 206d 6163  .            mac
+00011b80: 726f 5f66 696c 6520 3d20 222f 6377 6d61  ro_file = "/cwma
+00011b90: 6372 6f73 2e74 7874 220a 2020 2020 2020  cros.txt".      
+00011ba0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00011bb0: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
+00011bc0: 2022 2f73 7362 6d61 6372 6f73 2e74 7874   "/ssbmacros.txt
+00011bd0: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+00011be0: 2050 6174 6828 4441 5441 5f50 4154 4820   Path(DATA_PATH 
+00011bf0: 2b20 6d61 6372 6f5f 6669 6c65 292e 6578  + macro_file).ex
+00011c00: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
+00011c10: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00011c20: 2822 7265 6164 5f63 775f 6d61 6372 6f73  ("read_cw_macros
+00011c30: 3a20 636f 7079 696e 6720 6465 6661 756c  : copying defaul
+00011c40: 7420 6d61 6372 6f20 6669 6c65 2e22 290a  t macro file.").
+00011c50: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+00011c60: 6669 6c65 2857 4f52 4b49 4e47 5f50 4154  file(WORKING_PAT
+00011c70: 4820 2b20 222f 6461 7461 2220 2b20 6d61  H + "/data" + ma
+00011c80: 6372 6f5f 6669 6c65 2c20 4441 5441 5f50  cro_file, DATA_P
+00011c90: 4154 4820 2b20 6d61 6372 6f5f 6669 6c65  ATH + macro_file
+00011ca0: 290a 2020 2020 2020 2020 6f73 2e73 7973  ).        os.sys
+00011cb0: 7465 6d28 6622 7864 672d 6f70 656e 207b  tem(f"xdg-open {
+00011cc0: 4441 5441 5f50 4154 487d 7b6d 6163 726f  DATA_PATH}{macro
+00011cd0: 5f66 696c 657d 2229 0a0a 2020 2020 6465  _file}")..    de
+00011ce0: 6620 7265 6164 5f63 775f 6d61 6372 6f73  f read_cw_macros
+00011cf0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00011d00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011d10: 2020 2020 5265 6164 7320 696e 2074 6865      Reads in the
+00011d20: 2043 5720 6d61 6372 6f73 2c20 6669 7273   CW macros, firs
+00011d30: 7473 2069 7420 6368 6563 6b73 2074 6f20  ts it checks to 
+00011d40: 7365 6520 6966 2074 6865 2066 696c 6520  see if the file 
+00011d50: 6578 6973 7473 2e20 4966 2069 7420 646f  exists. If it do
+00011d60: 6573 206e 6f74 2c0a 2020 2020 2020 2020  es not,.        
+00011d70: 616e 6420 7468 6973 2068 6173 2062 6565  and this has bee
+00011d80: 6e20 7061 636b 6167 6564 2077 6974 6820  n packaged with 
+00011d90: 7079 696e 7374 616c 6c65 7220 6974 2077  pyinstaller it w
+00011da0: 696c 6c20 636f 7079 2074 6865 2064 6566  ill copy the def
+00011db0: 6175 6c74 2066 696c 6520 6672 6f6d 2074  ault file from t
+00011dc0: 6865 0a20 2020 2020 2020 2074 656d 7020  he.        temp 
+00011dd0: 6469 7265 6374 6f72 7920 7468 6973 2069  directory this i
+00011de0: 7320 7275 6e6e 696e 6720 6672 6f6d 2e2e  s running from..
+00011df0: 2e20 496e 2074 6865 6f72 792e 0a20 2020  . In theory..   
+00011e00: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00011e10: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+00011e20: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+00011e30: 2920 3d3d 2022 4357 223a 0a20 2020 2020  ) == "CW":.     
+00011e40: 2020 2020 2020 206d 6163 726f 5f66 696c         macro_fil
+00011e50: 6520 3d20 222f 6377 6d61 6372 6f73 2e74  e = "/cwmacros.t
+00011e60: 7874 220a 2020 2020 2020 2020 656c 7365  xt".        else
+00011e70: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
+00011e80: 6372 6f5f 6669 6c65 203d 2022 2f73 7362  cro_file = "/ssb
+00011e90: 6d61 6372 6f73 2e74 7874 220a 0a20 2020  macros.txt"..   
+00011ea0: 2020 2020 2069 6620 6e6f 7420 5061 7468       if not Path
+00011eb0: 2844 4154 415f 5041 5448 202b 206d 6163  (DATA_PATH + mac
+00011ec0: 726f 5f66 696c 6529 2e65 7869 7374 7328  ro_file).exists(
+00011ed0: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+00011ee0: 6f67 6765 722e 6465 6275 6728 2272 6561  ogger.debug("rea
+00011ef0: 645f 6377 5f6d 6163 726f 733a 2063 6f70  d_cw_macros: cop
+00011f00: 7969 6e67 2064 6566 6175 6c74 206d 6163  ying default mac
+00011f10: 726f 2066 696c 652e 2229 0a20 2020 2020  ro file.").     
+00011f20: 2020 2020 2020 2063 6f70 7966 696c 6528         copyfile(
+00011f30: 574f 524b 494e 475f 5041 5448 202b 2022  WORKING_PATH + "
+00011f40: 2f64 6174 6122 202b 206d 6163 726f 5f66  /data" + macro_f
+00011f50: 696c 652c 2044 4154 415f 5041 5448 202b  ile, DATA_PATH +
+00011f60: 206d 6163 726f 5f66 696c 6529 0a20 2020   macro_file).   
+00011f70: 2020 2020 2077 6974 6820 6f70 656e 2844       with open(D
+00011f80: 4154 415f 5041 5448 202b 206d 6163 726f  ATA_PATH + macro
+00011f90: 5f66 696c 652c 2022 7222 2c20 656e 636f  _file, "r", enco
+00011fa0: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
+00011fb0: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
+00011fc0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00011fd0: 7220 6c69 6e65 2069 6e20 6669 6c65 5f64  r line in file_d
+00011fe0: 6573 6372 6970 746f 723a 0a20 2020 2020  escriptor:.     
+00011ff0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00012000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012010: 2020 2020 6d6f 6465 2c20 666b 6579 2c20      mode, fkey, 
+00012020: 6275 7474 6f6e 6e61 6d65 2c20 6377 7465  buttonname, cwte
+00012030: 7874 203d 206c 696e 652e 7370 6c69 7428  xt = line.split(
+00012040: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
+00012050: 2020 2020 2020 2020 2069 6620 6d6f 6465           if mode
+00012060: 2e73 7472 6970 2829 2e75 7070 6572 2829  .strip().upper()
+00012070: 203d 3d20 2252 2220 616e 6420 7365 6c66   == "R" and self
+00012080: 2e70 7265 662e 6765 7428 2272 756e 5f73  .pref.get("run_s
+00012090: 7461 7465 2229 3a0a 2020 2020 2020 2020  tate"):.        
+000120a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120b0: 7365 6c66 2e66 6b65 7973 5b66 6b65 792e  self.fkeys[fkey.
+000120c0: 7374 7269 7028 295d 203d 2028 6275 7474  strip()] = (butt
+000120d0: 6f6e 6e61 6d65 2e73 7472 6970 2829 2c20  onname.strip(), 
+000120e0: 6377 7465 7874 2e73 7472 6970 2829 290a  cwtext.strip()).
+000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012100: 2020 2020 6966 206d 6f64 652e 7374 7269      if mode.stri
+00012110: 7028 292e 7570 7065 7228 2920 213d 2022  p().upper() != "
+00012120: 5222 2061 6e64 206e 6f74 2073 656c 662e  R" and not self.
+00012130: 7072 6566 2e67 6574 2822 7275 6e5f 7374  pref.get("run_st
+00012140: 6174 6522 293a 0a20 2020 2020 2020 2020  ate"):.         
+00012150: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012160: 656c 662e 666b 6579 735b 666b 6579 2e73  elf.fkeys[fkey.s
+00012170: 7472 6970 2829 5d20 3d20 2862 7574 746f  trip()] = (butto
+00012180: 6e6e 616d 652e 7374 7269 7028 292c 2063  nname.strip(), c
+00012190: 7774 6578 742e 7374 7269 7028 2929 0a20  wtext.strip()). 
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000121b0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+000121c0: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
+000121d0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+000121e0: 6765 722e 696e 666f 2822 7265 6164 5f63  ger.info("read_c
+000121f0: 775f 6d61 6372 6f73 3a20 2573 222c 2065  w_macros: %s", e
+00012200: 7272 290a 2020 2020 2020 2020 6b65 7973  rr).        keys
+00012210: 203d 2073 656c 662e 666b 6579 732e 6b65   = self.fkeys.ke
+00012220: 7973 2829 0a20 2020 2020 2020 2069 6620  ys().        if 
+00012230: 2246 3122 2069 6e20 6b65 7973 3a0a 2020  "F1" in keys:.  
+00012240: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+00012250: 312e 7365 7454 6578 7428 6622 4631 3a20  1.setText(f"F1: 
+00012260: 7b73 656c 662e 666b 6579 735b 2746 3127  {self.fkeys['F1'
+00012270: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
+00012280: 2020 2020 7365 6c66 2e46 312e 7365 7454      self.F1.setT
+00012290: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+000122a0: 735b 2246 3122 5d5b 315d 290a 2020 2020  s["F1"][1]).    
+000122b0: 2020 2020 6966 2022 4632 2220 696e 206b      if "F2" in k
+000122c0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+000122d0: 2073 656c 662e 4632 2e73 6574 5465 7874   self.F2.setText
+000122e0: 2866 2246 323a 207b 7365 6c66 2e66 6b65  (f"F2: {self.fke
+000122f0: 7973 5b27 4632 275d 5b30 5d7d 2229 0a20  ys['F2'][0]}"). 
+00012300: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012310: 4632 2e73 6574 546f 6f6c 5469 7028 7365  F2.setToolTip(se
+00012320: 6c66 2e66 6b65 7973 5b22 4632 225d 5b31  lf.fkeys["F2"][1
+00012330: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
+00012340: 3322 2069 6e20 6b65 7973 3a0a 2020 2020  3" in keys:.    
+00012350: 2020 2020 2020 2020 7365 6c66 2e46 332e          self.F3.
+00012360: 7365 7454 6578 7428 6622 4633 3a20 7b73  setText(f"F3: {s
+00012370: 656c 662e 666b 6579 735b 2746 3327 5d5b  elf.fkeys['F3'][
+00012380: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
+00012390: 2020 7365 6c66 2e46 332e 7365 7454 6f6f    self.F3.setToo
+000123a0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+000123b0: 2246 3322 5d5b 315d 290a 2020 2020 2020  "F3"][1]).      
+000123c0: 2020 6966 2022 4634 2220 696e 206b 6579    if "F4" in key
+000123d0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+000123e0: 656c 662e 4634 2e73 6574 5465 7874 2866  elf.F4.setText(f
+000123f0: 2246 343a 207b 7365 6c66 2e66 6b65 7973  "F4: {self.fkeys
+00012400: 5b27 4634 275d 5b30 5d7d 2229 0a20 2020  ['F4'][0]}").   
+00012410: 2020 2020 2020 2020 2073 656c 662e 4634           self.F4
+00012420: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00012430: 2e66 6b65 7973 5b22 4634 225d 5b31 5d29  .fkeys["F4"][1])
+00012440: 0a20 2020 2020 2020 2069 6620 2246 3522  .        if "F5"
+00012450: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+00012460: 2020 2020 2020 7365 6c66 2e46 352e 7365        self.F5.se
+00012470: 7454 6578 7428 6622 4635 3a20 7b73 656c  tText(f"F5: {sel
+00012480: 662e 666b 6579 735b 2746 3527 5d5b 305d  f.fkeys['F5'][0]
+00012490: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+000124a0: 7365 6c66 2e46 352e 7365 7454 6f6f 6c54  self.F5.setToolT
+000124b0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+000124c0: 3522 5d5b 315d 290a 2020 2020 2020 2020  5"][1]).        
+000124d0: 6966 2022 4636 2220 696e 206b 6579 733a  if "F6" in keys:
+000124e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000124f0: 662e 4636 2e73 6574 5465 7874 2866 2246  f.F6.setText(f"F
+00012500: 363a 207b 7365 6c66 2e66 6b65 7973 5b27  6: {self.fkeys['
+00012510: 4636 275d 5b30 5d7d 2229 0a20 2020 2020  F6'][0]}").     
+00012520: 2020 2020 2020 2073 656c 662e 4636 2e73         self.F6.s
+00012530: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
+00012540: 6b65 7973 5b22 4636 225d 5b31 5d29 0a20  keys["F6"][1]). 
+00012550: 2020 2020 2020 2069 6620 2246 3722 2069         if "F7" i
+00012560: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+00012570: 2020 2020 7365 6c66 2e46 372e 7365 7454      self.F7.setT
+00012580: 6578 7428 6622 4637 3a20 7b73 656c 662e  ext(f"F7: {self.
+00012590: 666b 6579 735b 2746 3727 5d5b 305d 7d22  fkeys['F7'][0]}"
+000125a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000125b0: 6c66 2e46 372e 7365 7454 6f6f 6c54 6970  lf.F7.setToolTip
+000125c0: 2873 656c 662e 666b 6579 735b 2246 3722  (self.fkeys["F7"
+000125d0: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
+000125e0: 2022 4638 2220 696e 206b 6579 733a 0a20   "F8" in keys:. 
+000125f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012600: 4638 2e73 6574 5465 7874 2866 2246 383a  F8.setText(f"F8:
+00012610: 207b 7365 6c66 2e66 6b65 7973 5b27 4638   {self.fkeys['F8
+00012620: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00012630: 2020 2020 2073 656c 662e 4638 2e73 6574       self.F8.set
+00012640: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+00012650: 7973 5b22 4638 225d 5b31 5d29 0a20 2020  ys["F8"][1]).   
+00012660: 2020 2020 2069 6620 2246 3922 2069 6e20       if "F9" in 
+00012670: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
+00012680: 2020 7365 6c66 2e46 392e 7365 7454 6578    self.F9.setTex
+00012690: 7428 6622 4639 3a20 7b73 656c 662e 666b  t(f"F9: {self.fk
+000126a0: 6579 735b 2746 3927 5d5b 305d 7d22 290a  eys['F9'][0]}").
+000126b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000126c0: 2e46 392e 7365 7454 6f6f 6c54 6970 2873  .F9.setToolTip(s
+000126d0: 656c 662e 666b 6579 735b 2246 3922 5d5b  elf.fkeys["F9"][
+000126e0: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
+000126f0: 4631 3022 2069 6e20 6b65 7973 3a0a 2020  F10" in keys:.  
+00012700: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+00012710: 3130 2e73 6574 5465 7874 2866 2246 3130  10.setText(f"F10
+00012720: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
+00012730: 3130 275d 5b30 5d7d 2229 0a20 2020 2020  10'][0]}").     
+00012740: 2020 2020 2020 2073 656c 662e 4631 302e         self.F10.
+00012750: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+00012760: 666b 6579 735b 2246 3130 225d 5b31 5d29  fkeys["F10"][1])
+00012770: 0a20 2020 2020 2020 2069 6620 2246 3131  .        if "F11
+00012780: 2220 696e 206b 6579 733a 0a20 2020 2020  " in keys:.     
+00012790: 2020 2020 2020 2073 656c 662e 4631 312e         self.F11.
+000127a0: 7365 7454 6578 7428 6622 4631 313a 207b  setText(f"F11: {
+000127b0: 7365 6c66 2e66 6b65 7973 5b27 4631 3127  self.fkeys['F11'
+000127c0: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
+000127d0: 2020 2020 7365 6c66 2e46 3131 2e73 6574      self.F11.set
+000127e0: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
+000127f0: 7973 5b22 4631 3122 5d5b 315d 290a 2020  ys["F11"][1]).  
+00012800: 2020 2020 2020 6966 2022 4631 3222 2069        if "F12" i
+00012810: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
+00012820: 2020 2020 7365 6c66 2e46 3132 2e73 6574      self.F12.set
+00012830: 5465 7874 2866 2246 3132 3a20 7b73 656c  Text(f"F12: {sel
+00012840: 662e 666b 6579 735b 2746 3132 275d 5b30  f.fkeys['F12'][0
+00012850: 5d7d 2229 0a20 2020 2020 2020 2020 2020  ]}").           
+00012860: 2073 656c 662e 4631 322e 7365 7454 6f6f   self.F12.setToo
+00012870: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+00012880: 2246 3132 225d 5b31 5d29 0a0a 2020 2020  "F12"][1])..    
+00012890: 6465 6620 6765 6e65 7261 7465 5f61 6469  def generate_adi
+000128a0: 6628 7365 6c66 293a 0a20 2020 2020 2020  f(self):.       
+000128b0: 2022 2222 4765 6e65 7261 7465 2041 4449   """Generate ADI
+000128c0: 4622 2222 0a20 2020 2020 2020 206c 6f67  F""".        log
+000128d0: 6765 722e 6465 6275 6728 222a 2a2a 2a2a  ger.debug("*****
+000128e0: 2a41 4449 462a 2a2a 2a2a 2229 0a20 2020  *ADIF*****").   
+000128f0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00012900: 742e 6164 6966 2873 656c 6629 0a0a 2020  t.adif(self)..  
+00012910: 2020 6465 6620 6765 6e65 7261 7465 5f63    def generate_c
+00012920: 6162 7269 6c6c 6f28 7365 6c66 293a 0a20  abrillo(self):. 
+00012930: 2020 2020 2020 2022 2222 4765 6e65 7261         """Genera
+00012940: 7465 7320 4361 6272 696c 6c6f 2066 696c  tes Cabrillo fil
+00012950: 652e 204d 6179 6265 2e22 2222 0a20 2020  e. Maybe.""".   
+00012960: 2020 2020 2023 2068 7474 7073 3a2f 2f77       # https://w
+00012970: 7777 2e63 7177 7078 2e63 6f6d 2f63 6162  ww.cqwpx.com/cab
+00012980: 7269 6c6c 6f2e 6874 6d0a 2020 2020 2020  rillo.htm.      
+00012990: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+000129a0: 2a2a 2a2a 2a2a 4361 6272 696c 6c6f 2a2a  ******Cabrillo**
+000129b0: 2a2a 2a22 290a 2020 2020 2020 2020 7365  ***").        se
+000129c0: 6c66 2e63 6f6e 7465 7374 2e63 6162 7269  lf.contest.cabri
+000129d0: 6c6c 6f28 7365 6c66 290a 0a0a 6465 6620  llo(self)...def 
+000129e0: 6c6f 6164 5f66 6f6e 7473 5f66 726f 6d5f  load_fonts_from_
+000129f0: 6469 7228 6469 7265 6374 6f72 793a 2073  dir(directory: s
+00012a00: 7472 2920 2d3e 2073 6574 3a0a 2020 2020  tr) -> set:.    
+00012a10: 2222 220a 2020 2020 5765 6c6c 2069 7420  """.    Well it 
+00012a20: 6c6f 6164 7320 666f 6e74 7320 6672 6f6d  loads fonts from
+00012a30: 2061 2064 6972 6563 746f 7279 2e2e 2e0a   a directory....
+00012a40: 2020 2020 2222 220a 2020 2020 666f 6e74      """.    font
+00012a50: 5f66 616d 696c 6965 7320 3d20 7365 7428  _families = set(
+00012a60: 290a 2020 2020 666f 7220 5f66 6920 696e  ).    for _fi in
+00012a70: 2051 4469 7228 6469 7265 6374 6f72 7929   QDir(directory)
+00012a80: 2e65 6e74 7279 496e 666f 4c69 7374 285b  .entryInfoList([
+00012a90: 222a 2e74 7466 222c 2022 2a2e 776f 6666  "*.ttf", "*.woff
+00012aa0: 222c 2022 2a2e 776f 6666 3222 5d29 3a0a  ", "*.woff2"]):.
+00012ab0: 2020 2020 2020 2020 5f69 6420 3d20 5146          _id = QF
+00012ac0: 6f6e 7444 6174 6162 6173 652e 6164 6441  ontDatabase.addA
+00012ad0: 7070 6c69 6361 7469 6f6e 466f 6e74 285f  pplicationFont(_
+00012ae0: 6669 2e61 6273 6f6c 7574 6546 696c 6550  fi.absoluteFileP
+00012af0: 6174 6828 2929 0a20 2020 2020 2020 2066  ath()).        f
+00012b00: 6f6e 745f 6661 6d69 6c69 6573 207c 3d20  ont_families |= 
+00012b10: 7365 7428 5146 6f6e 7444 6174 6162 6173  set(QFontDatabas
+00012b20: 652e 6170 706c 6963 6174 696f 6e46 6f6e  e.applicationFon
+00012b30: 7446 616d 696c 6965 7328 5f69 6429 290a  tFamilies(_id)).
+00012b40: 2020 2020 7265 7475 726e 2066 6f6e 745f      return font_
+00012b50: 6661 6d69 6c69 6573 0a0a 0a64 6566 2069  families...def i
+00012b60: 6e73 7461 6c6c 5f69 636f 6e73 2829 3a0a  nstall_icons():.
+00012b70: 2020 2020 2222 2249 6e73 7461 6c6c 2069      """Install i
+00012b80: 636f 6e73 2222 220a 2020 2020 6f73 2e73  cons""".    os.s
+00012b90: 7973 7465 6d28 0a20 2020 2020 2020 2022  ystem(.        "
+00012ba0: 7864 672d 6963 6f6e 2d72 6573 6f75 7263  xdg-icon-resourc
+00012bb0: 6520 696e 7374 616c 6c20 2d2d 7369 7a65  e install --size
+00012bc0: 2033 3220 2d2d 636f 6e74 6578 7420 6170   32 --context ap
+00012bd0: 7073 202d 2d6d 6f64 6520 7573 6572 2022  ps --mode user "
+00012be0: 0a20 2020 2020 2020 2066 227b 574f 524b  .        f"{WORK
+00012bf0: 494e 475f 5041 5448 7d2f 6461 7461 2f6b  ING_PATH}/data/k
+00012c00: 3667 7465 2e6e 6f74 316d 6d2d 3332 2e70  6gte.not1mm-32.p
+00012c10: 6e67 206b 3667 7465 2d6e 6f74 316d 6d22  ng k6gte-not1mm"
+00012c20: 0a20 2020 2029 0a20 2020 206f 732e 7379  .    ).    os.sy
+00012c30: 7374 656d 280a 2020 2020 2020 2020 2278  stem(.        "x
+00012c40: 6467 2d69 636f 6e2d 7265 736f 7572 6365  dg-icon-resource
+00012c50: 2069 6e73 7461 6c6c 202d 2d73 697a 6520   install --size 
+00012c60: 3634 202d 2d63 6f6e 7465 7874 2061 7070  64 --context app
+00012c70: 7320 2d2d 6d6f 6465 2075 7365 7220 220a  s --mode user ".
+00012c80: 2020 2020 2020 2020 6622 7b57 4f52 4b49          f"{WORKI
+00012c90: 4e47 5f50 4154 487d 2f64 6174 612f 6b36  NG_PATH}/data/k6
+00012ca0: 6774 652e 6e6f 7431 6d6d 2d36 342e 706e  gte.not1mm-64.pn
+00012cb0: 6720 6b36 6774 652d 6e6f 7431 6d6d 220a  g k6gte-not1mm".
+00012cc0: 2020 2020 290a 2020 2020 6f73 2e73 7973      ).    os.sys
+00012cd0: 7465 6d28 0a20 2020 2020 2020 2022 7864  tem(.        "xd
+00012ce0: 672d 6963 6f6e 2d72 6573 6f75 7263 6520  g-icon-resource 
+00012cf0: 696e 7374 616c 6c20 2d2d 7369 7a65 2031  install --size 1
+00012d00: 3238 202d 2d63 6f6e 7465 7874 2061 7070  28 --context app
+00012d10: 7320 2d2d 6d6f 6465 2075 7365 7220 220a  s --mode user ".
+00012d20: 2020 2020 2020 2020 6622 7b57 4f52 4b49          f"{WORKI
+00012d30: 4e47 5f50 4154 487d 2f64 6174 612f 6b36  NG_PATH}/data/k6
+00012d40: 6774 652e 6e6f 7431 6d6d 2d31 3238 2e70  gte.not1mm-128.p
+00012d50: 6e67 206b 3667 7465 2d6e 6f74 316d 6d22  ng k6gte-not1mm"
+00012d60: 0a20 2020 2029 0a20 2020 206f 732e 7379  .    ).    os.sy
+00012d70: 7374 656d 2866 2278 6467 2d64 6573 6b74  stem(f"xdg-deskt
+00012d80: 6f70 2d6d 656e 7520 696e 7374 616c 6c20  op-menu install 
+00012d90: 7b57 4f52 4b49 4e47 5f50 4154 487d 2f64  {WORKING_PATH}/d
+00012da0: 6174 612f 6b36 6774 652d 6e6f 7431 6d6d  ata/k6gte-not1mm
+00012db0: 2e64 6573 6b74 6f70 2229 0a0a 0a64 6566  .desktop")...def
+00012dc0: 2064 6f69 6d70 286d 6f64 6e61 6d65 293a   doimp(modname):
+00012dd0: 0a20 2020 2022 2222 7265 7475 726e 206d  .    """return m
+00012de0: 6f64 756c 6520 7061 7468 2222 220a 2020  odule path""".  
+00012df0: 2020 7265 7475 726e 2069 6d70 6f72 746c    return importl
+00012e00: 6962 2e69 6d70 6f72 745f 6d6f 6475 6c65  ib.import_module
+00012e10: 2866 226e 6f74 316d 6d2e 706c 7567 696e  (f"not1mm.plugin
+00012e20: 732e 7b6d 6f64 6e61 6d65 7d22 290a 0a0a  s.{modname}")...
+00012e30: 6465 6620 7275 6e28 293a 0a20 2020 2022  def run():.    "
+00012e40: 2222 0a20 2020 204d 6169 6e20 456e 7472  "".    Main Entr
+00012e50: 790a 2020 2020 2222 220a 0a20 2020 2069  y.    """..    i
+00012e60: 6e73 7461 6c6c 5f69 636f 6e73 2829 0a20  nstall_icons(). 
+00012e70: 2020 2074 696d 6572 2e73 7461 7274 2831     timer.start(1
+00012e80: 3030 3029 0a20 2020 2074 696d 6572 322e  000).    timer2.
+00012e90: 7374 6172 7428 3130 3030 290a 0a20 2020  start(1000)..   
+00012ea0: 2073 7973 2e65 7869 7428 6170 702e 6578   sys.exit(app.ex
+00012eb0: 6563 2829 290a 0a0a 6c6f 6767 6572 203d  ec())...logger =
+00012ec0: 206c 6f67 6769 6e67 2e67 6574 4c6f 6767   logging.getLogg
+00012ed0: 6572 2822 5f5f 6d61 696e 5f5f 2229 0a68  er("__main__").h
+00012ee0: 616e 646c 6572 203d 206c 6f67 6769 6e67  andler = logging
+00012ef0: 2e53 7472 6561 6d48 616e 646c 6572 2829  .StreamHandler()
+00012f00: 0a66 6f72 6d61 7474 6572 203d 206c 6f67  .formatter = log
+00012f10: 6769 6e67 2e46 6f72 6d61 7474 6572 280a  ging.Formatter(.
+00012f20: 2020 2020 6461 7465 666d 743d 2225 483a      datefmt="%H:
+00012f30: 254d 3a25 5322 2c0a 2020 2020 666d 743d  %M:%S",.    fmt=
+00012f40: 225b 2528 6173 6374 696d 6529 735d 2025  "[%(asctime)s] %
+00012f50: 286c 6576 656c 6e61 6d65 2973 2025 286d  (levelname)s %(m
+00012f60: 6f64 756c 6529 7320 2d20 2528 6675 6e63  odule)s - %(func
+00012f70: 4e61 6d65 2973 204c 696e 6520 2528 6c69  Name)s Line %(li
+00012f80: 6e65 6e6f 2964 3a20 2528 6d65 7373 6167  neno)d: %(messag
+00012f90: 6529 7322 2c0a 290a 6861 6e64 6c65 722e  e)s",.).handler.
+00012fa0: 7365 7446 6f72 6d61 7474 6572 2866 6f72  setFormatter(for
+00012fb0: 6d61 7474 6572 290a 6c6f 6767 6572 2e61  matter).logger.a
+00012fc0: 6464 4861 6e64 6c65 7228 6861 6e64 6c65  ddHandler(handle
+00012fd0: 7229 0a0a 6966 2050 6174 6828 222e 2f64  r)..if Path("./d
+00012fe0: 6562 7567 2229 2e65 7869 7374 7328 293a  ebug").exists():
+00012ff0: 0a20 2020 206c 6f67 6765 722e 7365 744c  .    logger.setL
+00013000: 6576 656c 286c 6f67 6769 6e67 2e44 4542  evel(logging.DEB
+00013010: 5547 290a 2020 2020 6c6f 6767 6572 2e64  UG).    logger.d
+00013020: 6562 7567 2822 6465 6275 6767 696e 6720  ebug("debugging 
+00013030: 6f6e 2229 0a65 6c73 653a 0a20 2020 206c  on").else:.    l
+00013040: 6f67 6765 722e 7365 744c 6576 656c 286c  ogger.setLevel(l
+00013050: 6f67 6769 6e67 2e57 4152 4e49 4e47 290a  ogging.WARNING).
+00013060: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+00013070: 6e67 2822 6465 6275 6767 696e 6720 6f66  ng("debugging of
+00013080: 6622 290a 0a61 7070 203d 2051 7457 6964  f")..app = QtWid
+00013090: 6765 7473 2e51 4170 706c 6963 6174 696f  gets.QApplicatio
+000130a0: 6e28 7379 732e 6172 6776 290a 6170 702e  n(sys.argv).app.
+000130b0: 7365 7453 7479 6c65 2822 4675 7369 6f6e  setStyle("Fusion
+000130c0: 2229 0a66 6f6e 745f 7061 7468 203d 2057  ").font_path = W
+000130d0: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
+000130e0: 6461 7461 220a 6661 6d69 6c69 6573 203d  data".families =
+000130f0: 206c 6f61 645f 666f 6e74 735f 6672 6f6d   load_fonts_from
+00013100: 5f64 6972 286f 732e 6673 7061 7468 2866  _dir(os.fspath(f
+00013110: 6f6e 745f 7061 7468 2929 0a6c 6f67 6765  ont_path)).logge
+00013120: 722e 696e 666f 2866 616d 696c 6965 7329  r.info(families)
+00013130: 0a77 696e 646f 7720 3d20 4d61 696e 5769  .window = MainWi
+00013140: 6e64 6f77 2829 0a68 6569 6768 7420 3d20  ndow().height = 
+00013150: 7769 6e64 6f77 2e70 7265 662e 6765 7428  window.pref.get(
+00013160: 2277 696e 646f 775f 6865 6967 6874 222c  "window_height",
+00013170: 2033 3030 290a 7769 6474 6820 3d20 7769   300).width = wi
+00013180: 6e64 6f77 2e70 7265 662e 6765 7428 2277  ndow.pref.get("w
+00013190: 696e 646f 775f 7769 6474 6822 2c20 3730  indow_width", 70
+000131a0: 3029 0a78 203d 2077 696e 646f 772e 7072  0).x = window.pr
+000131b0: 6566 2e67 6574 2822 7769 6e64 6f77 5f78  ef.get("window_x
+000131c0: 222c 202d 3129 0a79 203d 2077 696e 646f  ", -1).y = windo
+000131d0: 772e 7072 6566 2e67 6574 2822 7769 6e64  w.pref.get("wind
+000131e0: 6f77 5f79 222c 202d 3129 0a77 696e 646f  ow_y", -1).windo
+000131f0: 772e 7365 7447 656f 6d65 7472 7928 782c  w.setGeometry(x,
+00013200: 2079 2c20 7769 6474 682c 2068 6569 6768   y, width, heigh
+00013210: 7429 0a23 2077 696e 646f 772e 7365 7457  t).# window.setW
+00013220: 696e 646f 7754 6974 6c65 2866 224e 6f74  indowTitle(f"Not
+00013230: 314d 4d20 767b 5f5f 7665 7273 696f 6e5f  1MM v{__version_
+00013240: 5f7d 2229 0a77 696e 646f 772e 6361 6c6c  _}").window.call
+00013250: 7369 676e 2e73 6574 466f 6375 7328 290a  sign.setFocus().
+00013260: 7769 6e64 6f77 2e73 686f 7728 290a 7469  window.show().ti
+00013270: 6d65 7220 3d20 5174 436f 7265 2e51 5469  mer = QtCore.QTi
+00013280: 6d65 7228 290a 7469 6d65 722e 7469 6d65  mer().timer.time
+00013290: 6f75 742e 636f 6e6e 6563 7428 7769 6e64  out.connect(wind
+000132a0: 6f77 2e70 6f6c 6c5f 7261 6469 6f29 0a74  ow.poll_radio).t
+000132b0: 696d 6572 3220 3d20 5174 436f 7265 2e51  imer2 = QtCore.Q
+000132c0: 5469 6d65 7228 290a 7469 6d65 7232 2e74  Timer().timer2.t
+000132d0: 696d 656f 7574 2e63 6f6e 6e65 6374 2877  imeout.connect(w
+000132e0: 696e 646f 772e 6368 6563 6b5f 7564 705f  indow.check_udp_
+000132f0: 7472 6166 6669 6329 0a0a 6966 205f 5f6e  traffic)..if __n
+00013300: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+00013310: 5f5f 223a 0a20 2020 2072 756e 2829 0a    __":.    run().
```

### Comparing `not1mm-23.5.6/not1mm/bandmap.py` & `not1mm-23.5.7/not1mm/bandmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from datetime import datetime
 from json import JSONDecodeError, loads, dumps
 from pathlib import Path
 
 import logging
 import os
 import pkgutil
+import platform
 import sys
 import sqlite3
 
 from PyQt5 import QtCore, QtGui, Qt
 from PyQt5 import QtNetwork
 from PyQt5 import QtWidgets, uic
 
@@ -189,14 +190,16 @@
     rxMark = []
     rx_freq = None
     tx_freq = None
     something = None
     lineitemlist = []
     textItemList = []
     connected = False
+    bandwidth = 0
+    bandwidth_mark = []
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._udpwatch = None
         data_path = WORKING_PATH + "/data/bandmap.ui"
         uic.loadUi(data_path, self)
         self.agetime = self.clear_spot_olderSpinBox.value()
@@ -258,28 +261,33 @@
                 the_error = f"Not Unicode: {err}\n{bundle}"
                 logger.debug(the_error)
                 continue
             except JSONDecodeError as err:
                 the_error = f"Not JSON: {err}\n{bundle}"
                 logger.debug(the_error)
                 continue
-            if packet.get("cmd", "") == "RADIO_STATE":
+            if (
+                packet.get("cmd", "") == "RADIO_STATE"
+                and packet.get("station", "") == platform.node()
+            ):
                 self.set_band(packet.get("band") + "m", False)
                 self.rx_freq = float(packet.get("vfoa")) / 1000000
                 self.tx_freq = self.rx_freq
+                self.bandwidth = int(packet.get("bw", "0"))
                 step, _ = self.determine_step_digits()
                 self.drawTXRXMarks(step)
 
     def spot_clicked(self):
         """dunno"""
         items = self.bandmap_scene.selectedItems()
         for item in items:
             if item:
                 cmd = {}
                 cmd["cmd"] = "TUNE"
+                cmd["station"] = platform.node()
                 cmd["freq"] = items[0].property("freq")
                 cmd["spot"] = items[0].toPlainText().split()[0]
                 packet = bytes(dumps(cmd), encoding="ascii")
                 self.udpsocket.writeDatagram(
                     packet, QtNetwork.QHostAddress(MULTICAST_GROUP), MULTICAST_PORT
                 )
 
@@ -289,14 +297,15 @@
 
     def update(self):
         """doc"""
         self.update_timer.setInterval(UPDATE_INTERVAL)
         self.clear_all_callsign_from_scene()
         self.clear_freq_mark(self.rxMark)
         self.clear_freq_mark(self.txMark)
+        self.clear_freq_mark(self.bandwidth_mark)
         self.bandmap_scene.clear()
 
         step, _digits = self.determine_step_digits()
         steps = int(round((self.currentBand.end - self.currentBand.start) / step))
         self.graphicsView.setFixedSize(330, steps * PIXELSPERSTEP + 30)
         self.graphicsView.setScene(self.bandmap_scene)
         for i in range(steps):
@@ -339,15 +348,19 @@
         self.zoom -= 1
         self.zoom = max(self.zoom, 1)
         self.update()
 
     def drawTXRXMarks(self, step):
         """doc"""
         if self.rx_freq:
+            self.clear_freq_mark(self.bandwidth_mark)
             self.clear_freq_mark(self.rxMark)
+            self.draw_bandwidth(
+                self.rx_freq, step, QtGui.QColor(30, 30, 180), self.bandwidth_mark
+            )
             self.drawfreqmark(
                 self.rx_freq, step, QtGui.QColor(30, 180, 30), self.rxMark
             )
 
     def Freq2ScenePos(self, freq: float):
         """doc"""
         if freq < self.currentBand.start or freq > self.currentBand.end:
@@ -358,15 +371,14 @@
         )
         return ret
 
     def drawfreqmark(self, freq, step, color, currentPolygon):
         """doc"""
 
         self.clear_freq_mark(currentPolygon)
-
         # do not show the freq mark if it is outside the bandmap
         if freq < self.currentBand.start or freq > self.currentBand.end:
             return
 
         Yposition = self.Freq2ScenePos(freq).y()
 
         poly = QtGui.QPolygonF()
@@ -374,14 +386,36 @@
         poly.append(QtCore.QPointF(21, Yposition))
         poly.append(QtCore.QPointF(10, Yposition - 7))
         poly.append(QtCore.QPointF(10, Yposition + 7))
         pen = QtGui.QPen()
         brush = QtGui.QBrush(color)
         currentPolygon.append(self.bandmap_scene.addPolygon(poly, pen, brush))
 
+    def draw_bandwidth(self, freq, step, color, currentPolygon):
+        """bandwidth"""
+        logger.debug("%s", f"mark:{currentPolygon} f:{freq} b:{self.bandwidth}")
+        self.clear_freq_mark(currentPolygon)
+        if freq < self.currentBand.start or freq > self.currentBand.end:
+            return
+        if freq and self.bandwidth:
+            color = QtGui.QColor(30, 30, 180)
+            bw_start = freq - ((self.bandwidth / 2) / 1000000)
+            bw_end = freq + ((self.bandwidth / 2) / 1000000)
+            logger.debug("%s", f"s:{bw_start} e:{bw_end}")
+            Yposition_neg = self.Freq2ScenePos(bw_start).y()
+            Yposition_pos = self.Freq2ScenePos(bw_end).y()
+            poly = QtGui.QPolygonF()
+            poly.append(QtCore.QPointF(15, Yposition_neg))
+            poly.append(QtCore.QPointF(20, Yposition_neg))
+            poly.append(QtCore.QPointF(20, Yposition_pos))
+            poly.append(QtCore.QPointF(15, Yposition_pos))
+            pen = QtGui.QPen()
+            brush = QtGui.QBrush(color)
+            currentPolygon.append(self.bandmap_scene.addPolygon(poly, pen, brush))
+
     def update_stations(self):
         """doc"""
         self.update_timer.setInterval(UPDATE_INTERVAL)
         self.clear_all_callsign_from_scene()
         self.spot_aging()
         step, _digits = self.determine_step_digits()
 
@@ -482,14 +516,15 @@
     def receive(self):
         """doc"""
         data = self.socket.readAll()
         data = str(data, "utf-8").strip()
         if "login:" in data:
             self.send_command(self.callsignField.text())
             self.send_command(PREF.get("cluster_filter", ""))
+            self.send_command("set dx extension Name CTY State Section")
             self.send_command("set dx mode " + PREF.get("cluster_mode", "OPEN"))
             return
         if "DX de" in data:
             parts = data.split()
             spotter = parts[2]
             freq = parts[3]
             dx = parts[4]
```

### Comparing `not1mm-23.5.6/not1mm/data/Combinear.qss` & `not1mm-23.5.7/not1mm/data/Combinear.qss`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.5.7/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/MASTER.SCP` & `not1mm-23.5.7/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/about.ui` & `not1mm-23.5.7/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/bandmap.ui` & `not1mm-23.5.7/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/configuration.ui` & `not1mm-23.5.7/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/contests.sql` & `not1mm-23.5.7/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/cty.json` & `not1mm-23.5.7/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/editcontact.ui` & `not1mm-23.5.7/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/editmacro.ui` & `not1mm-23.5.7/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.5.7/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.5.7/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.5.7/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/logwindow.ui` & `not1mm-23.5.7/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/main.ui` & `not1mm-23.5.7/not1mm/data/main.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/new_contest.ui` & `not1mm-23.5.7/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/opon.ui` & `not1mm-23.5.7/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/0.wav` & `not1mm-23.5.7/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/1.wav` & `not1mm-23.5.7/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/2.wav` & `not1mm-23.5.7/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/3.wav` & `not1mm-23.5.7/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/4.wav` & `not1mm-23.5.7/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/5.wav` & `not1mm-23.5.7/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/6.wav` & `not1mm-23.5.7/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/7.wav` & `not1mm-23.5.7/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/73.wav` & `not1mm-23.5.7/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/8.wav` & `not1mm-23.5.7/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/9.wav` & `not1mm-23.5.7/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/a.wav` & `not1mm-23.5.7/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/again.wav` & `not1mm-23.5.7/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/b.wav` & `not1mm-23.5.7/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/c.wav` & `not1mm-23.5.7/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/contest.wav` & `not1mm-23.5.7/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/cq.wav` & `not1mm-23.5.7/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/d.wav` & `not1mm-23.5.7/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/e.wav` & `not1mm-23.5.7/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/f.wav` & `not1mm-23.5.7/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/g.wav` & `not1mm-23.5.7/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/h.wav` & `not1mm-23.5.7/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/i.wav` & `not1mm-23.5.7/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/j.wav` & `not1mm-23.5.7/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/k.wav` & `not1mm-23.5.7/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.5.7/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/l.wav` & `not1mm-23.5.7/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/m.wav` & `not1mm-23.5.7/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.5.7/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/n.wav` & `not1mm-23.5.7/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/nil.wav` & `not1mm-23.5.7/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/o.wav` & `not1mm-23.5.7/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/p.wav` & `not1mm-23.5.7/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/q.wav` & `not1mm-23.5.7/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/r.wav` & `not1mm-23.5.7/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/roger.wav` & `not1mm-23.5.7/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/s.wav` & `not1mm-23.5.7/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/space.wav` & `not1mm-23.5.7/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/t.wav` & `not1mm-23.5.7/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.5.7/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.5.7/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/u.wav` & `not1mm-23.5.7/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/v.wav` & `not1mm-23.5.7/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/w.wav` & `not1mm-23.5.7/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/x.wav` & `not1mm-23.5.7/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/y.wav` & `not1mm-23.5.7/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.5.7/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/phonetics/z.wav` & `not1mm-23.5.7/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/pickcontest.ui` & `not1mm-23.5.7/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/reddot.png` & `not1mm-23.5.7/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/data/settings.ui` & `not1mm-23.5.7/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/cat_interface.py` & `not1mm-23.5.7/not1mm/lib/cat_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,14 +152,52 @@
                 self.online = False
                 logger.debug("%s", exception)
                 self.rigctrlsocket = None
             return ""
         self.__initialize_rigctrld()
         return ""
 
+    def get_bw(self):
+        """Get current vfo bandwidth"""
+        if self.interface == "flrig":
+            return self.__getbw_flrig()
+        if self.interface == "rigctld":
+            return self.__getbw_rigctld()
+        return False
+
+    def __getbw_flrig(self):
+        """ccc"""
+        try:
+            self.online = True
+            return self.server.rig.get_bw()
+        except ConnectionRefusedError as exception:
+            self.online = False
+            logger.debug("getbw_flrig: %s", exception)
+            return ""
+
+    def __getbw_rigctld(self):
+        """ccc"""
+        if self.rigctrlsocket:
+            try:
+                self.online = True
+                self.rigctrlsocket.send(b"m\n")
+                mode = self.rigctrlsocket.recv(1024).decode()
+                mode = mode.strip().split()[1]
+                logger.debug("%s", mode)
+                return mode
+            except IndexError as exception:
+                logger.debug("%s", exception)
+            except socket.error as exception:
+                self.online = False
+                logger.debug("%s", exception)
+                self.rigctrlsocket = None
+            return ""
+        self.__initialize_rigctrld()
+        return ""
+
     def get_power(self):
         """Get power level from rig"""
         if self.interface == "flrig":
             return self.__getpower_flrig()
         if self.interface == "rigctld":
             return self.__getpower_rigctld()
         return False
```

### Comparing `not1mm-23.5.6/not1mm/lib/cwinterface.py` & `not1mm-23.5.7/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/database.py` & `not1mm-23.5.7/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/edit_macro.py` & `not1mm-23.5.7/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/edit_station.py` & `not1mm-23.5.7/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/ham_utility.py` & `not1mm-23.5.7/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/lookup.py` & `not1mm-23.5.7/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/multicast.py` & `not1mm-23.5.7/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/n1mm.py` & `not1mm-23.5.7/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/lib/settings.py` & `not1mm-23.5.7/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/logwindow.py` & `not1mm-23.5.7/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.5.7/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.5.7/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.5.7/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.5.7/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.5.7/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.5.7/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/arrl_field_day.py` & `not1mm-23.5.7/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.5.7/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.5.7/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.5.7/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.5.7/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.5.7/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.5.7/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.5.7/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/cwt.py` & `not1mm-23.5.7/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/general_logging.py` & `not1mm-23.5.7/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/jidx_cw.py` & `not1mm-23.5.7/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/jidx_ph.py` & `not1mm-23.5.7/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/plugins/winter_field_day.py` & `not1mm-23.5.7/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm/testing/test.py` & `not1mm-23.5.7/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/not1mm.egg-info/PKG-INFO` & `not1mm-23.5.7/not1mm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.5.6
+Version: 23.5.7
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -119,15 +119,16 @@
 - CQ World Wide SSB
 - CWOps CWT
 - Japan International DX CW
 - Japan International DX SSB
 
 ## Changes of note
 
-- [23-5-6] Added AR Cluster filter options for the bandmap.
+- [23-5-7] Added bandwidth marker to the bandmap.
+- [23-5-6] Added AR Cluster filter options for the bandmap. Added a station ID to the multicast packets. This will prevent erratic bevahiour if 2 stations are on the same network.
 - [23-5-5] Re-wrote most of the log window code. Added ARRL Sweepstakes.
 - [23-5-4] Fixed 'Operators' line in WPX cabrillo file. Fix window title not updating if no CAT control.
 - [23-5-3] Added '#' macro.
 - [23-5-1] Added 10 10 CW and Phone contests. Added a `Cluster` TAB for the AR Cluster server/port in the configuration settings.
 
 <details>
 
@@ -158,15 +159,15 @@
 - [23-3-31] Now saving station settings in the contest database.
 - [23-3-30] Added Open new and Open existing database
 - [23-3-29] Added a new contest dialog.
 - [23-3-27] Add menu item to recalculate mults.
 - [23-3-27] Fix cursor behaviour when editing text in callsign field.
 - [23-3-25] Fix minimum call length. Fix cabrillo tag. Add adif output.
 - [23-3-24] Added dupe checking. Added CAT check for flrig or rigctld. Added online flag for flrig.
-- [23-3-23] Added most of Cabrillo generation. Plan to test it this weekends CQ WPX SSB.
+- [23-3-23] Added json_data.get("cmd", "")most of Cabrillo generation. Plan to test it this weekends CQ WPX SSB.
 - [23-3-22] Add prefill of serial nr. set OP call on startup. Set IsMultiplier1 new unique wpx. Add OP and contest name to window title. and stuff.
 - [23-3-21] Worked on CQ WPX SSB plugin.
 - [23-3-20] Added a contact edit dialog. RightClick to edit contact. Changed placeholder text color in settings dialog. Hooked up CW speedchange widget. PgUp/PgDn to change speed.
 - [23-3-17] Added multicast UDP messages to update the log window when new contact made. You can now edit existing contacts in the log window. You can't delete them yet. Got rid of watchdog. Isolated common multicast code to it's own class.
 - [23-3-15] Added a rudimentary log view window.
 - [23-3-10] Started work on saving contacts to the DB. Added a claculate_wpx_prefix routine.
 - [23-3-9] Placed network call lookup in a thread. Display freq/mode for non CAT radios. Hooked up the CW macros to cwdaemon.
@@ -247,14 +248,16 @@
 
 ```bash
 not1mm
 ```
 
 ## Various data file locations
 
+json_data.get("cmd", "")
+
 ### Data
 
 If your system has an `XDG_DATA_HOME` environment variable set, the database and CW macro files can be found there. Otherwise they will be found at `yourhome/.local/share/not1mm`
 
 ### Config
 
 Configuration file(s) can be found at the location defined by `XDG_CONFIG_HOME`. Otherwise they will be found at `yourhome/.config/not1mm`
```

### Comparing `not1mm-23.5.6/not1mm.egg-info/SOURCES.txt` & `not1mm-23.5.7/not1mm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `not1mm-23.5.6/pyproject.toml` & `not1mm-23.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.5.6"
+version = "23.5.7"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `not1mm-23.5.6/testing/test.py` & `not1mm-23.5.7/testing/test.py`

 * *Files identical despite different names*

