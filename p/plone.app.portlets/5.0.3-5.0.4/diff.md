# Comparing `tmp/plone.app.portlets-5.0.3.tar.gz` & `tmp/plone.app.portlets-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.portlets-5.0.3.tar", last modified: Thu Apr 13 23:03:13 2023, max compression
+gzip compressed data, was "plone.app.portlets-5.0.4.tar", last modified: Mon May  8 19:38:08 2023, max compression
```

## Comparing `plone.app.portlets-5.0.3.tar` & `plone.app.portlets-5.0.4.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.187247 plone.app.portlets-5.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)    43723 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    45206 2023-04-13 23:03:13.187381 plone.app.portlets-5.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      510 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.149635 plone.app.portlets-5.0.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      680 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.149863 plone.app.portlets-5.0.3/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.152371 plone.app.portlets-5.0.3/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.158077 plone.app.portlets-5.0.3/plone/app/portlets/
--rw-r--r--   0 maurits    (501) staff       (20)      471 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/TODO.rst
--rw-r--r--   0 maurits    (501) staff       (20)       76 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1403 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/assignable.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.161801 plone.app.portlets-5.0.3/plone/app/portlets/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1979 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/adding.py
--rw-r--r--   0 maurits    (501) staff       (20)     7046 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    17971 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/editmanager.py
--rw-r--r--   0 maurits    (501) staff       (20)     8056 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/formhelper.py
--rw-r--r--   0 maurits    (501) staff       (20)     2081 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    13954 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/manage.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.167840 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      299 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/column.pt
--rw-r--r--   0 maurits    (501) staff       (20)      269 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/dashboard-column.pt
--rw-r--r--   0 maurits    (501) staff       (20)     8707 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/edit-manager-contextual.pt
--rw-r--r--   0 maurits    (501) staff       (20)     8900 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/edit-manager-macros.pt
--rw-r--r--   0 maurits    (501) staff       (20)      595 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/edit-manager.pt
--rw-r--r--   0 maurits    (501) staff       (20)      573 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/error_message.pt
--rw-r--r--   0 maurits    (501) staff       (20)      165 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/footer.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1639 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-content-type.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3844 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-contextual.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2242 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-dashboard.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2794 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-group-dashboard.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2622 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-group.pt
--rw-r--r--   0 maurits    (501) staff       (20)      403 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage_portlets_fallback.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1022 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/portlets-pageform.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3527 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/topbar-manage-portlets.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1299 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/z3cform-portlets-pageform.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5137 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     1214 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2679 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/browser/viewlets.py
--rw-r--r--   0 maurits    (501) staff       (20)     1109 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/cache.py
--rw-r--r--   0 maurits    (501) staff       (20)     2095 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/checker.py
--rw-r--r--   0 maurits    (501) staff       (20)     2103 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.170166 plone.app.portlets-5.0.3/plone/app/portlets/dashboard/
--rw-r--r--   0 maurits    (501) staff       (20)     2048 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/dashboard/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      728 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/dashboard/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/dashboard/dashboard.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/dashboard/dashboard.py
--rw-r--r--   0 maurits    (501) staff       (20)     1296 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/dashboard/user_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)      393 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/dashboard/user_actions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.171271 plone.app.portlets-5.0.3/plone/app/portlets/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1072 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      750 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/exportimport/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    29504 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/exportimport/portlets.py
--rw-r--r--   0 maurits    (501) staff       (20)     3738 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2639 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/manager.py
--rw-r--r--   0 maurits    (501) staff       (20)      549 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5155 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/metaconfigure.py
--rw-r--r--   0 maurits    (501) staff       (20)     3978 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/metadirectives.py
--rw-r--r--   0 maurits    (501) staff       (20)      276 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1398 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/permissions.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3467 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portletcontext.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.179198 plone.app.portlets-5.0.3/plone/app/portlets/portlets/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1829 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     6461 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)     2912 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/base.py
--rw-r--r--   0 maurits    (501) staff       (20)      111 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/calendar.py
--rw-r--r--   0 maurits    (501) staff       (20)      386 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/classic.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1993 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/classic.py
--rw-r--r--   0 maurits    (501) staff       (20)     2579 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/deferred_portlet.pt
--rw-r--r--   0 maurits    (501) staff       (20)      109 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     1680 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/language.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/language.py
--rw-r--r--   0 maurits    (501) staff       (20)     6140 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/login.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3262 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/login.py
--rw-r--r--   0 maurits    (501) staff       (20)     2315 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/navigation.pt
--rw-r--r--   0 maurits    (501) staff       (20)    18115 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)     3618 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/navigation_recurse.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2529 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/news.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4946 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/news.py
--rw-r--r--   0 maurits    (501) staff       (20)     3193 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/recent.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5291 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/recent.py
--rw-r--r--   0 maurits    (501) staff       (20)     2595 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/review.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5686 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/review.py
--rw-r--r--   0 maurits    (501) staff       (20)     2032 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/rss.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10922 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/rss.py
--rw-r--r--   0 maurits    (501) staff       (20)     2741 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/search.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2042 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/portlets/search.py
--rw-r--r--   0 maurits    (501) staff       (20)     5440 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/storage.py
--rw-r--r--   0 maurits    (501) staff       (20)     2009 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.186745 plone.app.portlets-5.0.3/plone/app/portlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)       51 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/atom_feed_maurits.xml
--rw-r--r--   0 maurits    (501) staff       (20)      661 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.146755 plone.app.portlets-5.0.3/plone/app/portlets/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.187044 plone.app.portlets-5.0.3/plone/app/portlets/tests/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)     3994 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/profiles/testing/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)      568 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/testDoctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     4196 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/testMemberDashboard.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8988 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_actions_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1821 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_cache.py
--rw-r--r--   0 maurits    (501) staff       (20)     4901 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_classic_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)    20221 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_configuration.py
--rw-r--r--   0 maurits    (501) staff       (20)     4544 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_context.py
--rw-r--r--   0 maurits    (501) staff       (20)     1814 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_dashboard.py
--rw-r--r--   0 maurits    (501) staff       (20)    15274 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)    10158 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_formextender.py
--rw-r--r--   0 maurits    (501) staff       (20)     5313 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_login_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)      508 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_manage_views.py
--rw-r--r--   0 maurits    (501) staff       (20)     2953 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_mapping.py
--rw-r--r--   0 maurits    (501) staff       (20)      565 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_namechooser.py
--rw-r--r--   0 maurits    (501) staff       (20)    28745 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_navigation_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     5186 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_news_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     4996 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_recent_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     2060 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_redirects.py
--rw-r--r--   0 maurits    (501) staff       (20)     5476 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_review_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     5387 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_rss_portlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     2088 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     4207 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     3732 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)      283 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     5365 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/plone/app/portlets/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:03:13.152072 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    45206 2023-04-13 23:03:13.000000 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5100 2023-04-13 23:03:13.000000 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:03:13.000000 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:03:13.000000 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:03:13.000000 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      542 2023-04-13 23:03:13.000000 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:03:13.000000 plone.app.portlets-5.0.3/plone.app.portlets.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-13 23:03:13.187972 plone.app.portlets-5.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2320 2023-04-13 23:03:12.000000 plone.app.portlets-5.0.3/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.256393 plone.app.portlets-5.0.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    43864 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    45347 2023-05-08 19:38:08.256607 plone.app.portlets-5.0.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      510 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.206073 plone.app.portlets-5.0.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      680 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.206477 plone.app.portlets-5.0.4/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.209967 plone.app.portlets-5.0.4/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.217019 plone.app.portlets-5.0.4/plone/app/portlets/
+-rw-r--r--   0 maurits    (501) staff       (20)      471 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/TODO.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1403 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/assignable.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.221171 plone.app.portlets-5.0.4/plone/app/portlets/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1979 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/adding.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7046 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    17971 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/editmanager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8056 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/formhelper.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2081 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13954 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/manage.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.227943 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)      299 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/column.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      269 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/dashboard-column.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     8707 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/edit-manager-contextual.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     8900 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/edit-manager-macros.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      595 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/edit-manager.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      573 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/error_message.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      165 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/footer.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1639 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-content-type.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3844 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-contextual.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2242 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-dashboard.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2794 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-group-dashboard.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2622 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-group.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      403 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage_portlets_fallback.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1022 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/portlets-pageform.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3527 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/topbar-manage-portlets.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1299 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/z3cform-portlets-pageform.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5137 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1214 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2679 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/browser/viewlets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1109 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/cache.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2095 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/checker.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2103 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.230475 plone.app.portlets-5.0.4/plone/app/portlets/dashboard/
+-rw-r--r--   0 maurits    (501) staff       (20)     2048 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/dashboard/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      728 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/dashboard/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2295 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/dashboard/dashboard.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2405 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/dashboard/dashboard.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1296 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/dashboard/user_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/dashboard/user_actions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.232131 plone.app.portlets-5.0.4/plone/app/portlets/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1072 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      750 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/exportimport/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29504 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/exportimport/portlets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3738 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2639 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/manager.py
+-rw-r--r--   0 maurits    (501) staff       (20)      549 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5155 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/metaconfigure.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3978 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/metadirectives.py
+-rw-r--r--   0 maurits    (501) staff       (20)      276 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1398 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/permissions.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3467 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portletcontext.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.243448 plone.app.portlets-5.0.4/plone/app/portlets/portlets/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1829 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     6461 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2912 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)      228 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/calendar.py
+-rw-r--r--   0 maurits    (501) staff       (20)      386 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/classic.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1993 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/classic.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2579 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/deferred_portlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      224 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1680 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/language.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/language.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6140 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/login.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3262 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/login.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2315 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/navigation.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    18115 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/navigation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3618 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/navigation_recurse.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2529 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/news.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4946 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/news.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3193 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/recent.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5291 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/recent.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2595 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/review.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5686 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/review.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2032 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/rss.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10922 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/rss.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2741 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/search.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2042 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/portlets/search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5440 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/storage.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2009 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.255559 plone.app.portlets-5.0.4/plone/app/portlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)       51 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/atom_feed_maurits.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.202246 plone.app.portlets-5.0.4/plone/app/portlets/tests/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.255994 plone.app.portlets-5.0.4/plone/app/portlets/tests/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)     3994 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/profiles/testing/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      568 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/testDoctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4196 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/testMemberDashboard.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8988 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_actions_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1821 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_cache.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4901 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_classic_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20221 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_configuration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4544 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1814 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_dashboard.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15274 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10158 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_formextender.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5313 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_login_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)      508 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_manage_views.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2953 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_mapping.py
+-rw-r--r--   0 maurits    (501) staff       (20)      565 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_namechooser.py
+-rw-r--r--   0 maurits    (501) staff       (20)    28745 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_navigation_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5186 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_news_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4996 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_recent_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2060 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_redirects.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5476 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_review_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5387 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_rss_portlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2088 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4207 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3732 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)      283 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/tests/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5365 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/plone/app/portlets/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:38:08.209553 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    45347 2023-05-08 19:38:08.000000 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5100 2023-05-08 19:38:08.000000 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:38:08.000000 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-08 19:38:08.000000 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:38:08.000000 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      526 2023-05-08 19:38:08.000000 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:38:08.000000 plone.app.portlets-5.0.4/plone.app.portlets.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1722 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-08 19:38:08.257349 plone.app.portlets-5.0.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2293 2023-05-08 19:38:07.000000 plone.app.portlets-5.0.4/setup.py
```

### Comparing `plone.app.portlets-5.0.3/CHANGES.rst` & `plone.app.portlets-5.0.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Fix circular dependency on `plone.app.event`.
+  [@jensens] (fix-circular-dependency)
+
+
 5.0.3 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files, declare dependencies.
```

### Comparing `plone.app.portlets-5.0.3/PKG-INFO` & `plone.app.portlets-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: plone.app.portlets
-Version: 5.0.3
+Version: 5.0.4
 Summary: Plone integration for the basic plone.portlets package
-Home-page: https://pypi.org/project/plone.app.portlets
+Home-page: https://github.com/plone/plone.app.portlets
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: portlets viewlets plone
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -45,14 +45,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Fix circular dependency on `plone.app.event`.
+  [@jensens] (fix-circular-dependency)
+
+
 5.0.3 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files, declare dependencies.
```

### Comparing `plone.app.portlets-5.0.3/docs/LICENSE.GPL` & `plone.app.portlets-5.0.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/docs/LICENSE.txt` & `plone.app.portlets-5.0.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/assignable.py` & `plone.app.portlets-5.0.4/plone/app/portlets/assignable.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/adding.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/adding.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/configure.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/editmanager.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/editmanager.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/formhelper.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/formhelper.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/interfaces.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/manage.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/manage.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/edit-manager-contextual.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/edit-manager-contextual.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/edit-manager-macros.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/edit-manager-macros.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/edit-manager.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/edit-manager.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/error_message.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/error_message.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-content-type.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-content-type.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-contextual.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-contextual.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-dashboard.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-dashboard.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-group-dashboard.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-group-dashboard.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/manage-group.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/manage-group.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/portlets-pageform.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/portlets-pageform.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/topbar-manage-portlets.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/topbar-manage-portlets.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/templates/z3cform-portlets-pageform.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/templates/z3cform-portlets-pageform.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/traversal.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/utils.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/browser/viewlets.py` & `plone.app.portlets-5.0.4/plone/app/portlets/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/cache.py` & `plone.app.portlets-5.0.4/plone/app/portlets/cache.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/checker.py` & `plone.app.portlets-5.0.4/plone/app/portlets/checker.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/configure.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/dashboard/__init__.py` & `plone.app.portlets-5.0.4/plone/app/portlets/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/dashboard/configure.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/dashboard/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/dashboard/dashboard.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/dashboard/dashboard.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/dashboard/dashboard.py` & `plone.app.portlets-5.0.4/plone/app/portlets/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/dashboard/user_actions.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/dashboard/user_actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/exportimport/configure.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/exportimport/interfaces.py` & `plone.app.portlets-5.0.4/plone/app/portlets/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/exportimport/portlets.py` & `plone.app.portlets-5.0.4/plone/app/portlets/exportimport/portlets.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/interfaces.py` & `plone.app.portlets-5.0.4/plone/app/portlets/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/manager.py` & `plone.app.portlets-5.0.4/plone/app/portlets/manager.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/meta.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/meta.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/metaconfigure.py` & `plone.app.portlets-5.0.4/plone/app/portlets/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/metadirectives.py` & `plone.app.portlets-5.0.4/plone/app/portlets/metadirectives.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/permissions.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/permissions.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portletcontext.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portletcontext.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/actions.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/actions.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/actions.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/base.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/classic.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/classic.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/configure.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/language.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/language.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/language.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/language.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/login.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/login.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/login.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/login.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/navigation.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/navigation.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/navigation.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/navigation_recurse.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/navigation_recurse.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/news.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/news.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/news.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/news.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/recent.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/recent.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/recent.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/recent.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/review.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/review.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/review.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/review.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/rss.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/rss.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/rss.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/rss.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/search.pt` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/search.pt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/portlets/search.py` & `plone.app.portlets-5.0.4/plone/app/portlets/portlets/search.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/storage.py` & `plone.app.portlets-5.0.4/plone/app/portlets/storage.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/testing.py` & `plone.app.portlets-5.0.4/plone/app/portlets/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/base.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/configure.zcml` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/profiles/testing/portlets.xml` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/profiles/testing/portlets.xml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/testDoctests.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/testDoctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/testMemberDashboard.rst` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/testMemberDashboard.rst`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_actions_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_actions_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_cache.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_classic_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_classic_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_configuration.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_context.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_dashboard.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_exportimport.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_formextender.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_formextender.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_login_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_login_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_mapping.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_namechooser.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_namechooser.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_navigation_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_navigation_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_news_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_news_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_recent_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_recent_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_redirects.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_review_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_review_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_rss_portlet.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_rss_portlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_setup.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_traversal.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/tests/test_utils.py` & `plone.app.portlets-5.0.4/plone/app/portlets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone/app/portlets/utils.py` & `plone.app.portlets-5.0.4/plone/app/portlets/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone.app.portlets.egg-info/PKG-INFO` & `plone.app.portlets-5.0.4/plone.app.portlets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: plone.app.portlets
-Version: 5.0.3
+Version: 5.0.4
 Summary: Plone integration for the basic plone.portlets package
-Home-page: https://pypi.org/project/plone.app.portlets
+Home-page: https://github.com/plone/plone.app.portlets
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: portlets viewlets plone
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
@@ -45,14 +45,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.4 (2023-05-08)
+------------------
+
+Bug fixes:
+
+
+- Fix circular dependency on `plone.app.event`.
+  [@jensens] (fix-circular-dependency)
+
+
 5.0.3 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files, declare dependencies.
```

### Comparing `plone.app.portlets-5.0.3/plone.app.portlets.egg-info/SOURCES.txt` & `plone.app.portlets-5.0.4/plone.app.portlets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/plone.app.portlets.egg-info/requires.txt` & `plone.app.portlets-5.0.4/plone.app.portlets.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 setuptools
 plone.base
 Zope
 BTrees
 ExtensionClass
 feedparser
 five.customerize
-plone.app.event
 plone.app.i18n
 plone.app.layout
 plone.app.uuid
 plone.app.vocabularies
 plone.app.z3cform
 plone.autoform
 plone.i18n
```

### Comparing `plone.app.portlets-5.0.3/pyproject.toml` & `plone.app.portlets-5.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.portlets-5.0.3/setup.py` & `plone.app.portlets-5.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "5.0.3"
+version = "5.0.4"
 
 setup(
     name="plone.app.portlets",
     version=version,
     description="Plone integration for the basic plone.portlets package",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
@@ -23,15 +23,15 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     keywords="portlets viewlets plone",
     author="Plone Foundation",
     author_email="plone-developers@lists.sourceforge.net",
-    url="https://pypi.org/project/plone.app.portlets",
+    url="https://github.com/plone/plone.app.portlets",
     license="GPL version 2",
     packages=find_packages(),
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     extras_require=dict(
@@ -48,15 +48,14 @@
         "setuptools",
         "plone.base",
         "Zope",
         "BTrees",
         "ExtensionClass",
         "feedparser",
         "five.customerize",
-        "plone.app.event",
         "plone.app.i18n",
         "plone.app.layout",
         "plone.app.uuid",
         "plone.app.vocabularies",
         "plone.app.z3cform",
         "plone.autoform",
         "plone.i18n",
```

