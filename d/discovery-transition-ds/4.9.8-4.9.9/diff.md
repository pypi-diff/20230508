# Comparing `tmp/discovery-transition-ds-4.9.8.tar.gz` & `tmp/discovery-transition-ds-4.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-transition-ds-4.9.8.tar", last modified: Thu Mar 16 18:08:26 2023, max compression
+gzip compressed data, was "discovery-transition-ds-4.9.9.tar", last modified: Sat Mar 18 20:16:12 2023, max compression
```

## Comparing `discovery-transition-ds-4.9.8.tar` & `discovery-transition-ds-4.9.9.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.502205 discovery-transition-ds-4.9.8/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11290 2023-03-16 18:08:26.502452 discovery-transition-ds-4.9.8/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10278 2023-02-16 18:41:13.000000 discovery-transition-ds-4.9.8/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.281191 discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11290 2023-03-16 18:08:26.000000 discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     4965 2023-03-16 18:08:26.000000 discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-03-16 18:08:26.000000 discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      104 2023-03-16 18:08:26.000000 discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-03-16 18:08:26.000000 discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.282135 discovery-transition-ds-4.9.8/ds_discovery/
--rwxr-xr-x   0 doatridge   (503) staff       (20)      686 2023-03-16 17:54:26.000000 discovery-transition-ds-4.9.8/ds_discovery/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.295096 discovery-transition-ds-4.9.8/ds_discovery/components/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21578 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7687 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8015 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/concept_tolerance.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31719 2023-01-22 23:47:02.000000 discovery-transition-ds-4.9.8/ds_discovery/components/controller.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)   102702 2023-03-15 17:28:56.000000 discovery-transition-ds-4.9.8/ds_discovery/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15776 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/event_book_portfolio.py
--rw-r--r--   0 doatridge   (503) staff       (20)    10972 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/feature_catalog.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7754 2023-01-24 23:41:56.000000 discovery-transition-ds-4.9.8/ds_discovery/components/models_builder.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6836 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/synthetic_builder.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    25236 2023-03-12 19:27:48.000000 discovery-transition-ds-4.9.8/ds_discovery/components/transitioning.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     8333 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/components/wrangling.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.295918 discovery-transition-ds-4.9.8/ds_discovery/engines/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/engines/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.297931 discovery-transition-ds-4.9.8/ds_discovery/engines/events/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/engines/events/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3649 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/engines/events/event_book_controller.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9730 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/engines/events/pandas_event_book.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.298520 discovery-transition-ds-4.9.8/ds_discovery/engines/executor/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/engines/executor/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.299677 discovery-transition-ds-4.9.8/ds_discovery/engines/executor/src/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/engines/executor/src/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1793 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/engines/executor/src/hadron_executor.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.303082 discovery-transition-ds-4.9.8/ds_discovery/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3430 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/handlers/event_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15567 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/handlers/pandas_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1018 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/handlers/pandas_pubsub.py
--rw-r--r--   0 doatridge   (503) staff       (20)    16172 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/handlers/s3_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.319676 discovery-transition-ds-4.9.8/ds_discovery/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    56618 2023-03-15 18:09:15.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8589 2023-02-20 19:28:08.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_frame_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    27492 2023-03-08 17:07:10.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_get_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9457 2023-02-20 20:47:03.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    52764 2023-03-16 18:06:21.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_model_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25435 2023-03-16 16:41:29.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    10715 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/concept_tolerance_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    35368 2023-01-25 16:23:33.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/controller_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9211 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/event_book_intent.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    53855 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/feature_catalog_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11206 2023-01-25 16:23:33.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/models_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    83641 2023-03-08 17:00:57.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/synthetic_intent.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    92824 2023-03-11 23:49:16.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/transition_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)   133386 2023-03-16 18:04:17.000000 discovery-transition-ds-4.9.8/ds_discovery/intent/wrangle_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.328198 discovery-transition-ds-4.9.8/ds_discovery/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)      660 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/concept_tolerance_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3372 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/controller_property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      477 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/event_book_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      689 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/feature_catalog_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      997 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/models_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      866 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/synthetic_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3960 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/transition_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      864 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/managers/wrangle_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.463497 discovery-transition-ds-4.9.8/ds_discovery/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25754 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/ds_discovery/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-03-16 18:08:26.503066 discovery-transition-ds-4.9.8/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2343 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.274096 discovery-transition-ds-4.9.8/tests/
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.477233 discovery-transition-ds-4.9.8/tests/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6683 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/abstract_common_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2715 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/commons_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6135 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/controller_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24304 2023-03-15 17:36:54.000000 discovery-transition-ds-4.9.8/tests/components/discovery_analyse_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     7167 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)      800 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/event_book_portfolio_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5084 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/event_book_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2905 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/feature_catalog_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1987 2023-01-25 16:27:42.000000 discovery-transition-ds-4.9.8/tests/components/models_builder_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2342 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/synthetic_builder_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    23954 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/transition_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1259 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/components/visual_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.478263 discovery-transition-ds-4.9.8/tests/engines/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/engines/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.480681 discovery-transition-ds-4.9.8/tests/engines/events/
--rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/engines/events/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2044 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/engines/events/event_book_controller_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.483078 discovery-transition-ds-4.9.8/tests/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3522 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/handlers/event_handler_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7548 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/handlers/pandas_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.498552 discovery-transition-ds-4.9.8/tests/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3853 2023-03-07 22:05:16.000000 discovery-transition-ds-4.9.8/tests/intent/abstract_common_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2590 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/controller_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2935 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/event_book_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7233 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/feature_calalog_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3315 2023-01-19 22:07:32.000000 discovery-transition-ds-4.9.8/tests/intent/model_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8371 2023-03-07 23:44:44.000000 discovery-transition-ds-4.9.8/tests/intent/synthetic_get_canonical_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5928 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_analysis_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13574 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_correlate_selection_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11060 2023-02-14 16:50:33.000000 discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_get_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    18720 2023-03-10 22:12:39.000000 discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_model_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4673 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/synthetic_pipeline_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3391 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/intent/transition_correlate_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    19441 2023-03-11 23:10:53.000000 discovery-transition-ds-4.9.8/tests/intent/transition_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20243 2023-03-11 00:01:41.000000 discovery-transition-ds-4.9.8/tests/intent/wrangle_intent_correlate_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8063 2023-03-16 18:07:01.000000 discovery-transition-ds-4.9.8/tests/intent/wrangle_intent_model_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4746 2023-02-26 20:52:48.000000 discovery-transition-ds-4.9.8/tests/intent/wrangle_intent_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.500156 discovery-transition-ds-4.9.8/tests/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2061 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/managers/transition_pm_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-16 18:08:26.501706 discovery-transition-ds-4.9.8/tests/scratch/
--rwxr-xr-x   0 doatridge   (503) staff       (20)       32 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/scratch/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)      862 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.8/tests/scratch/remote_run_demo.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.064399 discovery-transition-ds-4.9.9/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1507 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11290 2023-03-18 20:16:12.064635 discovery-transition-ds-4.9.9/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10278 2023-02-16 18:41:13.000000 discovery-transition-ds-4.9.9/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.851897 discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11290 2023-03-18 20:16:11.000000 discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     4965 2023-03-18 20:16:11.000000 discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-03-18 20:16:11.000000 discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      104 2023-03-18 20:16:11.000000 discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-03-18 20:16:11.000000 discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.852329 discovery-transition-ds-4.9.9/ds_discovery/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      686 2023-03-18 20:14:45.000000 discovery-transition-ds-4.9.9/ds_discovery/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.863141 discovery-transition-ds-4.9.9/ds_discovery/components/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21578 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7687 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8015 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/concept_tolerance.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31719 2023-01-22 23:47:02.000000 discovery-transition-ds-4.9.9/ds_discovery/components/controller.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)   102702 2023-03-15 17:28:56.000000 discovery-transition-ds-4.9.9/ds_discovery/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15776 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/event_book_portfolio.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    10972 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/feature_catalog.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7754 2023-01-24 23:41:56.000000 discovery-transition-ds-4.9.9/ds_discovery/components/models_builder.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6836 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/synthetic_builder.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    25236 2023-03-12 19:27:48.000000 discovery-transition-ds-4.9.9/ds_discovery/components/transitioning.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     8333 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/components/wrangling.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.863929 discovery-transition-ds-4.9.9/ds_discovery/engines/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/engines/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.865831 discovery-transition-ds-4.9.9/ds_discovery/engines/events/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/engines/events/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3649 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/engines/events/event_book_controller.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9730 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/engines/events/pandas_event_book.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.866388 discovery-transition-ds-4.9.9/ds_discovery/engines/executor/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/engines/executor/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.867603 discovery-transition-ds-4.9.9/ds_discovery/engines/executor/src/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/engines/executor/src/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1793 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/engines/executor/src/hadron_executor.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.870336 discovery-transition-ds-4.9.9/ds_discovery/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3430 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/handlers/event_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15567 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/handlers/pandas_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1018 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/handlers/pandas_pubsub.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    16172 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/handlers/s3_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.888056 discovery-transition-ds-4.9.9/ds_discovery/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    56618 2023-03-15 18:09:15.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8589 2023-02-20 19:28:08.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_frame_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    27492 2023-03-08 17:07:10.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_get_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9457 2023-02-20 20:47:03.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    54322 2023-03-18 20:01:16.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_model_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25435 2023-03-16 16:41:29.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    10715 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/concept_tolerance_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    35368 2023-01-25 16:23:33.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/controller_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9211 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/event_book_intent.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    53855 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/feature_catalog_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11206 2023-01-25 16:23:33.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/models_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    83641 2023-03-08 17:00:57.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/synthetic_intent.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    92824 2023-03-11 23:49:16.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/transition_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   133533 2023-03-17 23:07:12.000000 discovery-transition-ds-4.9.9/ds_discovery/intent/wrangle_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.896325 discovery-transition-ds-4.9.9/ds_discovery/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      660 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/concept_tolerance_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3372 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/controller_property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      477 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/event_book_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      689 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/feature_catalog_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      997 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/models_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      866 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/synthetic_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3960 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/transition_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      864 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/managers/wrangle_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.027525 discovery-transition-ds-4.9.9/ds_discovery/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25754 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/ds_discovery/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-03-18 20:16:12.065899 discovery-transition-ds-4.9.9/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2343 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:11.846700 discovery-transition-ds-4.9.9/tests/
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.037518 discovery-transition-ds-4.9.9/tests/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6683 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/abstract_common_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2715 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/commons_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6135 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/controller_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24304 2023-03-15 17:36:54.000000 discovery-transition-ds-4.9.9/tests/components/discovery_analyse_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     7167 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      800 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/event_book_portfolio_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5084 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/event_book_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2905 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/feature_catalog_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1987 2023-01-25 16:27:42.000000 discovery-transition-ds-4.9.9/tests/components/models_builder_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2342 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/synthetic_builder_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    23954 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/transition_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1259 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/components/visual_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.038038 discovery-transition-ds-4.9.9/tests/engines/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/engines/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.039489 discovery-transition-ds-4.9.9/tests/engines/events/
+-rw-r--r--   0 doatridge   (503) staff       (20)       31 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/engines/events/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2044 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/engines/events/event_book_controller_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.040869 discovery-transition-ds-4.9.9/tests/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3522 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/handlers/event_handler_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7548 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/handlers/pandas_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.061263 discovery-transition-ds-4.9.9/tests/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3853 2023-03-07 22:05:16.000000 discovery-transition-ds-4.9.9/tests/intent/abstract_common_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2590 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/controller_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2935 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/event_book_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7233 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/feature_calalog_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3315 2023-01-19 22:07:32.000000 discovery-transition-ds-4.9.9/tests/intent/model_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8371 2023-03-07 23:44:44.000000 discovery-transition-ds-4.9.9/tests/intent/synthetic_get_canonical_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5928 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_analysis_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13574 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_correlate_selection_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11060 2023-02-14 16:50:33.000000 discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_get_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    18720 2023-03-10 22:12:39.000000 discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_model_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4673 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/synthetic_pipeline_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3391 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/intent/transition_correlate_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    19441 2023-03-11 23:10:53.000000 discovery-transition-ds-4.9.9/tests/intent/transition_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20243 2023-03-11 00:01:41.000000 discovery-transition-ds-4.9.9/tests/intent/wrangle_intent_correlate_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    10704 2023-03-18 20:14:45.000000 discovery-transition-ds-4.9.9/tests/intent/wrangle_intent_model_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4746 2023-02-26 20:52:48.000000 discovery-transition-ds-4.9.9/tests/intent/wrangle_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.062364 discovery-transition-ds-4.9.9/tests/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2061 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/managers/transition_pm_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-03-18 20:16:12.063896 discovery-transition-ds-4.9.9/tests/scratch/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       32 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/scratch/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      862 2023-01-04 22:14:44.000000 discovery-transition-ds-4.9.9/tests/scratch/remote_run_demo.py
```

### Comparing `discovery-transition-ds-4.9.8/LICENSE.txt` & `discovery-transition-ds-4.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/PKG-INFO` & `discovery-transition-ds-4.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-transition-ds
-Version: 4.9.8
+Version: 4.9.9
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-transition-ds
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-transition-ds-4.9.8/README.rst` & `discovery-transition-ds-4.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/PKG-INFO` & `discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-transition-ds
-Version: 4.9.8
+Version: 4.9.9
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-transition-ds
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-transition-ds-4.9.8/discovery_transition_ds.egg-info/SOURCES.txt` & `discovery-transition-ds-4.9.9/discovery_transition_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/__init__.py` & `discovery-transition-ds-4.9.9/ds_discovery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 from ds_discovery.components.event_book_portfolio import EventBookPortfolio
 from ds_discovery.components.concept_tolerance import ConceptTolerance
 from ds_discovery.components.models_builder import ModelsBuilder
 from ds_discovery.components.controller import Controller
 from ds_discovery.components.commons import Commons
 
 # release version number picked up in the setup.py
-__version__ = '4.9.8'
+__version__ = '4.9.9'
```

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/abstract_common_component.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/commons.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/concept_tolerance.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/concept_tolerance.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/controller.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/controller.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/discovery.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/discovery.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/event_book_portfolio.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/event_book_portfolio.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/feature_catalog.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/feature_catalog.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/models_builder.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/models_builder.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/synthetic_builder.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/synthetic_builder.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/transitioning.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/transitioning.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/components/wrangling.py` & `discovery-transition-ds-4.9.9/ds_discovery/components/wrangling.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/engines/events/event_book_controller.py` & `discovery-transition-ds-4.9.9/ds_discovery/engines/events/event_book_controller.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/engines/events/pandas_event_book.py` & `discovery-transition-ds-4.9.9/ds_discovery/engines/events/pandas_event_book.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/engines/executor/src/hadron_executor.py` & `discovery-transition-ds-4.9.9/ds_discovery/engines/executor/src/hadron_executor.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/handlers/event_handlers.py` & `discovery-transition-ds-4.9.9/ds_discovery/handlers/event_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/handlers/pandas_handlers.py` & `discovery-transition-ds-4.9.9/ds_discovery/handlers/pandas_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/handlers/pandas_pubsub.py` & `discovery-transition-ds-4.9.9/ds_discovery/handlers/pandas_pubsub.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/handlers/s3_handlers.py` & `discovery-transition-ds-4.9.9/ds_discovery/handlers/s3_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_correlate_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_frame_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_frame_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_get_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_get_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_builder_model_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_builder_model_intent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import ast
+from difflib import ndiff
+
 import numpy as np
 import pandas as pd
 from abc import abstractmethod
 from typing import Any
 import pandas.api.types as ptypes
 from aistac.components.aistac_commons import DataAnalytics
 from ds_discovery.components.commons import Commons
@@ -213,21 +215,23 @@
         df_rtn = canonical.merge(right=other, how=how, left_on=left_on, right_on=right_on, on=on,
                           suffixes=suffixes, indicator=indicator, validate=validate)
         if replace_nulls:
             for column in df_rtn.columns.to_list():
                 Commons.fillna(df_rtn[column])
         return df_rtn
 
-    def _model_difference(self, canonical: Any, other: Any, on: str, reset_index: bool=None, seed: int=None):
+    def _model_difference(self, canonical: Any, other: Any, on_key: str, drop_no_diff: bool=None, index_on_key: bool=None,
+                          seed: int=None):
         """Compares two Datasets and returns the non-duplicate pairs
 
         :param canonical: a direct or generated pd.DataFrame. see context notes below
         :param other: a direct or generated pd.DataFrame. to concatenate
-        :param on: The header name of the key that joins the 2 files
-        :param reset_index: (optional) resets the index
+        :param on_key: The header name of the key that uniquely joins the canonical to others
+        :param drop_no_diff: (optional) drops columns with no difference
+        :param index_on_key: (optional) set the index to be the key
         :param seed: (optional) this is a placeholder, here for compatibility across methods
 
         The other is a pd.DataFrame, a pd.Series, int or list, a connector contract str reference or a set of
         parameter instructions on how to generate a pd.Dataframe. the description of each is:
 
         - pd.Dataframe -> a deep copy of the pd.DataFrame
         - pd.Series or list -> creates a pd.DataFrame of one column with the 'header' name or 'default' if not given
@@ -246,28 +250,62 @@
                     :seed (optional) if a seed should be applied
                     :run_book (optional) if specific intent should be run only
 
         """
         canonical = self._get_canonical(canonical)
         other = self._get_canonical(other, size=canonical.shape[0])
         _ = seed if isinstance(seed, int) else self._seed()
-        reset_index = reset_index if isinstance(reset_index, bool) else True
-        on = self._extract_value(on)
-        canonical.sort_values(on, inplace=True)
-        other.sort_values(on, inplace=True)
+        drop_no_diff = drop_no_diff if isinstance(drop_no_diff, bool) else False
+        index_on_key = index_on_key if isinstance(index_on_key, bool) else False
+        on_key = self._extract_value(on_key)
+        canonical.sort_values(on_key, inplace=True)
+        other.sort_values(on_key, inplace=True)
         # concat
         df = pd.concat([canonical, other])
         df = df.reset_index(drop=True)
         # group by
-        df_gpby = df.groupby(list(df.columns))
+        grouped = df.groupby(list(df.columns))
         # get index of unique records
-        idx = [x[0] for x in df_gpby.groups.values() if len(x) == 1]
-        if reset_index:
-            return df.reindex(idx).reset_index(drop=True)
-        return df.reindex(idx)
+        idx = [x[0] for x in grouped.groups.values() if len(x) == 1]
+        df = df.reindex(idx)
+        # ensure union of the ket
+
+        def levenshtein_distance(str1, str2, ):
+            counter = {"+": 0, "-": 0}
+            distance = 0
+            for edit_code, *_ in ndiff(str1, str2):
+                if edit_code == " ":
+                    distance += max(counter.values())
+                    counter = {"+": 0, "-": 0}
+                else:
+                    counter[edit_code] += 1
+            distance += max(counter.values())
+            return distance
+
+        # get the distance between differences
+        diff = pd.DataFrame()
+        for idx in range(0, df.shape[0], 2):
+            line = pd.Series(data=0, index=df.iloc[idx].index, dtype='int')
+            try:
+                for index, value in df.iloc[idx].items():
+                    if index == on_key:
+                        line.at[index] = value
+                    else:
+                        line.at[index] = levenshtein_distance(str(value), str(df.iloc[idx + 1].loc[index]))
+            except IndexError:
+                continue
+            diff = pd.concat([diff, line], axis=1)
+        diff = diff.T.reset_index(drop=True)
+        # set the index to the key
+        if index_on_key:
+            diff = diff.set_index(on_key)
+        # drop zeros
+        if drop_no_diff:
+            return diff.loc[:, (diff != 0).any(axis=0)]
+        return diff
 
     def _model_concat(self, canonical: Any, other: Any, as_rows: bool=None, headers: [str, list]=None,
                       drop: bool=None, dtype: [str, list]=None, exclude: bool=None, regex: [str, list]=None,
                       re_ignore_case: bool=None, shuffle: bool=None, seed: int=None) -> pd.DataFrame:
         """ returns the full column values directly from another connector data source.
 
         :param canonical: a pd.DataFrame as the reference dataframe
```

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/abstract_common_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/abstract_common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/concept_tolerance_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/concept_tolerance_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/controller_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/controller_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/event_book_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/event_book_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/feature_catalog_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/feature_catalog_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/models_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/models_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/synthetic_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/synthetic_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/transition_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/transition_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/intent/wrangle_intent.py` & `discovery-transition-ds-4.9.9/ds_discovery/intent/wrangle_intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,23 +406,24 @@
         # remove intent params
         params = locals()
         [params.pop(k) for k in self._INTENT_PARAMS]
         # set the seed and call the method
         seed = self._seed(seed=seed)
         return self._model_merge(seed=seed, **params)
 
-    def model_difference(self, canonical: Any, other: Any, on: str, reset_index: bool=None, seed: int=None, save_intent: bool=None,
-                     column_name: [int, str]=None, intent_order: int=None, replace_intent: bool=None,
-                     remove_duplicates: bool=None) -> pd.DataFrame:
+    def model_difference(self, canonical: Any, other: Any, on_key: str, drop_no_diff: bool=None, index_on_key: bool=None,
+                         seed: int=None, save_intent: bool=None,column_name: [int, str]=None, intent_order: int=None,
+                         replace_intent: bool=None, remove_duplicates: bool=None) -> pd.DataFrame:
         """ Compares two Datasets and returns the non-duplicate pairs
 
         :param canonical: a direct or generated pd.DataFrame. see context notes below
         :param other: a direct or generated pd.DataFrame. to concatenate
-        :param on: The header name of the key that joins the 2 files
-        :param reset_index: (optional) resets the index
+        :param on_key: The header name of the key that uniquely joins the canonical to others
+        :param drop_no_diff: (optional) drops columns with no difference
+        :param index_on_key: (optional) set the index to be the key
         :param seed: (optional) this is a placeholder, here for compatibility across methods
         :param save_intent: (optional) if the intent contract should be saved to the property manager
         :param column_name: (optional) the column name that groups intent to create a column
         :param intent_order: (optional) the order in which each intent should run.
                     - If None: default's to -1
                     - if -1: added to a level above any current instance of the intent section, level 0 if not found
                     - if int: added to the level specified, overwriting any that already exist
```

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/managers/concept_tolerance_property_manager.py` & `discovery-transition-ds-4.9.9/ds_discovery/managers/concept_tolerance_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/managers/controller_property_manager.py` & `discovery-transition-ds-4.9.9/ds_discovery/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/managers/feature_catalog_property_manager.py` & `discovery-transition-ds-4.9.9/ds_discovery/managers/feature_catalog_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/managers/models_property_manager.py` & `discovery-transition-ds-4.9.9/ds_discovery/managers/models_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/managers/synthetic_property_manager.py` & `discovery-transition-ds-4.9.9/ds_discovery/managers/synthetic_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/managers/transition_property_manager.py` & `discovery-transition-ds-4.9.9/ds_discovery/managers/transition_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/managers/wrangle_property_manager.py` & `discovery-transition-ds-4.9.9/ds_discovery/managers/wrangle_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_complaints.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_professions.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_uk_city.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_uk_postcode_district.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_us_city.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_us_street_names.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/lookup_us_street_suffix.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_companies_fortune1000.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_companies_inc5000.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_uk_postcodes_primary.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_age_salary.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_city_area_code.csv` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_city_zipcodes_rank.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_forename_mf.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_forename_unisex.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_full_address.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_healthcare_organisations.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_phone_code.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_profession_detail_rank.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/map_us_surname_rank.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/ds_discovery/sample/sample_data.py` & `discovery-transition-ds-4.9.9/ds_discovery/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/setup.py` & `discovery-transition-ds-4.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/abstract_common_component_test.py` & `discovery-transition-ds-4.9.9/tests/components/abstract_common_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/commons_test.py` & `discovery-transition-ds-4.9.9/tests/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/controller_test.py` & `discovery-transition-ds-4.9.9/tests/components/controller_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/discovery_analyse_test.py` & `discovery-transition-ds-4.9.9/tests/components/discovery_analyse_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/discovery_test.py` & `discovery-transition-ds-4.9.9/tests/components/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/event_book_portfolio_test.py` & `discovery-transition-ds-4.9.9/tests/components/event_book_portfolio_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/event_book_test.py` & `discovery-transition-ds-4.9.9/tests/components/event_book_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/feature_catalog_test.py` & `discovery-transition-ds-4.9.9/tests/components/feature_catalog_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/models_builder_test.py` & `discovery-transition-ds-4.9.9/tests/components/models_builder_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/synthetic_builder_test.py` & `discovery-transition-ds-4.9.9/tests/components/synthetic_builder_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/transition_test.py` & `discovery-transition-ds-4.9.9/tests/components/transition_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/components/visual_test.py` & `discovery-transition-ds-4.9.9/tests/components/visual_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/engines/events/event_book_controller_test.py` & `discovery-transition-ds-4.9.9/tests/engines/events/event_book_controller_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/handlers/event_handler_test.py` & `discovery-transition-ds-4.9.9/tests/handlers/event_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/handlers/pandas_handler_test.py` & `discovery-transition-ds-4.9.9/tests/handlers/pandas_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/abstract_common_intent_test.py` & `discovery-transition-ds-4.9.9/tests/intent/abstract_common_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/controller_intent_test.py` & `discovery-transition-ds-4.9.9/tests/intent/controller_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/event_book_intent_test.py` & `discovery-transition-ds-4.9.9/tests/intent/event_book_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/feature_calalog_intent_test.py` & `discovery-transition-ds-4.9.9/tests/intent/feature_calalog_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/model_intent_test.py` & `discovery-transition-ds-4.9.9/tests/intent/model_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/synthetic_get_canonical_test.py` & `discovery-transition-ds-4.9.9/tests/intent/synthetic_get_canonical_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_analysis_test.py` & `discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_analysis_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_correlate_selection_test.py` & `discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_correlate_selection_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_get_test.py` & `discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_get_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/synthetic_intent_model_test.py` & `discovery-transition-ds-4.9.9/tests/intent/synthetic_intent_model_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/synthetic_pipeline_test.py` & `discovery-transition-ds-4.9.9/tests/intent/synthetic_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/transition_correlate_test.py` & `discovery-transition-ds-4.9.9/tests/intent/transition_correlate_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/transition_intent_test.py` & `discovery-transition-ds-4.9.9/tests/intent/transition_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/wrangle_intent_correlate_test.py` & `discovery-transition-ds-4.9.9/tests/intent/wrangle_intent_correlate_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/intent/wrangle_intent_model_test.py` & `discovery-transition-ds-4.9.9/tests/intent/wrangle_intent_model_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -121,41 +121,87 @@
         df['B'] = tools.get_category(['a','b','c','d'], size=1000, relative_freq=[40,8,6,4], quantity=0.998, seed=99)
         result = tools.model_encode_count(df, headers=['B'])
         self.assertCountEqual([685, 137, 102, 74, 2], result['B'].value_counts().to_list())
 
     def test_model_difference_num(self):
         builder = SyntheticBuilder.from_memory()
         tools: SyntheticIntentModel = builder.tools
-        df = pd.DataFrame(data={"A": [1, 2, 3, 4, 5, 6, 7], "B": [1, 2, 3, 4, 3, 3, 1], 'C': [0, 2, 0, 4, 3, 2, 1]})
-        target = pd.DataFrame(data={"A": [1, 2, 3, 4, 5, 6, 7], "B": [1, 2, 5, 4, 3, 3, 1], 'C': [1, 2, 1, 4, 3, 2, 1]})
+        df = pd.DataFrame(data={"A":  list("ABCDEFG"), "B": [1, 2, 3, 4, 3, 3, 1], 'C': [0, 2, 0, 4, 3, 2, 1]})
+        target = pd.DataFrame(data={"A": list("ABCDEFG"), "B": [1, 2, 5, 4, 3, 3, 1], 'C': [1, 2, 3, 4, 3, 2, 1]})
         builder.add_connector_persist('target', uri_file='working/data/target.csv')
         builder.save_canonical('target', target)
-        result = tools.model_difference(df, 'target', on='A', reset_index=False)
-        self.assertEqual((4,3), result.shape)
-        self.assertEqual([0,7,2,9], result.index.tolist())
+        result = tools.model_difference(df, 'target', on_key='A')
+        self.assertEqual((2,3), result.shape)
+        self.assertEqual(['A', 'C'], result['A'].tolist())
+        self.assertEqual([0,1], result['B'].tolist())
+        self.assertEqual([1,1], result['C'].tolist())
+
 
     def test_model_difference_str(self):
         builder = SyntheticBuilder.from_memory()
         tools: SyntheticIntentModel = builder.tools
-        df = pd.DataFrame(data={"A": [1, 2, 3, 4, 5, 6, 7], "B": list("ABCFCBA"), 'C': list("BCDECFB")})
-        target = pd.DataFrame(data={"A": [1, 2, 3, 4, 5, 6, 7], "B": list("ABCDCBA"), 'C': list("BCDECFP")})
+        df = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("ABCFCBA"), 'C': list("BCDECFB")})
+        target = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("ABCDCBA"), 'C': list("BCDECFP")})
         builder.add_connector_persist('target', uri_file='working/data/target.csv')
         builder.save_canonical('target', target)
-        result = tools.model_difference(df, 'target', on='A', reset_index=False)
-        self.assertEqual([10,3,6,13], result.index.tolist())
+        result = tools.model_difference(df, 'target', on_key='A')
+        self.assertEqual((2,3), result.shape)
+        self.assertEqual(['D', 'G'], result['A'].tolist())
+        self.assertEqual([1, 0], result['B'].tolist())
+        self.assertEqual([0,1], result['C'].tolist())
 
     def test_model_difference_order(self):
         builder = SyntheticBuilder.from_memory()
         tools: SyntheticIntentModel = builder.tools
-        df = pd.DataFrame(data={"A": [1, 2, 3, 4, 5, 6, 7], "B": list("ABCFCBA"), 'C': list("BCDECFB")})
-        target = pd.DataFrame(data={"A": [6, 2, 3, 4, 5, 1, 7], "B": list("BBCDCAA"), 'C': list("FCDECBP")})
+        df = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("ABCFCBA"), 'C': list("BCDECFB"), 'D': [0, 2, 0, 4, 3, 2, 1]})
+        target = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("BBCDCAA"), 'C': list("BCDECFB"), 'D': [0, 2, 0, 4, 1, 2, 1]})
+        target.sample(frac = 1)
+        builder.add_connector_persist('target', uri_file='working/data/target.csv')
+        builder.save_canonical('target', target)
+        result = tools.model_difference(df, 'target', on_key='A', drop_no_diff=True)
+        self.assertEqual((4,3), result.shape)
+        self.assertEqual(['A', 'B', 'D'], result.columns.to_list())
+
+    def test_model_difference_drop(self):
+        builder = SyntheticBuilder.from_memory()
+        tools: SyntheticIntentModel = builder.tools
+        df = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("ABCFCBA"), 'C': list("BCDECFB"), 'D': [0, 2, 0, 4, 3, 2, 1]})
+        target = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("BBCDCAA"), 'C': list("BCDECFB"), 'D': [0, 2, 0, 4, 1, 2, 1]})
+        builder.add_connector_persist('target', uri_file='working/data/target.csv')
+        builder.save_canonical('target', target)
+        result = tools.model_difference(df, 'target', on_key='A', drop_no_diff=True)
+        self.assertEqual((4,3), result.shape)
+        self.assertEqual(['A', 'B', 'D'], result.columns.to_list())
+        self.assertEqual(df['C'].to_list(), target['C'].to_list())
+
+
+    def test_model_difference_index(self):
+        builder = SyntheticBuilder.from_memory()
+        tools: SyntheticIntentModel = builder.tools
+        df = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("ABCFCBA"), 'C': list("BCDECFB"), 'D': [0, 2, 0, 4, 3, 2, 1]})
+        target = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("BBCDCAA"), 'C': list("BCDECFB"), 'D': [0, 2, 0, 4, 1, 2, 1]})
         builder.add_connector_persist('target', uri_file='working/data/target.csv')
         builder.save_canonical('target', target)
-        result = tools.model_difference(df, 'target', on='A', reset_index=False)
-        self.assertEqual([10,3,6,13], result.index.tolist())
+        result = tools.model_difference(df, 'target', on_key='A', index_on_key=True)
+        self.assertEqual((4,3), result.shape)
+        self.assertEqual(['B', 'C', 'D'], result.columns.to_list())
+        self.assertEqual(['A', 'D', 'E', 'F'], result.index.tolist())
+
+    def test_model_difference_extra(self):
+        builder = SyntheticBuilder.from_memory()
+        tools: SyntheticIntentModel = builder.tools
+        # add an extra row to source
+        df = pd.DataFrame(data={"A": list("ABCDEFGH"), "B": list("ABCFCBAF"), 'C': list("BCDECFBB")})
+        target = pd.DataFrame(data={"A": list("ABCDEFG"), "B": list("ABCDCBA"), 'C': list("BCDECFP")})
+        builder.add_connector_persist('target', uri_file='working/data/target.csv')
+        builder.save_canonical('target', target)
+        result = tools.model_difference(df, 'target', on_key='A')
+        self.assertEqual((2,3), result.shape)
+        self.assertEqual(['D', 'G'], result['A'].tolist())
+
 
     def test_raise(self):
         with self.assertRaises(KeyError) as context:
             env = os.environ['NoEnvValueTest']
         self.assertTrue("'NoEnvValueTest'" in str(context.exception))
```

### Comparing `discovery-transition-ds-4.9.8/tests/intent/wrangle_intent_test.py` & `discovery-transition-ds-4.9.9/tests/intent/wrangle_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/managers/transition_pm_test.py` & `discovery-transition-ds-4.9.9/tests/managers/transition_pm_test.py`

 * *Files identical despite different names*

### Comparing `discovery-transition-ds-4.9.8/tests/scratch/remote_run_demo.py` & `discovery-transition-ds-4.9.9/tests/scratch/remote_run_demo.py`

 * *Files identical despite different names*

