# Comparing `tmp/flet-material-0.2.0.tar.gz` & `tmp/flet-material-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet-material-0.2.0.tar", last modified: Mon Apr 24 13:04:25 2023, max compression
+gzip compressed data, was "flet-material-0.3.0.tar", last modified: Mon May  8 17:35:11 2023, max compression
```

## Comparing `flet-material-0.2.0.tar` & `flet-material-0.3.0.tar`

### file list

```diff
@@ -1,152 +1,153 @@
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.258348 flet-material-0.2.0/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.205508 flet-material-0.2.0/.github/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.210761 flet-material-0.2.0/.github/workflows/
--rw-r--r--   0 ahmad      (501) staff       (20)      496 2023-04-23 18:54:25.000000 flet-material-0.2.0/.github/workflows/build.yml
--rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-04-24 09:59:38.000000 flet-material-0.2.0/.gitignore
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.211162 flet-material-0.2.0/.vscode/
--rw-r--r--   0 ahmad      (501) staff       (20)       64 2023-04-21 12:22:35.000000 flet-material-0.2.0/.vscode/settings.json
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-24 11:04:16.000000 flet-material-0.2.0/CHANGELOG.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-22 18:06:15.000000 flet-material-0.2.0/LICENSE
--rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-04-24 13:04:25.257946 flet-material-0.2.0/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     3839 2023-04-24 12:56:14.000000 flet-material-0.2.0/README.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.211694 flet-material-0.2.0/command/
--rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-23 08:17:07.000000 flet-material-0.2.0/command/__init__.py
--rw-r--r--   0 ahmad      (501) staff       (20)      682 2023-04-23 17:03:12.000000 flet-material-0.2.0/command/new_project.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.212032 flet-material-0.2.0/docs/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.212757 flet-material-0.2.0/docs/docs/
--rw-r--r--   0 ahmad      (501) staff       (20)     1819 2023-04-24 12:26:23.000000 flet-material-0.2.0/docs/docs/contribute.md
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.215803 flet-material-0.2.0/docs/docs/controls/
--rw-r--r--   0 ahmad      (501) staff       (20)     1975 2023-04-24 12:09:58.000000 flet-material-0.2.0/docs/docs/controls/alerts.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1357 2023-04-24 12:10:06.000000 flet-material-0.2.0/docs/docs/controls/annotations.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3198 2023-04-24 11:12:12.000000 flet-material-0.2.0/docs/docs/controls/badges.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1566 2023-04-23 16:04:13.000000 flet-material-0.2.0/docs/docs/controls/buttons.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1605 2023-04-24 12:10:25.000000 flet-material-0.2.0/docs/docs/controls/checkboxes.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1434 2023-04-24 12:10:31.000000 flet-material-0.2.0/docs/docs/controls/chips.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3023 2023-04-24 12:10:54.000000 flet-material-0.2.0/docs/docs/controls/dropdowns.md
--rw-r--r--   0 ahmad      (501) staff       (20)     2811 2023-04-23 14:49:45.000000 flet-material-0.2.0/docs/docs/controls/index.md
--rw-r--r--   0 ahmad      (501) staff       (20)     1296 2023-04-24 12:10:56.000000 flet-material-0.2.0/docs/docs/controls/switches.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3038 2023-04-24 12:28:23.000000 flet-material-0.2.0/docs/docs/index.md
--rw-r--r--   0 ahmad      (501) staff       (20)     3070 2023-04-24 12:35:43.000000 flet-material-0.2.0/docs/mkdocs.yml
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.217357 flet-material-0.2.0/docs/site/
--rw-r--r--   0 ahmad      (501) staff       (20)        8 2023-04-24 12:45:17.000000 flet-material-0.2.0/docs/site/.gitignore
--rw-r--r--   0 ahmad      (501) staff       (20)    28461 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/404.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.206826 flet-material-0.2.0/docs/site/assets/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.217603 flet-material-0.2.0/docs/site/assets/images/
--rw-r--r--   0 ahmad      (501) staff       (20)     1870 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/images/favicon.png
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.218731 flet-material-0.2.0/docs/site/assets/javascripts/
--rw-r--r--   0 ahmad      (501) staff       (20)   113367 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/bundle.51198bba.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)   950772 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/bundle.51198bba.min.js.map
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.221249 flet-material-0.2.0/docs/site/assets/javascripts/lunr/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.232393 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/
--rw-r--r--   0 ahmad      (501) staff       (20)    17074 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     4654 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     6119 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     6208 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    11499 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     9342 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10669 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     3383 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     9437 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    11232 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     2313 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     7973 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)      817 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     6026 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     4754 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10171 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10958 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    10331 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     3647 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     4523 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     2406 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     1031 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    15009 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)      784 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)     2062 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)    22878 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0 ahmad      (501) staff       (20)   677455 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/lunr/wordcut.js
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.233555 flet-material-0.2.0/docs/site/assets/javascripts/workers/
--rw-r--r--   0 ahmad      (501) staff       (20)    38916 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0 ahmad      (501) staff       (20)   209901 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/javascripts/workers/search.208ed371.min.js.map
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.236568 flet-material-0.2.0/docs/site/assets/stylesheets/
--rw-r--r--   0 ahmad      (501) staff       (20)   113417 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/main.ded33207.min.css
--rw-r--r--   0 ahmad      (501) staff       (20)    38957 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/main.ded33207.min.css.map
--rw-r--r--   0 ahmad      (501) staff       (20)    12355 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css
--rw-r--r--   0 ahmad      (501) staff       (20)     3646 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.237141 flet-material-0.2.0/docs/site/contribute/
--rw-r--r--   0 ahmad      (501) staff       (20)    32427 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/contribute/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.237796 flet-material-0.2.0/docs/site/controls/
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.238199 flet-material-0.2.0/docs/site/controls/alerts/
--rw-r--r--   0 ahmad      (501) staff       (20)    38198 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/alerts/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.238610 flet-material-0.2.0/docs/site/controls/annotations/
--rw-r--r--   0 ahmad      (501) staff       (20)    34841 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/annotations/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.238997 flet-material-0.2.0/docs/site/controls/badges/
--rw-r--r--   0 ahmad      (501) staff       (20)    48809 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/badges/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.239460 flet-material-0.2.0/docs/site/controls/buttons/
--rw-r--r--   0 ahmad      (501) staff       (20)    37505 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/buttons/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.239843 flet-material-0.2.0/docs/site/controls/checkboxes/
--rw-r--r--   0 ahmad      (501) staff       (20)    37319 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/checkboxes/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.240208 flet-material-0.2.0/docs/site/controls/chips/
--rw-r--r--   0 ahmad      (501) staff       (20)    36557 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/chips/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.240601 flet-material-0.2.0/docs/site/controls/dropdowns/
--rw-r--r--   0 ahmad      (501) staff       (20)    46447 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/dropdowns/index.html
--rw-r--r--   0 ahmad      (501) staff       (20)    32736 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.240964 flet-material-0.2.0/docs/site/controls/switches/
--rw-r--r--   0 ahmad      (501) staff       (20)    36069 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/controls/switches/index.html
--rw-r--r--   0 ahmad      (501) staff       (20)    38036 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/index.html
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.241333 flet-material-0.2.0/docs/site/search/
--rw-r--r--   0 ahmad      (501) staff       (20)    21578 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/search/search_index.json
--rw-r--r--   0 ahmad      (501) staff       (20)     1484 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/sitemap.xml
--rw-r--r--   0 ahmad      (501) staff       (20)      204 2023-04-24 12:44:20.000000 flet-material-0.2.0/docs/site/sitemap.xml.gz
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.245151 flet-material-0.2.0/flet_material/
--rw-r--r--   0 ahmad      (501) staff       (20)      421 2023-04-23 11:09:44.000000 flet-material-0.2.0/flet_material/__init__.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.251647 flet-material-0.2.0/flet_material/__pycache__/
--rw-r--r--   0 ahmad      (501) staff       (20)      706 2023-04-23 11:09:44.000000 flet-material-0.2.0/flet_material/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     4049 2023-04-24 11:44:19.000000 flet-material-0.2.0/flet_material/__pycache__/admonition.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1892 2023-04-22 18:01:00.000000 flet-material-0.2.0/flet_material/__pycache__/alert.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1697 2023-04-21 17:58:50.000000 flet-material-0.2.0/flet_material/__pycache__/annotation.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1834 2023-04-21 16:25:55.000000 flet-material-0.2.0/flet_material/__pycache__/annotations.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     3211 2023-04-23 15:51:31.000000 flet-material-0.2.0/flet_material/__pycache__/badge.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      738 2023-04-23 14:56:58.000000 flet-material-0.2.0/flet_material/__pycache__/base.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1597 2023-04-23 18:10:10.000000 flet-material-0.2.0/flet_material/__pycache__/button.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1525 2023-04-23 11:36:01.000000 flet-material-0.2.0/flet_material/__pycache__/checkbox.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-24 11:30:35.000000 flet-material-0.2.0/flet_material/__pycache__/chip.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-22 14:16:22.000000 flet-material-0.2.0/flet_material/__pycache__/switch.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     6919 2023-04-24 11:44:19.000000 flet-material-0.2.0/flet_material/admonition.py
--rw-r--r--   0 ahmad      (501) staff       (20)     2689 2023-04-22 18:01:00.000000 flet-material-0.2.0/flet_material/alert.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1503 2023-04-21 17:58:49.000000 flet-material-0.2.0/flet_material/annotation.py
--rw-r--r--   0 ahmad      (501) staff       (20)     4731 2023-04-23 15:51:31.000000 flet-material-0.2.0/flet_material/badge.py
--rw-r--r--   0 ahmad      (501) staff       (20)      358 2023-04-23 14:56:57.000000 flet-material-0.2.0/flet_material/base.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1425 2023-04-23 18:09:54.000000 flet-material-0.2.0/flet_material/button.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1038 2023-04-23 11:36:00.000000 flet-material-0.2.0/flet_material/checkbox.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1528 2023-04-24 11:30:35.000000 flet-material-0.2.0/flet_material/chip.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1399 2023-04-22 14:16:22.000000 flet-material-0.2.0/flet_material/switch.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.246825 flet-material-0.2.0/flet_material.egg-info/
--rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/PKG-INFO
--rw-r--r--   0 ahmad      (501) staff       (20)     4488 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/SOURCES.txt
--rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/dependency_links.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       83 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/entry_points.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       25 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/requires.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       21 2023-04-24 13:04:25.000000 flet-material-0.2.0/flet_material.egg-info/top_level.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       24 2023-04-22 18:53:13.000000 flet-material-0.2.0/requirements.txt
--rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-04-24 13:04:25.258414 flet-material-0.2.0/setup.cfg
--rw-r--r--   0 ahmad      (501) staff       (20)      805 2023-04-24 13:04:08.000000 flet-material-0.2.0/setup.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.254038 flet-material-0.2.0/styles/
--rw-r--r--   0 ahmad      (501) staff       (20)      271 2023-04-22 17:17:29.000000 flet-material-0.2.0/styles/__init__.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.256769 flet-material-0.2.0/styles/__pycache__/
--rw-r--r--   0 ahmad      (501) staff       (20)      499 2023-04-22 17:17:29.000000 flet-material-0.2.0/styles/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      708 2023-04-23 11:20:49.000000 flet-material-0.2.0/styles/__pycache__/admonition_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      493 2023-04-22 17:30:06.000000 flet-material-0.2.0/styles/__pycache__/alert_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      494 2023-04-22 17:08:25.000000 flet-material-0.2.0/styles/__pycache__/alert_styles.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      487 2023-04-22 16:10:03.000000 flet-material-0.2.0/styles/__pycache__/badge_style.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      287 2023-04-21 16:08:17.000000 flet-material-0.2.0/styles/__pycache__/fonts.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)     1040 2023-04-23 14:54:06.000000 flet-material-0.2.0/styles/__pycache__/theme.cpython-310.pyc
--rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-04-23 11:20:48.000000 flet-material-0.2.0/styles/admonition_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)      378 2023-04-22 17:30:06.000000 flet-material-0.2.0/styles/alert_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)      361 2023-04-22 16:10:02.000000 flet-material-0.2.0/styles/badge_style.py
--rw-r--r--   0 ahmad      (501) staff       (20)       90 2023-04-21 16:07:16.000000 flet-material-0.2.0/styles/fonts.py
--rw-r--r--   0 ahmad      (501) staff       (20)     1421 2023-04-23 14:18:26.000000 flet-material-0.2.0/styles/theme.py
-drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-04-24 13:04:25.257510 flet-material-0.2.0/tests/
--rw-r--r--   0 ahmad      (501) staff       (20)      514 2023-04-23 19:11:47.000000 flet-material-0.2.0/tests/test_admonitions.py
--rw-r--r--   0 ahmad      (501) staff       (20)      392 2023-04-23 17:39:36.000000 flet-material-0.2.0/tests/test_buttons.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.532707 flet-material-0.3.0/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.486137 flet-material-0.3.0/.github/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.490906 flet-material-0.3.0/.github/workflows/
+-rw-r--r--   0 ahmad      (501) staff       (20)      496 2023-04-23 18:54:25.000000 flet-material-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0 ahmad      (501) staff       (20)       37 2023-04-24 09:59:38.000000 flet-material-0.3.0/.gitignore
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.491398 flet-material-0.3.0/.vscode/
+-rw-r--r--   0 ahmad      (501) staff       (20)       64 2023-04-21 12:22:35.000000 flet-material-0.3.0/.vscode/settings.json
+-rw-r--r--   0 ahmad      (501) staff       (20)        0 2023-04-24 11:04:16.000000 flet-material-0.3.0/CHANGELOG.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1079 2023-04-22 18:06:15.000000 flet-material-0.3.0/LICENSE
+-rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-05-08 17:35:11.532453 flet-material-0.3.0/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     3798 2023-04-26 17:39:23.000000 flet-material-0.3.0/README.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.492080 flet-material-0.3.0/command/
+-rw-r--r--   0 ahmad      (501) staff       (20)       42 2023-04-24 15:51:24.000000 flet-material-0.3.0/command/__init__.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      641 2023-04-24 15:57:38.000000 flet-material-0.3.0/command/new_project.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.492723 flet-material-0.3.0/docs/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.493441 flet-material-0.3.0/docs/docs/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1819 2023-04-24 12:26:23.000000 flet-material-0.3.0/docs/docs/contribute.md
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.495972 flet-material-0.3.0/docs/docs/controls/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1975 2023-04-24 12:09:58.000000 flet-material-0.3.0/docs/docs/controls/alerts.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1357 2023-04-24 12:10:06.000000 flet-material-0.3.0/docs/docs/controls/annotations.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3198 2023-04-24 11:12:12.000000 flet-material-0.3.0/docs/docs/controls/badges.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1566 2023-04-23 16:04:13.000000 flet-material-0.3.0/docs/docs/controls/buttons.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1605 2023-04-24 12:10:25.000000 flet-material-0.3.0/docs/docs/controls/checkboxes.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1434 2023-04-24 12:10:31.000000 flet-material-0.3.0/docs/docs/controls/chips.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3025 2023-04-24 14:05:53.000000 flet-material-0.3.0/docs/docs/controls/dropdowns.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     2811 2023-04-23 14:49:45.000000 flet-material-0.3.0/docs/docs/controls/index.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     1296 2023-04-24 12:10:56.000000 flet-material-0.3.0/docs/docs/controls/switches.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3038 2023-04-24 12:28:23.000000 flet-material-0.3.0/docs/docs/index.md
+-rw-r--r--   0 ahmad      (501) staff       (20)     3070 2023-04-24 12:35:43.000000 flet-material-0.3.0/docs/mkdocs.yml
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.497536 flet-material-0.3.0/docs/site/
+-rw-r--r--   0 ahmad      (501) staff       (20)        8 2023-04-24 12:45:17.000000 flet-material-0.3.0/docs/site/.gitignore
+-rw-r--r--   0 ahmad      (501) staff       (20)    28461 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/404.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.487014 flet-material-0.3.0/docs/site/assets/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.497729 flet-material-0.3.0/docs/site/assets/images/
+-rw-r--r--   0 ahmad      (501) staff       (20)     1870 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/images/favicon.png
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.498650 flet-material-0.3.0/docs/site/assets/javascripts/
+-rw-r--r--   0 ahmad      (501) staff       (20)   113367 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   950772 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.502326 flet-material-0.3.0/docs/site/assets/javascripts/lunr/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.511946 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/
+-rw-r--r--   0 ahmad      (501) staff       (20)    17074 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4654 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6119 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6208 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    11499 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     9342 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10669 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     3383 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     9437 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    11232 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2313 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)       36 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     7973 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)      817 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     6026 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4754 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10171 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10958 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    10331 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     3647 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     4523 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2406 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     1031 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    15009 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)      784 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)     2062 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)    22878 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   677455 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/lunr/wordcut.js
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.512853 flet-material-0.3.0/docs/site/assets/javascripts/workers/
+-rw-r--r--   0 ahmad      (501) staff       (20)    38916 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0 ahmad      (501) staff       (20)   209901 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.516201 flet-material-0.3.0/docs/site/assets/stylesheets/
+-rw-r--r--   0 ahmad      (501) staff       (20)   113417 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css
+-rw-r--r--   0 ahmad      (501) staff       (20)    38957 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css.map
+-rw-r--r--   0 ahmad      (501) staff       (20)    12355 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css
+-rw-r--r--   0 ahmad      (501) staff       (20)     3646 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.516430 flet-material-0.3.0/docs/site/contribute/
+-rw-r--r--   0 ahmad      (501) staff       (20)    32427 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/contribute/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.516796 flet-material-0.3.0/docs/site/controls/
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517084 flet-material-0.3.0/docs/site/controls/alerts/
+-rw-r--r--   0 ahmad      (501) staff       (20)    38198 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/alerts/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517369 flet-material-0.3.0/docs/site/controls/annotations/
+-rw-r--r--   0 ahmad      (501) staff       (20)    34841 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/annotations/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517656 flet-material-0.3.0/docs/site/controls/badges/
+-rw-r--r--   0 ahmad      (501) staff       (20)    48809 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/badges/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.517990 flet-material-0.3.0/docs/site/controls/buttons/
+-rw-r--r--   0 ahmad      (501) staff       (20)    37505 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/buttons/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.518524 flet-material-0.3.0/docs/site/controls/checkboxes/
+-rw-r--r--   0 ahmad      (501) staff       (20)    37319 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/checkboxes/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.518941 flet-material-0.3.0/docs/site/controls/chips/
+-rw-r--r--   0 ahmad      (501) staff       (20)    36557 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/chips/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.519292 flet-material-0.3.0/docs/site/controls/dropdowns/
+-rw-r--r--   0 ahmad      (501) staff       (20)    46453 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/dropdowns/index.html
+-rw-r--r--   0 ahmad      (501) staff       (20)    32736 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.519642 flet-material-0.3.0/docs/site/controls/switches/
+-rw-r--r--   0 ahmad      (501) staff       (20)    36069 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/controls/switches/index.html
+-rw-r--r--   0 ahmad      (501) staff       (20)    38036 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/index.html
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.520087 flet-material-0.3.0/docs/site/search/
+-rw-r--r--   0 ahmad      (501) staff       (20)    21580 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/search/search_index.json
+-rw-r--r--   0 ahmad      (501) staff       (20)     1484 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/sitemap.xml
+-rw-r--r--   0 ahmad      (501) staff       (20)      204 2023-04-24 14:06:21.000000 flet-material-0.3.0/docs/site/sitemap.xml.gz
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.523089 flet-material-0.3.0/flet_material/
+-rw-r--r--   0 ahmad      (501) staff       (20)      421 2023-04-23 11:09:44.000000 flet-material-0.3.0/flet_material/__init__.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.527329 flet-material-0.3.0/flet_material/__pycache__/
+-rw-r--r--   0 ahmad      (501) staff       (20)      706 2023-04-23 11:09:44.000000 flet-material-0.3.0/flet_material/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     4049 2023-04-24 11:44:19.000000 flet-material-0.3.0/flet_material/__pycache__/admonition.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1892 2023-04-22 18:01:00.000000 flet-material-0.3.0/flet_material/__pycache__/alert.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1697 2023-04-21 17:58:50.000000 flet-material-0.3.0/flet_material/__pycache__/annotation.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1834 2023-04-21 16:25:55.000000 flet-material-0.3.0/flet_material/__pycache__/annotations.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     3211 2023-04-23 15:51:31.000000 flet-material-0.3.0/flet_material/__pycache__/badge.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      738 2023-04-23 14:56:58.000000 flet-material-0.3.0/flet_material/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1597 2023-04-23 18:10:10.000000 flet-material-0.3.0/flet_material/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1525 2023-04-23 11:36:01.000000 flet-material-0.3.0/flet_material/__pycache__/checkbox.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-24 11:30:35.000000 flet-material-0.3.0/flet_material/__pycache__/chip.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1698 2023-04-22 14:16:22.000000 flet-material-0.3.0/flet_material/__pycache__/switch.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     6919 2023-04-24 11:44:19.000000 flet-material-0.3.0/flet_material/admonition.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     2689 2023-04-22 18:01:00.000000 flet-material-0.3.0/flet_material/alert.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1503 2023-04-21 17:58:49.000000 flet-material-0.3.0/flet_material/annotation.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     4731 2023-04-23 15:51:31.000000 flet-material-0.3.0/flet_material/badge.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      358 2023-04-23 14:56:57.000000 flet-material-0.3.0/flet_material/base.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1425 2023-04-23 18:09:54.000000 flet-material-0.3.0/flet_material/button.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1125 2023-05-08 17:33:58.000000 flet-material-0.3.0/flet_material/checkbox.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1528 2023-04-24 11:30:35.000000 flet-material-0.3.0/flet_material/chip.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1399 2023-04-22 14:16:22.000000 flet-material-0.3.0/flet_material/switch.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.524150 flet-material-0.3.0/flet_material.egg-info/
+-rw-r--r--   0 ahmad      (501) staff       (20)      465 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/PKG-INFO
+-rw-r--r--   0 ahmad      (501) staff       (20)     4509 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)        1 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       83 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/entry_points.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       25 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/requires.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       21 2023-05-08 17:35:11.000000 flet-material-0.3.0/flet_material.egg-info/top_level.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       24 2023-04-22 18:53:13.000000 flet-material-0.3.0/requirements.txt
+-rw-r--r--   0 ahmad      (501) staff       (20)       38 2023-05-08 17:35:11.532749 flet-material-0.3.0/setup.cfg
+-rw-r--r--   0 ahmad      (501) staff       (20)      805 2023-05-08 17:34:47.000000 flet-material-0.3.0/setup.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.529135 flet-material-0.3.0/styles/
+-rw-r--r--   0 ahmad      (501) staff       (20)      271 2023-04-22 17:17:29.000000 flet-material-0.3.0/styles/__init__.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.531184 flet-material-0.3.0/styles/__pycache__/
+-rw-r--r--   0 ahmad      (501) staff       (20)      499 2023-04-22 17:17:29.000000 flet-material-0.3.0/styles/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      708 2023-04-23 11:20:49.000000 flet-material-0.3.0/styles/__pycache__/admonition_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      493 2023-04-22 17:30:06.000000 flet-material-0.3.0/styles/__pycache__/alert_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      494 2023-04-22 17:08:25.000000 flet-material-0.3.0/styles/__pycache__/alert_styles.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      487 2023-04-22 16:10:03.000000 flet-material-0.3.0/styles/__pycache__/badge_style.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      287 2023-04-21 16:08:17.000000 flet-material-0.3.0/styles/__pycache__/fonts.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)     1040 2023-04-23 14:54:06.000000 flet-material-0.3.0/styles/__pycache__/theme.cpython-310.pyc
+-rw-r--r--   0 ahmad      (501) staff       (20)      908 2023-04-23 11:20:48.000000 flet-material-0.3.0/styles/admonition_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      378 2023-04-22 17:30:06.000000 flet-material-0.3.0/styles/alert_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      361 2023-04-22 16:10:02.000000 flet-material-0.3.0/styles/badge_style.py
+-rw-r--r--   0 ahmad      (501) staff       (20)       90 2023-04-21 16:07:16.000000 flet-material-0.3.0/styles/fonts.py
+-rw-r--r--   0 ahmad      (501) staff       (20)     1421 2023-04-23 14:18:26.000000 flet-material-0.3.0/styles/theme.py
+drwxr-xr-x   0 ahmad      (501) staff       (20)        0 2023-05-08 17:35:11.532066 flet-material-0.3.0/tests/
+-rw-r--r--   0 ahmad      (501) staff       (20)      514 2023-04-23 19:11:47.000000 flet-material-0.3.0/tests/test_admonitions.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      392 2023-04-23 17:39:36.000000 flet-material-0.3.0/tests/test_buttons.py
+-rw-r--r--   0 ahmad      (501) staff       (20)      662 2023-04-26 17:52:03.000000 flet-material-0.3.0/tests/test_switch.py
```

### Comparing `flet-material-0.2.0/LICENSE` & `flet-material-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/README.md` & `flet-material-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <div align="center">
    <a href="[https://squidfunk.github.io/mkdocs-material/](https://flet.dev/)">
    <img src="https://github.com/flet-dev/flet/blob/main/media/logo/Icon-512.png" width="180" height="180" alt="Flet Material Library">
   </a>
 
-**A UI library for Flet framework**
+**A UI library for Flet**
 
  
  </div>
 
 <br>
 <br>
 <p align="center">
@@ -35,40 +35,36 @@
     src="https://img.shields.io/badge/docs-available-brightgreen.svg"
     alt="Docs"
   /></a>
 
   </p>
 
 <p align="center">
-Modernize your websites and applications by implementing customized Flet controls that improve user experince and overall visual quality. UI components are flexible and in line with current design trends. 
-
+Modernize your websites and applications by implementing customized Flet controls that improve user experience and overall visual quality. The UI components are flexible and aligned with current design trends.
 </p>
 
 
 
 ## 1. Installation
 
-Flet Material requires the following:
-
+To use Flet Material, you need to have the following installed:
 
 -   Latest version of Flet
 -   Python 3.5+
 
-If you don't have Flet isntalled, installing Flet Material automatically installs it for you.
+If you don't have Flet installed, installing Flet Material automatically installs it for you. You can install Flet Material using the following command:
 ```
 $ pip install flet-material
 ```
 
 
 
 ## 2. Application Setup
 
-Once you have Flet Material on your system, you can try and run the following code snippet to make sure eveything is working properly:
-
-If you don't have Flet isntalled, installing Flet Material automatically installs it for you.
+After installing Flet Material, you can test if it's working properly by running the following code snippet:
 
 ```python
 import flet as ft
 import flet_material as fm
 
 fm.Theme.set_theme(theme="teal")
 
@@ -89,44 +85,44 @@
    page.update()
 
 
 if __name__ == "__main__":
    ft.flet.app(target=main)
 ```
 
-If the package was installed correctly you should see a centered and customized button. 
+If the package was installed correctly, you should see a centered and customized button.
 
 ## 3. Code Breakdown
 
-The script may seem familier because it's very much like the basic Flet application setup. In fact it's the very same with some minor additions.
+The script is similar to the basic Flet application setup, with some minor additions.
 
-First, note the import statement at the top of the main file. This is the main library and all its components.
+At the top of the main file, you need to import the Flet Material library and all its components:
 ```python
 import flet_material as fm
 ```
 
-Below the imported modules is the ```Theme``` instance from ```flet_material```. This sets up the entire application theme so that all colors, primary and accent, are uniform and the same, giving the applications being built much appeal.
+Below the imported modules is the Theme instance from Flet Material. It sets up the entire application theme so that all colors, primary and accent, are uniform, giving the applications being built a consistent look and feel. For a list of supported theme colors, you can visit the library's documentation online.
 
 For a list of supported theme colors, you can visit the library's documentation online.
 
 ```python
 fm.Theme.set_theme(theme="teal")
 ```
 
-Finally, wihtin the ```main()``` method we have a new control called ```fm.Buttons()```, which simply inherits it's properties from several Flet classes and is customized.
+Finally, within the main() method, you can use a new control called fm.Buttons(), which inherits its properties from several Flet classes and can be customized to your liking:
 
 ```python
 button = fm.Buttons(
     width=220,
     height=55,
     title="Give this repo a star!",
 )
 ```
 
-That's it! You now have access to Flet Material library components!!
+That's it! You now have access to Flet Material library components!
 
 ## Contributing
 
 Contributions are highly encouraged and welcomed. Check out the [contributon section](https://flet-material.vercel.app/contribute/) of the documentation for more details. 
 
 
 ## License
```

### Comparing `flet-material-0.2.0/command/new_project.py` & `flet-material-0.3.0/command/new_project.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
 def main(page:ft.Page):
     page.bgcolor = fm.Theme.bgcolor
     page.update()
 
 if __name__ == "__main__":
     ft.flet.app(target=main)
-
-if __name__ == '__main__':
-    app.run()"""
+"""
 
     with open(f"{project_name}/main.py", "w") as f:
         f.write(template_code)
 
     click.echo(f"Created {project_name}/main.py")
```

### Comparing `flet-material-0.2.0/docs/docs/contribute.md` & `flet-material-0.3.0/docs/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/alerts.md` & `flet-material-0.3.0/docs/docs/controls/alerts.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/annotations.md` & `flet-material-0.3.0/docs/docs/controls/annotations.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/badges.md` & `flet-material-0.3.0/docs/docs/controls/badges.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/buttons.md` & `flet-material-0.3.0/docs/docs/controls/buttons.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/checkboxes.md` & `flet-material-0.3.0/docs/docs/controls/checkboxes.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/chips.md` & `flet-material-0.3.0/docs/docs/controls/chips.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/dropdowns.md` & `flet-material-0.3.0/docs/docs/controls/dropdowns.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Alerts
+# Dropdown
 
 Dropdowns are used to allow users to select one option from a list of choices. They are commonly used in menus and settings to provide a compact way to present a large number of options. Dropdowns can be designed in various styles, such as with a simple list or with additional information, such as icons or descriptions.
 
 
 The ***dropdown*** class is straightforward and easy to use. Choose where you want to place your annotation then create an instance of it, like this:
```

### Comparing `flet-material-0.2.0/docs/docs/controls/index.md` & `flet-material-0.3.0/docs/docs/controls/index.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/controls/switches.md` & `flet-material-0.3.0/docs/docs/controls/switches.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/docs/index.md` & `flet-material-0.3.0/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/mkdocs.yml` & `flet-material-0.3.0/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/404.html` & `flet-material-0.3.0/docs/site/404.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/images/favicon.png` & `flet-material-0.3.0/docs/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/bundle.51198bba.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/bundle.51198bba.min.js.map` & `flet-material-0.3.0/docs/site/assets/javascripts/bundle.51198bba.min.js.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.da.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.de.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.du.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.es.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.it.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.no.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.th.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/tinyseg.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/lunr/wordcut.js` & `flet-material-0.3.0/docs/site/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/workers/search.208ed371.min.js` & `flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/javascripts/workers/search.208ed371.min.js.map` & `flet-material-0.3.0/docs/site/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/stylesheets/main.ded33207.min.css` & `flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/stylesheets/main.ded33207.min.css.map` & `flet-material-0.3.0/docs/site/assets/stylesheets/main.ded33207.min.css.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css` & `flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map` & `flet-material-0.3.0/docs/site/assets/stylesheets/palette.a0c5b2b5.min.css.map`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/contribute/index.html` & `flet-material-0.3.0/docs/site/contribute/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/alerts/index.html` & `flet-material-0.3.0/docs/site/controls/alerts/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/annotations/index.html` & `flet-material-0.3.0/docs/site/controls/annotations/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/badges/index.html` & `flet-material-0.3.0/docs/site/controls/badges/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/buttons/index.html` & `flet-material-0.3.0/docs/site/controls/buttons/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/checkboxes/index.html` & `flet-material-0.3.0/docs/site/controls/checkboxes/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/chips/index.html` & `flet-material-0.3.0/docs/site/controls/chips/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/dropdowns/index.html` & `flet-material-0.3.0/docs/site/controls/dropdowns/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#alerts" class="md-skip">
+        <a href="#dropdown" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
@@ -563,15 +563,15 @@
                 
                   
 
   
   
 
 
-<h1 id="alerts">Alerts</h1>
+<h1 id="dropdown">Dropdown</h1>
 <p>Dropdowns are used to allow users to select one option from a list of choices. They are commonly used in menus and settings to provide a compact way to present a large number of options. Dropdowns can be designed in various styles, such as with a simple list or with additional information, such as icons or descriptions.</p>
 <p>The <strong><em>dropdown</em></strong> class is straightforward and easy to use. Choose where you want to place your annotation then create an instance of it, like this:</p>
 <p><span style="font-size:1rem;">Basic Dropdown Example</span></p>
 <div class="admonition tip">
 <p class="admonition-title">Flet Material Alerts</p>
 <p>The Flet Material Library classes inherit from the controls provided by Flet. In this case, the <code>fm.Admonitions()</code> class inherits from Flet's <code>ft.Container()</code> class, this means all properties of the latter are accessable through the former. </p>
 </div>
```

#### html2text {}

```diff
@@ -35,15 +35,15 @@
           o Checkboxes
           o Chips
           o ⁰  Dropdowns   Dropdowns    Table of contents
                 # Expandable_Dropdown
                 # Fixed_Dropdown_(Title_only)
           o Switches
     * Contribute
-****** Alerts ******
+****** Dropdown ******
 Dropdowns are used to allow users to select one option from a list of choices.
 They are commonly used in menus and settings to provide a compact way to
 present a large number of options. Dropdowns can be designed in various styles,
 such as with a simple list or with additional information, such as icons or
 descriptions.
 The dropdown class is straightforward and easy to use. Choose where you want to
 place your annotation then create an instance of it, like this:
```

### Comparing `flet-material-0.2.0/docs/site/controls/index.html` & `flet-material-0.3.0/docs/site/controls/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/controls/switches/index.html` & `flet-material-0.3.0/docs/site/controls/switches/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/index.html` & `flet-material-0.3.0/docs/site/index.html`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/docs/site/search/search_index.json` & `flet-material-0.3.0/docs/site/search/search_index.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983333333333333%*

 * *Differences: {"'docs'": "{21: {'title': 'Dropdown'}}"}*

```diff
@@ -113,15 +113,15 @@
             "location": "controls/chips/",
             "text": "<p>Chips are small UI elements used to display small amounts of information in a compact way. They can be used to show user information, such as a profile picture or name, or to display tags or categories. Chips can be designed in various shapes and sizes, and can be used to represent different types of data.</p> <p>The chips class is straightforward and easy to use. Choose where you want to place your annotation then create an instance of it, like this:</p> <p>Basic Chips Example</p> <p>Flet Material Chips</p> <p>The Flet Material Library classes inherit from the controls provided by Flet. In this case, the <code>fm.FilterChip()</code> class inherits from Flet's <code>ft.Container()</code> class, this means all properties of the latter are accessable through the former. </p> Chipsparameters <pre><code>import flet as ft\nimport flet_material as fm\nfm.Theme.set_theme(theme=\"blue\")\ndef main(page: ft.Page):\npage.bgcolor = fm.Theme.bgcolor\npage.horizontal_alignment = \"center\"\npage.vertical_alignment = \"center\"\nchip = fm.FilterChip(title=\"Hello World!\", chip_width=123)\npage.add(chip)\npage.update()\nif __name__ == \"__main__\":\nft.flet.app(target=main)\n</code></pre> <p>title: str - The title to be displayed. </p> <p>width: int - Set the width to accomodate both controls. </p>",
             "title": "Chips"
         },
         {
             "location": "controls/dropdowns/",
             "text": "<p>Dropdowns are used to allow users to select one option from a list of choices. They are commonly used in menus and settings to provide a compact way to present a large number of options. Dropdowns can be designed in various styles, such as with a simple list or with additional information, such as icons or descriptions.</p> <p>The dropdown class is straightforward and easy to use. Choose where you want to place your annotation then create an instance of it, like this:</p> <p>Basic Dropdown Example</p> <p>Flet Material Alerts</p> <p>The Flet Material Library classes inherit from the controls provided by Flet. In this case, the <code>fm.Admonitions()</code> class inherits from Flet's <code>ft.Container()</code> class, this means all properties of the latter are accessable through the former. </p>",
-            "title": "Alerts"
+            "title": "Dropdown"
         },
         {
             "location": "controls/dropdowns/#expandable-dropdown",
             "text": "Expandable Dropdownparameters <pre><code>import flet as ft\nimport flet_material as fm\nfm.Theme.set_theme(theme=\"blue\")\ndef main(page: ft.Page):\npage.bgcolor = fm.Theme.bgcolor\npage.horizontal_alignment = \"center\"\npage.vertical_alignment = \"center\"\ndrop = fm.Admonitions(\ntype_=\"note\", expanded_height=300, expanded=False, controls_list=None\n)\npage.add(drop)\npage.update()\nif __name__ == \"__main__\":\nft.flet.app(target=main)\n</code></pre> <p>type_: str - The type of title to be displayed. The following parameters are supported:</p> <pre><code>- \"note\", \"abstract\", \"info\", \"tip\", \"success\", \"warning\", \"danger\"\n</code></pre> <p>expanded_height: int - Sets the height when the dropdown is clicked.</p> <p>expanded: bool - If placed outside a ft.Row() or ft.Column(), should be set to False, otherwise set to True. </p> <p>controls_list: list - The list of controls that can be added inside the dropdown. </p>",
             "title": "Expandable Dropdown"
         },
         {
```

### Comparing `flet-material-0.2.0/docs/site/sitemap.xml` & `flet-material-0.3.0/docs/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/__init__.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/admonition.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/admonition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/alert.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/alert.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/annotation.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/annotation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/annotations.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/annotations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/badge.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/badge.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/base.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/button.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/checkbox.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/checkbox.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/chip.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/chip.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/__pycache__/switch.cpython-310.pyc` & `flet-material-0.3.0/flet_material/__pycache__/switch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/admonition.py` & `flet-material-0.3.0/flet_material/admonition.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/alert.py` & `flet-material-0.3.0/flet_material/alert.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/annotation.py` & `flet-material-0.3.0/flet_material/annotation.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/badge.py` & `flet-material-0.3.0/flet_material/badge.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/button.py` & `flet-material-0.3.0/flet_material/button.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/checkbox.py` & `flet-material-0.3.0/flet_material/checkbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import flet as ft
 from flet_material.base import Theme
 import time
 
 
 class CheckBox(ft.Container, Theme):
-    def __init__(self, shape: str, *args, **kwargs):
+    def __init__(self, shape: str, value: bool, disabled: bool, *args, **kwargs):
         self.checkbox: ft.Control = ft.Checkbox(
             fill_color=Theme.primary_theme,
             check_color="white",
             scale=ft.Scale(0.95),
+            value=value,
+            disabled=disabled,
             on_change=lambda e: self.animate_checkbox(e),
         )
 
         kwargs.setdefault("width", 25)
         kwargs.setdefault("height", 25)
         kwargs.setdefault("shape", ft.BoxShape(shape))
         kwargs.setdefault("bgcolor", Theme.primary_theme)
         kwargs.setdefault("content", self.checkbox)
-        kwargs.setdefault("scale", 0.9)
+        kwargs.setdefault("scale", 0.8)
         kwargs.setdefault("animate_scale", ft.Animation(500, "bounceOut"))
         kwargs.setdefault("on_click", lambda e: self.animate_checkbox(e))
 
         super().__init__(*args, **kwargs)
 
     def animate_checkbox(self, e):
-        self.scale = ft.Scale(0.85)
+        self.scale = ft.Scale(0.65)
         self.update()
         time.sleep(0.15)
-        self.scale = ft.Scale(1)
+        self.scale = ft.Scale(0.8)
         self.update()
```

### Comparing `flet-material-0.2.0/flet_material/chip.py` & `flet-material-0.3.0/flet_material/chip.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material/switch.py` & `flet-material-0.3.0/flet_material/switch.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/flet_material.egg-info/SOURCES.txt` & `flet-material-0.3.0/flet_material.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -110,8 +110,9 @@
 styles/__pycache__/admonition_style.cpython-310.pyc
 styles/__pycache__/alert_style.cpython-310.pyc
 styles/__pycache__/alert_styles.cpython-310.pyc
 styles/__pycache__/badge_style.cpython-310.pyc
 styles/__pycache__/fonts.cpython-310.pyc
 styles/__pycache__/theme.cpython-310.pyc
 tests/test_admonitions.py
-tests/test_buttons.py
+tests/test_buttons.py
+tests/test_switch.py
```

### Comparing `flet-material-0.2.0/setup.py` & `flet-material-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="flet-material",
-    version="0.2.0",
+    version="0.3.0",
     author="S. Ahmad P. Hakimi",
     author_email="pourhakimi@pm.me",
     description="Material UI Library for Flet",
     long_description="",
     long_description_content_type="text/markdown",
     url="https://github.com/LineIndent/material_design_flet",
     packages=["flet_material", "styles"],
```

### Comparing `flet-material-0.2.0/styles/__pycache__/admonition_style.cpython-310.pyc` & `flet-material-0.3.0/styles/__pycache__/admonition_style.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/styles/__pycache__/theme.cpython-310.pyc` & `flet-material-0.3.0/styles/__pycache__/theme.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/styles/admonition_style.py` & `flet-material-0.3.0/styles/admonition_style.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/styles/theme.py` & `flet-material-0.3.0/styles/theme.py`

 * *Files identical despite different names*

### Comparing `flet-material-0.2.0/tests/test_admonitions.py` & `flet-material-0.3.0/tests/test_admonitions.py`

 * *Files identical despite different names*

