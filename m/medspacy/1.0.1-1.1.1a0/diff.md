# Comparing `tmp/medspacy-1.0.1.tar.gz` & `tmp/medspacy-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspacy-1.0.1.tar", last modified: Mon Nov 28 20:19:52 2022, max compression
+gzip compressed data, was "medspacy-1.1.1a0.tar", last modified: Mon May  8 15:13:58 2023, max compression
```

## Comparing `medspacy-1.0.1.tar` & `medspacy-1.1.1a0.tar`

### file list

```diff
@@ -1,145 +1,146 @@
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.609281 medspacy-1.0.1/
--rw-rw-rw-   0        0        0     1086 2022-10-17 23:12:39.000000 medspacy-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     7128 2022-11-28 20:19:52.608280 medspacy-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2022-10-17 23:12:39.000000 medspacy-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.460780 medspacy-1.0.1/medspacy/
--rw-rw-rw-   0        0        0      225 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/__init__.py
--rw-rw-rw-   0        0        0     9786 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/_extensions.py
--rw-rw-rw-   0        0        0       23 2022-11-28 20:17:59.000000 medspacy-1.0.1/medspacy/_version.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.219281 medspacy-1.0.1/medspacy/common/
--rw-rw-rw-   0        0        0       33 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/__init__.py
--rw-rw-rw-   0        0        0     2130 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/base_rule.py
--rw-rw-rw-   0        0        0     6003 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/medspacy_matcher.py
--rw-rw-rw-   0        0        0     6845 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/regex_matcher.py
--rw-rw-rw-   0        0        0     6335 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/common/util.py
--rw-rw-rw-   0        0        0      518 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/components.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.288280 medspacy-1.0.1/medspacy/context/
--rw-rw-rw-   0        0        0      354 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/__init__.py
--rw-rw-rw-   0        0        0    13692 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context.py
--rw-rw-rw-   0        0        0     4572 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_graph.py
--rw-rw-rw-   0        0        0    15439 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_modifier.py
--rw-rw-rw-   0        0        0    11079 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/context_rule.py
--rw-rw-rw-   0        0        0      687 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/context/util.py
--rw-rw-rw-   0        0        0     1934 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/custom_tokenizer.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.386281 medspacy-1.0.1/medspacy/io/
--rw-rw-rw-   0        0        0      250 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/__init__.py
--rw-rw-rw-   0        0        0     5027 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/config_example.py
--rw-rw-rw-   0        0        0      133 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db.py
--rw-rw-rw-   0        0        0     3415 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_connect.py
--rw-rw-rw-   0        0        0      910 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_reader.py
--rw-rw-rw-   0        0        0     5737 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/db_writer.py
--rw-rw-rw-   0        0        0    11707 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/doc_consumer.py
--rw-rw-rw-   0        0        0     2847 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/io/pipeline.py
--rw-rw-rw-   0        0        0       98 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/ner.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.447780 medspacy-1.0.1/medspacy/postprocess/
--rw-rw-rw-   0        0        0      298 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/__init__.py
--rw-rw-rw-   0        0        0     8954 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_functions.py
--rw-rw-rw-   0        0        0     1529 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_pattern.py
--rw-rw-rw-   0        0        0     3450 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessing_rule.py
--rw-rw-rw-   0        0        0     4313 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/postprocess/postprocessor.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.478281 medspacy-1.0.1/medspacy/preprocess/
--rw-rw-rw-   0        0        0      142 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/__init__.py
--rw-rw-rw-   0        0        0     4507 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/preprocessing_rule.py
--rw-rw-rw-   0        0        0     1840 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/preprocess/preprocessor.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.530780 medspacy-1.0.1/medspacy/section_detection/
--rw-rw-rw-   0        0        0      192 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/__init__.py
--rw-rw-rw-   0        0        0     5399 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/section.py
--rw-rw-rw-   0        0        0     6085 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/section_rule.py
--rw-rw-rw-   0        0        0    22288 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/sectionizer.py
--rw-rw-rw-   0        0        0     1627 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/section_detection/util.py
--rw-rw-rw-   0        0        0      765 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/sentence_splitting.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.569781 medspacy-1.0.1/medspacy/target_matcher/
--rw-rw-rw-   0        0        0      123 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/__init__.py
--rw-rw-rw-   0        0        0     2873 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/concept_tagger.py
--rw-rw-rw-   0        0        0     7355 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/target_matcher.py
--rw-rw-rw-   0        0        0     5196 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/target_matcher/target_rule.py
--rw-rw-rw-   0        0        0     8771 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/util.py
--rw-rw-rw-   0        0        0    11337 2022-10-17 23:12:39.000000 medspacy-1.0.1/medspacy/visualization.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.531280 medspacy-1.0.1/medspacy.egg-info/
--rw-rw-rw-   0        0        0     7128 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9130 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-11-28 20:19:51.000000 medspacy-1.0.1/medspacy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.564783 medspacy-1.0.1/resources/
--rw-rw-rw-   0        0        0    29201 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/context_rules.json
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.351781 medspacy-1.0.1/resources/quickumls/
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.601782 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
--rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.619279 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
--rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.835780 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
--rw-rw-rw-   0        0        0     6116 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
--rw-rw-rw-   0        0        0     6892 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-rw-rw-   0        0        0     2788 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-rw-rw-   0        0        0     2664 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-rw-rw-   0        0        0     2744 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-rw-rw-   0        0        0     3016 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-rw-rw-   0        0        0     2904 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-rw-rw-   0        0        0     3140 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-rw-rw-   0        0        0     3228 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-rw-rw-   0        0        0     3460 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-rw-rw-   0        0        0     3148 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-rw-rw-   0        0        0     7344 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-rw-rw-   0        0        0     3224 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-rw-rw-   0        0        0     4984 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-rw-rw-   0        0        0     5152 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-rw-rw-   0        0        0     5024 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-rw-rw-   0        0        0     3384 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-rw-rw-   0        0        0     3824 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-rw-rw-   0        0        0     3544 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-rw-rw-   0        0        0     4064 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-rw-rw-   0        0        0     3624 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-rw-rw-   0        0        0     5160 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-rw-rw-   0        0        0     3788 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-rw-rw-   0        0        0     5368 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-rw-rw-   0        0        0     2384 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.863781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
--rw-rw-rw-   0        0        0      183 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:51.881781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
--rw-rw-rw-   0        0        0    20480 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
--rw-rw-rw-   0        0        0    12288 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
--rw-rw-rw-   0        0        0        7 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
--rw-rw-rw-   0        0        0        3 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.164781 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
--rw-rw-rw-   0        0        0     2912 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
--rw-rw-rw-   0        0        0     6162 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
--rw-rw-rw-   0        0        0     2540 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
--rw-rw-rw-   0        0        0     2574 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
--rw-rw-rw-   0        0        0     2642 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
--rw-rw-rw-   0        0        0     2884 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
--rw-rw-rw-   0        0        0     2778 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
--rw-rw-rw-   0        0        0     2990 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
--rw-rw-rw-   0        0        0     3066 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
--rw-rw-rw-   0        0        0     3262 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
--rw-rw-rw-   0        0        0     2984 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
--rw-rw-rw-   0        0        0     5574 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
--rw-rw-rw-   0        0        0     3050 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
--rw-rw-rw-   0        0        0     4526 2022-10-17 23:12:39.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
--rw-rw-rw-   0        0        0     3546 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
--rw-rw-rw-   0        0        0     4616 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
--rw-rw-rw-   0        0        0     3186 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
--rw-rw-rw-   0        0        0     3576 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
--rw-rw-rw-   0        0        0     3322 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
--rw-rw-rw-   0        0        0     3780 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
--rw-rw-rw-   0        0        0     3390 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
--rw-rw-rw-   0        0        0     4696 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
--rw-rw-rw-   0        0        0     3528 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
--rw-rw-rw-   0        0        0     4828 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
--rw-rw-rw-   0        0        0     2336 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
--rw-rw-rw-   0        0        0    24473 2022-11-28 20:06:06.000000 medspacy-1.0.1/resources/rush_rules.tsv
--rw-rw-rw-   0        0        0    12637 2022-10-17 23:12:40.000000 medspacy-1.0.1/resources/section_patterns.json
--rw-rw-rw-   0        0        0       42 2022-11-28 20:19:52.609781 medspacy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2529 2022-11-28 20:17:36.000000 medspacy-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-28 20:19:52.605780 medspacy-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     3078 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_extensions.py
--rw-rw-rw-   0        0        0     7542 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_medspacy.py
--rw-rw-rw-   0        0        0     3678 2022-10-17 23:12:40.000000 medspacy-1.0.1/tests/test_notebooks.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.898040 medspacy-1.1.1a0/
+-rw-rw-rw-   0        0        0     1086 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/LICENSE
+-rw-rw-rw-   0        0        0     8429 2023-05-08 15:13:58.897040 medspacy-1.1.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     6790 2023-05-05 20:36:33.000000 medspacy-1.1.1a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.825596 medspacy-1.1.1a0/medspacy/
+-rw-rw-rw-   0        0        0      225 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/__init__.py
+-rw-rw-rw-   0        0        0     9786 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/_extensions.py
+-rw-rw-rw-   0        0        0       24 2023-05-08 15:13:45.000000 medspacy-1.1.1a0/medspacy/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.877917 medspacy-1.1.1a0/medspacy/common/
+-rw-rw-rw-   0        0        0       33 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/common/__init__.py
+-rw-rw-rw-   0        0        0     2130 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/common/base_rule.py
+-rw-rw-rw-   0        0        0     6003 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/common/medspacy_matcher.py
+-rw-rw-rw-   0        0        0     6845 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/common/regex_matcher.py
+-rw-rw-rw-   0        0        0     6335 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/common/util.py
+-rw-rw-rw-   0        0        0      518 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/components.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.880923 medspacy-1.1.1a0/medspacy/context/
+-rw-rw-rw-   0        0        0      354 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/context/__init__.py
+-rw-rw-rw-   0        0        0    13785 2023-05-05 21:54:27.000000 medspacy-1.1.1a0/medspacy/context/context.py
+-rw-rw-rw-   0        0        0     4572 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/context/context_graph.py
+-rw-rw-rw-   0        0        0    15439 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/context/context_modifier.py
+-rw-rw-rw-   0        0        0    11648 2023-05-05 16:50:11.000000 medspacy-1.1.1a0/medspacy/context/context_rule.py
+-rw-rw-rw-   0        0        0      687 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/context/util.py
+-rw-rw-rw-   0        0        0     1934 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/custom_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.885377 medspacy-1.1.1a0/medspacy/io/
+-rw-rw-rw-   0        0        0      250 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/__init__.py
+-rw-rw-rw-   0        0        0     5027 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/config_example.py
+-rw-rw-rw-   0        0        0      133 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/db.py
+-rw-rw-rw-   0        0        0     3415 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/db_connect.py
+-rw-rw-rw-   0        0        0      910 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/db_reader.py
+-rw-rw-rw-   0        0        0     5737 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/db_writer.py
+-rw-rw-rw-   0        0        0    11707 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/doc_consumer.py
+-rw-rw-rw-   0        0        0     2847 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/io/pipeline.py
+-rw-rw-rw-   0        0        0       98 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/ner.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.888633 medspacy-1.1.1a0/medspacy/postprocess/
+-rw-rw-rw-   0        0        0      298 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     8954 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/postprocess/postprocessing_functions.py
+-rw-rw-rw-   0        0        0     1536 2023-02-17 20:33:05.000000 medspacy-1.1.1a0/medspacy/postprocess/postprocessing_pattern.py
+-rw-rw-rw-   0        0        0     3450 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/postprocess/postprocessing_rule.py
+-rw-rw-rw-   0        0        0     4731 2023-05-05 16:50:11.000000 medspacy-1.1.1a0/medspacy/postprocess/postprocessor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.889633 medspacy-1.1.1a0/medspacy/preprocess/
+-rw-rw-rw-   0        0        0      142 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/preprocess/__init__.py
+-rw-rw-rw-   0        0        0     4507 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/preprocess/preprocessing_rule.py
+-rw-rw-rw-   0        0        0     1840 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/preprocess/preprocessor.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.892447 medspacy-1.1.1a0/medspacy/section_detection/
+-rw-rw-rw-   0        0        0      192 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/section_detection/__init__.py
+-rw-rw-rw-   0        0        0     5399 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/section_detection/section.py
+-rw-rw-rw-   0        0        0     6085 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/section_detection/section_rule.py
+-rw-rw-rw-   0        0        0    22288 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/section_detection/sectionizer.py
+-rw-rw-rw-   0        0        0     1627 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/section_detection/util.py
+-rw-rw-rw-   0        0        0      765 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/sentence_splitting.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.895030 medspacy-1.1.1a0/medspacy/target_matcher/
+-rw-rw-rw-   0        0        0      123 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/target_matcher/__init__.py
+-rw-rw-rw-   0        0        0     2913 2023-02-17 20:33:05.000000 medspacy-1.1.1a0/medspacy/target_matcher/concept_tagger.py
+-rw-rw-rw-   0        0        0     7355 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/target_matcher/target_matcher.py
+-rw-rw-rw-   0        0        0     5196 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/target_matcher/target_rule.py
+-rw-rw-rw-   0        0        0     8771 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/util.py
+-rw-rw-rw-   0        0        0    11337 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/medspacy/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.836850 medspacy-1.1.1a0/medspacy.egg-info/
+-rw-rw-rw-   0        0        0     8429 2023-05-08 15:13:58.000000 medspacy-1.1.1a0/medspacy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9145 2023-05-08 15:13:58.000000 medspacy-1.1.1a0/medspacy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 15:13:58.000000 medspacy-1.1.1a0/medspacy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-05-08 15:13:58.000000 medspacy-1.1.1a0/medspacy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-08 15:13:58.000000 medspacy-1.1.1a0/medspacy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      773 2023-05-08 15:01:39.000000 medspacy-1.1.1a0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.838765 medspacy-1.1.1a0/resources/
+-rw-rw-rw-   0        0        0    29201 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/context_rules.json
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.816591 medspacy-1.1.1a0/resources/quickumls/
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.840902 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.841901 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    12288 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.856858 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     6116 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6892 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2788 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2664 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2744 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     3016 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2904 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     3140 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3228 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3460 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     3148 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     7344 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3224 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4984 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     5152 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     5024 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3384 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3824 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3544 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     4064 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3624 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     5160 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3788 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     5368 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2384 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.858859 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/
+-rw-rw-rw-   0        0        0      183 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.859859 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/
+-rw-rw-rw-   0        0        0    20480 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite
+-rw-rw-rw-   0        0        0    12288 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite
+-rw-rw-rw-   0        0        0        7 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/database_backend.flag
+-rw-rw-rw-   0        0        0        3 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/language.flag
+-rw-rw-rw-   0        0        0        0 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/lowercase.flag
+-rw-rw-rw-   0        0        0        0 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/normalize-unicode.flag
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.875255 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/
+-rw-rw-rw-   0        0        0     2912 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring
+-rw-rw-rw-   0        0        0     6162 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb
+-rw-rw-rw-   0        0        0     2540 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb
+-rw-rw-rw-   0        0        0     2574 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb
+-rw-rw-rw-   0        0        0     2642 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb
+-rw-rw-rw-   0        0        0     2884 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb
+-rw-rw-rw-   0        0        0     2778 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb
+-rw-rw-rw-   0        0        0     2990 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb
+-rw-rw-rw-   0        0        0     3066 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb
+-rw-rw-rw-   0        0        0     3262 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb
+-rw-rw-rw-   0        0        0     2984 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb
+-rw-rw-rw-   0        0        0     5574 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb
+-rw-rw-rw-   0        0        0     3050 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb
+-rw-rw-rw-   0        0        0     4526 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb
+-rw-rw-rw-   0        0        0     3546 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb
+-rw-rw-rw-   0        0        0     4616 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb
+-rw-rw-rw-   0        0        0     3186 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb
+-rw-rw-rw-   0        0        0     3576 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb
+-rw-rw-rw-   0        0        0     3322 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb
+-rw-rw-rw-   0        0        0     3780 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb
+-rw-rw-rw-   0        0        0     3390 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb
+-rw-rw-rw-   0        0        0     4696 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb
+-rw-rw-rw-   0        0        0     3528 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb
+-rw-rw-rw-   0        0        0     4828 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb
+-rw-rw-rw-   0        0        0     2336 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb
+-rw-rw-rw-   0        0        0    24473 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/rush_rules.tsv
+-rw-rw-rw-   0        0        0    12637 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/resources/section_patterns.json
+-rw-rw-rw-   0        0        0       42 2023-05-08 15:13:58.898040 medspacy-1.1.1a0/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-05-05 20:36:33.000000 medspacy-1.1.1a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:13:58.896036 medspacy-1.1.1a0/tests/
+-rw-rw-rw-   0        0        0        0 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3078 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/tests/test_extensions.py
+-rw-rw-rw-   0        0        0     7542 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/tests/test_medspacy.py
+-rw-rw-rw-   0        0        0     3678 2022-12-01 03:21:19.000000 medspacy-1.1.1a0/tests/test_notebooks.py
```

### Comparing `medspacy-1.0.1/LICENSE` & `medspacy-1.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/PKG-INFO` & `medspacy-1.1.1a0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: medspacy
-Version: 1.0.1
-Summary: Library for clinical NLP with spaCy.
-Author: medSpaCy
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
 
 # medspacy
 Library for clinical NLP with spaCy. 
 
 ![alt text](./images/medspacy_logo.png "medSpaCy logo")
@@ -31,16 +22,15 @@
 - `medspacy.ner`: Utilities for extracting concepts from clinical text
 - `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
 for detecting semantic modifiers and attributes of entities, including negation and uncertainty
 - `medspacy.section_detection`: Clinical section detection and segmentation
 - `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
 - `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
 - `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
-- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS).  More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
-	- NOTE: This component is installed by default on MacOS and Linux but not Windows.  For more defails and Windows installation: [QuickUMLS on Windows](windows_and_quickumls.md)
+- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [our fork](https://github.com/medspacy/QuickUMLS) of [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS). More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
 
 Future work could include I/O, relations extraction, and pre-trained clinical models.
 
 **As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
 
 # Usage
 ## Installation
```

### Comparing `medspacy-1.0.1/README.md` & `medspacy-1.1.1a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: medspacy
+Version: 1.1.1a0
+Summary: Library for clinical NLP with spaCy.
+Author: medSpaCy
+License: MIT License
+        
+        Copyright (c) 2020 medspacy
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Source, https://github.com/medspacy/medspacy
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
 
 # medspacy
 Library for clinical NLP with spaCy. 
 
 ![alt text](./images/medspacy_logo.png "medSpaCy logo")
@@ -22,16 +56,15 @@
 - `medspacy.ner`: Utilities for extracting concepts from clinical text
 - `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
 for detecting semantic modifiers and attributes of entities, including negation and uncertainty
 - `medspacy.section_detection`: Clinical section detection and segmentation
 - `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
 - `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
 - `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
-- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS).  More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
-	- NOTE: This component is installed by default on MacOS and Linux but not Windows.  For more defails and Windows installation: [QuickUMLS on Windows](windows_and_quickumls.md)
+- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [our fork](https://github.com/medspacy/QuickUMLS) of [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS). More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
 
 Future work could include I/O, relations extraction, and pre-trained clinical models.
 
 **As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
 
 # Usage
 ## Installation
```

### Comparing `medspacy-1.0.1/medspacy/_extensions.py` & `medspacy-1.1.1a0/medspacy/_extensions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/common/base_rule.py` & `medspacy-1.1.1a0/medspacy/common/base_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/common/medspacy_matcher.py` & `medspacy-1.1.1a0/medspacy/common/medspacy_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/common/regex_matcher.py` & `medspacy-1.1.1a0/medspacy/common/regex_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/common/util.py` & `medspacy-1.1.1a0/medspacy/common/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/components.py` & `medspacy-1.1.1a0/medspacy/components.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/context/context.py` & `medspacy-1.1.1a0/medspacy/context/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,16 +239,19 @@
         self.__matcher.add(rules)
 
     @classmethod
     def register_graph_attributes(cls):
         """
         Registers spaCy attribute extensions: Span._.modifiers and Doc._.context_graph.
         """
-        Span.set_extension("modifiers", default=(), force=True)
-        Doc.set_extension("context_graph", default=None, force=True)
+        try:
+            Span.set_extension("modifiers", default=(), force=True)
+            Doc.set_extension("context_graph", default=None, force=True)
+        except ValueError:  # Extension already set
+            pass
 
     @classmethod
     def register_default_attributes(cls):
         """
         Registers the default values for the Span attributes defined in `DEFAULT_ATTRIBUTES`.
         """
         for attr_name in [
```

### Comparing `medspacy-1.0.1/medspacy/context/context_graph.py` & `medspacy-1.1.1a0/medspacy/context/context_graph.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/context/context_modifier.py` & `medspacy-1.1.1a0/medspacy/context/context_modifier.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/context/context_rule.py` & `medspacy-1.1.1a0/medspacy/context/context_rule.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,26 +200,42 @@
                 "JSON object contains invalid keys: {0}.\n"
                 "Must be one of: {1}".format(invalid_keys, cls._ALLOWED_KEYS)
             )
             raise ValueError(msg)
         rule = ConTextRule(**rule_dict)
         return rule
 
-    def to_dict(self) -> Dict[str, str]:
+    def to_dict(self):
         """
         Converts ConTextItems to a python dictionary. Used when writing context rules to a json file.
 
         Returns:
             The dictionary containing the ConTextRule info.
         """
         rule_dict = {}
         for key in self._ALLOWED_KEYS:
             value = self.__dict__.get(key)
+            if isinstance(value, set):
+                value = list(value)
             if value is not None:
                 rule_dict[key] = value
         return rule_dict
 
+    @classmethod
+    def to_json(cls, context_rules: List[ConTextRule], filepath: str):
+        """Writes ConTextItems to a json file.
+
+            Args:
+            context_rules: a list of ContextRules that will be written to a file.
+            filepath: the .json file to contain modifier rules
+        """
+        import json
+
+        data = {"context_rules": [rule.to_dict() for rule in context_rules]}
+        with open(filepath, "w") as file:
+            json.dump(data, file, indent=4)
+
     def __repr__(self):
         return (
             f"ConTextRule(literal='{self.literal}', category='{self.category}', pattern={self.pattern}, "
             f"direction='{self.direction}')"
         )
```

### Comparing `medspacy-1.0.1/medspacy/context/util.py` & `medspacy-1.1.1a0/medspacy/context/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/custom_tokenizer.py` & `medspacy-1.1.1a0/medspacy/custom_tokenizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/io/config_example.py` & `medspacy-1.1.1a0/medspacy/io/config_example.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/io/db_connect.py` & `medspacy-1.1.1a0/medspacy/io/db_connect.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/io/db_reader.py` & `medspacy-1.1.1a0/medspacy/io/db_reader.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/io/db_writer.py` & `medspacy-1.1.1a0/medspacy/io/db_writer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/io/doc_consumer.py` & `medspacy-1.1.1a0/medspacy/io/doc_consumer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/io/pipeline.py` & `medspacy-1.1.1a0/medspacy/io/pipeline.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/postprocess/postprocessing_functions.py` & `medspacy-1.1.1a0/medspacy/postprocess/postprocessing_functions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/postprocess/postprocessing_pattern.py` & `medspacy-1.1.1a0/medspacy/postprocess/postprocessing_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class PostprocessingPattern:
     """
     PostprocessingPatterns are callable functions and equality values wrapped together that will create triggers
     in the later Postprocessor as part of PostprocessingRules.
     """
 
-    def __init__(self, condition: Callable, success_value: Any, **kwargs):
+    def __init__(self, condition: Callable, success_value: Any = True, **kwargs):
         """
         A PostprocessingPattern defines a single condition to check against an entity.
 
         Args:
             condition: A function to call on an entity. If the result of the function call equals success_value, then
                 the pattern passes.
             success_value: The value which should be returned by condition(ent) in order for the pattern to pass. Must
```

### Comparing `medspacy-1.0.1/medspacy/postprocess/postprocessing_rule.py` & `medspacy-1.1.1a0/medspacy/postprocess/postprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/postprocess/postprocessor.py` & `medspacy-1.1.1a0/medspacy/postprocess/postprocessor.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,22 +110,31 @@
         else:
             spans = doc.spans[self._span_group_name]
 
         for i in range(len(spans) - 1, -1, -1):
             ent = spans[i]
             if self.debug:
                 print(ent)
+
+            # let's keep track of whether the rule makes a change to spans
+            span_count_before_rule = None
+            if self._input_span_type == "ents":
+                span_count_before_rule = len(doc.ents)
+            else:
+                span_count_before_rule = len(doc.spans[self.span_group_name])
+
             for rule in self.rules:
                 rule(ent, i, debug=self.debug)
-                # Check if the entity was removed -if it was, skip to the next entity
+                # Check if the entity was removed based on span counts before and after rule execution
+                # if it was, skip to the next entity
                 try:
                     if self._input_span_type == "ents":
-                        if len(doc.ents[i]) != len(spans):
+                        if len(doc.ents) != span_count_before_rule:
                             break
                     else:
-                        if len(doc.spans[self.span_group_name]) == len(spans):
+                        if len(doc.spans[self.span_group_name]) != span_count_before_rule:
                             break
                 except IndexError:
                     break
             # if self.debug:
             #     print()
         return doc
```

### Comparing `medspacy-1.0.1/medspacy/preprocess/preprocessing_rule.py` & `medspacy-1.1.1a0/medspacy/preprocess/preprocessing_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/preprocess/preprocessor.py` & `medspacy-1.1.1a0/medspacy/preprocess/preprocessor.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/section_detection/section.py` & `medspacy-1.1.1a0/medspacy/section_detection/section.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/section_detection/section_rule.py` & `medspacy-1.1.1a0/medspacy/section_detection/section_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/section_detection/sectionizer.py` & `medspacy-1.1.1a0/medspacy/section_detection/sectionizer.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/section_detection/util.py` & `medspacy-1.1.1a0/medspacy/section_detection/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/sentence_splitting.py` & `medspacy-1.1.1a0/medspacy/sentence_splitting.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/target_matcher/concept_tagger.py` & `medspacy-1.1.1a0/medspacy/target_matcher/concept_tagger.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,22 +32,20 @@
             attr_name: The name of the attribute to set to tokens.
         """
         self.nlp = nlp
         self.name = name
         self._attr_name = attr_name
         self.__matcher = MedspacyMatcher(nlp, name=name)
 
-        # If the token attribute hasn't been set, add it now
-        # try:
-        #     Token.set_extension(attr_name, default="")
-        # except:
-        #     pass
-
-        # not sure if silent errors here are beneficial, removing try statement for now.
-        Token.set_extension(self._attr_name, default="")
+        # If the token attribute hasn't been registered, add it now
+        # If it has already been set, then we can pass.
+        # This will happen, for example, if you've already instantiated
+        # the ConceptTagger and it registered the attribute.
+        if not Token.has_extension(attr_name):
+            Token.set_extension(attr_name, default="")
 
     @property
     def attr_name(self) -> str:
         """
         The name of the attribute that will be set on each matched token.
 
         Returns:
```

### Comparing `medspacy-1.0.1/medspacy/target_matcher/target_matcher.py` & `medspacy-1.1.1a0/medspacy/target_matcher/target_matcher.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/target_matcher/target_rule.py` & `medspacy-1.1.1a0/medspacy/target_matcher/target_rule.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/util.py` & `medspacy-1.1.1a0/medspacy/util.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy/visualization.py` & `medspacy-1.1.1a0/medspacy/visualization.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/medspacy.egg-info/PKG-INFO` & `medspacy-1.1.1a0/medspacy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,37 @@
 Metadata-Version: 2.1
 Name: medspacy
-Version: 1.0.1
+Version: 1.1.1a0
 Summary: Library for clinical NLP with spaCy.
 Author: medSpaCy
+License: MIT License
+        
+        Copyright (c) 2020 medspacy
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Source, https://github.com/medspacy/medspacy
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![Build Status](https://github.com/medspacy/medspacy/workflows/medspacy/badge.svg)
 
@@ -31,16 +56,15 @@
 - `medspacy.ner`: Utilities for extracting concepts from clinical text
 - `medspacy.context`: Implementation of the [ConText](https://www.sciencedirect.com/science/article/pii/S1532046409000744)
 for detecting semantic modifiers and attributes of entities, including negation and uncertainty
 - `medspacy.section_detection`: Clinical section detection and segmentation
 - `medspacy.postprocess`: Flexible framework for modifying and removing extracted entities
 - `medspacy.io`: Utilities for converting processed texts to structured data and interacting with databases
 - `medspacy.visualization`: Utilities for visualizing concepts and relationships extracted from text
-- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS).  More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
-	- NOTE: This component is installed by default on MacOS and Linux but not Windows.  For more defails and Windows installation: [QuickUMLS on Windows](windows_and_quickumls.md)
+- `SpacyQuickUMLS`: UMLS concept extraction compatible with spacy and medspacy implemented by [our fork](https://github.com/medspacy/QuickUMLS) of [QuickUMLS](https://github.com/Georgetown-IR-Lab/QuickUMLS). More detail on this component, how to use it, how to generate UMLS resources beyond the small UMLS sample can be found in [this notebook](notebooks/11-QuickUMLS_Extraction.ipynb).
 
 Future work could include I/O, relations extraction, and pre-trained clinical models.
 
 **As of 10/2/2021 (version 0.2.0.0), medspaCy supports spaCy v3**
 
 # Usage
 ## Installation
```

### Comparing `medspacy-1.0.1/medspacy.egg-info/SOURCES.txt` & `medspacy-1.1.1a0/medspacy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 medspacy/__init__.py
 medspacy/_extensions.py
 medspacy/_version.py
 medspacy/components.py
 medspacy/custom_tokenizer.py
 medspacy/ner.py
```

### Comparing `medspacy-1.0.1/resources/context_rules.json` & `medspacy-1.1.1a0/resources/context_rules.json`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_POSIX_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/cui.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/cui-semtypes.db/semtypes.unqlite`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.120.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.14.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.15.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.17.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.20.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.21.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.22.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.24.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.26.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.27.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.28.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.29.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.30.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.31.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.32.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.33.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.35.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.37.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.38.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.39.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.40.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.43.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.79.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb` & `medspacy-1.1.1a0/resources/quickumls/QuickUMLS_SAMPLE_lowercase_Windows_unqlite/umls-simstring.db/umls-terms.simstring.8.cdb`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/rush_rules.tsv` & `medspacy-1.1.1a0/resources/rush_rules.tsv`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/resources/section_patterns.json` & `medspacy-1.1.1a0/resources/section_patterns.json`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/setup.py` & `medspacy-1.1.1a0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,17 @@
 from setuptools import setup, find_packages
-from sys import platform
 
 # read the contents of the README file
 import os
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-additional_installs = []
-if platform.startswith("win"):
-    print(
-        "Not installing QuickUMLS for Windows since it currently requires conda (as opposed to just pip)"
-    )
-else:
-    # Using a trick from StackOverflow to set an impossibly high version number
-    # to force getting latest from GitHub as opposed to PyPi
-    # since QuickUMLS has not made a release with some recent MedSpacy contributions...
-    quickumls_package = "medspacy_quickumls==2.7"
-    additional_installs.append(quickumls_package)
-    print("Attempting to install quickumls package: {}".format(quickumls_package))
-
 # function to recursively get files for resourcee
 def package_files(directory):
     paths = []
     for (p, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join("..", p, filename))
     return paths
@@ -58,18 +44,18 @@
 setup(
     name="medspacy",
     version=get_version(),
     description="Library for clinical NLP with spaCy.",
     author="medSpaCy",
     packages=find_packages(),
     install_requires=[
-        "spacy>=3.4.1",
+        "spacy>=3.4.1, <4.0",
         "PyRuSH>=1.0.8",
         "pysbd==0.3.4",
         "jsonschema",
-    ]
-    + additional_installs,
+        "medspacy_quickumls==3.0"
+    ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={"medspacy": resource_files},
     python_requires=">=3.8.0",
 )
```

### Comparing `medspacy-1.0.1/tests/test_extensions.py` & `medspacy-1.1.1a0/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/tests/test_medspacy.py` & `medspacy-1.1.1a0/tests/test_medspacy.py`

 * *Files identical despite different names*

### Comparing `medspacy-1.0.1/tests/test_notebooks.py` & `medspacy-1.1.1a0/tests/test_notebooks.py`

 * *Files identical despite different names*

