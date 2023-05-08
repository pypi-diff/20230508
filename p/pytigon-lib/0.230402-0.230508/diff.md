# Comparing `tmp/pytigon-lib-0.230402.tar.gz` & `tmp/pytigon-lib-0.230508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytigon-lib-0.230402.tar", last modified: Sun Apr  2 17:37:44 2023, max compression
+gzip compressed data, was "pytigon-lib-0.230508.tar", last modified: Mon May  8 20:07:03 2023, max compression
```

## Comparing `pytigon-lib-0.230402.tar` & `pytigon-lib-0.230508.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.537065 pytigon-lib-0.230402/
--rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/LICENSE
--rw-rw-r--   0 sch       (1000) sch       (1000)     1116 2023-04-02 17:37:44.537065 pytigon-lib-0.230402/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)       13 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/README.md
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.521064 pytigon-lib-0.230402/pytigon_lib/
--rw-rw-r--   0 sch       (1000) sch       (1000)     3005 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/__init__.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.525065 pytigon-lib-0.230402/pytigon_lib/schandroid/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schandroid/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     7772 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schandroid/android_client.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.525065 pytigon-lib-0.230402/pytigon_lib/schdjangoext/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      582 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/allauth.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1773 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_ihtml.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2062 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_init.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1223 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_manage.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      888 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_settings.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1234 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/email.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5134 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/fastform.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9613 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/fields.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2663 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/formfields.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5543 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/formwidgets.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1665 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/graphql.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/import_from_db.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6144 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/models.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1550 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/oauth_for_graphql.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    16441 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/python_style_template_loader.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5248 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/render.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2523 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/rest_tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4038 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/server.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     7421 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/spreadsheet_render.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1885 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      354 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schdjangoext/widgets.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.525065 pytigon-lib-0.230402/pytigon_lib/schfs/
--rw-rw-r--   0 sch       (1000) sch       (1000)      986 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schfs/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1632 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schfs/tasks.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14885 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schfs/vfstools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.529065 pytigon-lib-0.230402/pytigon_lib/schhtml/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12942 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/atom.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    19894 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/basedc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    16635 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/basehtmltags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12020 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/cairodc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6237 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/css.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13853 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/docxdc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2422 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/html_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2764 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/htmltools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14974 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/htmlviewer.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.529065 pytigon-lib-0.230402/pytigon_lib/schhtml/icss/
--rw-rw-r--   0 sch       (1000) sch       (1000)     6965 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/icss/wiki.icss
--rw-rw-r--   0 sch       (1000) sch       (1000)     1197 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/main.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5643 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/parser.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13718 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/pdfdc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    11680 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/render_helpers.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.529065 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9267 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/atom_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    10781 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/block_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1796 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/css_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2563 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/extra_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    15761 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/p_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2533 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/page_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    25539 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/tags/table_tags.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13671 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/wxdc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9959 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/wxgc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13494 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhtml/xlsxdc.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.529065 pytigon-lib-0.230402/pytigon_lib/schhttptools/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhttptools/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4659 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhttptools/asgi_bridge.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      694 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhttptools/get_oauth2_refresh_token.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    21255 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhttptools/httpclient.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2224 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhttptools/rest_client.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2814 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schhttptools/websocket.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.529065 pytigon-lib-0.230402/pytigon_lib/schindent/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schindent/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8784 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schindent/indent_markdown.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    29893 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schindent/indent_style.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8288 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schindent/indent_tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      890 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schindent/py_to_js.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.533065 pytigon-lib-0.230402/pytigon_lib/schparser/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schparser/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     6553 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schparser/html_parsers.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.533065 pytigon-lib-0.230402/pytigon_lib/schspreadsheet/
--rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schspreadsheet/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    12631 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schspreadsheet/odf_process.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    19135 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schspreadsheet/ooxml_process.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3323 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schspreadsheet/ooxml_tools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.533065 pytigon-lib-0.230402/pytigon_lib/schtable/
--rw-rw-r--   0 sch       (1000) sch       (1000)      733 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtable/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     9070 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtable/dbtable.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5880 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtable/table.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    13468 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtable/vfstable.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.533065 pytigon-lib-0.230402/pytigon_lib/schtasks/
--rw-rw-r--   0 sch       (1000) sch       (1000)        0 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtasks/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3435 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtasks/publish.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2449 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtasks/remote_screen.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    14934 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtasks/schschedule.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1420 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtasks/term_tools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.533065 pytigon-lib-0.230402/pytigon_lib/schtools/
--rw-rw-r--   0 sch       (1000) sch       (1000)      897 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5325 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/cc.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2713 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/createparm.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1671 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/env.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    16079 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/href_action.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3153 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/images.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3304 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/imap4client.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    10973 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/install.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5872 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/install_init.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     1262 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/llvm_exec.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     8367 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/main_paths.py
--rw-rw-r--   0 sch       (1000) sch       (1000)      991 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/platform_info.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4644 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/process.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2535 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/schhtmlgen.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     2540 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/schjson.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3423 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/screenshot.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     5077 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/tools.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4031 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schtools/wiki.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.537065 pytigon-lib-0.230402/pytigon_lib/schviews/
--rw-rw-r--   0 sch       (1000) sch       (1000)    56422 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schviews/__init__.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3313 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schviews/actions.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     7613 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schviews/form_fun.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     3979 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schviews/perms.py
--rw-rw-r--   0 sch       (1000) sch       (1000)     4416 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schviews/tree.py
--rw-rw-r--   0 sch       (1000) sch       (1000)    21901 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/pytigon_lib/schviews/viewtools.py
-drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-04-02 17:37:44.525065 pytigon-lib-0.230402/pytigon_lib.egg-info/
--rw-rw-r--   0 sch       (1000) sch       (1000)     1116 2023-04-02 17:37:44.000000 pytigon-lib-0.230402/pytigon_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sch       (1000) sch       (1000)     3908 2023-04-02 17:37:44.000000 pytigon-lib-0.230402/pytigon_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-04-02 17:37:44.000000 pytigon-lib-0.230402/pytigon_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       95 2023-04-02 17:37:44.000000 pytigon-lib-0.230402/pytigon_lib.egg-info/requires.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       12 2023-04-02 17:37:44.000000 pytigon-lib-0.230402/pytigon_lib.egg-info/top_level.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       95 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/requirements.txt
--rw-rw-r--   0 sch       (1000) sch       (1000)       38 2023-04-02 17:37:44.537065 pytigon-lib-0.230402/setup.cfg
--rw-rw-r--   0 sch       (1000) sch       (1000)     1935 2023-04-02 17:20:16.000000 pytigon-lib-0.230402/setup.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.072782 pytigon-lib-0.230508/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7633 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/LICENSE
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1167 2023-05-08 20:07:03.072782 pytigon-lib-0.230508/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)       13 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/README.md
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.052782 pytigon-lib-0.230508/pytigon_lib/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3326 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/__init__.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.056782 pytigon-lib-0.230508/pytigon_lib/schandroid/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schandroid/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7772 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schandroid/android_client.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.056782 pytigon-lib-0.230508/pytigon_lib/schdjangoext/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      582 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/allauth.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1773 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_ihtml.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2062 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_init.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1223 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_manage.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      888 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_settings.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1234 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/email.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5260 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/fastform.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9613 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/fields.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2663 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/formfields.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5543 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/formwidgets.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1665 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/graphql.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2984 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/import_from_db.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6144 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/models.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1550 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/oauth_for_graphql.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    16441 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/python_style_template_loader.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5248 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/render.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2523 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/rest_tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4038 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/server.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7421 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/spreadsheet_render.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1885 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      354 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schdjangoext/widgets.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.060782 pytigon-lib-0.230508/pytigon_lib/schfs/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      986 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schfs/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1632 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schfs/tasks.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14885 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schfs/vfstools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.060782 pytigon-lib-0.230508/pytigon_lib/schhtml/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12942 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/atom.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    19894 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/basedc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    16635 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/basehtmltags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12020 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/cairodc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6237 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/css.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13853 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/docxdc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2422 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/html_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2764 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/htmltools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14974 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/htmlviewer.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.060782 pytigon-lib-0.230508/pytigon_lib/schhtml/icss/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6965 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/icss/wiki.icss
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1197 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/main.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5643 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/parser.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13718 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/pdfdc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    11680 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/render_helpers.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.064782 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9267 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/atom_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10781 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/block_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1796 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/css_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2563 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/extra_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    15761 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/p_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2533 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/page_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    25539 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/tags/table_tags.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13671 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/wxdc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9959 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/wxgc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13494 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhtml/xlsxdc.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.064782 pytigon-lib-0.230508/pytigon_lib/schhttptools/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhttptools/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4659 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhttptools/asgi_bridge.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      694 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhttptools/get_oauth2_refresh_token.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    21255 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhttptools/httpclient.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2224 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhttptools/rest_client.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2814 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schhttptools/websocket.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.064782 pytigon-lib-0.230508/pytigon_lib/schindent/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schindent/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8784 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schindent/indent_markdown.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    29893 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schindent/indent_style.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8288 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schindent/indent_tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      890 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schindent/py_to_js.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.064782 pytigon-lib-0.230508/pytigon_lib/schparser/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schparser/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     6553 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schparser/html_parsers.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.068782 pytigon-lib-0.230508/pytigon_lib/schspreadsheet/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      737 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schspreadsheet/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    12631 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schspreadsheet/odf_process.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    19135 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schspreadsheet/ooxml_process.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3323 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schspreadsheet/ooxml_tools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.068782 pytigon-lib-0.230508/pytigon_lib/schtable/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      733 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtable/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     9070 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtable/dbtable.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5880 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtable/table.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    13468 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtable/vfstable.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.068782 pytigon-lib-0.230508/pytigon_lib/schtasks/
+-rw-rw-r--   0 sch       (1000) sch       (1000)        0 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtasks/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3435 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtasks/publish.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2449 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtasks/remote_screen.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    14934 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtasks/schschedule.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1420 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtasks/term_tools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.072782 pytigon-lib-0.230508/pytigon_lib/schtools/
+-rw-rw-r--   0 sch       (1000) sch       (1000)      897 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5325 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/cc.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2713 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/createparm.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1671 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/env.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    16079 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/href_action.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3153 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/images.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3304 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/imap4client.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    10973 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/install.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8181 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/install_init.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1262 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/llvm_exec.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     8367 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/main_paths.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)      991 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/platform_info.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4644 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/process.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2535 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/schhtmlgen.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     2540 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/schjson.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3423 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/screenshot.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     5077 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/tools.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4031 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schtools/wiki.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.072782 pytigon-lib-0.230508/pytigon_lib/schviews/
+-rw-rw-r--   0 sch       (1000) sch       (1000)    57500 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schviews/__init__.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3313 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schviews/actions.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     7613 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schviews/form_fun.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3979 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schviews/perms.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)     4416 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schviews/tree.py
+-rw-rw-r--   0 sch       (1000) sch       (1000)    21901 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/pytigon_lib/schviews/viewtools.py
+drwxrwxr-x   0 sch       (1000) sch       (1000)        0 2023-05-08 20:07:03.056782 pytigon-lib-0.230508/pytigon_lib.egg-info/
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1167 2023-05-08 20:07:02.000000 pytigon-lib-0.230508/pytigon_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sch       (1000) sch       (1000)     3908 2023-05-08 20:07:02.000000 pytigon-lib-0.230508/pytigon_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)        1 2023-05-08 20:07:02.000000 pytigon-lib-0.230508/pytigon_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       95 2023-05-08 20:07:02.000000 pytigon-lib-0.230508/pytigon_lib.egg-info/requires.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       12 2023-05-08 20:07:02.000000 pytigon-lib-0.230508/pytigon_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       95 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/requirements.txt
+-rw-rw-r--   0 sch       (1000) sch       (1000)       38 2023-05-08 20:07:03.072782 pytigon-lib-0.230508/setup.cfg
+-rw-rw-r--   0 sch       (1000) sch       (1000)     1985 2023-05-08 20:06:06.000000 pytigon-lib-0.230508/setup.py
```

### Comparing `pytigon-lib-0.230402/LICENSE` & `pytigon-lib-0.230508/LICENSE`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/PKG-INFO` & `pytigon-lib-0.230508/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-lib
-Version: 0.230402
+Version: 0.230508
 Summary: Pytigon library
 Home-page: UNKNOWN
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 License-File: LICENSE
```

### Comparing `pytigon-lib-0.230402/pytigon_lib/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,17 +79,26 @@
         sys.path.append(cfg["ROOT_PATH"])
     if not cfg["PRJ_PATH_ALT"] in sys.path:
         sys.path.append(cfg["PRJ_PATH_ALT"])
 
     p1 = os.path.join(cfg["ROOT_PATH"], "ext_lib")
     p2 = os.path.join(cfg["ROOT_PATH"], "appdata", "plugins")
     p3 = os.path.join(cfg["DATA_PATH"], "plugins")
+    if prj_name:
+        p4 = os.path.join(cfg["DATA_PATH"], prj_name, "syslib")
 
     if not p1 in sys.path:
         sys.path.append(p1)
     if not p2 in sys.path:
         sys.path.append(p2)
     if not p3 in sys.path:
         sys.path.append(p3)
+    if prj_name and not p4 in sys.path:
+        sys.path.append(p4)
+
+    if prj_name:
+        prjlib_path = os.path.join(cfg["DATA_PATH"], prj_name, "prjlib")
+        if not prjlib_path in sys.path:
+            sys.path.append(prjlib_path)
 
 
 #    environ['LD_LIBRARY_PATH'] = os.path.join(cfg['DATA_PATH'], "ext_prg", "tcc")
```

### Comparing `pytigon-lib-0.230402/pytigon_lib/schandroid/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schandroid/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schandroid/android_client.py` & `pytigon-lib-0.230508/pytigon_lib/schandroid/android_client.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/allauth.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/allauth.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_ihtml.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_ihtml.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_init.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_init.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_manage.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_manage.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/django_settings.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/django_settings.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/email.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/email.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/fastform.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/fastform.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,23 +120,32 @@
         else:
             field_type = forms.CharField
             line2 = line
     name, title, required = _get_name_and_title(line2)
     return name, field_type, title, required, kwargs
 
 
-def form_from_str(input_str, init_data={}, base_form_class=forms.Form, prefix=""):
+def form_from_str(
+    input_str,
+    init_data={},
+    base_form_class=forms.Form,
+    prefix="",
+    globals_dict=globals(),
+    locals_dict=locals(),
+):
     if "base_form" in input_str:
         make_form_str = (
             "def make_form_class(base_form, init_data):\n"
             + "\n".join(["    " + pos for pos in input_str.split("\n")])
             + "\n"
         )
-        exec(make_form_str)
-        _Form = locals()["make_form_class"](base_form_class, init_data)
+        d = globals_dict | locals_dict
+        l = {}
+        exec(make_form_str, d, l)
+        _Form = l["make_form_class"](base_form_class, init_data)
         return _Form
     else:
 
         class _Form(base_form_class):
             def __init__(self, *args, **kwargs):
                 super(_Form, self).__init__(*args, **kwargs)
```

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/fields.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/fields.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/formfields.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/formfields.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/formwidgets.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/formwidgets.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/graphql.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/graphql.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/import_from_db.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/import_from_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import types
 import os
 import importlib.abc
 from importlib.machinery import ModuleSpec
+from django.conf import settings
 
 
 class DBModuleLoader(importlib.abc.SourceLoader):
     def get_filename(self, path):
         return path.replace(".", os.sep) + ".dbpy"
 
     def get_data(self, path):
@@ -48,7 +49,44 @@
                 full_path = full_name.replace(".", os.sep) + ".dbpy"
                 return ModuleSpec(full_name, DBModuleLoader(), origin=full_path)
         else:
             return None
 
 
 sys.meta_path.insert(0, DBFinder())
+
+
+class ModuleStruct:
+    def __init__(self, globals_dict, locals_dict):
+        self.__dict__.update(globals_dict)
+        self.__dict__.update(locals_dict)
+
+
+def run_code_from_db_field(
+    src_name, obj, field_name, function_name, locals_dict, globals_dict, **argv
+):
+    field = getattr(obj, field_name)
+    if field:
+        gen_path = os.path.join(settings.DATA_PATH, settings.PRJ_NAME, "syslib")
+        gen_name = src_name.format(**(locals_dict | globals_dict))
+
+        src_file_path = os.path.join(gen_path, gen_name)
+
+        if os.path.exists(src_file_path):
+            field_utf = field.encode("utf-8")
+            file_stats = os.stat(src_file_path)
+            if file_stats.st_size != len(field_utf):
+                with open(src_file_path, "wb") as f:
+                    f.write(field_utf)
+        else:
+            os.makedirs(gen_path, exist_ok=True)
+            with open(src_file_path, "wb") as f:
+                f.write(field.encode("utf-8"))
+
+        x = __import__(gen_name.replace(".py", ""))
+        fun = getattr(x, function_name)
+        return fun(**argv)
+
+        # exec(field, globals(), locals())
+        # return locals()["function_name"](**argv)
+    else:
+        return None
```

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/models.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/models.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/oauth_for_graphql.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/oauth_for_graphql.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/python_style_template_loader.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/python_style_template_loader.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/render.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/render.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/rest_tools.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/rest_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/server.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/server.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/spreadsheet_render.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/spreadsheet_render.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schdjangoext/tools.py` & `pytigon-lib-0.230508/pytigon_lib/schdjangoext/tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schfs/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schfs/tasks.py` & `pytigon-lib-0.230508/pytigon_lib/schfs/tasks.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schfs/vfstools.py` & `pytigon-lib-0.230508/pytigon_lib/schfs/vfstools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/atom.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/atom.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/basedc.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/basedc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/basehtmltags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/basehtmltags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/cairodc.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/cairodc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/css.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/css.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/docxdc.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/docxdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/html_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/html_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/htmltools.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/htmltools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/htmlviewer.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/htmlviewer.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/icss/wiki.icss` & `pytigon-lib-0.230508/pytigon_lib/schhtml/icss/wiki.icss`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/main.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/main.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/parser.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/parser.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/pdfdc.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/pdfdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/render_helpers.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/render_helpers.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/atom_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/atom_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/block_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/block_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/css_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/css_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/extra_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/extra_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/p_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/p_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/page_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/page_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/tags/table_tags.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/tags/table_tags.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/wxdc.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/wxdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/wxgc.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/wxgc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhtml/xlsxdc.py` & `pytigon-lib-0.230508/pytigon_lib/schhtml/xlsxdc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhttptools/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schhttptools/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhttptools/asgi_bridge.py` & `pytigon-lib-0.230508/pytigon_lib/schhttptools/asgi_bridge.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhttptools/get_oauth2_refresh_token.py` & `pytigon-lib-0.230508/pytigon_lib/schhttptools/get_oauth2_refresh_token.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhttptools/httpclient.py` & `pytigon-lib-0.230508/pytigon_lib/schhttptools/httpclient.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhttptools/rest_client.py` & `pytigon-lib-0.230508/pytigon_lib/schhttptools/rest_client.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schhttptools/websocket.py` & `pytigon-lib-0.230508/pytigon_lib/schhttptools/websocket.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schindent/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schindent/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schindent/indent_markdown.py` & `pytigon-lib-0.230508/pytigon_lib/schindent/indent_markdown.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schindent/indent_style.py` & `pytigon-lib-0.230508/pytigon_lib/schindent/indent_style.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schindent/indent_tools.py` & `pytigon-lib-0.230508/pytigon_lib/schindent/indent_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schindent/py_to_js.py` & `pytigon-lib-0.230508/pytigon_lib/schindent/py_to_js.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schparser/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schparser/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schparser/html_parsers.py` & `pytigon-lib-0.230508/pytigon_lib/schparser/html_parsers.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schspreadsheet/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schspreadsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schspreadsheet/odf_process.py` & `pytigon-lib-0.230508/pytigon_lib/schspreadsheet/odf_process.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schspreadsheet/ooxml_process.py` & `pytigon-lib-0.230508/pytigon_lib/schspreadsheet/ooxml_process.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schspreadsheet/ooxml_tools.py` & `pytigon-lib-0.230508/pytigon_lib/schspreadsheet/ooxml_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtable/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schtable/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtable/dbtable.py` & `pytigon-lib-0.230508/pytigon_lib/schtable/dbtable.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtable/table.py` & `pytigon-lib-0.230508/pytigon_lib/schtable/table.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtable/vfstable.py` & `pytigon-lib-0.230508/pytigon_lib/schtable/vfstable.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtasks/publish.py` & `pytigon-lib-0.230508/pytigon_lib/schtasks/publish.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtasks/remote_screen.py` & `pytigon-lib-0.230508/pytigon_lib/schtasks/remote_screen.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtasks/schschedule.py` & `pytigon-lib-0.230508/pytigon_lib/schtasks/schschedule.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtasks/term_tools.py` & `pytigon-lib-0.230508/pytigon_lib/schtasks/term_tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/__init__.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/cc.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/cc.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/createparm.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/createparm.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/env.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/env.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/href_action.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/href_action.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/images.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/images.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/imap4client.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/imap4client.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/install.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/install.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/install_init.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/install_init.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import sys
 from pytigon_lib.schfs import extractall
 import zipfile
 from distutils.dir_util import copy_tree
 import configparser
 from pytigon_lib.schtools.process import py_manage
 from pytigon_lib.schtools.cc import make
+from pytigon_lib.schtools.process import py_run
 
 
 def _mkdir(path, ext=None):
     if ext:
         p = os.path.join(path, ext)
     else:
         p = path
@@ -52,15 +53,68 @@
             cfg2.read(ini2)
             t2 = cfg2["DEFAULT"]["GEN_TIME"]
             if t2 < t1:
                 return True
     return False
 
 
+def pip_install(pip_str, prjlib, confirm=False, upgrade=False):
+    packages = [x.strip() for x in pip_str.split(" ") if x]
+    print("pip install: ", pip_str)
+    exit_code, output_tab, err_tab = py_run(
+        [
+            "-m",
+            "pip",
+            "--disable-pip-version-check",
+            "install",
+            f"--target={prjlib}",
+        ]
+        + (
+            [
+                "--upgrade",
+            ]
+            if upgrade
+            else []
+        )
+        + packages
+    )
+    success = False
+    if output_tab:
+        for pos in output_tab:
+            if pos:
+                print("pip info: ", pos)
+            if "Successfully installed" in pos:
+                success = True
+    if err_tab:
+        for pos in err_tab:
+            if pos:
+                print("pip error: ", pos)
+
+    if success and confirm:
+        with open(os.path.join(prjlib, "install.txt"), "wt") as f:
+            f.write("OK")
+
+
+def upgrade_local_libs():
+    from django.conf import settings
+
+    prjlib = os.path.join(settings.DATA_PATH, settings.PRJ_NAME, "prjlib")
+    config_file = os.path.join(settings.PRJ_PATH, settings.PRJ_NAME, "install.ini")
+    if os.path.exists(config_file):
+        config = configparser.ConfigParser()
+        config.read(config_file)
+        if "DEFAULT" in config:
+            pip_str = config["DEFAULT"].get("PIP", "")
+            if pip_str:
+                pip_install(pip_str, prjlib, confirm=True, upgrade=True)
+
+
 def init(prj, root_path, data_path, prj_path, static_app_path, paths=None):
+    if prj == "_schall":
+        return
     _root_path = os.path.normpath(root_path)
     _data_path = os.path.normpath(data_path)
     _prj_path = os.path.normpath(prj_path)
     _static_app_path = os.path.normpath(static_app_path)
     _base_compiler_path = os.path.join(_data_path, "ext_prg")
     test1 = 0 if os.path.exists(_prj_path) else 1
     test2 = 0 if os.path.exists(_data_path) else 1
@@ -148,16 +202,35 @@
     ]
     for p in _paths:
         _mkdir(_data_path, p)
     if paths:
         for p in paths:
             _mkdir(p)
 
-    prjlib = os.path.join(os.path.join(_prj_path, prj), "prjlib")
+    prjlib = os.path.join(_data_path, prj, "prjlib")
+    if not os.path.exists(prjlib) or not os.path.exists(
+        os.path.join(prjlib, "install.txt")
+    ):
+        if not os.path.exists(prjlib):
+            os.mkdir(prjlib)
+        config_file = os.path.join(prj_path, prj, "install.ini")
+        if os.path.exists(config_file):
+            config = configparser.ConfigParser()
+            config.read(config_file)
+            if "DEFAULT" in config:
+                pip_str = config["DEFAULT"].get("PIP", "")
+                if pip_str:
+                    pip_install(pip_str, prjlib, confirm=True)
+
     if os.path.exists(prjlib):
         if not prjlib in sys.path:
             sys.path.append(prjlib)
         if test1 or test2 or test3:
             ret = make(_data_path, os.path.join(_prj_path, prj), prj)
             if ret:
                 for pos in ret:
                     print(pos)
+    syslib = os.path.join(_data_path, prj, "syslib")
+    if not os.path.exists(syslib):
+        os.makedirs(syslib)
+        with open(os.path.join(syslib, "__init__.py"), "wt") as f:
+            f.write(" ")
```

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/llvm_exec.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/llvm_exec.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/main_paths.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/main_paths.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/platform_info.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/platform_info.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/process.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/process.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/schhtmlgen.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/schhtmlgen.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/schjson.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/schjson.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/screenshot.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/screenshot.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/tools.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/tools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schtools/wiki.py` & `pytigon-lib-0.230508/pytigon_lib/schtools/wiki.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schviews/__init__.py` & `pytigon-lib-0.230508/pytigon_lib/schviews/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,51 +167,82 @@
             return HttpResponse("OK")
         else:
             data = request.POST["data"]
             buf = data.replace("\r\n", "\n")
             # if type(buf)==str:
             #    buf = buf.encode('utf-8')
             obj = model.objects.get(id=pk)
-            setattr(obj, field_edit_name, buf)
+            if "fragment" in request.GET:
+                buf2 = getattr(obj, field_edit_name)
+                if buf2 == None:
+                    buf2 = ""
+                if request.GET["fragment"] == "header":
+                    if "$$$" in buf2:
+                        buf = buf + "$$$" + buf2.split("$$$")[1]
+                elif request.GET["fragment"] == "footer":
+                    buf = buf2.split("$$$")[0] + "$$$" + buf
+                setattr(obj, field_edit_name, buf)
+            else:
+                setattr(obj, field_edit_name, buf)
             save(obj, request, "editor", {"field": field_edit_name})
             return HttpResponse("OK")
     else:
         obj = model.objects.get(id=pk)
         table_name = model._meta.object_name
         txt = getattr(obj, field_edit_name)
+        if txt == None:
+            txt = ""
+        if "fragment" in request.GET:
+            if request.GET["fragment"] == "header":
+                txt = txt.split("$$$")[0]
+            elif request.GET["fragment"] == "footer":
+                if "$$$" in txt:
+                    txt = txt.split("$$$")[1]
+                else:
+                    txt = ""
+
         f = None
         for field in obj._meta.fields:
             if field.name == field_edit_name:
                 f = field
                 break
+
+        x = request.get_full_path().split("?", 1)
+        if len(x) > 1:
+            get_param = "?" + x[1]
+        else:
+            get_param = ""
+
         if field_name:
             save_path = (
                 app
                 + "/table/"
                 + tab
                 + "/"
                 + str(parent_pk)
                 + "/"
                 + table_name
                 + "/"
                 + str(pk)
                 + "/"
                 + field_edit_name
                 + "/py/editor/"
+                + get_param
             )
         else:
             save_path = (
                 app
                 + "/table/"
                 + table_name
                 + "/"
                 + str(pk)
                 + "/"
                 + field_edit_name
                 + "/py/editor/"
+                + get_param
             )
         c = {
             "app": app,
             "tab": table_name,
             "pk": pk,
             "object": obj,
             "field_name": field_edit_name,
```

### Comparing `pytigon-lib-0.230402/pytigon_lib/schviews/actions.py` & `pytigon-lib-0.230508/pytigon_lib/schviews/actions.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schviews/form_fun.py` & `pytigon-lib-0.230508/pytigon_lib/schviews/form_fun.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schviews/perms.py` & `pytigon-lib-0.230508/pytigon_lib/schviews/perms.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schviews/tree.py` & `pytigon-lib-0.230508/pytigon_lib/schviews/tree.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib/schviews/viewtools.py` & `pytigon-lib-0.230508/pytigon_lib/schviews/viewtools.py`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/pytigon_lib.egg-info/PKG-INFO` & `pytigon-lib-0.230508/pytigon_lib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytigon-lib
-Version: 0.230402
+Version: 0.230508
 Summary: Pytigon library
 Home-page: UNKNOWN
 Author: Sławomir Chołaj
 Author-email: slawomir.cholaj@gmail.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3
 License-File: LICENSE
```

### Comparing `pytigon-lib-0.230402/pytigon_lib.egg-info/SOURCES.txt` & `pytigon-lib-0.230508/pytigon_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytigon-lib-0.230402/setup.py` & `pytigon-lib-0.230508/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open("requirements.txt") as f:
     tmp = f.read().strip().split("\n")
     install_requires = [pos for pos in tmp if "://" not in pos]
     dependency_links = [pos for pos in tmp if "://" in pos]
 
 setup(
     name="pytigon-lib",
-    version="0.230402",
+    version="0.230508",
     description="Pytigon library",
     author="Sławomir Chołaj",
     author_email="slawomir.cholaj@gmail.com",
     license="LGPLv3",
     packages=find_packages(),
     package_data={
         "": extra_files,
@@ -41,14 +41,15 @@
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3",
```

