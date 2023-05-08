# Comparing `tmp/plone.app.dexterity-3.0.5.tar.gz` & `tmp/plone.app.dexterity-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.dexterity-3.0.5.tar", last modified: Thu Apr 13 23:00:21 2023, max compression
+gzip compressed data, was "plone.app.dexterity-3.1.0.tar", last modified: Mon May  8 19:40:13 2023, max compression
```

## Comparing `plone.app.dexterity-3.0.5.tar` & `plone.app.dexterity-3.1.0.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.884066 plone.app.dexterity-3.0.5/
--rw-r--r--   0 maurits    (501) staff       (20)    32040 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    44362 2023-04-13 23:00:21.884211 plone.app.dexterity-3.0.5/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6519 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4640 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/RELEASE_NOTES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.837452 plone.app.dexterity-3.0.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      760 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3310 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/Makefile
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.842091 plone.app.dexterity-3.0.5/docs/advanced/
--rw-r--r--   0 maurits    (501) staff       (20)     1951 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14910 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/catalog-indexing-strategies.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9635 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/custom-add-and-edit-forms.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3181 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/custom-content-classes.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2145 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/defaults.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5191 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/event-handlers.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4599 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/files-and-images.rst
--rw-r--r--   0 maurits    (501) staff       (20)      492 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6971 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/permissions.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/references.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7451 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/rich-text-markup-transformations.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5276 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/static-resources.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3814 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/validators.rst
--rw-r--r--   0 maurits    (501) staff       (20)    13226 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/vocabularies.rst
--rw-r--r--   0 maurits    (501) staff       (20)    21829 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/webdav-and-other-file-representations.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16315 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/advanced/workflow.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.844355 plone.app.dexterity-3.0.5/docs/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/behavior-basics.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5438 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/creating-and-registering-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2083 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10191 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/providing-marker-interfaces.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5855 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/schema-only-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)    11007 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/behaviors/testing-behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7095 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)    10739 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/custom-views.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2354 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/designing.rst
--rw-r--r--   0 maurits    (501) staff       (20)      460 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)      943 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/install.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/intro.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/model-driven-types.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6303 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/prerequisite.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.846612 plone.app.dexterity-3.0.5/docs/reference/
--rw-r--r--   0 maurits    (501) staff       (20)     9806 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/dexterity-xml.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14982 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/fields.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8261 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/form-schema-hints.rst
--rw-r--r--   0 maurits    (501) staff       (20)      270 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    35076 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/manipulating-content-objects.rst
--rw-r--r--   0 maurits    (501) staff       (20)      871 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/misc.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6133 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/standard-behaviours.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3419 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/reference/widgets.rst
--rw-r--r--   0 maurits    (501) staff       (20)    16977 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/schema-driven-types.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.847821 plone.app.dexterity-3.0.5/docs/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)    14392 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/integration-tests.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10941 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/mock-testing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/docs/testing/unit-tests.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.848084 plone.app.dexterity-3.0.5/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.851495 plone.app.dexterity-3.0.5/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.854796 plone.app.dexterity-3.0.5/plone/app/dexterity/
--rw-r--r--   0 maurits    (501) staff       (20)      672 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)       76 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.857800 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5114 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     6908 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     1102 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/discussion.py
--rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/exclfromnav.py
--rw-r--r--   0 maurits    (501) staff       (20)      963 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/filename.py
--rw-r--r--   0 maurits    (501) staff       (20)     1808 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/id.py
--rw-r--r--   0 maurits    (501) staff       (20)    12317 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/metadata.py
--rw-r--r--   0 maurits    (501) staff       (20)     4533 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)      441 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/related.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.858899 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2827 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_contrains.py
--rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_id.py
--rw-r--r--   0 maurits    (501) staff       (20)     4370 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_metadata.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.866950 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/add_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     1597 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/behaviors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4442 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/blank.css
--rw-r--r--   0 maurits    (501) staff       (20)     1223 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/clone_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     4177 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1740 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/container.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/default_page_warning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/export.py
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     6792 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3408 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.py
--rw-r--r--   0 maurits    (501) staff       (20)     6391 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/import_types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1307 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/item.pt
--rw-r--r--   0 maurits    (501) staff       (20)      429 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     2493 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/modeleditor.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5644 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/modeleditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     2264 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.py
--rw-r--r--   0 maurits    (501) staff       (20)     1297 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/tabbed_forms.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10142 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1098 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1350 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing_row.pt
--rw-r--r--   0 maurits    (501) staff       (20)      710 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/typesformwrapper.pt
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/browser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      547 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/events.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2219 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/factories.py
--rw-r--r--   0 maurits    (501) staff       (20)     3667 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      482 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      271 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/overrides.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4664 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/permissions.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.830563 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.867606 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      186 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/default/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.868126 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      248 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.868654 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2214 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Document.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2467 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Folder.xml
--rw-r--r--   0 maurits    (501) staff       (20)      356 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1661 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/serialize.py
--rw-r--r--   0 maurits    (501) staff       (20)     1074 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.873270 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/discussion.txt
--rw-r--r--   0 maurits    (501) staff       (20)    22722 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/editing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1851 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/filename.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.873619 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/import/
--rw-r--r--   0 maurits    (501) staff       (20)     5804 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/import/dexterity_export.zip
--rw-r--r--   0 maurits    (501) staff       (20)     2498 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/metadata.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/namefromtitle.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3592 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/nextprevious.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.873892 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/robot/test_types.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/schema_events.txt
--rw-r--r--   0 maurits    (501) staff       (20)    19024 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_constrains.py
--rw-r--r--   0 maurits    (501) staff       (20)      778 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     1857 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_export.py
--rw-r--r--   0 maurits    (501) staff       (20)     2851 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_import.py
--rw-r--r--   0 maurits    (501) staff       (20)     8202 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_nextprevious.py
--rw-r--r--   0 maurits    (501) staff       (20)     9191 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_permissions.py
--rw-r--r--   0 maurits    (501) staff       (20)      826 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_robot.py
--rw-r--r--   0 maurits    (501) staff       (20)     1586 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_upgrades.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.877166 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/
--rw-r--r--   0 maurits    (501) staff       (20)      555 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      293 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5051 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/converters.py
--rw-r--r--   0 maurits    (501) staff       (20)      890 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/indexer.py
--rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2339 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     1340 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/supermodel.py
--rw-r--r--   0 maurits    (501) staff       (20)     2662 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.880573 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)    11423 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    21311 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/file.pdf
--rw-r--r--   0 maurits    (501) staff       (20)      376 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/helpers.py
--rw-r--r--   0 maurits    (501) staff       (20)      434 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
--rw-r--r--   0 maurits    (501) staff       (20)      792 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_behaviors.py
--rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_directives.py
--rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     3767 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
--rw-r--r--   0 maurits    (501) staff       (20)     1793 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.883795 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2416 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      249 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to1.py
--rw-r--r--   0 maurits    (501) staff       (20)      195 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2.py
--rw-r--r--   0 maurits    (501) staff       (20)      221 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2000.py
--rw-r--r--   0 maurits    (501) staff       (20)      631 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2001.py
--rw-r--r--   0 maurits    (501) staff       (20)      268 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2002.py
--rw-r--r--   0 maurits    (501) staff       (20)      606 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2003.py
--rw-r--r--   0 maurits    (501) staff       (20)      976 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2004.py
--rw-r--r--   0 maurits    (501) staff       (20)     1444 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2005.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:00:21.851255 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    44362 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     6632 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      829 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      287 2023-04-13 23:00:21.884672 plone.app.dexterity-3.0.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     3209 2023-04-13 23:00:21.000000 plone.app.dexterity-3.0.5/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.121605 plone.app.dexterity-3.1.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    32191 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    44513 2023-05-08 19:40:13.121822 plone.app.dexterity-3.1.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6519 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4640 2023-05-08 19:40:11.000000 plone.app.dexterity-3.1.0/RELEASE_NOTES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.057749 plone.app.dexterity-3.1.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    12282 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      760 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3310 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/Makefile
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.064704 plone.app.dexterity-3.1.0/docs/advanced/
+-rw-r--r--   0 maurits    (501) staff       (20)     1951 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14910 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/catalog-indexing-strategies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9635 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/custom-add-and-edit-forms.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3181 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/custom-content-classes.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2145 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/defaults.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5191 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/event-handlers.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4599 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/files-and-images.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      492 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6971 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/permissions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7156 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/references.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7451 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/rich-text-markup-transformations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5276 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/static-resources.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3814 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/validators.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    13226 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/vocabularies.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    21829 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/webdav-and-other-file-representations.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16315 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/advanced/workflow.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.067620 plone.app.dexterity-3.1.0/docs/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)     1931 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/behavior-basics.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5438 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/creating-and-registering-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2083 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10191 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/providing-marker-interfaces.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5855 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/schema-only-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    11007 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/behaviors/testing-behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7095 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10739 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/custom-views.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2354 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/designing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      460 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      943 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/install.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5693 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/intro.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3973 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/model-driven-types.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6303 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/prerequisite.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.071017 plone.app.dexterity-3.1.0/docs/reference/
+-rw-r--r--   0 maurits    (501) staff       (20)     9806 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/dexterity-xml.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14982 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/fields.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8261 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/form-schema-hints.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      270 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    35076 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/manipulating-content-objects.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      871 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/misc.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6133 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/standard-behaviours.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3419 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/reference/widgets.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    16977 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/schema-driven-types.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.072674 plone.app.dexterity-3.1.0/docs/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    14392 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/integration-tests.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10941 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/mock-testing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     5860 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/docs/testing/unit-tests.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.073091 plone.app.dexterity-3.1.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.076912 plone.app.dexterity-3.1.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.081401 plone.app.dexterity-3.1.0/plone/app/dexterity/
+-rw-r--r--   0 maurits    (501) staff       (20)      672 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       76 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.085468 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5114 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     6908 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1102 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/discussion.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1759 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/exclfromnav.py
+-rw-r--r--   0 maurits    (501) staff       (20)      963 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/filename.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1808 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/id.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12317 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/metadata.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4533 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)      441 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/related.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.087044 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2827 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_contrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5128 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_id.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4370 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_metadata.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.097647 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1751 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/add_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2884 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5024 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/blank.css
+-rw-r--r--   0 maurits    (501) staff       (20)     1223 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/clone_type.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4177 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1740 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/container.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/default_page_warning.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     4539 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6792 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3408 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6391 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/import_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1307 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/item.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      429 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2493 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5644 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2264 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1177 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1297 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/tabbed_forms.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10142 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1098 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1350 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing_row.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      710 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/typesformwrapper.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/browser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2770 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      547 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/events.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2219 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/factories.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3667 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      482 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      271 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/overrides.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4664 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/permissions.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.047597 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.098486 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      186 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.099321 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      248 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.100149 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2214 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Document.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2467 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Folder.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      356 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1661 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/serialize.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1074 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.106796 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/discussion.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    22722 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/editing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1851 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/filename.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.107213 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/import/
+-rw-r--r--   0 maurits    (501) staff       (20)     5804 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/import/dexterity_export.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     2498 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/metadata.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1777 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/namefromtitle.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3592 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/nextprevious.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.107647 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     1082 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/robot/test_types.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1458 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/schema_events.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    19024 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_constrains.py
+-rw-r--r--   0 maurits    (501) staff       (20)      778 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1857 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2851 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8202 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_nextprevious.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9191 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_permissions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      826 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_robot.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1586 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_upgrades.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.112191 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/
+-rw-r--r--   0 maurits    (501) staff       (20)      555 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      293 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2066 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5051 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/converters.py
+-rw-r--r--   0 maurits    (501) staff       (20)      890 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5290 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/indexer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1046 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2339 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1340 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/supermodel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2662 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.117282 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3249 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11423 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2524 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    21311 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/file.pdf
+-rw-r--r--   0 maurits    (501) staff       (20)      376 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/helpers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      434 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_basic_behavior.py
+-rw-r--r--   0 maurits    (501) staff       (20)      792 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_behaviors.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1610 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_directives.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3656 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3767 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1793 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1170 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.121271 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2416 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      249 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to1.py
+-rw-r--r--   0 maurits    (501) staff       (20)      195 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2.py
+-rw-r--r--   0 maurits    (501) staff       (20)      221 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2000.py
+-rw-r--r--   0 maurits    (501) staff       (20)      631 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2001.py
+-rw-r--r--   0 maurits    (501) staff       (20)      268 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2002.py
+-rw-r--r--   0 maurits    (501) staff       (20)      606 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2003.py
+-rw-r--r--   0 maurits    (501) staff       (20)      976 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2004.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1444 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2005.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-08 19:40:13.076510 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    44513 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     6632 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      829 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1889 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      287 2023-05-08 19:40:13.122584 plone.app.dexterity-3.1.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     3209 2023-05-08 19:40:12.000000 plone.app.dexterity-3.1.0/setup.py
```

### Comparing `plone.app.dexterity-3.0.5/CHANGES.rst` & `plone.app.dexterity-3.1.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.0 (2023-05-08)
+------------------
+
+New features:
+
+
+- Content types control panel: Show behavior name and interface. @ksuess, @stevepiercy (#363)
+
+
 3.0.5 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix for searchable Named(Blob)File indexer. Safely convert to str.
```

### Comparing `plone.app.dexterity-3.0.5/PKG-INFO` & `plone.app.dexterity-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.0.5
+Version: 3.1.0
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -327,14 +327,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.0 (2023-05-08)
+------------------
+
+New features:
+
+
+- Content types control panel: Show behavior name and interface. @ksuess, @stevepiercy (#363)
+
+
 3.0.5 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix for searchable Named(Blob)File indexer. Safely convert to str.
```

### Comparing `plone.app.dexterity-3.0.5/README.rst` & `plone.app.dexterity-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/RELEASE_NOTES.rst` & `plone.app.dexterity-3.1.0/RELEASE_NOTES.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/LICENSE.GPL` & `plone.app.dexterity-3.1.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/LICENSE.txt` & `plone.app.dexterity-3.1.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/Makefile` & `plone.app.dexterity-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/behaviours.rst` & `plone.app.dexterity-3.1.0/docs/advanced/behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/catalog-indexing-strategies.rst` & `plone.app.dexterity-3.1.0/docs/advanced/catalog-indexing-strategies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/custom-add-and-edit-forms.rst` & `plone.app.dexterity-3.1.0/docs/advanced/custom-add-and-edit-forms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/custom-content-classes.rst` & `plone.app.dexterity-3.1.0/docs/advanced/custom-content-classes.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/defaults.rst` & `plone.app.dexterity-3.1.0/docs/advanced/defaults.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/event-handlers.rst` & `plone.app.dexterity-3.1.0/docs/advanced/event-handlers.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/files-and-images.rst` & `plone.app.dexterity-3.1.0/docs/advanced/files-and-images.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/permissions.rst` & `plone.app.dexterity-3.1.0/docs/advanced/permissions.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/references.rst` & `plone.app.dexterity-3.1.0/docs/advanced/references.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/rich-text-markup-transformations.rst` & `plone.app.dexterity-3.1.0/docs/advanced/rich-text-markup-transformations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/static-resources.rst` & `plone.app.dexterity-3.1.0/docs/advanced/static-resources.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/validators.rst` & `plone.app.dexterity-3.1.0/docs/advanced/validators.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/vocabularies.rst` & `plone.app.dexterity-3.1.0/docs/advanced/vocabularies.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/webdav-and-other-file-representations.rst` & `plone.app.dexterity-3.1.0/docs/advanced/webdav-and-other-file-representations.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/advanced/workflow.rst` & `plone.app.dexterity-3.1.0/docs/advanced/workflow.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/behaviors/behavior-basics.rst` & `plone.app.dexterity-3.1.0/docs/behaviors/behavior-basics.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/behaviors/creating-and-registering-behaviors.rst` & `plone.app.dexterity-3.1.0/docs/behaviors/creating-and-registering-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/behaviors/intro.rst` & `plone.app.dexterity-3.1.0/docs/behaviors/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/behaviors/providing-marker-interfaces.rst` & `plone.app.dexterity-3.1.0/docs/behaviors/providing-marker-interfaces.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/behaviors/schema-only-behaviors.rst` & `plone.app.dexterity-3.1.0/docs/behaviors/schema-only-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/behaviors/testing-behaviors.rst` & `plone.app.dexterity-3.1.0/docs/behaviors/testing-behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/conf.py` & `plone.app.dexterity-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/custom-views.rst` & `plone.app.dexterity-3.1.0/docs/custom-views.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/designing.rst` & `plone.app.dexterity-3.1.0/docs/designing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/install.rst` & `plone.app.dexterity-3.1.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/intro.rst` & `plone.app.dexterity-3.1.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/model-driven-types.rst` & `plone.app.dexterity-3.1.0/docs/model-driven-types.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/prerequisite.rst` & `plone.app.dexterity-3.1.0/docs/prerequisite.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/reference/dexterity-xml.rst` & `plone.app.dexterity-3.1.0/docs/reference/dexterity-xml.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/reference/fields.rst` & `plone.app.dexterity-3.1.0/docs/reference/fields.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/reference/form-schema-hints.rst` & `plone.app.dexterity-3.1.0/docs/reference/form-schema-hints.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/reference/manipulating-content-objects.rst` & `plone.app.dexterity-3.1.0/docs/reference/manipulating-content-objects.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/reference/misc.rst` & `plone.app.dexterity-3.1.0/docs/reference/misc.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/reference/standard-behaviours.rst` & `plone.app.dexterity-3.1.0/docs/reference/standard-behaviours.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/reference/widgets.rst` & `plone.app.dexterity-3.1.0/docs/reference/widgets.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/schema-driven-types.rst` & `plone.app.dexterity-3.1.0/docs/schema-driven-types.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/testing/integration-tests.rst` & `plone.app.dexterity-3.1.0/docs/testing/integration-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/testing/mock-testing.rst` & `plone.app.dexterity-3.1.0/docs/testing/mock-testing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/docs/testing/unit-tests.rst` & `plone.app.dexterity-3.1.0/docs/testing/unit-tests.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/TODO.txt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/configure.zcml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/constrains.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/discussion.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/discussion.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/exclfromnav.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/exclfromnav.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/filename.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/filename.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/id.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/id.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/metadata.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/nextprevious.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/nextprevious.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_contrains.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_contrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_id.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_id.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/behaviors/tests/test_metadata.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/behaviors/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/add_type.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/add_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/behaviors.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.pt`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,181 @@
 00000000: 3c74 616c 3a72 6f6f 743e 0a20 203c 6469  <tal:root>.  <di
 00000010: 7620 636c 6173 733d 2270 6f72 7461 6c4d  v class="portalM
 00000020: 6573 7361 6765 220a 2020 2020 2020 2074  essage".       t
 00000030: 616c 3a63 6f6e 6469 7469 6f6e 3d22 7669  al:condition="vi
 00000040: 6577 2f73 7461 7475 7322 0a20 2020 2020  ew/status".     
 00000050: 2020 7461 6c3a 636f 6e74 656e 743d 2276    tal:content="v
 00000060: 6965 772f 7374 6174 7573 220a 2020 3e3c  iew/status".  ><
-00000070: 2f64 6976 3e0a 0a20 203c 666f 726d 2061  /div>..  <form a
-00000080: 6374 696f 6e3d 222e 220a 2020 2020 2020  ction=".".      
-00000090: 2020 6d65 7468 6f64 3d22 706f 7374 220a    method="post".
-000000a0: 2020 2020 2020 2020 7461 6c3a 6174 7472          tal:attr
-000000b0: 6962 7574 6573 3d22 0a20 2020 2020 2020  ibutes=".       
-000000c0: 2020 2061 6374 696f 6e20 7265 7175 6573     action reques
-000000d0: 742f 6765 7455 524c 3b0a 2020 2020 2020  t/getURL;.      
-000000e0: 2020 2020 656e 6374 7970 6520 7669 6577      enctype view
-000000f0: 2f65 6e63 7479 7065 3b0a 2020 2020 2020  /enctype;.      
-00000100: 2020 220a 2020 3e0a 2020 2020 3c74 616c    ".  >.    <tal
-00000110: 3a77 6964 6765 7473 2072 6570 6561 743d  :widgets repeat=
-00000120: 2277 6964 6765 7420 7669 6577 2f77 6964  "widget view/wid
-00000130: 6765 7473 2f76 616c 7565 737c 6e6f 7468  gets/values|noth
-00000140: 696e 6722 3e0a 0a20 2020 2020 203c 6469  ing">..      <di
-00000150: 7620 636c 6173 733d 2266 6965 6c64 220a  v class="field".
-00000160: 2020 2020 2020 2020 2020 2074 616c 3a64             tal:d
-00000170: 6566 696e 653d 220a 2020 2020 2020 2020  efine=".        
-00000180: 2020 2020 2065 7272 6f72 2077 6964 6765       error widge
-00000190: 742f 6572 726f 723b 0a20 2020 2020 2020  t/error;.       
-000001a0: 2020 2020 2020 6869 6464 656e 2070 7974        hidden pyt
-000001b0: 686f 6e3a 7769 6467 6574 2e6d 6f64 6520  hon:widget.mode 
-000001c0: 3d3d 2027 6869 6464 656e 273b 0a20 2020  == 'hidden';.   
-000001d0: 2020 2020 2020 2020 220a 2020 2020 2020          ".      
-000001e0: 2020 2020 2074 616c 3a61 7474 7269 6275       tal:attribu
-000001f0: 7465 733d 220a 2020 2020 2020 2020 2020  tes=".          
-00000200: 2020 2063 6c61 7373 2070 7974 686f 6e3a     class python:
-00000210: 276d 622d 3320 6669 656c 6427 202b 2028  'mb-3 field' + (
-00000220: 6572 726f 7220 616e 6420 2761 6c65 7274  error and 'alert
-00000230: 2061 6c65 7274 2d77 6172 6e69 6e67 2720   alert-warning' 
-00000240: 6f72 2027 2729 3b0a 2020 2020 2020 2020  or '');.        
-00000250: 2020 2022 0a20 2020 2020 203e 0a0a 2020     ".      >..  
-00000260: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00000270: 733d 2266 6965 6c64 5265 7175 6972 6564  s="fieldRequired
-00000280: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000290: 7469 746c 653d 2252 6571 7569 7265 6422  title="Required"
-000002a0: 0a20 2020 2020 2020 2020 2020 2020 2074  .              t
-000002b0: 616c 3a63 6f6e 6469 7469 6f6e 3d22 7079  al:condition="py
-000002c0: 7468 6f6e 3a77 6964 6765 742e 7265 7175  thon:widget.requ
-000002d0: 6972 6564 2061 6e64 206e 6f74 2068 6964  ired and not hid
-000002e0: 6465 6e22 0a20 2020 2020 2020 2020 2020  den".           
-000002f0: 2020 2069 3138 6e3a 6174 7472 6962 7574     i18n:attribut
-00000300: 6573 3d22 7469 746c 6520 7469 746c 655f  es="title title_
-00000310: 7265 7175 6972 6564 3b22 0a20 2020 2020  required;".     
-00000320: 2020 2020 2020 2020 2069 3138 6e3a 7472           i18n:tr
-00000330: 616e 736c 6174 653d 226c 6162 656c 5f72  anslate="label_r
-00000340: 6571 7569 7265 6422 0a20 2020 2020 2020  equired".       
-00000350: 203e 0a20 2020 2020 2028 5265 7175 6972   >.      (Requir
-00000360: 6564 290a 2020 2020 2020 2020 3c2f 7370  ed).        </sp
-00000370: 616e 3e0a 0a20 2020 2020 2020 203c 6469  an>..        <di
-00000380: 7620 7461 6c3a 636f 6e64 6974 696f 6e3d  v tal:condition=
-00000390: 2265 7272 6f72 220a 2020 2020 2020 2020  "error".        
-000003a0: 2020 2020 2074 616c 3a63 6f6e 7465 6e74       tal:content
-000003b0: 3d22 7374 7275 6374 7572 6520 6572 726f  ="structure erro
-000003c0: 722f 7265 6e64 6572 220a 2020 2020 2020  r/render".      
-000003d0: 2020 3e0a 2020 2020 2020 4572 726f 720a    >.      Error.
-000003e0: 2020 2020 2020 2020 3c2f 6469 763e 0a0a          </div>..
-000003f0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00000400: 7373 3d22 7769 6467 6574 223e 0a20 2020  ss="widget">.   
-00000410: 2020 2020 2020 203c 696e 7075 7420 7479         <input ty
-00000420: 7065 3d22 7465 7874 220a 2020 2020 2020  pe="text".      
-00000430: 2020 2020 2020 2020 2020 2074 616c 3a72             tal:r
-00000440: 6570 6c61 6365 3d22 7374 7275 6374 7572  eplace="structur
-00000450: 6520 7769 6467 6574 2f72 656e 6465 7222  e widget/render"
-00000460: 0a20 2020 2020 2020 2020 202f 3e0a 2020  .          />.  
-00000470: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00000480: 7373 3d22 666f 726d 2d74 6578 7422 0a20  ss="form-text". 
-00000490: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-000004a0: 6c3a 6465 6669 6e65 3d22 0a20 2020 2020  l:define=".     
-000004b0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-000004c0: 7269 7074 696f 6e20 7769 6467 6574 2f66  ription widget/f
-000004d0: 6965 6c64 2f64 6573 6372 6970 7469 6f6e  ield/description
-000004e0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-000004f0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00000500: 2020 7461 6c3a 636f 6e64 6974 696f 6e3d    tal:condition=
-00000510: 2270 7974 686f 6e3a 6465 7363 7269 7074  "python:descript
-00000520: 696f 6e20 616e 6420 6e6f 7420 6869 6464  ion and not hidd
-00000530: 656e 220a 2020 2020 2020 2020 2020 2020  en".            
-00000540: 2020 2074 616c 3a63 6f6e 7465 6e74 3d22     tal:content="
-00000550: 6465 7363 7269 7074 696f 6e22 0a20 2020  description".   
-00000560: 2020 2020 2020 2020 2020 2020 6931 386e              i18n
-00000570: 3a74 7261 6e73 6c61 7465 3d22 220a 2020  :translate="".  
-00000580: 2020 2020 2020 2020 3e66 6965 6c64 2064          >field d
-00000590: 6573 6372 6970 7469 6f6e 0a20 2020 2020  escription.     
-000005a0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-000005b0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000005c0: 203c 2f64 6976 3e0a 0a20 2020 203c 2f74   </div>..    </t
-000005d0: 616c 3a77 6964 6765 7473 3e0a 2020 2020  al:widgets>.    
-000005e0: 3c6d 6574 616c 3a61 6374 696f 6e73 206d  <metal:actions m
-000005f0: 6574 616c 3a75 7365 2d6d 6163 726f 3d22  etal:use-macro="
-00000600: 636f 6e74 6578 742f 4040 706c 6f6e 6566  context/@@plonef
-00000610: 6f72 6d2d 6d61 6372 6f73 2f61 6374 696f  orm-macros/actio
-00000620: 6e73 2220 2f3e 0a20 203c 2f66 6f72 6d3e  ns" />.  </form>
-00000630: 0a3c 2f74 616c 3a72 6f6f 743e 0a         .</tal:root>.
+00000070: 2f64 6976 3e0a 0a20 203c 7461 626c 6520  /div>..  <table 
+00000080: 636c 6173 733d 2274 6162 6c65 223e 0a20  class="table">. 
+00000090: 2020 203c 7468 6561 643e 0a20 2020 2020     <thead>.     
+000000a0: 203c 7472 3e0a 2020 2020 2020 2020 3c74   <tr>.        <t
+000000b0: 6820 636c 6173 733d 2277 2d32 3522 3e0a  h class="w-25">.
+000000c0: 2020 2020 2020 2020 3c2f 7468 3e0a 2020          </th>.  
+000000d0: 2020 2020 2020 3c74 6820 636c 6173 733d        <th class=
+000000e0: 2277 2d32 3522 3e0a 2020 2020 2020 2020  "w-25">.        
+000000f0: 2020 3c73 7061 6e20 6931 386e 3a74 7261    <span i18n:tra
+00000100: 6e73 6c61 7465 3d22 6c61 6265 6c5f 6e61  nslate="label_na
+00000110: 6d65 5f6f 665f 6265 6861 7669 6f72 223e  me_of_behavior">
+00000120: 4e61 6d65 206f 6620 6265 6861 7669 6f72  Name of behavior
+00000130: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+00000140: 3c2f 7468 3e0a 2020 2020 2020 2020 3c74  </th>.        <t
+00000150: 683e 0a20 2020 2020 2020 2020 203c 7370  h>.          <sp
+00000160: 616e 2069 3138 6e3a 7472 616e 736c 6174  an i18n:translat
+00000170: 653d 226c 6162 656c 5f69 6e74 6572 6661  e="label_interfa
+00000180: 6365 5f6f 665f 6265 6861 7669 6f72 223e  ce_of_behavior">
+00000190: 496e 7465 7266 6163 6520 6f66 2062 6568  Interface of beh
+000001a0: 6176 696f 723c 2f73 7061 6e3e 0a20 2020  avior</span>.   
+000001b0: 2020 2020 203c 2f74 683e 0a20 2020 2020       </th>.     
+000001c0: 203c 2f74 723e 0a20 2020 203c 2f74 6865   </tr>.    </the
+000001d0: 6164 3e0a 2020 3c2f 7461 626c 653e 0a0a  ad>.  </table>..
+000001e0: 2020 3c66 6f72 6d20 6163 7469 6f6e 3d22    <form action="
+000001f0: 2e22 0a20 2020 2020 2020 206d 6574 686f  .".        metho
+00000200: 643d 2270 6f73 7422 0a20 2020 2020 2020  d="post".       
+00000210: 2074 616c 3a61 7474 7269 6275 7465 733d   tal:attributes=
+00000220: 220a 2020 2020 2020 2020 2020 6163 7469  ".          acti
+00000230: 6f6e 2072 6571 7565 7374 2f67 6574 5552  on request/getUR
+00000240: 4c3b 0a20 2020 2020 2020 2020 2065 6e63  L;.          enc
+00000250: 7479 7065 2076 6965 772f 656e 6374 7970  type view/enctyp
+00000260: 653b 0a20 2020 2020 2020 2022 0a20 203e  e;.        ".  >
+00000270: 0a20 2020 203c 7461 6c3a 7769 6467 6574  .    <tal:widget
+00000280: 7320 7265 7065 6174 3d22 7769 6467 6574  s repeat="widget
+00000290: 2076 6965 772f 7769 6467 6574 732f 7661   view/widgets/va
+000002a0: 6c75 6573 7c6e 6f74 6869 6e67 223e 0a20  lues|nothing">. 
+000002b0: 2020 2020 203c 7461 6c3a 6465 6669 6e65       <tal:define
+000002c0: 2074 616c 3a64 6566 696e 653d 220a 2020   tal:define=".  
+000002d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002e0: 2020 6265 6861 7669 6f72 5f6e 616d 6520    behavior_name 
+000002f0: 7079 7468 6f6e 3a20 7769 6467 6574 2e66  python: widget.f
+00000300: 6965 6c64 2e5f 5f6e 616d 655f 5f3b 0a20  ield.__name__;. 
+00000310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000320: 2020 2062 6568 6176 696f 725f 7265 6720     behavior_reg 
+00000330: 7079 7468 6f6e 3a20 7669 6577 2e62 6568  python: view.beh
+00000340: 6176 696f 7273 5b62 6568 6176 696f 725f  aviors[behavior_
+00000350: 6e61 6d65 5d3b 0a20 2020 2020 2020 2020  name];.         
+00000360: 2020 2020 2020 2020 2022 3e0a 2020 2020           ">.    
+00000370: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000380: 6669 656c 6422 0a20 2020 2020 2020 2020  field".         
+00000390: 2020 2020 7461 6c3a 6465 6669 6e65 3d22      tal:define="
+000003a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003b0: 6572 726f 7220 7769 6467 6574 2f65 7272  error widget/err
+000003c0: 6f72 3b0a 2020 2020 2020 2020 2020 2020  or;.            
+000003d0: 2020 2068 6964 6465 6e20 7079 7468 6f6e     hidden python
+000003e0: 3a77 6964 6765 742e 6d6f 6465 203d 3d20  :widget.mode == 
+000003f0: 2768 6964 6465 6e27 3b0a 2020 2020 2020  'hidden';.      
+00000400: 2020 2020 2020 2022 0a20 2020 2020 2020         ".       
+00000410: 2020 2020 2020 7461 6c3a 6174 7472 6962        tal:attrib
+00000420: 7574 6573 3d22 0a20 2020 2020 2020 2020  utes=".         
+00000430: 2020 2020 2020 636c 6173 7320 7079 7468        class pyth
+00000440: 6f6e 3a27 6d62 2d33 2066 6965 6c64 2720  on:'mb-3 field' 
+00000450: 2b20 2865 7272 6f72 2061 6e64 2027 616c  + (error and 'al
+00000460: 6572 7420 616c 6572 742d 7761 726e 696e  ert alert-warnin
+00000470: 6727 206f 7220 2727 293b 0a20 2020 2020  g' or '');.     
+00000480: 2020 2020 2020 2020 220a 2020 2020 2020          ".      
+00000490: 2020 3e0a 0a20 2020 2020 2020 2020 203c    >..          <
+000004a0: 7370 616e 2063 6c61 7373 3d22 6669 656c  span class="fiel
+000004b0: 6452 6571 7569 7265 6422 0a20 2020 2020  dRequired".     
+000004c0: 2020 2020 2020 2020 2020 2074 6974 6c65             title
+000004d0: 3d22 5265 7175 6972 6564 220a 2020 2020  ="Required".    
+000004e0: 2020 2020 2020 2020 2020 2020 7461 6c3a              tal:
+000004f0: 636f 6e64 6974 696f 6e3d 2270 7974 686f  condition="pytho
+00000500: 6e3a 7769 6467 6574 2e72 6571 7569 7265  n:widget.require
+00000510: 6420 616e 6420 6e6f 7420 6869 6464 656e  d and not hidden
+00000520: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000530: 2020 6931 386e 3a61 7474 7269 6275 7465    i18n:attribute
+00000540: 733d 2274 6974 6c65 2074 6974 6c65 5f72  s="title title_r
+00000550: 6571 7569 7265 643b 220a 2020 2020 2020  equired;".      
+00000560: 2020 2020 2020 2020 2020 6931 386e 3a74            i18n:t
+00000570: 7261 6e73 6c61 7465 3d22 6c61 6265 6c5f  ranslate="label_
+00000580: 7265 7175 6972 6564 220a 2020 2020 2020  required".      
+00000590: 2020 2020 3e0a 2020 2020 2020 2020 2852      >.        (R
+000005a0: 6571 7569 7265 6429 0a20 2020 2020 2020  equired).       
+000005b0: 2020 203c 2f73 7061 6e3e 0a0a 2020 2020     </span>..    
+000005c0: 2020 2020 2020 3c64 6976 2074 616c 3a63        <div tal:c
+000005d0: 6f6e 6469 7469 6f6e 3d22 6572 726f 7222  ondition="error"
+000005e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000005f0: 7461 6c3a 636f 6e74 656e 743d 2273 7472  tal:content="str
+00000600: 7563 7475 7265 2065 7272 6f72 2f72 656e  ucture error/ren
+00000610: 6465 7222 0a20 2020 2020 2020 2020 203e  der".          >
+00000620: 0a20 2020 2020 2020 2045 7272 6f72 0a20  .        Error. 
+00000630: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
+00000640: 0a20 2020 2020 2020 2020 203c 6469 7620  .          <div 
+00000650: 636c 6173 733d 2277 6964 6765 7422 3e0a  class="widget">.
+00000660: 2020 2020 2020 2020 2020 2020 3c74 6162              <tab
+00000670: 6c65 2063 6c61 7373 3d22 7461 626c 6520  le class="table 
+00000680: 7461 626c 652d 626f 7264 6572 6c65 7373  table-borderless
+00000690: 2074 6162 6c65 2d73 6d22 3e0a 2020 2020   table-sm">.    
+000006a0: 2020 2020 2020 2020 2020 3c74 626f 6479            <tbody
+000006b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000006c0: 2020 3c74 723e 0a20 2020 2020 2020 2020    <tr>.         
+000006d0: 2020 2020 2020 2020 203c 7464 2063 6c61           <td cla
+000006e0: 7373 3d22 772d 3235 223e 0a20 2020 2020  ss="w-25">.     
+000006f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000700: 696e 7075 7420 7479 7065 3d22 7465 7874  input type="text
+00000710: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000720: 2020 2020 2020 2020 2020 2020 2074 616c               tal
+00000730: 3a72 6570 6c61 6365 3d22 7374 7275 6374  :replace="struct
+00000740: 7572 6520 7769 6467 6574 2f72 656e 6465  ure widget/rende
+00000750: 7222 0a20 2020 2020 2020 2020 2020 2020  r".             
+00000760: 2020 2020 2020 202f 3e0a 2020 2020 2020         />.      
+00000770: 2020 2020 2020 2020 2020 2020 3c2f 7464              </td
+00000780: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000790: 2020 2020 3c74 6420 636c 6173 733d 2277      <td class="w
+000007a0: 2d32 3522 0a20 2020 2020 2020 2020 2020  -25".           
+000007b0: 2020 2020 2020 2020 2020 2074 616c 3a63             tal:c
+000007c0: 6f6e 7465 6e74 3d22 6265 6861 7669 6f72  ontent="behavior
+000007d0: 5f6e 616d 6522 0a20 2020 2020 2020 2020  _name".         
+000007e0: 2020 2020 2020 2020 203e 6e61 6d65 206f           >name o
+000007f0: 6620 6265 6861 7669 6f72 3c2f 7464 3e0a  f behavior</td>.
+00000800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000810: 2020 3c74 6420 7461 6c3a 636f 6e74 656e    <td tal:conten
+00000820: 743d 2270 7974 686f 6e3a 6265 6861 7669  t="python:behavi
+00000830: 6f72 5f72 6567 2e69 6e74 6572 6661 6365  or_reg.interface
+00000840: 2e5f 5f69 6465 6e74 6966 6965 725f 5f22  .__identifier__"
+00000850: 3e69 6e74 6572 6661 6365 206f 6620 6265  >interface of be
+00000860: 6861 7669 6f72 3c2f 7464 3e0a 2020 2020  havior</td>.    
+00000870: 2020 2020 2020 2020 2020 2020 3c2f 7472              </tr
+00000880: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000890: 2020 3c74 7220 7461 6c3a 6465 6669 6e65    <tr tal:define
+000008a0: 3d22 0a20 2020 2020 2020 2020 2020 2020  =".             
+000008b0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+000008c0: 7469 6f6e 2077 6964 6765 742f 6669 656c  tion widget/fiel
+000008d0: 642f 6465 7363 7269 7074 696f 6e3b 0a20  d/description;. 
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 2020 2022 0a20 2020 2020 2020 2020 2020     ".           
+00000900: 2020 2020 2020 2020 2074 616c 3a63 6f6e           tal:con
+00000910: 6469 7469 6f6e 3d22 7079 7468 6f6e 3a64  dition="python:d
+00000920: 6573 6372 6970 7469 6f6e 2061 6e64 206e  escription and n
+00000930: 6f74 2068 6964 6465 6e22 0a20 2020 2020  ot hidden".     
+00000940: 2020 2020 2020 2020 2020 203e 0a20 2020             >.   
+00000950: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000960: 7464 2063 6f6c 7370 616e 3d22 3322 3e0a  td colspan="3">.
+00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000980: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+00000990: 2266 6f72 6d2d 7465 7874 220a 2020 2020  "form-text".    
+000009a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009b0: 2020 2020 2020 7461 6c3a 636f 6e74 656e        tal:conten
+000009c0: 743d 2264 6573 6372 6970 7469 6f6e 220a  t="description".
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009e0: 2020 2020 2020 2020 2020 6931 386e 3a74            i18n:t
+000009f0: 7261 6e73 6c61 7465 3d22 220a 2020 2020  ranslate="".    
+00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a10: 3e66 6965 6c64 2064 6573 6372 6970 7469  >field descripti
+00000a20: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
+00000a30: 2020 2020 2020 203c 2f73 7061 6e3e 0a20         </span>. 
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 203c 2f74 643e 0a20 2020 2020 2020 2020   </td>.         
+00000a60: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
+00000a70: 2020 2020 2020 2020 2020 203c 2f74 626f             </tbo
+00000a80: 6479 3e0a 2020 2020 2020 2020 2020 2020  dy>.            
+00000a90: 3c2f 7461 626c 653e 0a20 2020 2020 2020  </table>.       
+00000aa0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000ab0: 2020 3c2f 6469 763e 0a0a 2020 2020 2020    </div>..      
+00000ac0: 3c2f 7461 6c3a 6465 6669 6e65 3e0a 0a0a  </tal:define>...
+00000ad0: 2020 2020 3c2f 7461 6c3a 7769 6467 6574      </tal:widget
+00000ae0: 733e 0a20 2020 203c 6d65 7461 6c3a 6163  s>.    <metal:ac
+00000af0: 7469 6f6e 7320 6d65 7461 6c3a 7573 652d  tions metal:use-
+00000b00: 6d61 6372 6f3d 2263 6f6e 7465 7874 2f40  macro="context/@
+00000b10: 4070 6c6f 6e65 666f 726d 2d6d 6163 726f  @ploneform-macro
+00000b20: 732f 6163 7469 6f6e 7322 202f 3e0a 2020  s/actions" />.  
+00000b30: 3c2f 666f 726d 3e0a 3c2f 7461 6c3a 726f  </form>.</tal:ro
+00000b40: 6f74 3e0a                                ot>.
```

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/behaviors.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/behaviors.py`

 * *Files 7% similar despite different names*

```diff
@@ -89,14 +89,30 @@
     buttons = deepcopy(form.EditForm.buttons)
     buttons["apply"].title = _("Save")
 
     def getContent(self):
         return BehaviorConfigurationAdapter(self.context)
 
     @property
+    def behaviors(self):
+        """Return dict of (behavior name, reg)"""
+        counts = Counter([id(reg) for name, reg in getUtilitiesFor(IBehavior)])
+        behavs = {}
+        for name, reg in getUtilitiesFor(IBehavior):
+            if name in TTW_BEHAVIOR_BLACKLIST:
+                # skip blacklisted
+                continue
+            with_name = counts[id(reg)] > 1
+            if with_name and reg.name != name:
+                continue
+            fname = safe_text(reg.name if reg.name else name)
+            behavs[fname] = reg
+        return behavs
+
+    @property
     def fields(self):
         counts = Counter([id(reg) for name, reg in getUtilitiesFor(IBehavior)])
         fields = []
         for name, reg in getUtilitiesFor(IBehavior):
             if name in TTW_BEHAVIOR_BLACKLIST:
                 # skip blacklisted
                 continue
```

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/clone_type.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/clone_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/configure.zcml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/container.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/container.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/default_page_warning.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/default_page_warning.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/export.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/export.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/fields.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/fields.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/folder_listing.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/folder_listing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/import_types.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/import_types.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/item.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/item.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/modeleditor.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/modeleditor.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/modeleditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/overview.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/overview.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/tabbed_forms.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/tabbed_forms.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/types_listing_row.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/types_listing_row.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/browser/typesformwrapper.pt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/browser/typesformwrapper.pt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/configure.zcml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/events.zcml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/events.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/factories.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/factories.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/interfaces.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/permissions.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/default/controlpanel.xml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Document.xml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Document.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/profiles/testing/types/Folder.xml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/profiles/testing/types/Folder.xml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/serialize.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/serialize.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/testing.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/discussion.txt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/discussion.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/editing.rst` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/editing.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/filename.txt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/filename.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/import/dexterity_export.zip` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/import/dexterity_export.zip`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/metadata.txt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/metadata.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/namefromtitle.txt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/namefromtitle.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/nextprevious.txt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/nextprevious.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/robot/test_types.robot` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/robot/test_types.robot`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/schema_events.txt` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/schema_events.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_constrains.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_constrains.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_doctests.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_export.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_import.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_nextprevious.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_nextprevious.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_permissions.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_robot.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/tests/test_upgrades.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/tests/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/__init__.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/configure.zcml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/converters.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/converters.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/directives.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/indexer.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/indexer.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/interfaces.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/schemaeditor.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/supermodel.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/supermodel.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/testing.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/behaviors.rst` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/behaviors.rst`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/configure.zcml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/file.pdf` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/file.pdf`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_behaviors.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_directives.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_directives.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_schemaeditor.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_supermodel_handler.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/tests/test_utils.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/textindexer/utils.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/textindexer/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/configure.zcml` & `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2001.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2001.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2003.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2003.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2004.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2004.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone/app/dexterity/upgrades/to2005.py` & `plone.app.dexterity-3.1.0/plone/app/dexterity/upgrades/to2005.py`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/PKG-INFO` & `plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.dexterity
-Version: 3.0.5
+Version: 3.1.0
 Summary: Dexterity is a content type framework for CMF  applications, with particular emphasis on Plone. It can be viewed as an alternative to Archetypes that is more light-weight and modular.
 Home-page: http://plone.org/products/dexterity
 Author: Martin Aspeli, David Glick, et al
 Author-email: dexterity-development@googlegroups.com
 License: GPL
 Keywords: plone ttw dexterity schema interface
 Classifier: Development Status :: 5 - Production/Stable
@@ -327,14 +327,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.1.0 (2023-05-08)
+------------------
+
+New features:
+
+
+- Content types control panel: Show behavior name and interface. @ksuess, @stevepiercy (#363)
+
+
 3.0.5 (2023-04-14)
 ------------------
 
 Bug fixes:
 
 
 - Fix for searchable Named(Blob)File indexer. Safely convert to str.
```

### Comparing `plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/SOURCES.txt` & `plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/plone.app.dexterity.egg-info/requires.txt` & `plone.app.dexterity-3.1.0/plone.app.dexterity.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/pyproject.toml` & `plone.app.dexterity-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.dexterity-3.0.5/setup.py` & `plone.app.dexterity-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.5"
+version = "3.1.0"
 
 short_description = (
     "Dexterity is a content type framework for CMF  applications, "
     "with particular emphasis on Plone. It can be viewed as an "
     "alternative to Archetypes that is more light-weight and modular."
 )
```

