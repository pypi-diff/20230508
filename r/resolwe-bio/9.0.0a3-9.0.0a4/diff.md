# Comparing `tmp/resolwe-bio-9.0.0a3.tar.gz` & `tmp/resolwe-bio-9.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resolwe-bio-9.0.0a3.tar", last modified: Wed May  2 10:17:56 2018, max compression
+gzip compressed data, was "dist/resolwe-bio-9.0.0a4.tar", last modified: Mon May 14 12:46:07 2018, max compression
```

## Comparing `resolwe-bio-9.0.0a3.tar` & `resolwe-bio-9.0.0a4.tar`

### file list

```diff
@@ -1,925 +1,929 @@
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/
--rw-r--r--   0 domen      (501) staff       (20)     5690 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/PKG-INFO
--rw-r--r--   0 domen      (501) staff       (20)    13070 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/.pylintrc
--rw-r--r--   0 domen      (501) staff       (20)      575 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/.resolwebio-filetypes.yml
--rw-r--r--   0 domen      (501) staff       (20)    11358 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/LICENSE
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio.egg-info/
--rw-r--r--   0 domen      (501) staff       (20)     5690 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio.egg-info/PKG-INFO
--rw-r--r--   0 domen      (501) staff       (20)        1 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio.egg-info/not-zip-safe
--rw-r--r--   0 domen      (501) staff       (20)    39981 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio.egg-info/SOURCES.txt
--rw-r--r--   0 domen      (501) staff       (20)      334 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio.egg-info/requires.txt
--rw-r--r--   0 domen      (501) staff       (20)       12 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio.egg-info/top_level.txt
--rw-r--r--   0 domen      (501) staff       (20)        1 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio.egg-info/dependency_links.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/
--rw-r--r--   0 domen      (501) staff       (20)      644 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0005_make_date_indexes.py
--rw-r--r--   0 domen      (501) staff       (20)      535 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0010_add_relation_types.py
--rw-r--r--   0 domen      (501) staff       (20)      478 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0006_alter_versionfield.py
--rw-r--r--   0 domen      (501) staff       (20)      690 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0004_add_owner.py
--rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     2343 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0008_migrate_sample.py
--rw-r--r--   0 domen      (501) staff       (20)     1019 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0009_delete_sample.py
--rw-r--r--   0 domen      (501) staff       (20)      466 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0007_sample_descriptor_dirty.py
--rw-r--r--   0 domen      (501) staff       (20)     2401 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0001_initial.py
--rw-r--r--   0 domen      (501) staff       (20)      444 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0002_sample_presample.py
--rw-r--r--   0 domen      (501) staff       (20)      705 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/migrations/0003_fix_jsonfields.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/
--rwxr-xr-x   0 domen      (501) staff       (20)      620 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/convert_DE_excel_table.py
--rwxr-xr-x   0 domen      (501) staff       (20)     5119 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/basespace_download.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2119 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/plot_enhancers.py
--rwxr-xr-x   0 domen      (501) staff       (20)      958 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_library_type.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2375 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/make_igv_session_archive.py
--rwxr-xr-x   0 domen      (501) staff       (20)      784 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/VCF_ad_extract.py
--rwxr-xr-x   0 domen      (501) staff       (20)     5180 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/xgff.py
--rwxr-xr-x   0 domen      (501) staff       (20)    18647 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/make_multireport.py
--rwxr-xr-x   0 domen      (501) staff       (20)     9251 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/xexpression.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1328 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_star_expressions.py
--rwxr-xr-x   0 domen      (501) staff       (20)      738 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/cufflinks_sample_groups.py
--rwxr-xr-x   0 domen      (501) staff       (20)     3185 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/transmart_fetch.R
--rw-r--r--   0 domen      (501) staff       (20)     7149 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/transmart_utils.py
--rwxr-xr-x   0 domen      (501) staff       (20)     7460 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/samplehcluster.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2846 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/goea.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2976 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/lofreq2_indel_ovlp.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2099 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/expressionmerge.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1442 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/xgtf2gff.py
--rwxr-xr-x   0 domen      (501) staff       (20)      516 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/cuffnorm_group_labels.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1743 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/mergebowtiestats.py
--rwxr-xr-x   0 domen      (501) staff       (20)     3372 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/etc.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2414 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/rnaseq.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1631 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/peak2geneScore.R
--rwxr-xr-x   0 domen      (501) staff       (20)     9964 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/demultiplex.py
--rw-r--r--   0 domen      (501) staff       (20)     6612 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/clustering_leaf_ordering.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1052 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/run_edger.R
--rwxr-xr-x   0 domen      (501) staff       (20)     1392 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/format_index_files.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1543 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/deseq.R
--rwxr-xr-x   0 domen      (501) staff       (20)    10893 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/garvan_coverage.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1076 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/make_igv_session.py
--rwxr-xr-x   0 domen      (501) staff       (20)      611 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/diffexp_filtering.R
--rwxr-xr-x   0 domen      (501) staff       (20)     6446 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/expression_aggregator.py
--rw-r--r--   0 domen      (501) staff       (20)      213 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/utils.py
--rwxr-xr-x   0 domen      (501) staff       (20)    11687 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/make_report.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2071 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/expressionmerge_archive.py
--rwxr-xr-x   0 domen      (501) staff       (20)     3844 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/mappability.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2641 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_diffexp.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1152 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/geneset2storage.py
--rwxr-xr-x   0 domen      (501) staff       (20)     4616 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/pca.py
--rwxr-xr-x   0 domen      (501) staff       (20)     7835 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/genehcluster.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2124 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/find_similar.py
--rwxr-xr-x   0 domen      (501) staff       (20)     3877 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/plotcoverage_html.py
--rwxr-xr-x   0 domen      (501) staff       (20)     3434 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/transmart_import.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1632 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/detect_strandedness.sh
--rwxr-xr-x   0 domen      (501) staff       (20)      672 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/fastqc.sh
--rwxr-xr-x   0 domen      (501) staff       (20)     3642 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/compatibilty_check.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1718 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/mergeetc.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1849 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/expression_fpkm_tpm.R
--rwxr-xr-x   0 domen      (501) staff       (20)     1070 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_cuffnorm.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1921 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/mergebowtie2stats_paired.py
--rwxr-xr-x   0 domen      (501) staff       (20)      651 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/add_header.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2341 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_closest_features.R
--rwxr-xr-x   0 domen      (501) staff       (20)     1609 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/importETC.py
--rwxr-xr-x   0 domen      (501) staff       (20)      674 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_encoding_type.py
--rwxr-xr-x   0 domen      (501) staff       (20)     2671 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/volcanoplot.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1606 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/mergebowtie2stats.py
--rwxr-xr-x   0 domen      (501) staff       (20)     3082 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/feature_location.py
--rwxr-xr-x   0 domen      (501) staff       (20)      574 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/unique_sample_names.py
--rwxr-xr-x   0 domen      (501) staff       (20)      996 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/microarrayQC.R
--rwxr-xr-x   0 domen      (501) staff       (20)     1003 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/bamliquidator_table.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1591 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/go_genesets.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1952 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/cuffnorm_output_table_headers.py
--rwxr-xr-x   0 domen      (501) staff       (20)     6776 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/xtabcoverage.py
--rwxr-xr-x   0 domen      (501) staff       (20)     6168 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/make_amplicon_table.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1425 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/gff3_to_gtf.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1524 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/validate_master_file.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1255 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a3/resolwe_bio/tools/expression2storage.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/
--rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)      482 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0003_add_map_index.py
--rw-r--r--   0 domen      (501) staff       (20)     1139 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0002_alter_field_max_length.py
--rw-r--r--   0 domen      (501) staff       (20)     2273 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0001_initial.py
--rw-r--r--   0 domen      (501) staff       (20)      477 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0004_add_unique_together.py
--rw-r--r--   0 domen      (501) staff       (20)     2230 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0005_species.py
--rw-r--r--   0 domen      (501) staff       (20)     4114 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/models.py
--rw-r--r--   0 domen      (501) staff       (20)      731 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/serializers.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/
--rw-r--r--   0 domen      (501) staff       (20)    10892 2018-04-04 14:30:41.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/test_feature.py
--rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     1265 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/test_import_kb.py
--rw-r--r--   0 domen      (501) staff       (20)     6051 2018-04-04 14:30:41.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/test_mapping.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/management/
--rw-r--r--   0 domen      (501) staff       (20)       25 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/management/__init__.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/
--rw-r--r--   0 domen      (501) staff       (20)     4918 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/insert_features.py
--rw-r--r--   0 domen      (501) staff       (20)       34 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     1620 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/utils.py
--rw-r--r--   0 domen      (501) staff       (20)     5038 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/insert_mappings.py
--rw-r--r--   0 domen      (501) staff       (20)      245 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)      355 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/apps.py
--rw-r--r--   0 domen      (501) staff       (20)      525 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/admin.py
--rw-r--r--   0 domen      (501) staff       (20)     3815 2018-03-28 20:35:19.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/elastic_indexes.py
--rw-r--r--   0 domen      (501) staff       (20)      770 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/filters.py
--rw-r--r--   0 domen      (501) staff       (20)     7352 2018-04-04 14:30:41.000000 resolwe-bio-9.0.0a3/resolwe_bio/kb/views.py
--rw-r--r--   0 domen      (501) staff       (20)      134 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/models.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/transmart/
--rw-r--r--   0 domen      (501) staff       (20)     2014 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/transmart/import.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/go_enrichment/
--rw-r--r--   0 domen      (501) staff       (20)     2893 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/go_enrichment/go.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/
--rw-r--r--   0 domen      (501) staff       (20)     5018 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/edgeR.yml
--rw-r--r--   0 domen      (501) staff       (20)     4554 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/deseq.yml
--rw-r--r--   0 domen      (501) staff       (20)     9429 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/cuffdiff.yml
--rw-r--r--   0 domen      (501) staff       (20)      870 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/abstract.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/
--rw-r--r--   0 domen      (501) staff       (20)      904 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_list.yml
--rw-r--r--   0 domen      (501) staff       (20)     1306 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_hidden_fields.yml
--rw-r--r--   0 domen      (501) staff       (20)     1117 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_disabled_fields.yml
--rw-r--r--   0 domen      (501) staff       (20)     6955 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_basic_fields.yml
--rw-r--r--   0 domen      (501) staff       (20)     1061 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_sleep_progress.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/amplicon/
--rw-r--r--   0 domen      (501) staff       (20)     1748 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/amplicon/amplicon_table.yml
--rw-r--r--   0 domen      (501) staff       (20)     2010 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/amplicon/target_metrics.yml
--rw-r--r--   0 domen      (501) staff       (20)     7402 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/amplicon/bwa_trim.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/assembly/
--rw-r--r--   0 domen      (501) staff       (20)     4276 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/assembly/abyss.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/clustering/
--rw-r--r--   0 domen      (501) staff       (20)     4060 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/clustering/pca.yml
--rw-r--r--   0 domen      (501) staff       (20)     1244 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/clustering/find_similar.yml
--rw-r--r--   0 domen      (501) staff       (20)    12221 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/clustering/hierarchical_clustering.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/
--rw-r--r--   0 domen      (501) staff       (20)    41865 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/bbduk_star_featurecounts.yml
--rw-r--r--   0 domen      (501) staff       (20)    23046 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/cutadapt_star_htseq.yml
--rw-r--r--   0 domen      (501) staff       (20)    10532 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/rnaseq.yml
--rw-r--r--   0 domen      (501) staff       (20)     1273 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/wgbs.yml
--rw-r--r--   0 domen      (501) staff       (20)     1682 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/heat_seq.yml
--rw-r--r--   0 domen      (501) staff       (20)     5340 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/bbduk_star_htseq.yml
--rw-r--r--   0 domen      (501) staff       (20)    13388 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/amplicon.yml
--rw-r--r--   0 domen      (501) staff       (20)      809 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/cuffquant.yml
--rw-r--r--   0 domen      (501) staff       (20)    19834 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/cutadapt_star_rsem.yml
--rw-r--r--   0 domen      (501) staff       (20)     2279 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/mirna.yml
--rw-r--r--   0 domen      (501) staff       (20)     5787 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/chemut.yml
--rw-r--r--   0 domen      (501) staff       (20)     1085 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/chip_seq.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/
--rw-r--r--   0 domen      (501) staff       (20)     2563 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/nucleotide_seq.yml
--rw-r--r--   0 domen      (501) staff       (20)     6870 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/geneset.yml
--rw-r--r--   0 domen      (501) staff       (20)     3798 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/master_file.yml
--rw-r--r--   0 domen      (501) staff       (20)     7124 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/genome.yml
--rw-r--r--   0 domen      (501) staff       (20)     1913 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/go_gaf.yml
--rw-r--r--   0 domen      (501) staff       (20)     4675 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/annotation.yml
--rw-r--r--   0 domen      (501) staff       (20)      896 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/sam_header.yml
--rw-r--r--   0 domen      (501) staff       (20)    12787 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/expressions.yml
--rw-r--r--   0 domen      (501) staff       (20)     9629 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/sra_file.yml
--rw-r--r--   0 domen      (501) staff       (20)      921 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/variants_bed.yml
--rw-r--r--   0 domen      (501) staff       (20)     5810 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/differential_exp.yml
--rw-r--r--   0 domen      (501) staff       (20)     1126 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/etc.yml
--rw-r--r--   0 domen      (501) staff       (20)     1156 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/basespace.yml
--rw-r--r--   0 domen      (501) staff       (20)      441 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/abstract_bed.yml
--rw-r--r--   0 domen      (501) staff       (20)     2720 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/cuffquant.yml
--rw-r--r--   0 domen      (501) staff       (20)     1382 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/snpeff.yml
--rw-r--r--   0 domen      (501) staff       (20)     1294 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/target_pcr_metrics.yml
--rw-r--r--   0 domen      (501) staff       (20)     2047 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/variants_vcf.yml
--rw-r--r--   0 domen      (501) staff       (20)     1418 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/pathway_map.yml
--rw-r--r--   0 domen      (501) staff       (20)     1280 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/hmmer_database.yml
--rw-r--r--   0 domen      (501) staff       (20)     1138 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/go_obo.yml
--rw-r--r--   0 domen      (501) staff       (20)     1081 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/mappability_bigwig.yml
--rw-r--r--   0 domen      (501) staff       (20)      970 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/mappability_tab.yml
--rw-r--r--   0 domen      (501) staff       (20)     1966 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/annotation_bed.yml
--rw-r--r--   0 domen      (501) staff       (20)     6018 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/seq_reads_multiplexed.yml
--rw-r--r--   0 domen      (501) staff       (20)     6775 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/bam.yml
--rw-r--r--   0 domen      (501) staff       (20)    14786 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/seq_reads.yml
--rw-r--r--   0 domen      (501) staff       (20)     1059 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/microarray_affy.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/annotation/
--rw-r--r--   0 domen      (501) staff       (20)     4393 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/annotation/cuffmerge.yml
--rw-r--r--   0 domen      (501) staff       (20)     2558 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/annotation/feature_location.yml
--rw-r--r--   0 domen      (501) staff       (20)      543 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/annotation/abstract.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/WGBS/
--rw-r--r--   0 domen      (501) staff       (20)     3873 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/WGBS/mcall.yml
--rw-r--r--   0 domen      (501) staff       (20)     4050 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/WGBS/bsmap.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/
--rw-r--r--   0 domen      (501) staff       (20)     3543 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/macs14.yml
--rw-r--r--   0 domen      (501) staff       (20)     2594 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/scoring.yml
--rw-r--r--   0 domen      (501) staff       (20)     4225 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/rose2.yml
--rw-r--r--   0 domen      (501) staff       (20)    13606 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/macs2.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/microarray/
--rw-r--r--   0 domen      (501) staff       (20)     1871 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/microarray/microarray_qc.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/
--rw-r--r--   0 domen      (501) staff       (20)    24667 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/star.yml
--rw-r--r--   0 domen      (501) staff       (20)     5071 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/hisat2.yml
--rw-r--r--   0 domen      (501) staff       (20)    10716 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/tophat.yml
--rw-r--r--   0 domen      (501) staff       (20)    24280 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/bowtie.yml
--rw-r--r--   0 domen      (501) staff       (20)     6237 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/subread.yml
--rw-r--r--   0 domen      (501) staff       (20)    16172 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/bwa.yml
--rw-r--r--   0 domen      (501) staff       (20)      536 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/abstract.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/genome_browser/
--rw-r--r--   0 domen      (501) staff       (20)     1598 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/genome_browser/igv_bam.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/
--rw-r--r--   0 domen      (501) staff       (20)    26014 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/featureCounts.yml
--rw-r--r--   0 domen      (501) staff       (20)     5357 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/dicty_bcm.yml
--rw-r--r--   0 domen      (501) staff       (20)     1616 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/merge_expressions.yml
--rw-r--r--   0 domen      (501) staff       (20)    14353 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/htseq_count.yml
--rw-r--r--   0 domen      (501) staff       (20)     1143 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/merge_etc.yml
--rw-r--r--   0 domen      (501) staff       (20)     4250 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/index_fasta_nucl.yml
--rw-r--r--   0 domen      (501) staff       (20)     1030 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/etc.yml
--rw-r--r--   0 domen      (501) staff       (20)     8276 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/cuffnorm.yml
--rw-r--r--   0 domen      (501) staff       (20)     4546 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/cuffquant.yml
--rw-r--r--   0 domen      (501) staff       (20)     2486 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/mappability.yml
--rw-r--r--   0 domen      (501) staff       (20)     4240 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/rsem.yml
--rw-r--r--   0 domen      (501) staff       (20)     2746 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/salmon_index.yml
--rw-r--r--   0 domen      (501) staff       (20)     2687 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/expression_aggregator.yml
--rw-r--r--   0 domen      (501) staff       (20)     6271 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/cufflinks.yml
--rw-r--r--   0 domen      (501) staff       (20)      860 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/abstract.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/exome_coverage/
--rw-r--r--   0 domen      (501) staff       (20)     2445 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/exome_coverage/coverage_report.yml
--rw-r--r--   0 domen      (501) staff       (20)     3751 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/exome_coverage/coveragebed.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/
--rw-r--r--   0 domen      (501) staff       (20)     2913 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/hsqutils.yml
--rw-r--r--   0 domen      (501) staff       (20)    45518 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/bbduk.yml
--rw-r--r--   0 domen      (501) staff       (20)     2647 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/merge_to_paired_end.yml
--rw-r--r--   0 domen      (501) staff       (20)    17803 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/cutadapt.yml
--rw-r--r--   0 domen      (501) staff       (20)     6168 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/cutadapt_amplicon.yml
--rw-r--r--   0 domen      (501) staff       (20)     8614 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/prinseq_lite.yml
--rw-r--r--   0 domen      (501) staff       (20)    10039 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/fastq_mcf.yml
--rw-r--r--   0 domen      (501) staff       (20)     5884 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/cutadapt_custom.yml
--rw-r--r--   0 domen      (501) staff       (20)    10557 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/sortmerna.yml
--rw-r--r--   0 domen      (501) staff       (20)    28004 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/trimmomatic.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/
--rw-r--r--   0 domen      (501) staff       (20)     3657 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/preprocess_bam.yml
--rw-r--r--   0 domen      (501) staff       (20)     5784 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/gatk.yml
--rw-r--r--   0 domen      (501) staff       (20)    11783 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/vc_chemut.yml
--rw-r--r--   0 domen      (501) staff       (20)     3547 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/samtools.yml
--rw-r--r--   0 domen      (501) staff       (20)     5871 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/filtering_chemut.yml
--rw-r--r--   0 domen      (501) staff       (20)     2874 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/snpeff.yml
--rw-r--r--   0 domen      (501) staff       (20)     2388 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/hsqutils-dedup.yml
--rw-r--r--   0 domen      (501) staff       (20)     2304 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/lofreq.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/plots/
--rw-r--r--   0 domen      (501) staff       (20)     6877 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/plots/bamplot.yml
--rw-r--r--   0 domen      (501) staff       (20)     6700 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/plots/bamliquidator.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reports/
--rw-r--r--   0 domen      (501) staff       (20)     3272 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reports/amplicon_report.yml
--rw-r--r--   0 domen      (501) staff       (20)     4364 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/reports/amplicon_multi_report.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/
--rw-r--r--   0 domen      (501) staff       (20)     1243 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/annotation_gtf.yml
--rw-r--r--   0 domen      (501) staff       (20)     1254 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/annotation_gff3.yml
--rw-r--r--   0 domen      (501) staff       (20)     1238 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/refseq.yml
--rw-r--r--   0 domen      (501) staff       (20)     1465 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/bam_coverage.yml
--rw-r--r--   0 domen      (501) staff       (20)     2012 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/annotation_bed.yml
--rw-r--r--   0 domen      (501) staff       (20)     4175 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/bam_coverage_normalized.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/
--rw-r--r--   0 domen      (501) staff       (20)     1257 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/gff_to_gtf.yml
--rw-r--r--   0 domen      (501) staff       (20)     4407 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/bam_split.yml
--rw-r--r--   0 domen      (501) staff       (20)     1619 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/refseq_compatibility.yml
--rw-r--r--   0 domen      (501) staff       (20)     1295 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/bam_coverage.yml
--rw-r--r--   0 domen      (501) staff       (20)    10427 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/prepare_geo.yml
--rw-r--r--   0 domen      (501) staff       (20)     3410 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/library_strandedness.yml
--rw-r--r--   0 domen      (501) staff       (20)     4106 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/archive.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/unit/
--rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/unit/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     3768 2018-04-09 16:06:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/unit/test_api.py
--rw-r--r--   0 domen      (501) staff       (20)      706 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/unit/test_tools.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/
--rw-r--r--   0 domen      (501) staff       (20)     1118 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_genome_browser.py
--rwxr-xr-x   0 domen      (501) staff       (20)     1723 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_wgbs.py
--rw-r--r--   0 domen      (501) staff       (20)    18699 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_reads_filtering.py
--rw-r--r--   0 domen      (501) staff       (20)     4370 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_plots.py
--rw-r--r--   0 domen      (501) staff       (20)     3150 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_coverage.py
--rw-r--r--   0 domen      (501) staff       (20)     2929 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_amplicon.py
--rw-r--r--   0 domen      (501) staff       (20)     2745 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_demultiplex.py
--rw-r--r--   0 domen      (501) staff       (20)    19185 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_expression.py
--rw-r--r--   0 domen      (501) staff       (20)     5207 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_generate_report.py
--rw-r--r--   0 domen      (501) staff       (20)     2394 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_expression_aggregator.py
--rw-r--r--   0 domen      (501) staff       (20)     1457 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_reads_manipulation.py
--rw-r--r--   0 domen      (501) staff       (20)       57 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     4883 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_files_to_reads.py
--rw-r--r--   0 domen      (501) staff       (20)      895 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_genome_coverage.py
--rw-r--r--   0 domen      (501) staff       (20)    11749 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_transmart.py
--rw-r--r--   0 domen      (501) staff       (20)    14408 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_alignment.py
--rw-r--r--   0 domen      (501) staff       (20)     2650 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_import.py
--rw-r--r--   0 domen      (501) staff       (20)     4045 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_jbrowse.py
--rw-r--r--   0 domen      (501) staff       (20)    17969 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_upload.py
--rw-r--r--   0 domen      (501) staff       (20)     1057 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_assembler.py
--rw-r--r--   0 domen      (501) staff       (20)      711 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_pathway_map.py
--rw-r--r--   0 domen      (501) staff       (20)    11724 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_variant_calling.py
--rw-r--r--   0 domen      (501) staff       (20)     4105 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_chipseq.py
--rw-r--r--   0 domen      (501) staff       (20)     2126 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_enrichment.py
--rw-r--r--   0 domen      (501) staff       (20)     1707 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_processor.py
--rw-r--r--   0 domen      (501) staff       (20)      826 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_microarray.py
--rw-r--r--   0 domen      (501) staff       (20)     3875 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_pca.py
--rw-r--r--   0 domen      (501) staff       (20)     9454 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_support_processors.py
--rw-r--r--   0 domen      (501) staff       (20)     7431 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_clustering.py
--rw-r--r--   0 domen      (501) staff       (20)     5280 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_diff_expression.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/
--rw-r--r--   0 domen      (501) staff       (20)     1078 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_wgbs.py
--rw-r--r--   0 domen      (501) staff       (20)     3070 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_amplicon.py
--rw-r--r--   0 domen      (501) staff       (20)     2035 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_chemut.py
--rw-r--r--   0 domen      (501) staff       (20)    15663 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_rna_seq.py
--rw-r--r--   0 domen      (501) staff       (20)       54 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     1925 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_mirna.py
--rw-r--r--   0 domen      (501) staff       (20)     1669 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_heat_seq.py
--rw-r--r--   0 domen      (501) staff       (20)      575 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_chip_seq.py
--rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/__init__.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/
--rw-r--r--   0 domen      (501) staff       (20)    17774 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)    25637 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bt2_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)       84 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/expression_htseq.json.gz
--rw-r--r--   0 domen      (501) staff       (20)   133746 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs14_control.bam
--rw-r--r--   0 domen      (501) staff       (20)   872689 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/HS chr21_ensembl.fa.gz
--rw-r--r--   0 domen      (501) staff       (20)   166778 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/expressions-py3.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     1296 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_filtering.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)       99 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_1_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      395 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_mem_paired_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      113 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gene_counts_star_single.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      371 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gene_cluster_data.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      147 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_mac_line_ending.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)    46099 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G_masterfile_corrupted.txt
--rw-r--r--   0 domen      (501) staff       (20)       62 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mate2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)       95 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/star_expression_paired.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      312 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ChIP-Seq-Control.bam.bai
--rwxr-xr-x   0 domen      (501) staff       (20)      127 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/annotation dicty.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)       81 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/matabolic pathway.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      116 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sp_test.fasta
--rw-r--r--   0 domen      (501) staff       (20)       65 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_bbduk_star_htseq_single_cpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      808 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/00Hr.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1280 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_fw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1218 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bed_track.bed
--rw-r--r--   0 domen      (501) staff       (20)      679 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem.fa.gz
--rw-r--r--   0 domen      (501) staff       (20)      971 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/s_1_2.qseq.small.txt.bz2
--rw-r--r--   0 domen      (501) staff       (20)      598 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     1010 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/features.tab
--rw-r--r--   0 domen      (501) staff       (20)      715 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_prinseq_single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      104 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_position_sorted.bam.bai
--rw-r--r--   0 domen      (501) staff       (20)   178819 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/silva-arc-23s-id98.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)      136 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_2_tpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      533 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_trimmomatic_single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      121 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/tophat_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      740 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_fastqmcf_single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    12121 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_sw_paired_reads_mapped.bam
--rw-r--r--   0 domen      (501) staff       (20)     2081 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1_transformed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    16062 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_expressions_1.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/4-cuffquant.cxb
--rw-r--r--   0 domen      (501) staff       (20)       97 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/feature_counts_out_fpkm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)   249709 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)     3538 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.gatkHC.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_mem_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      954 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot.bed
--rw-r--r--   0 domen      (501) staff       (20)     2644 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/fw reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1677 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/subread_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      411 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset-py3.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/3-cuffquant.cxb
--rwxr-xr-x   0 domen      (501) staff       (20)     6148 2018-01-25 16:29:21.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/.DS_Store
--rw-r--r--   0 domen      (501) staff       (20)     1248 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_wo_rRNA_paired_forw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      787 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sp_test.bam
--rw-r--r--   0 domen      (501) staff       (20)     3510 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56gsid_10k.targetPCRmetrics.txt
--rw-r--r--   0 domen      (501) staff       (20)     6309 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/s_1_1.qseq.small.txt.bz2
--rw-r--r--   0 domen      (501) staff       (20)      675 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_unmapped_1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      549 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/prepare_geo_RNA-Seq.txt
--rw-r--r--   0 domen      (501) staff       (20)      201 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/SRR2124780.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     7217 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/dbsnp_138.b37.chr2_small.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)      289 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/picard.perTargetCov.txt
--rw-r--r--   0 domen      (501) staff       (20)       66 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/feature_counts_out_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)    10773 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_master_file_olapfreebed.bed
--rw-r--r--   0 domen      (501) staff       (20)     5614 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ncRNA_sample2.bam
--rw-r--r--   0 domen      (501) staff       (20)      597 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/box_plot.json.gz
--rw-r--r--   0 domen      (501) staff       (20)    15991 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_expressions_3.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      756 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/paired_end_forward.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     3482 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Test_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)   249709 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      100 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/purpureum_ortholog-10-28-2014.cropped.txt.gz
--rwxr-xr-x   0 domen      (501) staff       (20)    13801 2017-12-26 13:22:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/subread_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)     5809 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/igv_human.lf.vcf
--rw-r--r--   0 domen      (501) staff       (20)       70 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_tpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      332 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/annotation_ok.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)      758 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      104 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads rsem2.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)    58288 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs14_case.bam
--rw-r--r--   0 domen      (501) staff       (20)   156292 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/expressions-py2.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      150 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_1_norm.json.gz
--rw-r--r--   0 domen      (501) staff       (20)    18459 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_paired_abyss_1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    15454 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_genes.txt
--rw-r--r--   0 domen      (501) staff       (20)      965 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding_transformed_R2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    14375 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G_masterfile_170113.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)    67499 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/SRR2124780_2 1k.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      230 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/peaks.bed
--rw-r--r--   0 domen      (501) staff       (20)      200 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/purpureum_mappability_50.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      618 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/features_update.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      195 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sp_test.gtf
--rw-r--r--   0 domen      (501) staff       (20)      201 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sample_cluster_data.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA forw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      694 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_bbduk_star test.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    31768 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot_ alignment1.bam
--rw-r--r--   0 domen      (501) staff       (20)     7653 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ncRNA_sample1.bam
--rw-r--r--   0 domen      (501) staff       (20)    11705 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rose2_enhancer_table.txt
--rw-r--r--   0 domen      (501) staff       (20)      158 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/clustering_NCBI_1.gz
--rw-r--r--   0 domen      (501) staff       (20)      243 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/annotation dicty.gff.gz
--rw-r--r--   0 domen      (501) staff       (20)     4082 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Mills_and_1000G_gold_standard.indels.b37.chr22_small.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)      175 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_single1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)       60 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_reads_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      218 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/clustering_expressions_2.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      201 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rsem_isoforms_paired.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      667 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/prepare_geo_ChIP-Seq.txt
--rw-r--r--   0 domen      (501) staff       (20)     1759 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L002_R1_001.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    71006 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k_mate2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      785 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk test reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      372 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gaf_dicty_cropped.gz
--rw-r--r--   0 domen      (501) staff       (20)     1268 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_wo_rRNA_paired_rew.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      261 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_custom_paired_reverse_trimmed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      170 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_custom_paired_forward_trimmed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    68516 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_trimmed_mate1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)       47 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.2.tsv
--rw-r--r--   0 domen      (501) staff       (20)      347 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/annotation_red.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)       60 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_ccshs.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     2680 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rw reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    65861 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/SRR2124780_1 1k.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      167 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_forward2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1338 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA_rew.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     2823 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.gatkHC4.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)     1190 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cufflinks_transcripts.gtf
--rw-r--r--   0 domen      (501) staff       (20)     6208 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_b37_chr22_frag.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)       65 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_bbduk_star_htseq_paired_cpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)   675378 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k_mate1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     4954 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_paired_R2 workflow_bbduk_star_htseq.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     3121 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    13355 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_hisat2_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)     9652 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_subread_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)      965 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding_transformed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    61934 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mouse_genes.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       43 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_2.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       39 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/venn.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      493 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_table_output_all.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      330 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/good.bed
--rw-r--r--   0 domen      (501) staff       (20)      339 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chemut.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)      144 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_single_trimmed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      459 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset-py3.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      125 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_ccsrp.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      392 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bsmap_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      395 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_sw_paired_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      668 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/deseq2_output.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      195 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rsem_genes_paired.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      357 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffnorm_genes.fpkm_table
--rw-r--r--   0 domen      (501) staff       (20)       20 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k_covMetrics.txt
--rw-r--r--   0 domen      (501) staff       (20)      482 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/dm6_header.sam
--rw-r--r--   0 domen      (501) staff       (20)      540 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_capture_targets.bed
--rw-r--r--   0 domen      (501) staff       (20)      548 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/deseq2_volcano_plot.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     1275 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_rw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)   426777 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_mate1_paired_filtered.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      290 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_rRNA_paired.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     2084 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      834 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mappings_gsea.tab.zip
--rw-r--r--   0 domen      (501) staff       (20)      124 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp.json.gz
--rw-r--r--   0 domen      (501) staff       (20)   331289 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/etc-py3.json.gz
--rw-r--r--   0 domen      (501) staff       (20)       94 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/wgbs.bam.HG.bed
--rw-r--r--   0 domen      (501) staff       (20)     1047 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_pseudoaligner.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      140 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/merged_expset_subset.tab
--rw-r--r--   0 domen      (501) staff       (20)      393 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_bt_paired_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      810 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/features_gsea.tab.zip
--rw-r--r--   0 domen      (501) staff       (20)      583 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G_masterfile_test.txt
--rw-r--r--   0 domen      (501) staff       (20)      201 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chip_seq.bed
--rw-r--r--   0 domen      (501) staff       (20)     2703 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/fw reads_2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1248 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_wo_rRNA_single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      630 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset-py2.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     2135 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1_R2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      302 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G masterfile_dup_amplicon_names.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)      574 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_paired_report.txt
--rw-r--r--   0 domen      (501) staff       (20)    18544 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffquant_1.cxb
--rw-r--r--   0 domen      (501) staff       (20)      357 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pca_plot.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     2176 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_dm6.bam.bai
--rw-r--r--   0 domen      (501) staff       (20)     2225 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_bwa_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)      315 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/deseq2.json.gz
--rw-r--r--   0 domen      (501) staff       (20)    62781 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_mm10.bam
--rw-r--r--   0 domen      (501) staff       (20)      128 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.tsv
--rw-r--r--   0 domen      (501) staff       (20)      108 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads rsem.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)    18727 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/dbsnp_138.b37.chr22_small.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)      458 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs annotation.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)      110 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_1.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     1004 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      241 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56gsid_10k.perTargetCov.txt
--rw-r--r--   0 domen      (501) staff       (20)   332826 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/etc-py2.json.gz
--rw-r--r--   0 domen      (501) staff       (20)       80 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/feature_counts_out_tpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      267 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID.gatkHC.finalvars.txt
--rw-r--r--   0 domen      (501) staff       (20)      308 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/merged_expset_all.tab
--rw-r--r--   0 domen      (501) staff       (20)      195 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_rRNA_single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      569 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_out.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     1004 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding_R2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1695 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/3ptrim_new56Gprimers.fa.gz
--rw-r--r--   0 domen      (501) staff       (20)      907 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot.gff
--rw-r--r--   0 domen      (501) staff       (20)    18544 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffquant_2.cxb
--rw-r--r--   0 domen      (501) staff       (20)     1004 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chemut_genome.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)      364 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs2_peakscore_genomicContext_old
--rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/seq_reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      191 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_report.txt
--rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA_forw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      139 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/wgbs.bam.G.bed
--rw-r--r--   0 domen      (501) staff       (20)      143 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_custom_single_trimmed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      280 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/diffexp_edgeR.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      842 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mm10_header.sam
--rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       43 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs14_peaks.bed
--rw-r--r--   0 domen      (501) staff       (20)      188 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bowtie_paired_reads_report.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       60 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mirna_featurecounts_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      108 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/etc.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_sw_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      299 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G masterfile_lowercase_bases.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)    10773 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_master_file_nomergebed.bed
--rw-r--r--   0 domen      (501) staff       (20)      116 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_unmapped.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      187 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/de_file_cuffdiff.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     3529 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Test_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    18501 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_paired_abyss_2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     5092 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.read3.small.qseq.bz2
--rw-r--r--   0 domen      (501) staff       (20)     3304 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)      153 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_windows_line_ending.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)       43 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_venn.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       87 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_matrix.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      399 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_trim_stats.txt
--rw-r--r--   0 domen      (501) staff       (20)     4375 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_paired_R1 workflow_bbduk_star_htseq.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1335 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_fw_reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1159 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_samtools.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)     1179 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_position_sorted.bam
--rw-r--r--   0 domen      (501) staff       (20)   126321 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_summary.html
--rw-r--r--   0 domen      (501) staff       (20)      102 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_3_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     1051 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_b37_chr2_small.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)     1677 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L002_R2_001.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      987 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/go_genesets.mgi.gz
--rw-r--r--   0 domen      (501) staff       (20)    19498 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_bt_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)       66 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/3_prime_adapter.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)       37 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/s_1.tsv
--rw-r--r--   0 domen      (501) staff       (20)      750 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.lf.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)   120260 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chr1_part.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)      939 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)       49 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chip_seq_geneScore.xls
--rw-r--r--   0 domen      (501) staff       (20)     1603 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/wgbs.bam_stat.txt
--rw-r--r--   0 domen      (501) staff       (20)     2167 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ontology_dicty_cropped.obo.gz
--rw-r--r--   0 domen      (501) staff       (20)       69 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mirna_featurecounts_fpkm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      113 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gene_counts_star_paired.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_rnaseq_single_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     1334 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_prinseq_paired_fw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      343 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pca_plot_ncbi.json.gz
--rw-r--r--   0 domen      (501) staff       (20)       65 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/auto_detect_strand_tpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      169 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      422 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_table_output.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      673 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_unmapped_2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      147 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_unix_line_ending.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)       44 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_mem_unmapped_reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     6656 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/etc_upload_input.xls
--rw-r--r--   0 domen      (501) staff       (20)       93 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k_ampmeancov.covd
--rw-r--r--   0 domen      (501) staff       (20)       95 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/star_expression_single.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       67 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_venn.json.gz
--rw-r--r--   0 domen      (501) staff       (20)   281732 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)       82 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_fpkm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      758 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/paired_end_reverse.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1183 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_name_sorted.bam
--rw-r--r--   0 domen      (501) staff       (20)    24100 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_probe_info.txt
--rw-r--r--   0 domen      (501) staff       (20)      916 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_filtered_variants.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)     1341 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/5ptrim_new56Gprimers.fa.gz
--rw-r--r--   0 domen      (501) staff       (20)      821 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mappings.tab.zip
--rw-r--r--   0 domen      (501) staff       (20)      104 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_bam_upload_index.bam.bai
--rw-r--r--   0 domen      (501) staff       (20)    10036 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_master_file_merged.bed
--rw-r--r--   0 domen      (501) staff       (20)      339 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/raw_cuffdiff.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)    63817 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/CM_mate1.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)   395673 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/seq_reads_fastqc.zip
--rw-r--r--   0 domen      (501) staff       (20)       80 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/expression_bcm_rpkm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      103 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_5_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      212 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sample_cluster_data_NCBI.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     2665 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/adapters.fasta
--rw-r--r--   0 domen      (501) staff       (20)     1554 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ontology_mus_cropped.obo.gz
--rw-r--r--   0 domen      (501) staff       (20)    12879 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Jbrowse_genome_coverage.bw
--rw-r--r--   0 domen      (501) staff       (20)    35359 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/AX4_mate1.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)      396 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/wgbs.bam
--rw-r--r--   0 domen      (501) staff       (20)     2044 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ncRNA_genome.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)   788254 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/silva-arc-16s-id95.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)     1417 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/demultiplexed_reads_rw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)       70 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_cpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     1275 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_rw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      231 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/edgeR.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      585 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/feature_counts_detect_strandedness.bam
--rw-r--r--   0 domen      (501) staff       (20)    31848 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffquant_mapping.bam
--rw-r--r--   0 domen      (501) staff       (20)      298 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/salmon_cds.fa.gz
--rw-r--r--   0 domen      (501) staff       (20)    51642 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_dm6.bam
--rw-r--r--   0 domen      (501) staff       (20)     2081 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1_transformed_R2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      460 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/HS chr21_short.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)      154 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/clustering_NCBI.gz
--rw-r--r--   0 domen      (501) staff       (20)   362869 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_mate1.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)   559048 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_aligment.bam
--rw-r--r--   0 domen      (501) staff       (20)   114556 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid.bam
--rw-r--r--   0 domen      (501) staff       (20)      112 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_genome.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)      375 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bad.bed
--rw-r--r--   0 domen      (501) staff       (20)      188 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bowtie_use_SE_report.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)    16021 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_expressions_2.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       60 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_bbduk_star_htseq_paired_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      475 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mappings_update.tab
--rw-r--r--   0 domen      (501) staff       (20)      767 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffmerge_transcripts.gtf
--rw-r--r--   0 domen      (501) staff       (20)      320 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_reverse.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)       62 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mate1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1143 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat-seq.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)   524296 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamliquidator_summary.html
--rw-r--r--   0 domen      (501) staff       (20)      528 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/go_enriched_terms_dicty.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     1776 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_mm10.bam.bai
--rw-r--r--   0 domen      (501) staff       (20)    14384 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs14_chr22.bed
--rw-r--r--   0 domen      (501) staff       (20)   328968 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chr21_small.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)      156 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt forward1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      621 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     1074 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mm10_small.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)      174 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/SRR1661332.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1111 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.read2.small.qseq.bz2
--rw-r--r--   0 domen      (501) staff       (20)      576 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset-py2.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      172 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_paired_forward_trimmed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      249 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_paired_reverse_trimmed.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1057 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_sw_reads_mapped.bam
--rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/6-cuffquant.cxb
--rwxr-xr-x   0 domen      (501) staff       (20)     1080 2017-12-26 13:22:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads.bam
--rw-r--r--   0 domen      (501) staff       (20)      239 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/diff_exp_check_types.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      414 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/go_enriched_terms_mouse.json.gz
--rw-r--r--   0 domen      (501) staff       (20)    13972 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_adapters.fasta
--rw-r--r--   0 domen      (501) staff       (20)      202 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ncRNA_annotation.gff.gz
--rw-r--r--   0 domen      (501) staff       (20)      168 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bowtie_single_reads_report.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      363 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chip_seq_peakscore_genomicContext
--rw-r--r--   0 domen      (501) staff       (20)       99 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_2_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       37 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_3.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      602 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/log_box_plot.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      192 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rsem_genes_single.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      259 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/annotation_rsem.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)     8396 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_probe_info.txt
--rw-r--r--   0 domen      (501) staff       (20)       85 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/test_etc.json.gz
--rw-r--r--   0 domen      (501) staff       (20)       73 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffquant_exp.tab
--rw-r--r--   0 domen      (501) staff       (20)       64 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_2.json.gz
--rw-r--r--   0 domen      (501) staff       (20)      266 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/diff_exp_check_geneid_type.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      197 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rsem_isoforms_single.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      284 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/tophat_paired_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)       56 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/upload_file.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)      394 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/subread_paired_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)       84 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/merged_etc.tab
--rw-r--r--   0 domen      (501) staff       (20)      412 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_coverage.bam
--rw-r--r--   0 domen      (501) staff       (20)    16827 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chip_seq_control.bam
--rw-r--r--   0 domen      (501) staff       (20)      783 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/20Hr.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1345 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_rv_reads.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1357 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_prinseq_paired_rw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      224 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/feature_locations.json.gz
--rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_rnaseq_paired_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)    24452 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_primers.bed
--rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_bt_reads_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      197 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/clustering_expressions_3.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     1596 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rose2_test.txt
--rw-r--r--   0 domen      (501) staff       (20)      645 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/HSQUtils_dedup_summary.txt
--rw-r--r--   0 domen      (501) staff       (20)     3357 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs genome.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)    10983 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chip_seq_case.bam
--rw-r--r--   0 domen      (501) staff       (20)    24934 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bt_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)      156 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/clustering_NCBI_2.gz
--rw-r--r--   0 domen      (501) staff       (20)     1273 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_fw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    31768 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot_alignment.bam
--rw-r--r--   0 domen      (501) staff       (20)    37060 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/AX4_mate2.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)       66 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/5_prime_adapter.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)      102 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_4_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      264 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ChIP-Seq-Case.bam.bai
--rw-r--r--   0 domen      (501) staff       (20)     1423 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.lf.vcf
--rw-r--r--   0 domen      (501) staff       (20)    66079 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/human_genes.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       83 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/merged_etc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      167 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffnorm_all_fpkm_means.txt
--rw-r--r--   0 domen      (501) staff       (20)     1177 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/demultiplexed_reads_fw.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     2135 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    36818 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/dicty_genes.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      135 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffnorm_expression.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       60 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_ccshp.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     3784 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/1000G_phase1.indels.b37_chr2_small.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)      939 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/my.strange.genome name$.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)      104 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_bam_upload_index.bai
--rw-r--r--   0 domen      (501) staff       (20)      787 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sp_test_compatibility_report.txt
--rw-r--r--   0 domen      (501) staff       (20)      538 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gff_to_gtf_annotation.gtf
--rw-r--r--   0 domen      (501) staff       (20)      343 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/igv_session_bam.xml
--rw-r--r--   0 domen      (501) staff       (20)    20746 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_bt2_index.tar.gz
--rw-r--r--   0 domen      (501) staff       (20)   427201 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_mate2_paired_filtered.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      212 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/clustering_expressions_1.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     3030 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/wgbs.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    61781 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/CM_mate2.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)     1383 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cDNA_reference.fasta.gz
--rw-r--r--   0 domen      (501) staff       (20)     1759 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    12223 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/feature_counts_paired.bam
--rw-r--r--   0 domen      (501) staff       (20)      479 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gaf_mgi_cropped.gz
--rw-r--r--   0 domen      (501) staff       (20)      210 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffdiff.json.gz
--rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/5-cuffquant.cxb
--rw-r--r--   0 domen      (501) staff       (20)      264 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gene_cluster_data_NCBI.json.gz
--rw-r--r--   0 domen      (501) staff       (20)    70093 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k_mate1.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     5696 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.read1.small.qseq.bz2
--rw-r--r--   0 domen      (501) staff       (20)      642 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Jbrowse_norm_genome_coverage.bw
--rw-r--r--   0 domen      (501) staff       (20)       65 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mirna_featurecounts_tpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     1315 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hg19_chr20_small.gtf.gz
--rw-r--r--   0 domen      (501) staff       (20)      135 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exp_1_tpm.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)      323 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bowtie2_paired_end_report.txt
--rw-r--r--   0 domen      (501) staff       (20)    69449 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_trimmed_mate2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)    19264 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_coverage.bw
--rw-r--r--   0 domen      (501) staff       (20)      294 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bowtie2_use_SE_report.txt
--rw-r--r--   0 domen      (501) staff       (20)   343439 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_mate2.fq.gz
--rw-r--r--   0 domen      (501) staff       (20)    17421 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_single bbduk_star_htseq_reads_single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      124 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_ccsrs.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)       61 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_bbduk_star_htseq_single_rc.tab.gz
--rw-r--r--   0 domen      (501) staff       (20)     6363 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/s_1_3.qseq.small.txt.bz2
--rw-r--r--   0 domen      (501) staff       (20)      116 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID.lf.finalvars.txt
--rw-r--r--   0 domen      (501) staff       (20)       58 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_3.json.gz
--rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA_forw_single.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)     2670 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rw reads_2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)   680291 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k_mate2.fastq.gz
--rw-r--r--   0 domen      (501) staff       (20)      557 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exons_coverage.txt.gz
--rw-r--r--   0 domen      (501) staff       (20)     2181 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/igv_human.lf.vcf.gz
--rw-r--r--   0 domen      (501) staff       (20)      281 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bowtie2_reads_report.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/commands/
--rw-r--r--   0 domen      (501) staff       (20)     8987 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/commands/test_generators.py
--rw-r--r--   0 domen      (501) staff       (20)       57 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/tests/commands/__init__.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/
--rw-r--r--   0 domen      (501) staff       (20)       25 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/__init__.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/
--rw-r--r--   0 domen      (501) staff       (20)     4461 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_geneset.py
--rw-r--r--   0 domen      (501) staff       (20)    10549 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_samples.py
--rw-r--r--   0 domen      (501) staff       (20)       34 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)    10771 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_diffexpr_deseq.py
--rw-r--r--   0 domen      (501) staff       (20)    11891 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_diffexpr_cuffdiff.py
--rw-r--r--   0 domen      (501) staff       (20)     5839 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/utils.py
--rw-r--r--   0 domen      (501) staff       (20)     4645 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_etc.py
--rw-r--r--   0 domen      (501) staff       (20)      188 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/__init__.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/resolwe_bio/utils/
--rw-r--r--   0 domen      (501) staff       (20)      202 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/utils/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     7423 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/utils/test.py
--rw-r--r--   0 domen      (501) staff       (20)      354 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/resolwe_bio/utils/filter.py
--rw-r--r--   0 domen      (501) staff       (20)      208 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/apps.py
--rw-r--r--   0 domen      (501) staff       (20)     1462 2018-04-09 16:06:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/extensions.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/
--rw-r--r--   0 domen      (501) staff       (20)     3013 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/bbduk-star-featurecounts.yml
--rw-r--r--   0 domen      (501) staff       (20)     3477 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/sample_detailed.yml
--rw-r--r--   0 domen      (501) staff       (20)     4176 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/sample_vaccinesurvey.yml
--rw-r--r--   0 domen      (501) staff       (20)      991 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/diffexp.yml
--rw-r--r--   0 domen      (501) staff       (20)      340 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/dicty.yml
--rw-r--r--   0 domen      (501) staff       (20)     2049 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/bcm.yml
--rw-r--r--   0 domen      (501) staff       (20)     2081 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/rnaseq.yml
--rw-r--r--   0 domen      (501) staff       (20)     6559 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/reads.yml
--rw-r--r--   0 domen      (501) staff       (20)      162 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/geneset.yml
--rw-r--r--   0 domen      (501) staff       (20)     1073 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/transmart.yml
--rw-r--r--   0 domen      (501) staff       (20)     5736 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/reads_detailed.yml
--rw-r--r--   0 domen      (501) staff       (20)     1891 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/amplicon.yml
--rw-r--r--   0 domen      (501) staff       (20)     3929 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/sample_geo.yml
--rw-r--r--   0 domen      (501) staff       (20)     2907 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/etc.yml
--rw-r--r--   0 domen      (501) staff       (20)      871 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/cutadapt-star-htseq.yml
--rw-r--r--   0 domen      (501) staff       (20)     3954 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/microarray_affy.yml
--rw-r--r--   0 domen      (501) staff       (20)     2202 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a3/resolwe_bio/descriptors/bbduk-star-htseq.yml
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/packages-manual/
--rw-r--r--   0 domen      (501) staff       (20)        0 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/packages-manual/.placeholder
--rw-r--r--   0 domen      (501) staff       (20)      251 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/Dockerfile
--rw-r--r--   0 domen      (501) staff       (20)      233 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/packages-debian.txt
--rw-r--r--   0 domen      (501) staff       (20)      226 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/packages-python3.txt
--rw-r--r--   0 domen      (501) staff       (20)      351 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/README.md
--rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/packages-debian-buildreq.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/assets/
--rw-r--r--   0 domen      (501) staff       (20)     5641 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/assets/logo_genialis.pdf
--rw-r--r--   0 domen      (501) staff       (20)     3929 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/assets/template_amplicon_report.tex
--rw-r--r--   0 domen      (501) staff       (20)     4995 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/assets/template_amplicon_report_multi_sample.tex
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/
--rw-r--r--   0 domen      (501) staff       (20)     1077 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/r-packages.sh
--rw-r--r--   0 domen      (501) staff       (20)      317 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/primerclip.sh
--rw-r--r--   0 domen      (501) staff       (20)      404 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/lofreq.sh
--rw-r--r--   0 domen      (501) staff       (20)      367 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/gatk.sh
--rw-r--r--   0 domen      (501) staff       (20)      460 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/bokeh-assets.sh
--rw-r--r--   0 domen      (501) staff       (20)      717 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/snpeff.sh
--rw-r--r--   0 domen      (501) staff       (20)       55 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/README.txt
--rw-r--r--   0 domen      (501) staff       (20)      441 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/samtools.sh
--rw-r--r--   0 domen      (501) staff       (20)      251 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/Dockerfile
--rw-r--r--   0 domen      (501) staff       (20)       84 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-debian.txt
--rw-r--r--   0 domen      (501) staff       (20)       63 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual.txt
--rw-r--r--   0 domen      (501) staff       (20)        9 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-r.txt
--rw-r--r--   0 domen      (501) staff       (20)     2107 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-python3.txt
--rw-r--r--   0 domen      (501) staff       (20)      470 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/README.md
--rw-r--r--   0 domen      (501) staff       (20)      290 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-debian-buildreq.txt
--rw-r--r--   0 domen      (501) staff       (20)       28 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-r-bioconductor.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/assets/
--rw-r--r--   0 domen      (501) staff       (20)      454 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/assets/amplicon_html_template.html
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/
--rw-r--r--   0 domen      (501) staff       (20)      149 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-python2-stage2.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/
--rw-r--r--   0 domen      (501) staff       (20)      919 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/jbrowse.sh
--rw-r--r--   0 domen      (501) staff       (20)      397 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/subread.sh
--rw-r--r--   0 domen      (501) staff       (20)      354 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/ea-utils.sh
--rw-r--r--   0 domen      (501) staff       (20)      382 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/sra-toolkit.sh
--rw-r--r--   0 domen      (501) staff       (20)     1567 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/r-packages.sh
--rw-r--r--   0 domen      (501) staff       (20)      311 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/primerclip.sh
--rw-r--r--   0 domen      (501) staff       (20)      333 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/gotea.sh
--rw-r--r--   0 domen      (501) staff       (20)      367 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/lofreq.sh
--rw-r--r--   0 domen      (501) staff       (20)      427 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/moabs.sh
--rw-r--r--   0 domen      (501) staff       (20)      321 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/bbmap.sh
--rw-r--r--   0 domen      (501) staff       (20)      749 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/snpeff.sh
--rw-r--r--   0 domen      (501) staff       (20)      521 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/hsqutils.sh
--rw-r--r--   0 domen      (501) staff       (20)      401 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/bedtools.sh
--rw-r--r--   0 domen      (501) staff       (20)      458 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/trans-decoder.sh
--rw-r--r--   0 domen      (501) staff       (20)      502 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/bcftools.sh
--rw-r--r--   0 domen      (501) staff       (20)      402 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/genome-tools.sh
--rw-r--r--   0 domen      (501) staff       (20)      356 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/fastqc.sh
--rw-r--r--   0 domen      (501) staff       (20)      449 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/hisat2.sh
--rw-r--r--   0 domen      (501) staff       (20)      443 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/samtools.sh
--rw-r--r--   0 domen      (501) staff       (20)      356 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/bedops.sh
--rw-r--r--   0 domen      (501) staff       (20)      471 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/kent-utils.sh
--rw-r--r--   0 domen      (501) staff       (20)      441 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/star.sh
--rw-r--r--   0 domen      (501) staff       (20)      387 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/cufflinks.sh
--rw-r--r--   0 domen      (501) staff       (20)      423 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/prinseq.sh
--rw-r--r--   0 domen      (501) staff       (20)      193 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/Dockerfile
--rw-r--r--   0 domen      (501) staff       (20)      609 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-debian.txt
--rw-r--r--   0 domen      (501) staff       (20)      209 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual.txt
--rw-r--r--   0 domen      (501) staff       (20)       47 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-r.txt
--rw-r--r--   0 domen      (501) staff       (20)     2579 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-python2.txt
--rw-r--r--   0 domen      (501) staff       (20)      319 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-python3.txt
--rw-r--r--   0 domen      (501) staff       (20)      280 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/README.md
--rw-r--r--   0 domen      (501) staff       (20)      380 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-debian-buildreq.txt
--rw-r--r--   0 domen      (501) staff       (20)      282 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-r-bioconductor.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-manual/
--rw-r--r--   0 domen      (501) staff       (20)     1092 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-manual/wigtobigwig.sh
--rw-r--r--   0 domen      (501) staff       (20)      241 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-manual/bamliquidator.sh
--rw-r--r--   0 domen      (501) staff       (20)      127 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/Dockerfile
--rw-r--r--   0 domen      (501) staff       (20)      479 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-debian.txt
--rw-r--r--   0 domen      (501) staff       (20)       26 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-manual.txt
--rw-r--r--   0 domen      (501) staff       (20)      677 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-python2.txt
--rw-r--r--   0 domen      (501) staff       (20)      372 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/README.md
--rw-r--r--   0 domen      (501) staff       (20)      112 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-debian-buildreq.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-manual/
--rw-r--r--   0 domen      (501) staff       (20)      657 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-manual/sra-toolkit.sh
--rw-r--r--   0 domen      (501) staff       (20)      383 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-manual/igvtools.sh
--rw-r--r--   0 domen      (501) staff       (20)      356 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-manual/fastqc.sh
--rw-r--r--   0 domen      (501) staff       (20)      127 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/Dockerfile
--rw-r--r--   0 domen      (501) staff       (20)       70 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-debian.txt
--rw-r--r--   0 domen      (501) staff       (20)       27 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-manual.txt
--rw-r--r--   0 domen      (501) staff       (20)     1122 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-python3.txt
--rw-r--r--   0 domen      (501) staff       (20)      284 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/README.md
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/
--rw-r--r--   0 domen      (501) staff       (20)      330 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/rsem.sh
--rw-r--r--   0 domen      (501) staff       (20)      397 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/subread.sh
--rw-r--r--   0 domen      (501) staff       (20)      644 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/trimmomatic.sh
--rw-r--r--   0 domen      (501) staff       (20)     1151 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/r-packages.sh
--rw-r--r--   0 domen      (501) staff       (20)      333 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/gotea.sh
--rw-r--r--   0 domen      (501) staff       (20)      321 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/bbmap.sh
--rw-r--r--   0 domen      (501) staff       (20)      421 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/salmon.sh
--rw-r--r--   0 domen      (501) staff       (20)      435 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/bedtools.sh
--rw-r--r--   0 domen      (501) staff       (20)      356 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/fastqc.sh
--rw-r--r--   0 domen      (501) staff       (20)      444 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/hisat2.sh
--rw-r--r--   0 domen      (501) staff       (20)      441 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/samtools.sh
--rw-r--r--   0 domen      (501) staff       (20)      441 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/star.sh
--rw-r--r--   0 domen      (501) staff       (20)      387 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/cufflinks.sh
--rw-r--r--   0 domen      (501) staff       (20)      127 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/Dockerfile
--rw-r--r--   0 domen      (501) staff       (20)      268 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-debian.txt
--rw-r--r--   0 domen      (501) staff       (20)      102 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual.txt
--rw-r--r--   0 domen      (501) staff       (20)       18 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-r.txt
--rw-r--r--   0 domen      (501) staff       (20)     1651 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-python3.txt
--rw-r--r--   0 domen      (501) staff       (20)      657 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/README.md
--rw-r--r--   0 domen      (501) staff       (20)      132 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-debian-buildreq.txt
--rw-r--r--   0 domen      (501) staff       (20)       46 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-r-bioconductor.txt
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/
--rw-r--r--   0 domen      (501) staff       (20)     3135 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-16.04
--rw-r--r--   0 domen      (501) staff       (20)     2484 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/common.sh
--rw-r--r--   0 domen      (501) staff       (20)     3135 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-17.10
--rw-r--r--   0 domen      (501) staff       (20)     3135 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-18.04
--rw-r--r--   0 domen      (501) staff       (20)      530 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/README.md
--rw-r--r--   0 domen      (501) staff       (20)     3135 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-14.04
--rw-r--r--   0 domen      (501) staff       (20)      788 2018-05-02 10:16:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/__about__.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/expression_filters/
--rw-r--r--   0 domen      (501) staff       (20)       68 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/expression_filters/__init__.py
--rw-r--r--   0 domen      (501) staff       (20)     1321 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/expression_filters/sample.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/resolwe_bio/fixtures/
--rw-r--r--   0 domen      (501) staff       (20)      248 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/fixtures/relationtypes.yaml
--rw-r--r--   0 domen      (501) staff       (20)     1455 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/resolwe_bio/filters.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/tests/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/tests/test_data/
--rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a3/tests/test_data/README.rst
--rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/tests/__init__.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/tests/test_runtime/
--rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a3/tests/test_runtime/README.rst
--rw-r--r--   0 domen      (501) staff       (20)      278 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a3/tests/routing.py
--rw-r--r--   0 domen      (501) staff       (20)      351 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/tests/.env
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/tests/test_upload/
--rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a3/tests/test_upload/README.rst
--rw-r--r--   0 domen      (501) staff       (20)     5970 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a3/tests/settings.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/tests/fixtures/
--rw-r--r--   0 domen      (501) staff       (20)     1668 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/tests/fixtures/data.yaml
--rw-r--r--   0 domen      (501) staff       (20)     1461 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/tests/fixtures/collection.yaml
--rw-r--r--   0 domen      (501) staff       (20)     1012 2018-03-28 20:35:19.000000 resolwe-bio-9.0.0a3/tests/docker-compose.yml
--rwxr-xr-x   0 domen      (501) staff       (20)      357 2018-03-07 07:28:32.000000 resolwe-bio-9.0.0a3/tests/manage.py
--rw-r--r--   0 domen      (501) staff       (20)     1616 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a3/tests/urls.py
--rw-r--r--   0 domen      (501) staff       (20)      655 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a3/MANIFEST.in
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/docs/
--rw-r--r--   0 domen      (501) staff       (20)      480 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/index.rst
--rw-r--r--   0 domen      (501) staff       (20)       78 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/catalog-definitions.rst
--rw-r--r--   0 domen      (501) staff       (20)      339 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/catalog.rst
--rw-r--r--   0 domen      (501) staff       (20)     7099 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/docs/contributing.rst
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/docs/_templates/
--rw-r--r--   0 domen      (501) staff       (20)      477 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/_templates/page.html
--rw-r--r--   0 domen      (501) staff       (20)     3113 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/conf.py
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/docs/_static/
-drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-02 10:17:55.000000 resolwe-bio-9.0.0a3/docs/_static/css/
--rw-r--r--   0 domen      (501) staff       (20)      244 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/_static/css/custom.css
--rw-r--r--   0 domen      (501) staff       (20)      985 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/proc.rst
--rw-r--r--   0 domen      (501) staff       (20)      651 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/catalog-types.rst
--rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/ref.rst
--rw-r--r--   0 domen      (501) staff       (20)       92 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/catalog-category.rst
--rw-r--r--   0 domen      (501) staff       (20)    33265 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a3/docs/CHANGELOG.rst
--rw-r--r--   0 domen      (501) staff       (20)     2645 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a3/docs/descriptor.rst
--rw-r--r--   0 domen      (501) staff       (20)     3224 2018-04-20 10:05:08.000000 resolwe-bio-9.0.0a3/setup.py
--rw-r--r--   0 domen      (501) staff       (20)     3551 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a3/tox.ini
--rw-r--r--   0 domen      (501) staff       (20)      275 2018-05-02 10:17:56.000000 resolwe-bio-9.0.0a3/setup.cfg
--rw-r--r--   0 domen      (501) staff       (20)     3716 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a3/README.rst
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/
+-rw-r--r--   0 domen      (501) staff       (20)     5690 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/PKG-INFO
+-rw-r--r--   0 domen      (501) staff       (20)    13070 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/.pylintrc
+-rw-r--r--   0 domen      (501) staff       (20)      575 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/.resolwebio-filetypes.yml
+-rw-r--r--   0 domen      (501) staff       (20)    11358 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/LICENSE
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio.egg-info/
+-rw-r--r--   0 domen      (501) staff       (20)     5690 2018-05-14 12:46:06.000000 resolwe-bio-9.0.0a4/resolwe_bio.egg-info/PKG-INFO
+-rw-r--r--   0 domen      (501) staff       (20)        1 2018-05-14 12:44:43.000000 resolwe-bio-9.0.0a4/resolwe_bio.egg-info/not-zip-safe
+-rw-r--r--   0 domen      (501) staff       (20)    40170 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio.egg-info/SOURCES.txt
+-rw-r--r--   0 domen      (501) staff       (20)      334 2018-05-14 12:46:06.000000 resolwe-bio-9.0.0a4/resolwe_bio.egg-info/requires.txt
+-rw-r--r--   0 domen      (501) staff       (20)       12 2018-05-14 12:46:06.000000 resolwe-bio-9.0.0a4/resolwe_bio.egg-info/top_level.txt
+-rw-r--r--   0 domen      (501) staff       (20)        1 2018-05-14 12:46:06.000000 resolwe-bio-9.0.0a4/resolwe_bio.egg-info/dependency_links.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/
+-rw-r--r--   0 domen      (501) staff       (20)      644 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0005_make_date_indexes.py
+-rw-r--r--   0 domen      (501) staff       (20)      535 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0010_add_relation_types.py
+-rw-r--r--   0 domen      (501) staff       (20)      478 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0006_alter_versionfield.py
+-rw-r--r--   0 domen      (501) staff       (20)      690 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0004_add_owner.py
+-rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     2343 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0008_migrate_sample.py
+-rw-r--r--   0 domen      (501) staff       (20)     1019 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0009_delete_sample.py
+-rw-r--r--   0 domen      (501) staff       (20)      466 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0007_sample_descriptor_dirty.py
+-rw-r--r--   0 domen      (501) staff       (20)     2401 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0001_initial.py
+-rw-r--r--   0 domen      (501) staff       (20)      444 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0002_sample_presample.py
+-rw-r--r--   0 domen      (501) staff       (20)      705 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/migrations/0003_fix_jsonfields.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/
+-rwxr-xr-x   0 domen      (501) staff       (20)      620 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/convert_DE_excel_table.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     5119 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/basespace_download.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2119 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/plot_enhancers.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      958 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_library_type.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2375 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/make_igv_session_archive.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      784 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/VCF_ad_extract.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     5180 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/xgff.py
+-rwxr-xr-x   0 domen      (501) staff       (20)    18708 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/make_multireport.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     9251 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/xexpression.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1328 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_star_expressions.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     3990 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/postprocess_snpeff.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      738 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/cufflinks_sample_groups.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     3185 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/transmart_fetch.R
+-rw-r--r--   0 domen      (501) staff       (20)     7149 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/transmart_utils.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     7460 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/samplehcluster.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2846 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/goea.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2976 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/lofreq2_indel_ovlp.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2099 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/expressionmerge.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1442 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/xgtf2gff.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      516 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/cuffnorm_group_labels.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1743 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/mergebowtiestats.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     3372 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/etc.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2414 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/rnaseq.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1631 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/peak2geneScore.R
+-rwxr-xr-x   0 domen      (501) staff       (20)     9964 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/demultiplex.py
+-rw-r--r--   0 domen      (501) staff       (20)     6612 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/clustering_leaf_ordering.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1052 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/run_edger.R
+-rwxr-xr-x   0 domen      (501) staff       (20)     1392 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/format_index_files.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1543 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/deseq.R
+-rwxr-xr-x   0 domen      (501) staff       (20)    10893 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/garvan_coverage.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1076 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/make_igv_session.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      611 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/diffexp_filtering.R
+-rwxr-xr-x   0 domen      (501) staff       (20)     6446 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/expression_aggregator.py
+-rw-r--r--   0 domen      (501) staff       (20)      213 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/utils.py
+-rwxr-xr-x   0 domen      (501) staff       (20)    12266 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/make_report.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2071 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/expressionmerge_archive.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     3844 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/mappability.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2641 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_diffexp.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1152 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/geneset2storage.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     4616 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/pca.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     7835 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/genehcluster.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2124 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/find_similar.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     3877 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/plotcoverage_html.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     3434 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/transmart_import.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1632 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/detect_strandedness.sh
+-rwxr-xr-x   0 domen      (501) staff       (20)      672 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/fastqc.sh
+-rwxr-xr-x   0 domen      (501) staff       (20)     3642 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/compatibilty_check.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1718 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/mergeetc.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2263 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/expression_fpkm_tpm.R
+-rwxr-xr-x   0 domen      (501) staff       (20)     1070 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_cuffnorm.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1921 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/mergebowtie2stats_paired.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      651 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/add_header.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2341 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_closest_features.R
+-rwxr-xr-x   0 domen      (501) staff       (20)     1609 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/importETC.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      674 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_encoding_type.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     2671 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/volcanoplot.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1606 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/mergebowtie2stats.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     3082 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/feature_location.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      574 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/unique_sample_names.py
+-rwxr-xr-x   0 domen      (501) staff       (20)      996 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/microarrayQC.R
+-rwxr-xr-x   0 domen      (501) staff       (20)     1003 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/bamliquidator_table.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1591 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/go_genesets.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1952 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/cuffnorm_output_table_headers.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     6776 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/xtabcoverage.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     6168 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/make_amplicon_table.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1425 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/gff3_to_gtf.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1524 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/validate_master_file.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1255 2017-12-26 13:22:49.000000 resolwe-bio-9.0.0a4/resolwe_bio/tools/expression2storage.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/
+-rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)      482 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0003_add_map_index.py
+-rw-r--r--   0 domen      (501) staff       (20)     1139 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0002_alter_field_max_length.py
+-rw-r--r--   0 domen      (501) staff       (20)     2273 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0001_initial.py
+-rw-r--r--   0 domen      (501) staff       (20)      477 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0004_add_unique_together.py
+-rw-r--r--   0 domen      (501) staff       (20)     2230 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0005_species.py
+-rw-r--r--   0 domen      (501) staff       (20)     4114 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/models.py
+-rw-r--r--   0 domen      (501) staff       (20)      731 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/serializers.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/
+-rw-r--r--   0 domen      (501) staff       (20)    10892 2018-04-04 14:30:41.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/test_feature.py
+-rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     1265 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/test_import_kb.py
+-rw-r--r--   0 domen      (501) staff       (20)     6051 2018-04-04 14:30:41.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/test_mapping.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/management/
+-rw-r--r--   0 domen      (501) staff       (20)       25 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/management/__init__.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/
+-rw-r--r--   0 domen      (501) staff       (20)     4918 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/insert_features.py
+-rw-r--r--   0 domen      (501) staff       (20)       34 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     1620 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/utils.py
+-rw-r--r--   0 domen      (501) staff       (20)     5038 2018-03-28 13:06:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/insert_mappings.py
+-rw-r--r--   0 domen      (501) staff       (20)      245 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)      355 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/apps.py
+-rw-r--r--   0 domen      (501) staff       (20)      525 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/admin.py
+-rw-r--r--   0 domen      (501) staff       (20)     3815 2018-03-28 20:35:19.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/elastic_indexes.py
+-rw-r--r--   0 domen      (501) staff       (20)      770 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/filters.py
+-rw-r--r--   0 domen      (501) staff       (20)     7352 2018-04-04 14:30:41.000000 resolwe-bio-9.0.0a4/resolwe_bio/kb/views.py
+-rw-r--r--   0 domen      (501) staff       (20)      134 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/models.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/transmart/
+-rw-r--r--   0 domen      (501) staff       (20)     2014 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/transmart/import.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/go_enrichment/
+-rw-r--r--   0 domen      (501) staff       (20)     2893 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/go_enrichment/go.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/
+-rw-r--r--   0 domen      (501) staff       (20)     5018 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/edgeR.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4554 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/deseq.yml
+-rw-r--r--   0 domen      (501) staff       (20)     9429 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/cuffdiff.yml
+-rw-r--r--   0 domen      (501) staff       (20)      870 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/abstract.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/
+-rw-r--r--   0 domen      (501) staff       (20)      904 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_list.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1306 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_hidden_fields.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1117 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_disabled_fields.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6955 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_basic_fields.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1061 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_sleep_progress.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/amplicon/
+-rw-r--r--   0 domen      (501) staff       (20)     1748 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/amplicon/amplicon_table.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2010 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/amplicon/target_metrics.yml
+-rw-r--r--   0 domen      (501) staff       (20)     7402 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/amplicon/bwa_trim.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/assembly/
+-rw-r--r--   0 domen      (501) staff       (20)     4276 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/assembly/abyss.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/clustering/
+-rw-r--r--   0 domen      (501) staff       (20)     4060 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/clustering/pca.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1244 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/clustering/find_similar.yml
+-rw-r--r--   0 domen      (501) staff       (20)    12221 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/clustering/hierarchical_clustering.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/
+-rw-r--r--   0 domen      (501) staff       (20)    41865 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/bbduk_star_featurecounts.yml
+-rw-r--r--   0 domen      (501) staff       (20)    23046 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/cutadapt_star_htseq.yml
+-rw-r--r--   0 domen      (501) staff       (20)    10532 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/rnaseq.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1273 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/wgbs.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1682 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/heat_seq.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5340 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/bbduk_star_htseq.yml
+-rw-r--r--   0 domen      (501) staff       (20)    13388 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/amplicon.yml
+-rw-r--r--   0 domen      (501) staff       (20)      809 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/cuffquant.yml
+-rw-r--r--   0 domen      (501) staff       (20)    19834 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/cutadapt_star_rsem.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2279 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/mirna.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5787 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/chemut.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1085 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/chip_seq.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/
+-rw-r--r--   0 domen      (501) staff       (20)     2563 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/nucleotide_seq.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6870 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/geneset.yml
+-rw-r--r--   0 domen      (501) staff       (20)     3798 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/master_file.yml
+-rw-r--r--   0 domen      (501) staff       (20)     7124 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/genome.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1913 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/go_gaf.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4675 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/annotation.yml
+-rw-r--r--   0 domen      (501) staff       (20)      896 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/sam_header.yml
+-rw-r--r--   0 domen      (501) staff       (20)    12787 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/expressions.yml
+-rw-r--r--   0 domen      (501) staff       (20)     9629 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/sra_file.yml
+-rw-r--r--   0 domen      (501) staff       (20)      921 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/variants_bed.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5810 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/differential_exp.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1126 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/etc.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1156 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/basespace.yml
+-rw-r--r--   0 domen      (501) staff       (20)      441 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/abstract_bed.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2720 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/cuffquant.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1382 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/snpeff.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1294 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/target_pcr_metrics.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2047 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/variants_vcf.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1418 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/pathway_map.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1280 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/hmmer_database.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1138 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/go_obo.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1081 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/mappability_bigwig.yml
+-rw-r--r--   0 domen      (501) staff       (20)      970 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/mappability_tab.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1966 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/annotation_bed.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6018 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/seq_reads_multiplexed.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6775 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/bam.yml
+-rw-r--r--   0 domen      (501) staff       (20)    14786 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/seq_reads.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1059 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/microarray_affy.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/annotation/
+-rw-r--r--   0 domen      (501) staff       (20)     4393 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/annotation/cuffmerge.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2558 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/annotation/feature_location.yml
+-rw-r--r--   0 domen      (501) staff       (20)      543 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/annotation/abstract.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/WGBS/
+-rw-r--r--   0 domen      (501) staff       (20)     3873 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/WGBS/mcall.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4050 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/WGBS/bsmap.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/
+-rw-r--r--   0 domen      (501) staff       (20)     3543 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/macs14.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2594 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/scoring.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4225 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/rose2.yml
+-rw-r--r--   0 domen      (501) staff       (20)    13606 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/macs2.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/microarray/
+-rw-r--r--   0 domen      (501) staff       (20)     1871 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/microarray/microarray_qc.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/
+-rw-r--r--   0 domen      (501) staff       (20)    24667 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/star.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5071 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/hisat2.yml
+-rw-r--r--   0 domen      (501) staff       (20)    10716 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/tophat.yml
+-rw-r--r--   0 domen      (501) staff       (20)    24280 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/bowtie.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6237 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/subread.yml
+-rw-r--r--   0 domen      (501) staff       (20)    16172 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/bwa.yml
+-rw-r--r--   0 domen      (501) staff       (20)      536 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/abstract.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/genome_browser/
+-rw-r--r--   0 domen      (501) staff       (20)     1598 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/genome_browser/igv_bam.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/
+-rw-r--r--   0 domen      (501) staff       (20)    26014 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/featureCounts.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5357 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/dicty_bcm.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1616 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/merge_expressions.yml
+-rw-r--r--   0 domen      (501) staff       (20)    14353 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/htseq_count.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1143 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/merge_etc.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4250 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/index_fasta_nucl.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1030 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/etc.yml
+-rw-r--r--   0 domen      (501) staff       (20)     8276 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/cuffnorm.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4546 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/cuffquant.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2486 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/mappability.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4240 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/rsem.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2746 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/salmon_index.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2687 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/expression_aggregator.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6271 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/cufflinks.yml
+-rw-r--r--   0 domen      (501) staff       (20)      860 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/abstract.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/exome_coverage/
+-rw-r--r--   0 domen      (501) staff       (20)     2445 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/exome_coverage/coverage_report.yml
+-rw-r--r--   0 domen      (501) staff       (20)     3751 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/exome_coverage/coveragebed.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/
+-rw-r--r--   0 domen      (501) staff       (20)     2913 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/hsqutils.yml
+-rw-r--r--   0 domen      (501) staff       (20)    45518 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/bbduk.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2647 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/merge_to_paired_end.yml
+-rw-r--r--   0 domen      (501) staff       (20)    17803 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/cutadapt.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6168 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/cutadapt_amplicon.yml
+-rw-r--r--   0 domen      (501) staff       (20)     8614 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/prinseq_lite.yml
+-rw-r--r--   0 domen      (501) staff       (20)    10039 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/fastq_mcf.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5884 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/cutadapt_custom.yml
+-rw-r--r--   0 domen      (501) staff       (20)    10557 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/sortmerna.yml
+-rw-r--r--   0 domen      (501) staff       (20)    28004 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/trimmomatic.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/
+-rw-r--r--   0 domen      (501) staff       (20)     3657 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/preprocess_bam.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5784 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/gatk.yml
+-rw-r--r--   0 domen      (501) staff       (20)    11783 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/vc_chemut.yml
+-rw-r--r--   0 domen      (501) staff       (20)     3547 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/samtools.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5871 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/filtering_chemut.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2689 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/snpeff.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2388 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/hsqutils-dedup.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2304 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/lofreq.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/plots/
+-rw-r--r--   0 domen      (501) staff       (20)     6877 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/plots/bamplot.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6700 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/plots/bamliquidator.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reports/
+-rw-r--r--   0 domen      (501) staff       (20)     3272 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reports/amplicon_report.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4363 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/reports/amplicon_multi_report.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/
+-rw-r--r--   0 domen      (501) staff       (20)     1243 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/annotation_gtf.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1254 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/annotation_gff3.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1238 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/refseq.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1465 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/bam_coverage.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2012 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/annotation_bed.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4175 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/bam_coverage_normalized.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/
+-rw-r--r--   0 domen      (501) staff       (20)     1257 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/gff_to_gtf.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4407 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/bam_split.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1619 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/refseq_compatibility.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1295 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/bam_coverage.yml
+-rw-r--r--   0 domen      (501) staff       (20)    10427 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/prepare_geo.yml
+-rw-r--r--   0 domen      (501) staff       (20)     3410 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/library_strandedness.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4106 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/archive.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/unit/
+-rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/unit/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     3768 2018-04-09 16:06:55.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/unit/test_api.py
+-rw-r--r--   0 domen      (501) staff       (20)      706 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/unit/test_tools.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/
+-rw-r--r--   0 domen      (501) staff       (20)     1118 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_genome_browser.py
+-rwxr-xr-x   0 domen      (501) staff       (20)     1723 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_wgbs.py
+-rw-r--r--   0 domen      (501) staff       (20)    18699 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_reads_filtering.py
+-rw-r--r--   0 domen      (501) staff       (20)     4370 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_plots.py
+-rw-r--r--   0 domen      (501) staff       (20)     3150 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_coverage.py
+-rw-r--r--   0 domen      (501) staff       (20)     2929 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_amplicon.py
+-rw-r--r--   0 domen      (501) staff       (20)     2745 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_demultiplex.py
+-rw-r--r--   0 domen      (501) staff       (20)    19153 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_expression.py
+-rw-r--r--   0 domen      (501) staff       (20)     5207 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_generate_report.py
+-rw-r--r--   0 domen      (501) staff       (20)     2394 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_expression_aggregator.py
+-rw-r--r--   0 domen      (501) staff       (20)     1457 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_reads_manipulation.py
+-rw-r--r--   0 domen      (501) staff       (20)       57 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     4883 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_files_to_reads.py
+-rw-r--r--   0 domen      (501) staff       (20)      895 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_genome_coverage.py
+-rw-r--r--   0 domen      (501) staff       (20)    11749 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_transmart.py
+-rw-r--r--   0 domen      (501) staff       (20)    14408 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_alignment.py
+-rw-r--r--   0 domen      (501) staff       (20)     2650 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_import.py
+-rw-r--r--   0 domen      (501) staff       (20)     4045 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_jbrowse.py
+-rw-r--r--   0 domen      (501) staff       (20)    17969 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_upload.py
+-rw-r--r--   0 domen      (501) staff       (20)     1057 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_assembler.py
+-rw-r--r--   0 domen      (501) staff       (20)      711 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_pathway_map.py
+-rw-r--r--   0 domen      (501) staff       (20)    12246 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_variant_calling.py
+-rw-r--r--   0 domen      (501) staff       (20)     4105 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_chipseq.py
+-rw-r--r--   0 domen      (501) staff       (20)     2126 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_enrichment.py
+-rw-r--r--   0 domen      (501) staff       (20)     1707 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_processor.py
+-rw-r--r--   0 domen      (501) staff       (20)      826 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_microarray.py
+-rw-r--r--   0 domen      (501) staff       (20)     3875 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_pca.py
+-rw-r--r--   0 domen      (501) staff       (20)     9454 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_support_processors.py
+-rw-r--r--   0 domen      (501) staff       (20)     7431 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_clustering.py
+-rw-r--r--   0 domen      (501) staff       (20)     5280 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_diff_expression.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/
+-rw-r--r--   0 domen      (501) staff       (20)     1078 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_wgbs.py
+-rw-r--r--   0 domen      (501) staff       (20)     3070 2018-04-20 07:57:31.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_amplicon.py
+-rw-r--r--   0 domen      (501) staff       (20)     2035 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_chemut.py
+-rw-r--r--   0 domen      (501) staff       (20)    15663 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_rna_seq.py
+-rw-r--r--   0 domen      (501) staff       (20)       54 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     1925 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_mirna.py
+-rw-r--r--   0 domen      (501) staff       (20)     1669 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_heat_seq.py
+-rw-r--r--   0 domen      (501) staff       (20)      575 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_chip_seq.py
+-rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/__init__.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/
+-rw-r--r--   0 domen      (501) staff       (20)    17774 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)    25637 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bt2_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)       84 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/expression_htseq.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)   133746 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs14_control.bam
+-rw-r--r--   0 domen      (501) staff       (20)   872689 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/HS chr21_ensembl.fa.gz
+-rw-r--r--   0 domen      (501) staff       (20)   166778 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/expressions-py3.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1296 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_filtering.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)       99 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_1_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      395 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_mem_paired_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      113 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gene_counts_star_single.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      371 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gene_cluster_data.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      147 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_mac_line_ending.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)    46099 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G_masterfile_corrupted.txt
+-rw-r--r--   0 domen      (501) staff       (20)       62 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mate2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)       95 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/star_expression_paired.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      312 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ChIP-Seq-Control.bam.bai
+-rwxr-xr-x   0 domen      (501) staff       (20)      127 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/annotation dicty.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)       81 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/matabolic pathway.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      116 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sp_test.fasta
+-rw-r--r--   0 domen      (501) staff       (20)       65 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_bbduk_star_htseq_single_cpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      808 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/00Hr.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1280 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_fw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1218 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bed_track.bed
+-rw-r--r--   0 domen      (501) staff       (20)      679 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem.fa.gz
+-rw-r--r--   0 domen      (501) staff       (20)      971 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/s_1_2.qseq.small.txt.bz2
+-rw-r--r--   0 domen      (501) staff       (20)      598 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1010 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/features.tab
+-rw-r--r--   0 domen      (501) staff       (20)      715 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_prinseq_single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      104 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_position_sorted.bam.bai
+-rw-r--r--   0 domen      (501) staff       (20)   178819 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/silva-arc-23s-id98.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)      136 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_2_tpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      533 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_trimmomatic_single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      121 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/tophat_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      740 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_fastqmcf_single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    12121 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_sw_paired_reads_mapped.bam
+-rw-r--r--   0 domen      (501) staff       (20)     2081 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1_transformed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    16062 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_expressions_1.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/4-cuffquant.cxb
+-rw-r--r--   0 domen      (501) staff       (20)      199 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_counts_out_fpkm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)   249709 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     3538 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.gatkHC.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_mem_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      954 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot.bed
+-rw-r--r--   0 domen      (501) staff       (20)     2644 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/fw reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1677 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L001_R2_001.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/subread_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      411 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset-py3.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/3-cuffquant.cxb
+-rwxr-xr-x   0 domen      (501) staff       (20)     6148 2018-01-25 16:29:21.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/.DS_Store
+-rw-r--r--   0 domen      (501) staff       (20)     1248 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_wo_rRNA_paired_forw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      787 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sp_test.bam
+-rw-r--r--   0 domen      (501) staff       (20)     3510 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56gsid_10k.targetPCRmetrics.txt
+-rw-r--r--   0 domen      (501) staff       (20)     6309 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/s_1_1.qseq.small.txt.bz2
+-rw-r--r--   0 domen      (501) staff       (20)      675 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_unmapped_1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      549 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/prepare_geo_RNA-Seq.txt
+-rw-r--r--   0 domen      (501) staff       (20)      201 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/SRR2124780.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     7217 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/dbsnp_138.b37.chr2_small.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      289 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/picard.perTargetCov.txt
+-rw-r--r--   0 domen      (501) staff       (20)      162 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_counts_out_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)    10773 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_master_file_olapfreebed.bed
+-rw-r--r--   0 domen      (501) staff       (20)     5614 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ncRNA_sample2.bam
+-rw-r--r--   0 domen      (501) staff       (20)      597 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/box_plot.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)    15991 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_expressions_3.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      756 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/paired_end_forward.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     3482 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Test_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)   249709 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      100 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/purpureum_ortholog-10-28-2014.cropped.txt.gz
+-rwxr-xr-x   0 domen      (501) staff       (20)    13801 2017-12-26 13:22:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/subread_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)     5809 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/igv_human.lf.vcf
+-rw-r--r--   0 domen      (501) staff       (20)       70 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_tpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      332 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/annotation_ok.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      758 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      104 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads rsem2.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    58288 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs14_case.bam
+-rw-r--r--   0 domen      (501) staff       (20)   156292 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/expressions-py2.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      150 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_1_norm.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)    18459 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_paired_abyss_1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    15454 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_genes.txt
+-rw-r--r--   0 domen      (501) staff       (20)      965 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding_transformed_R2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    14375 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G_masterfile_170113.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)    67499 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/SRR2124780_2 1k.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      230 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/peaks.bed
+-rw-r--r--   0 domen      (501) staff       (20)      200 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/purpureum_mappability_50.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      618 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/features_update.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      195 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sp_test.gtf
+-rw-r--r--   0 domen      (501) staff       (20)      201 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sample_cluster_data.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA forw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      694 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_bbduk_star test.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    31768 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot_ alignment1.bam
+-rw-r--r--   0 domen      (501) staff       (20)     7653 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ncRNA_sample1.bam
+-rw-r--r--   0 domen      (501) staff       (20)    11705 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rose2_enhancer_table.txt
+-rw-r--r--   0 domen      (501) staff       (20)      158 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/clustering_NCBI_1.gz
+-rw-r--r--   0 domen      (501) staff       (20)      243 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/annotation dicty.gff.gz
+-rw-r--r--   0 domen      (501) staff       (20)     4082 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Mills_and_1000G_gold_standard.indels.b37.chr22_small.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      175 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_single1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)       60 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_reads_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      218 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/clustering_expressions_2.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      201 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rsem_isoforms_paired.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      667 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/prepare_geo_ChIP-Seq.txt
+-rw-r--r--   0 domen      (501) staff       (20)     1759 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L002_R1_001.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    71006 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k_mate2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      785 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk test reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      372 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gaf_dicty_cropped.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1268 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_wo_rRNA_paired_rew.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      261 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_custom_paired_reverse_trimmed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      170 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_custom_paired_forward_trimmed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    68516 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_trimmed_mate1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)       47 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.2.tsv
+-rw-r--r--   0 domen      (501) staff       (20)      347 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/annotation_red.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)       60 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_ccshs.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2680 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rw reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    65861 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/SRR2124780_1 1k.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      167 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_forward2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1338 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA_rew.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2823 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.gatkHC4.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1190 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cufflinks_transcripts.gtf
+-rw-r--r--   0 domen      (501) staff       (20)     6208 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_b37_chr22_frag.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)       65 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_bbduk_star_htseq_paired_cpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)   675378 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k_mate1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     4954 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_paired_R2 workflow_bbduk_star_htseq.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     3121 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    13355 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_hisat2_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)     9652 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_subread_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)      965 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding_transformed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    61934 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mouse_genes.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       43 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_2.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       39 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/venn.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      493 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_table_output_all.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      330 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/good.bed
+-rw-r--r--   0 domen      (501) staff       (20)      339 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chemut.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      144 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_single_trimmed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      459 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset-py3.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      125 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_ccsrp.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      392 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bsmap_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      395 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_sw_paired_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      668 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/deseq2_output.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      195 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rsem_genes_paired.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      357 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffnorm_genes.fpkm_table
+-rw-r--r--   0 domen      (501) staff       (20)       20 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k_covMetrics.txt
+-rw-r--r--   0 domen      (501) staff       (20)      482 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/dm6_header.sam
+-rw-r--r--   0 domen      (501) staff       (20)      540 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_capture_targets.bed
+-rw-r--r--   0 domen      (501) staff       (20)      548 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/deseq2_volcano_plot.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1275 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_rw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)   426777 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_mate1_paired_filtered.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      290 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_rRNA_paired.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2084 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      834 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mappings_gsea.tab.zip
+-rw-r--r--   0 domen      (501) staff       (20)      124 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)   331289 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/etc-py3.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)       94 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/wgbs.bam.HG.bed
+-rw-r--r--   0 domen      (501) staff       (20)     1047 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_pseudoaligner.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      140 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/merged_expset_subset.tab
+-rw-r--r--   0 domen      (501) staff       (20)      393 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_bt_paired_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      810 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/features_gsea.tab.zip
+-rw-r--r--   0 domen      (501) staff       (20)      583 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G_masterfile_test.txt
+-rw-r--r--   0 domen      (501) staff       (20)      201 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chip_seq.bed
+-rw-r--r--   0 domen      (501) staff       (20)     2703 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/fw reads_2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1248 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_wo_rRNA_single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      630 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset-py2.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2135 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1_R2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      302 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G masterfile_dup_amplicon_names.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)      574 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_paired_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)    18544 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffquant_1.cxb
+-rw-r--r--   0 domen      (501) staff       (20)      357 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pca_plot.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2176 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_dm6.bam.bai
+-rw-r--r--   0 domen      (501) staff       (20)     2225 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_bwa_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)      315 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/deseq2.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)    62781 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_mm10.bam
+-rw-r--r--   0 domen      (501) staff       (20)      128 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.tsv
+-rw-r--r--   0 domen      (501) staff       (20)      108 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads rsem.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    18727 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/dbsnp_138.b37.chr22_small.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      458 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs annotation.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      110 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_1.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1004 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      241 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56gsid_10k.perTargetCov.txt
+-rw-r--r--   0 domen      (501) staff       (20)   332826 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/etc-py2.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      198 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_counts_out_tpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      267 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID.gatkHC.finalvars.txt
+-rw-r--r--   0 domen      (501) staff       (20)      308 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/merged_expset_all.tab
+-rw-r--r--   0 domen      (501) staff       (20)      195 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_rRNA_single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      569 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_out.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1004 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding_R2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    23506 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_counts hs.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1695 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/3ptrim_new56Gprimers.fa.gz
+-rw-r--r--   0 domen      (501) staff       (20)      907 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot.gff
+-rw-r--r--   0 domen      (501) staff       (20)    18544 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffquant_2.cxb
+-rw-r--r--   0 domen      (501) staff       (20)     1004 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chemut_genome.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)      364 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs2_peakscore_genomicContext_old
+-rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/seq_reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      191 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA_forw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      139 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/wgbs.bam.G.bed
+-rw-r--r--   0 domen      (501) staff       (20)      143 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_custom_single_trimmed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      280 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/diffexp_edgeR.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      842 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mm10_header.sam
+-rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       43 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs14_peaks.bed
+-rw-r--r--   0 domen      (501) staff       (20)      188 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bowtie_paired_reads_report.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       60 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mirna_featurecounts_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      108 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/etc.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_sw_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      299 2018-05-02 10:15:25.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G masterfile_lowercase_bases.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)    10773 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_master_file_nomergebed.bed
+-rw-r--r--   0 domen      (501) staff       (20)      116 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_unmapped.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      187 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/de_file_cuffdiff.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     3529 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Test_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    18501 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_paired_abyss_2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     5092 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.read3.small.qseq.bz2
+-rw-r--r--   0 domen      (501) staff       (20)     3304 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)      153 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_windows_line_ending.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)       43 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_venn.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       87 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_matrix.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      399 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_trim_stats.txt
+-rw-r--r--   0 domen      (501) staff       (20)     4375 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_paired_R1 workflow_bbduk_star_htseq.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1335 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_fw_reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1159 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_samtools.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1179 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_position_sorted.bam
+-rw-r--r--   0 domen      (501) staff       (20)   126321 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_summary.html
+-rw-r--r--   0 domen      (501) staff       (20)      102 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_3_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1051 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_b37_chr2_small.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1677 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L002_R2_001.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      987 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/go_genesets.mgi.gz
+-rw-r--r--   0 domen      (501) staff       (20)    19498 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_bt_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)       66 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/3_prime_adapter.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)       37 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/s_1.tsv
+-rw-r--r--   0 domen      (501) staff       (20)      750 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.lf.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)   120260 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chr1_part.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)      939 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)       49 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chip_seq_geneScore.xls
+-rw-r--r--   0 domen      (501) staff       (20)     1603 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/wgbs.bam_stat.txt
+-rw-r--r--   0 domen      (501) staff       (20)     2167 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ontology_dicty_cropped.obo.gz
+-rw-r--r--   0 domen      (501) staff       (20)       69 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mirna_featurecounts_fpkm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      396 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID.gatk.finalvars.txt
+-rw-r--r--   0 domen      (501) staff       (20)      113 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gene_counts_star_paired.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_rnaseq_single_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1334 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_prinseq_paired_fw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      343 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pca_plot_ncbi.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)       65 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/auto_detect_strand_tpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      169 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      422 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_table_output.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      673 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_unmapped_2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      147 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_unix_line_ending.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)       44 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_mem_unmapped_reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     6656 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/etc_upload_input.xls
+-rw-r--r--   0 domen      (501) staff       (20)       93 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k_ampmeancov.covd
+-rw-r--r--   0 domen      (501) staff       (20)       95 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/star_expression_single.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       67 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_venn.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)   281732 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)       82 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_fpkm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      758 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/paired_end_reverse.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1183 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_name_sorted.bam
+-rw-r--r--   0 domen      (501) staff       (20)    24100 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_probe_info.txt
+-rw-r--r--   0 domen      (501) staff       (20)      916 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_filtered_variants.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1341 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/5ptrim_new56Gprimers.fa.gz
+-rw-r--r--   0 domen      (501) staff       (20)      821 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mappings.tab.zip
+-rw-r--r--   0 domen      (501) staff       (20)      104 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_bam_upload_index.bam.bai
+-rw-r--r--   0 domen      (501) staff       (20)    10036 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_master_file_merged.bed
+-rw-r--r--   0 domen      (501) staff       (20)      339 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/raw_cuffdiff.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)    63817 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/CM_mate1.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)   395673 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/seq_reads_fastqc.zip
+-rw-r--r--   0 domen      (501) staff       (20)       80 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/expression_bcm_rpkm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      103 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_5_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      212 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sample_cluster_data_NCBI.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2665 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/adapters.fasta
+-rw-r--r--   0 domen      (501) staff       (20)     1554 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ontology_mus_cropped.obo.gz
+-rw-r--r--   0 domen      (501) staff       (20)    12879 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Jbrowse_genome_coverage.bw
+-rw-r--r--   0 domen      (501) staff       (20)    35359 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/AX4_mate1.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      396 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/wgbs.bam
+-rw-r--r--   0 domen      (501) staff       (20)     2044 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ncRNA_genome.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)   788254 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/silva-arc-16s-id95.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1417 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/demultiplexed_reads_rw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)       70 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_cpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1275 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_rw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      231 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/edgeR.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      585 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_counts_detect_strandedness.bam
+-rw-r--r--   0 domen      (501) staff       (20)    31848 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffquant_mapping.bam
+-rw-r--r--   0 domen      (501) staff       (20)      298 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/salmon_cds.fa.gz
+-rw-r--r--   0 domen      (501) staff       (20)    51642 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_dm6.bam
+-rw-r--r--   0 domen      (501) staff       (20)     2081 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1_transformed_R2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      460 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/HS chr21_short.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      154 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/clustering_NCBI.gz
+-rw-r--r--   0 domen      (501) staff       (20)   362869 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_mate1.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)   559048 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_aligment.bam
+-rw-r--r--   0 domen      (501) staff       (20)   114556 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid.bam
+-rw-r--r--   0 domen      (501) staff       (20)     8414 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k0.gatkHC.vcf
+-rw-r--r--   0 domen      (501) staff       (20)      112 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_genome.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)      375 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bad.bed
+-rw-r--r--   0 domen      (501) staff       (20)      188 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bowtie_use_SE_report.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)    16021 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_expressions_2.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       60 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_bbduk_star_htseq_paired_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      475 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mappings_update.tab
+-rw-r--r--   0 domen      (501) staff       (20)      767 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffmerge_transcripts.gtf
+-rw-r--r--   0 domen      (501) staff       (20)      320 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_reverse.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)       62 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mate1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1143 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat-seq.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)   524296 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamliquidator_summary.html
+-rw-r--r--   0 domen      (501) staff       (20)      528 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/go_enriched_terms_dicty.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1776 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_mm10.bam.bai
+-rw-r--r--   0 domen      (501) staff       (20)    14384 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs14_chr22.bed
+-rw-r--r--   0 domen      (501) staff       (20)   328968 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chr21_small.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)      156 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt forward1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      621 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1074 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mm10_small.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      174 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/SRR1661332.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1111 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.read2.small.qseq.bz2
+-rw-r--r--   0 domen      (501) staff       (20)      576 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset-py2.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      172 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_paired_forward_trimmed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      249 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_paired_reverse_trimmed.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1057 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_sw_reads_mapped.bam
+-rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/6-cuffquant.cxb
+-rwxr-xr-x   0 domen      (501) staff       (20)     1080 2017-12-26 13:22:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads.bam
+-rw-r--r--   0 domen      (501) staff       (20)      239 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/diff_exp_check_types.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      414 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/go_enriched_terms_mouse.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)    13972 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_adapters.fasta
+-rw-r--r--   0 domen      (501) staff       (20)      202 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ncRNA_annotation.gff.gz
+-rw-r--r--   0 domen      (501) staff       (20)      168 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bowtie_single_reads_report.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      363 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chip_seq_peakscore_genomicContext
+-rw-r--r--   0 domen      (501) staff       (20)       99 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_2_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       37 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_3.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      602 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/log_box_plot.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      192 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rsem_genes_single.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      259 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/annotation_rsem.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)     8396 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_probe_info.txt
+-rw-r--r--   0 domen      (501) staff       (20)       85 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/test_etc.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)       73 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffquant_exp.tab
+-rw-r--r--   0 domen      (501) staff       (20)       64 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_2.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)      266 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/diff_exp_check_geneid_type.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      197 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rsem_isoforms_single.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      284 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/tophat_paired_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)       56 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/upload_file.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)      394 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/subread_paired_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)       84 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/merged_etc.tab
+-rw-r--r--   0 domen      (501) staff       (20)      412 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_coverage.bam
+-rw-r--r--   0 domen      (501) staff       (20)    16827 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chip_seq_control.bam
+-rw-r--r--   0 domen      (501) staff       (20)      783 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/20Hr.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1345 2018-03-29 20:59:09.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_rv_reads.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1357 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_prinseq_paired_rw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      224 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_locations.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_rnaseq_paired_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)    24452 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_primers.bed
+-rw-r--r--   0 domen      (501) staff       (20)      376 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_bt_reads_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      197 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/clustering_expressions_3.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1596 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rose2_test.txt
+-rw-r--r--   0 domen      (501) staff       (20)      645 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/HSQUtils_dedup_summary.txt
+-rw-r--r--   0 domen      (501) staff       (20)   129789 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_counts hs_paired.bam
+-rw-r--r--   0 domen      (501) staff       (20)     3357 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs genome.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)    10983 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chip_seq_case.bam
+-rw-r--r--   0 domen      (501) staff       (20)    24934 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bt_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)      156 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/clustering_NCBI_2.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1273 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_fw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    31768 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot_alignment.bam
+-rw-r--r--   0 domen      (501) staff       (20)    37060 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/AX4_mate2.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)       66 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/5_prime_adapter.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)      102 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_4_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      264 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ChIP-Seq-Case.bam.bai
+-rw-r--r--   0 domen      (501) staff       (20)     1508 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.lf.vcf
+-rw-r--r--   0 domen      (501) staff       (20)    66079 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/human_genes.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       83 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/merged_etc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      167 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffnorm_all_fpkm_means.txt
+-rw-r--r--   0 domen      (501) staff       (20)     1177 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/demultiplexed_reads_fw.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2135 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    36818 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/dicty_genes.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      135 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffnorm_expression.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       60 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_ccshp.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     3784 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/1000G_phase1.indels.b37_chr2_small.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      939 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/my.strange.genome name$.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)      104 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_bam_upload_index.bai
+-rw-r--r--   0 domen      (501) staff       (20)      787 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sp_test_compatibility_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)      538 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gff_to_gtf_annotation.gtf
+-rw-r--r--   0 domen      (501) staff       (20)      343 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/igv_session_bam.xml
+-rw-r--r--   0 domen      (501) staff       (20)    20746 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_bt2_index.tar.gz
+-rw-r--r--   0 domen      (501) staff       (20)   427201 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_mate2_paired_filtered.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      212 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/clustering_expressions_1.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     3030 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/wgbs.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    61781 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/CM_mate2.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1383 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cDNA_reference.fasta.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1759 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      479 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gaf_mgi_cropped.gz
+-rw-r--r--   0 domen      (501) staff       (20)      210 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffdiff.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)    18544 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/5-cuffquant.cxb
+-rw-r--r--   0 domen      (501) staff       (20)      264 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gene_cluster_data_NCBI.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)    70093 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k_mate1.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     5696 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.read1.small.qseq.bz2
+-rw-r--r--   0 domen      (501) staff       (20)      642 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Jbrowse_norm_genome_coverage.bw
+-rw-r--r--   0 domen      (501) staff       (20)       65 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mirna_featurecounts_tpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1315 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hg19_chr20_small.gtf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      135 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exp_1_tpm.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)      323 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bowtie2_paired_end_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)    69449 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_trimmed_mate2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    19264 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_coverage.bw
+-rw-r--r--   0 domen      (501) staff       (20)      294 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bowtie2_use_SE_report.txt
+-rw-r--r--   0 domen      (501) staff       (20)   343439 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_mate2.fq.gz
+-rw-r--r--   0 domen      (501) staff       (20)    17421 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_single bbduk_star_htseq_reads_single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      124 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_ccsrs.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)       61 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_bbduk_star_htseq_single_rc.tab.gz
+-rw-r--r--   0 domen      (501) staff       (20)     6363 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/s_1_3.qseq.small.txt.bz2
+-rw-r--r--   0 domen      (501) staff       (20)      116 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID.lf.finalvars.txt
+-rw-r--r--   0 domen      (501) staff       (20)       58 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_3.json.gz
+-rw-r--r--   0 domen      (501) staff       (20)     1329 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA_forw_single.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2670 2018-04-05 13:55:13.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rw reads_2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)   680291 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k_mate2.fastq.gz
+-rw-r--r--   0 domen      (501) staff       (20)      557 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exons_coverage.txt.gz
+-rw-r--r--   0 domen      (501) staff       (20)     2181 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/igv_human.lf.vcf.gz
+-rw-r--r--   0 domen      (501) staff       (20)      281 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bowtie2_reads_report.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/commands/
+-rw-r--r--   0 domen      (501) staff       (20)     8987 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/commands/test_generators.py
+-rw-r--r--   0 domen      (501) staff       (20)       57 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/tests/commands/__init__.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/
+-rw-r--r--   0 domen      (501) staff       (20)       25 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/__init__.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/
+-rw-r--r--   0 domen      (501) staff       (20)     4461 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_geneset.py
+-rw-r--r--   0 domen      (501) staff       (20)    10549 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_samples.py
+-rw-r--r--   0 domen      (501) staff       (20)       34 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)    10771 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_diffexpr_deseq.py
+-rw-r--r--   0 domen      (501) staff       (20)    11891 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_diffexpr_cuffdiff.py
+-rw-r--r--   0 domen      (501) staff       (20)     5839 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/utils.py
+-rw-r--r--   0 domen      (501) staff       (20)     4645 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_etc.py
+-rw-r--r--   0 domen      (501) staff       (20)      188 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/__init__.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/utils/
+-rw-r--r--   0 domen      (501) staff       (20)      202 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/utils/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     7423 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/utils/test.py
+-rw-r--r--   0 domen      (501) staff       (20)      354 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/resolwe_bio/utils/filter.py
+-rw-r--r--   0 domen      (501) staff       (20)      208 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/apps.py
+-rw-r--r--   0 domen      (501) staff       (20)     1462 2018-04-09 16:06:55.000000 resolwe-bio-9.0.0a4/resolwe_bio/extensions.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/
+-rw-r--r--   0 domen      (501) staff       (20)     3013 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/bbduk-star-featurecounts.yml
+-rw-r--r--   0 domen      (501) staff       (20)     3477 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/sample_detailed.yml
+-rw-r--r--   0 domen      (501) staff       (20)     4176 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/sample_vaccinesurvey.yml
+-rw-r--r--   0 domen      (501) staff       (20)      991 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/diffexp.yml
+-rw-r--r--   0 domen      (501) staff       (20)      340 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/dicty.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2049 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/bcm.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2081 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/rnaseq.yml
+-rw-r--r--   0 domen      (501) staff       (20)     6559 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/reads.yml
+-rw-r--r--   0 domen      (501) staff       (20)      162 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/geneset.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1073 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/transmart.yml
+-rw-r--r--   0 domen      (501) staff       (20)     5736 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/reads_detailed.yml
+-rw-r--r--   0 domen      (501) staff       (20)     1891 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/amplicon.yml
+-rw-r--r--   0 domen      (501) staff       (20)     3929 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/sample_geo.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2907 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/etc.yml
+-rw-r--r--   0 domen      (501) staff       (20)      871 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/cutadapt-star-htseq.yml
+-rw-r--r--   0 domen      (501) staff       (20)     3954 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/microarray_affy.yml
+-rw-r--r--   0 domen      (501) staff       (20)     2202 2018-04-25 17:12:42.000000 resolwe-bio-9.0.0a4/resolwe_bio/descriptors/bbduk-star-htseq.yml
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/packages-manual/
+-rw-r--r--   0 domen      (501) staff       (20)        0 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/packages-manual/.placeholder
+-rw-r--r--   0 domen      (501) staff       (20)      251 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/Dockerfile
+-rw-r--r--   0 domen      (501) staff       (20)      233 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/packages-debian.txt
+-rw-r--r--   0 domen      (501) staff       (20)      226 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/packages-python3.txt
+-rw-r--r--   0 domen      (501) staff       (20)      351 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/README.md
+-rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/packages-debian-buildreq.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/assets/
+-rw-r--r--   0 domen      (501) staff       (20)     5641 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/assets/logo_genialis.pdf
+-rw-r--r--   0 domen      (501) staff       (20)     5219 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/assets/template_amplicon_report.tex
+-rw-r--r--   0 domen      (501) staff       (20)     5086 2018-05-14 09:12:22.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/assets/template_amplicon_report_multi_sample.tex
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/
+-rw-r--r--   0 domen      (501) staff       (20)     1077 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/r-packages.sh
+-rw-r--r--   0 domen      (501) staff       (20)      317 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/primerclip.sh
+-rw-r--r--   0 domen      (501) staff       (20)      404 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/lofreq.sh
+-rw-r--r--   0 domen      (501) staff       (20)      367 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/gatk.sh
+-rw-r--r--   0 domen      (501) staff       (20)      460 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/bokeh-assets.sh
+-rw-r--r--   0 domen      (501) staff       (20)      717 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/snpeff.sh
+-rw-r--r--   0 domen      (501) staff       (20)       55 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/README.txt
+-rw-r--r--   0 domen      (501) staff       (20)      441 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/samtools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      251 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/Dockerfile
+-rw-r--r--   0 domen      (501) staff       (20)       84 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-debian.txt
+-rw-r--r--   0 domen      (501) staff       (20)       63 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual.txt
+-rw-r--r--   0 domen      (501) staff       (20)        9 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-r.txt
+-rw-r--r--   0 domen      (501) staff       (20)     2107 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-python3.txt
+-rw-r--r--   0 domen      (501) staff       (20)      470 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/README.md
+-rw-r--r--   0 domen      (501) staff       (20)      290 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-debian-buildreq.txt
+-rw-r--r--   0 domen      (501) staff       (20)       28 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-r-bioconductor.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/assets/
+-rw-r--r--   0 domen      (501) staff       (20)      454 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/assets/amplicon_html_template.html
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/
+-rw-r--r--   0 domen      (501) staff       (20)      149 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-python2-stage2.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/
+-rw-r--r--   0 domen      (501) staff       (20)      919 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/jbrowse.sh
+-rw-r--r--   0 domen      (501) staff       (20)      397 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/subread.sh
+-rw-r--r--   0 domen      (501) staff       (20)      354 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/ea-utils.sh
+-rw-r--r--   0 domen      (501) staff       (20)      382 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/sra-toolkit.sh
+-rw-r--r--   0 domen      (501) staff       (20)     1567 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/r-packages.sh
+-rw-r--r--   0 domen      (501) staff       (20)      311 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/primerclip.sh
+-rw-r--r--   0 domen      (501) staff       (20)      333 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/gotea.sh
+-rw-r--r--   0 domen      (501) staff       (20)      367 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/lofreq.sh
+-rw-r--r--   0 domen      (501) staff       (20)      427 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/moabs.sh
+-rw-r--r--   0 domen      (501) staff       (20)      321 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/bbmap.sh
+-rw-r--r--   0 domen      (501) staff       (20)      749 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/snpeff.sh
+-rw-r--r--   0 domen      (501) staff       (20)      521 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/hsqutils.sh
+-rw-r--r--   0 domen      (501) staff       (20)      401 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/bedtools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      458 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/trans-decoder.sh
+-rw-r--r--   0 domen      (501) staff       (20)      502 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/bcftools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      402 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/genome-tools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      356 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/fastqc.sh
+-rw-r--r--   0 domen      (501) staff       (20)      449 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/hisat2.sh
+-rw-r--r--   0 domen      (501) staff       (20)      443 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/samtools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      356 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/bedops.sh
+-rw-r--r--   0 domen      (501) staff       (20)      471 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/kent-utils.sh
+-rw-r--r--   0 domen      (501) staff       (20)      441 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/star.sh
+-rw-r--r--   0 domen      (501) staff       (20)      387 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/cufflinks.sh
+-rw-r--r--   0 domen      (501) staff       (20)      423 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/prinseq.sh
+-rw-r--r--   0 domen      (501) staff       (20)      193 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/Dockerfile
+-rw-r--r--   0 domen      (501) staff       (20)      609 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-debian.txt
+-rw-r--r--   0 domen      (501) staff       (20)      209 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual.txt
+-rw-r--r--   0 domen      (501) staff       (20)       47 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-r.txt
+-rw-r--r--   0 domen      (501) staff       (20)     2579 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-python2.txt
+-rw-r--r--   0 domen      (501) staff       (20)      319 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-python3.txt
+-rw-r--r--   0 domen      (501) staff       (20)      280 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/README.md
+-rw-r--r--   0 domen      (501) staff       (20)      380 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-debian-buildreq.txt
+-rw-r--r--   0 domen      (501) staff       (20)      282 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-r-bioconductor.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-manual/
+-rw-r--r--   0 domen      (501) staff       (20)     1092 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-manual/wigtobigwig.sh
+-rw-r--r--   0 domen      (501) staff       (20)      241 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-manual/bamliquidator.sh
+-rw-r--r--   0 domen      (501) staff       (20)      127 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/Dockerfile
+-rw-r--r--   0 domen      (501) staff       (20)      479 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-debian.txt
+-rw-r--r--   0 domen      (501) staff       (20)       26 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-manual.txt
+-rw-r--r--   0 domen      (501) staff       (20)      677 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-python2.txt
+-rw-r--r--   0 domen      (501) staff       (20)      372 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/README.md
+-rw-r--r--   0 domen      (501) staff       (20)      112 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-debian-buildreq.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-manual/
+-rw-r--r--   0 domen      (501) staff       (20)      657 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-manual/sra-toolkit.sh
+-rw-r--r--   0 domen      (501) staff       (20)      383 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-manual/igvtools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      356 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-manual/fastqc.sh
+-rw-r--r--   0 domen      (501) staff       (20)      127 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/Dockerfile
+-rw-r--r--   0 domen      (501) staff       (20)       70 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-debian.txt
+-rw-r--r--   0 domen      (501) staff       (20)       27 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-manual.txt
+-rw-r--r--   0 domen      (501) staff       (20)     1122 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-python3.txt
+-rw-r--r--   0 domen      (501) staff       (20)      284 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/README.md
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/
+-rw-r--r--   0 domen      (501) staff       (20)      330 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/rsem.sh
+-rw-r--r--   0 domen      (501) staff       (20)      397 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/subread.sh
+-rw-r--r--   0 domen      (501) staff       (20)      644 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/trimmomatic.sh
+-rw-r--r--   0 domen      (501) staff       (20)     1151 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/r-packages.sh
+-rw-r--r--   0 domen      (501) staff       (20)      333 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/gotea.sh
+-rw-r--r--   0 domen      (501) staff       (20)      321 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/bbmap.sh
+-rw-r--r--   0 domen      (501) staff       (20)      421 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/salmon.sh
+-rw-r--r--   0 domen      (501) staff       (20)      435 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/bedtools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      356 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/fastqc.sh
+-rw-r--r--   0 domen      (501) staff       (20)      444 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/hisat2.sh
+-rw-r--r--   0 domen      (501) staff       (20)      441 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/samtools.sh
+-rw-r--r--   0 domen      (501) staff       (20)      441 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/star.sh
+-rw-r--r--   0 domen      (501) staff       (20)      387 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/cufflinks.sh
+-rw-r--r--   0 domen      (501) staff       (20)      127 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/Dockerfile
+-rw-r--r--   0 domen      (501) staff       (20)      268 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-debian.txt
+-rw-r--r--   0 domen      (501) staff       (20)      102 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual.txt
+-rw-r--r--   0 domen      (501) staff       (20)       18 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-r.txt
+-rw-r--r--   0 domen      (501) staff       (20)     1651 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-python3.txt
+-rw-r--r--   0 domen      (501) staff       (20)      657 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/README.md
+-rw-r--r--   0 domen      (501) staff       (20)      132 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-debian-buildreq.txt
+-rw-r--r--   0 domen      (501) staff       (20)       46 2018-04-13 10:35:48.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-r-bioconductor.txt
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/
+-rw-r--r--   0 domen      (501) staff       (20)     3135 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-16.04
+-rw-r--r--   0 domen      (501) staff       (20)     2484 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/common.sh
+-rw-r--r--   0 domen      (501) staff       (20)     3135 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-17.10
+-rw-r--r--   0 domen      (501) staff       (20)     3135 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-18.04
+-rw-r--r--   0 domen      (501) staff       (20)      530 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/README.md
+-rw-r--r--   0 domen      (501) staff       (20)     3135 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-14.04
+-rw-r--r--   0 domen      (501) staff       (20)      788 2018-05-14 12:44:14.000000 resolwe-bio-9.0.0a4/resolwe_bio/__about__.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/expression_filters/
+-rw-r--r--   0 domen      (501) staff       (20)       68 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/expression_filters/__init__.py
+-rw-r--r--   0 domen      (501) staff       (20)     1321 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/expression_filters/sample.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/resolwe_bio/fixtures/
+-rw-r--r--   0 domen      (501) staff       (20)      248 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/fixtures/relationtypes.yaml
+-rw-r--r--   0 domen      (501) staff       (20)     1455 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/resolwe_bio/filters.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/tests/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/tests/test_data/
+-rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a4/tests/test_data/README.rst
+-rw-r--r--   0 domen      (501) staff       (20)        0 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/tests/__init__.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/tests/test_runtime/
+-rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a4/tests/test_runtime/README.rst
+-rw-r--r--   0 domen      (501) staff       (20)      278 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a4/tests/routing.py
+-rw-r--r--   0 domen      (501) staff       (20)      351 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/tests/.env
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/tests/test_upload/
+-rw-r--r--   0 domen      (501) staff       (20)      118 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a4/tests/test_upload/README.rst
+-rw-r--r--   0 domen      (501) staff       (20)     5970 2018-03-28 12:55:15.000000 resolwe-bio-9.0.0a4/tests/settings.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/tests/fixtures/
+-rw-r--r--   0 domen      (501) staff       (20)     1668 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/tests/fixtures/data.yaml
+-rw-r--r--   0 domen      (501) staff       (20)     1461 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/tests/fixtures/collection.yaml
+-rw-r--r--   0 domen      (501) staff       (20)     1012 2018-03-28 20:35:19.000000 resolwe-bio-9.0.0a4/tests/docker-compose.yml
+-rwxr-xr-x   0 domen      (501) staff       (20)      357 2018-03-07 07:28:32.000000 resolwe-bio-9.0.0a4/tests/manage.py
+-rw-r--r--   0 domen      (501) staff       (20)     1616 2017-12-26 15:46:53.000000 resolwe-bio-9.0.0a4/tests/urls.py
+-rw-r--r--   0 domen      (501) staff       (20)      655 2018-04-19 10:10:36.000000 resolwe-bio-9.0.0a4/MANIFEST.in
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/docs/
+-rw-r--r--   0 domen      (501) staff       (20)      480 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/index.rst
+-rw-r--r--   0 domen      (501) staff       (20)       78 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/catalog-definitions.rst
+-rw-r--r--   0 domen      (501) staff       (20)      339 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/catalog.rst
+-rw-r--r--   0 domen      (501) staff       (20)     7099 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/docs/contributing.rst
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/docs/_templates/
+-rw-r--r--   0 domen      (501) staff       (20)      477 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/_templates/page.html
+-rw-r--r--   0 domen      (501) staff       (20)     3113 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/conf.py
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/docs/_static/
+drwxr-xr-x   0 domen      (501) staff       (20)        0 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/docs/_static/css/
+-rw-r--r--   0 domen      (501) staff       (20)      244 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/_static/css/custom.css
+-rw-r--r--   0 domen      (501) staff       (20)      985 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/proc.rst
+-rw-r--r--   0 domen      (501) staff       (20)      651 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/catalog-types.rst
+-rw-r--r--   0 domen      (501) staff       (20)       65 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/ref.rst
+-rw-r--r--   0 domen      (501) staff       (20)       92 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/catalog-category.rst
+-rw-r--r--   0 domen      (501) staff       (20)    33701 2018-05-14 12:41:05.000000 resolwe-bio-9.0.0a4/docs/CHANGELOG.rst
+-rw-r--r--   0 domen      (501) staff       (20)     2645 2017-12-26 15:46:08.000000 resolwe-bio-9.0.0a4/docs/descriptor.rst
+-rw-r--r--   0 domen      (501) staff       (20)     3224 2018-05-14 09:13:02.000000 resolwe-bio-9.0.0a4/setup.py
+-rw-r--r--   0 domen      (501) staff       (20)     3551 2018-03-21 08:17:24.000000 resolwe-bio-9.0.0a4/tox.ini
+-rw-r--r--   0 domen      (501) staff       (20)      275 2018-05-14 12:46:07.000000 resolwe-bio-9.0.0a4/setup.cfg
+-rw-r--r--   0 domen      (501) staff       (20)     3716 2018-03-21 08:17:23.000000 resolwe-bio-9.0.0a4/README.rst
```

### Comparing `resolwe-bio-9.0.0a3/PKG-INFO` & `resolwe-bio-9.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: resolwe-bio
-Version: 9.0.0a3
+Version: 9.0.0a4
 Summary: Bioinformatics pipelines for the Resolwe platform
 Home-page: https://github.com/genialis/resolwe-bio
 Author: Genialis d.o.o.
 Author-email: dev-team@genialis.com
 License: Apache License (2.0)
 Description-Content-Type: UNKNOWN
 Description: ======================
```

### Comparing `resolwe-bio-9.0.0a3/.pylintrc` & `resolwe-bio-9.0.0a4/.pylintrc`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/.resolwebio-filetypes.yml` & `resolwe-bio-9.0.0a4/.resolwebio-filetypes.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/LICENSE` & `resolwe-bio-9.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio.egg-info/PKG-INFO` & `resolwe-bio-9.0.0a4/resolwe_bio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: resolwe-bio
-Version: 9.0.0a3
+Version: 9.0.0a4
 Summary: Bioinformatics pipelines for the Resolwe platform
 Home-page: https://github.com/genialis/resolwe-bio
 Author: Genialis d.o.o.
 Author-email: dev-team@genialis.com
 License: Apache License (2.0)
 Description-Content-Type: UNKNOWN
 Description: ======================
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio.egg-info/SOURCES.txt` & `resolwe-bio-9.0.0a4/resolwe_bio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -334,20 +334,22 @@
 resolwe_bio/tests/files/3-cuffquant.cxb
 resolwe_bio/tests/files/3_prime_adapter.fasta.gz
 resolwe_bio/tests/files/3ptrim_new56Gprimers.fa.gz
 resolwe_bio/tests/files/4-cuffquant.cxb
 resolwe_bio/tests/files/5-cuffquant.cxb
 resolwe_bio/tests/files/56G masterfile_dup_amplicon_names.txt.gz
 resolwe_bio/tests/files/56G masterfile_lowercase_bases.txt.gz
+resolwe_bio/tests/files/56GSID.gatk.finalvars.txt
 resolwe_bio/tests/files/56GSID.gatkHC.finalvars.txt
 resolwe_bio/tests/files/56GSID.lf.finalvars.txt
 resolwe_bio/tests/files/56GSID_10k.gatkHC.vcf.gz
 resolwe_bio/tests/files/56GSID_10k.gatkHC4.vcf.gz
 resolwe_bio/tests/files/56GSID_10k.lf.vcf
 resolwe_bio/tests/files/56GSID_10k.lf.vcf.gz
+resolwe_bio/tests/files/56GSID_10k0.gatkHC.vcf
 resolwe_bio/tests/files/56GSID_10k_ampmeancov.covd
 resolwe_bio/tests/files/56GSID_10k_covMetrics.txt
 resolwe_bio/tests/files/56GSID_10k_mate1.fastq.gz
 resolwe_bio/tests/files/56GSID_10k_mate2.fastq.gz
 resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_genes.txt
 resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_summary.html
 resolwe_bio/tests/files/56GSID_1k_mate1.fastq.gz
@@ -506,19 +508,20 @@
 resolwe_bio/tests/files/exp_matrix.json.gz
 resolwe_bio/tests/files/exp_unix_line_ending.txt.gz
 resolwe_bio/tests/files/exp_windows_line_ending.txt.gz
 resolwe_bio/tests/files/expression_bcm_rpkm.tab.gz
 resolwe_bio/tests/files/expression_htseq.json.gz
 resolwe_bio/tests/files/expressions-py2.json.gz
 resolwe_bio/tests/files/expressions-py3.json.gz
+resolwe_bio/tests/files/feature_counts hs.gtf.gz
+resolwe_bio/tests/files/feature_counts hs_paired.bam
 resolwe_bio/tests/files/feature_counts_detect_strandedness.bam
 resolwe_bio/tests/files/feature_counts_out_fpkm.tab.gz
 resolwe_bio/tests/files/feature_counts_out_rc.tab.gz
 resolwe_bio/tests/files/feature_counts_out_tpm.tab.gz
-resolwe_bio/tests/files/feature_counts_paired.bam
 resolwe_bio/tests/files/feature_locations.json.gz
 resolwe_bio/tests/files/features.tab
 resolwe_bio/tests/files/features_gsea.tab.zip
 resolwe_bio/tests/files/features_update.tab.gz
 resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_fw.fastq.gz
 resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_rw.fastq.gz
 resolwe_bio/tests/files/filtered_reads_fastqmcf_single.fastq.gz
@@ -818,14 +821,15 @@
 resolwe_bio/tools/parse_encoding_type.py
 resolwe_bio/tools/parse_library_type.py
 resolwe_bio/tools/parse_star_expressions.py
 resolwe_bio/tools/pca.py
 resolwe_bio/tools/peak2geneScore.R
 resolwe_bio/tools/plot_enhancers.py
 resolwe_bio/tools/plotcoverage_html.py
+resolwe_bio/tools/postprocess_snpeff.py
 resolwe_bio/tools/rnaseq.py
 resolwe_bio/tools/run_edger.R
 resolwe_bio/tools/samplehcluster.py
 resolwe_bio/tools/transmart_fetch.R
 resolwe_bio/tools/transmart_import.py
 resolwe_bio/tools/transmart_utils.py
 resolwe_bio/tools/unique_sample_names.py
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/migrations/0005_make_date_indexes.py` & `resolwe-bio-9.0.0a4/resolwe_bio/migrations/0005_make_date_indexes.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/migrations/0010_add_relation_types.py` & `resolwe-bio-9.0.0a4/resolwe_bio/migrations/0010_add_relation_types.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/migrations/0004_add_owner.py` & `resolwe-bio-9.0.0a4/resolwe_bio/migrations/0004_add_owner.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/migrations/0008_migrate_sample.py` & `resolwe-bio-9.0.0a4/resolwe_bio/migrations/0008_migrate_sample.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/migrations/0009_delete_sample.py` & `resolwe-bio-9.0.0a4/resolwe_bio/migrations/0009_delete_sample.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/migrations/0001_initial.py` & `resolwe-bio-9.0.0a4/resolwe_bio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/migrations/0003_fix_jsonfields.py` & `resolwe-bio-9.0.0a4/resolwe_bio/migrations/0003_fix_jsonfields.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/convert_DE_excel_table.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/convert_DE_excel_table.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/basespace_download.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/basespace_download.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/plot_enhancers.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/plot_enhancers.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_library_type.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_library_type.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/make_igv_session_archive.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/make_igv_session_archive.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/VCF_ad_extract.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/VCF_ad_extract.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/xgff.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/xgff.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/make_multireport.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/make_multireport.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,21 +123,21 @@
         url = 'http://www.ncbi.nlm.nih.gov/snp/?term={}'.format(snpid)
     elif snpid.startswith('COSM'):
         url = 'http://cancer.sanger.ac.uk/cosmic/mutation/overview?genome=37\&id={}'.format(snpid.lstrip('COSM'))
     elif snpid.startswith('COSN'):
         url = 'http://cancer.sanger.ac.uk/cosmic/ncv/overview?genome=37\&id={}'.format(snpid.lstrip('COSN'))
     else:
         return snpid
-    return '\\href{{{}}}{{{}}}'.format(url, snpid)
+    return '\\href{{{}}}{{{}}}'.format(url, _escape_latex(snpid))
 
 
 def gene_href(gene_name):
     """Create LaTeX hyperlink for given GENE ID."""
     url = 'http://www.ncbi.nlm.nih.gov/gene/?term={}'.format(gene_name)
-    return '\\href{{{}}}{{{}}}'.format(url, gene_name)
+    return '\\href{{{}}}{{{}}}'.format(url, _escape_latex(gene_name))
 
 
 def parse_stats(stats_file):
     """Parse stats file."""
     stats = {}
     with open(stats_file) as sfile:
         for row_raw in sfile:
@@ -239,23 +239,23 @@
 
     output_file("{}.html".format(fig_name.replace(" ", "")), title=fig_name)
     save(p)
 
 
 def format_aa_change(aa_list):
     """Create Amino Acid Change information."""
+    output = set()
     if aa_list:
-        aa = aa_list[0]
-        match_obj = re.match(r'p\.([A-Za-z]*)[0-9]*([A-Za-z]*)', aa)
-        if match_obj and match_obj.group(1) == match_obj.group(2):
-            return 'Synon'
-        else:
-            return aa
-    else:
-        return ''
+        for aa in aa_list:
+            match_obj = re.match(r'p\.([A-Za-z]*)[0-9]*([A-Za-z]*)', aa)
+            if match_obj and match_obj.group(1) == match_obj.group(2):
+                output.add('Synon')
+            else:
+                output.add(_escape_latex(aa))
+    return output
 
 
 def format_float(value, decimals=DECIMALS, to_percent=False):
     """Round string representation of float to ``decimals`` decimal places.
 
     If ``to_percent``==True, also multiply by 100 and add latex percent sign.
     """
@@ -290,32 +290,31 @@
         common_columns.append('EFF[*].AA')
         legacy_aa_data = get_legacy_aa_data(varfile)
         vcf_table_tmp = [line + [legacy_aa_data[i]] for i, line in enumerate(vcf_table_tmp)]
     # Escape user inputs and change header:
     common_columns = [header_glossary.get(x, x) for x in common_columns]
     vcf_table = []
     for line_tmp in vcf_table_tmp:
-        line_tmp = [_escape_latex(cell) for cell in line_tmp]
         alt_cell, af_cell = line_tmp[3], line_tmp[4]
         # One line can contain two or more ALT values (and consequently two or more AF values)
         for alt, af_ in zip(alt_cell.split(','), af_cell.split(',')):
             if float(af_) >= float(args.afthreshold):
                 vcf_table.append(line_tmp[:3] + [alt] + [af_] + line_tmp[5:])
 
     # Fill variants dict with the variants that are shared
     for line in vcf_table:
         variant_name = '{}_chr{}_{}'.format(line[-3], line[0], line[1])
         variants.setdefault(variant_name, []).append([sample, line[4]])
 
     # Create hyperlink, and format amino acid changes:
     vcf_table = [
         line[:-3] +
-        [gene_href(line[-3])] +
+        [' '.join(map(gene_href, line[-3].split(',')))] +
         [' '.join(map(snp_href, line[-2].split(';')))] +
-        [format_aa_change(line[-1].split(','))]
+        [' '.join(format_aa_change(line[-1].split(',')))]
         for line in vcf_table
     ]
     return vcf_table, common_columns
 
 
 def make_names_unique(names):
     """
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/xexpression.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/xexpression.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_star_expressions.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_star_expressions.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/cufflinks_sample_groups.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/cufflinks_sample_groups.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/transmart_fetch.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/transmart_fetch.R`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/transmart_utils.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/transmart_utils.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/samplehcluster.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/samplehcluster.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/goea.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/goea.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/lofreq2_indel_ovlp.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/lofreq2_indel_ovlp.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/expressionmerge.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/expressionmerge.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/xgtf2gff.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/xgtf2gff.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/cuffnorm_group_labels.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/cuffnorm_group_labels.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/mergebowtiestats.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/mergebowtiestats.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/etc.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/etc.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/rnaseq.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/rnaseq.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/peak2geneScore.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/peak2geneScore.R`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/demultiplex.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/demultiplex.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/clustering_leaf_ordering.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/clustering_leaf_ordering.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/run_edger.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/run_edger.R`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/format_index_files.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/format_index_files.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/deseq.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/deseq.R`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/garvan_coverage.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/garvan_coverage.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/make_igv_session.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/make_igv_session.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/diffexp_filtering.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/diffexp_filtering.R`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/expression_aggregator.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/expression_aggregator.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/make_report.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/make_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 """Generate amplicon report."""
 import argparse
 import csv
 import os
+import re
 import subprocess
 
 DECIMALS = 2  # Decimal precision when presenting results:
 
 parser = argparse.ArgumentParser(description="Fill data into tex template file.")
 parser.add_argument('--sample', help="Sample name.")
 parser.add_argument('--panel', help="Panel name")
@@ -134,39 +135,54 @@
         url = 'http://www.ncbi.nlm.nih.gov/snp/?term={}'.format(snpid)
     elif snpid.startswith('COSM'):
         url = 'http://cancer.sanger.ac.uk/cosmic/mutation/overview?genome=37\&id={}'.format(snpid.lstrip('COSM'))
     elif snpid.startswith('COSN'):
         url = 'http://cancer.sanger.ac.uk/cosmic/ncv/overview?genome=37\&id={}'.format(snpid.lstrip('COSN'))
     else:
         return snpid
-    return '\\href{{{}}}{{{}}}'.format(url, snpid)
+    return '\\href{{{}}}{{{}}}'.format(url, escape_latex(snpid))
 
 
 def gene_href(gene_name):
     """Create LaTeX hyperlink for given GENE ID."""
     url = 'http://www.ncbi.nlm.nih.gov/gene/?term={}'.format(gene_name)
-    return '\\href{{{}}}{{{}}}'.format(url, gene_name)
+    return '\\href{{{}}}{{{}}}'.format(url, escape_latex(gene_name))
+
+
+def format_aa_change(aa_list):
+    """Create Amino Acid Change information."""
+    output = set()
+    if aa_list:
+        for aa in aa_list:
+            match_obj = re.match(r'p\.([A-Za-z]*)[0-9]*([A-Za-z]*)', aa)
+            if match_obj and match_obj.group(1) == match_obj.group(2):
+                output.add('Synon')
+            else:
+                output.add(escape_latex(aa))
+    return output
 
 
 def make_variant_table(variant_file, header, af_threshold):
     """Make variant table."""
     var_table = []
     with open(variant_file, 'r') as vfile:
         for row_raw in csv.DictReader(vfile, delimiter='\t'):
             # Reorder columns according to header
             row = [row_raw[column_name] for column_name in header]
 
-            gene_column = gene_href(row[-2])  # Create gene hypelinks
-            snp_column = ' '.join(map(snp_href, row[-1].split(';')))  # Create SNP hypelinks
+            row[-3] = ' '.join(map(gene_href, row[-3].split(',')))  # Create gene hypelinks
+            row[-2] = ' '.join(map(snp_href, row[-2].split(';')))  # Create SNP hypelinks
+            row[-1] = ' '.join(format_aa_change(row[-1].split(',')))  # Create amino acid column
+
             # One line can contain two or more ALT values (and consequently two or more AF values)
             # We need to split such "multiple" entries to one alt value per row
             alt_cell, afq_cell = row[3], row[4]
             for alt, afq in zip(alt_cell.split(','), afq_cell.split(',')):
                 if float(afq) >= af_threshold:
-                    var_table.append(row[:3] + [alt] + [afq] + row[5:-2] + [gene_column] + [snp_column])
+                    var_table.append(row[:3] + [alt] + [afq] + row[5:])
     return var_table
 
 
 if __name__ == '__main__':
     args = parser.parse_args()
 
     # Open template and fill it with data:
@@ -222,26 +238,27 @@
         # Make tables with variants for each variant caller.
         table_text = ''
         af_threshold = float(args.afthreshold)
         header_glossary = {'GEN[0].AD': 'AD', 'EFF[*].GENE': 'GENE', 'EFF[*].AA': 'AA'}
         for variant_file in args.annot_vars:
             # We have multiple (=2) variant files: this are NOT *.vcf files, but tabular files derived from them.
             # The problem is that their columns (and header names) differ depending on the variant caller tool.
+            COMMON_FIELDS = ['CHROM', 'POS', 'REF', 'ALT', 'AF', 'DP']
             if 'gatkhc.finalvars' in variant_file.lower():
-                header = ['CHROM', 'POS', 'REF', 'ALT', 'AF', 'DP', 'GEN[0].AD', 'FS', 'EFF[*].GENE', 'ID']
+                header = COMMON_FIELDS + ['GEN[0].AD', 'FS', 'EFF[*].GENE', 'ID', 'EFF[*].AA']
                 caption = 'GATK HaplotypeCaller variant calls'
             elif 'lf.finalvars' in variant_file.lower():
-                header = ['CHROM', 'POS', 'REF', 'ALT', 'AF', 'DP', 'DP4', 'SB', 'EFF[*].GENE', 'ID']
+                header = COMMON_FIELDS + ['DP4', 'SB', 'EFF[*].GENE', 'ID', 'EFF[*].AA']
                 caption = 'Lofreq variant calls'
             else:
                 raise ValueError('This variant caller is not supported for report generation')
 
             var_table = make_variant_table(variant_file, header, af_threshold)
             header = [escape_latex(header_glossary.get(col_name, col_name)) for col_name in header]
-            long_cls = [2, 3, -1]  # Potentially long columns are REF, ALT and ID
+            long_cls = [2, 3, -2, -1]  # Potentially long columns are REF, ALT, ID and AA
             table_text += list_to_tex_table(var_table, header=header, caption=caption, long_columns=long_cls)
             table_text += '\n\\newpage\n'
 
         template = template.replace('{#VCF_TABLES#}', table_text)
 
         # Write template to 'report.tex'
         template_out.write(template)
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/expressionmerge_archive.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/expressionmerge_archive.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/mappability.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/mappability.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_diffexp.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_diffexp.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/geneset2storage.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/geneset2storage.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/pca.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/pca.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/genehcluster.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/genehcluster.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/find_similar.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/find_similar.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/plotcoverage_html.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/plotcoverage_html.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/transmart_import.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/transmart_import.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/detect_strandedness.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/detect_strandedness.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/fastqc.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/fastqc.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/compatibilty_check.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/compatibilty_check.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/mergeetc.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/mergeetc.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/expression_fpkm_tpm.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/expression_fpkm_tpm.R`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 #!/usr/bin/Rscript
-require('rtracklayer') ; require('argparse')
+suppressPackageStartupMessages(require('rtracklayer'))
+suppressPackageStartupMessages(require('argparse'))
 
 parser = ArgumentParser(description='Calculate expression values in FPKM and TPM units.')
 parser$add_argument('annotation', help='Gene model (GTF/GFF) annotation file')
 parser$add_argument('format', help='Annotation version/format')
 parser$add_argument('feature_type', help='Feature type (e.g. exon)')
 parser$add_argument('id_attribute', help='GFF attribute to be used as feature ID (e.g. gene_id)')
 parser$add_argument('counts_file', help='Read-count data')
 
 args = parser$parse_args(commandArgs(trailingOnly=TRUE))
 
 # retrieve exon lengths
 annot <- import.gff(args$annotation, format=args$format, genome="NA", feature.type=args$feature_type)
-exon_lengths=width(annot)
-names(exon_lengths)=elementMetadata(annot)[,args$id_attribute]
+exon_lengths <- width(annot)
+names(exon_lengths) <- elementMetadata(annot)[, args$id_attribute]
 
-# calculate gene lengths
-exon_lengths_by_gene=split(exon_lengths, names(exon_lengths))
-gene_lengths=sapply(exon_lengths_by_gene, sum)
+# calculate gene or transcript lengths
+gene_lengths <- sapply(split(exon_lengths, names(exon_lengths)), FUN = sum)
 
 # normalise counts by library size
-counts <- read.delim(args$counts_file, header = FALSE)
-rownames(counts) <- counts[,1]
-counts[,1] <- NULL
-lib_size=colSums(counts)
-ncounts=t(t(counts)/lib_size)
+ncounts <- read.delim(args$counts_file, header = FALSE)
+names(ncounts) <- c("Gene", "raw_count")
+ncounts$norm_count <- ncounts$raw_count / sum(ncounts$raw_count) # library_size
 
 # obtain CPM
-cpm=ncounts*1e6
+cpm <- ncounts$norm_count * 1e6
+names(cpm) <- ncounts$Gene
+cpm <- cpm[order(names(cpm))] # lexicographically order cpm
+
+# select common genes
+common_genes <- intersect(ncounts$Gene, names(gene_lengths))
+subset_ncounts <- ncounts[as.character(ncounts$Gene) %in% common_genes, ]
+
+# prepare gene_lengths in format for merging with ncounts
+gene_lengths <- data.frame(Gene = names(gene_lengths), gene_lengths = unname(gene_lengths))
+subset_ncounts <- merge(subset_ncounts, gene_lengths)
 
-# normalise counts by gene length
-common_genes=intersect(row.names(ncounts), names(gene_lengths))
-subset_ncounts=ncounts[row.names(ncounts) %in% common_genes,]
-gene_lengths=gene_lengths[names(gene_lengths) %in% common_genes]
-ncounts_length_norm=subset_ncounts/gene_lengths
+# normalized count normalized by gene length
+subset_ncounts$norm <- with(subset_ncounts, norm_count/gene_lengths)
 
 # obtain RPKMs
-rpkm=ncounts_length_norm*1e9
+rpkm <- subset_ncounts$norm * 1e9
+names(rpkm) <- subset_ncounts$Gene
 
 # obtain TPM
 tpm = exp(log(rpkm) - log(sum(rpkm)) + log(1e6))
 
 # write data tables
 write.table(cpm, file="cpm_wo_header.tab", sep="\t", na="0", quote = FALSE, col.names = FALSE)
 write.table(rpkm, file="fpkm_wo_header.tab", sep="\t", na="0", quote = FALSE, col.names = FALSE)
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_cuffnorm.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_cuffnorm.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/mergebowtie2stats_paired.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/mergebowtie2stats_paired.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/add_header.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/add_header.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_closest_features.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_closest_features.R`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/importETC.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/importETC.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/parse_encoding_type.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/parse_encoding_type.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/volcanoplot.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/volcanoplot.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/mergebowtie2stats.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/mergebowtie2stats.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/feature_location.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/feature_location.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/unique_sample_names.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/unique_sample_names.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/microarrayQC.R` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/microarrayQC.R`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/bamliquidator_table.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/bamliquidator_table.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/go_genesets.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/go_genesets.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/cuffnorm_output_table_headers.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/cuffnorm_output_table_headers.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/xtabcoverage.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/xtabcoverage.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/make_amplicon_table.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/make_amplicon_table.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/gff3_to_gtf.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/gff3_to_gtf.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/validate_master_file.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/validate_master_file.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tools/expression2storage.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tools/expression2storage.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0002_alter_field_max_length.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0002_alter_field_max_length.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0001_initial.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/migrations/0005_species.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/migrations/0005_species.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/models.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/models.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/serializers.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/serializers.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/test_feature.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/test_import_kb.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/test_import_kb.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/tests/test_mapping.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/insert_features.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/insert_features.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/utils.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/utils.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/management/commands/insert_mappings.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/management/commands/insert_mappings.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/admin.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/admin.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/elastic_indexes.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/elastic_indexes.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/filters.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/filters.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/kb/views.py` & `resolwe-bio-9.0.0a4/resolwe_bio/kb/views.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/transmart/import.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/transmart/import.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/go_enrichment/go.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/go_enrichment/go.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/edgeR.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/edgeR.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/deseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/deseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/cuffdiff.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/cuffdiff.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/differential_expression/abstract.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/differential_expression/abstract.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_list.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_list.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_hidden_fields.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_hidden_fields.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_disabled_fields.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_disabled_fields.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_basic_fields.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_basic_fields.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/unit_tests/test_sleep_progress.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/unit_tests/test_sleep_progress.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/amplicon/amplicon_table.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/amplicon/amplicon_table.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/amplicon/target_metrics.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/amplicon/target_metrics.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/amplicon/bwa_trim.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/amplicon/bwa_trim.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/assembly/abyss.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/assembly/abyss.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/clustering/pca.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/clustering/pca.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/clustering/find_similar.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/clustering/find_similar.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/clustering/hierarchical_clustering.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/clustering/hierarchical_clustering.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/bbduk_star_featurecounts.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/bbduk_star_featurecounts.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/cutadapt_star_htseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/cutadapt_star_htseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/rnaseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/rnaseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/wgbs.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/wgbs.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/heat_seq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/heat_seq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/bbduk_star_htseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/bbduk_star_htseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/amplicon.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/amplicon.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/cuffquant.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/cuffquant.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/cutadapt_star_rsem.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/cutadapt_star_rsem.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/mirna.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/mirna.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/chemut.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/chemut.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/workflows/chip_seq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/workflows/chip_seq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/nucleotide_seq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/nucleotide_seq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/geneset.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/geneset.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/master_file.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/master_file.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/genome.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/genome.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/go_gaf.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/go_gaf.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/annotation.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/annotation.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/sam_header.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/sam_header.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/expressions.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/expressions.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/sra_file.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/sra_file.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/variants_bed.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/variants_bed.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/differential_exp.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/differential_exp.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/etc.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/etc.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/basespace.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/basespace.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/cuffquant.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/cuffquant.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/snpeff.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/snpeff.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/target_pcr_metrics.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/target_pcr_metrics.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/variants_vcf.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/variants_vcf.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/pathway_map.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/pathway_map.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/hmmer_database.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/hmmer_database.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/go_obo.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/go_obo.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/mappability_bigwig.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/mappability_bigwig.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/mappability_tab.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/mappability_tab.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/annotation_bed.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/annotation_bed.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/seq_reads_multiplexed.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/seq_reads_multiplexed.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/bam.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/bam.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/seq_reads.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/seq_reads.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/import_data/microarray_affy.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/import_data/microarray_affy.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/annotation/cuffmerge.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/annotation/cuffmerge.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/annotation/feature_location.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/annotation/feature_location.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/annotation/abstract.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/annotation/abstract.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/WGBS/mcall.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/WGBS/mcall.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/WGBS/bsmap.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/WGBS/bsmap.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/macs14.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/macs14.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/scoring.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/scoring.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/rose2.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/rose2.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/chip_seq/macs2.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/chip_seq/macs2.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/microarray/microarray_qc.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/microarray/microarray_qc.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/star.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/star.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/hisat2.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/hisat2.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/tophat.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/tophat.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/bowtie.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/bowtie.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/subread.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/subread.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/bwa.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/bwa.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/alignment/abstract.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/alignment/abstract.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/genome_browser/igv_bam.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/genome_browser/igv_bam.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/featureCounts.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/featureCounts.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/dicty_bcm.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/dicty_bcm.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/merge_expressions.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/merge_expressions.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/htseq_count.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/htseq_count.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/merge_etc.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/merge_etc.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/index_fasta_nucl.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/index_fasta_nucl.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/etc.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/etc.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/cuffnorm.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/cuffnorm.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/cuffquant.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/cuffquant.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/mappability.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/mappability.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/rsem.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/rsem.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/salmon_index.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/salmon_index.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/expression_aggregator.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/expression_aggregator.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/cufflinks.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/cufflinks.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/expression/abstract.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/expression/abstract.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/exome_coverage/coverage_report.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/exome_coverage/coverage_report.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/exome_coverage/coveragebed.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/exome_coverage/coveragebed.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/hsqutils.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/hsqutils.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/bbduk.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/bbduk.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/merge_to_paired_end.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/merge_to_paired_end.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/cutadapt.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/cutadapt.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/cutadapt_amplicon.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/cutadapt_amplicon.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/prinseq_lite.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/prinseq_lite.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/fastq_mcf.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/fastq_mcf.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/cutadapt_custom.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/cutadapt_custom.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/sortmerna.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/sortmerna.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reads_processing/trimmomatic.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reads_processing/trimmomatic.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/preprocess_bam.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/preprocess_bam.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/gatk.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/gatk.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/vc_chemut.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/vc_chemut.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/samtools.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/samtools.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/filtering_chemut.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/filtering_chemut.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/snpeff.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/snpeff.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     expression-engine: jinja
     executor:
       docker:
         image: resolwebio/legacy:1.0.0
     resources:
       memory: 16384
   data_name: "snpEff ({{ variants|sample_name|default('?') }})"
-  version: 0.1.7
+  version: 0.1.8
   type: data:snpeff
   category: analyses:variants
   flow_collection: sample
   persistence: CACHED
   description: >
     Variant annotation using snpEff package.
   input:
@@ -62,34 +62,33 @@
       re-checkrc
 
       {% for kv in known_vars_annot %}
         OUT_VCF=tmp_{{loop.index}}.vcf
         NAME=`basename {{kv.vcf.file}} .vcf.gz`
         ln -s {{ kv.vcf.file }} "${NAME}.vcf.gz"
         ln -s {{ kv.tbi.file }} "${NAME}.vcf.gz.tbi"
-        SnpSift annotate "${NAME}.vcf.gz" tmp_{{loop.index0}}.vcf > tmp_{{loop.index}}.vcf
+        SnpSift annotate "${NAME}.vcf.gz" tmp_{{loop.index0}}.vcf > "${OUT_VCF}"
         re-checkrc
       {% endfor %}
 
+      mv snpEff_genes.txt "${VAR_NAME}_snpEff_genes.txt"
+      re-save-file snpeff_genes "${VAR_NAME}_snpEff_genes.txt"
+      mv snpEff_summary.html "${VAR_NAME}_snpEff_summary.html"
+      re-save-file summary "${VAR_NAME}_snpEff_summary.html"
+
+      # Extract relevant fields from the vcf file
       {% if var_source == 'lofreq' %}
         FIELDS='CHROM POS ID REF ALT QUAL DP AF SB DP4'
       {% elif var_source == 'gatk_hc' %}
         FIELDS='CHROM POS ID REF ALT QUAL DP AF FS GEN[0].AD'
       {% endif %}
-
-      #extract relevant fields from the vcf
-      SnpSift extractFields ${OUT_VCF} ${FIELDS} "EFF[*].GENE" "EFF[*].AA" > annoFields.vcf
+      SnpSift extractFields ${OUT_VCF} ${FIELDS} "EFF[*].GENE" "EFF[*].AA" > extracted_tmp.txt
       re-checkrc
 
-      cut -f 1-11 annoFields.vcf > temp1
-      echo "EFF[*].AA" > temp2
-      awk 'FNR>1 { for(i=1;i<=NF;i++) { if($i~/p\./){printf "%s,", $i} } printf "\n"}' OFS="\t" annoFields.vcf  >> temp2
-      paste temp1 temp2 > temp3
-      # Also substitute all commas in DP4 column (10th column) with semicolons:
-      awk 'FS="\t" {gsub(",",";",$10)} OFS="\t"' temp3 > "${VAR_NAME}.finalvars.txt"
-
-      mv snpEff_genes.txt "${VAR_NAME}_snpEff_genes.txt"
-      mv snpEff_summary.html "${VAR_NAME}_snpEff_summary.html"
+      # Post-process extracted_tmp.txt
+      postprocess_snpeff.py \
+        --infile extracted_tmp.txt \
+        --var-source {{var_source}} \
+        --outfile "${VAR_NAME}.finalvars.txt"
+      re-checkrc
 
       re-save-file annotation "${VAR_NAME}.finalvars.txt"
-      re-save-file snpeff_genes "${VAR_NAME}_snpEff_genes.txt"
-      re-save-file summary "${VAR_NAME}_snpEff_summary.html"
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/hsqutils-dedup.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/hsqutils-dedup.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/variant_calling/lofreq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/variant_calling/lofreq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/plots/bamplot.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/plots/bamplot.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/plots/bamliquidator.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/plots/bamliquidator.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reports/amplicon_report.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reports/amplicon_report.yml`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 - slug: amplicon-report
   name: Amplicon report
   requirements:
     expression-engine: jinja
     executor:
       docker:
-        image: resolwebio/latex:1.0.5
+        image: resolwebio/latex:1.0.6
   data_name: "Report ({{ coverage|sample_name|default('?') }})"
-  version: 1.0.0
+  version: 1.0.1
   type: data:report:amplicon
   category: analyses:variants
   flow_collection: sample
   persistence: CACHED
   description: >
     Create amplicon report.
   input:
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/reports/amplicon_multi_report.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/reports/amplicon_multi_report.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 - slug: amplicon-archive-multi-report
   name: Archive and make multi-sample report for amplicon data
   data_name: Amplicon archive and multi-sample report
   requirements:
     expression-engine: jinja
     executor:
       docker:
-        image: resolwebio/latex:1.0.4
-  version: 0.2.1
+        image: resolwebio/latex:1.0.6
+  version: 0.2.2
   type: "data:archive:samples:amplicon"
   category: other
   persistence: TEMP
   scheduling_class: interactive
   description: >
     Create an archive of output files. The ouput folder structure is
     organized by sample slug and data object's output-field names.
@@ -111,8 +111,7 @@
 
       if [ -f multireport.tex ]; then
         # Reference source file (multireport.tex) for the debugging purposes if it exists
         re-save-file archive results.zip multireport.tex
       else
          re-save-file archive results.zip
       fi
-
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/annotation_gtf.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/annotation_gtf.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/annotation_gff3.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/annotation_gff3.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/refseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/refseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/bam_coverage.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/bam_coverage.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/annotation_bed.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/annotation_bed.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/jbrowse/bam_coverage_normalized.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/jbrowse/bam_coverage_normalized.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/gff_to_gtf.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/gff_to_gtf.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/bam_split.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/bam_split.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/refseq_compatibility.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/refseq_compatibility.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/bam_coverage.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/bam_coverage.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/prepare_geo.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/prepare_geo.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/library_strandedness.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/library_strandedness.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/processes/support_processors/archive.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/processes/support_processors/archive.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/unit/test_api.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/unit/test_tools.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/unit/test_tools.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_genome_browser.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_genome_browser.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_wgbs.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_wgbs.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_reads_filtering.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_reads_filtering.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_plots.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_plots.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_coverage.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_coverage.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_amplicon.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_amplicon.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_demultiplex.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_demultiplex.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_expression.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,58 +358,58 @@
         etcmerge = self.run_process('mergeetc', inputs)
         self.assertFile(etcmerge, "expset", "merged_etc.tab.gz", compression='gzip')
 
     @tag_process('feature_counts')
     def test_feature_counts(self):
         with self.preparation_stage():
             inputs = {
-                'src': 'annotation dicty.gtf.gz',
-                'source': 'DICTYBASE',
-                'species': 'Dictyostelium discoideum',
-                'build': 'dd-05-2009'
+                'src': 'feature_counts hs.gtf.gz',
+                'source': 'ENSEMBL',
+                'species': 'Homo sapiens',
+                'build': 'GRCh38_ens90',
             }
             annotation_gtf = self.run_process('upload-gtf', inputs)
             annotation_gff3 = self.prepare_annotation_gff()
 
             bam_single_inputs = {
                 'src': 'reads.bam',
                 'species': 'Dictyostelium discoideum',
                 'build': 'dd-05-2009'
             }
             bam_single = self.run_process('upload-bam', bam_single_inputs)
 
             inputs = {
-                'src': 'feature_counts_paired.bam',
-                'species': 'Dictyostelium discoideum',
-                'build': 'dd-05-2009'
+                'src': 'feature_counts hs_paired.bam',
+                'species': 'Homo sapiens',
+                'build': 'GRCh38_ens90',
             }
             bam_paired = self.run_process('upload-bam', inputs)
 
         inputs = {
             'alignment': {
                 'aligned_reads': bam_paired.id,
             },
             'annotation': {
                 'annotation': annotation_gtf.id,
-                'id_attribute': 'transcript_id',
+                'id_attribute': 'gene_id',
             },
             'advanced': {
                 'paired_end': {
                     'is_paired_end': True,
                     'require_both_ends_mapped': True,
                 },
             },
         }
 
         expression = self.run_process('feature_counts', inputs)
         self.assertFile(expression, 'rc', 'feature_counts_out_rc.tab.gz', compression='gzip')
         self.assertFile(expression, 'fpkm', 'feature_counts_out_fpkm.tab.gz', compression='gzip')
         self.assertFile(expression, 'exp', 'feature_counts_out_tpm.tab.gz', compression='gzip')
-        self.assertFields(expression, 'species', 'Dictyostelium discoideum')
-        self.assertFields(expression, 'build', 'dd-05-2009')
+        self.assertFields(expression, 'species', 'Homo sapiens')
+        self.assertFields(expression, 'build', 'GRCh38_ens90')
         self.assertFields(expression, 'feature_type', 'gene')
 
         inputs = {
             'alignment': {
                 'aligned_reads': bam_single.id,
             },
             'annotation': {
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_generate_report.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_generate_report.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_expression_aggregator.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_expression_aggregator.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_reads_manipulation.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_reads_manipulation.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_files_to_reads.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_files_to_reads.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_genome_coverage.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_genome_coverage.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_transmart.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_transmart.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_alignment.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_alignment.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_import.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_import.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_jbrowse.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_jbrowse.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_upload.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_upload.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_assembler.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_assembler.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_pathway_map.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_pathway_map.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_variant_calling.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_variant_calling.py`

 * *Files 3% similar despite different names*

```diff
@@ -298,28 +298,38 @@
         )
         self.assertFields(lofreq_vars, 'build', 'b37')
         self.assertFields(lofreq_vars, 'species', 'Homo sapiens')
 
     @tag_process('snpeff')
     def test_snpeff(self):
         with self.preparation_stage():
-            lf_input = {
+            variants_lf = self.run_process('upload-variants-vcf', {
                 'src': '56GSID_10k.lf.vcf',
                 'species': 'Homo sapiens',
-                'build': 'b37'
-            }
-            variants_lf = self.run_process('upload-variants-vcf', lf_input)
-            dbsnp_input = {
+                'build': 'b37',
+            })
+            variants_gatk = self.run_process('upload-variants-vcf', {
+                'src': '56GSID_10k0.gatkHC.vcf',
+                'species': 'Homo sapiens',
+                'build': 'b37',
+            })
+            dbsnp = self.run_process('upload-variants-vcf', {
                 'src': 'dbsnp_138.b37.chr2_small.vcf.gz',
                 'species': 'Homo sapiens',
-                'build': 'b37'
-            }
-            dbsnp = self.run_process('upload-variants-vcf', dbsnp_input)
+                'build': 'b37',
+            })
 
-        inputs = {
+        final_var_lf = self.run_process('snpeff', {
             'variants': variants_lf.id,
             'known_vars_annot': [dbsnp.id],
-            'var_source': 'lofreq'
-        }
-
-        final_var_lf = self.run_process('snpeff', inputs)
+            'var_source': 'lofreq',
+        })
         self.assertFile(final_var_lf, 'annotation', '56GSID.lf.finalvars.txt')
+        # pylint: disable=deprecated-method
+        self.assertRegex(final_var_lf.process_warning[0], r'Inconsistency for entry .*')
+
+        final_var_gatk = self.run_process('snpeff', {
+            'variants': variants_gatk.id,
+            'known_vars_annot': [dbsnp.id],
+            'var_source': 'gatk_hc',
+        })
+        self.assertFile(final_var_gatk, 'annotation', '56GSID.gatk.finalvars.txt')
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_chipseq.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_chipseq.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_enrichment.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_enrichment.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_processor.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_processor.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_microarray.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_microarray.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_pca.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_pca.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_support_processors.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_support_processors.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_clustering.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_clustering.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/processes/test_diff_expression.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/processes/test_diff_expression.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_wgbs.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_wgbs.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_amplicon.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_amplicon.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_chemut.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_chemut.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_rna_seq.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_rna_seq.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_mirna.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_mirna.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_heat_seq.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_heat_seq.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/workflows/test_chip_seq.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/workflows/test_chip_seq.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bt2_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bt2_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs14_control.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs14_control.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/HS chr21_ensembl.fa.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/HS chr21_ensembl.fa.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/expressions-py3.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/expressions-py3.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_filtering.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_filtering.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G_masterfile_corrupted.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G_masterfile_corrupted.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/00Hr.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/00Hr.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_fw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_fw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bed_track.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bed_track.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem.fa.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem.fa.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/s_1_2.qseq.small.txt.bz2` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/s_1_2.qseq.small.txt.bz2`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/features.tab` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/features.tab`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_prinseq_single.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_prinseq_single.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/silva-arc-23s-id98.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/silva-arc-23s-id98.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_trimmomatic_single.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_trimmomatic_single.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_fastqmcf_single.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_fastqmcf_single.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_sw_paired_reads_mapped.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_sw_paired_reads_mapped.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1_transformed.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1_transformed.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_expressions_1.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_expressions_1.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/4-cuffquant.cxb` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/4-cuffquant.cxb`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.gatkHC.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.gatkHC.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/fw reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/fw reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L001_R2_001.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L001_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/3-cuffquant.cxb` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/3-cuffquant.cxb`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/.DS_Store` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/.DS_Store`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_wo_rRNA_paired_forw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_wo_rRNA_paired_forw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sp_test.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sp_test.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56gsid_10k.targetPCRmetrics.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56gsid_10k.targetPCRmetrics.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/s_1_1.qseq.small.txt.bz2` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/s_1_1.qseq.small.txt.bz2`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_unmapped_1.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_unmapped_1.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/prepare_geo_RNA-Seq.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/prepare_geo_RNA-Seq.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/dbsnp_138.b37.chr2_small.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/dbsnp_138.b37.chr2_small.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_master_file_olapfreebed.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_master_file_olapfreebed.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ncRNA_sample2.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ncRNA_sample2.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/box_plot.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/box_plot.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_expressions_3.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_expressions_3.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/paired_end_forward.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/paired_end_forward.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Test_S1_L002_R1_001.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Test_S1_L002_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate1.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/subread_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/subread_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/igv_human.lf.vcf` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/igv_human.lf.vcf`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs14_case.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs14_case.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/expressions-py2.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/expressions-py2.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_paired_abyss_1.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_paired_abyss_1.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_genes.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_genes.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding_transformed_R2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding_transformed_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G_masterfile_170113.txt.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G_masterfile_170113.txt.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/SRR2124780_2 1k.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/SRR2124780_2 1k.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/features_update.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/features_update.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA forw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA forw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/workflow_bbduk_star test.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/workflow_bbduk_star test.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot_ alignment1.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot_ alignment1.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ncRNA_sample1.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ncRNA_sample1.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rose2_enhancer_table.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rose2_enhancer_table.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Mills_and_1000G_gold_standard.indels.b37.chr22_small.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Mills_and_1000G_gold_standard.indels.b37.chr22_small.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/prepare_geo_ChIP-Seq.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/prepare_geo_ChIP-Seq.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L002_R1_001.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L002_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k_mate2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k_mate2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk test reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk test reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_wo_rRNA_paired_rew.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_wo_rRNA_paired_rew.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_trimmed_mate1.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_trimmed_mate1.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rw reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rw reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/SRR2124780_1 1k.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/SRR2124780_1 1k.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA_rew.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA_rew.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.gatkHC4.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.gatkHC4.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cufflinks_transcripts.gtf` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cufflinks_transcripts.gtf`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_b37_chr22_frag.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_b37_chr22_frag.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k_mate1.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k_mate1.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_paired_R2 workflow_bbduk_star_htseq.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_paired_R2 workflow_bbduk_star_htseq.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_hisat2_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_hisat2_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_subread_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_subread_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding_transformed.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding_transformed.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mouse_genes.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mouse_genes.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/deseq2_output.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/deseq2_output.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_capture_targets.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_capture_targets.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/deseq2_volcano_plot.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/deseq2_volcano_plot.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_rw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_trimmomatic_paired_rw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_mate1_paired_filtered.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_mate1_paired_filtered.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mappings_gsea.tab.zip` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mappings_gsea.tab.zip`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/etc-py3.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/etc-py3.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_pseudoaligner.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_pseudoaligner.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/features_gsea.tab.zip` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/features_gsea.tab.zip`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56G_masterfile_test.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56G_masterfile_test.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/fw reads_2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/fw reads_2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_wo_rRNA_single.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_wo_rRNA_single.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset-py2.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset-py2.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1_R2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_paired_report.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_paired_report.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffquant_1.cxb` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffquant_1.cxb`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_dm6.bam.bai` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_dm6.bam.bai`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_bwa_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_bwa_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_mm10.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_mm10.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/dbsnp_138.b37.chr22_small.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/dbsnp_138.b37.chr22_small.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/etc-py2.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/etc-py2.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset_out.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset_out.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding_R2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/3ptrim_new56Gprimers.fa.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/3ptrim_new56Gprimers.fa.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot.gff` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot.gff`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffquant_2.cxb` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffquant_2.cxb`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chemut_genome.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chemut_genome.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/seq_reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/seq_reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA_forw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA_forw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mm10_header.sam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mm10_header.sam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_master_file_nomergebed.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_master_file_nomergebed.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Test_S1_L001_R1_001.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Test_S1_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads_paired_abyss_2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads_paired_abyss_2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.read3.small.qseq.bz2` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.read3.small.qseq.bz2`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_paired_R1 workflow_bbduk_star_htseq.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_paired_R1 workflow_bbduk_star_htseq.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_fw_reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_fw_reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_samtools.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_samtools.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_position_sorted.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_position_sorted.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_summary.html` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k.gatkHC_snpEff_summary.html`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_b37_chr2_small.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_b37_chr2_small.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L002_R2_001.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L002_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/go_genesets.mgi.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/go_genesets.mgi.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_bt_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_bt_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.lf.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.lf.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chr1_part.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chr1_part.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/wgbs.bam_stat.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/wgbs.bam_stat.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ontology_dicty_cropped.obo.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ontology_dicty_cropped.obo.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_prinseq_paired_fw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_prinseq_paired_fw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hisat2_unmapped_2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hisat2_unmapped_2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/etc_upload_input.xls` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/etc_upload_input.xls`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_trimmed_mate2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/paired_end_reverse.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/paired_end_reverse.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/alignment_name_sorted.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/alignment_name_sorted.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_probe_info.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_probe_info.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/variant_calling_filtered_variants.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/variant_calling_filtered_variants.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/5ptrim_new56Gprimers.fa.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/5ptrim_new56Gprimers.fa.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mappings.tab.zip` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mappings.tab.zip`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_master_file_merged.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_master_file_merged.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/CM_mate1.fq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/CM_mate1.fq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/seq_reads_fastqc.zip` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/seq_reads_fastqc.zip`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/adapters.fasta` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/adapters.fasta`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ontology_mus_cropped.obo.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ontology_mus_cropped.obo.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Jbrowse_genome_coverage.bw` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Jbrowse_genome_coverage.bw`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/AX4_mate1.fq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/AX4_mate1.fq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/ncRNA_genome.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/ncRNA_genome.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/silva-arc-16s-id95.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/silva-arc-16s-id95.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/demultiplexed_reads_rw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/demultiplexed_reads_rw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_rw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_rw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/feature_counts_detect_strandedness.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/feature_counts_detect_strandedness.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffquant_mapping.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffquant_mapping.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_dm6.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_dm6.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1_transformed_R2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1_transformed_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_mate1.fq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_mate1.fq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_aligment.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_aligment.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_expressions_2.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_expressions_2.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cuffmerge_transcripts.gtf` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cuffmerge_transcripts.gtf`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat-seq.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat-seq.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamliquidator_summary.html` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamliquidator_summary.html`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/go_enriched_terms_dicty.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/go_enriched_terms_dicty.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hybrid_mm10.bam.bai` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hybrid_mm10.bam.bai`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/macs14_chr22.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/macs14_chr22.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chr21_small.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chr21_small.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/mm10_small.gtf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/mm10_small.gtf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.read2.small.qseq.bz2` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.read2.small.qseq.bz2`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/geneset-py2.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/geneset-py2.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bwa_sw_reads_mapped.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bwa_sw_reads_mapped.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/6-cuffquant.cxb` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/6-cuffquant.cxb`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/reads.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/reads.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_adapters.fasta` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_adapters.fasta`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/log_box_plot.json.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/log_box_plot.json.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_probe_info.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_probe_info.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chip_seq_control.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chip_seq_control.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/20Hr.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/20Hr.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bbduk_rv_reads.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bbduk_rv_reads.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_prinseq_paired_rw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_prinseq_paired_rw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/amplicon_primers.bed` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/amplicon_primers.bed`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rose2_test.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rose2_test.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/HSQUtils_dedup_summary.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/HSQUtils_dedup_summary.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs genome.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs genome.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/chip_seq_case.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/chip_seq_case.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bt_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bt_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_fw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/filtered_reads_fastqmcf_paired_fw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/bamplot_alignment.bam` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/bamplot_alignment.bam`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/AX4_mate2.fq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/AX4_mate2.fq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k.lf.vcf` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k.lf.vcf`

 * *Files 8% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 ##INFO=<ID=HRUN,Number=1,Type=Integer,Description="Homopolymer length to the right of report indel position">
 ##FILTER=<ID=min_dp_10,Description="Minimum Coverage 10">
 ##FILTER=<ID=sb_fdr,Description="Strand-Bias Multiple Testing Correction: fdr corr. pvalue > 0.001000">
 ##FILTER=<ID=min_snvqual_41,Description="Minimum SNV Quality (Phred) 41">
 ##FILTER=<ID=min_indelqual_24,Description="Minimum Indel Quality (Phred) 24">
 #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
 2	1640	.	A	AC	710	PASS	DP=114;AF=0.236842;SB=4;DP4=46,41,11,16;INDEL;HRUN=8
+2	1640	.	A	AC,ACC	710	PASS	DP=114;AF=0.236842,0.42;SB=4;DP4=46,41,11,16;INDEL;HRUN=8
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/human_genes.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/human_genes.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/demultiplexed_reads_fw.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/demultiplexed_reads_fw.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/old_encoding1.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/old_encoding1.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/dicty_genes.tab.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/dicty_genes.tab.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/1000G_phase1.indels.b37_chr2_small.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/1000G_phase1.indels.b37_chr2_small.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/my.strange.genome name$.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/my.strange.genome name$.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/sp_test_compatibility_report.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/sp_test_compatibility_report.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/gff_to_gtf_annotation.gtf` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/gff_to_gtf_annotation.gtf`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_rsem_bt2_index.tar.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_rsem_bt2_index.tar.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hsqutils_reads_mate2_paired_filtered.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hsqutils_reads_mate2_paired_filtered.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/wgbs.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/wgbs.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/CM_mate2.fq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/CM_mate2.fq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cDNA_reference.fasta.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cDNA_reference.fasta.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/TestPaired_S1_L001_R1_001.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/TestPaired_S1_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/5-cuffquant.cxb` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/5-cuffquant.cxb`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_1k_mate1.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_1k_mate1.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/pool24.read1.small.qseq.bz2` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/pool24.read1.small.qseq.bz2`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/Jbrowse_norm_genome_coverage.bw` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/Jbrowse_norm_genome_coverage.bw`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hg19_chr20_small.gtf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hg19_chr20_small.gtf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/cutadapt_trimmed_mate2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/cutadapt_trimmed_mate2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/genome_coverage.bw` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/genome_coverage.bw`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/heat_seq_mate2.fq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/heat_seq_mate2.fq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/hs_single bbduk_star_htseq_reads_single.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/hs_single bbduk_star_htseq_reads_single.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/s_1_3.qseq.small.txt.bz2` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/s_1_3.qseq.small.txt.bz2`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rRNA_forw_single.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rRNA_forw_single.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/rw reads_2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/rw reads_2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/56GSID_10k_mate2.fastq.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/56GSID_10k_mate2.fastq.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/exons_coverage.txt.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/exons_coverage.txt.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/files/igv_human.lf.vcf.gz` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/files/igv_human.lf.vcf.gz`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/tests/commands/test_generators.py` & `resolwe-bio-9.0.0a4/resolwe_bio/tests/commands/test_generators.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_geneset.py` & `resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_geneset.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_samples.py` & `resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_samples.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_diffexpr_deseq.py` & `resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_diffexpr_deseq.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_diffexpr_cuffdiff.py` & `resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_diffexpr_cuffdiff.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/management/commands/utils.py` & `resolwe-bio-9.0.0a4/resolwe_bio/management/commands/utils.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/management/commands/generate_etc.py` & `resolwe-bio-9.0.0a4/resolwe_bio/management/commands/generate_etc.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/utils/test.py` & `resolwe-bio-9.0.0a4/resolwe_bio/utils/test.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/extensions.py` & `resolwe-bio-9.0.0a4/resolwe_bio/extensions.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/bbduk-star-featurecounts.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/bbduk-star-featurecounts.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/sample_detailed.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/sample_detailed.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/sample_vaccinesurvey.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/sample_vaccinesurvey.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/diffexp.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/diffexp.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/bcm.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/bcm.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/rnaseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/rnaseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/reads.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/reads.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/transmart.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/transmart.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/reads_detailed.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/reads_detailed.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/amplicon.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/amplicon.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/sample_geo.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/sample_geo.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/etc.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/etc.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/cutadapt-star-htseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/cutadapt-star-htseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/microarray_affy.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/microarray_affy.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/descriptors/bbduk-star-htseq.yml` & `resolwe-bio-9.0.0a4/resolwe_bio/descriptors/bbduk-star-htseq.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/assets/logo_genialis.pdf` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/assets/logo_genialis.pdf`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/latex/assets/template_amplicon_report_multi_sample.tex` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/latex/assets/template_amplicon_report_multi_sample.tex`

 * *Files 4% similar despite different names*

```diff
@@ -119,25 +119,24 @@
 {\captionof{table}{Legend}
 \noindent
 \rowcolors{2}{gray2}{white}
 \begin{oldlongtable}[l]{l W}
 \rowcolor{gray2}
 CHROM & Chromosome\\
 POS & Position\\
-ID & Variant identity\\
 REF & Reference base\\
 ALT & Alternative base (i.e., variant)\\
-QUAL & Phred-scaled quality score for the assertion made in ALT. i.e. -10log10 prob(call in ALT is wrong)\\
+AF & Allele frequency, also called "variant frequency". For the GATK caller, empirical AF is computed as the ratio of allele depth (AD) to read depth (DP). LoFreq similarly computes AF as the frequency of variant reads. \\
 DP & Filtered read depth\\
-AF & Allele frequency\\
-FS & FisherStrand (Phred-scaled p-value using Fisher's Exact Test to detect strand bias (the variation being seen on only the forward or only the reverse strand) in the reads.  More bias is indicative of false positive calls. Be wary of SNP with FS > 60.0 and an indel with FS > 200.0.)\\
 AD & Allele depth\\
-GENE & Affected gene\\
-SB & Strand bias\\
+FS & FisherStrand (Phred-scaled p-value using Fisher's Exact Test to detect strand bias (the variation being seen on only the forward or only the reverse strand) in the reads.  More bias is indicative of false positive calls. Be wary of SNP with FS > 60.0 and an indel with FS > 200.0.)\\
 DP4 & Number of 1) forward ref alleles; 2) reverse ref; 3) forward non-ref; 4) reverse non-ref alleles, used in variant calling. Sum can be smaller than DP because low-quality bases are not counted.\\
+SB & Strand bias\\
+GENE & Affected gene\\
+ID & Variant identity\\
 AA & Amino acid change\\
 \end{oldlongtable}
 {
 \addtocounter{table}{-1}}}
 \newpage
 
 {{#VCF_TABLES#}}
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/r-packages.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/r-packages.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-manual/snpeff.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-manual/snpeff.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/dnaseq/packages-python3.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/dnaseq/packages-python3.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/jbrowse.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/jbrowse.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/r-packages.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/r-packages.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/snpeff.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/snpeff.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-manual/hsqutils.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-manual/hsqutils.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-debian.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-debian.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/legacy/packages-python2.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/legacy/packages-python2.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-manual/wigtobigwig.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-manual/wigtobigwig.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/chipseq/packages-python2.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/chipseq/packages-python2.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-manual/sra-toolkit.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-manual/sra-toolkit.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/utils/packages-python3.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/utils/packages-python3.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/trimmomatic.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/trimmomatic.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-manual/r-packages.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-manual/r-packages.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/packages-python3.txt` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/packages-python3.txt`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/rnaseq/README.md` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/rnaseq/README.md`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-16.04` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-16.04`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/common.sh` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/common.sh`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-17.10` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-17.10`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-18.04` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-18.04`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/README.md` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/README.md`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/docker_images/base/Dockerfile.ubuntu-14.04` & `resolwe-bio-9.0.0a4/resolwe_bio/docker_images/base/Dockerfile.ubuntu-14.04`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/__about__.py` & `resolwe-bio-9.0.0a4/resolwe_bio/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #       interfere with a global variable __name__ denoting object's name.
 __title__ = 'resolwe-bio'
 __summary__ = 'Bioinformatics pipelines for the Resolwe platform'
 __url__ = 'https://github.com/genialis/resolwe-bio'
 
 # Semantic versioning is used. For more information see:
 # https://packaging.python.org/en/latest/distributing/#semantic-versioning-preferred
-__version__ = '9.0.0a3'
+__version__ = '9.0.0a4'
 
 __author__ = 'Genialis d.o.o.'
 __email__ = 'dev-team@genialis.com'
 
 __license__ = 'Apache License (2.0)'
 __copyright__ = '2015-2018, ' + __author__
```

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/expression_filters/sample.py` & `resolwe-bio-9.0.0a4/resolwe_bio/expression_filters/sample.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/resolwe_bio/filters.py` & `resolwe-bio-9.0.0a4/resolwe_bio/filters.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/tests/settings.py` & `resolwe-bio-9.0.0a4/tests/settings.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/tests/fixtures/data.yaml` & `resolwe-bio-9.0.0a4/tests/fixtures/data.yaml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/tests/fixtures/collection.yaml` & `resolwe-bio-9.0.0a4/tests/fixtures/collection.yaml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/tests/docker-compose.yml` & `resolwe-bio-9.0.0a4/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/tests/urls.py` & `resolwe-bio-9.0.0a4/tests/urls.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/MANIFEST.in` & `resolwe-bio-9.0.0a4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/docs/contributing.rst` & `resolwe-bio-9.0.0a4/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/docs/conf.py` & `resolwe-bio-9.0.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/docs/proc.rst` & `resolwe-bio-9.0.0a4/docs/proc.rst`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/docs/catalog-types.rst` & `resolwe-bio-9.0.0a4/docs/catalog-types.rst`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/docs/CHANGELOG.rst` & `resolwe-bio-9.0.0a4/docs/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,25 +40,32 @@
 - Add ``template_amplicon_report.tex`` to ``resolwebio/latex`` Docker image
   assets
 - Add SnpEff tool and bokeh assets to ``resolwebio/dnaseq`` Docker image
 - Add automated library strand detection to ``feature_counts`` quantification process
 - Add FastQC option ``nogroup`` to ``bbduk-single`` and ``bbduk-paired`` processes
 - Add CPM normalization to ``htseq-count-raw`` process
 - Add ``workflow-bbduk-star-htseq-paired``
+- Add legend to amplicon report template in ``resolwebio/latex`` Docker image
 
 Fixed
 -----
 - Fix manual installation of packages in Docker images to handle dots and
   spaces in file names correctly
 - Fix COSMIC url template in ``amplicon-table`` process
 - Fix Create IGV session in Archive samples process
 - Fix ``source`` tracking in ``cufflinks`` and ``cuffquant`` processes
 - Fix amplicon master file validation script. Check and report error if
   duplicated amplicon names are included. Validation will now pass also
   for primer sequences in lowercase.
+- Fix allele frequency (AF) calculation in ``snpeff`` process
+- Fix bug in script for calculating FPKM. Because genes of raw counts from
+  ``featureCounts`` were not lexicographically sorted, division of normalized counts
+  was done with values from other, incorrect, genes. Results from ``featureCounts``,
+  but not ``HTSeq-count`` process, were affected.
+
 
 
 ==================
 8.1.0 - 2018-04-13
 ==================
 
 Changed
```

### Comparing `resolwe-bio-9.0.0a3/docs/descriptor.rst` & `resolwe-bio-9.0.0a4/docs/descriptor.rst`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/setup.py` & `resolwe-bio-9.0.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/tox.ini` & `resolwe-bio-9.0.0a4/tox.ini`

 * *Files identical despite different names*

### Comparing `resolwe-bio-9.0.0a3/README.rst` & `resolwe-bio-9.0.0a4/README.rst`

 * *Files identical despite different names*

