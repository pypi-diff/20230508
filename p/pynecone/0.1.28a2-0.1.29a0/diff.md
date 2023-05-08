# Comparing `tmp/pynecone-0.1.28a2.tar.gz` & `tmp/pynecone-0.1.29a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.28a2.tar", max compression
+gzip compressed data, was "pynecone-0.1.29a0.tar", max compression
```

## Comparing `pynecone-0.1.28a2.tar` & `pynecone-0.1.29a0.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.28a2/LICENSE
--rw-r--r--   0        0        0     7887 2023-04-27 23:08:51.375669 pynecone-0.1.28a2/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.28a2/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-04-27 02:06:35.747526 pynecone-0.1.28a2/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.28a2/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.28a2/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.28a2/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.28a2/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   248832 2023-04-28 22:48:11.602895 pynecone-0.1.28a2/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.28a2/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0     1017 2023-04-28 22:48:11.603117 pynecone-0.1.28a2/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.28a2/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.28a2/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.28a2/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     6809 2023-05-02 03:38:26.994341 pynecone-0.1.28a2/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0      823 2023-04-30 03:30:20.667423 pynecone-0.1.28a2/pynecone/__init__.py
--rw-r--r--   0        0        0    19779 2023-05-02 04:24:21.320783 pynecone-0.1.28a2/pynecone/app.py
--rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.28a2/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.28a2/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     5856 2023-04-29 22:32:13.534526 pynecone-0.1.28a2/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     5590 2023-04-27 23:08:51.378717 pynecone-0.1.28a2/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     9084 2023-04-24 22:10:28.096707 pynecone-0.1.28a2/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6371 2023-05-02 03:38:26.995205 pynecone-0.1.28a2/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.28a2/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      726 2023-04-27 21:37:27.235866 pynecone-0.1.28a2/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.28a2/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.28a2/pynecone/components/base/document.py
--rw-r--r--   0        0        0      242 2022-11-18 20:43:33.735533 pynecone-0.1.28a2/pynecone/components/base/head.py
--rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.28a2/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.28a2/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    21824 2023-05-02 03:38:26.995788 pynecone-0.1.28a2/pynecone/components/component.py
--rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.28a2/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.28a2/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2486 2023-03-16 23:52:12.744773 pynecone-0.1.28a2/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4161 2023-04-27 23:08:51.379280 pynecone-0.1.28a2/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.28a2/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.28a2/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.28a2/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.28a2/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.28a2/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.28a2/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.28a2/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.28a2/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.28a2/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.28a2/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.28a2/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.28a2/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.28a2/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.28a2/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.28a2/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1103 2023-05-02 03:38:26.996194 pynecone-0.1.28a2/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1717 2023-05-02 03:37:37.426206 pynecone-0.1.28a2/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2469 2023-04-27 23:08:51.379545 pynecone-0.1.28a2/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.28a2/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.28a2/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2323 2023-05-02 03:38:26.996626 pynecone-0.1.28a2/pynecone/components/forms/formcontrol.py
--rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.28a2/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3068 2023-04-30 03:30:20.667778 pynecone-0.1.28a2/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3916 2023-03-10 00:25:42.698330 pynecone-0.1.28a2/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.28a2/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.28a2/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3004 2023-03-16 23:52:12.745021 pynecone-0.1.28a2/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.28a2/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3475 2023-03-16 23:52:12.745104 pynecone-0.1.28a2/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     2782 2023-03-10 00:25:42.699714 pynecone-0.1.28a2/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.28a2/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1550 2023-03-10 00:25:42.700204 pynecone-0.1.28a2/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2907 2023-04-27 23:08:51.379851 pynecone-0.1.28a2/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.28a2/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-27 02:06:35.753790 pynecone-0.1.28a2/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17359 2023-04-27 02:06:35.754541 pynecone-0.1.28a2/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.28a2/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.28a2/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.28a2/pynecone/components/layout/box.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.28a2/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.28a2/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.28a2/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.28a2/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.28a2/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.28a2/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.28a2/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.28a2/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.28a2/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.28a2/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.28a2/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.28a2/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.28a2/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.28a2/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.28a2/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.28a2/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.28a2/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.28a2/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.28a2/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.28a2/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1005 2023-04-28 22:48:11.604564 pynecone-0.1.28a2/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.28a2/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      483 2022-12-07 23:08:48.795126 pynecone-0.1.28a2/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.28a2/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.28a2/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.28a2/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.28a2/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.28a2/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.28a2/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.28a2/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.28a2/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.28a2/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.28a2/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     6463 2023-05-02 03:38:26.996965 pynecone-0.1.28a2/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.28a2/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.28a2/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.28a2/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.28a2/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     2973 2023-04-27 02:06:35.755989 pynecone-0.1.28a2/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.28a2/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.28a2/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.28a2/pynecone/config.py
--rw-r--r--   0        0        0     8765 2023-04-27 23:08:51.380182 pynecone-0.1.28a2/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.28a2/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.28a2/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.28a2/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.28a2/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.28a2/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1289 2023-04-27 02:06:35.759113 pynecone-0.1.28a2/pynecone/el/element.py
--rw-r--r--   0        0        0   108515 2023-04-27 02:06:35.759585 pynecone-0.1.28a2/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2666 2023-04-27 02:06:35.759864 pynecone-0.1.28a2/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10217 2023-05-02 04:23:25.151320 pynecone-0.1.28a2/pynecone/event.py
--rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.28a2/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     3259 2023-04-27 23:08:51.380497 pynecone-0.1.28a2/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1022 2023-04-27 02:06:35.761080 pynecone-0.1.28a2/pynecone/middleware/logging_middleware.py
--rw-r--r--   0        0        0     1193 2023-04-27 02:06:35.761405 pynecone-0.1.28a2/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.28a2/pynecone/model.py
--rw-r--r--   0        0        0     8093 2023-04-27 02:06:35.762135 pynecone-0.1.28a2/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.28a2/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.28a2/pynecone/route.py
--rw-r--r--   0        0        0    27024 2023-05-02 04:23:29.094934 pynecone-0.1.28a2/pynecone/state.py
--rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.28a2/pynecone/style.py
--rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.28a2/pynecone/telemetry.py
--rw-r--r--   0        0        0     4252 2023-04-27 23:08:51.381036 pynecone-0.1.28a2/pynecone/utils/build.py
--rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.28a2/pynecone/utils/console.py
--rw-r--r--   0        0        0     3597 2023-04-27 23:08:51.381176 pynecone-0.1.28a2/pynecone/utils/exec.py
--rw-r--r--   0        0        0    10780 2023-05-02 03:38:31.006798 pynecone-0.1.28a2/pynecone/utils/format.py
--rw-r--r--   0        0        0      544 2023-03-16 23:52:12.757094 pynecone-0.1.28a2/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.28a2/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0     9121 2023-04-27 23:08:51.381523 pynecone-0.1.28a2/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.28a2/pynecone/utils/processes.py
--rw-r--r--   0        0        0     4299 2023-03-16 23:52:12.757408 pynecone-0.1.28a2/pynecone/utils/types.py
--rw-r--r--   0        0        0    26099 2023-05-02 00:04:31.434609 pynecone-0.1.28a2/pynecone/var.py
--rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.28a2/pynecone/watch.py
--rw-r--r--   0        0        0     1758 2023-05-02 04:24:30.637791 pynecone-0.1.28a2/pyproject.toml
--rw-r--r--   0        0        0     9379 1970-01-01 00:00:00.000000 pynecone-0.1.28a2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.29a0/LICENSE
+-rw-r--r--   0        0        0     7887 2023-04-27 23:08:51.375669 pynecone-0.1.29a0/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.29a0/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-04-27 02:06:35.747526 pynecone-0.1.29a0/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.29a0/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.29a0/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.29a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.29a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   248832 2023-04-28 22:48:11.602895 pynecone-0.1.29a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.29a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1017 2023-04-28 22:48:11.603117 pynecone-0.1.29a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.29a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.29a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.29a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     6809 2023-05-08 01:08:23.211689 pynecone-0.1.29a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0      823 2023-05-04 17:13:55.078914 pynecone-0.1.29a0/pynecone/__init__.py
+-rw-r--r--   0        0        0    19916 2023-05-08 20:37:22.019202 pynecone-0.1.29a0/pynecone/app.py
+-rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.29a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.29a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6132 2023-05-06 20:59:13.474169 pynecone-0.1.29a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     5590 2023-04-27 23:08:51.378717 pynecone-0.1.29a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     9101 2023-05-06 20:59:13.474329 pynecone-0.1.29a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     6371 2023-05-06 19:53:35.862302 pynecone-0.1.29a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.29a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      726 2023-04-27 21:37:27.235866 pynecone-0.1.29a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.29a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.29a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-05-06 20:59:13.474461 pynecone-0.1.29a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.29a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.29a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    21974 2023-05-06 20:59:13.474653 pynecone-0.1.29a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.29a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.29a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2535 2023-05-06 20:59:13.475051 pynecone-0.1.29a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4032 2023-05-06 20:59:13.475185 pynecone-0.1.29a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.29a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.29a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.29a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.29a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.29a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.29a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.29a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.29a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.29a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.29a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.29a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.29a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.29a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.29a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.29a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1103 2023-05-06 19:53:35.863124 pynecone-0.1.29a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1717 2023-05-02 03:37:37.426206 pynecone-0.1.29a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2469 2023-04-27 23:08:51.379545 pynecone-0.1.29a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.29a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.29a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0     2323 2023-05-06 19:53:35.863529 pynecone-0.1.29a0/pynecone/components/forms/formcontrol.py
+-rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.29a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3090 2023-05-06 20:59:13.475345 pynecone-0.1.29a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0     3912 2023-05-06 20:59:13.475496 pynecone-0.1.29a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.29a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.29a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3058 2023-05-08 03:51:56.284163 pynecone-0.1.29a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.29a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3471 2023-05-06 20:59:13.475639 pynecone-0.1.29a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     2778 2023-05-06 20:59:13.475767 pynecone-0.1.29a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.29a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1546 2023-05-06 20:59:13.475886 pynecone-0.1.29a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2930 2023-05-06 20:59:13.476022 pynecone-0.1.29a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.29a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-27 02:06:35.753790 pynecone-0.1.29a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17359 2023-04-27 02:06:35.754541 pynecone-0.1.29a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.29a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.29a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.29a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.29a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.29a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.29a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.29a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.29a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.29a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.29a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-04-27 02:06:35.755389 pynecone-0.1.29a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.29a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.29a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.29a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.29a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.29a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.29a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.29a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.29a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.29a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.29a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.29a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.29a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1005 2023-04-28 22:48:11.604564 pynecone-0.1.29a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.29a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      506 2023-05-06 20:59:13.476372 pynecone-0.1.29a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.29a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.29a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.29a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.29a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.29a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.29a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.29a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.29a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.29a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.29a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     6463 2023-05-06 19:53:35.864116 pynecone-0.1.29a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.29a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.29a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.29a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.29a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3287 2023-05-06 20:59:13.476517 pynecone-0.1.29a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.29a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.29a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     5296 2023-04-27 02:06:35.756502 pynecone-0.1.29a0/pynecone/config.py
+-rw-r--r--   0        0        0     8847 2023-05-08 20:37:22.019401 pynecone-0.1.29a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.29a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.29a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.29a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.29a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.29a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1289 2023-04-27 02:06:35.759113 pynecone-0.1.29a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108517 2023-05-06 20:59:13.476953 pynecone-0.1.29a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2666 2023-04-27 02:06:35.759864 pynecone-0.1.29a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    10030 2023-05-08 20:37:22.019708 pynecone-0.1.29a0/pynecone/event.py
+-rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.29a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1601 2023-05-08 20:37:22.020068 pynecone-0.1.29a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1052 2023-05-08 20:37:22.020367 pynecone-0.1.29a0/pynecone/middleware/logging_middleware.py
+-rw-r--r--   0        0        0     1167 2023-05-08 20:37:22.020507 pynecone-0.1.29a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2085 2023-04-27 23:08:51.380631 pynecone-0.1.29a0/pynecone/model.py
+-rw-r--r--   0        0        0     8093 2023-05-06 19:53:33.712419 pynecone-0.1.29a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.29a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.29a0/pynecone/route.py
+-rw-r--r--   0        0        0    26926 2023-05-08 03:51:56.284895 pynecone-0.1.29a0/pynecone/state.py
+-rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.29a0/pynecone/style.py
+-rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.29a0/pynecone/telemetry.py
+-rw-r--r--   0        0        0     4252 2023-04-27 23:08:51.381036 pynecone-0.1.29a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.29a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     3597 2023-04-27 23:08:51.381176 pynecone-0.1.29a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    10844 2023-05-08 20:37:22.020758 pynecone-0.1.29a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      586 2023-05-06 20:59:13.477652 pynecone-0.1.29a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.29a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0     9247 2023-05-07 04:39:58.171126 pynecone-0.1.29a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.29a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     4389 2023-05-07 04:39:58.171321 pynecone-0.1.29a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0    30631 2023-05-07 04:39:58.171540 pynecone-0.1.29a0/pynecone/var.py
+-rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.29a0/pynecone/watch.py
+-rw-r--r--   0        0        0     1758 2023-05-08 20:40:11.847947 pynecone-0.1.29a0/pyproject.toml
+-rw-r--r--   0        0        0     9379 1970-01-01 00:00:00.000000 pynecone-0.1.29a0/PKG-INFO
```

### Comparing `pynecone-0.1.28a2/LICENSE` & `pynecone-0.1.29a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/README.md` & `pynecone-0.1.29a0/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.29a0/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.29a0/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.29a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.29a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/web/package.json` & `pynecone-0.1.29a0/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.29a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.29a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.29a0/pynecone/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/__init__.py` & `pynecone-0.1.29a0/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/app.py` & `pynecone-0.1.29a0/pynecone/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pynecone.route import (
     DECORATED_ROUTES,
     catchall_in_route,
     catchall_prefix,
     get_route_args,
     verify_route_validity,
 )
-from pynecone.state import DefaultState, Delta, State, StateManager, StateUpdate
+from pynecone.state import DefaultState, State, StateManager, StateUpdate
 from pynecone.utils import format, types
 
 # Define custom types.
 ComponentCallable = Callable[[], Component]
 Reducer = Callable[[Event], Coroutine[Any, Any, StateUpdate]]
 
 
@@ -58,16 +58,16 @@
 
     # The styling to apply to each component.
     style: ComponentStyle = {}
 
     # Middleware to add to the app.
     middleware: List[Middleware] = []
 
-    # Event handlers to trigger when a page loads.
-    load_events: Dict[str, Union[EventHandler, List[EventHandler]]] = {}
+    # List of event handlers to trigger when a page loads.
+    load_events: Dict[str, List[EventHandler]] = {}
 
     def __init__(self, *args, **kwargs):
         """Initialize the app.
 
         Args:
             *args: Args to initialize the app with.
             **kwargs: Kwargs to initialize the app with.
@@ -145,24 +145,22 @@
             cors.CORSMiddleware,
             allow_credentials=True,
             allow_methods=["*"],
             allow_headers=["*"],
             allow_origins=["*"],
         )
 
-    async def preprocess(
-        self, state: State, event: Event
-    ) -> Optional[Union[StateUpdate, List[StateUpdate]]]:
+    async def preprocess(self, state: State, event: Event) -> Optional[StateUpdate]:
         """Preprocess the event.
 
         This is where middleware can modify the event before it is processed.
         Each middleware is called in the order it was added to the app.
 
-        If a middleware returns a delta, the event is not processed and the
-        delta is returned.
+        If a middleware returns an update, the event is not processed and the
+        update is returned.
 
         Args:
             state: The state to preprocess.
             event: The event to preprocess.
 
         Returns:
             An optional state to return.
@@ -172,43 +170,41 @@
                 out = await middleware.preprocess(app=self, state=state, event=event)
             else:
                 out = middleware.preprocess(app=self, state=state, event=event)
             if out is not None:
                 return out  # type: ignore
 
     async def postprocess(
-        self, state: State, event: Event, delta: Delta
-    ) -> Optional[Delta]:
+        self, state: State, event: Event, update: StateUpdate
+    ) -> StateUpdate:
         """Postprocess the event.
 
         This is where middleware can modify the delta after it is processed.
         Each middleware is called in the order it was added to the app.
 
-        If a middleware returns a delta, the delta is not processed and the
-        delta is returned.
-
         Args:
             state: The state to postprocess.
             event: The event to postprocess.
-            delta: The delta to postprocess.
+            update: The current state update.
 
         Returns:
-            An optional state to return.
+            The state update to return.
         """
         for middleware in self.middleware:
             if asyncio.iscoroutinefunction(middleware.postprocess):
                 out = await middleware.postprocess(
-                    app=self, state=state, event=event, delta=delta
+                    app=self, state=state, event=event, update=update
                 )
             else:
                 out = middleware.postprocess(
-                    app=self, state=state, event=event, delta=delta
+                    app=self, state=state, event=event, update=update
                 )
             if out is not None:
                 return out  # type: ignore
+        return update
 
     def add_middleware(self, middleware: Middleware, index: Optional[int] = None):
         """Add middleware to the app.
 
         Args:
             middleware: The middleware to add.
             index: The index to add the middleware at.
@@ -285,17 +281,34 @@
         # Format the route.
         route = format.format_route(route)
 
         # Add the page.
         self._check_routes_conflict(route)
         self.pages[route] = component
 
+        # Add the load events.
         if on_load:
+            if not isinstance(on_load, list):
+                on_load = [on_load]
             self.load_events[route] = on_load
 
+    def get_load_events(self, route: str) -> List[EventHandler]:
+        """Get the load events for a route.
+
+        Args:
+            route: The route to get the load events for.
+
+        Returns:
+            The load events for the route.
+        """
+        route = route.lstrip("/")
+        if route == "":
+            route = constants.INDEX_ROUTE
+        return self.load_events.get(route, [])
+
     def _check_routes_conflict(self, new_route: str):
         """Verify if there is any conflict between the new route and any existing route.
 
         Based on conflicts that NextJS would throw if not intercepted.
 
         Raises:
             ValueError: exception showing which conflict exist with the route to be added
@@ -407,15 +420,15 @@
 
         # Compile the custom components.
         compiler.compile_components(custom_components)
 
 
 async def process(
     app: App, event: Event, sid: str, headers: Dict, client_ip: str
-) -> List[StateUpdate]:
+) -> StateUpdate:
     """Process an event.
 
     Args:
         app: The app to process the event for.
         event: The event to process.
         sid: The Socket.IO session id.
         headers: The client headers.
@@ -440,35 +453,29 @@
     )
 
     # Also pass router_data to all substates. (TODO: this isn't recursive currently)
     for _, substate in state.substates.items():
         substate.router_data = state.router_data
 
     # Preprocess the event.
-    pre = await app.preprocess(state, event)
-    if isinstance(pre, StateUpdate):
-        return [pre]
-    updates = pre
-
-    # Apply the event to the state.
-    if updates is None:
-        updates = [await state._process(event)]
-        app.state_manager.set_state(event.token, state)
-
-    # Postprocess the event.
-    post_list = []
-    for update in updates:
-        post = await app.postprocess(state, event, update.delta)  # type: ignore
-        post_list.append(post) if post else None
+    update = await app.preprocess(state, event)
+
+    # Only process the event if there is no update.
+    if update is None:
+        # Apply the event to the state.
+        update = await state._process(event)
+
+        # Postprocess the event.
+        update = await app.postprocess(state, event, update)
 
-    if len(post_list) > 0:
-        return [StateUpdate(delta=post) for post in post_list]
+    # Update the state.
+    app.state_manager.set_state(event.token, state)
 
-    # Return the updates.
-    return updates
+    # Return the update.
+    return update
 
 
 async def ping() -> str:
     """Test API endpoint.
 
     Returns:
         The response.
@@ -594,19 +601,18 @@
             for (k, v) in environ["asgi.scope"]["headers"]
         }
 
         # Get the client IP
         client_ip = environ["REMOTE_ADDR"]
 
         # Process the events.
-        updates = await process(self.app, event, sid, headers, client_ip)
+        update = await process(self.app, event, sid, headers, client_ip)
 
         # Emit the event.
-        for update in updates:
-            await self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)  # type: ignore
+        await self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)  # type: ignore
 
     async def on_ping(self, sid):
         """Event for testing the API endpoint.
 
         Args:
             sid: The Socket.IO session id.
         """
```

### Comparing `pynecone-0.1.28a2/pynecone/base.py` & `pynecone-0.1.29a0/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/compiler/compiler.py` & `pynecone-0.1.29a0/pynecone/compiler/compiler.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,28 +7,33 @@
 
 from pynecone import constants
 from pynecone.compiler import templates, utils
 from pynecone.components.component import Component, CustomComponent
 from pynecone.state import State
 from pynecone.style import Style
 from pynecone.utils import imports, path_ops
+from pynecone.var import ImportVar
 
 # Imports to be included in every Pynecone app.
 DEFAULT_IMPORTS: imports.ImportDict = {
-    "react": {"useEffect", "useRef", "useState"},
-    "next/router": {"useRouter"},
+    "react": {
+        ImportVar(tag="useEffect"),
+        ImportVar(tag="useRef"),
+        ImportVar(tag="useState"),
+    },
+    "next/router": {ImportVar(tag="useRouter")},
     f"/{constants.STATE_PATH}": {
-        "connect",
-        "updateState",
-        "uploadFiles",
-        "E",
-        "isTrue",
+        ImportVar(tag="connect"),
+        ImportVar(tag="updateState"),
+        ImportVar(tag="uploadFiles"),
+        ImportVar(tag="E"),
+        ImportVar(tag="isTrue"),
     },
-    "": {"focus-visible/dist/focus-visible"},
-    "@chakra-ui/react": {constants.USE_COLOR_MODE},
+    "": {ImportVar(tag="focus-visible/dist/focus-visible")},
+    "@chakra-ui/react": {ImportVar(tag=constants.USE_COLOR_MODE)},
 }
 
 
 def _compile_document_root(root: Component) -> str:
     """Compile the document root.
 
     Args:
@@ -87,16 +92,16 @@
     Args:
         components: The components to compile.
 
     Returns:
         The compiled components.
     """
     imports = {
-        "react": {"memo"},
-        f"/{constants.STATE_PATH}": {"E", "isTrue"},
+        "react": {ImportVar(tag="memo")},
+        f"/{constants.STATE_PATH}": {ImportVar(tag="E"), ImportVar(tag="isTrue")},
     }
     component_defs = []
 
     # Compile each component.
     for component in components:
         component_def, component_imports = utils.compile_custom_component(component)
         component_defs.append(component_def)
```

### Comparing `pynecone-0.1.28a2/pynecone/compiler/templates.py` & `pynecone-0.1.29a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/compiler/utils.py` & `pynecone-0.1.29a0/pynecone/compiler/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,40 +21,37 @@
     Title,
 )
 from pynecone.components.component import Component, CustomComponent
 from pynecone.event import get_hydrate_event
 from pynecone.state import State
 from pynecone.style import Style
 from pynecone.utils import format, imports, path_ops
+from pynecone.var import ImportVar
 
 # To re-export this function.
 merge_imports = imports.merge_imports
 
 
-def compile_import_statement(lib: str, fields: Set[str]) -> str:
+def compile_import_statement(lib: str, fields: Set[ImportVar]) -> str:
     """Compile an import statement.
 
     Args:
         lib: The library to import from.
         fields: The set of fields to import from the library.
 
     Returns:
         The compiled import statement.
     """
     # Check for default imports.
-    defaults = {
-        field
-        for field in fields
-        if field.lower() == lib.lower().replace("-", "").replace("/", "")
-    }
+    defaults = {field for field in fields if field.is_default}
     assert len(defaults) < 2
 
     # Get the default import, and the specific imports.
-    default = next(iter(defaults), "")
-    rest = fields - defaults
+    default = next(iter({field.name for field in defaults}), "")
+    rest = {field.name for field in fields - defaults}
     return templates.format_import(lib=lib, default=default, rest=rest)
 
 
 def compile_imports(imports: imports.ImportDict) -> str:
     """Compile an import dict.
 
     Args:
```

### Comparing `pynecone-0.1.28a2/pynecone/components/__init__.py` & `pynecone-0.1.29a0/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/base/bare.py` & `pynecone-0.1.29a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/base/document.py` & `pynecone-0.1.29a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/base/link.py` & `pynecone-0.1.29a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/base/meta.py` & `pynecone-0.1.29a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/component.py` & `pynecone-0.1.29a0/pynecone/components/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     EventSpec,
     call_event_fn,
     call_event_handler,
     get_handler_args,
 )
 from pynecone.style import Style
 from pynecone.utils import format, imports, path_ops, types
-from pynecone.var import BaseVar, Var
+from pynecone.var import BaseVar, ImportVar, Var
 
 
 class Component(Base, ABC):
     """The base class for all Pynecone components."""
 
     # The children nested within the component.
     children: List[Component] = []
@@ -39,14 +39,20 @@
 
     # The library that the component is based on.
     library: Optional[str] = None
 
     # The tag to use when rendering the component.
     tag: Optional[str] = None
 
+    # The alias for the tag.
+    alias: Optional[str] = None
+
+    # Whether the import is default or named.
+    is_default: Optional[bool] = False
+
     # A unique key for the component.
     key: Any = None
 
     # The id for the component.
     id: Any = None
 
     # The class name for the component.
@@ -210,15 +216,17 @@
             events = []
             for v in value:
                 if isinstance(v, EventHandler):
                     # Call the event handler to get the event.
                     event = call_event_handler(v, arg)
 
                     # Check that the event handler takes no args if it's uncontrolled.
-                    if not is_controlled_event and len(event.args) > 0:
+                    if not is_controlled_event and (
+                        event.args is not None and len(event.args) > 0
+                    ):
                         raise ValueError(
                             f"Event handler: {v.fn} for uncontrolled event {event_trigger} should not take any args."
                         )
 
                     # Add the event to the chain.
                     events.append(event)
                 elif isinstance(v, EventSpec):
@@ -271,23 +279,14 @@
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
         return {}
 
-    @classmethod
-    def get_alias(cls) -> Optional[str]:
-        """Get the alias for the component.
-
-        Returns:
-            The alias.
-        """
-        return None
-
     def __repr__(self) -> str:
         """Represent the component in React.
 
         Returns:
             The code to render the component.
         """
         return self.render()
@@ -303,17 +302,18 @@
     def _render(self) -> Tag:
         """Define how to render the component in React.
 
         Returns:
             The tag to render.
         """
         # Create the base tag.
-        alias = self.get_alias()
-        name = alias if alias is not None else self.tag
-        tag = Tag(name=name, special_props=self.special_props)
+        tag = Tag(
+            name=self.tag if not self.alias else self.alias,
+            special_props=self.special_props,
+        )
 
         # Add component props to the tag.
         props = {attr: getattr(self, attr) for attr in self.get_props()}
 
         # Special case for props named `type_`.
         if hasattr(self, "type_"):
             props["type"] = self.type_  # type: ignore
@@ -441,17 +441,15 @@
             code |= child.get_custom_code()
 
         # Return the code.
         return code
 
     def _get_imports(self) -> imports.ImportDict:
         if self.library is not None and self.tag is not None:
-            alias = self.get_alias()
-            tag = self.tag if alias is None else " as ".join([self.tag, alias])
-            return {self.library: {tag}}
+            return {self.library: {self.import_var}}
         return {}
 
     def get_imports(self) -> imports.ImportDict:
         """Get all the libraries and fields that are used by the component.
 
         Returns:
             The import dict with the required imports.
@@ -517,14 +515,23 @@
         # Store the seen components in a set to avoid infinite recursion.
         if seen is None:
             seen = set()
         for child in self.children:
             custom_components |= child.get_custom_components(seen=seen)
         return custom_components
 
+    @property
+    def import_var(self):
+        """The tag to import.
+
+        Returns:
+            An import var.
+        """
+        return ImportVar(tag=self.tag, is_default=self.is_default, alias=self.alias)
+
     def is_full_control(self, kwargs: dict) -> bool:
         """Return if the component is fully controlled input.
 
         Args:
             kwargs: The component kwargs.
 
         Returns:
```

### Comparing `pynecone-0.1.28a2/pynecone/components/datadisplay/code.py` & `pynecone-0.1.29a0/pynecone/components/datadisplay/code.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 
 from typing import Dict
 
 from pynecone.components.component import Component
 from pynecone.components.libs.chakra import ChakraComponent
 from pynecone.style import Style
 from pynecone.utils import imports
-from pynecone.var import Var
+from pynecone.var import ImportVar, Var
 
 # Path to the prism styles.
 PRISM_STYLES_PATH = "/styles/code/prism"
 
 
 class CodeBlock(Component):
     """A code block."""
 
     library = "react-syntax-highlighter"
 
     tag = "Prism"
 
+    is_default = True
+
     # The theme to use ("light" or "dark").
     theme: Var[str]
 
     # The language to use.
     language: Var[str]
 
     # If this is enabled line numbers will be shown next to the code block.
@@ -40,15 +42,15 @@
     # Props passed down to the code tag.
     code_tag_props: Var[Dict[str, str]]
 
     def _get_imports(self) -> imports.ImportDict:
         merged_imports = super()._get_imports()
         if self.theme is not None:
             merged_imports = imports.merge_imports(
-                merged_imports, {PRISM_STYLES_PATH: {self.theme.name}}
+                merged_imports, {PRISM_STYLES_PATH: {ImportVar(tag=self.theme.name)}}
             )
         return merged_imports
 
     @classmethod
     def create(cls, *children, **props):
         """Create a text component.
```

### Comparing `pynecone-0.1.28a2/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.29a0/pynecone/components/datadisplay/datatable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Table components."""
 
-from typing import Any, List, Optional
+from typing import Any, List
 
 from pynecone.components.component import Component
 from pynecone.components.tags import Tag
 from pynecone.utils import format, imports, types
-from pynecone.var import BaseVar, ComputedVar, Var
+from pynecone.var import BaseVar, ComputedVar, ImportVar, Var
 
 
 class Gridjs(Component):
     """A component that wraps a nivo bar component."""
 
     library = "gridjs-react"
 
 
 class DataTable(Gridjs):
     """A data table component."""
 
     tag = "Grid"
 
+    alias = "DataTableGrid"
+
     # The data to display. Either a list of lists or a pandas dataframe.
     data: Any
 
     # The list of columns to display. Required if data is a list and should not be provided
     # if the data field is a dataframe
     columns: Var[List]
 
@@ -35,23 +37,14 @@
     # Enable resizable columns.
     resizable: Var[bool]
 
     # Enable pagination.
     pagination: Var[bool]
 
     @classmethod
-    def get_alias(cls) -> Optional[str]:
-        """Get the alias for the component.
-
-        Returns:
-            The alias.
-        """
-        return "DataTableGrid"
-
-    @classmethod
     def create(cls, *children, **props):
         """Create a datatable component.
 
         Args:
             *children: The children of the component.
             **props: The props to pass to the component.
 
@@ -98,15 +91,16 @@
         return super().create(
             *children,
             **props,
         )
 
     def _get_imports(self) -> imports.ImportDict:
         return imports.merge_imports(
-            super()._get_imports(), {"": {"gridjs/dist/theme/mermaid.css"}}
+            super()._get_imports(),
+            {"": {ImportVar(tag="gridjs/dist/theme/mermaid.css")}},
         )
 
     def _render(self) -> Tag:
         if isinstance(self.data, Var):
             self.columns = BaseVar(
                 name=f"{self.data.name}.columns"
                 if types.is_dataframe(self.data.type_)
```

### Comparing `pynecone-0.1.28a2/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.29a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/datadisplay/list.py` & `pynecone-0.1.29a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.29a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/datadisplay/table.py` & `pynecone-0.1.29a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.29a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.29a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/feedback/alert.py` & `pynecone-0.1.29a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.29a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/feedback/progress.py` & `pynecone-0.1.29a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.29a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/feedback/spinner.py` & `pynecone-0.1.29a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/__init__.py` & `pynecone-0.1.29a0/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/button.py` & `pynecone-0.1.29a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/checkbox.py` & `pynecone-0.1.29a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.29a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/editable.py` & `pynecone-0.1.29a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/formcontrol.py` & `pynecone-0.1.29a0/pynecone/components/forms/formcontrol.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.29a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/input.py` & `pynecone-0.1.29a0/pynecone/components/forms/input.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """An input component."""
 
 from typing import Dict
 
 from pynecone.components.component import EVENT_ARG
 from pynecone.components.libs.chakra import ChakraComponent
 from pynecone.utils import imports
-from pynecone.var import Var
+from pynecone.var import ImportVar, Var
 
 
 class Input(ChakraComponent):
     """The Input component is a component that is used to get user input in a text field."""
 
     tag = "Input"
 
-    # State var to bind the the input.
+    # State var to bind the input.
     value: Var[str]
 
     # The default value of the input.
     default_value: Var[str]
 
     # The placeholder text.
     placeholder: Var[str]
@@ -48,15 +48,15 @@
 
     # "lg" | "md" | "sm" | "xs"
     size: Var[str]
 
     def _get_imports(self) -> imports.ImportDict:
         return imports.merge_imports(
             super()._get_imports(),
-            {"/utils/state": {"set_val"}},
+            {"/utils/state": {ImportVar(tag="set_val")}},
         )
 
     @classmethod
     def get_controlled_triggers(cls) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
```

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/numberinput.py` & `pynecone-0.1.29a0/pynecone/components/forms/numberinput.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class NumberInput(ChakraComponent):
     """The wrapper that provides context and logic to the components."""
 
     tag = "NumberInput"
 
-    # State var to bind the the input.
+    # State var to bind the input.
     value: Var[int]
 
     # If true, the input's value will change based on mouse wheel.
     allow_mouse_wheel: Var[bool]
 
     # This controls the value update when you blur out of the input. - If true and the value is greater than max, the value will be reset to max - Else, the value remains the same.
     clamped_value_on_blur: Var[bool]
```

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/pininput.py` & `pynecone-0.1.29a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/radio.py` & `pynecone-0.1.29a0/pynecone/components/forms/radio.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     """A grouping of individual radio options."""
 
     tag = "RadioGroup"
 
     # State var to bind the the input.
     value: Var[Any]
 
+    # The default value.
+    default_value: Var[Any]
+
     @classmethod
     def get_controlled_triggers(cls) -> Dict[str, Var]:
         """Get the event triggers that pass the component's value to the handler.
 
         Returns:
             A dict mapping the event trigger to the var that is passed to the handler.
         """
```

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.29a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/select.py` & `pynecone-0.1.29a0/pynecone/components/forms/select.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class Select(ChakraComponent):
     """Select component is a component that allows users pick a value from predefined options. Ideally, it should be used when there are more than 5 options, otherwise you might consider using a radio group instead."""
 
     tag = "Select"
 
-    # State var to bind the the select.
+    # State var to bind the select.
     value: Var[str]
 
     # The default value of the select.
     default_value: Var[str]
 
     # The placeholder text.
     placeholder: Var[str]
```

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/slider.py` & `pynecone-0.1.29a0/pynecone/components/forms/slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Slider(ChakraComponent):
     """The wrapper that provides context and functionality for all children."""
 
     tag = "Slider"
 
-    # State var to bind the the input.
+    # State var to bind the input.
     value: Var[int]
 
     # The color scheme.
     color_scheme: Var[str]
 
     # The placeholder text.
     default_value: Var[int]
```

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/switch.py` & `pynecone-0.1.29a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/textarea.py` & `pynecone-0.1.29a0/pynecone/components/forms/textarea.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class TextArea(ChakraComponent):
     """A text area component."""
 
     tag = "Textarea"
 
-    # State var to bind the the input.
+    # State var to bind the input.
     value: Var[str]
 
     # The default value of the textarea.
     default_value: Var[str]
 
     # The placeholder text.
     placeholder: Var[str]
```

### Comparing `pynecone-0.1.28a2/pynecone/components/forms/upload.py` & `pynecone-0.1.29a0/pynecone/components/forms/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 class Upload(Component):
     """A file upload component."""
 
     library = "react-dropzone"
 
     tag = "ReactDropzone"
 
+    is_default = True
+
     # The list of accepted file types. This should be a dictionary of MIME types as keys and array of file formats as
     # values.
     # supported MIME types: https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types
     accept: Var[Optional[Dict[str, List]]]
 
     # Whether the dropzone is disabled.
     disabled: Var[bool]
```

### Comparing `pynecone-0.1.28a2/pynecone/components/graphing/plotly.py` & `pynecone-0.1.29a0/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/graphing/victory.py` & `pynecone-0.1.29a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/__init__.py` & `pynecone-0.1.29a0/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/box.py` & `pynecone-0.1.29a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/cond.py` & `pynecone-0.1.29a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/flex.py` & `pynecone-0.1.29a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/foreach.py` & `pynecone-0.1.29a0/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/grid.py` & `pynecone-0.1.29a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/html.py` & `pynecone-0.1.29a0/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/responsive.py` & `pynecone-0.1.29a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/stack.py` & `pynecone-0.1.29a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/layout/wrap.py` & `pynecone-0.1.29a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/media/avatar.py` & `pynecone-0.1.29a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/media/icon.py` & `pynecone-0.1.29a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/media/image.py` & `pynecone-0.1.29a0/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.29a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/navigation/link.py` & `pynecone-0.1.29a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.29a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/overlay/__init__.py` & `pynecone-0.1.29a0/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.29a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/overlay/drawer.py` & `pynecone-0.1.29a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/overlay/menu.py` & `pynecone-0.1.29a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/overlay/modal.py` & `pynecone-0.1.29a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/overlay/popover.py` & `pynecone-0.1.29a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.29a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/tags/cond_tag.py` & `pynecone-0.1.29a0/pynecone/components/tags/cond_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.29a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/tags/tag.py` & `pynecone-0.1.29a0/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/tags/tagless.py` & `pynecone-0.1.29a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/components/typography/markdown.py` & `pynecone-0.1.29a0/pynecone/components/typography/markdown.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Markdown component."""
 
 import textwrap
 from typing import List, Union
 
 from pynecone.components.component import Component
 from pynecone.utils import types
-from pynecone.var import BaseVar, Var
+from pynecone.var import BaseVar, ImportVar, Var
 
 
 class Markdown(Component):
     """A markdown component."""
 
     library = "react-markdown"
 
     tag = "ReactMarkdown"
 
+    is_default = True
+
     @classmethod
     def create(cls, *children, **props) -> Component:
         """Create a markdown component.
 
         Args:
             children: The children of the component.
             props: The properties of the component.
@@ -35,28 +37,28 @@
         if isinstance(src, str):
             src = textwrap.dedent(src)
         return super().create(src, **props)
 
     def _get_imports(self):
         imports = super()._get_imports()
         imports["@chakra-ui/react"] = {
-            "Heading",
-            "Code",
-            "Text",
-            "Link",
-            "UnorderedList",
-            "OrderedList",
-            "ListItem",
+            ImportVar(tag="Heading"),
+            ImportVar(tag="Code"),
+            ImportVar(tag="Text"),
+            ImportVar(tag="Link"),
+            ImportVar(tag="UnorderedList"),
+            ImportVar(tag="OrderedList"),
+            ImportVar(tag="ListItem"),
         }
-        imports["react-syntax-highlighter"] = {"Prism"}
-        imports["remark-math"] = {"remarkMath"}
-        imports["remark-gfm"] = {"remarkGfm"}
-        imports["rehype-katex"] = {"rehypeKatex"}
-        imports["rehype-raw"] = {"rehypeRaw"}
-        imports[""] = {"katex/dist/katex.min.css"}
+        imports["react-syntax-highlighter"] = {ImportVar(tag="Prism", is_default=True)}
+        imports["remark-math"] = {ImportVar(tag="remarkMath", is_default=True)}
+        imports["remark-gfm"] = {ImportVar(tag="remarkGfm", is_default=True)}
+        imports["rehype-katex"] = {ImportVar(tag="rehypeKatex", is_default=True)}
+        imports["rehype-raw"] = {ImportVar(tag="rehypeRaw", is_default=True)}
+        imports[""] = {ImportVar(tag="katex/dist/katex.min.css")}
         return imports
 
     def _render(self):
         return (
             super()
             ._render()
             .add_props(
```

### Comparing `pynecone-0.1.28a2/pynecone/config.py` & `pynecone-0.1.29a0/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/constants.py` & `pynecone-0.1.29a0/pynecone/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # The name of the Pynecone module.
 MODULE_NAME = "pynecone"
 # The name of the pip install package.
 PACKAGE_NAME = "pynecone"
 # The current version of Pynecone.
 VERSION = pkg_resources.get_distribution(PACKAGE_NAME).version
 # Minimum version of Node.js required to run Pynecone.
-MIN_NODE_VERSION = "12.22.0"
+MIN_NODE_VERSION = "16.6.0"
 
 # Valid bun versions.
 MIN_BUN_VERSION = "0.5.8"
 MAX_BUN_VERSION = "0.5.9"
 INVALID_BUN_VERSIONS = ["0.5.5", "0.5.6", "0.5.7"]
 
 # Files and directories used to init a new project.
@@ -67,25 +67,25 @@
 # The backend default port.
 BACKEND_PORT = "8000"
 # The backend api url.
 API_URL = "http://localhost:8000"
 # The default path where bun is installed.
 BUN_PATH = "$HOME/.bun/bin/bun"
 # Command to install bun.
-INSTALL_BUN = "curl -fsSL https://bun.sh/install | bash -s -- bun-v0.5.9"
+INSTALL_BUN = f"curl -fsSL https://bun.sh/install | bash -s -- bun-v{MAX_BUN_VERSION}"
 # Default host in dev mode.
 BACKEND_HOST = "0.0.0.0"
 # The default timeout when launching the gunicorn server.
 TIMEOUT = 120
 # The command to run the backend in production mode.
 RUN_BACKEND_PROD = f"gunicorn --worker-class uvicorn.workers.UvicornH11Worker --preload --timeout {TIMEOUT} --log-level critical".split()
 RUN_BACKEND_PROD_WINDOWS = f"uvicorn --timeout-keep-alive {TIMEOUT}".split()
 # Socket.IO web server
 PING_INTERVAL = 25
-PING_TIMEOUT = 5
+PING_TIMEOUT = 120
 
 # Compiler variables.
 # The extension for compiled Javascript files.
 JS_EXT = ".js"
 # The extension for python files.
 PY_EXT = ".py"
 # The expected variable name where the pc.App is stored.
@@ -102,14 +102,16 @@
 PROCESSING = "processing"
 # The name of the state variable.
 STATE = "state"
 # The name of the events variable.
 EVENTS = "events"
 # The name of the initial hydrate event.
 HYDRATE = "hydrate"
+# The name of the is_hydrated variable.
+IS_HYDRATED = "is_hydrated"
 # The name of the index page.
 INDEX_ROUTE = "index"
 # The name of the document root page.
 DOCUMENT_ROOT = "_document"
 # The name of the theme page.
 THEME = "theme"
 # The prefix used to create setters for state vars.
```

### Comparing `pynecone-0.1.28a2/pynecone/el/constants/html.py` & `pynecone-0.1.29a0/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/el/constants/pynecone.py` & `pynecone-0.1.29a0/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/el/constants/react.py` & `pynecone-0.1.29a0/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/el/element.py` & `pynecone-0.1.29a0/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/el/elements/__init__.py` & `pynecone-0.1.29a0/pynecone/el/elements/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Union
 
 from pynecone.el.element import Element
 from pynecone.var import Var as PCVar
 
 
 class A(Element):  # noqa: E742
-    """Display the a element."""
+    """Display the 'a' element."""
 
     tag = "a"
 
     access_key: PCVar[Union[str, int, bool]]
     auto_capitalize: PCVar[Union[str, int, bool]]
     content_editable: PCVar[Union[str, int, bool]]
     context_menu: PCVar[Union[str, int, bool]]
```

### Comparing `pynecone-0.1.28a2/pynecone/el/precompile.py` & `pynecone-0.1.29a0/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/event.py` & `pynecone-0.1.29a0/pynecone/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # The event name.
     name: str
 
     # The routing data where event occurred
     router_data: Dict[str, Any] = {}
 
     # The event payload.
-    payload: Dict[Any, Any] = {}
+    payload: Dict[str, Any] = {}
 
 
 class EventHandler(Base):
     """An event handler responds to an event to update the state."""
 
     # The function to call in response to the event.
     fn: Callable
@@ -323,24 +323,22 @@
 
     Args:
         event_spec: The event spec.
         arg: The controlled event argument.
 
     Returns:
         The handler args.
-
-    Raises:
-        ValueError: If the event handler has an invalid signature.
     """
     args = inspect.getfullargspec(event_spec.handler.fn).args
-    if len(args) < 2:
-        raise ValueError(
-            f"Event handler has an invalid signature, needed a method with a parameter, got {event_spec.handler}."
-        )
-    return event_spec.args if len(args) > 2 else ((Var.create_safe(args[1]), arg),)
+
+    return (
+        event_spec.args
+        if len(args) > 2
+        else (((Var.create_safe(args[1]), arg),) if len(args) == 2 else tuple())
+    )
 
 
 def fix_events(
     events: Optional[List[Union[EventHandler, EventSpec]]], token: str
 ) -> List[Event]:
     """Fix a list of events returned by an event handler.
```

### Comparing `pynecone-0.1.28a2/pynecone/middleware/logging_middleware.py` & `pynecone-0.1.29a0/pynecone/middleware/logging_middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Logging middleware."""
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from pynecone.event import Event
 from pynecone.middleware.middleware import Middleware
-from pynecone.state import Delta, State
+from pynecone.state import State, StateUpdate
 
 if TYPE_CHECKING:
     from pynecone.app import App
 
 
 class LoggingMiddleware(Middleware):
     """Middleware to log requests and responses."""
@@ -20,17 +20,19 @@
         Args:
             app: The app to apply the middleware to.
             state: The client state.
             event: The event to preprocess.
         """
         print(f"Event {event}")
 
-    async def postprocess(self, app: App, state: State, event: Event, delta: Delta):
+    async def postprocess(
+        self, app: App, state: State, event: Event, update: StateUpdate
+    ):
         """Postprocess the event.
 
         Args:
             app: The app to apply the middleware to.
             state: The client state.
             event: The event to postprocess.
-            delta: The delta to postprocess.
+            update: The current state update.
         """
-        print(f"Delta {delta}")
+        print(f"Update {update}")
```

### Comparing `pynecone-0.1.28a2/pynecone/middleware/middleware.py` & `pynecone-0.1.29a0/pynecone/middleware/middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 """Base Pynecone middleware."""
 from __future__ import annotations
 
 from abc import ABC
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Optional
 
 from pynecone.base import Base
 from pynecone.event import Event
-from pynecone.state import Delta, State, StateUpdate
+from pynecone.state import State, StateUpdate
 
 if TYPE_CHECKING:
     from pynecone.app import App
 
 
 class Middleware(Base, ABC):
     """Middleware to preprocess and postprocess requests."""
 
     async def preprocess(
         self, app: App, state: State, event: Event
-    ) -> Optional[Union[StateUpdate, List[StateUpdate]]]:
+    ) -> Optional[StateUpdate]:
         """Preprocess the event.
 
         Args:
             app: The app.
             state: The client state.
             event: The event to preprocess.
 
         Returns:
-            An optional state to return.
+            An optional state update to return.
         """
         return None
 
     async def postprocess(
-        self, app: App, state: State, event: Event, delta
-    ) -> Optional[Delta]:
+        self, app: App, state: State, event: Event, update: StateUpdate
+    ) -> StateUpdate:
         """Postprocess the event.
 
         Args:
             app: The app.
             state: The client state.
             event: The event to postprocess.
-            delta: The delta to postprocess.
+            update: The current state update.
 
         Returns:
             An optional state to return.
         """
-        return None
+        return update
```

### Comparing `pynecone-0.1.28a2/pynecone/model.py` & `pynecone-0.1.29a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/pc.py` & `pynecone-0.1.29a0/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/route.py` & `pynecone-0.1.29a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/state.py` & `pynecone-0.1.29a0/pynecone/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Define the pynecone state specification."""
 from __future__ import annotations
 
 import asyncio
+import copy
 import functools
 import traceback
 from abc import ABC
 from collections import defaultdict
 from typing import (
     Any,
     Callable,
@@ -70,19 +71,16 @@
 
     # The routing path that triggered the state
     router_data: Dict[str, Any] = {}
 
     # Mapping of var name to set of computed variables that depend on it
     computed_var_dependencies: Dict[str, Set[str]] = {}
 
-    # Whether to track accessed vars.
-    track_vars: bool = False
-
-    # The current set of accessed vars during tracking.
-    tracked_vars: Set[str] = set()
+    # Per-instance copy of backend variable values
+    _backend_vars: Dict[str, Any] = {}
 
     def __init__(self, *args, parent_state: Optional[State] = None, **kwargs):
         """Initialize the state.
 
         Args:
             *args: The args to pass to the Pydantic init method.
             parent_state: The parent state.
@@ -98,30 +96,26 @@
         # Convert the event handlers to functions.
         for name, event_handler in self.event_handlers.items():
             fn = functools.partial(event_handler.fn, self)
             fn.__module__ = event_handler.fn.__module__  # type: ignore
             fn.__qualname__ = event_handler.fn.__qualname__  # type: ignore
             setattr(self, name, fn)
 
-        # Initialize the mutable fields.
-        self._init_mutable_fields()
-
         # Initialize computed vars dependencies.
         self.computed_var_dependencies = defaultdict(set)
-        for cvar in self.computed_vars:
-            self.tracked_vars = set()
+        for cvar_name, cvar in self.computed_vars.items():
+            # Add the dependencies.
+            for var in cvar.deps():
+                self.computed_var_dependencies[var].add(cvar_name)
 
-            # Enable tracking and get the computed var.
-            self.track_vars = True
-            self.__getattribute__(cvar)
-            self.track_vars = False
+        # Initialize the mutable fields.
+        self._init_mutable_fields()
 
-            # Add the dependencies.
-            for var in self.tracked_vars:
-                self.computed_var_dependencies[var].add(cvar)
+        # Create a fresh copy of the backend variables for this instance
+        self._backend_vars = copy.deepcopy(self.backend_vars)
 
     def _init_mutable_fields(self):
         """Initialize mutable fields.
 
         So that mutation to them can be detected by the app:
         * list
         """
@@ -195,15 +189,14 @@
             if isinstance(v, ComputedVar)
         }
         cls.vars = {
             **cls.inherited_vars,
             **cls.base_vars,
             **cls.computed_vars,
         }
-        cls.computed_var_dependencies = {}
         cls.event_handlers = {}
 
         # Setup the base vars at the class level.
         for prop in cls.base_vars.values():
             cls._init_var(prop)
 
         # Set up the event handlers.
@@ -229,16 +222,15 @@
         return set(cls.inherited_vars) | {
             "parent_state",
             "substates",
             "dirty_vars",
             "dirty_substates",
             "router_data",
             "computed_var_dependencies",
-            "track_vars",
-            "tracked_vars",
+            "_backend_vars",
         }
 
     @classmethod
     @functools.lru_cache()
     def get_parent_state(cls) -> Optional[Type[State]]:
         """Get the parent state.
 
@@ -496,53 +488,43 @@
         for param, value in args.items():
             if value == constants.RouteArgType.SINGLE:
                 func = argsingle_factory(param)
             elif value == constants.RouteArgType.LIST:
                 func = arglist_factory(param)
             else:
                 continue
-            cls.computed_vars[param] = func.set_state(cls)  # type: ignore
+            # link dynamically created ComputedVar to this state class for dep determination
+            func.__objclass__ = cls
+            func.fget.__name__ = param
+            cls.vars[param] = cls.computed_vars[param] = func.set_state(cls)  # type: ignore
             setattr(cls, param, func)
 
     def __getattribute__(self, name: str) -> Any:
         """Get the state var.
 
         If the var is inherited, get the var from the parent state.
 
-        If the Var is a dependent of a ComputedVar, track this status in computed_var_dependencies.
-
         Args:
             name: The name of the var.
 
         Returns:
             The value of the var.
         """
         # If the state hasn't been initialized yet, return the default value.
         if not super().__getattribute__("__dict__"):
             return super().__getattribute__(name)
 
-        # Check if tracking is enabled.
-        if super().__getattribute__("track_vars"):
-            # Get the non-computed vars.
-            all_vars = {
-                **super().__getattribute__("vars"),
-                **super().__getattribute__("backend_vars"),
-            }
-            # Add the var to the tracked vars.
-            if name in all_vars:
-                super().__getattribute__("tracked_vars").add(name)
-
         inherited_vars = {
             **super().__getattribute__("inherited_vars"),
             **super().__getattribute__("inherited_backend_vars"),
         }
         if name in inherited_vars:
             return getattr(super().__getattribute__("parent_state"), name)
-        elif name in super().__getattribute__("backend_vars"):
-            return super().__getattribute__("backend_vars").__getitem__(name)
+        elif name in super().__getattribute__("_backend_vars"):
+            return super().__getattribute__("_backend_vars").__getitem__(name)
         return super().__getattribute__(name)
 
     def __setattr__(self, name: str, value: Any):
         """Set the attribute.
 
         If the attribute is inherited, set the attribute on the parent state.
 
@@ -552,25 +534,25 @@
         """
         # Set the var on the parent state.
         inherited_vars = {**self.inherited_vars, **self.inherited_backend_vars}
         if name in inherited_vars:
             setattr(self.parent_state, name, value)
             return
 
-        if types.is_backend_variable(name):
-            self.backend_vars.__setitem__(name, value)
+        if types.is_backend_variable(name) and name != "_backend_vars":
+            self._backend_vars.__setitem__(name, value)
             self.dirty_vars.add(name)
             self.mark_dirty()
             return
 
         # Set the attribute.
         super().__setattr__(name, value)
 
         # Add the var to the dirty list.
-        if name in self.vars:
+        if name in self.vars or name in self.computed_var_dependencies:
             self.dirty_vars.add(name)
             self.mark_dirty()
 
     def reset(self):
         """Reset all the base vars to their default values."""
         # Reset the base vars.
         fields = self.get_fields()
@@ -672,75 +654,82 @@
 
         # Reset the dirty vars.
         self.clean()
 
         # Return the state update.
         return StateUpdate(delta=delta, events=events)
 
-    def _dirty_computed_vars(
-        self, from_vars: Optional[Set[str]] = None, check: bool = False
-    ) -> Set[str]:
-        """Get ComputedVars that need to be recomputed based on dirty_vars.
+    def _mark_dirty_computed_vars(self) -> None:
+        """Mark ComputedVars that need to be recalculated based on dirty_vars."""
+        dirty_vars = self.dirty_vars
+        while dirty_vars:
+            calc_vars, dirty_vars = dirty_vars, set()
+            for cvar in self._dirty_computed_vars(from_vars=calc_vars):
+                self.dirty_vars.add(cvar)
+                dirty_vars.add(cvar)
+                actual_var = self.computed_vars.get(cvar)
+                if actual_var:
+                    actual_var.mark_dirty(instance=self)
+
+    def _dirty_computed_vars(self, from_vars: Optional[Set[str]] = None) -> Set[str]:
+        """Determine ComputedVars that need to be recalculated based on the given vars.
 
         Args:
             from_vars: find ComputedVar that depend on this set of vars. If unspecified, will use the dirty_vars.
-            check: Whether to perform the check.
 
         Returns:
             Set of computed vars to include in the delta.
         """
-        # If checking is disabled, return all computed vars.
-        if not check:
-            return set(self.computed_vars)
-
-        # Return only the computed vars that depend on the dirty vars.
         return set(
             cvar
             for dirty_var in from_vars or self.dirty_vars
-            for cvar in self.computed_vars
-            if cvar in self.computed_var_dependencies.get(dirty_var, set())
+            for cvar in self.computed_var_dependencies[dirty_var]
         )
 
-    def get_delta(self, check: bool = False) -> Delta:
+    def get_delta(self) -> Delta:
         """Get the delta for the state.
 
-        Args:
-            check: Whether to check for dirty computed vars.
-
         Returns:
             The delta for the state.
         """
         delta = {}
 
-        # Return the dirty vars, as well as computed vars depending on dirty vars.
+        # Recursively find the substate deltas.
+        substates = self.substates
+        for substate in self.dirty_substates:
+            delta.update(substates[substate].get_delta())
+
+        # Return the dirty vars and dependent computed vars
+        delta_vars = self.dirty_vars.intersection(self.base_vars).union(
+            self._dirty_computed_vars()
+        )
         subdelta = {
             prop: getattr(self, prop)
-            for prop in self.dirty_vars | self._dirty_computed_vars(check=check)
+            for prop in delta_vars
             if not types.is_backend_variable(prop)
         }
         if len(subdelta) > 0:
             delta[self.get_full_name()] = subdelta
 
-        # Recursively find the substate deltas.
-        substates = self.substates
-        for substate in self.dirty_substates:
-            delta.update(substates[substate].get_delta())
-
         # Format the delta.
         delta = format.format_state(delta)
 
         # Return the delta.
         return delta
 
     def mark_dirty(self):
         """Mark the substate and all parent states as dirty."""
         if self.parent_state is not None:
             self.parent_state.dirty_substates.add(self.get_name())
             self.parent_state.mark_dirty()
 
+        # have to mark computed vars dirty to allow access to newly computed
+        # values within the same ComputedVar function
+        self._mark_dirty_computed_vars()
+
     def clean(self):
         """Reset the dirty vars."""
         # Recursively clean the substates.
         for substate in self.dirty_substates:
             self.substates[substate].clean()
 
         # Clean this state.
```

### Comparing `pynecone-0.1.28a2/pynecone/style.py` & `pynecone-0.1.29a0/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/telemetry.py` & `pynecone-0.1.29a0/pynecone/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/utils/build.py` & `pynecone-0.1.29a0/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/utils/console.py` & `pynecone-0.1.29a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/utils/exec.py` & `pynecone-0.1.29a0/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/utils/format.py` & `pynecone-0.1.29a0/pynecone/utils/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,17 @@
         event_spec: The event to format.
 
     Returns:
         The compiled event.
     """
     args = ",".join(
         [
-            ":".join((name.name, json.dumps(val.name) if val.is_string else val.name))
+            ":".join(
+                (name.name, json.dumps(val.name) if val.is_string else val.full_name)
+            )
             for name, val in event_spec.args
         ]
     )
     return f"E(\"{format_event_handler(event_spec.handler)}\", {wrap(args, '{')})"
 
 
 def format_upload_event(event_spec: EventSpec) -> str:
@@ -319,15 +321,15 @@
 
     Returns:
         The compiled event.
     """
     from pynecone.compiler import templates
 
     event_spec = event_chain.events[0]
-    arg = event_spec.args[0][1]
+    arg = event_spec.args[0][1] if event_spec.args else None
     state_name = event_chain.state_name
     chain = ",".join([format_event(event) for event in event_chain.events])
     event = templates.FULL_CONTROL(state_name=state_name, arg=arg, chain=chain)
     return event
 
 
 def format_query_params(router_data: Dict[str, Any]) -> Dict[str, str]:
```

### Comparing `pynecone-0.1.28a2/pynecone/utils/imports.py` & `pynecone-0.1.29a0/pynecone/utils/imports.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Import operations."""
 
 from collections import defaultdict
 from typing import Dict, Set
 
-ImportDict = Dict[str, Set[str]]
+from pynecone.var import ImportVar
+
+ImportDict = Dict[str, Set[ImportVar]]
 
 
 def merge_imports(*imports) -> ImportDict:
     """Merge two import dicts together.
 
     Args:
         *imports: The list of import dicts to merge.
```

### Comparing `pynecone-0.1.28a2/pynecone/utils/path_ops.py` & `pynecone-0.1.29a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/utils/prerequisites.py` & `pynecone-0.1.29a0/pynecone/utils/prerequisites.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,55 +9,56 @@
 import subprocess
 import sys
 from pathlib import Path
 from types import ModuleType
 from typing import Optional
 
 import typer
+from packaging import version
 from redis import Redis
 
 from pynecone import constants
 from pynecone.config import get_config
 from pynecone.utils import console, path_ops
 
 
-def check_node_version(min_version):
+def check_node_version(min_version=constants.MIN_NODE_VERSION):
     """Check the version of Node.js.
 
     Args:
         min_version: The minimum version of Node.js required.
 
     Returns:
         Whether the version of Node.js is high enough.
     """
     try:
         # Run the node -v command and capture the output
         result = subprocess.run(
             ["node", "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
-        # The output will be in the form "vX.Y.Z", so we can split it on the "v" character and take the second part
-        version = result.stdout.decode().strip().split("v")[1]
+        # The output will be in the form "vX.Y.Z", but version.parse() can handle it
+        current_version = version.parse(result.stdout.decode())
         # Compare the version numbers
-        return version.split(".") >= min_version.split(".")
+        return current_version >= version.parse(min_version)
     except Exception:
         return False
 
 
-def get_bun_version() -> Optional[str]:
+def get_bun_version() -> Optional[version.Version]:
     """Get the version of bun.
 
     Returns:
         The version of bun.
     """
     try:
         # Run the bun -v command and capture the output
         result = subprocess.run(
             ["bun", "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
-        return result.stdout.decode().strip()
+        return version.parse(result.stdout.decode().strip())
     except Exception:
         return None
 
 
 def get_package_manager() -> str:
     """Get the package manager executable.
 
@@ -68,15 +69,15 @@
         FileNotFoundError: If bun or npm is not installed.
         Exit: If the app directory is invalid.
 
     """
     config = get_config()
 
     # Check that the node version is valid.
-    if not check_node_version(constants.MIN_NODE_VERSION):
+    if not check_node_version():
         console.print(
             f"[red]Node.js version {constants.MIN_NODE_VERSION} or higher is required to run Pynecone."
         )
         raise typer.Exit()
 
     # On Windows, we use npm instead of bun.
     if platform.system() == "Windows" or config.disable_bun:
@@ -216,24 +217,24 @@
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: If the required packages are not installed.
         Exit: If the bun version is not supported.
     """
     bun_version = get_bun_version()
-    if bun_version is not None and bun_version in constants.INVALID_BUN_VERSIONS:
+    if bun_version is not None and (
+        bun_version < version.parse(constants.MIN_BUN_VERSION)
+        or bun_version > version.parse(constants.MAX_BUN_VERSION)
+        or str(bun_version) in constants.INVALID_BUN_VERSIONS
+    ):
         console.print(
             f"""[red]Bun version {bun_version} is not supported by Pynecone. Please change your to bun version to be between {constants.MIN_BUN_VERSION} and {constants.MAX_BUN_VERSION}."""
         )
         console.print(
-            f"""[red]Upgrade by running the following command:[/red]
-
-curl -fsSL https://bun.sh/install | bash -s -- bun-v{constants.MAX_BUN_VERSION}
-
-"""
+            f"""[red]Upgrade by running the following command:[/red]\n\n{constants.INSTALL_BUN}"""
         )
         raise typer.Exit()
 
     # Bun is not supported on Windows.
     if platform.system() == "Windows":
         console.log("Skipping bun installation on Windows.")
         return
```

### Comparing `pynecone-0.1.28a2/pynecone/utils/processes.py` & `pynecone-0.1.29a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pynecone/utils/types.py` & `pynecone-0.1.29a0/pynecone/utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Contains custom types and methods to check types."""
 
 from __future__ import annotations
 
 import contextlib
+import typing
 from typing import Any, Callable, Tuple, Type, Union, _GenericAlias  # type: ignore
 
 from pynecone.base import Base
 
 # Union of generic types.
 GenericType = Union[Type, _GenericAlias]
 
@@ -131,14 +132,16 @@
 
     Args:
         value: The value to check.
 
     Returns:
         Whether the value is a dataframe.
     """
+    if is_generic_alias(value) or value == typing.Any:
+        return False
     return value.__name__ == "DataFrame"
 
 
 def is_figure(value: Type) -> bool:
     """Check if the given value is a figure.
 
     Args:
```

### Comparing `pynecone-0.1.28a2/pynecone/var.py` & `pynecone-0.1.29a0/pynecone/var.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 """Define a state var."""
 from __future__ import annotations
 
+import contextlib
+import dis
 import json
 import random
 import string
 from abc import ABC
+from types import FunctionType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
     Optional,
+    Set,
     Type,
     Union,
     _GenericAlias,  # type: ignore
+    cast,
     get_type_hints,
 )
 
 from plotly.graph_objects import Figure
 from plotly.io import to_json
 from pydantic.fields import ModelField
 
 from pynecone import constants
 from pynecone.base import Base
 from pynecone.utils import format, types
 
 if TYPE_CHECKING:
     from pynecone.state import State
 
-
 # Set of unique variable names.
 USED_VARIABLES = set()
 
 
 def get_unique_variable_name() -> str:
     """Get a unique variable name.
 
@@ -265,34 +269,40 @@
         Args:
             name: The name of the attribute.
 
         Returns:
             The var attribute.
 
         Raises:
-            Exception: If the attribute is not found.
+            AttributeError: If the var is wrongly annotated or can't find attribute.
+            TypeError: If an annotation to the var isn't provided.
         """
         try:
             return super().__getattribute__(name)
         except Exception as e:
             # Check if the attribute is one of the class fields.
-            if (
-                not name.startswith("_")
-                and hasattr(self.type_, "__fields__")
-                and name in self.type_.__fields__
-            ):
-                type_ = self.type_.__fields__[name].outer_type_
-                if isinstance(type_, ModelField):
-                    type_ = type_.type_
-                return BaseVar(
-                    name=f"{self.name}.{name}",
-                    type_=type_,
-                    state=self.state,
-                )
-            raise e
+            if not name.startswith("_"):
+                if self.type_ == Any:
+                    raise TypeError(
+                        f"You must provide an annotation for the state var `{self.full_name}`. Annotation cannot be `{self.type_}`"
+                    ) from None
+                if hasattr(self.type_, "__fields__") and name in self.type_.__fields__:
+                    type_ = self.type_.__fields__[name].outer_type_
+                    if isinstance(type_, ModelField):
+                        type_ = type_.type_
+                    return BaseVar(
+                        name=f"{self.name}.{name}",
+                        type_=type_,
+                        state=self.state,
+                    )
+            raise AttributeError(
+                f"The State var `{self.full_name}` has no attribute '{name}' or may have been annotated "
+                f"wrongly.\n"
+                f"original message: {e.args[0]}"
+            ) from e
 
     def operation(
         self,
         op: str = "",
         other: Optional[Var] = None,
         type_: Optional[Type] = None,
         flip: bool = False,
@@ -784,28 +794,114 @@
             setattr(state, self.name, value)
 
         setter.__qualname__ = self.get_setter_name()
 
         return setter
 
 
-class ComputedVar(property, Var):
+class ComputedVar(Var, property):
     """A field with computed getters."""
 
     @property
     def name(self) -> str:
         """Get the name of the var.
 
         Returns:
             The name of the var.
         """
         assert self.fget is not None, "Var must have a getter."
         return self.fget.__name__
 
     @property
+    def cache_attr(self) -> str:
+        """Get the attribute used to cache the value on the instance.
+
+        Returns:
+            An attribute name.
+        """
+        return f"__cached_{self.name}"
+
+    def __get__(self, instance, owner):
+        """Get the ComputedVar value.
+
+        If the value is already cached on the instance, return the cached value.
+
+        If this ComputedVar doesn't know what type of object it is attached to, then save
+        a reference as self.__objclass__.
+
+        Args:
+            instance: the instance of the class accessing this computed var.
+            owner: the class that this descriptor is attached to.
+
+        Returns:
+            The value of the var for the given instance.
+        """
+        if not hasattr(self, "__objclass__"):
+            self.__objclass__ = owner
+
+        if instance is None:
+            return super().__get__(instance, owner)
+
+        # handle caching
+        if not hasattr(instance, self.cache_attr):
+            setattr(instance, self.cache_attr, super().__get__(instance, owner))
+        return getattr(instance, self.cache_attr)
+
+    def deps(self, obj: Optional[FunctionType] = None) -> Set[str]:
+        """Determine var dependencies of this ComputedVar.
+
+        Save references to attributes accessed on "self".  Recursively called
+        when the function makes a method call on "self".
+
+        Args:
+            obj: the object to disassemble (defaults to the fget function).
+
+        Returns:
+            A set of variable names accessed by the given obj.
+
+        Raises:
+            RuntimeError: if this ComputedVar does not have a reference to the class
+                it is attached to. (Assign var.__objclass__ manually to workaround.)
+        """
+        d = set()
+        if obj is None:
+            if self.fget is not None:
+                obj = cast(FunctionType, self.fget)
+            else:
+                return set()
+        if not obj.__code__.co_varnames:
+            # cannot reference self if method takes no args
+            return set()
+        self_name = obj.__code__.co_varnames[0]
+        self_is_top_of_stack = False
+        for instruction in dis.get_instructions(obj):
+            if instruction.opname == "LOAD_FAST" and instruction.argval == self_name:
+                self_is_top_of_stack = True
+                continue
+            if self_is_top_of_stack and instruction.opname == "LOAD_ATTR":
+                d.add(instruction.argval)
+            elif self_is_top_of_stack and instruction.opname == "LOAD_METHOD":
+                if not hasattr(self, "__objclass__"):
+                    raise RuntimeError(
+                        f"ComputedVar {self.name!r} is not bound to a State subclass.",
+                    )
+                d.update(self.deps(obj=getattr(self.__objclass__, instruction.argval)))
+            self_is_top_of_stack = False
+        return d
+
+    def mark_dirty(self, instance) -> None:
+        """Mark this ComputedVar as dirty.
+
+        Args:
+            instance: the state instance that needs to recompute the value.
+        """
+        with contextlib.suppress(AttributeError):
+            delattr(instance, self.cache_attr)
+
+    @property
     def type_(self):
         """Get the type of the var.
 
         Returns:
             The type of the var.
         """
         hints = get_type_hints(self.fget)
@@ -984,7 +1080,37 @@
 
         Args:
             args: The args passed.
             kwargs: The kwargs passed.
         """
         super().__delitem__(*args, **kwargs)
         self._reassign_field()
+
+
+class ImportVar(Base):
+    """An import var."""
+
+    # The name of the import tag.
+    tag: Optional[str]
+
+    # whether the import is default or named.
+    is_default: Optional[bool] = False
+
+    # The tag alias.
+    alias: Optional[str] = None
+
+    @property
+    def name(self) -> str:
+        """The name of the import.
+
+        Returns:
+            The name(tag name with alias) of tag.
+        """
+        return self.tag if not self.alias else " as ".join([self.tag, self.alias])  # type: ignore
+
+    def __hash__(self) -> int:
+        """Define a hash function for the import var.
+
+        Returns:
+            The hash of the var.
+        """
+        return hash((self.tag, self.is_default, self.alias))
```

### Comparing `pynecone-0.1.28a2/pynecone/watch.py` & `pynecone-0.1.29a0/pynecone/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.28a2/pyproject.toml` & `pynecone-0.1.29a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.28a2"
+version = "0.1.29a0"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.28a2/PKG-INFO` & `pynecone-0.1.29a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.28a2
+Version: 0.1.29a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

