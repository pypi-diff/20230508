# Comparing `tmp/dcoraid-0.9.0.tar.gz` & `tmp/dcoraid-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcoraid-0.9.0.tar", last modified: Thu Dec  9 13:38:32 2021, max compression
+gzip compressed data, was "dcoraid-0.9.1.tar", last modified: Fri Dec 10 19:52:22 2021, max compression
```

## Comparing `dcoraid-0.9.0.tar` & `dcoraid-0.9.1.tar`

### file list

```diff
@@ -1,236 +1,236 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.226426 dcoraid-0.9.0/
--rw-r--r--   0 runner     (501) staff       (20)    11623 2021-12-09 13:38:04.000000 dcoraid-0.9.0/CHANGELOG
--rw-r--r--   0 runner     (501) staff       (20)    35149 2021-12-09 13:38:04.000000 dcoraid-0.9.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      206 2021-12-09 13:38:04.000000 dcoraid-0.9.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2261 2021-12-09 13:38:32.226629 dcoraid-0.9.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1441 2021-12-09 13:38:04.000000 dcoraid-0.9.0/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.139017 dcoraid-0.9.0/dcoraid/
--rw-r--r--   0 runner     (501) staff       (20)      210 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1867 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)     7095 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/_version.py
--rw-r--r--   0 runner     (501) staff       (20)       82 2021-12-09 13:38:14.000000 dcoraid-0.9.0/dcoraid/_version_save.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.143233 dcoraid-0.9.0/dcoraid/api/
--rw-r--r--   0 runner     (501) staff       (20)      459 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/api/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10078 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/api/ckan_api.py
--rw-r--r--   0 runner     (501) staff       (20)     8058 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/api/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)      365 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/api/errors.py
--rw-r--r--   0 runner     (501) staff       (20)     2442 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/cli.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/common.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.144795 dcoraid-0.9.0/dcoraid/dbmodel/
--rw-r--r--   0 runner     (501) staff       (20)       88 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/dbmodel/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7558 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/dbmodel/db_api.py
--rw-r--r--   0 runner     (501) staff       (20)     2727 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/dbmodel/db_core.py
--rw-r--r--   0 runner     (501) staff       (20)     3030 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/dbmodel/extract.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.146378 dcoraid-0.9.0/dcoraid/download/
--rw-r--r--   0 runner     (501) staff       (20)       83 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/download/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    11741 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/download/job.py
--rw-r--r--   0 runner     (501) staff       (20)     6923 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/download/queue.py
--rw-r--r--   0 runner     (501) staff       (20)     1034 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/download/task.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.148114 dcoraid-0.9.0/dcoraid/gui/
--rw-r--r--   0 runner     (501) staff       (20)       40 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1231 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/api.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.151221 dcoraid-0.9.0/dcoraid/gui/dbview/
--rw-r--r--   0 runner     (501) staff       (20)       52 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/dbview/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      686 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/dbview/drag_table_widget.py
--rw-r--r--   0 runner     (501) staff       (20)     4295 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/dbview/filter_base.py
--rw-r--r--   0 runner     (501) staff       (20)     3813 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/dbview/filter_base.ui
--rw-r--r--   0 runner     (501) staff       (20)     7111 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/dbview/filter_chain.py
--rw-r--r--   0 runner     (501) staff       (20)     3056 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/dbview/filter_chain.ui
--rw-r--r--   0 runner     (501) staff       (20)     5695 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/dbview/filter_views.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.152306 dcoraid-0.9.0/dcoraid/gui/download/
--rw-r--r--   0 runner     (501) staff       (20)        0 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/download/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7092 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/download/widget_download.py
--rw-r--r--   0 runner     (501) staff       (20)     1923 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/download/widget_download.ui
--rw-r--r--   0 runner     (501) staff       (20)    13995 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/main.py
--rw-r--r--   0 runner     (501) staff       (20)    16960 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/main.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.153567 dcoraid-0.9.0/dcoraid/gui/maintenance/
--rw-r--r--   0 runner     (501) staff       (20)        0 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/maintenance/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3162 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/maintenance/widget_maintenance.py
--rw-r--r--   0 runner     (501) staff       (20)     1478 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/maintenance/widget_maintenance.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.154899 dcoraid-0.9.0/dcoraid/gui/preferences/
--rw-r--r--   0 runner     (501) staff       (20)       61 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/preferences/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    10219 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/preferences/dlg_preferences.py
--rw-r--r--   0 runner     (501) staff       (20)    10512 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/preferences/dlg_preferences.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.156161 dcoraid-0.9.0/dcoraid/gui/tools/
--rw-r--r--   0 runner     (501) staff       (20)      119 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/tools/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      737 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/tools/bg_thread.py
--rw-r--r--   0 runner     (501) staff       (20)     1069 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/tools/wait_cursor.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.162356 dcoraid-0.9.0/dcoraid/gui/upload/
--rw-r--r--   0 runner     (501) staff       (20)        0 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2942 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/circle_mgr.py
--rw-r--r--   0 runner     (501) staff       (20)    16937 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/dlg_upload.py
--rw-r--r--   0 runner     (501) staff       (20)    23395 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/dlg_upload.ui
--rw-r--r--   0 runner     (501) staff       (20)     1007 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/resource_schema_preset.py
--rw-r--r--   0 runner     (501) staff       (20)     6981 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/resources_model.py
--rw-r--r--   0 runner     (501) staff       (20)     6298 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_schema.py
--rw-r--r--   0 runner     (501) staff       (20)    10317 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_supplement_item.py
--rw-r--r--   0 runner     (501) staff       (20)     6887 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_supplement_item.ui
--rw-r--r--   0 runner     (501) staff       (20)     3219 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_supplement_tags.ui
--rw-r--r--   0 runner     (501) staff       (20)     2660 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_tablecell_actions.py
--rw-r--r--   0 runner     (501) staff       (20)     2915 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_tablecell_actions.ui
--rw-r--r--   0 runner     (501) staff       (20)    14576 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_upload.py
--rw-r--r--   0 runner     (501) staff       (20)     3248 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/upload/widget_upload.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.163703 dcoraid-0.9.0/dcoraid/gui/wizard/
--rw-r--r--   0 runner     (501) staff       (20)     7718 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/wizard/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1806 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/wizard/access_token.py
--rw-r--r--   0 runner     (501) staff       (20)    16217 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/gui/wizard/wizard.ui
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.166748 dcoraid-0.9.0/dcoraid/img/
--rw-r--r--   0 runner     (501) staff       (20)      117 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     8218 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/dcoraid_text.png
--rw-r--r--   0 runner     (501) staff       (20)    13988 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/dcoraid_text.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.167711 dcoraid-0.9.0/dcoraid/img/icon-theme/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.169102 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/
--rw-r--r--   0 runner     (501) staff       (20)     9362 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/COPYING-ICONS
--rw-r--r--   0 runner     (501) staff       (20)    26527 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/COPYING.LIB
--rw-r--r--   0 runner     (501) staff       (20)      271 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/README
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.131430 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.175359 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/
--rw-r--r--   0 runner     (501) staff       (20)      457 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)      766 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      626 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/dialog-close.svg
--rw-r--r--   0 runner     (501) staff       (20)      422 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      504 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      504 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      603 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/document-open-folder.svg
--rw-r--r--   0 runner     (501) staff       (20)      603 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      733 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      577 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/documentinfo.svg
--rw-r--r--   0 runner     (501) staff       (20)      673 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/edit-clear.svg
--rw-r--r--   0 runner     (501) staff       (20)      989 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/gtk-preferences.svg
--rw-r--r--   0 runner     (501) staff       (20)      633 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/messagebox_warning.svg
--rw-r--r--   0 runner     (501) staff       (20)     1060 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/preferences-activities.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.181715 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/
--rw-r--r--   0 runner     (501) staff       (20)      447 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)      962 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      487 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-close.svg
--rw-r--r--   0 runner     (501) staff       (20)      467 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      567 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      567 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      472 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/document-open-folder.svg
--rw-r--r--   0 runner     (501) staff       (20)      472 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      788 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      640 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/documentinfo.svg
--rw-r--r--   0 runner     (501) staff       (20)      663 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/edit-clear.svg
--rw-r--r--   0 runner     (501) staff       (20)      904 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/gtk-preferences.svg
--rw-r--r--   0 runner     (501) staff       (20)      637 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/messagebox_warning.svg
--rw-r--r--   0 runner     (501) staff       (20)     1087 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/preferences-activities.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.188059 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/
--rw-r--r--   0 runner     (501) staff       (20)      481 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)      996 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      521 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-close.svg
--rw-r--r--   0 runner     (501) staff       (20)      501 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      601 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      601 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      506 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/document-open-folder.svg
--rw-r--r--   0 runner     (501) staff       (20)      506 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      822 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      674 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/documentinfo.svg
--rw-r--r--   0 runner     (501) staff       (20)      697 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/edit-clear.svg
--rw-r--r--   0 runner     (501) staff       (20)      938 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/gtk-preferences.svg
--rw-r--r--   0 runner     (501) staff       (20)      671 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/messagebox_warning.svg
--rw-r--r--   0 runner     (501) staff       (20)     1074 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/preferences-activities.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.191746 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/
--rw-r--r--   0 runner     (501) staff       (20)      421 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/application-exit.svg
--rw-r--r--   0 runner     (501) staff       (20)      733 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/dialog-cancel.svg
--rw-r--r--   0 runner     (501) staff       (20)      375 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/dialog-messages.svg
--rw-r--r--   0 runner     (501) staff       (20)      355 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/dialog-ok-apply.svg
--rw-r--r--   0 runner     (501) staff       (20)      355 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/dialog-ok.svg
--rw-r--r--   0 runner     (501) staff       (20)      391 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/document-open.svg
--rw-r--r--   0 runner     (501) staff       (20)      665 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/document-save.svg
--rw-r--r--   0 runner     (501) staff       (20)      728 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/gtk-preferences.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.132406 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.192163 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/16/
--rw-r--r--   0 runner     (501) staff       (20)      529 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/16/dialog-information.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.194025 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/22/
--rw-r--r--   0 runner     (501) staff       (20)      525 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/22/dialog-error.svg
--rw-r--r--   0 runner     (501) staff       (20)      473 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/22/dialog-information.svg
--rw-r--r--   0 runner     (501) staff       (20)      680 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/22/dialog-question.svg
--rw-r--r--   0 runner     (501) staff       (20)      329 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/22/dialog-warning.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.195878 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/24/
--rw-r--r--   0 runner     (501) staff       (20)      559 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/24/dialog-error.svg
--rw-r--r--   0 runner     (501) staff       (20)      507 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/24/dialog-information.svg
--rw-r--r--   0 runner     (501) staff       (20)      714 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/24/dialog-question.svg
--rw-r--r--   0 runner     (501) staff       (20)      363 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/24/dialog-warning.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.197651 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/
--rw-r--r--   0 runner     (501) staff       (20)     2991 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-error.svg
--rw-r--r--   0 runner     (501) staff       (20)     2726 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-information.svg
--rw-r--r--   0 runner     (501) staff       (20)     3645 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-question.svg
--rw-r--r--   0 runner     (501) staff       (20)     2892 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-warning.svg
--rw-r--r--   0 runner     (501) staff       (20)     4881 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/collect_icons.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.198096 dcoraid-0.9.0/dcoraid/img/icon-theme/dcoraid/
--rw-r--r--   0 runner     (501) staff       (20)     7277 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/dcoraid/dcor.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.198510 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/
--rw-r--r--   0 runner     (501) staff       (20)    88456 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/LICENSE.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.214213 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/
--rw-r--r--   0 runner     (501) staff       (20)      602 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/ban.svg
--rw-r--r--   0 runner     (501) staff       (20)      717 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/book.svg
--rw-r--r--   0 runner     (501) staff       (20)      746 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/broom.svg
--rw-r--r--   0 runner     (501) staff       (20)      662 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/check-double.svg
--rw-r--r--   0 runner     (501) staff       (20)      724 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/child.svg
--rw-r--r--   0 runner     (501) staff       (20)      348 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/circle.svg
--rw-r--r--   0 runner     (501) staff       (20)      789 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/clinic-medical.svg
--rw-r--r--   0 runner     (501) staff       (20)      954 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/code-branch.svg
--rw-r--r--   0 runner     (501) staff       (20)     2664 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/cogs.svg
--rw-r--r--   0 runner     (501) staff       (20)      721 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/download.svg
--rw-r--r--   0 runner     (501) staff       (20)      727 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/exclamation-triangle.svg
--rw-r--r--   0 runner     (501) staff       (20)      609 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/eye.svg
--rw-r--r--   0 runner     (501) staff       (20)      484 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/filter.svg
--rw-r--r--   0 runner     (501) staff       (20)      406 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/folder.svg
--rw-r--r--   0 runner     (501) staff       (20)     1017 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/globe.svg
--rw-r--r--   0 runner     (501) staff       (20)      616 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/hat-wizard.svg
--rw-r--r--   0 runner     (501) staff       (20)      646 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/hourglass.svg
--rw-r--r--   0 runner     (501) staff       (20)      587 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/info.svg
--rw-r--r--   0 runner     (501) staff       (20)     1039 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/people-arrows.svg
--rw-r--r--   0 runner     (501) staff       (20)     1427 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/people-carry.svg
--rw-r--r--   0 runner     (501) staff       (20)      923 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/puzzle-piece.svg
--rw-r--r--   0 runner     (501) staff       (20)      621 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/redo.svg
--rw-r--r--   0 runner     (501) staff       (20)      940 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/shipping-fast.svg
--rw-r--r--   0 runner     (501) staff       (20)      470 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/slash.svg
--rw-r--r--   0 runner     (501) staff       (20)      871 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/street-view.svg
--rw-r--r--   0 runner     (501) staff       (20)      569 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/tag.svg
--rw-r--r--   0 runner     (501) staff       (20)      638 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/trash-alt.svg
--rw-r--r--   0 runner     (501) staff       (20)      513 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/trash.svg
--rw-r--r--   0 runner     (501) staff       (20)      818 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/undo.svg
--rw-r--r--   0 runner     (501) staff       (20)      732 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/upload.svg
--rw-r--r--   0 runner     (501) staff       (20)      714 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/user-lock.svg
--rw-r--r--   0 runner     (501) staff       (20)      865 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/user-times.svg
--rw-r--r--   0 runner     (501) staff       (20)      535 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/user.svg
--rw-r--r--   0 runner     (501) staff       (20)      923 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/users.svg
--rw-r--r--   0 runner     (501) staff       (20)      629 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon-theme/index.theme
--rw-r--r--   0 runner     (501) staff       (20)     3426 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon.png
--rw-r--r--   0 runner     (501) staff       (20)     8091 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/icon.svg
--rw-r--r--   0 runner     (501) staff       (20)    32327 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/splash.png
--rw-r--r--   0 runner     (501) staff       (20)    17873 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/img/splash.svg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.216038 dcoraid-0.9.0/dcoraid/upload/
--rw-r--r--   0 runner     (501) staff       (20)      107 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/upload/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    20310 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/upload/job.py
--rw-r--r--   0 runner     (501) staff       (20)    12106 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/upload/queue.py
--rw-r--r--   0 runner     (501) staff       (20)    14928 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/upload/task.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.217322 dcoraid-0.9.0/dcoraid/worker/
--rw-r--r--   0 runner     (501) staff       (20)       77 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/worker/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2773 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/worker/daemon.py
--rw-r--r--   0 runner     (501) staff       (20)     2050 2021-12-09 13:38:04.000000 dcoraid-0.9.0/dcoraid/worker/kthread.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.141579 dcoraid-0.9.0/dcoraid.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2261 2021-12-09 13:38:31.000000 dcoraid-0.9.0/dcoraid.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     8694 2021-12-09 13:38:32.000000 dcoraid-0.9.0/dcoraid.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2021-12-09 13:38:31.000000 dcoraid-0.9.0/dcoraid.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      112 2021-12-09 13:38:31.000000 dcoraid-0.9.0/dcoraid.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)       66 2021-12-09 13:38:31.000000 dcoraid-0.9.0/dcoraid.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2021-12-09 13:38:31.000000 dcoraid-0.9.0/dcoraid.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       73 2021-12-09 13:38:32.227264 dcoraid-0.9.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1411 2021-12-09 13:38:04.000000 dcoraid-0.9.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-09 13:38:32.226016 dcoraid-0.9.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)     4519 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/common.py
--rw-r--r--   0 runner     (501) staff       (20)     4091 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/conftest.py
--rw-r--r--   0 runner     (501) staff       (20)      764 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_access_token.py
--rw-r--r--   0 runner     (501) staff       (20)     5427 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_api_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1135 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_cli_upload_task.py
--rw-r--r--   0 runner     (501) staff       (20)      732 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_common.py
--rw-r--r--   0 runner     (501) staff       (20)     6087 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_dbmodel_api.py
--rw-r--r--   0 runner     (501) staff       (20)     5188 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_download_job.py
--rw-r--r--   0 runner     (501) staff       (20)     5344 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_download_queue.py
--rw-r--r--   0 runner     (501) staff       (20)      637 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_download_task.py
--rw-r--r--   0 runner     (501) staff       (20)    12582 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_gui.py
--rw-r--r--   0 runner     (501) staff       (20)     7541 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_upload_job.py
--rw-r--r--   0 runner     (501) staff       (20)    11662 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_upload_queue.py
--rw-r--r--   0 runner     (501) staff       (20)    21729 2021-12-09 13:38:04.000000 dcoraid-0.9.0/tests/test_upload_task.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.206833 dcoraid-0.9.1/
+-rw-r--r--   0 runner     (501) staff       (20)    11798 2021-12-10 19:51:52.000000 dcoraid-0.9.1/CHANGELOG
+-rw-r--r--   0 runner     (501) staff       (20)    35149 2021-12-10 19:51:52.000000 dcoraid-0.9.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      206 2021-12-10 19:51:52.000000 dcoraid-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     2261 2021-12-10 19:52:22.207028 dcoraid-0.9.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1441 2021-12-10 19:51:52.000000 dcoraid-0.9.1/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:21.989528 dcoraid-0.9.1/dcoraid/
+-rw-r--r--   0 runner     (501) staff       (20)      210 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7095 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)       82 2021-12-10 19:52:02.000000 dcoraid-0.9.1/dcoraid/_version_save.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.002452 dcoraid-0.9.1/dcoraid/api/
+-rw-r--r--   0 runner     (501) staff       (20)      459 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/api/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10078 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/api/ckan_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     8058 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/api/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)      365 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/api/errors.py
+-rw-r--r--   0 runner     (501) staff       (20)     2528 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/common.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.004275 dcoraid-0.9.1/dcoraid/dbmodel/
+-rw-r--r--   0 runner     (501) staff       (20)       88 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/dbmodel/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7558 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/dbmodel/db_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     2727 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/dbmodel/db_core.py
+-rw-r--r--   0 runner     (501) staff       (20)     3030 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/dbmodel/extract.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.022180 dcoraid-0.9.1/dcoraid/download/
+-rw-r--r--   0 runner     (501) staff       (20)       83 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/download/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    11741 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/download/job.py
+-rw-r--r--   0 runner     (501) staff       (20)     6923 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/download/queue.py
+-rw-r--r--   0 runner     (501) staff       (20)     1034 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/download/task.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.024151 dcoraid-0.9.1/dcoraid/gui/
+-rw-r--r--   0 runner     (501) staff       (20)       40 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1231 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/api.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.027555 dcoraid-0.9.1/dcoraid/gui/dbview/
+-rw-r--r--   0 runner     (501) staff       (20)       52 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/dbview/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      686 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/dbview/drag_table_widget.py
+-rw-r--r--   0 runner     (501) staff       (20)     4295 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/dbview/filter_base.py
+-rw-r--r--   0 runner     (501) staff       (20)     3813 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/dbview/filter_base.ui
+-rw-r--r--   0 runner     (501) staff       (20)     7111 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/dbview/filter_chain.py
+-rw-r--r--   0 runner     (501) staff       (20)     3056 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/dbview/filter_chain.ui
+-rw-r--r--   0 runner     (501) staff       (20)     5695 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/dbview/filter_views.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.028784 dcoraid-0.9.1/dcoraid/gui/download/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/download/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7092 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/download/widget_download.py
+-rw-r--r--   0 runner     (501) staff       (20)     1923 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/download/widget_download.ui
+-rw-r--r--   0 runner     (501) staff       (20)    13995 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/main.py
+-rw-r--r--   0 runner     (501) staff       (20)    16960 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/main.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.029870 dcoraid-0.9.1/dcoraid/gui/maintenance/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/maintenance/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3162 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/maintenance/widget_maintenance.py
+-rw-r--r--   0 runner     (501) staff       (20)     1478 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/maintenance/widget_maintenance.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.031224 dcoraid-0.9.1/dcoraid/gui/preferences/
+-rw-r--r--   0 runner     (501) staff       (20)       61 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/preferences/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10219 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/preferences/dlg_preferences.py
+-rw-r--r--   0 runner     (501) staff       (20)    10512 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/preferences/dlg_preferences.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.032539 dcoraid-0.9.1/dcoraid/gui/tools/
+-rw-r--r--   0 runner     (501) staff       (20)      119 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/tools/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      737 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/tools/bg_thread.py
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/tools/wait_cursor.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.065788 dcoraid-0.9.1/dcoraid/gui/upload/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2942 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/circle_mgr.py
+-rw-r--r--   0 runner     (501) staff       (20)    16937 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/dlg_upload.py
+-rw-r--r--   0 runner     (501) staff       (20)    23395 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/dlg_upload.ui
+-rw-r--r--   0 runner     (501) staff       (20)     1007 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/resource_schema_preset.py
+-rw-r--r--   0 runner     (501) staff       (20)     6981 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/resources_model.py
+-rw-r--r--   0 runner     (501) staff       (20)     6298 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_schema.py
+-rw-r--r--   0 runner     (501) staff       (20)    10317 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_supplement_item.py
+-rw-r--r--   0 runner     (501) staff       (20)     6887 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_supplement_item.ui
+-rw-r--r--   0 runner     (501) staff       (20)     3219 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_supplement_tags.ui
+-rw-r--r--   0 runner     (501) staff       (20)     2660 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_tablecell_actions.py
+-rw-r--r--   0 runner     (501) staff       (20)     2915 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_tablecell_actions.ui
+-rw-r--r--   0 runner     (501) staff       (20)    14576 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_upload.py
+-rw-r--r--   0 runner     (501) staff       (20)     3248 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/upload/widget_upload.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.067075 dcoraid-0.9.1/dcoraid/gui/wizard/
+-rw-r--r--   0 runner     (501) staff       (20)     7718 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/wizard/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1806 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/wizard/access_token.py
+-rw-r--r--   0 runner     (501) staff       (20)    16217 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/gui/wizard/wizard.ui
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.070211 dcoraid-0.9.1/dcoraid/img/
+-rw-r--r--   0 runner     (501) staff       (20)      117 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     8218 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/dcoraid_text.png
+-rw-r--r--   0 runner     (501) staff       (20)    13988 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/dcoraid_text.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.071070 dcoraid-0.9.1/dcoraid/img/icon-theme/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.072564 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/
+-rw-r--r--   0 runner     (501) staff       (20)     9362 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/COPYING-ICONS
+-rw-r--r--   0 runner     (501) staff       (20)    26527 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/COPYING.LIB
+-rw-r--r--   0 runner     (501) staff       (20)      271 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/README
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:21.978471 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.090383 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/
+-rw-r--r--   0 runner     (501) staff       (20)      457 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)      766 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      626 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/dialog-close.svg
+-rw-r--r--   0 runner     (501) staff       (20)      422 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      504 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      504 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      603 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/document-open-folder.svg
+-rw-r--r--   0 runner     (501) staff       (20)      603 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      733 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      577 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/documentinfo.svg
+-rw-r--r--   0 runner     (501) staff       (20)      673 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/edit-clear.svg
+-rw-r--r--   0 runner     (501) staff       (20)      989 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/gtk-preferences.svg
+-rw-r--r--   0 runner     (501) staff       (20)      633 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/messagebox_warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1060 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/preferences-activities.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.099502 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/
+-rw-r--r--   0 runner     (501) staff       (20)      447 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)      962 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      487 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-close.svg
+-rw-r--r--   0 runner     (501) staff       (20)      467 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      567 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      567 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      472 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/document-open-folder.svg
+-rw-r--r--   0 runner     (501) staff       (20)      472 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      788 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      640 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/documentinfo.svg
+-rw-r--r--   0 runner     (501) staff       (20)      663 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/edit-clear.svg
+-rw-r--r--   0 runner     (501) staff       (20)      904 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/gtk-preferences.svg
+-rw-r--r--   0 runner     (501) staff       (20)      637 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/messagebox_warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1087 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/preferences-activities.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.126794 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/
+-rw-r--r--   0 runner     (501) staff       (20)      481 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)      996 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      521 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-close.svg
+-rw-r--r--   0 runner     (501) staff       (20)      501 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      601 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      601 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      506 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/document-open-folder.svg
+-rw-r--r--   0 runner     (501) staff       (20)      506 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      822 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      674 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/documentinfo.svg
+-rw-r--r--   0 runner     (501) staff       (20)      697 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/edit-clear.svg
+-rw-r--r--   0 runner     (501) staff       (20)      938 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/gtk-preferences.svg
+-rw-r--r--   0 runner     (501) staff       (20)      671 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/messagebox_warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1074 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/preferences-activities.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.131096 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/
+-rw-r--r--   0 runner     (501) staff       (20)      421 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/application-exit.svg
+-rw-r--r--   0 runner     (501) staff       (20)      733 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/dialog-cancel.svg
+-rw-r--r--   0 runner     (501) staff       (20)      375 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/dialog-messages.svg
+-rw-r--r--   0 runner     (501) staff       (20)      355 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/dialog-ok-apply.svg
+-rw-r--r--   0 runner     (501) staff       (20)      355 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/dialog-ok.svg
+-rw-r--r--   0 runner     (501) staff       (20)      391 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/document-open.svg
+-rw-r--r--   0 runner     (501) staff       (20)      665 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/document-save.svg
+-rw-r--r--   0 runner     (501) staff       (20)      728 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/gtk-preferences.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:21.979547 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.131531 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/16/
+-rw-r--r--   0 runner     (501) staff       (20)      529 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/16/dialog-information.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.133408 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/22/
+-rw-r--r--   0 runner     (501) staff       (20)      525 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/22/dialog-error.svg
+-rw-r--r--   0 runner     (501) staff       (20)      473 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/22/dialog-information.svg
+-rw-r--r--   0 runner     (501) staff       (20)      680 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/22/dialog-question.svg
+-rw-r--r--   0 runner     (501) staff       (20)      329 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/22/dialog-warning.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.148233 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/24/
+-rw-r--r--   0 runner     (501) staff       (20)      559 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/24/dialog-error.svg
+-rw-r--r--   0 runner     (501) staff       (20)      507 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/24/dialog-information.svg
+-rw-r--r--   0 runner     (501) staff       (20)      714 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/24/dialog-question.svg
+-rw-r--r--   0 runner     (501) staff       (20)      363 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/24/dialog-warning.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.150239 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/
+-rw-r--r--   0 runner     (501) staff       (20)     2991 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-error.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2726 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-information.svg
+-rw-r--r--   0 runner     (501) staff       (20)     3645 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-question.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2892 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-warning.svg
+-rw-r--r--   0 runner     (501) staff       (20)     4881 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/collect_icons.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.150612 dcoraid-0.9.1/dcoraid/img/icon-theme/dcoraid/
+-rw-r--r--   0 runner     (501) staff       (20)     7277 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/dcoraid/dcor.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.150985 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/
+-rw-r--r--   0 runner     (501) staff       (20)    88456 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/LICENSE.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.186382 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/
+-rw-r--r--   0 runner     (501) staff       (20)      602 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/ban.svg
+-rw-r--r--   0 runner     (501) staff       (20)      717 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/book.svg
+-rw-r--r--   0 runner     (501) staff       (20)      746 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/broom.svg
+-rw-r--r--   0 runner     (501) staff       (20)      662 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/check-double.svg
+-rw-r--r--   0 runner     (501) staff       (20)      724 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/child.svg
+-rw-r--r--   0 runner     (501) staff       (20)      348 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/circle.svg
+-rw-r--r--   0 runner     (501) staff       (20)      789 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/clinic-medical.svg
+-rw-r--r--   0 runner     (501) staff       (20)      954 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/code-branch.svg
+-rw-r--r--   0 runner     (501) staff       (20)     2664 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/cogs.svg
+-rw-r--r--   0 runner     (501) staff       (20)      721 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/download.svg
+-rw-r--r--   0 runner     (501) staff       (20)      727 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/exclamation-triangle.svg
+-rw-r--r--   0 runner     (501) staff       (20)      609 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/eye.svg
+-rw-r--r--   0 runner     (501) staff       (20)      484 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/filter.svg
+-rw-r--r--   0 runner     (501) staff       (20)      406 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/folder.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1017 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/globe.svg
+-rw-r--r--   0 runner     (501) staff       (20)      616 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/hat-wizard.svg
+-rw-r--r--   0 runner     (501) staff       (20)      646 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/hourglass.svg
+-rw-r--r--   0 runner     (501) staff       (20)      587 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/info.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1039 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/people-arrows.svg
+-rw-r--r--   0 runner     (501) staff       (20)     1427 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/people-carry.svg
+-rw-r--r--   0 runner     (501) staff       (20)      923 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/puzzle-piece.svg
+-rw-r--r--   0 runner     (501) staff       (20)      621 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/redo.svg
+-rw-r--r--   0 runner     (501) staff       (20)      940 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/shipping-fast.svg
+-rw-r--r--   0 runner     (501) staff       (20)      470 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/slash.svg
+-rw-r--r--   0 runner     (501) staff       (20)      871 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/street-view.svg
+-rw-r--r--   0 runner     (501) staff       (20)      569 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/tag.svg
+-rw-r--r--   0 runner     (501) staff       (20)      638 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/trash-alt.svg
+-rw-r--r--   0 runner     (501) staff       (20)      513 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/trash.svg
+-rw-r--r--   0 runner     (501) staff       (20)      818 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/undo.svg
+-rw-r--r--   0 runner     (501) staff       (20)      732 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/upload.svg
+-rw-r--r--   0 runner     (501) staff       (20)      714 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/user-lock.svg
+-rw-r--r--   0 runner     (501) staff       (20)      865 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/user-times.svg
+-rw-r--r--   0 runner     (501) staff       (20)      535 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/user.svg
+-rw-r--r--   0 runner     (501) staff       (20)      923 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/users.svg
+-rw-r--r--   0 runner     (501) staff       (20)      629 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon-theme/index.theme
+-rw-r--r--   0 runner     (501) staff       (20)     3426 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon.png
+-rw-r--r--   0 runner     (501) staff       (20)     8091 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/icon.svg
+-rw-r--r--   0 runner     (501) staff       (20)    32327 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/splash.png
+-rw-r--r--   0 runner     (501) staff       (20)    17873 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/img/splash.svg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.188374 dcoraid-0.9.1/dcoraid/upload/
+-rw-r--r--   0 runner     (501) staff       (20)      107 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/upload/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    20310 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/upload/job.py
+-rw-r--r--   0 runner     (501) staff       (20)    12106 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/upload/queue.py
+-rw-r--r--   0 runner     (501) staff       (20)    14928 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/upload/task.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.189610 dcoraid-0.9.1/dcoraid/worker/
+-rw-r--r--   0 runner     (501) staff       (20)       77 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/worker/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2773 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/worker/daemon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2050 2021-12-10 19:51:52.000000 dcoraid-0.9.1/dcoraid/worker/kthread.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.000691 dcoraid-0.9.1/dcoraid.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2261 2021-12-10 19:52:21.000000 dcoraid-0.9.1/dcoraid.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     8694 2021-12-10 19:52:21.000000 dcoraid-0.9.1/dcoraid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2021-12-10 19:52:21.000000 dcoraid-0.9.1/dcoraid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      112 2021-12-10 19:52:21.000000 dcoraid-0.9.1/dcoraid.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)       66 2021-12-10 19:52:21.000000 dcoraid-0.9.1/dcoraid.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2021-12-10 19:52:21.000000 dcoraid-0.9.1/dcoraid.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       73 2021-12-10 19:52:22.207623 dcoraid-0.9.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1411 2021-12-10 19:51:52.000000 dcoraid-0.9.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2021-12-10 19:52:22.206442 dcoraid-0.9.1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     4556 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/common.py
+-rw-r--r--   0 runner     (501) staff       (20)     4091 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner     (501) staff       (20)      764 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_access_token.py
+-rw-r--r--   0 runner     (501) staff       (20)     5427 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_api_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1149 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_cli_upload_task.py
+-rw-r--r--   0 runner     (501) staff       (20)      732 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_common.py
+-rw-r--r--   0 runner     (501) staff       (20)     6087 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_dbmodel_api.py
+-rw-r--r--   0 runner     (501) staff       (20)     5188 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_download_job.py
+-rw-r--r--   0 runner     (501) staff       (20)     5344 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_download_queue.py
+-rw-r--r--   0 runner     (501) staff       (20)      637 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_download_task.py
+-rw-r--r--   0 runner     (501) staff       (20)    12582 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_gui.py
+-rw-r--r--   0 runner     (501) staff       (20)     7541 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_upload_job.py
+-rw-r--r--   0 runner     (501) staff       (20)    11662 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_upload_queue.py
+-rw-r--r--   0 runner     (501) staff       (20)    21729 2021-12-10 19:51:52.000000 dcoraid-0.9.1/tests/test_upload_task.py
```

### Comparing `dcoraid-0.9.0/CHANGELOG` & `dcoraid-0.9.1/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.9.1
+ - fix: don't print upload job when upload is completed in CLI
+ - fix: daemonize background thread in CLI dcoraid-upload-task
+ - setup: bump dclab from 0.38.2 to 0.39.3
 0.9.0
  - feat: add CLI command dcoraid-upload-task for uploading individual
    tasks from the command line, bypassing the GUI (#37)
 0.8.6:
  - tests: did not run on Windows
 0.8.5
  - enh: introduce APIOutdatedError (server response)
```

### Comparing `dcoraid-0.9.0/LICENSE` & `dcoraid-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/PKG-INFO` & `dcoraid-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcoraid
-Version: 0.9.0
+Version: 0.9.1
 Summary: GUI for managing data on DCOR
 Home-page: https://github.com/DCOR-dev/DCOR-Aid
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v3
 Description: |DCOR-Aid|
         ==========
```

### Comparing `dcoraid-0.9.0/README.rst` & `dcoraid-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/__main__.py` & `dcoraid-0.9.1/dcoraid/__main__.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/_version.py` & `dcoraid-0.9.1/dcoraid/_version.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/api/ckan_api.py` & `dcoraid-0.9.1/dcoraid/api/ckan_api.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/api/dataset.py` & `dcoraid-0.9.1/dcoraid/api/dataset.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/cli.py` & `dcoraid-0.9.1/dcoraid/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         newline = True
         time.sleep(1)
     if newline:
         # Only print new line if we printed something before.
         print("")
 
 
-def upload_task(path_task=None, server=None, api_key=None):
+def upload_task(path_task=None, server=None, api_key=None, ret_job=False):
     """Upload a .dcoraid-task file to a DCOR instance"""
     if path_task is None or server is None or api_key is None:
         parser = upload_task_parser()
         args = parser.parse_args()
         path_task = args.path_task
         server = args.server
         api_key = args.api_key
@@ -39,22 +39,24 @@
     print(f"Dataset ID is {uj.dataset_id}.")
     print("Compressing resources.")
     uj.task_compress_resources()
     print("Uploading resources.")
     # thread that prints the upload progress
     monitor_thread = threading.Thread(target=monitor_upload_progress,
                                       name="Upload Monitor",
-                                      args=(uj,))
+                                      args=(uj,),
+                                      daemon=True)
     monitor_thread.start()
     uj.task_upload_resources()
     monitor_thread.join()
     print("Verifying upload.")
     uj.task_verify_resources()
     print("Done.")
-    return uj
+    if ret_job:
+        return uj
 
 
 def upload_task_parser():
     descr = (
         "Upload a .dcoraid-task file to a DCOR instance. Example usage::\n"
         + "\n    dcoraid-upload-task upload_job.dcoraid-task "
         + "dcor-dev.mpl.mpg.de eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJqdGkiO"
```

### Comparing `dcoraid-0.9.0/dcoraid/common.py` & `dcoraid-0.9.1/dcoraid/common.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/dbmodel/db_api.py` & `dcoraid-0.9.1/dcoraid/dbmodel/db_api.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/dbmodel/db_core.py` & `dcoraid-0.9.1/dcoraid/dbmodel/db_core.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/dbmodel/extract.py` & `dcoraid-0.9.1/dcoraid/dbmodel/extract.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/download/job.py` & `dcoraid-0.9.1/dcoraid/download/job.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/download/queue.py` & `dcoraid-0.9.1/dcoraid/download/queue.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/download/task.py` & `dcoraid-0.9.1/dcoraid/download/task.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/api.py` & `dcoraid-0.9.1/dcoraid/gui/api.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/dbview/drag_table_widget.py` & `dcoraid-0.9.1/dcoraid/gui/dbview/drag_table_widget.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/dbview/filter_base.py` & `dcoraid-0.9.1/dcoraid/gui/dbview/filter_base.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/dbview/filter_base.ui` & `dcoraid-0.9.1/dcoraid/gui/dbview/filter_base.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/dbview/filter_chain.py` & `dcoraid-0.9.1/dcoraid/gui/dbview/filter_chain.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/dbview/filter_chain.ui` & `dcoraid-0.9.1/dcoraid/gui/dbview/filter_chain.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/dbview/filter_views.py` & `dcoraid-0.9.1/dcoraid/gui/dbview/filter_views.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/download/widget_download.py` & `dcoraid-0.9.1/dcoraid/gui/download/widget_download.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/download/widget_download.ui` & `dcoraid-0.9.1/dcoraid/gui/download/widget_download.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/main.py` & `dcoraid-0.9.1/dcoraid/gui/main.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/main.ui` & `dcoraid-0.9.1/dcoraid/gui/main.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/maintenance/widget_maintenance.py` & `dcoraid-0.9.1/dcoraid/gui/maintenance/widget_maintenance.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/maintenance/widget_maintenance.ui` & `dcoraid-0.9.1/dcoraid/gui/maintenance/widget_maintenance.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/preferences/dlg_preferences.py` & `dcoraid-0.9.1/dcoraid/gui/preferences/dlg_preferences.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/preferences/dlg_preferences.ui` & `dcoraid-0.9.1/dcoraid/gui/preferences/dlg_preferences.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/tools/bg_thread.py` & `dcoraid-0.9.1/dcoraid/gui/tools/bg_thread.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/tools/wait_cursor.py` & `dcoraid-0.9.1/dcoraid/gui/tools/wait_cursor.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/circle_mgr.py` & `dcoraid-0.9.1/dcoraid/gui/upload/circle_mgr.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/dlg_upload.py` & `dcoraid-0.9.1/dcoraid/gui/upload/dlg_upload.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/dlg_upload.ui` & `dcoraid-0.9.1/dcoraid/gui/upload/dlg_upload.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/resource_schema_preset.py` & `dcoraid-0.9.1/dcoraid/gui/upload/resource_schema_preset.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/resources_model.py` & `dcoraid-0.9.1/dcoraid/gui/upload/resources_model.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_schema.py` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_schema.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_supplement_item.py` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_supplement_item.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_supplement_item.ui` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_supplement_item.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_supplement_tags.ui` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_supplement_tags.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_tablecell_actions.py` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_tablecell_actions.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_tablecell_actions.ui` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_tablecell_actions.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_upload.py` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_upload.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/upload/widget_upload.ui` & `dcoraid-0.9.1/dcoraid/gui/upload/widget_upload.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/wizard/__init__.py` & `dcoraid-0.9.1/dcoraid/gui/wizard/__init__.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/wizard/access_token.py` & `dcoraid-0.9.1/dcoraid/gui/wizard/access_token.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/gui/wizard/wizard.ui` & `dcoraid-0.9.1/dcoraid/gui/wizard/wizard.ui`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/dcoraid_text.png` & `dcoraid-0.9.1/dcoraid/img/dcoraid_text.png`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/dcoraid_text.svg` & `dcoraid-0.9.1/dcoraid/img/dcoraid_text.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/COPYING-ICONS` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/COPYING-ICONS`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/COPYING.LIB` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/COPYING.LIB`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/dialog-cancel.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/dialog-close.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/dialog-close.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/document-open-folder.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/document-open-folder.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/document-open.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/document-open.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/document-save.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/document-save.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/documentinfo.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/documentinfo.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/edit-clear.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/gtk-preferences.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/messagebox_warning.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/messagebox_warning.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/16/preferences-activities.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/16/preferences-activities.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-cancel.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok-apply.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/document-save.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/document-save.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/documentinfo.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/documentinfo.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/edit-clear.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/gtk-preferences.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/messagebox_warning.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/messagebox_warning.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/22/preferences-activities.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/22/preferences-activities.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-cancel.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-close.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-close.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok-apply.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/document-save.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/document-save.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/documentinfo.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/documentinfo.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/edit-clear.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/gtk-preferences.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/messagebox_warning.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/messagebox_warning.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/24/preferences-activities.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/24/preferences-activities.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/dialog-cancel.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/document-save.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/document-save.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/actions/32/gtk-preferences.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/actions/32/gtk-preferences.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/16/dialog-information.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/16/dialog-information.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/22/dialog-error.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/22/dialog-error.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/22/dialog-question.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/22/dialog-question.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/24/dialog-error.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/24/dialog-error.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/24/dialog-question.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/24/dialog-question.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-error.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-error.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-information.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-information.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-question.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-question.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/breeze/status/64/dialog-warning.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/breeze/status/64/dialog-warning.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/collect_icons.py` & `dcoraid-0.9.1/dcoraid/img/icon-theme/collect_icons.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/dcoraid/dcor.png` & `dcoraid-0.9.1/dcoraid/img/icon-theme/dcoraid/dcor.png`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/LICENSE.txt` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/ban.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/ban.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/book.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/book.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/broom.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/broom.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/check-double.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/check-double.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/child.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/child.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/clinic-medical.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/clinic-medical.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/code-branch.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/code-branch.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/cogs.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/cogs.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/download.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/download.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/exclamation-triangle.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/exclamation-triangle.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/eye.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/eye.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/globe.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/globe.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/hat-wizard.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/hat-wizard.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/hourglass.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/hourglass.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/info.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/info.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/people-arrows.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/people-arrows.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/people-carry.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/people-carry.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/puzzle-piece.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/redo.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/redo.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/shipping-fast.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/shipping-fast.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/street-view.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/street-view.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/tag.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/tag.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/trash-alt.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/trash-alt.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/trash.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/trash.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/undo.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/undo.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/upload.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/upload.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/user-lock.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/user-lock.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/user-times.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/user-times.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/user.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/user.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/fontawesome/solid/users.svg` & `dcoraid-0.9.1/dcoraid/img/icon-theme/fontawesome/solid/users.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon-theme/index.theme` & `dcoraid-0.9.1/dcoraid/img/icon-theme/index.theme`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon.png` & `dcoraid-0.9.1/dcoraid/img/icon.png`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/icon.svg` & `dcoraid-0.9.1/dcoraid/img/icon.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/splash.png` & `dcoraid-0.9.1/dcoraid/img/splash.png`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/img/splash.svg` & `dcoraid-0.9.1/dcoraid/img/splash.svg`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/upload/job.py` & `dcoraid-0.9.1/dcoraid/upload/job.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/upload/queue.py` & `dcoraid-0.9.1/dcoraid/upload/queue.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/upload/task.py` & `dcoraid-0.9.1/dcoraid/upload/task.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/worker/daemon.py` & `dcoraid-0.9.1/dcoraid/worker/daemon.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid/worker/kthread.py` & `dcoraid-0.9.1/dcoraid/worker/kthread.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/dcoraid.egg-info/PKG-INFO` & `dcoraid-0.9.1/dcoraid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcoraid
-Version: 0.9.0
+Version: 0.9.1
 Summary: GUI for managing data on DCOR
 Home-page: https://github.com/DCOR-dev/DCOR-Aid
 Author: Paul Müller
 Author-email: dev@craban.de
 License: GPL v3
 Description: |DCOR-Aid|
         ==========
```

### Comparing `dcoraid-0.9.0/dcoraid.egg-info/SOURCES.txt` & `dcoraid-0.9.1/dcoraid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/setup.py` & `dcoraid-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     packages=find_packages(),
     package_dir={name: name},
     include_package_data=True,
     license="GPL v3",
     description=description,
     long_description=open('README.rst').read() if exists('README.rst') else '',
     install_requires=[
-        "dclab[dcor]==0.38.2",  # pin for triage
+        "dclab[dcor]==0.39.3",  # pin for triage
         "requests>=2.13",
         "requests_toolbelt",  # multipart uploads with progress
         ],
     extras_require={
         "GUI": ["pyqt5"],
         },
     python_requires='>=3.8, <4',
```

### Comparing `dcoraid-0.9.0/tests/common.py` & `dcoraid-0.9.1/tests/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,23 +63,23 @@
     joblist = UploadQueue(api=api)
     joblist.new_job(dataset_id=data["id"],
                     paths=[dpath])
     wait_for_job(joblist, data["id"])
     return api.get("package_show", id=data["id"])
 
 
-def make_upload_task(task_id=None,
+def make_upload_task(task_id=True,  # tester may pass `None` to disable
                      dataset_id=None,
                      dataset_dict=True,
                      resource_paths=[dpath],
                      resource_names=["gorgonzola.rtdc"],
                      resource_supplements=None,
                      ):
     """Return path to example task file"""
-    if task_id is None:
+    if task_id is True:
         task_id = str(uuid.uuid4())
     if dataset_dict and not isinstance(dataset_dict, dict):
         dataset_dict = make_dataset_dict(hint="task_test")
     if dataset_dict and dataset_id is None:
         dataset_id = dataset_dict.get("id")
     td = pathlib.Path(tempfile.mkdtemp(prefix="task_"))
     # copy resources there
```

### Comparing `dcoraid-0.9.0/tests/conftest.py` & `dcoraid-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_access_token.py` & `dcoraid-0.9.1/tests/test_access_token.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_api_dataset.py` & `dcoraid-0.9.1/tests/test_api_dataset.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_cli_upload_task.py` & `dcoraid-0.9.1/tests/test_cli_upload_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from common import get_api, make_upload_task
 
 
 def test_cli_basic():
     path_task = make_upload_task(resource_names=["cli_upload.rtdc"])
     api = get_api()
-    uj = cli.upload_task(path_task, api.server, api.api_key)
+    uj = cli.upload_task(path_task, api.server, api.api_key, ret_job=True)
     pkg_dict = api.get("package_show", id=uj.dataset_id)
     assert pkg_dict["resources"][0]["name"] == "cli_upload.rtdc"
 
 
 @pytest.mark.parametrize("entry,emsg",
                          [["license_id", "Please choose a license_id"],
                           ["owner_org", "A circle must be provided"],
```

### Comparing `dcoraid-0.9.0/tests/test_common.py` & `dcoraid-0.9.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_dbmodel_api.py` & `dcoraid-0.9.1/tests/test_dbmodel_api.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_download_job.py` & `dcoraid-0.9.1/tests/test_download_job.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_download_queue.py` & `dcoraid-0.9.1/tests/test_download_queue.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_download_task.py` & `dcoraid-0.9.1/tests/test_download_task.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_gui.py` & `dcoraid-0.9.1/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_upload_job.py` & `dcoraid-0.9.1/tests/test_upload_job.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_upload_queue.py` & `dcoraid-0.9.1/tests/test_upload_queue.py`

 * *Files identical despite different names*

### Comparing `dcoraid-0.9.0/tests/test_upload_task.py` & `dcoraid-0.9.1/tests/test_upload_task.py`

 * *Files identical despite different names*

