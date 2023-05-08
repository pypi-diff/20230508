# Comparing `tmp/docassemble.demo-1.4.8.tar.gz` & `tmp/docassemble.demo-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.demo-1.4.8.tar", last modified: Thu Aug 25 13:37:24 2022, max compression
+gzip compressed data, was "docassemble.demo-1.4.9.tar", last modified: Sat Sep 10 18:15:55 2022, max compression
```

## Comparing `docassemble.demo-1.4.8.tar` & `docassemble.demo-1.4.9.tar`

### file list

```diff
@@ -1,671 +1,672 @@
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.201667 docassemble.demo-1.4.8/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:54.000000 docassemble.demo-1.4.8/MANIFEST.in
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      664 2022-08-25 13:37:24.201667 docassemble.demo-1.4.8/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.149667 docassemble.demo-1.4.8/docassemble/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      154 2015-04-16 10:10:01.000000 docassemble.demo-1.4.8/docassemble/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.153667 docassemble.demo-1.4.8/docassemble/demo/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       22 2022-08-25 13:37:07.000000 docassemble.demo-1.4.8/docassemble/demo/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.153667 docassemble.demo-1.4.8/docassemble/demo/alembic/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       38 2019-08-18 19:33:12.000000 docassemble.demo-1.4.8/docassemble/demo/alembic/README
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2125 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/alembic/env.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      494 2019-08-18 19:33:12.000000 docassemble.demo-1.4.8/docassemble/demo/alembic/script.py.mako
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1647 2019-08-18 19:33:12.000000 docassemble.demo-1.4.8/docassemble/demo/alembic.ini
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      881 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/attorney.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1874 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/calendar.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      935 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/cards.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      223 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/change_suffix.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14857 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/companydb.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.149667 docassemble.demo-1.4.8/docassemble/demo/data/
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.153667 docassemble.demo-1.4.8/docassemble/demo/data/objects/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1658 2016-08-10 02:21:26.000000 docassemble.demo-1.4.8/docassemble/demo/data/objects/organizations.yml
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.157667 docassemble.demo-1.4.8/docassemble/demo/data/questions/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      314 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/animal.yml
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.157667 docassemble.demo-1.4.8/docassemble/demo/data/questions/bestnumber/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      258 2019-03-03 17:43:24.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/bestnumber/code.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      378 2015-11-11 15:10:56.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/bestnumber/en.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      384 2015-11-11 15:10:41.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/bestnumber/es.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       51 2015-11-11 14:48:01.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/bestnumber/interview.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    16447 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/conflict_check.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1580 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/demo-basic-questions-address.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2541 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/demo-basic-questions-name.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      243 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/demo-basic-questions.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      256 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/event-role-event.yml
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.169667 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      403 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/ab-test.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1374 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/advocate.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1788 2022-03-26 01:52:09.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/ajax.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      737 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/all-mandatory.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1987 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/background-tail.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      388 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/bates-number.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      438 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/bootstrap-theme.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      721 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/branch-mandatory.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      827 2022-07-28 22:47:53.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/button-checkboxes.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2901 2022-04-21 10:18:19.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/calendar.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       20 2022-06-08 14:37:11.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/cards.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1563 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/clauses.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1810 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/collate.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9799 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/companies.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      721 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/complete-attribute-method.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      982 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/context-code.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      983 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/context-manual.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      843 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/context.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1484 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/counter.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4202 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/courtfile.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6107 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/custody.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      370 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/customdate.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3302 2022-04-19 10:46:18.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/daglobal.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1987 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/demo-multi-sign-2.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1735 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/demo-multi-sign.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4239 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/demo-with-basic-questions.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      835 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/dependency-demo-code.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      564 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/dependency-demo.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      535 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/discovery.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      695 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/docxproperties.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1469 2022-04-30 13:16:43.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/duplicate.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1435 2022-06-08 18:50:38.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/explain.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      381 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/fish-example.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      907 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/flags.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1320 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/food-with-sig.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      402 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/fruits-database.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      815 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/generic-document.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      337 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/get-time.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2433 2022-04-19 10:46:18.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/globalprofile.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2433 2022-04-19 10:46:18.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/globalprofile2.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1795 2022-04-19 23:39:18.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/globalprofile3.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      950 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-drive.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1068 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-sheet-2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1203 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-sheet-3.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      998 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-sheet.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      737 2022-06-08 14:47:21.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/graph.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1283 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/harry-potter-or-heidegger.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1441 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/hook-on-gather.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      969 2022-03-26 00:36:25.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/indexdemo.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      598 2022-03-26 01:45:11.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/indexdemoquery.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2694 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/interview_in_interview.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       81 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/jinjayaml-included.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      709 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/jinjayaml.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1071 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/jsondemo.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      589 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/life_story.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2739 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/macros.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      598 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background-2.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      628 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      504 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/make-ocr-pdf.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1307 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/markdown-template.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      567 2021-11-05 23:59:36.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/ml-export-playground.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6799 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/multi-signature.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2631 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/multi-user.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1817 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/navbar-language.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1736 2022-05-17 10:26:00.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/nested-list-docx-table.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2983 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/new-or-existing.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1397 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/oauth-test-2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1276 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/oauth-test-3.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1340 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/oauth-test-4.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      492 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/oauth-test.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2115 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/object-checkboxes-copy.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      940 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/object-checkboxes-custom.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      453 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/objects-from-file-dadict.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      736 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/objects-from-file-gather.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      394 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/objects-from-file-json.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      520 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/objects-from-file-template.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      411 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/objects-from-file.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      432 2022-03-05 21:44:03.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/overlay-pdf-multi.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      616 2022-03-05 21:34:31.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/overlay-pdf.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1272 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/phone-number-2.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1119 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/phone-number.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      646 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/predict-activity-activity.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      634 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/predict-activity.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      355 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/predict-happy-sad-area.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      351 2021-12-27 04:59:09.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/predict-happy-sad.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      760 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/prevent-dependency-satisfaction.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1736 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/preview.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2201 2022-05-16 03:02:48.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/primary-interview.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1005 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/progressive-disclosure.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      727 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-dom.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      863 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-hidden.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      684 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-log.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      634 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-script.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      429 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/questionless.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      579 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/quotes-in-code.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1925 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/random-forest-interview.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1268 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/random-forest.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      433 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/raw-data-example.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      455 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/raw.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1040 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/realtimegd.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      963 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/realtimegd2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1256 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/redact-docx.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1743 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/redact-pdf.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      871 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/repeatable.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      188 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/report-version.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      304 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/run-python-module-2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      288 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/run-python-module-3.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      431 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/run-python-module-tests.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      290 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/run-python-module.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2095 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/save-continue-later.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      371 2022-05-16 00:00:33.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/secondary-interview.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      858 2022-04-09 12:56:16.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/setparts.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3025 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/sign.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2234 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signature-diversion.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1986 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signature-preview.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      776 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signature-template.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25366 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signdoc.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      811 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/single-code.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      749 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/snapshot.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1436 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/someone-already-mentioned.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      878 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/stage-one.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      601 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/stage-two.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1426 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/subdoc-params.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/subdocument.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      485 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/tagged-pdf.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1317 2022-06-07 23:52:50.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testcards.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      680 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testcooking.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1296 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testdatabase.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1394 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testgeolocate.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      222 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testssn.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      738 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/translation.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      593 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/turnips-worms.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1801 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/universal-document.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      772 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/update-references.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      441 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/upload-file-size.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      625 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/validation-code.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      456 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/validation-test-two.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      455 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/validation-test.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      540 2022-04-09 13:22:47.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/watermark.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      651 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/wc_common.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      991 2021-11-05 23:59:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/wc_side_of_bed.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       72 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/hello.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      156 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/hello2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      478 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/hello3.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      714 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/hello4.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      901 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/hello5.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      594 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/hello6.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      299 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/hello7.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      340 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/income.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      266 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/interview-about-flowers.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      257 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/interview-about-fruit.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      287 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/interview-about-vegetables.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      739 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/list.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    39692 2022-04-30 15:49:50.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/questions.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2640 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/roletest.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1240 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/roletestmany.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      101 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/sample-function.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      127 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/samplequestion.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      181 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/samplesignature.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      173 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/sets-exit-choices.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      251 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/sets-exit-url.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      160 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/sets-exit.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4638 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/sign.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      166 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/some-questions.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      222 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/test-docx-template.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       22 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/test-example-list.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      786 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/test-sig-form.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      103 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/test-url.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3001 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/test.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      834 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testaction.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      664 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testaction2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      258 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testage.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      904 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testattach.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      692 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testbuildfl.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      990 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testbuildfl2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1143 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testcron.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1211 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testcron2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1370 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testcronbg.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      520 2022-01-04 03:03:30.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testdadict.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      534 2022-01-04 03:03:41.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testdalist2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      288 2022-01-04 03:03:10.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testdaobjectfail.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      279 2022-01-04 03:03:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testdaobjectsucceed.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      680 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testdivorce.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      385 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testdocx.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      809 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testemail.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1611 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testfields.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      306 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testforloop.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      719 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testgeneric.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      554 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testimage.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      801 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testlist0.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      388 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testlist1.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      385 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testlist2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      414 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testlist3.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      364 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testmcmako.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      320 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testobjectfield.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      273 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testobjectfieldradio.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      495 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testobjectlist.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      587 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testobjects.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      606 2022-03-05 18:00:15.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testpermissions.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      356 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testperson.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6136 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testpg.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2525 2022-01-04 03:03:22.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testpickle.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      648 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testplural.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1247 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testproblem.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      659 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testpulldown.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      293 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testqr.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      474 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testqr2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      221 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testresponse.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      789 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      907 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview2.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      774 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview3.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      872 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview4.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      196 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testsandbox.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      196 2022-03-25 17:41:50.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testtr.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      512 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testunicode.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       90 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testurlarg.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      347 2021-11-05 23:59:55.000000 docassemble.demo-1.4.8/docassemble/demo/data/questions/testurlarg2.yml
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.169667 docassemble.demo-1.4.8/docassemble/demo/data/sources/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      844 2017-06-06 10:38:05.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/claims.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      914 2019-09-23 01:41:44.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/contacts.json
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      473 2019-09-23 01:26:01.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/contacts.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6983 2019-09-17 00:30:27.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/context_es.xlsx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      332 2017-02-18 18:44:59.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/fishes.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4928 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/fruit_data.xlsx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       73 2017-05-24 01:00:59.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/fruitseeds.yml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4093 2019-09-22 02:23:19.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/ml-random-forest-interview.json
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1500 2017-10-22 02:32:29.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/ml-random-forest.json
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23773 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/questions_es.xlsx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      290 2017-02-18 19:31:05.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/raw_data.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14162 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/signdoc_es.xlsx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5503 2022-03-25 17:34:56.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/testtr_en.xlsx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5441 2022-03-25 17:39:54.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/testtr_es.xlsx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      152 2016-09-25 16:03:42.000000 docassemble.demo-1.4.8/docassemble/demo/data/sources/training-data.json
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.197667 docassemble.demo-1.4.8/docassemble/demo/data/static/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      464 2019-05-31 10:02:20.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/README.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2826 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/abkhazia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3768 2015-10-19 04:08:20.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/accident3.eps
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13037 2015-10-19 04:07:41.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/accident3.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1913 2015-04-26 23:20:10.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/accident3.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1468 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/afghanistan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1728 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/aland-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1330 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/albania.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1321 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/algeria.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1552 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/american-samoa.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/andorra.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1589 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/angola.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2935 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/anguilla.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1424 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/antigua-and-barbuda.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1197 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/argentina.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/armenia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    55475 2019-01-21 20:08:21.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/art.jpg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1392 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/aruba.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3034 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/australia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1023 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/austria.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1667 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/azerbaijan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2769 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/azores-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bahamas.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      902 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bahrain.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1728 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/balearic-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      657 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bangladesh.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1441 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/barbados.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2556 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/basque-country.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1644 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/belarus.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      984 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/belgium.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1463 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/belize.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      933 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/benin.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2121 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bermuda.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1762 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bhutan-1.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1971 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bhutan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bolivia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1572 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bonaire.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2083 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bosnia-and-herzegovina.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1279 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/botswana.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1231 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/brazil.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6165 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/british-columbia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8368 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/british-indian-ocean-territory.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2567 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/british-virgin-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2118 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/brunei.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/bulgaria.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      953 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/burkina-faso.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1910 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/burundi.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      721 2022-07-28 22:47:53.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/button-checkboxes.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1373 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cambodia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1212 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cameroon.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1214 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/canada.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1011 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/canary-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2853 2019-01-21 20:19:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/canvas.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3128 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cape-verde.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2792 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cayman-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1889 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/central-african-republic.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2987 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ceuta.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1011 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/chad.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/chile.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1280 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/china.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2949 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/christmas-island.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2766 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cocos-island.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      903 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/colombia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2436 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/comoros.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3252 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cook-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1432 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/corsica.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1043 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/costa-rica.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3156 2015-10-19 04:08:26.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/crawling.eps
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7325 2015-10-19 04:07:56.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/crawling.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1323 2015-04-26 19:57:56.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/crawling.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3150 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/croatia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      460 2015-11-28 00:30:23.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/crown.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1569 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cuba.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1318 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/curacao.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1332 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/cyprus.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      895 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/czech-republic.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2872 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/datereplace.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1617 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/democratic-republic-of-congo.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1167 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/denmark.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1205 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/djibouti.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4573 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/dominica.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1480 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/dominican-republic.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18697 2022-04-09 13:15:32.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/draft.eps
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1111 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/east-timor.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1546 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ecuador.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1209 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/egypt.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1000 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/england.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/equatorial-guinea.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1507 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/eritrea.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      982 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/estonia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1588 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ethiopia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2240 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/european-union.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2549 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/falkland-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1478 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/faroe-islands.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7406 2021-05-05 12:56:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/favicon.ico
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2063 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/fiji.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      942 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/finland.svg
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.197667 docassemble.demo-1.4.8/docassemble/demo/data/static/flags/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      448 2019-05-30 16:21:00.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/flags/README.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      841 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/france.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1407 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/french-polynesia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1010 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/gabon.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/galapagos-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/gambia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1975 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/georgia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      984 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/germany.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1187 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ghana.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1895 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/gibraltar.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4232 2016-12-13 12:22:03.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/globe.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1353 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/greece.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      940 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/greenland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3280 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/grenada.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1963 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/guam.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1505 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/guatemala.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1332 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/guernsey.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1286 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/guinea-bissau.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1027 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/guinea.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1513 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/guyana.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1272 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/haiti.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1665 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/hawaii.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8812 2019-04-25 02:52:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/hello7.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    54798 2017-05-17 10:17:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/hello_planet.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1880 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/honduras.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1740 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/hong-kong.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      685 2015-11-28 00:29:13.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/house.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1008 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/hungary.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1463 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/iceland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1182 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/india.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/indonesia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1618 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/iran.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/iraq.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ireland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1008 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/isle-of-man.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1514 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/israel.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      841 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/italy.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ivory-coast.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1111 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/jamaica.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      653 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/japan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1437 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/jersey.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1276 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/jordan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1400 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/kazakhstan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2015 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/kenya.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5112 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/kiribati.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2114 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/kosovo.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1134 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/kuwait.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1859 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/kyrgyzstan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1093 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/laos.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      850 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/latvia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1003 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/lebanon.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1158 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/lesotho.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2566 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/liberia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1580 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/libya.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1134 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/liechtenstein.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1012 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/lithuania.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)   185381 2021-12-05 22:33:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/lumen.min.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/luxembourg.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2419 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/macao.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      879 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/madagascar.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1618 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/madeira.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4224 2018-03-09 13:31:11.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/main_doc_params.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6599 2019-06-11 11:24:20.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/main_document.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      775 2019-06-11 11:12:22.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/maindocpicture.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1187 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/malawi.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1843 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/malaysia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1027 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/maldives.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1006 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/mali.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      919 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/malta.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1459 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/marshall-island.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3328 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/martinique.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1079 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/mauritania.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1111 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/mauritius.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2573 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/melilla.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1376 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/mexico.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1432 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/micronesia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1712 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/moldova.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/monaco.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1709 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/mongolia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1917 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/montenegro.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1913 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/montserrat.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1191 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/morocco.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1693 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/mozambique.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       29 2015-10-27 01:02:38.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/my.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1200 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/myanmar.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       45 2017-08-09 01:23:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/myglobal.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       44 2017-08-09 00:51:52.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/myglobal.js
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1524 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/namibia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2236 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/nato.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1273 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/nauru.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       85 2019-05-07 10:39:26.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/navbar60.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       85 2019-05-07 10:39:31.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/navbar65.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1877 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/nepal.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/netherlands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2267 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/new-zealand.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1468 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/nicaragua.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1083 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/niger.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      852 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/nigeria.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2589 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/niue.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1180 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/norfolk-island.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1319 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/north-korea.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1472 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/northen-cyprus.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4073 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/northern-marianas-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1464 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/norway.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1413 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/oman.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1728 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/orkney-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1006 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ossetia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1522 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/pakistan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      657 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/palau.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1010 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/palestine.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1225 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/panama.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2768 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/papua-new-guinea.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1418 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/paraguay.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      852 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/peru.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1856 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/philippines.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2078 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/pitcairn-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1234 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/portugal.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      191 2019-02-16 13:27:19.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/progressivedisclosure.css
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1377 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/puerto-rico.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      979 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/qatar.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1083 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/rapa-nui.svg
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.197667 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3177 2017-04-10 04:36:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/android-chrome-192x192.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4992 2017-04-10 04:36:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/android-chrome-512x512.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3087 2017-04-10 04:36:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/apple-touch-icon.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      246 2017-04-10 04:36:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/browserconfig.xml
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      778 2017-04-10 04:36:08.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/favicon-16x16.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1060 2017-04-10 04:36:08.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/favicon-32x32.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7406 2017-04-10 04:36:08.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/favicon.ico
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      403 2017-04-10 04:36:08.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/manifest.json
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2681 2017-04-10 04:36:08.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/mstile-150x150.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      836 2017-04-10 04:36:08.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/safari-pinned-tab.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1670 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/republic-of-macedonia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      680 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/republic-of-poland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1074 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/republic-of-the-congo.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1063 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/romania.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      926 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/russia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1379 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/rwanda.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1243 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/saba-island.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1594 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/saint-kitts-and-nevis.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1440 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/salvador.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1836 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/samoa.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   334145 2016-04-19 01:39:37.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sample-sig-form-2.pdf
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   600070 2016-04-19 01:39:37.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sample-sig-form.pdf
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   211605 2015-04-26 21:43:51.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sample-support-order.jpg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2091 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/san-marino.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1406 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sao-tome-and-principe.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sardinia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1772 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/saudi-arabia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)  1370905 2015-11-18 03:32:46.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-1.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)  1195233 2015-11-18 11:19:39.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-1.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   728083 2015-11-18 03:33:22.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-2.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   639303 2015-11-18 11:20:00.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-2.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   696319 2015-11-18 03:33:28.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-3.mp3
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   595080 2015-11-18 11:20:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-3.ogg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1180 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/scotland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1227 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/senegal.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2008 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/serbia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1237 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/seychelles.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1006 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sierra-leone.svg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4145 2021-05-05 12:56:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sign-here.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2003 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/singapore.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2498 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sint-eustatius.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1762 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sint-maarten.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1998 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/slovakia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1154 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/slovenia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2164 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/solomon-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      787 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/somalia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2194 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/somaliland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1500 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/south-africa.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3242 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/south-korea.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1426 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/south-sudan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1016 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/spain.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1783 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sri-lanka.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1943 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/st-barts.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      850 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/st-lucia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1331 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/st-vincent-and-the-grenadines.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4311 2018-03-09 13:31:04.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sub_doc_params.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6734 2019-06-11 11:18:23.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sub_document.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      978 2019-06-11 11:11:40.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/subdocpicture.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1129 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sudan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1281 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/suriname.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1912 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/swaziland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1167 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/sweden.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      829 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/switzerland.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1247 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/syria.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1440 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/taiwan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2626 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/tajikistan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1132 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/tanzania.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1043 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/thailand.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2319 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/tibet.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1326 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/togo.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1779 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/tokelau.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      996 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/tonga.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1021 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/transnistria.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1377 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/trinidad-and-tobago.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1226 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/tunisia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1160 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/turkey.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4394 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/turkmenistan.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2346 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/turks-and-caicos.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3572 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/tuvalu.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1986 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/uganda.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/ukraine.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      988 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/united-arab-emirates.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2599 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/united-kingdom.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2516 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/united-nations.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2295 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/united-states-of-america.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4253 2020-02-19 12:23:38.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/universal-test.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1636 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/uruguay.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5154 2015-10-19 04:08:33.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/users6.eps
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    19620 2015-10-19 04:08:08.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/users6.png
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3048 2015-04-26 19:57:56.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/users6.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4227 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/uzbekistn.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4189 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/vanuatu.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1725 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/vatican-city.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2679 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/venezuela.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      787 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/vietnam.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1934 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/virgin-islands.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1491 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/wales.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1629 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/western-sahara.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      817 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/yemen.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1287 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/zambia.svg
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2516 2016-09-22 12:09:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/static/zimbabwe.svg
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.201667 docassemble.demo-1.4.8/docassemble/demo/data/templates/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4363 2017-05-31 11:17:38.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/Agreement_To_Transfer.docx
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   183307 2021-05-05 12:56:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/Transfer-of-Ownership.pdf
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       76 2015-10-28 10:32:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/base_template.md
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4257 2019-05-16 02:34:00.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/context.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5083 2020-03-22 22:02:42.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/contract.docx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4785 2021-05-05 12:56:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/declaration_certificate_service.docx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4901 2021-05-05 12:56:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/declaration_of_favorite_fruit.docx
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    11738 2021-05-05 12:56:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/doc-with-toc.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4152 2019-07-10 11:25:43.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/docx-with-metadata.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5007 2020-01-09 13:48:02.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/exhibit_insert.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4801 2018-11-25 16:52:07.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/food_template.docx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4455 2021-05-05 12:56:34.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/fruit_declaration.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4288 2019-07-20 19:19:44.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/generic-document.docx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4805 2022-06-08 00:38:01.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/graph.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    54798 2017-05-17 10:17:58.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/hello_planet.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      357 2015-10-28 10:25:10.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/hello_template.md
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4309 2019-04-24 15:15:17.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/life_story.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4275 2018-11-25 16:49:02.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/logo_template.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4397 2018-03-09 13:47:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/main_doc_params.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6599 2019-06-11 11:17:31.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/main_document.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4286 2018-09-08 16:50:21.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/markdown_template_demo.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1277 2019-11-16 00:23:59.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/myinterviews.html
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      287 2017-08-08 21:19:30.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/mystart.html
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5351 2022-05-15 00:30:39.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/nested_list_table.docx
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5013 2022-03-05 21:32:15.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/numbering_template.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4210 2018-09-15 19:54:45.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/quotes-in-code.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4503 2018-09-03 23:11:39.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/redact_demo.docx
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)    32134 2018-09-03 23:11:39.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/redact_demo.pdf
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)   334145 2016-03-05 13:47:30.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/sample-sig-form-2.pdf
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)   600070 2016-03-05 13:47:30.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/sample-sig-form.pdf
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      156 2019-09-26 19:26:17.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/sample.cpp
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4302 2019-06-05 00:28:03.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/signature_template.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4283 2018-03-10 23:31:25.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/sub_doc_params.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6734 2019-06-11 11:24:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/sub_document.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4111 2019-02-27 04:16:12.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/tagged.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4849 2019-11-26 12:39:45.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/team.docx
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4102 2018-01-29 04:19:06.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/template_test.docx
--rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)   174617 2018-05-13 16:59:19.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/testsigform.pdf
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4177 2019-05-01 01:04:39.000000 docassemble.demo-1.4.8/docassemble/demo/data/templates/twostage.docx
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.201667 docassemble.demo-1.4.8/docassemble/demo/data/translations/
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       47 2015-11-13 02:39:14.000000 docassemble.demo-1.4.8/docassemble/demo/data/translations/words.yml
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9823 2022-08-08 12:46:18.000000 docassemble.demo-1.4.8/docassemble/demo/demodb.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      225 2022-08-05 11:52:44.000000 docassemble.demo-1.4.8/docassemble/demo/ein.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      112 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/fish.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      576 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/fishlist.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      835 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/fruit_database.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      466 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/gd_fetch.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      221 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/gettime.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3530 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/google_drive.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1045 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/google_sheets.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2980 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/google_vision2.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      458 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/graph.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       23 2019-04-24 00:02:48.000000 docassemble.demo-1.4.8/docassemble/demo/hello.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      642 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/income.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1525 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/index.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      247 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/legume.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      917 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/oauthsheets.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      202 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/objects.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      815 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/progressivedisclosure.py
--rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5854 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/random-test.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      503 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/read_snapshot.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9747 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/reldemodb.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9988 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/sign.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      319 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/somefuncs.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      965 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/ssn.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      693 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/testcontexttest.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      367 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/tests.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      852 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/translate.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3997 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/user_permissions.py
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       61 2022-08-05 12:12:33.000000 docassemble.demo-1.4.8/docassemble/demo/validationfuncs.py
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      193 2022-08-05 21:01:20.000000 docassemble.demo-1.4.8/docassemble/demo/validationfuncstwo.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-08-25 13:37:24.149667 docassemble.demo-1.4.8/docassemble.demo.egg-info/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      664 2022-08-25 13:37:23.000000 docassemble.demo-1.4.8/docassemble.demo.egg-info/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)    30976 2022-08-25 13:37:23.000000 docassemble.demo-1.4.8/docassemble.demo.egg-info/SOURCES.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-08-25 13:37:23.000000 docassemble.demo-1.4.8/docassemble.demo.egg-info/dependency_links.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-08-25 13:37:23.000000 docassemble.demo-1.4.8/docassemble.demo.egg-info/namespace_packages.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-08-25 13:37:23.000000 docassemble.demo-1.4.8/docassemble.demo.egg-info/not-zip-safe
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       70 2022-08-25 13:37:23.000000 docassemble.demo-1.4.8/docassemble.demo.egg-info/requires.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-08-25 13:37:23.000000 docassemble.demo-1.4.8/docassemble.demo.egg-info/top_level.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       79 2022-08-25 13:37:24.201667 docassemble.demo-1.4.8/setup.cfg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2600 2022-08-25 13:37:07.000000 docassemble.demo-1.4.8/setup.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.982522 docassemble.demo-1.4.9/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:54.000000 docassemble.demo-1.4.9/MANIFEST.in
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      664 2022-09-10 18:15:55.982522 docassemble.demo-1.4.9/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.934522 docassemble.demo-1.4.9/docassemble/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      154 2015-04-16 10:10:01.000000 docassemble.demo-1.4.9/docassemble/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.938522 docassemble.demo-1.4.9/docassemble/demo/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       22 2022-09-10 18:15:31.000000 docassemble.demo-1.4.9/docassemble/demo/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.938522 docassemble.demo-1.4.9/docassemble/demo/alembic/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       38 2019-08-18 19:33:12.000000 docassemble.demo-1.4.9/docassemble/demo/alembic/README
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2125 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/alembic/env.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      494 2019-08-18 19:33:12.000000 docassemble.demo-1.4.9/docassemble/demo/alembic/script.py.mako
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1647 2019-08-18 19:33:12.000000 docassemble.demo-1.4.9/docassemble/demo/alembic.ini
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      881 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/attorney.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1874 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/calendar.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      935 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/cards.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      223 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/change_suffix.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14959 2022-09-08 12:22:53.000000 docassemble.demo-1.4.9/docassemble/demo/companydb.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.934522 docassemble.demo-1.4.9/docassemble/demo/data/
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.938522 docassemble.demo-1.4.9/docassemble/demo/data/objects/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1658 2016-08-10 02:21:26.000000 docassemble.demo-1.4.9/docassemble/demo/data/objects/organizations.yml
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.942522 docassemble.demo-1.4.9/docassemble/demo/data/questions/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      314 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/animal.yml
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.942522 docassemble.demo-1.4.9/docassemble/demo/data/questions/bestnumber/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      258 2019-03-03 17:43:24.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/bestnumber/code.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      378 2015-11-11 15:10:56.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/bestnumber/en.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      384 2015-11-11 15:10:41.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/bestnumber/es.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       51 2015-11-11 14:48:01.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/bestnumber/interview.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    16447 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/conflict_check.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1580 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/demo-basic-questions-address.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2541 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/demo-basic-questions-name.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      243 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/demo-basic-questions.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      256 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/event-role-event.yml
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.950522 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      403 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/ab-test.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1374 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/advocate.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1788 2022-03-26 01:52:09.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/ajax.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      737 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/all-mandatory.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1987 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/background-tail.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      388 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/bates-number.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      438 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/bootstrap-theme.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      721 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/branch-mandatory.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      827 2022-07-28 22:47:53.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/button-checkboxes.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2901 2022-04-21 10:18:19.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/calendar.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       20 2022-06-08 14:37:11.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/cards.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1563 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/clauses.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1810 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/collate.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     9799 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/companies.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      721 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/complete-attribute-method.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      982 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/context-code.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      983 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/context-manual.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      843 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/context.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1484 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/counter.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4202 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/courtfile.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6107 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/custody.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      370 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/customdate.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3302 2022-04-19 10:46:18.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/daglobal.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1987 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/demo-multi-sign-2.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1735 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/demo-multi-sign.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4239 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/demo-with-basic-questions.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      835 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/dependency-demo-code.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      564 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/dependency-demo.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      535 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/discovery.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      695 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/docxproperties.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1469 2022-04-30 13:16:43.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/duplicate.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1435 2022-06-08 18:50:38.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/explain.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      381 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/fish-example.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      907 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/flags.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1320 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/food-with-sig.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      402 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/fruits-database.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      815 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/generic-document.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      337 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/get-time.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2433 2022-04-19 10:46:18.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/globalprofile.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2433 2022-04-19 10:46:18.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/globalprofile2.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1795 2022-04-19 23:39:18.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/globalprofile3.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      950 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-drive.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1068 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-sheet-2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1203 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-sheet-3.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      998 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-sheet.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      737 2022-06-08 14:47:21.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/graph.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1283 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/harry-potter-or-heidegger.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1441 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/hook-on-gather.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      969 2022-03-26 00:36:25.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/indexdemo.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      598 2022-03-26 01:45:11.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/indexdemoquery.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2694 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/interview_in_interview.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       81 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/jinjayaml-included.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      709 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/jinjayaml.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1071 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/jsondemo.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      589 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/life_story.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2739 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/macros.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      598 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background-2.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      628 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      504 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/make-ocr-pdf.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1307 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/markdown-template.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      567 2021-11-05 23:59:36.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/ml-export-playground.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     6799 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/multi-signature.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2631 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/multi-user.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1817 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/navbar-language.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1736 2022-05-17 10:26:00.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/nested-list-docx-table.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2983 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/new-or-existing.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1397 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/oauth-test-2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1276 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/oauth-test-3.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1340 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/oauth-test-4.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      492 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/oauth-test.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2115 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/object-checkboxes-copy.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      940 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/object-checkboxes-custom.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      453 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/objects-from-file-dadict.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      736 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/objects-from-file-gather.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      394 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/objects-from-file-json.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      520 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/objects-from-file-template.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      411 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/objects-from-file.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      432 2022-03-05 21:44:03.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/overlay-pdf-multi.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      616 2022-03-05 21:34:31.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/overlay-pdf.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      564 2022-09-08 11:38:23.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pdfextract.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1272 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/phone-number-2.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1119 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/phone-number.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      646 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/predict-activity-activity.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      634 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/predict-activity.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      355 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/predict-happy-sad-area.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      351 2021-12-27 04:59:09.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/predict-happy-sad.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      760 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/prevent-dependency-satisfaction.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1736 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/preview.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2201 2022-05-16 03:02:48.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/primary-interview.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1005 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/progressive-disclosure.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      727 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-dom.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      863 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-hidden.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      684 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-log.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      634 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-script.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      429 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/questionless.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      579 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/quotes-in-code.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1925 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/random-forest-interview.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1268 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/random-forest.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      433 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/raw-data-example.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      455 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/raw.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1040 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/realtimegd.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      963 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/realtimegd2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1256 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/redact-docx.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1743 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/redact-pdf.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      871 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/repeatable.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      188 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/report-version.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      304 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/run-python-module-2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      288 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/run-python-module-3.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      431 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/run-python-module-tests.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      290 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/run-python-module.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2095 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/save-continue-later.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      371 2022-05-16 00:00:33.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/secondary-interview.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      858 2022-04-09 12:56:16.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/setparts.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3025 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/sign.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2234 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signature-diversion.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1986 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signature-preview.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      776 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signature-template.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    25478 2022-08-31 14:14:31.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signdoc.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      811 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/single-code.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      749 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/snapshot.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1436 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/someone-already-mentioned.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      878 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/stage-one.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      601 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/stage-two.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1426 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/subdoc-params.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/subdocument.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      485 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/tagged-pdf.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1317 2022-06-07 23:52:50.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testcards.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      680 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testcooking.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1296 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testdatabase.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1394 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testgeolocate.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      222 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testssn.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      738 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/translation.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      593 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/turnips-worms.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1801 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/universal-document.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      772 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/update-references.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      441 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/upload-file-size.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      625 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/validation-code.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      456 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/validation-test-two.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      455 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/validation-test.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      540 2022-04-09 13:22:47.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/watermark.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      651 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/wc_common.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      991 2021-11-05 23:59:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/wc_side_of_bed.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       72 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/hello.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      156 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/hello2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      478 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/hello3.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      714 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/hello4.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      901 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/hello5.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      594 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/hello6.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      299 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/hello7.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      340 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/income.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      266 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/interview-about-flowers.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      257 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/interview-about-fruit.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      287 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/interview-about-vegetables.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      739 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/list.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    39692 2022-04-30 15:49:50.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/questions.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2640 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/roletest.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1240 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/roletestmany.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      101 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/sample-function.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      127 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/samplequestion.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      181 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/samplesignature.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      173 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/sets-exit-choices.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      251 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/sets-exit-url.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      160 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/sets-exit.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4638 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/sign.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      166 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/some-questions.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      222 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/test-docx-template.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       22 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/test-example-list.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      786 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/test-sig-form.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      103 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/test-url.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3001 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/test.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      834 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testaction.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      664 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testaction2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      258 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testage.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      904 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testattach.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      692 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testbuildfl.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      990 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testbuildfl2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1143 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testcron.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1211 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testcron2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1370 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testcronbg.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      520 2022-01-04 03:03:30.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testdadict.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      534 2022-01-04 03:03:41.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testdalist2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      288 2022-01-04 03:03:10.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testdaobjectfail.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      279 2022-01-04 03:03:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testdaobjectsucceed.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      680 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testdivorce.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      385 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testdocx.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      809 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testemail.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1611 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testfields.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      306 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testforloop.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      719 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testgeneric.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      554 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testimage.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      801 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testlist0.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      388 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testlist1.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      385 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testlist2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      414 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testlist3.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      364 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testmcmako.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      320 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testobjectfield.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      273 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testobjectfieldradio.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      495 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testobjectlist.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      587 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testobjects.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      606 2022-03-05 18:00:15.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testpermissions.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      356 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testperson.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6136 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testpg.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2525 2022-01-04 03:03:22.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testpickle.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      648 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testplural.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1247 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testproblem.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      659 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testpulldown.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      293 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testqr.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      474 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testqr2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      221 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testresponse.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      789 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      907 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview2.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      774 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview3.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      872 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview4.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      196 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testsandbox.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      196 2022-03-25 17:41:50.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testtr.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      512 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testunicode.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       90 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testurlarg.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      347 2021-11-05 23:59:55.000000 docassemble.demo-1.4.9/docassemble/demo/data/questions/testurlarg2.yml
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.954522 docassemble.demo-1.4.9/docassemble/demo/data/sources/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      844 2017-06-06 10:38:05.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/claims.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      914 2019-09-23 01:41:44.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/contacts.json
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      473 2019-09-23 01:26:01.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/contacts.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6983 2019-09-17 00:30:27.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/context_es.xlsx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      332 2017-02-18 18:44:59.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/fishes.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4928 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/fruit_data.xlsx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       73 2017-05-24 01:00:59.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/fruitseeds.yml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4093 2019-09-22 02:23:19.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/ml-random-forest-interview.json
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1500 2017-10-22 02:32:29.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/ml-random-forest.json
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    23773 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/questions_es.xlsx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      290 2017-02-18 19:31:05.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/raw_data.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    14162 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/signdoc_es.xlsx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5503 2022-03-25 17:34:56.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/testtr_en.xlsx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5441 2022-03-25 17:39:54.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/testtr_es.xlsx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      152 2016-09-25 16:03:42.000000 docassemble.demo-1.4.9/docassemble/demo/data/sources/training-data.json
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.978522 docassemble.demo-1.4.9/docassemble/demo/data/static/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      464 2019-05-31 10:02:20.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/README.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2826 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/abkhazia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3768 2015-10-19 04:08:20.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/accident3.eps
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    13037 2015-10-19 04:07:41.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/accident3.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1913 2015-04-26 23:20:10.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/accident3.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1468 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/afghanistan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1728 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/aland-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1330 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/albania.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1321 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/algeria.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1552 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/american-samoa.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/andorra.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1589 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/angola.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2935 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/anguilla.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1424 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/antigua-and-barbuda.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1197 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/argentina.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/armenia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    55475 2019-01-21 20:08:21.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/art.jpg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1392 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/aruba.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3034 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/australia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1023 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/austria.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1667 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/azerbaijan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2769 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/azores-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bahamas.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      902 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bahrain.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1728 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/balearic-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      657 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bangladesh.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1441 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/barbados.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2556 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/basque-country.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1644 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/belarus.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      984 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/belgium.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1463 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/belize.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      933 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/benin.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2121 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bermuda.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1762 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bhutan-1.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1971 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bhutan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bolivia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1572 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bonaire.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2083 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bosnia-and-herzegovina.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1279 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/botswana.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1231 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/brazil.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6165 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/british-columbia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8368 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/british-indian-ocean-territory.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2567 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/british-virgin-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2118 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/brunei.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/bulgaria.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      953 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/burkina-faso.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1910 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/burundi.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      721 2022-07-28 22:47:53.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/button-checkboxes.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1373 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cambodia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1212 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cameroon.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1214 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/canada.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1011 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/canary-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2853 2019-01-21 20:19:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/canvas.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3128 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cape-verde.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2792 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cayman-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1889 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/central-african-republic.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2987 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ceuta.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1011 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/chad.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/chile.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1280 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/china.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2949 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/christmas-island.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2766 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cocos-island.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      903 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/colombia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2436 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/comoros.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3252 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cook-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1432 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/corsica.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1043 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/costa-rica.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3156 2015-10-19 04:08:26.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/crawling.eps
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7325 2015-10-19 04:07:56.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/crawling.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1323 2015-04-26 19:57:56.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/crawling.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3150 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/croatia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      460 2015-11-28 00:30:23.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/crown.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1569 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cuba.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1318 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/curacao.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1332 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/cyprus.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      895 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/czech-republic.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2872 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/datereplace.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1617 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/democratic-republic-of-congo.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1167 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/denmark.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1205 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/djibouti.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4573 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/dominica.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1480 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/dominican-republic.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    18697 2022-04-09 13:15:32.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/draft.eps
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1111 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/east-timor.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1546 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ecuador.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1209 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/egypt.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1000 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/england.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/equatorial-guinea.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1507 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/eritrea.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      982 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/estonia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1588 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ethiopia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2240 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/european-union.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2549 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/falkland-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1478 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/faroe-islands.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     7406 2021-05-05 12:56:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/favicon.ico
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2063 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/fiji.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      942 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/finland.svg
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.978522 docassemble.demo-1.4.9/docassemble/demo/data/static/flags/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      448 2019-05-30 16:21:00.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/flags/README.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      841 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/france.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1407 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/french-polynesia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1010 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/gabon.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/galapagos-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1025 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/gambia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1975 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/georgia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      984 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/germany.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1187 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ghana.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1895 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/gibraltar.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4232 2016-12-13 12:22:03.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/globe.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1353 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/greece.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      940 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/greenland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3280 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/grenada.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1963 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/guam.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1505 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/guatemala.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1332 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/guernsey.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1286 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/guinea-bissau.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1027 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/guinea.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1513 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/guyana.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1272 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/haiti.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1665 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/hawaii.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     8812 2019-04-25 02:52:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/hello7.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    54798 2017-05-17 10:17:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/hello_planet.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1880 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/honduras.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1740 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/hong-kong.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      685 2015-11-28 00:29:13.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/house.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1008 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/hungary.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1463 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/iceland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1182 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/india.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/indonesia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1618 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/iran.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1539 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/iraq.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ireland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1008 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/isle-of-man.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1514 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/israel.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      841 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/italy.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1009 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ivory-coast.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1111 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/jamaica.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      653 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/japan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1437 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/jersey.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1276 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/jordan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1400 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/kazakhstan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2015 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/kenya.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5112 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/kiribati.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2114 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/kosovo.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1134 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/kuwait.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1859 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/kyrgyzstan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1093 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/laos.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      850 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/latvia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1003 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/lebanon.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1158 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/lesotho.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2566 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/liberia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1580 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/libya.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1134 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/liechtenstein.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1012 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/lithuania.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)   185381 2021-12-05 22:33:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/lumen.min.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/luxembourg.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2419 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/macao.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      879 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/madagascar.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1618 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/madeira.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4224 2018-03-09 13:31:11.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/main_doc_params.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6599 2019-06-11 11:24:20.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/main_document.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      775 2019-06-11 11:12:22.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/maindocpicture.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1187 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/malawi.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1843 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/malaysia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1027 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/maldives.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1006 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/mali.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      919 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/malta.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1459 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/marshall-island.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3328 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/martinique.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1079 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/mauritania.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1111 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/mauritius.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2573 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/melilla.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1376 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/mexico.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1432 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/micronesia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1712 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/moldova.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/monaco.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1709 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/mongolia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1917 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/montenegro.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1913 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/montserrat.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1191 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/morocco.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1693 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/mozambique.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       29 2015-10-27 01:02:38.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/my.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1200 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/myanmar.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       45 2017-08-09 01:23:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/myglobal.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       44 2017-08-09 00:51:52.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/myglobal.js
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1524 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/namibia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2236 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/nato.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1273 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/nauru.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       85 2019-05-07 10:39:26.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/navbar60.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       85 2019-05-07 10:39:31.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/navbar65.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1877 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/nepal.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/netherlands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2267 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/new-zealand.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1468 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/nicaragua.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1083 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/niger.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      852 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/nigeria.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2589 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/niue.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1180 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/norfolk-island.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1319 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/north-korea.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1472 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/northen-cyprus.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4073 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/northern-marianas-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1464 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/norway.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1413 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/oman.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1728 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/orkney-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1006 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ossetia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1522 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/pakistan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      657 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/palau.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1010 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/palestine.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1225 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/panama.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2768 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/papua-new-guinea.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1418 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/paraguay.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      852 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/peru.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1856 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/philippines.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2078 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/pitcairn-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1234 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/portugal.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      191 2019-02-16 13:27:19.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/progressivedisclosure.css
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1377 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/puerto-rico.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      979 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/qatar.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1083 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/rapa-nui.svg
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.978522 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3177 2017-04-10 04:36:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/android-chrome-192x192.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4992 2017-04-10 04:36:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/android-chrome-512x512.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3087 2017-04-10 04:36:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/apple-touch-icon.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      246 2017-04-10 04:36:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/browserconfig.xml
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      778 2017-04-10 04:36:08.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/favicon-16x16.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1060 2017-04-10 04:36:08.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/favicon-32x32.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     7406 2017-04-10 04:36:08.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/favicon.ico
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      403 2017-04-10 04:36:08.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/manifest.json
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2681 2017-04-10 04:36:08.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/mstile-150x150.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      836 2017-04-10 04:36:08.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/safari-pinned-tab.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1670 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/republic-of-macedonia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      680 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/republic-of-poland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1074 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/republic-of-the-congo.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1063 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/romania.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      926 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/russia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1379 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/rwanda.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1243 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/saba-island.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1594 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/saint-kitts-and-nevis.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1440 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/salvador.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1836 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/samoa.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   334145 2016-04-19 01:39:37.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sample-sig-form-2.pdf
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   600070 2016-04-19 01:39:37.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sample-sig-form.pdf
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   211605 2015-04-26 21:43:51.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sample-support-order.jpg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2091 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/san-marino.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1406 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sao-tome-and-principe.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2839 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sardinia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1772 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/saudi-arabia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)  1370905 2015-11-18 03:32:46.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-1.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)  1195233 2015-11-18 11:19:39.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-1.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   728083 2015-11-18 03:33:22.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-2.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   639303 2015-11-18 11:20:00.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-2.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   696319 2015-11-18 03:33:28.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-3.mp3
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)   595080 2015-11-18 11:20:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-3.ogg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1180 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/scotland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1227 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/senegal.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2008 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/serbia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1237 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/seychelles.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1006 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sierra-leone.svg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4145 2021-05-05 12:56:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sign-here.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2003 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/singapore.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2498 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sint-eustatius.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1762 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sint-maarten.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1998 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/slovakia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1154 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/slovenia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2164 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/solomon-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      787 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/somalia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2194 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/somaliland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1500 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/south-africa.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3242 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/south-korea.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1426 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/south-sudan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1016 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/spain.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1783 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sri-lanka.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1943 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/st-barts.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      850 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/st-lucia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1331 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/st-vincent-and-the-grenadines.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4311 2018-03-09 13:31:04.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sub_doc_params.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6734 2019-06-11 11:18:23.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sub_document.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      978 2019-06-11 11:11:40.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/subdocpicture.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1129 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sudan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1281 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/suriname.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1912 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/swaziland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1167 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/sweden.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      829 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/switzerland.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1247 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/syria.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1440 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/taiwan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2626 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/tajikistan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1132 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/tanzania.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1043 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/thailand.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2319 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/tibet.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1326 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/togo.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1779 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/tokelau.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      996 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/tonga.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1021 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/transnistria.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1377 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/trinidad-and-tobago.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1226 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/tunisia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1160 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/turkey.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4394 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/turkmenistan.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2346 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/turks-and-caicos.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3572 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/tuvalu.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1986 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/uganda.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      678 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/ukraine.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      988 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/united-arab-emirates.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2599 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/united-kingdom.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2516 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/united-nations.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2295 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/united-states-of-america.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4253 2020-02-19 12:23:38.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/universal-test.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1636 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/uruguay.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5154 2015-10-19 04:08:33.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/users6.eps
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    19620 2015-10-19 04:08:08.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/users6.png
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     3048 2015-04-26 19:57:56.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/users6.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4227 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/uzbekistn.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4189 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/vanuatu.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1725 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/vatican-city.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2679 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/venezuela.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      787 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/vietnam.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1934 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/virgin-islands.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1491 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/wales.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1629 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/western-sahara.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      817 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/yemen.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1287 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/zambia.svg
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     2516 2016-09-22 12:09:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/static/zimbabwe.svg
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.982522 docassemble.demo-1.4.9/docassemble/demo/data/templates/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4363 2017-05-31 11:17:38.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/Agreement_To_Transfer.docx
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)   183307 2021-05-05 12:56:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/Transfer-of-Ownership.pdf
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       76 2015-10-28 10:32:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/base_template.md
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4257 2019-05-16 02:34:00.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/context.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5083 2020-03-22 22:02:42.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/contract.docx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4785 2021-05-05 12:56:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/declaration_certificate_service.docx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4901 2021-05-05 12:56:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/declaration_of_favorite_fruit.docx
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)    11738 2021-05-05 12:56:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/doc-with-toc.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4152 2019-07-10 11:25:43.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/docx-with-metadata.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     5007 2020-01-09 13:48:02.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/exhibit_insert.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4801 2018-11-25 16:52:07.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/food_template.docx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4455 2021-05-05 12:56:34.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/fruit_declaration.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4288 2019-07-20 19:19:44.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/generic-document.docx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     4805 2022-06-08 00:38:01.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/graph.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)    54798 2017-05-17 10:17:58.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/hello_planet.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      357 2015-10-28 10:25:10.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/hello_template.md
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4309 2019-04-24 15:15:17.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/life_story.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4275 2018-11-25 16:49:02.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/logo_template.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4397 2018-03-09 13:47:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/main_doc_params.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6599 2019-06-11 11:17:31.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/main_document.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4286 2018-09-08 16:50:21.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/markdown_template_demo.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     1277 2019-11-16 00:23:59.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/myinterviews.html
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      287 2017-08-08 21:19:30.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/mystart.html
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5351 2022-05-15 00:30:39.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/nested_list_table.docx
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     5013 2022-03-05 21:32:15.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/numbering_template.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4210 2018-09-15 19:54:45.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/quotes-in-code.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4503 2018-09-03 23:11:39.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/redact_demo.docx
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)    32134 2018-09-03 23:11:39.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/redact_demo.pdf
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)   334145 2016-03-05 13:47:30.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/sample-sig-form-2.pdf
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)   600070 2016-03-05 13:47:30.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/sample-sig-form.pdf
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      156 2019-09-26 19:26:17.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/sample.cpp
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4302 2019-06-05 00:28:03.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/signature_template.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4283 2018-03-10 23:31:25.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/sub_doc_params.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     6734 2019-06-11 11:24:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/sub_document.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4111 2019-02-27 04:16:12.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/tagged.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4849 2019-11-26 12:39:45.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/team.docx
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4102 2018-01-29 04:19:06.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/template_test.docx
+-rwxrwxr-x   0 jpyle     (1000) jpyle     (1000)   174617 2018-05-13 16:59:19.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/testsigform.pdf
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)     4177 2019-05-01 01:04:39.000000 docassemble.demo-1.4.9/docassemble/demo/data/templates/twostage.docx
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.982522 docassemble.demo-1.4.9/docassemble/demo/data/translations/
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       47 2015-11-13 02:39:14.000000 docassemble.demo-1.4.9/docassemble/demo/data/translations/words.yml
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9823 2022-08-08 12:46:18.000000 docassemble.demo-1.4.9/docassemble/demo/demodb.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)      225 2022-08-05 11:52:44.000000 docassemble.demo-1.4.9/docassemble/demo/ein.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      112 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/fish.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      576 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/fishlist.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      835 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/fruit_database.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      466 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/gd_fetch.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      221 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/gettime.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3530 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/google_drive.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1045 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/google_sheets.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2980 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/google_vision2.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      458 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/graph.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       23 2019-04-24 00:02:48.000000 docassemble.demo-1.4.9/docassemble/demo/hello.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      642 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/income.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1525 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/index.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      247 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/legume.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      917 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/oauthsheets.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      202 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/objects.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      815 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/progressivedisclosure.py
+-rwxr-xr-x   0 jpyle     (1000) jpyle     (1000)     5854 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/random-test.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      503 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/read_snapshot.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9747 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/reldemodb.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     9988 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/sign.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      319 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/somefuncs.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      965 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/ssn.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      693 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/testcontexttest.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      367 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/tests.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      852 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/translate.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     3997 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/user_permissions.py
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       61 2022-08-05 12:12:33.000000 docassemble.demo-1.4.9/docassemble/demo/validationfuncs.py
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      193 2022-08-05 21:01:20.000000 docassemble.demo-1.4.9/docassemble/demo/validationfuncstwo.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2022-09-10 18:15:55.934522 docassemble.demo-1.4.9/docassemble.demo.egg-info/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      664 2022-09-10 18:15:55.000000 docassemble.demo-1.4.9/docassemble.demo.egg-info/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)    31032 2022-09-10 18:15:55.000000 docassemble.demo-1.4.9/docassemble.demo.egg-info/SOURCES.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-09-10 18:15:55.000000 docassemble.demo-1.4.9/docassemble.demo.egg-info/dependency_links.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-09-10 18:15:55.000000 docassemble.demo-1.4.9/docassemble.demo.egg-info/namespace_packages.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2022-09-10 18:15:55.000000 docassemble.demo-1.4.9/docassemble.demo.egg-info/not-zip-safe
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       70 2022-09-10 18:15:55.000000 docassemble.demo-1.4.9/docassemble.demo.egg-info/requires.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2022-09-10 18:15:55.000000 docassemble.demo-1.4.9/docassemble.demo.egg-info/top_level.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       79 2022-09-10 18:15:55.982522 docassemble.demo-1.4.9/setup.cfg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     2600 2022-09-10 18:15:31.000000 docassemble.demo-1.4.9/setup.py
```

### Comparing `docassemble.demo-1.4.8/PKG-INFO` & `docassemble.demo-1.4.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.demo
-Version: 1.4.8
+Version: 1.4.9
 Summary: A demonstration package for docassemble.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Description: See the [docassemble web site] for a description of **docassemble**
         and installation instructions.
```

### Comparing `docassemble.demo-1.4.8/docassemble/demo/alembic/env.py` & `docassemble.demo-1.4.9/docassemble/demo/alembic/env.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/alembic.ini` & `docassemble.demo-1.4.9/docassemble/demo/alembic.ini`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/attorney.py` & `docassemble.demo-1.4.9/docassemble/demo/attorney.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/calendar.py` & `docassemble.demo-1.4.9/docassemble/demo/calendar.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/cards.py` & `docassemble.demo-1.4.9/docassemble/demo/cards.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/companydb.py` & `docassemble.demo-1.4.9/docassemble/demo/companydb.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,14 +396,16 @@
 
     def db_null(self, column):
         if column == 'name':
             del self.name.text
         elif column == 'upload_id':
             del self.upload[0].number
             self.upload[0].ok = False
+            if hasattr(self.upload[0], 'initialized'):
+                del self.upload[0].initialized
         elif column == 'date':
             del self.date
         elif column == 'filename':
             del self.upload[0].filename
             self.upload[0].has_specific_filename = False
         elif column == 'extension':
             del self.upload[0].extension
```

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/objects/organizations.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/objects/organizations.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/conflict_check.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/conflict_check.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/demo-basic-questions-address.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/demo-basic-questions-address.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/demo-basic-questions-name.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/demo-basic-questions-name.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/advocate.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/advocate.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/ajax.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/ajax.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/all-mandatory.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/all-mandatory.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/background-tail.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/background-tail.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/branch-mandatory.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/branch-mandatory.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/button-checkboxes.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/button-checkboxes.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/calendar.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/calendar.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/clauses.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/clauses.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/collate.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/collate.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/companies.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/companies.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/complete-attribute-method.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/complete-attribute-method.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/context-code.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/context-code.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/context-manual.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/context-manual.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/context.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/context.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/counter.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/counter.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/courtfile.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/courtfile.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/custody.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/custody.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/daglobal.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/daglobal.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/demo-multi-sign-2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/demo-multi-sign-2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/demo-multi-sign.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/demo-multi-sign.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/demo-with-basic-questions.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/demo-with-basic-questions.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/dependency-demo-code.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/dependency-demo-code.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/dependency-demo.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/dependency-demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/discovery.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/discovery.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/docxproperties.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/docxproperties.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/duplicate.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/duplicate.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/explain.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/explain.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/flags.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/flags.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/food-with-sig.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/food-with-sig.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/generic-document.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/generic-document.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/globalprofile.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/globalprofile.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/globalprofile2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/globalprofile2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/globalprofile3.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/globalprofile3.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-drive.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-drive.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-sheet-2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-sheet-2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-sheet-3.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-sheet-3.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/google-sheet.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/google-sheet.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/graph.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/graph.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/harry-potter-or-heidegger.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/harry-potter-or-heidegger.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/hook-on-gather.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/hook-on-gather.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/indexdemo.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/indexdemo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/indexdemoquery.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/indexdemoquery.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/interview_in_interview.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/interview_in_interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/jinjayaml.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/jinjayaml.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/jsondemo.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/jsondemo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/life_story.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/life_story.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/macros.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/macros.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background-2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background-2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/make-ocr-pdf-in-background.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/markdown-template.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/markdown-template.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/ml-export-playground.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/ml-export-playground.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/multi-signature.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/multi-signature.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/multi-user.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/multi-user.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/navbar-language.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/navbar-language.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/nested-list-docx-table.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/nested-list-docx-table.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/new-or-existing.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/new-or-existing.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/oauth-test-2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/oauth-test-2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/oauth-test-3.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/oauth-test-3.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/oauth-test-4.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/oauth-test-4.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/object-checkboxes-copy.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/object-checkboxes-copy.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/object-checkboxes-custom.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/object-checkboxes-custom.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/objects-from-file-gather.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/objects-from-file-gather.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/objects-from-file-template.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/objects-from-file-template.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/overlay-pdf.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/overlay-pdf.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/phone-number-2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/phone-number-2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/phone-number.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/phone-number.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/predict-activity-activity.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/predict-activity-activity.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/predict-activity.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/predict-activity.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/prevent-dependency-satisfaction.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/prevent-dependency-satisfaction.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/preview.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/preview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/primary-interview.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/primary-interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/progressive-disclosure.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/progressive-disclosure.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-dom.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-dom.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-hidden.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-hidden.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-log.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-log.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/pytojs-script.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/pytojs-script.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/quotes-in-code.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/quotes-in-code.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/random-forest-interview.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/random-forest-interview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/random-forest.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/random-forest.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/realtimegd.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/realtimegd.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/realtimegd2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/realtimegd2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/redact-docx.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/redact-docx.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/redact-pdf.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/redact-pdf.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/repeatable.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/repeatable.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/save-continue-later.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/save-continue-later.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/setparts.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/setparts.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/sign.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/sign.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signature-diversion.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signature-diversion.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signature-preview.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signature-preview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signature-template.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signature-template.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/signdoc.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/signdoc.yml`

 * *Files 1% similar despite different names*

```diff
@@ -385,15 +385,15 @@
   To include the date when the signer signs, you can write
   "{{ signature_date }}" in the place where you want the date to
   appear.  The format of the date will be "August 2, 2021."
   If you want the date to appear in numeric format, write
   "{{ signature_date.format('MM/dd/yyyy') }}".
 
   To include your signature as well, you can include
-  "{{ advocate_signature}}" and "{{ advocate_signature_date }}" in
+  "{{ advocate_signature }}" and "{{ advocate_signature_date }}" in
   the same way.  You will sign first before the document is sent
   to the signer.
 
   To include the signer's name, or your name, write "{{ signer }}" or
   "{{ advocate }}".
 ---
 template: pdf_file_instructions
@@ -814,10 +814,12 @@
 only sets: default_signature_updated_for_language
 code: |
   if get_language() == 'es':
     signature = '(Aquí aparecerá su firma)'
   default_signature_updated_for_language = True
 ---
 code: |
+  if defined('advocate_signature') and isinstance(advocate_signature, str):
+    undefine('advocate_signature')
   if defined('advocate_wants_to_keep_signature') and advocate_wants_to_keep_signature:
     store.set('signature', advocate_signature.slurp(auto_decode=False))
   advocate_signature_saved_if_necessary = True
```

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/single-code.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/single-code.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/snapshot.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/snapshot.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/someone-already-mentioned.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/someone-already-mentioned.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/stage-one.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/stage-one.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/stage-two.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/stage-two.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/subdoc-params.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/subdoc-params.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/subdocument.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/subdocument.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testcards.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testcards.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testcooking.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testcooking.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testdatabase.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testdatabase.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/testgeolocate.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/testgeolocate.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/translation.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/translation.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/turnips-worms.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/turnips-worms.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/universal-document.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/universal-document.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/update-references.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/update-references.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/validation-code.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/validation-code.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/watermark.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/watermark.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/wc_common.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/wc_common.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/examples/wc_side_of_bed.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/examples/wc_side_of_bed.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/hello4.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/hello4.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/hello5.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/hello5.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/hello6.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/hello6.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/list.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/list.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/questions.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/questions.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/roletest.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/roletest.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/roletestmany.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/roletestmany.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/sign.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/sign.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/test-sig-form.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/test-sig-form.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/test.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/test.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testaction.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testaction.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testaction2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testaction2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testattach.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testattach.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testbuildfl.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testbuildfl.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testbuildfl2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testbuildfl2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testcron.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testcron.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testcron2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testcron2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testcronbg.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testcronbg.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testdadict.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testdadict.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testdalist2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testdalist2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testdivorce.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testdivorce.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testemail.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testemail.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testfields.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testfields.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testgeneric.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testgeneric.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testimage.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testimage.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testlist0.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testlist0.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testobjects.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testobjects.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testpermissions.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testpermissions.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testpg.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testpg.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testpickle.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testpickle.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testplural.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testplural.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testproblem.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testproblem.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testpulldown.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testpulldown.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview2.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview2.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview3.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview3.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testreview4.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testreview4.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/questions/testunicode.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/questions/testunicode.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/claims.yml` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/claims.yml`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/contacts.json` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/contacts.json`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/context_es.xlsx` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/context_es.xlsx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/fruit_data.xlsx` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/fruit_data.xlsx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/ml-random-forest-interview.json` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/ml-random-forest-interview.json`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/ml-random-forest.json` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/ml-random-forest.json`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/questions_es.xlsx` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/questions_es.xlsx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/signdoc_es.xlsx` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/signdoc_es.xlsx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/testtr_en.xlsx` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/testtr_en.xlsx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/sources/testtr_es.xlsx` & `docassemble.demo-1.4.9/docassemble/demo/data/sources/testtr_es.xlsx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/abkhazia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/abkhazia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/accident3.eps` & `docassemble.demo-1.4.9/docassemble/demo/data/static/accident3.eps`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/accident3.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/accident3.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/accident3.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/accident3.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/afghanistan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/afghanistan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/aland-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/aland-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/albania.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/albania.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/algeria.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/algeria.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/american-samoa.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/american-samoa.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/andorra.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/andorra.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/angola.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/angola.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/anguilla.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/anguilla.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/antigua-and-barbuda.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/antigua-and-barbuda.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/argentina.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/argentina.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/armenia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/armenia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/art.jpg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/art.jpg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/aruba.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/aruba.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/australia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/australia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/austria.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/austria.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/azerbaijan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/azerbaijan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/azores-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/azores-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bahamas.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bahamas.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bahrain.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bahrain.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/balearic-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/balearic-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bangladesh.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bangladesh.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/barbados.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/barbados.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/basque-country.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/basque-country.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/belarus.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/belarus.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/belgium.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/belgium.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/belize.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/belize.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/benin.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/benin.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bermuda.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bermuda.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bhutan-1.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bhutan-1.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bhutan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bhutan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bolivia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bolivia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bonaire.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bonaire.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bosnia-and-herzegovina.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bosnia-and-herzegovina.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/botswana.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/botswana.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/brazil.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/brazil.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/british-columbia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/british-columbia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/british-indian-ocean-territory.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/british-indian-ocean-territory.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/british-virgin-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/british-virgin-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/brunei.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/brunei.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/bulgaria.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/bulgaria.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/burkina-faso.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/burkina-faso.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/burundi.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/burundi.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/button-checkboxes.css` & `docassemble.demo-1.4.9/docassemble/demo/data/static/button-checkboxes.css`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cambodia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cambodia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cameroon.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cameroon.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/canada.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/canada.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/canary-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/canary-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/canvas.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/canvas.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cape-verde.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cape-verde.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cayman-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cayman-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/central-african-republic.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/central-african-republic.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ceuta.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ceuta.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/chad.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/chad.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/chile.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/chile.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/china.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/china.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/christmas-island.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/christmas-island.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cocos-island.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cocos-island.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/colombia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/colombia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/comoros.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/comoros.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cook-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cook-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/corsica.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/corsica.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/costa-rica.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/costa-rica.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/crawling.eps` & `docassemble.demo-1.4.9/docassemble/demo/data/static/crawling.eps`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/crawling.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/crawling.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/crawling.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/crawling.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/croatia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/croatia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cuba.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cuba.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/curacao.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/curacao.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/cyprus.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/cyprus.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/czech-republic.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/czech-republic.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/datereplace.js` & `docassemble.demo-1.4.9/docassemble/demo/data/static/datereplace.js`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/democratic-republic-of-congo.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/democratic-republic-of-congo.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/denmark.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/denmark.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/djibouti.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/djibouti.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/dominica.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/dominica.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/dominican-republic.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/dominican-republic.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/draft.eps` & `docassemble.demo-1.4.9/docassemble/demo/data/static/draft.eps`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/east-timor.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/east-timor.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ecuador.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ecuador.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/egypt.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/egypt.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/england.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/england.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/equatorial-guinea.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/equatorial-guinea.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/eritrea.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/eritrea.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/estonia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/estonia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ethiopia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ethiopia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/european-union.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/european-union.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/falkland-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/falkland-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/faroe-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/faroe-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/favicon.ico` & `docassemble.demo-1.4.9/docassemble/demo/data/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/fiji.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/fiji.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/finland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/finland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/france.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/france.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/french-polynesia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/french-polynesia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/gabon.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/gabon.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/galapagos-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/galapagos-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/gambia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/gambia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/georgia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/georgia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/germany.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/germany.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ghana.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ghana.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/gibraltar.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/gibraltar.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/globe.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/globe.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/greece.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/greece.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/greenland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/greenland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/grenada.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/grenada.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/guam.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/guam.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/guatemala.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/guatemala.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/guernsey.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/guernsey.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/guinea-bissau.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/guinea-bissau.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/guinea.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/guinea.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/guyana.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/guyana.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/haiti.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/haiti.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/hawaii.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/hawaii.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/hello7.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/hello7.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/hello_planet.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/static/hello_planet.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/honduras.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/honduras.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/hong-kong.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/hong-kong.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/house.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/house.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/hungary.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/hungary.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/iceland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/iceland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/india.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/india.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/indonesia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/indonesia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/iran.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/iran.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/iraq.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/iraq.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ireland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ireland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/isle-of-man.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/isle-of-man.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/israel.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/israel.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/italy.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/italy.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ivory-coast.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ivory-coast.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/jamaica.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/jamaica.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/japan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/japan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/jersey.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/jersey.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/jordan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/jordan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/kazakhstan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/kazakhstan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/kenya.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/kenya.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/kiribati.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/kiribati.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/kosovo.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/kosovo.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/kuwait.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/kuwait.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/kyrgyzstan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/kyrgyzstan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/laos.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/laos.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/latvia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/latvia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/lebanon.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/lebanon.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/lesotho.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/lesotho.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/liberia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/liberia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/libya.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/libya.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/liechtenstein.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/liechtenstein.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/lithuania.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/lithuania.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/lumen.min.css` & `docassemble.demo-1.4.9/docassemble/demo/data/static/lumen.min.css`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/luxembourg.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/luxembourg.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/macao.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/macao.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/madagascar.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/madagascar.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/madeira.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/madeira.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/main_doc_params.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/static/main_doc_params.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/main_document.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/static/main_document.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/maindocpicture.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/maindocpicture.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/malawi.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/malawi.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/malaysia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/malaysia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/maldives.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/maldives.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/mali.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/mali.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/malta.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/malta.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/marshall-island.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/marshall-island.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/martinique.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/martinique.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/mauritania.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/mauritania.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/mauritius.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/mauritius.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/melilla.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/melilla.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/mexico.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/mexico.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/micronesia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/micronesia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/moldova.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/moldova.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/monaco.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/monaco.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/mongolia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/mongolia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/montenegro.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/montenegro.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/montserrat.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/montserrat.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/morocco.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/morocco.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/mozambique.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/mozambique.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/myanmar.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/myanmar.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/namibia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/namibia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/nato.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/nato.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/nauru.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/nauru.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/nepal.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/nepal.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/netherlands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/netherlands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/new-zealand.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/new-zealand.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/nicaragua.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/nicaragua.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/niger.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/niger.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/nigeria.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/nigeria.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/niue.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/niue.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/norfolk-island.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/norfolk-island.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/north-korea.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/north-korea.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/northen-cyprus.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/northen-cyprus.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/northern-marianas-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/northern-marianas-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/norway.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/norway.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/oman.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/oman.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/orkney-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/orkney-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ossetia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ossetia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/pakistan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/pakistan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/palau.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/palau.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/palestine.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/palestine.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/panama.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/panama.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/papua-new-guinea.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/papua-new-guinea.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/paraguay.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/paraguay.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/peru.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/peru.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/philippines.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/philippines.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/pitcairn-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/pitcairn-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/portugal.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/portugal.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/puerto-rico.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/puerto-rico.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/qatar.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/qatar.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/rapa-nui.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/rapa-nui.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/android-chrome-192x192.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/android-chrome-512x512.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/apple-touch-icon.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/favicon-16x16.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/favicon-32x32.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/favicon.ico` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/mstile-150x150.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/redicon/safari-pinned-tab.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/redicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/republic-of-macedonia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/republic-of-macedonia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/republic-of-poland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/republic-of-poland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/republic-of-the-congo.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/republic-of-the-congo.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/romania.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/romania.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/russia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/russia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/rwanda.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/rwanda.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/saba-island.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/saba-island.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/saint-kitts-and-nevis.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/saint-kitts-and-nevis.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/salvador.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/salvador.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/samoa.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/samoa.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sample-sig-form-2.pdf` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sample-sig-form-2.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sample-sig-form.pdf` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sample-sig-form.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sample-support-order.jpg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sample-support-order.jpg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/san-marino.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/san-marino.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sao-tome-and-principe.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sao-tome-and-principe.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sardinia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sardinia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/saudi-arabia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/saudi-arabia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-1.mp3` & `docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-1.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-1.ogg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-1.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-2.mp3` & `docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-2.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-2.ogg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-2.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-3.mp3` & `docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-3.mp3`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/schumann-clip-3.ogg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/schumann-clip-3.ogg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/scotland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/scotland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/senegal.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/senegal.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/serbia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/serbia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/seychelles.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/seychelles.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sierra-leone.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sierra-leone.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sign-here.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sign-here.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/singapore.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/singapore.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sint-eustatius.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sint-eustatius.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sint-maarten.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sint-maarten.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/slovakia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/slovakia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/slovenia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/slovenia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/solomon-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/solomon-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/somalia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/somalia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/somaliland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/somaliland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/south-africa.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/south-africa.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/south-korea.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/south-korea.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/south-sudan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/south-sudan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/spain.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/spain.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sri-lanka.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sri-lanka.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/st-barts.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/st-barts.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/st-lucia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/st-lucia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/st-vincent-and-the-grenadines.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/st-vincent-and-the-grenadines.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sub_doc_params.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sub_doc_params.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sub_document.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sub_document.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/subdocpicture.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/subdocpicture.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sudan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sudan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/suriname.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/suriname.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/swaziland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/swaziland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/sweden.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/sweden.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/switzerland.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/switzerland.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/syria.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/syria.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/taiwan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/taiwan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/tajikistan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/tajikistan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/tanzania.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/tanzania.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/thailand.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/thailand.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/tibet.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/tibet.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/togo.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/togo.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/tokelau.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/tokelau.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/tonga.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/tonga.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/transnistria.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/transnistria.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/trinidad-and-tobago.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/trinidad-and-tobago.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/tunisia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/tunisia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/turkey.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/turkey.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/turkmenistan.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/turkmenistan.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/turks-and-caicos.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/turks-and-caicos.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/tuvalu.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/tuvalu.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/uganda.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/uganda.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/ukraine.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/ukraine.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/united-arab-emirates.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/united-arab-emirates.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/united-kingdom.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/united-kingdom.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/united-nations.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/united-nations.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/united-states-of-america.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/united-states-of-america.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/universal-test.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/static/universal-test.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/uruguay.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/uruguay.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/users6.eps` & `docassemble.demo-1.4.9/docassemble/demo/data/static/users6.eps`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/users6.png` & `docassemble.demo-1.4.9/docassemble/demo/data/static/users6.png`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/users6.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/users6.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/uzbekistn.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/uzbekistn.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/vanuatu.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/vanuatu.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/vatican-city.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/vatican-city.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/venezuela.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/venezuela.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/vietnam.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/vietnam.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/virgin-islands.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/virgin-islands.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/wales.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/wales.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/western-sahara.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/western-sahara.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/yemen.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/yemen.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/zambia.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/zambia.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/static/zimbabwe.svg` & `docassemble.demo-1.4.9/docassemble/demo/data/static/zimbabwe.svg`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/Agreement_To_Transfer.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/Agreement_To_Transfer.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/Transfer-of-Ownership.pdf` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/Transfer-of-Ownership.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/context.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/context.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/contract.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/contract.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/declaration_certificate_service.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/declaration_certificate_service.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/declaration_of_favorite_fruit.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/declaration_of_favorite_fruit.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/doc-with-toc.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/doc-with-toc.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/docx-with-metadata.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/docx-with-metadata.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/exhibit_insert.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/exhibit_insert.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/food_template.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/food_template.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/fruit_declaration.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/fruit_declaration.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/generic-document.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/generic-document.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/graph.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/graph.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/hello_planet.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/hello_planet.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/life_story.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/life_story.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/logo_template.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/logo_template.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/main_doc_params.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/main_doc_params.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/main_document.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/main_document.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/markdown_template_demo.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/markdown_template_demo.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/myinterviews.html` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/myinterviews.html`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/nested_list_table.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/nested_list_table.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/numbering_template.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/numbering_template.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/quotes-in-code.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/quotes-in-code.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/redact_demo.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/redact_demo.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/redact_demo.pdf` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/redact_demo.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/sample-sig-form-2.pdf` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/sample-sig-form-2.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/sample-sig-form.pdf` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/sample-sig-form.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/signature_template.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/signature_template.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/sub_doc_params.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/sub_doc_params.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/sub_document.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/sub_document.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/tagged.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/tagged.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/team.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/team.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/template_test.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/template_test.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/testsigform.pdf` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/testsigform.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/data/templates/twostage.docx` & `docassemble.demo-1.4.9/docassemble/demo/data/templates/twostage.docx`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/demodb.py` & `docassemble.demo-1.4.9/docassemble/demo/demodb.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/fishlist.py` & `docassemble.demo-1.4.9/docassemble/demo/fishlist.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/fruit_database.py` & `docassemble.demo-1.4.9/docassemble/demo/fruit_database.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/google_drive.py` & `docassemble.demo-1.4.9/docassemble/demo/google_drive.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/google_sheets.py` & `docassemble.demo-1.4.9/docassemble/demo/google_sheets.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/google_vision2.py` & `docassemble.demo-1.4.9/docassemble/demo/google_vision2.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/income.py` & `docassemble.demo-1.4.9/docassemble/demo/income.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/index.py` & `docassemble.demo-1.4.9/docassemble/demo/index.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/oauthsheets.py` & `docassemble.demo-1.4.9/docassemble/demo/oauthsheets.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/progressivedisclosure.py` & `docassemble.demo-1.4.9/docassemble/demo/progressivedisclosure.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/random-test.py` & `docassemble.demo-1.4.9/docassemble/demo/random-test.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/reldemodb.py` & `docassemble.demo-1.4.9/docassemble/demo/reldemodb.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/sign.py` & `docassemble.demo-1.4.9/docassemble/demo/sign.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/ssn.py` & `docassemble.demo-1.4.9/docassemble/demo/ssn.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/testcontexttest.py` & `docassemble.demo-1.4.9/docassemble/demo/testcontexttest.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/translate.py` & `docassemble.demo-1.4.9/docassemble/demo/translate.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble/demo/user_permissions.py` & `docassemble.demo-1.4.9/docassemble/demo/user_permissions.py`

 * *Files identical despite different names*

### Comparing `docassemble.demo-1.4.8/docassemble.demo.egg-info/PKG-INFO` & `docassemble.demo-1.4.9/docassemble.demo.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble.demo
-Version: 1.4.8
+Version: 1.4.9
 Summary: A demonstration package for docassemble.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Description: See the [docassemble web site] for a description of **docassemble**
         and installation instructions.
```

### Comparing `docassemble.demo-1.4.8/docassemble.demo.egg-info/SOURCES.txt` & `docassemble.demo-1.4.9/docassemble.demo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 docassemble/demo/data/questions/examples/objects-from-file-dadict.yml
 docassemble/demo/data/questions/examples/objects-from-file-gather.yml
 docassemble/demo/data/questions/examples/objects-from-file-json.yml
 docassemble/demo/data/questions/examples/objects-from-file-template.yml
 docassemble/demo/data/questions/examples/objects-from-file.yml
 docassemble/demo/data/questions/examples/overlay-pdf-multi.yml
 docassemble/demo/data/questions/examples/overlay-pdf.yml
+docassemble/demo/data/questions/examples/pdfextract.yml
 docassemble/demo/data/questions/examples/phone-number-2.yml
 docassemble/demo/data/questions/examples/phone-number.yml
 docassemble/demo/data/questions/examples/predict-activity-activity.yml
 docassemble/demo/data/questions/examples/predict-activity.yml
 docassemble/demo/data/questions/examples/predict-happy-sad-area.yml
 docassemble/demo/data/questions/examples/predict-happy-sad.yml
 docassemble/demo/data/questions/examples/prevent-dependency-satisfaction.yml
```

### Comparing `docassemble.demo-1.4.8/setup.py` & `docassemble.demo-1.4.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,26 +42,26 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.demo',
-      version='1.4.8',
+      version='1.4.9',
       python_requires='>=3.8',
       description=('A demonstration package for docassemble.'),
       long_description=read("README.md"),
       long_description_content_type='text/markdown',
       author='Jonathan Pyle',
       author_email='jhpyle@gmail.com',
       license='MIT',
       url='https://docassemble.org',
       packages=find_packages(),
       namespace_packages=['docassemble'],
       install_requires=[
-          'docassemble==1.4.8',
-          'docassemble.base==1.4.8',
+          'docassemble==1.4.9',
+          'docassemble.base==1.4.9',
           'googledrivedownloader==0.4'
       ],
       zip_safe=False,
       package_data=find_package_data(where=os.path.join('docassemble', 'demo', ''), package='docassemble.demo')
       )
```

