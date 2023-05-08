# Comparing `tmp/cg-29.8.1.tar.gz` & `tmp/cg-29.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cg-29.8.1.tar", last modified: Mon May  8 11:52:01 2023, max compression
+gzip compressed data, was "dist/cg-29.8.2.tar", last modified: Mon May  8 12:13:23 2023, max compression
```

## Comparing `cg-29.8.1.tar` & `cg-29.8.2.tar`

### file list

```diff
@@ -1,1245 +1,1245 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 11:51:46.000000 cg-29.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-08 11:52:01.000000 cg-29.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-08 11:51:46.000000 cg-29.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 11:51:46.000000 cg-29.8.1/cg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/crud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/crud/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/crud/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/crud/find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/cgstats/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/cgstats/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/support_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/unaligned.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/db/models/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/demux_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/dragen_demux_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/parsers/adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/parsers/conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/parsers/demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/parsers/quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/parsers/run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/cgstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/crunchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/crunchy/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/crunchy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/crunchy/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/demux_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sample_sheet/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/hermes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/hermes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/hermes/hermes_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/hermes/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17538 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/housekeeper/hk.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/housekeeper/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/invoice/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/invoice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/lims/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/lims/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/lims/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/lims/samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/loqus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/madeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/madeline/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/mip/confighandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/orderform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/orderform/excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/orderform/json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/orderform/orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/scout/scout_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/scout/scoutapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/slurm/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/slurm/slurm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/apps/tb/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/tb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/tb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/tb/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-08 11:51:46.000000 cg-29.8.1/cg/apps/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/compress/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/compress/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/compress/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/delete/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/delete/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/delete/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/delete/observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/deliver/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/demultiplex/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/demultiplex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/demultiplex/demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/demultiplex/finish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/demultiplex/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/demultiplex/sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/generate/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/generate/report/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/generate/report/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/generate/report/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/set/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/set/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/set/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/store/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/store/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/clinical_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/fohm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/nipt/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/nipt/ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/nipt/statina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/upload/observations/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/observations/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/observations/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/balsamic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/balsamic/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/balsamic/pon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/balsamic/qc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/balsamic/umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/fastq/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/fluffy/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/microsalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/microsalt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mip/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mip/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/mip_dna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mip_dna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mip_dna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/mip_rna/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mip_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mip_rna/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/mutant/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mutant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/mutant/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/nextflow/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/rnafusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/rnafusion/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/taxprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/taxprofiler/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/cli/workflow/tower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/tower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 11:51:46.000000 cg-29.8.1/cg/cli/workflow/tower/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/cgstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/demultiplexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/gene_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/housekeeper_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/orderforms.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/pdc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/sample_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/scout_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/sequencing.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 11:51:46.000000 cg-29.8.1/cg/constants/tb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-08 11:51:46.000000 cg-29.8.1/cg/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 11:51:46.000000 cg-29.8.1/cg/io/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-08 11:51:46.000000 cg-29.8.1/cg/io/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-08 11:51:46.000000 cg-29.8.1/cg/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-08 11:51:46.000000 cg-29.8.1/cg/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 11:51:46.000000 cg-29.8.1/cg/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/archive/ddn_dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/backup/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/backup/pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/clean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/clean/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/clean/demultiplexed_flow_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/clean/flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/compress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/compress/compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/compress/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/deliver_ticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/demultiplex/delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/demultiplex/demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/demultiplex/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/encryption/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/observations/balsamic_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/observations/mip_dna_observations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/observations/observations_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/balsamic_qc_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/balsamic_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/balsamic_umi_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/case_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/fastq_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/fluffy_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/lims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/metagenome_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/microbial_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/microsalt_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/mip_dna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/mip_rna_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/pool_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/rml_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/sars_cov_2_submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/orders/ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/templates/balsamic_report.html
--rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/templates/bootstrap.html
--rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/report/templates/mip-dna_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/rsync/rsync_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/rsync/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/tar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/tar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/tar/tar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/transfer/external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/transfer/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/transfer/lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/balsamic/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/fohm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/fohm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/fohm/fohm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/gisaid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/gisaid/gisaid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/gisaid/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/gt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/mip/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/mip/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/nipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/nipt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/nipt/nipt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/rnafusion/rnafusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/balsamic_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/balsamic_umi_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/hk_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/mip_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/rnafusion_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/scout/uploadscoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/upload/vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/balsamic_pon.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/balsamic_qc.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/balsamic_umi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/fluffy.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/mip_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/mip_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/mutant.py
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/nextflow_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/prepare_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/rnafusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/taxprofiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-08 11:51:46.000000 cg-29.8.1/cg/meta/workflow/tower_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/balsamic/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/balsamic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/balsamic/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/cg_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/cgstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/cgstats/flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/cgstats/stats_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/compression_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/deliverables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/deliverables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/deliverables/metric_deliverables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/demultiplex/demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/demultiplex/flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/demultiplex/run_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/demultiplex/sbatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/file_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/invoice/invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/lims/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/lims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/lims/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/mip/mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/mip/mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/mip/mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/mip/mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/nextflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/nextflow/deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/nextflow/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/observations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/observations/input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/orders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/excel_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/json_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/orderform_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/sample_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/orders/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/report/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/report/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/report/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/rnafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/rnafusion/rnafusion_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/scout/scout_load_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/slurm/sbatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/taxprofiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/models/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-08 11:51:46.000000 cg-29.8.1/cg/models/workflow/mutant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-08 11:51:46.000000 cg-29.8.1/cg/resources/20181012_Indices.csv
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 11:51:46.000000 cg-29.8.1/cg/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-08 11:51:46.000000 cg-29.8.1/cg/resources/rnafusion_bundle_filenames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/server/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/invoices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/server/invoices/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/server/invoices/templates/invoices/
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/invoices/templates/invoices/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/invoices/templates/invoices/invoice.html
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/invoices/templates/invoices/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/invoices/templates/invoices/new.html
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/invoices/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/server/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/server/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 11:51:46.000000 cg-29.8.1/cg/server/templates/admin/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/store/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    32042 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    39247 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_analysis_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_case_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/filters/status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    30042 2023-05-08 11:51:46.000000 cg-29.8.1/cg/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/utils/checksum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/checksum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/checksum/checksum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/utils/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/click/EnumChoice.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg/utils/flask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/flask/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-08 11:51:46.000000 cg-29.8.1/cg/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39785 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 11:52:00.000000 cg-29.8.1/cg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-08 11:51:46.000000 cg-29.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-08 11:51:46.000000 cg-29.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:52:01.000000 cg-29.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-08 11:51:46.000000 cg-29.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/cgstats/
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/cgstats/crud/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/crud/test_create_novaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/crud/test_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/cgstats/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/parsers/test_adapter_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/parsers/test_conversion_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/parsers/test_demux_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/parsers/test_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/parsers/test_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/test_cgstats_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/cgstats/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/coverage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/coverage/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/crunchy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/crunchy/test_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/crunchy/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/crunchy/test_crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/crunchy/test_spring_decompression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/demultiplex/test_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/demultiplex/test_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/gens/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/gens/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/gens/test_gens_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/gt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/gt/test_gt_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/hk/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/hk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/hk/test__getattr__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/hk/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/hk/test_bundles.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/hk/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/hk/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/hk/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/lims/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/lims/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/lims/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/loqus/
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/loqus/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/loqus/test_loqusdb_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/madeline/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/madeline/test_madeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/mip/test_config_mip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/mutacc_auto/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/mutacc_auto/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/mutacc_auto/test_mutacc_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/orderform/
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/orderform/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/orderform/test_excel_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/orderform/test_excel_sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/orderform/test_json_orderform_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/orderform/test_orderform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/scout/test_get_causative_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/scout/test_get_scout_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/scout/test_scout_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/scout/test_scout_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/slurm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/slurm/test_slurm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/test_apps_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/test_osticket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/apps/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-08 11:51:46.000000 cg-29.8.1/tests/apps/vogue/test_vogue_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/add/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/add/test_cli_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/add/test_cli_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/add/test_cli_add_family.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/add/test_cli_add_relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/add/test_cli_add_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/backup/test_backup_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/clean/test_balsamic_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/clean/test_clean_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/clean/test_hk_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/clean/test_hk_case_bundle_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/clean/test_microbial_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/clean/test_rsync_past_run_dirs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/compress/
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/compress/test_cli_compress_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/compress/test_cli_decompress_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/compress/test_compress_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/compress/test_store_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/delete/test_cli_delete_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/delete/test_cli_delete_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/deliver/test_deliver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/deliver/test_rsync_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/deliver/test_run_deliver_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/test_add_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/test_create_sample_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/test_demultiplex_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/test_finish_demux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/test_stats_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/demultiplex/test_validate_sample_sheet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/generate/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/generate/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/generate/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/generate/report/test_cli_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/generate/report/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/generate/test_cli_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/get/test_cli_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/get/test_cli_get_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/get/test_cli_get_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/get/test_cli_get_flow_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/get/test_cli_get_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/set/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/set/test_cli_set_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/set/test_cli_set_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/set/test_cli_set_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/set/test_cli_set_list_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/set/test_cli_set_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/set/test_cli_set_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/store/
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/store/test_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/test_cli_status_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/cli/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_scout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_genotype.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_gens.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_nipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_nipt_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_nipt_statina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/upload/test_cli_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)    31891 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15354 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/balsamic/test_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/balsamic/test_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/balsamic/test_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/balsamic/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/balsamic/test_store_housekeeper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fastq/test_fastq_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/fluffy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fluffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fluffy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fluffy/test_cli_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fluffy/test_cli_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fluffy/test_cli_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/fluffy/test_cli_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/microsalt/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/microsalt/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/microsalt/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/microsalt/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/microsalt/test_microsalt_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/cli/workflow/taxprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/taxprofiler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/test_cli_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-08 11:51:46.000000 cg-29.8.1/tests/cli/workflow/test_cli_workflow_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)    64049 2023-05-08 11:51:46.000000 cg-29.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/DEMUX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/analysis/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/analysis/balsamic/tn_wgs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/analysis/microsalt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
--rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/analysis/mip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/ADM2.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/ADM3.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/adm1.cram
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/adm1.mt.bam
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/multiqc.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/report.pdf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/smn.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/snv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/snv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/str.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/sv.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/sv_research.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/analysis/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/rnafusion/multiqc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/analysis/sample_coverage.bed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/balsamic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/balsamic/case/
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/balsamic/case/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/balsamic/case/metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/balsamic/case/metadata_directory.yml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/crunchy/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/crunchy/spring_metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
--rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/hiseq_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/
--rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/fluffy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/fluffy/2020-23219-05/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/fluffy/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/fluffy/deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/fluffy/multiqc_report.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/fluffy/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/gt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/gt/yellowhog.bcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/madeline/
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/madeline/madeline.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/mip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/case_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/
--rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
--rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/store/
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/store/case_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/mip/sample_file.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/scout/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/scout/643594.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/scout/case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/scout/export_causatives.json
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/scout/none_case_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/scout/other_sex_case.json
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/scout/panel_export.bed
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/scout/panel_export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/apps/shipping/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/apps/shipping/scout-deploy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/cgweb_orders/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/balsamic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/fastq.json
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/metagenome.json
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/microsalt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/mip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/mip_rna.json
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/rml.json
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/cgweb_orders/sarscov2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/data/SampleSheet.csv
--rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/data/cgfixture.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/data/fastq.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/data/hkstore.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/data/yellowhog/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/data/yellowhog/pedigree.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/io/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/io/example_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/io/example_json.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/orderforms/
--rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1508.27.fastq.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1508.27.mip.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1603.11.microbial.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1604.15.rml.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/NIPT-json.json
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/fixtures/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/report/case_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/report/lims_exported_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-08 11:51:46.000000 cg-29.8.1/tests/fixtures/report/lims_family.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-08 11:51:46.000000 cg-29.8.1/tests/io/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-08 11:51:46.000000 cg-29.8.1/tests/io/test_io_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-08 11:51:46.000000 cg-29.8.1/tests/io/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-08 11:51:46.000000 cg-29.8.1/tests/io/test_io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-08 11:51:46.000000 cg-29.8.1/tests/io/test_io_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/archive/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/archive/test_archiving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/backup/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24603 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/backup/test_meta_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/backup/test_meta_pdc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/clean/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/clean/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/clean/test_clean_demultiplexed_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/clean/test_clean_flow_cell_run_directories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/compress/
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/compress/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/compress/test_clean_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/compress/test_compress_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/compress/test_compress_meta_fastq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/compress/test_decompress_spring_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/compress/test_meta_compress_update_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/deliver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/deliver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/deliver/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/deliver/test_deliver_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/deliver/test_delivery_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/demultiplex/
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/demultiplex/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/demultiplex/test_delete_demultiplex_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/demultiplex/test_demux_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/demultiplex/test_rename_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/encryption/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/encryption/test_encryption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/observations/test_meta_upload_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/orders/
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_PoolSubmitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_meta_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_meta_orders_lims.py
--rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_meta_orders_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/orders/test_ticket_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/report/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/report/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/report/test_balsamic_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/report/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/report/test_mip_dna_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/report/test_report_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/rsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/rsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/rsync/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/rsync/test_rsync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/test_invoice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/transfer/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/transfer/test_external_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/transfer/test_meta_transfer_flowcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/transfer/test_meta_transfer_lims.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/balsamic/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/gisaid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/gisaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/gisaid/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/gisaid/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/gisaid/fixtures/four_samples.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/mutacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/mutacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/mutacc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/nipt/
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/nipt/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/nipt/test_nipt_upload_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/scout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/scout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/scout/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/scout/test_generate_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    32161 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/scout/test_scout_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/test_meta_upload_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/test_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/test_upload_genotypes_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/upload/vogue/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/vogue/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/upload/vogue/test_upload_vogue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/meta/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/workflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/workflow/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/workflow/test_balsamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/workflow/test_microsalt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-08 11:51:46.000000 cg-29.8.1/tests/meta/workflow/test_prepare_fastq_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/balsamic_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/crunchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/hk_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/limsmock.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/madeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/mip_analysis_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/osticket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/process_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/scout.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/store_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-08 11:51:46.000000 cg-29.8.1/tests/mocks/tb_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/balsamic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/balsamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/balsamic/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/balsamic/test_balsamic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/demultiplexing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/demultiplexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/demultiplexing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/demultiplexing/test_demux_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/demultiplexing/test_flowcell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/demultiplexing/test_run_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/mip/
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/mip/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/mip/test_mip_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/mip/test_mip_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/mip/test_mip_metrics_deliverables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/mip/test_mip_sample_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/nextflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/nextflow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/nextflow/test_nextflow_deliver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/observations/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/observations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/observations/test_observations_input_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/report/test_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/models/rnafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/rnafusion/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/rnafusion/test_rnafusion_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/test_cg_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/test_compression_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/test_file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-08 11:51:46.000000 cg-29.8.1/tests/models/test_flowcell_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/server/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 11:51:46.000000 cg-29.8.1/tests/server/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 11:51:46.000000 cg-29.8.1/tests/server/test_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 11:51:46.000000 cg-29.8.1/tests/server/test_server_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-08 11:51:46.000000 cg-29.8.1/tests/small_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/store/api/add/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/add/test_store_add_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/add/test_store_add_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/add/test_store_add_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/add/test_store_add_flow_celll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19418 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/store/api/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/delete/test_store_api_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/store/api/find/
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/find/test_find_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/find/test_find_basic_data_application_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/find/test_find_business_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/find/test_find_business_data_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/find/test_find_business_data_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/find/test_find_business_data_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/store/api/status/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_analyses_to_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_analyses_to_delivery_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_store_api_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_store_api_status_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_store_api_status_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_store_api_status_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_store_api_status_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/status/test_store_api_status_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/api/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_analyses_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_application_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_application_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_bed_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_bed_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_case_sample_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    39481 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_cases_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_collaboration_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_customer_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_flow_cell_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_invoice_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_organism_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_panel_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_pool_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_samples_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/filters/test_status_user_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/test_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-05-08 11:51:46.000000 cg-29.8.1/tests/store_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 11:51:46.000000 cg-29.8.1/tests/test_store_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/tests/fixtures/apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/tests/fixtures/apps/demultiplexing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:00.000000 cg-29.8.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/tests/fixtures/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/tests/fixtures/data/fastq.fastq.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:52:01.000000 cg-29.8.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:51:46.000000 cg-29.8.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-08 11:51:46.000000 cg-29.8.1/tests/utils/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-08 11:51:46.000000 cg-29.8.1/tests/utils/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 11:51:46.000000 cg-29.8.1/tests/utils/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-08 11:51:46.000000 cg-29.8.1/tests/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-08 11:51:46.000000 cg-29.8.1/tests/utils/test_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-08 11:51:46.000000 cg-29.8.1/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 12:13:11.000000 cg-29.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-08 12:13:23.000000 cg-29.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-08 12:13:11.000000 cg-29.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 12:13:11.000000 cg-29.8.2/cg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/crud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/crud/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/crud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/crud/find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/cgstats/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/cgstats/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/support_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/unaligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/db/models/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/demux_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/dragen_demux_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/parsers/adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/parsers/conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/parsers/demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/parsers/quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/parsers/run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/cgstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/crunchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12884 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/crunchy/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/crunchy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/crunchy/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/demux_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sample_sheet/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/hermes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/hermes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/hermes/hermes_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/hermes/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17538 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/housekeeper/hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/housekeeper/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/invoice/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/invoice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   113439 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    81032 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   113363 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    80886 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/lims/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/lims/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/lims/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/lims/samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/loqus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/madeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/madeline/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/mip/confighandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/orderform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/orderform/excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/orderform/json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/orderform/orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/scout/scout_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/scout/scoutapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/slurm/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/slurm/slurm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/apps/tb/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/tb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/tb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/tb/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-08 12:13:11.000000 cg-29.8.2/cg/apps/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/compress/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/compress/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/compress/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/delete/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/delete/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/delete/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/delete/observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/deliver/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/demultiplex/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/demultiplex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/demultiplex/demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/demultiplex/finish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/demultiplex/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/demultiplex/sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/generate/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/generate/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/generate/report/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/generate/report/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8386 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/set/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/set/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/set/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/store/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/store/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/clinical_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/fohm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/nipt/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/nipt/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/nipt/statina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/upload/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/observations/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/observations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/balsamic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/balsamic/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/balsamic/pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/balsamic/qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/balsamic/umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/fastq/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/fluffy/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/microsalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/microsalt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mip/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mip/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/mip_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mip_dna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mip_dna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/mip_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mip_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mip_rna/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/mutant/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mutant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/mutant/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/nextflow/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/rnafusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/rnafusion/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/taxprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/taxprofiler/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/cli/workflow/tower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/tower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 12:13:11.000000 cg-29.8.2/cg/cli/workflow/tower/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/cgstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/demultiplexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/gene_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/housekeeper_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/orderforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/pdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/sample_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/scout_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/sequencing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-08 12:13:11.000000 cg-29.8.2/cg/constants/tb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-08 12:13:11.000000 cg-29.8.2/cg/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 12:13:11.000000 cg-29.8.2/cg/io/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-08 12:13:11.000000 cg-29.8.2/cg/io/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-08 12:13:11.000000 cg-29.8.2/cg/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-08 12:13:11.000000 cg-29.8.2/cg/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 12:13:11.000000 cg-29.8.2/cg/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/archive/ddn_dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18893 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/backup/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/backup/pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/clean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/clean/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/clean/demultiplexed_flow_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/clean/flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/compress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/compress/compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/compress/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/deliver_ticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/demultiplex/delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/demultiplex/demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/demultiplex/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/encryption/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/observations/balsamic_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/observations/mip_dna_observations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/observations/observations_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/balsamic_qc_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/balsamic_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/balsamic_umi_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/case_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/fastq_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/fluffy_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/metagenome_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/microbial_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/microsalt_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/mip_dna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/mip_rna_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/pool_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/rml_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/sars_cov_2_submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/orders/ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    78964 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/templates/balsamic_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)   151463 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/templates/bootstrap.html
+-rw-r--r--   0 runner    (1001) docker     (123)    77831 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/report/templates/mip-dna_report.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/rsync/rsync_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/rsync/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/tar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/tar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/tar/tar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/transfer/external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/transfer/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/transfer/lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/balsamic/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/fohm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/fohm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/fohm/fohm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/gisaid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/gisaid/gisaid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/gisaid/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/gt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/mip/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/mip/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/nipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/nipt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/nipt/nipt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/rnafusion/rnafusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/balsamic_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/balsamic_umi_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/hk_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/mip_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/rnafusion_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/scout/uploadscoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/upload/vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20192 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28473 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/balsamic_pon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/balsamic_qc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/balsamic_umi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/fluffy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14337 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/mip_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/mip_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10762 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/mutant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/nextflow_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/prepare_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/rnafusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/taxprofiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-08 12:13:11.000000 cg-29.8.2/cg/meta/workflow/tower_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/balsamic/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/balsamic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/balsamic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/cg_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/cgstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/cgstats/flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/cgstats/stats_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/compression_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/deliverables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/deliverables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/deliverables/metric_deliverables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/demultiplex/demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/demultiplex/flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/demultiplex/run_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/demultiplex/sbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/file_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/invoice/invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/lims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/lims/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/mip/mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/mip/mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/mip/mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/mip/mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/nextflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/nextflow/deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/nextflow/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/observations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/observations/input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/excel_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/json_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/orderform_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/sample_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/orders/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/report/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/report/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/report/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/rnafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/rnafusion/rnafusion_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/scout/scout_load_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/slurm/sbatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/taxprofiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/models/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-08 12:13:11.000000 cg-29.8.2/cg/models/workflow/mutant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    25590 2023-05-08 12:13:11.000000 cg-29.8.2/cg/resources/20181012_Indices.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-08 12:13:11.000000 cg-29.8.2/cg/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-08 12:13:11.000000 cg-29.8.2/cg/resources/rnafusion_bundle_filenames.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/server/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/invoices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/server/invoices/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/server/invoices/templates/invoices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/invoices/templates/invoices/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/invoices/templates/invoices/invoice.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/invoices/templates/invoices/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/invoices/templates/invoices/new.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/invoices/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/server/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/server/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-08 12:13:11.000000 cg-29.8.2/cg/server/templates/admin/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32042 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39247 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_analysis_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_case_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/filters/status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30042 2023-05-08 12:13:11.000000 cg-29.8.2/cg/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/utils/checksum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/checksum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/checksum/checksum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/utils/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/click/EnumChoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg/utils/flask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/flask/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-08 12:13:11.000000 cg-29.8.2/cg/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39785 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 12:13:23.000000 cg-29.8.2/cg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-08 12:13:11.000000 cg-29.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-08 12:13:11.000000 cg-29.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:13:23.000000 cg-29.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-08 12:13:11.000000 cg-29.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/cgstats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/cgstats/crud/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/crud/test_create_novaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/crud/test_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/cgstats/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/parsers/test_adapter_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/parsers/test_conversion_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/parsers/test_demux_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/parsers/test_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/parsers/test_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/test_cgstats_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/cgstats/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/coverage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/coverage/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/crunchy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/crunchy/test_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/crunchy/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/crunchy/test_crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/crunchy/test_spring_decompression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/demultiplex/test_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/demultiplex/test_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/gens/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/gens/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/gens/test_gens_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/gt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/gt/test_gt_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/hk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/hk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/hk/test__getattr__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/hk/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/hk/test_bundles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/hk/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/hk/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/hk/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/lims/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/lims/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/lims/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/loqus/
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/loqus/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/loqus/test_loqusdb_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/madeline/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/madeline/test_madeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/mip/test_config_mip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/mutacc_auto/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/mutacc_auto/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/mutacc_auto/test_mutacc_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/orderform/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/orderform/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/orderform/test_excel_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/orderform/test_excel_sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/orderform/test_json_orderform_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/orderform/test_orderform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/scout/test_get_causative_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/scout/test_get_scout_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/scout/test_scout_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/scout/test_scout_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/slurm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/slurm/test_slurm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/test_apps_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/test_osticket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/apps/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-08 12:13:11.000000 cg-29.8.2/tests/apps/vogue/test_vogue_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/add/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/add/test_cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/add/test_cli_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/add/test_cli_add_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/add/test_cli_add_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/add/test_cli_add_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/backup/test_backup_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/clean/test_balsamic_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/clean/test_clean_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/clean/test_hk_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/clean/test_hk_case_bundle_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/clean/test_microbial_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/clean/test_rsync_past_run_dirs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/compress/test_cli_compress_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/compress/test_cli_decompress_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/compress/test_compress_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/compress/test_store_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/delete/test_cli_delete_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/delete/test_cli_delete_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/deliver/test_deliver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/deliver/test_rsync_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/deliver/test_run_deliver_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/test_add_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/test_create_sample_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/test_demultiplex_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/test_finish_demux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/test_stats_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/demultiplex/test_validate_sample_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/generate/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/generate/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/generate/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/generate/report/test_cli_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/generate/report/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/generate/test_cli_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/get/test_cli_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/get/test_cli_get_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/get/test_cli_get_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/get/test_cli_get_flow_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/get/test_cli_get_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/set/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/set/test_cli_set_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/set/test_cli_set_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/set/test_cli_set_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/set/test_cli_set_list_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/set/test_cli_set_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/set/test_cli_set_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/store/test_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/test_cli_status_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_genotype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_nipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_nipt_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_nipt_statina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/upload/test_cli_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)    31891 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15354 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/balsamic/test_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/balsamic/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/balsamic/test_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/balsamic/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/balsamic/test_store_housekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fastq/test_fastq_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/fluffy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fluffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fluffy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fluffy/test_cli_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fluffy/test_cli_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fluffy/test_cli_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/fluffy/test_cli_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/microsalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/microsalt/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/microsalt/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/microsalt/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/microsalt/test_microsalt_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/cli/workflow/taxprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/taxprofiler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/test_cli_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-08 12:13:11.000000 cg-29.8.2/tests/cli/workflow/test_cli_workflow_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64049 2023-05-08 12:13:11.000000 cg-29.8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/DEMUX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/Unaligned5/Project_337334/Sample_ADM1136A3_XTC08/ADM1136A3_XTC08_AGTGGTCA_L002_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/balsamic/tn_wgs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/balsamic/tn_wgs/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/balsamic/tn_wgs/ascat.output.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/balsamic/tn_wgs/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/balsamic/tn_wgs/sv.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/microsalt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)    14644 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/mip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/ADM1.baf.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/ADM1.cov.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/ADM2.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/ADM3.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/adm1.cram
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/adm1.mt.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/multiqc.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/report.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/smn.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/snv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/snv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/str.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/sv.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/sv_research.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/mip/dna/vcf2cytosure.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/analysis/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/rnafusion/multiqc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/analysis/sample_coverage.bed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/balsamic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/balsamic/case/
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/balsamic/case/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/balsamic/case/metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/balsamic/case/metadata_directory.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/balsamic/case/metadata_file_tags.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/crunchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/crunchy/spring_metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    53877 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Project_150392/Sample_ACC7769A10/HN3FKDSXY_AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Adapter_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/Quality_Metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/dummy_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338370 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz.md5
+-rw-r--r--   0 runner    (1001) docker     (123)   338349 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/150392/ACC7769A10/AL-P-00425491-N-03103120-KH20210330-PN20210331_S1_L001_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L001_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Undetermined_S0_L002_R2_001.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/CopyComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RTAComplete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/demuxstarted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/hiseq_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)    92887 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/fluffy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/fluffy/2020-23219-05/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/fluffy/2020-23219-05/2020-23219-05.WCXpredict_aberrations.filt.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/fluffy/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/fluffy/deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/fluffy/fluffy_fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/fluffy/multiqc_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/fluffy/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/gt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/gt/yellowhog.bcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/madeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/madeline/madeline.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/case_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37367 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/empty_case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/empty_case_metrics_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/empty_case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/empty_delivery_report.html
+-rw-r--r--   0 runner    (1001) docker     (123)    62741 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/store/case_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/mip/sample_file.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/scout/643594.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/scout/case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/scout/export_causatives.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/scout/none_case_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/scout/other_sex_case.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/scout/panel_export.bed
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/scout/panel_export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/apps/shipping/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/apps/shipping/scout-deploy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/cgweb_orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/balsamic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/fastq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/metagenome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/microsalt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/mip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/mip_rna.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/rml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/cgweb_orders/sarscov2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/data/SampleSheet.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   258048 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/data/cgfixture.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/data/fastq.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    49152 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/data/hkstore.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/data/yellowhog/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/data/yellowhog/pedigree.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/io/example_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/io/example_json.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/orderforms/
+-rw-r--r--   0 runner    (1001) docker     (123)   257271 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256694 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257319 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   256733 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1508.27.fastq.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257317 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1508.27.mip.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   257230 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    95490 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1603.11.microbial.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   158941 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1604.15.rml.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    88438 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)   228196 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    18639 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/NIPT-json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/fixtures/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/report/case_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/report/lims_exported_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-08 12:13:11.000000 cg-29.8.2/tests/fixtures/report/lims_family.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-08 12:13:11.000000 cg-29.8.2/tests/io/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-05-08 12:13:11.000000 cg-29.8.2/tests/io/test_io_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-08 12:13:11.000000 cg-29.8.2/tests/io/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-08 12:13:11.000000 cg-29.8.2/tests/io/test_io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-08 12:13:11.000000 cg-29.8.2/tests/io/test_io_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/archive/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/archive/test_archiving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/backup/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24603 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/backup/test_meta_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/backup/test_meta_pdc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/clean/
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/clean/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/clean/test_clean_demultiplexed_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/clean/test_clean_flow_cell_run_directories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/compress/
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/compress/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/compress/test_clean_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/compress/test_compress_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/compress/test_compress_meta_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/compress/test_decompress_spring_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/compress/test_meta_compress_update_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/deliver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/deliver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/deliver/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/deliver/test_deliver_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/deliver/test_delivery_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/demultiplex/
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/demultiplex/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/demultiplex/test_delete_demultiplex_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/demultiplex/test_demux_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/demultiplex/test_rename_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/encryption/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12857 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/encryption/test_encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/observations/test_meta_upload_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/orders/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_PoolSubmitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19944 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_meta_orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_meta_orders_lims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_meta_orders_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/orders/test_ticket_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/report/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/report/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/report/test_balsamic_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/report/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/report/test_mip_dna_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/report/test_report_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/rsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/rsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/rsync/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/rsync/test_rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/test_invoice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/transfer/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/transfer/test_external_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/transfer/test_meta_transfer_flowcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/transfer/test_meta_transfer_lims.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/balsamic/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/gisaid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/gisaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/gisaid/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/gisaid/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/gisaid/fixtures/four_samples.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/gisaid/fixtures/invalid_housekeeper.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/gisaid/fixtures/valid_gisaid.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/gisaid/fixtures/valid_housekeeper.fasta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/mutacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/mutacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/mutacc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/nipt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/nipt/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/nipt/test_nipt_upload_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/scout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/scout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/scout/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/scout/test_generate_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32161 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/scout/test_scout_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/test_meta_upload_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/test_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/test_upload_genotypes_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/upload/vogue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/vogue/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/upload/vogue/test_upload_vogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/meta/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/workflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/workflow/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/workflow/test_balsamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/workflow/test_microsalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-08 12:13:11.000000 cg-29.8.2/tests/meta/workflow/test_prepare_fastq_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/balsamic_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/crunchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20596 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/hk_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/limsmock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/madeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/mip_analysis_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/osticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/process_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/scout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/store_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-08 12:13:11.000000 cg-29.8.2/tests/mocks/tb_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/balsamic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/balsamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/balsamic/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/balsamic/test_balsamic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/demultiplexing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/demultiplexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/demultiplexing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/demultiplexing/test_demux_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/demultiplexing/test_flowcell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/demultiplexing/test_run_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/mip/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/mip/test_mip_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/mip/test_mip_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/mip/test_mip_metrics_deliverables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/mip/test_mip_sample_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/nextflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/nextflow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/nextflow/test_nextflow_deliver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/observations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/observations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/observations/test_observations_input_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/report/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/models/rnafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/rnafusion/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/rnafusion/test_rnafusion_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/test_cg_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/test_compression_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/test_file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-08 12:13:11.000000 cg-29.8.2/tests/models/test_flowcell_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-08 12:13:11.000000 cg-29.8.2/tests/server/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-08 12:13:11.000000 cg-29.8.2/tests/server/test_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-08 12:13:11.000000 cg-29.8.2/tests/server/test_server_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-08 12:13:11.000000 cg-29.8.2/tests/small_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/store/api/add/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/add/test_store_add_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/add/test_store_add_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/add/test_store_add_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/add/test_store_add_flow_celll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19418 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/store/api/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/delete/test_store_api_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/store/api/find/
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/find/test_find_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/find/test_find_basic_data_application_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/find/test_find_business_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/find/test_find_business_data_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/find/test_find_business_data_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14017 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/find/test_find_business_data_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/store/api/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_analyses_to_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_analyses_to_delivery_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9788 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_store_api_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_store_api_status_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54170 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_store_api_status_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_store_api_status_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_store_api_status_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/status/test_store_api_status_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/api/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_analyses_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_application_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_application_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_bed_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_bed_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_case_sample_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39481 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_cases_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_collaboration_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_customer_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_flow_cell_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_invoice_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_organism_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_panel_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_pool_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_samples_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/filters/test_status_user_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/test_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-05-08 12:13:11.000000 cg-29.8.2/tests/store_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 12:13:11.000000 cg-29.8.2/tests/test_store_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/tests/fixtures/apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/tests/fixtures/apps/demultiplexing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/copycomplete.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/tests/fixtures/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/tests/fixtures/data/fastq.fastq.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:23.000000 cg-29.8.2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:13:11.000000 cg-29.8.2/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-08 12:13:11.000000 cg-29.8.2/tests/utils/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-08 12:13:11.000000 cg-29.8.2/tests/utils/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 12:13:11.000000 cg-29.8.2/tests/utils/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-08 12:13:11.000000 cg-29.8.2/tests/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-08 12:13:11.000000 cg-29.8.2/tests/utils/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-08 12:13:11.000000 cg-29.8.2/tests/utils/test_utils.py
```

### Comparing `cg-29.8.1/PKG-INFO` & `cg-29.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 29.8.1
+Version: 29.8.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-29.8.1/README.md` & `cg-29.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/crud/create.py` & `cg-29.8.2/cg/apps/cgstats/crud/create.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/crud/delete.py` & `cg-29.8.2/cg/apps/cgstats/crud/delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/crud/find.py` & `cg-29.8.2/cg/apps/cgstats/crud/find.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/base.py` & `cg-29.8.2/cg/apps/cgstats/db/models/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/datasource.py` & `cg-29.8.2/cg/apps/cgstats/db/models/datasource.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/demux.py` & `cg-29.8.2/cg/apps/cgstats/db/models/demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/flowcell.py` & `cg-29.8.2/cg/apps/cgstats/db/models/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/project.py` & `cg-29.8.2/cg/apps/cgstats/db/models/project.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/sample.py` & `cg-29.8.2/cg/apps/cgstats/db/models/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/support_params.py` & `cg-29.8.2/cg/apps/cgstats/db/models/support_params.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/unaligned.py` & `cg-29.8.2/cg/apps/cgstats/db/models/unaligned.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/db/models/version.py` & `cg-29.8.2/cg/apps/cgstats/db/models/version.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/demux_sample.py` & `cg-29.8.2/cg/apps/cgstats/demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/dragen_demux_sample.py` & `cg-29.8.2/cg/apps/cgstats/dragen_demux_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/parsers/adapter_metrics.py` & `cg-29.8.2/cg/apps/cgstats/parsers/adapter_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/parsers/conversion_stats.py` & `cg-29.8.2/cg/apps/cgstats/parsers/conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/parsers/demux_stats.py` & `cg-29.8.2/cg/apps/cgstats/parsers/demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py` & `cg-29.8.2/cg/apps/cgstats/parsers/dragen_demultiplexing_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/parsers/quality_metrics.py` & `cg-29.8.2/cg/apps/cgstats/parsers/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/parsers/run_info.py` & `cg-29.8.2/cg/apps/cgstats/parsers/run_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/cgstats/stats.py` & `cg-29.8.2/cg/apps/cgstats/stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/coverage/api.py` & `cg-29.8.2/cg/apps/coverage/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/crunchy/crunchy.py` & `cg-29.8.2/cg/apps/crunchy/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/crunchy/files.py` & `cg-29.8.2/cg/apps/crunchy/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/crunchy/sbatch.py` & `cg-29.8.2/cg/apps/crunchy/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/demultiplex_api.py` & `cg-29.8.2/cg/apps/demultiplex/demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/demux_report.py` & `cg-29.8.2/cg/apps/demultiplex/demux_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/sample_sheet/create.py` & `cg-29.8.2/cg/apps/demultiplex/sample_sheet/create.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/sample_sheet/dummy_sample.py` & `cg-29.8.2/cg/apps/demultiplex/sample_sheet/dummy_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/sample_sheet/index.py` & `cg-29.8.2/cg/apps/demultiplex/sample_sheet/index.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/sample_sheet/models.py` & `cg-29.8.2/cg/apps/demultiplex/sample_sheet/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py` & `cg-29.8.2/cg/apps/demultiplex/sample_sheet/novaseq_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/sample_sheet/validate.py` & `cg-29.8.2/cg/apps/demultiplex/sample_sheet/validate.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/demultiplex/sbatch.py` & `cg-29.8.2/cg/apps/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/gens.py` & `cg-29.8.2/cg/apps/gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/gt.py` & `cg-29.8.2/cg/apps/gt.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/hermes/hermes_api.py` & `cg-29.8.2/cg/apps/hermes/hermes_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/hermes/models.py` & `cg-29.8.2/cg/apps/hermes/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/housekeeper/hk.py` & `cg-29.8.2/cg/apps/housekeeper/hk.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/invoice/render.py` & `cg-29.8.2/cg/apps/invoice/render.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/invoice/templates/KI_pool_invoice.xlsx` & `cg-29.8.2/cg/apps/invoice/templates/KI_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/invoice/templates/KI_sample_invoice.xlsx` & `cg-29.8.2/cg/apps/invoice/templates/KI_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/invoice/templates/KTH_pool_invoice.xlsx` & `cg-29.8.2/cg/apps/invoice/templates/KTH_pool_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/invoice/templates/KTH_sample_invoice.xlsx` & `cg-29.8.2/cg/apps/invoice/templates/KTH_sample_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/lims/api.py` & `cg-29.8.2/cg/apps/lims/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/lims/batch.py` & `cg-29.8.2/cg/apps/lims/batch.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/lims/order.py` & `cg-29.8.2/cg/apps/lims/order.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/lims/samplesheet.py` & `cg-29.8.2/cg/apps/lims/samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/loqus.py` & `cg-29.8.2/cg/apps/loqus.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/madeline/api.py` & `cg-29.8.2/cg/apps/madeline/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/mip/confighandler.py` & `cg-29.8.2/cg/apps/mip/confighandler.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/mutacc_auto.py` & `cg-29.8.2/cg/apps/mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/orderform/excel_orderform_parser.py` & `cg-29.8.2/cg/apps/orderform/excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/orderform/json_orderform_parser.py` & `cg-29.8.2/cg/apps/orderform/json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/orderform/orderform_parser.py` & `cg-29.8.2/cg/apps/orderform/orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/osticket.py` & `cg-29.8.2/cg/apps/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/scout/scout_export.py` & `cg-29.8.2/cg/apps/scout/scout_export.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/scout/scoutapi.py` & `cg-29.8.2/cg/apps/scout/scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/slurm/sbatch.py` & `cg-29.8.2/cg/apps/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/slurm/slurm_api.py` & `cg-29.8.2/cg/apps/slurm/slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/tb/api.py` & `cg-29.8.2/cg/apps/tb/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/tb/models.py` & `cg-29.8.2/cg/apps/tb/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/apps/vogue.py` & `cg-29.8.2/cg/apps/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/add.py` & `cg-29.8.2/cg/cli/add.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/backup.py` & `cg-29.8.2/cg/cli/backup.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/base.py` & `cg-29.8.2/cg/cli/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/clean.py` & `cg-29.8.2/cg/cli/clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/compress/base.py` & `cg-29.8.2/cg/cli/compress/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/compress/fastq.py` & `cg-29.8.2/cg/cli/compress/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/compress/helpers.py` & `cg-29.8.2/cg/cli/compress/helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/delete/base.py` & `cg-29.8.2/cg/cli/delete/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/delete/case.py` & `cg-29.8.2/cg/cli/delete/case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/delete/cases.py` & `cg-29.8.2/cg/cli/delete/cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/delete/observations.py` & `cg-29.8.2/cg/cli/delete/observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/deliver/base.py` & `cg-29.8.2/cg/cli/deliver/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/demultiplex/add.py` & `cg-29.8.2/cg/cli/demultiplex/add.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/demultiplex/base.py` & `cg-29.8.2/cg/cli/demultiplex/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/demultiplex/demux.py` & `cg-29.8.2/cg/cli/demultiplex/demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/demultiplex/finish.py` & `cg-29.8.2/cg/cli/demultiplex/finish.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/demultiplex/report.py` & `cg-29.8.2/cg/cli/demultiplex/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/demultiplex/sample_sheet.py` & `cg-29.8.2/cg/cli/demultiplex/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/export.py` & `cg-29.8.2/cg/cli/export.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/generate/report/base.py` & `cg-29.8.2/cg/cli/generate/report/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/generate/report/options.py` & `cg-29.8.2/cg/cli/generate/report/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/generate/report/utils.py` & `cg-29.8.2/cg/cli/generate/report/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/get.py` & `cg-29.8.2/cg/cli/get.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/set/base.py` & `cg-29.8.2/cg/cli/set/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/set/case.py` & `cg-29.8.2/cg/cli/set/case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/set/cases.py` & `cg-29.8.2/cg/cli/set/cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/status.py` & `cg-29.8.2/cg/cli/status.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/store/fastq.py` & `cg-29.8.2/cg/cli/store/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/store/store.py` & `cg-29.8.2/cg/cli/store/store.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/transfer.py` & `cg-29.8.2/cg/cli/transfer.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/base.py` & `cg-29.8.2/cg/cli/upload/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/clinical_delivery.py` & `cg-29.8.2/cg/cli/upload/clinical_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/coverage.py` & `cg-29.8.2/cg/cli/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/delivery_report.py` & `cg-29.8.2/cg/cli/upload/delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/fohm.py` & `cg-29.8.2/cg/cli/upload/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/genotype.py` & `cg-29.8.2/cg/cli/upload/genotype.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/gens.py` & `cg-29.8.2/cg/cli/upload/gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/gisaid.py` & `cg-29.8.2/cg/cli/upload/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/mutacc.py` & `cg-29.8.2/cg/cli/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/nipt/base.py` & `cg-29.8.2/cg/cli/upload/nipt/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/nipt/ftp.py` & `cg-29.8.2/cg/cli/upload/nipt/ftp.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/nipt/statina.py` & `cg-29.8.2/cg/cli/upload/nipt/statina.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/observations/observations.py` & `cg-29.8.2/cg/cli/upload/observations/observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/observations/utils.py` & `cg-29.8.2/cg/cli/upload/observations/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/scout.py` & `cg-29.8.2/cg/cli/upload/scout.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/utils.py` & `cg-29.8.2/cg/cli/upload/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/validate.py` & `cg-29.8.2/cg/cli/upload/validate.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/upload/vogue.py` & `cg-29.8.2/cg/cli/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/balsamic/base.py` & `cg-29.8.2/cg/cli/workflow/balsamic/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/balsamic/options.py` & `cg-29.8.2/cg/cli/workflow/balsamic/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/balsamic/pon.py` & `cg-29.8.2/cg/cli/workflow/balsamic/pon.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/balsamic/qc.py` & `cg-29.8.2/cg/cli/workflow/balsamic/qc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/balsamic/umi.py` & `cg-29.8.2/cg/cli/workflow/balsamic/umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/base.py` & `cg-29.8.2/cg/cli/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/commands.py` & `cg-29.8.2/cg/cli/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/fastq/base.py` & `cg-29.8.2/cg/cli/workflow/fastq/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/fluffy/base.py` & `cg-29.8.2/cg/cli/workflow/fluffy/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/microsalt/base.py` & `cg-29.8.2/cg/cli/workflow/microsalt/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/mip/base.py` & `cg-29.8.2/cg/cli/workflow/mip/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/mip/options.py` & `cg-29.8.2/cg/cli/workflow/mip/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/mip_dna/base.py` & `cg-29.8.2/cg/cli/workflow/mip_dna/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/mip_rna/base.py` & `cg-29.8.2/cg/cli/workflow/mip_rna/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/mutant/base.py` & `cg-29.8.2/cg/cli/workflow/mutant/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/nextflow/options.py` & `cg-29.8.2/cg/cli/workflow/nextflow/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/rnafusion/base.py` & `cg-29.8.2/cg/cli/workflow/rnafusion/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/rnafusion/options.py` & `cg-29.8.2/cg/cli/workflow/rnafusion/options.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/cli/workflow/taxprofiler/base.py` & `cg-29.8.2/cg/cli/workflow/taxprofiler/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/__init__.py` & `cg-29.8.2/cg/constants/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     CAPTUREKIT_CANCER_OPTIONS,
     CAPTUREKIT_OPTIONS,
     CASE_ACTIONS,
     COLLABORATORS,
     COMBOS,
     CONTAINER_OPTIONS,
     DEFAULT_CAPTURE_KIT,
-    FLOWCELL_Q30_THRESHOLD,
     FLOWCELL_STATUS,
     PREP_CATEGORIES,
     SEX_OPTIONS,
     STATUS_OPTIONS,
     DataDelivery,
     FileExtensions,
     FlowCellStatus,
@@ -22,7 +21,8 @@
 from cg.constants.housekeeper_tags import HK_FASTQ_TAGS, HK_MULTIQC_HTML_TAG, SequencingFileTag
 from cg.constants.paths import TMP_DIR
 from cg.constants.priority import Priority
 from cg.constants.process import EXIT_FAIL, EXIT_SUCCESS, RETURN_SUCCESS
 from cg.constants.report import *
 from cg.constants.sample_sources import ANALYSIS_SOURCES, METAGENOME_SOURCES
 from cg.constants.symbols import SINGLE_QUOTE, SPACE
+from cg.constants.sequencing import FLOWCELL_Q30_THRESHOLD
```

### Comparing `cg-29.8.1/cg/constants/compression.py` & `cg-29.8.2/cg/constants/compression.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/constants.py` & `cg-29.8.2/cg/constants/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Constants for cg."""
 
 import click
-from cgmodels.cg.constants import StrEnum
 
-from cg.constants.sequencing import Sequencers
-from cg.utils.date import get_date
 from cg.utils.enums import StrEnum
+from cg.utils.date import get_date
 
 VALID_DATA_IN_PRODUCTION = get_date("2017-09-27")
 
 MAX_ITEMS_TO_RETRIEVE = 50
 
 SCALE_TO_MILLION_READ_PAIRS = 2_000_000
 
@@ -60,20 +58,14 @@
     REQUESTED: str = "requested"
     PROCESSING: str = "processing"
     RETRIEVED: str = "retrieved"
 
 
 FLOWCELL_STATUS = [status.value for status in FlowCellStatus]
 
-FLOWCELL_Q30_THRESHOLD = {
-    Sequencers.HISEQX: 75,
-    Sequencers.HISEQGA: 80,
-    Sequencers.NOVASEQ: 75,
-}
-
 
 class AnalysisType(StrEnum):
     TARGETED_GENOME_SEQUENCING: str = "tgs"
     WHOLE_EXOME_SEQUENCING: str = "wes"
     WHOLE_GENOME_SEQUENCING: str = "wgs"
     WHOLE_TRANSCRIPTOME_SEQUENCING: str = "wts"
     OTHER: str = "other"
```

### Comparing `cg-29.8.1/cg/constants/delivery.py` & `cg-29.8.2/cg/constants/delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/demultiplexing.py` & `cg-29.8.2/cg/constants/demultiplexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 import click
-from cgmodels.cg.constants import StrEnum
+from cg.utils.enums import StrEnum
 
 
 class BclConverter(StrEnum):
     """Define the BCL converter."""
 
     DRAGEN: str = "dragen"
     BCL2FASTQ: str = "bcl2fastq"
```

### Comparing `cg-29.8.1/cg/constants/encryption.py` & `cg-29.8.2/cg/constants/encryption.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Constants specific for encryption"""
 
-from cgmodels.cg.constants import StrEnum
-
-from cg.utils.enums import ListEnum
+from cg.utils.enums import ListEnum, StrEnum
 
 
 class CipherAlgorithm(StrEnum):
     TRIPLE_DES: str = "3DES"
     AES: str = "AES"
     AES192: str = "AES192"
     AES256: str = "AES256"
```

### Comparing `cg-29.8.1/cg/constants/gene_panel.py` & `cg-29.8.2/cg/constants/gene_panel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Gene panel specific constants."""
 from typing import List
 
-from cgmodels.cg.constants import StrEnum
+from cg.utils.enums import StrEnum
 
 GENOME_BUILD_37 = "37"
 GENOME_BUILD_38 = "GRCh38"
 
 
 class GenePanelMasterList(StrEnum):
     BRAIN: str = "BRAIN"
```

### Comparing `cg-29.8.1/cg/constants/housekeeper_tags.py` & `cg-29.8.2/cg/constants/housekeeper_tags.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/lims.py` & `cg-29.8.2/cg/constants/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/nextflow.py` & `cg-29.8.2/cg/constants/nextflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/observations.py` & `cg-29.8.2/cg/constants/observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/orderforms.py` & `cg-29.8.2/cg/constants/orderforms.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/priority.py` & `cg-29.8.2/cg/constants/priority.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/report.py` & `cg-29.8.2/cg/constants/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/rnafusion.py` & `cg-29.8.2/cg/constants/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/scout_upload.py` & `cg-29.8.2/cg/constants/scout_upload.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/constants/sequencing.py` & `cg-29.8.2/cg/constants/sequencing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Constants related to all things sequencing"""
-from cgmodels.cg.constants import StrEnum
+from cg.utils.enums import StrEnum
 
 
 class Sequencers(StrEnum):
     """Sequencer instruments."""
 
     ALL: str = "all"
     HISEQX: str = "hiseqx"
@@ -30,14 +30,20 @@
     "ST-E00269": Sequencers.HISEQX,
     "A00187": Sequencers.NOVASEQ,
     "A00621": Sequencers.NOVASEQ,
     "A00689": Sequencers.NOVASEQ,
     "A01901": Sequencers.NOVASEQ,
 }
 
+FLOWCELL_Q30_THRESHOLD = {
+    Sequencers.HISEQX: 75,
+    Sequencers.HISEQGA: 80,
+    Sequencers.NOVASEQ: 75,
+}
+
 
 class SequencingMethod(StrEnum):
     """Sequencing method types."""
 
     TGS: str = "tgs"
     WES: str = "wes"
     WGS: str = "wgs"
```

### Comparing `cg-29.8.1/cg/constants/subject.py` & `cg-29.8.2/cg/constants/subject.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/exc.py` & `cg-29.8.2/cg/exc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/io/api.py` & `cg-29.8.2/cg/io/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/io/controller.py` & `cg-29.8.2/cg/io/controller.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/io/csv.py` & `cg-29.8.2/cg/io/csv.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/io/json.py` & `cg-29.8.2/cg/io/json.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/io/yaml.py` & `cg-29.8.2/cg/io/yaml.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/archive/ddn_dataflow.py` & `cg-29.8.2/cg/meta/archive/ddn_dataflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/backup/backup.py` & `cg-29.8.2/cg/meta/backup/backup.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/backup/pdc.py` & `cg-29.8.2/cg/meta/backup/pdc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/clean/api.py` & `cg-29.8.2/cg/meta/clean/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/clean/demultiplexed_flow_cells.py` & `cg-29.8.2/cg/meta/clean/demultiplexed_flow_cells.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/clean/flow_cell_run_directories.py` & `cg-29.8.2/cg/meta/clean/flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/compress/compress.py` & `cg-29.8.2/cg/meta/compress/compress.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/compress/files.py` & `cg-29.8.2/cg/meta/compress/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/deliver.py` & `cg-29.8.2/cg/meta/deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/deliver_ticket.py` & `cg-29.8.2/cg/meta/deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/demultiplex/delete_demultiplex_api.py` & `cg-29.8.2/cg/meta/demultiplex/delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/demultiplex/demux_post_processing.py` & `cg-29.8.2/cg/meta/demultiplex/demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/demultiplex/files.py` & `cg-29.8.2/cg/meta/demultiplex/files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/encryption/encryption.py` & `cg-29.8.2/cg/meta/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/invoice.py` & `cg-29.8.2/cg/meta/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/meta.py` & `cg-29.8.2/cg/meta/meta.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/observations/balsamic_observations_api.py` & `cg-29.8.2/cg/meta/observations/balsamic_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/observations/mip_dna_observations_api.py` & `cg-29.8.2/cg/meta/observations/mip_dna_observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/observations/observations_api.py` & `cg-29.8.2/cg/meta/observations/observations_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/api.py` & `cg-29.8.2/cg/meta/orders/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/case_submitter.py` & `cg-29.8.2/cg/meta/orders/case_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/fastq_submitter.py` & `cg-29.8.2/cg/meta/orders/fastq_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/lims.py` & `cg-29.8.2/cg/meta/orders/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/metagenome_submitter.py` & `cg-29.8.2/cg/meta/orders/metagenome_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/microbial_submitter.py` & `cg-29.8.2/cg/meta/orders/microbial_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/pool_submitter.py` & `cg-29.8.2/cg/meta/orders/pool_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/sars_cov_2_submitter.py` & `cg-29.8.2/cg/meta/orders/sars_cov_2_submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/submitter.py` & `cg-29.8.2/cg/meta/orders/submitter.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/orders/ticket_handler.py` & `cg-29.8.2/cg/meta/orders/ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/balsamic.py` & `cg-29.8.2/cg/meta/report/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/balsamic_umi.py` & `cg-29.8.2/cg/meta/report/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/field_validators.py` & `cg-29.8.2/cg/meta/report/field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/mip_dna.py` & `cg-29.8.2/cg/meta/report/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/report_api.py` & `cg-29.8.2/cg/meta/report/report_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/templates/balsamic_report.html` & `cg-29.8.2/cg/meta/report/templates/balsamic_report.html`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/templates/bootstrap.html` & `cg-29.8.2/cg/meta/report/templates/bootstrap.html`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/report/templates/mip-dna_report.html` & `cg-29.8.2/cg/meta/report/templates/mip-dna_report.html`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/rsync/rsync_api.py` & `cg-29.8.2/cg/meta/rsync/rsync_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/tar/tar.py` & `cg-29.8.2/cg/meta/tar/tar.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/transfer/external_data.py` & `cg-29.8.2/cg/meta/transfer/external_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/transfer/flowcell.py` & `cg-29.8.2/cg/meta/transfer/flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/transfer/lims.py` & `cg-29.8.2/cg/meta/transfer/lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/balsamic/balsamic.py` & `cg-29.8.2/cg/meta/upload/balsamic/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/coverage.py` & `cg-29.8.2/cg/meta/upload/coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/fohm/fohm.py` & `cg-29.8.2/cg/meta/upload/fohm/fohm.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/gisaid/constants.py` & `cg-29.8.2/cg/meta/upload/gisaid/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/gisaid/gisaid.py` & `cg-29.8.2/cg/meta/upload/gisaid/gisaid.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/gisaid/models.py` & `cg-29.8.2/cg/meta/upload/gisaid/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/gt.py` & `cg-29.8.2/cg/meta/upload/gt.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/mip/mip_dna.py` & `cg-29.8.2/cg/meta/upload/mip/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/mip/mip_rna.py` & `cg-29.8.2/cg/meta/upload/mip/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/mutacc.py` & `cg-29.8.2/cg/meta/upload/mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/nipt/nipt.py` & `cg-29.8.2/cg/meta/upload/nipt/nipt.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/rnafusion/rnafusion.py` & `cg-29.8.2/cg/meta/upload/rnafusion/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/scout/balsamic_config_builder.py` & `cg-29.8.2/cg/meta/upload/scout/balsamic_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/scout/balsamic_umi_config_builder.py` & `cg-29.8.2/cg/meta/upload/scout/balsamic_umi_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/scout/hk_tags.py` & `cg-29.8.2/cg/meta/upload/scout/hk_tags.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/scout/mip_config_builder.py` & `cg-29.8.2/cg/meta/upload/scout/mip_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/scout/rnafusion_config_builder.py` & `cg-29.8.2/cg/meta/upload/scout/rnafusion_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/scout/scout_config_builder.py` & `cg-29.8.2/cg/meta/upload/scout/scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/scout/uploadscoutapi.py` & `cg-29.8.2/cg/meta/upload/scout/uploadscoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/upload_api.py` & `cg-29.8.2/cg/meta/upload/upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/upload/vogue.py` & `cg-29.8.2/cg/meta/upload/vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/analysis.py` & `cg-29.8.2/cg/meta/workflow/analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/balsamic.py` & `cg-29.8.2/cg/meta/workflow/balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/balsamic_pon.py` & `cg-29.8.2/cg/meta/workflow/balsamic_pon.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/balsamic_qc.py` & `cg-29.8.2/cg/meta/workflow/balsamic_qc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/balsamic_umi.py` & `cg-29.8.2/cg/meta/workflow/balsamic_umi.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/fastq.py` & `cg-29.8.2/cg/meta/workflow/fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/fluffy.py` & `cg-29.8.2/cg/meta/workflow/fluffy.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/microsalt.py` & `cg-29.8.2/cg/meta/workflow/microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/mip.py` & `cg-29.8.2/cg/meta/workflow/mip.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/mip_dna.py` & `cg-29.8.2/cg/meta/workflow/mip_dna.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/mip_rna.py` & `cg-29.8.2/cg/meta/workflow/mip_rna.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/mutant.py` & `cg-29.8.2/cg/meta/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/nextflow_common.py` & `cg-29.8.2/cg/meta/workflow/nextflow_common.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/prepare_fastq.py` & `cg-29.8.2/cg/meta/workflow/prepare_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/rnafusion.py` & `cg-29.8.2/cg/meta/workflow/rnafusion.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/taxprofiler.py` & `cg-29.8.2/cg/meta/workflow/taxprofiler.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/meta/workflow/tower_common.py` & `cg-29.8.2/cg/meta/workflow/tower_common.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/balsamic/config.py` & `cg-29.8.2/cg/models/balsamic/config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/balsamic/metrics.py` & `cg-29.8.2/cg/models/balsamic/metrics.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/cg_config.py` & `cg-29.8.2/cg/models/cg_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/cgstats/stats_sample.py` & `cg-29.8.2/cg/models/cgstats/stats_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/compression_data.py` & `cg-29.8.2/cg/models/compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/deliverables/metric_deliverables.py` & `cg-29.8.2/cg/models/deliverables/metric_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/demultiplex/demux_results.py` & `cg-29.8.2/cg/models/demultiplex/demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/demultiplex/flow_cell.py` & `cg-29.8.2/cg/models/demultiplex/flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/demultiplex/run_parameters.py` & `cg-29.8.2/cg/models/demultiplex/run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/demultiplex/sbatch.py` & `cg-29.8.2/cg/models/demultiplex/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/file_data.py` & `cg-29.8.2/cg/models/file_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/invoice/invoice.py` & `cg-29.8.2/cg/models/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/lims/sample.py` & `cg-29.8.2/cg/models/lims/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/mip/mip_config.py` & `cg-29.8.2/cg/models/mip/mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/mip/mip_metrics_deliverables.py` & `cg-29.8.2/cg/models/mip/mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/mip/mip_sample_info.py` & `cg-29.8.2/cg/models/mip/mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/nextflow/deliverables.py` & `cg-29.8.2/cg/models/nextflow/deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/nextflow/sample.py` & `cg-29.8.2/cg/models/nextflow/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/observations/input_files.py` & `cg-29.8.2/cg/models/observations/input_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/orders/constants.py` & `cg-29.8.2/cg/models/orders/constants.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/orders/excel_sample.py` & `cg-29.8.2/cg/models/orders/excel_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/orders/json_sample.py` & `cg-29.8.2/cg/models/orders/json_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/orders/order.py` & `cg-29.8.2/cg/models/orders/order.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/orders/orderform_schema.py` & `cg-29.8.2/cg/models/orders/orderform_schema.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/orders/sample_base.py` & `cg-29.8.2/cg/models/orders/sample_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/orders/samples.py` & `cg-29.8.2/cg/models/orders/samples.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/report/metadata.py` & `cg-29.8.2/cg/models/report/metadata.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/report/report.py` & `cg-29.8.2/cg/models/report/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/report/sample.py` & `cg-29.8.2/cg/models/report/sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/report/validators.py` & `cg-29.8.2/cg/models/report/validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/rnafusion/rnafusion_sample.py` & `cg-29.8.2/cg/models/rnafusion/rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/scout/scout_load_config.py` & `cg-29.8.2/cg/models/scout/scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/slurm/sbatch.py` & `cg-29.8.2/cg/models/slurm/sbatch.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/models/workflow/mutant.py` & `cg-29.8.2/cg/models/workflow/mutant.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/resources/20181012_Indices.csv` & `cg-29.8.2/cg/resources/20181012_Indices.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/resources/rnafusion_bundle_filenames.csv` & `cg-29.8.2/cg/resources/rnafusion_bundle_filenames.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/admin.py` & `cg-29.8.2/cg/server/admin.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/api.py` & `cg-29.8.2/cg/server/api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/app.py` & `cg-29.8.2/cg/server/app.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/config.py` & `cg-29.8.2/cg/server/config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/ext.py` & `cg-29.8.2/cg/server/ext.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/invoices/templates/invoices/index.html` & `cg-29.8.2/cg/server/invoices/templates/invoices/index.html`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/invoices/templates/invoices/invoice.html` & `cg-29.8.2/cg/server/invoices/templates/invoices/invoice.html`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/invoices/templates/invoices/layout.html` & `cg-29.8.2/cg/server/invoices/templates/invoices/layout.html`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/invoices/templates/invoices/new.html` & `cg-29.8.2/cg/server/invoices/templates/invoices/new.html`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/server/invoices/views.py` & `cg-29.8.2/cg/server/invoices/views.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/api/add.py` & `cg-29.8.2/cg/store/api/add.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/api/base.py` & `cg-29.8.2/cg/store/api/base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/api/core.py` & `cg-29.8.2/cg/store/api/core.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/api/delete.py` & `cg-29.8.2/cg/store/api/delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/api/find_basic_data.py` & `cg-29.8.2/cg/store/api/find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/api/find_business_data.py` & `cg-29.8.2/cg/store/api/find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/api/status.py` & `cg-29.8.2/cg/store/api/status.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_analysis_filters.py` & `cg-29.8.2/cg/store/filters/status_analysis_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_application_filters.py` & `cg-29.8.2/cg/store/filters/status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_application_version_filters.py` & `cg-29.8.2/cg/store/filters/status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_bed_filters.py` & `cg-29.8.2/cg/store/filters/status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_bed_version_filters.py` & `cg-29.8.2/cg/store/filters/status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_case_filters.py` & `cg-29.8.2/cg/store/filters/status_case_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_case_sample_filters.py` & `cg-29.8.2/cg/store/filters/status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_collaboration_filters.py` & `cg-29.8.2/cg/store/filters/status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_customer_filters.py` & `cg-29.8.2/cg/store/filters/status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_flow_cell_filters.py` & `cg-29.8.2/cg/store/filters/status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_invoice_filters.py` & `cg-29.8.2/cg/store/filters/status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_organism_filters.py` & `cg-29.8.2/cg/store/filters/status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_panel_filters.py` & `cg-29.8.2/cg/store/filters/status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_pool_filters.py` & `cg-29.8.2/cg/store/filters/status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_sample_filters.py` & `cg-29.8.2/cg/store/filters/status_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/filters/status_user_filters.py` & `cg-29.8.2/cg/store/filters/status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/store/models.py` & `cg-29.8.2/cg/store/models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/checksum/checksum.py` & `cg-29.8.2/cg/utils/checksum/checksum.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/click/EnumChoice.py` & `cg-29.8.2/cg/utils/click/EnumChoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/commands.py` & `cg-29.8.2/cg/utils/commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/date.py` & `cg-29.8.2/cg/utils/date.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/dict.py` & `cg-29.8.2/cg/utils/dict.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/dispatcher.py` & `cg-29.8.2/cg/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/email.py` & `cg-29.8.2/cg/utils/email.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/flask/enum.py` & `cg-29.8.2/cg/utils/flask/enum.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg/utils/utils.py` & `cg-29.8.2/cg/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/cg.egg-info/PKG-INFO` & `cg-29.8.2/cg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg
-Version: 29.8.1
+Version: 29.8.2
 Summary: Clinical Genomics command center
 Home-page: https://github.com/Clinical-Genomics/cg
 Author: Clinical Genomics
 Author-email: support@clinicalgenomics.se
 License: UNKNOWN
 Description: 
         # cg
```

### Comparing `cg-29.8.1/cg.egg-info/SOURCES.txt` & `cg-29.8.2/cg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/requirements.txt` & `cg-29.8.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/setup.py` & `cg-29.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     with io.open(os.path.join(HERE, "README.md"), encoding="utf-8") as f:
         LONG_DESCRIPTION = "\n" + f.read()
 except FileNotFoundError:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name=NAME,
-    version="29.8.1",
+    version="29.8.2",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     include_package_data=True,
```

### Comparing `cg-29.8.1/tests/apps/cgstats/conftest.py` & `cg-29.8.2/tests/apps/cgstats/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/cgstats/crud/test_create_novaseq.py` & `cg-29.8.2/tests/apps/cgstats/crud/test_create_novaseq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/cgstats/crud/test_delete.py` & `cg-29.8.2/tests/apps/cgstats/crud/test_delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/cgstats/parsers/test_conversion_stats.py` & `cg-29.8.2/tests/apps/cgstats/parsers/test_conversion_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/cgstats/parsers/test_demux_stats.py` & `cg-29.8.2/tests/apps/cgstats/parsers/test_demux_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/cgstats/parsers/test_run_info.py` & `cg-29.8.2/tests/apps/cgstats/parsers/test_run_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/cgstats/test_cgstats_create.py` & `cg-29.8.2/tests/apps/cgstats/test_cgstats_create.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/cgstats/test_stats.py` & `cg-29.8.2/tests/apps/cgstats/test_stats.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/conftest.py` & `cg-29.8.2/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/coverage/test_coverage.py` & `cg-29.8.2/tests/apps/coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/crunchy/conftest.py` & `cg-29.8.2/tests/apps/crunchy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/crunchy/test_compress_fastq.py` & `cg-29.8.2/tests/apps/crunchy/test_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/crunchy/test_config.py` & `cg-29.8.2/tests/apps/crunchy/test_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/crunchy/test_crunchy.py` & `cg-29.8.2/tests/apps/crunchy/test_crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/crunchy/test_spring_decompression.py` & `cg-29.8.2/tests/apps/crunchy/test_spring_decompression.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/demultiplex/conftest.py` & `cg-29.8.2/tests/apps/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/demultiplex/test_convert_to_sample_sheet.py` & `cg-29.8.2/tests/apps/demultiplex/test_convert_to_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/demultiplex/test_demultiplex_api.py` & `cg-29.8.2/tests/apps/demultiplex/test_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/demultiplex/test_sample_sheet.py` & `cg-29.8.2/tests/apps/demultiplex/test_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/demultiplex/test_validate_sample_sheet.py` & `cg-29.8.2/tests/apps/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/gens/test_gens_api.py` & `cg-29.8.2/tests/apps/gens/test_gens_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/gt/conftest.py` & `cg-29.8.2/tests/apps/gt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/gt/test_gt_api.py` & `cg-29.8.2/tests/apps/gt/test_gt_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/hk/conftest.py` & `cg-29.8.2/tests/apps/hk/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/hk/test__getattr__.py` & `cg-29.8.2/tests/apps/hk/test__getattr__.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/hk/test_add_file.py` & `cg-29.8.2/tests/apps/hk/test_add_file.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/hk/test_bundles.py` & `cg-29.8.2/tests/apps/hk/test_bundles.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/hk/test_core.py` & `cg-29.8.2/tests/apps/hk/test_core.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/hk/test_file.py` & `cg-29.8.2/tests/apps/hk/test_file.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/hk/test_version.py` & `cg-29.8.2/tests/apps/hk/test_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/lims/conftest.py` & `cg-29.8.2/tests/apps/lims/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/lims/test_api.py` & `cg-29.8.2/tests/apps/lims/test_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/loqus/conftest.py` & `cg-29.8.2/tests/apps/loqus/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/loqus/test_loqusdb_api.py` & `cg-29.8.2/tests/apps/loqus/test_loqusdb_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/madeline/conftest.py` & `cg-29.8.2/tests/apps/madeline/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/madeline/test_madeline.py` & `cg-29.8.2/tests/apps/madeline/test_madeline.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/mip/conftest.py` & `cg-29.8.2/tests/apps/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/mip/test_config_mip.py` & `cg-29.8.2/tests/apps/mip/test_config_mip.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/mutacc_auto/conftest.py` & `cg-29.8.2/tests/apps/mutacc_auto/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/mutacc_auto/test_mutacc_auto.py` & `cg-29.8.2/tests/apps/mutacc_auto/test_mutacc_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/orderform/conftest.py` & `cg-29.8.2/tests/apps/orderform/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/orderform/test_excel_orderform_parser.py` & `cg-29.8.2/tests/apps/orderform/test_excel_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/orderform/test_excel_sample_schema.py` & `cg-29.8.2/tests/apps/orderform/test_excel_sample_schema.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/orderform/test_json_orderform_parser.py` & `cg-29.8.2/tests/apps/orderform/test_json_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/orderform/test_orderform_parser.py` & `cg-29.8.2/tests/apps/orderform/test_orderform_parser.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/scout/conftest.py` & `cg-29.8.2/tests/apps/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/scout/test_get_causative_variants.py` & `cg-29.8.2/tests/apps/scout/test_get_causative_variants.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/scout/test_get_scout_cases.py` & `cg-29.8.2/tests/apps/scout/test_get_scout_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/scout/test_scout_load_config.py` & `cg-29.8.2/tests/apps/scout/test_scout_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/scout/test_scout_models.py` & `cg-29.8.2/tests/apps/scout/test_scout_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/slurm/conftest.py` & `cg-29.8.2/tests/apps/slurm/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/slurm/test_slurm_api.py` & `cg-29.8.2/tests/apps/slurm/test_slurm_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/test_apps_environ.py` & `cg-29.8.2/tests/apps/test_apps_environ.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/test_osticket.py` & `cg-29.8.2/tests/apps/test_osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/vogue/conftest.py` & `cg-29.8.2/tests/apps/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/apps/vogue/test_vogue_api.py` & `cg-29.8.2/tests/apps/vogue/test_vogue_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/add/test_cli_add.py` & `cg-29.8.2/tests/cli/add/test_cli_add.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/add/test_cli_add_customer.py` & `cg-29.8.2/tests/cli/add/test_cli_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/add/test_cli_add_family.py` & `cg-29.8.2/tests/cli/add/test_cli_add_family.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/add/test_cli_add_relationship.py` & `cg-29.8.2/tests/cli/add/test_cli_add_relationship.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/add/test_cli_add_sample.py` & `cg-29.8.2/tests/cli/add/test_cli_add_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/backup/conftest.py` & `cg-29.8.2/tests/cli/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/backup/test_backup_command.py` & `cg-29.8.2/tests/cli/backup/test_backup_command.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/clean/conftest.py` & `cg-29.8.2/tests/cli/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/clean/test_balsamic_clean.py` & `cg-29.8.2/tests/cli/clean/test_balsamic_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/clean/test_clean_hk_bundle_files.py` & `cg-29.8.2/tests/cli/clean/test_clean_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/clean/test_hk_bundle_files.py` & `cg-29.8.2/tests/cli/clean/test_hk_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/clean/test_hk_case_bundle_files.py` & `cg-29.8.2/tests/cli/clean/test_hk_case_bundle_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/clean/test_microbial_clean.py` & `cg-29.8.2/tests/cli/clean/test_microbial_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/clean/test_rsync_past_run_dirs.py` & `cg-29.8.2/tests/cli/clean/test_rsync_past_run_dirs.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/compress/conftest.py` & `cg-29.8.2/tests/cli/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/compress/test_cli_compress_fastq.py` & `cg-29.8.2/tests/cli/compress/test_cli_compress_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/compress/test_cli_decompress_spring.py` & `cg-29.8.2/tests/cli/compress/test_cli_decompress_spring.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/compress/test_compress_helpers.py` & `cg-29.8.2/tests/cli/compress/test_compress_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/compress/test_store_fastq.py` & `cg-29.8.2/tests/cli/compress/test_store_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/conftest.py` & `cg-29.8.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/delete/test_cli_delete_case.py` & `cg-29.8.2/tests/cli/delete/test_cli_delete_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/delete/test_cli_delete_cases.py` & `cg-29.8.2/tests/cli/delete/test_cli_delete_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/deliver/conftest.py` & `cg-29.8.2/tests/cli/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/deliver/test_deliver_base.py` & `cg-29.8.2/tests/cli/deliver/test_deliver_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/deliver/test_rsync_base.py` & `cg-29.8.2/tests/cli/deliver/test_rsync_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/deliver/test_run_deliver_cmd.py` & `cg-29.8.2/tests/cli/deliver/test_run_deliver_cmd.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/demultiplex/conftest.py` & `cg-29.8.2/tests/cli/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/demultiplex/test_add_flowcell.py` & `cg-29.8.2/tests/cli/demultiplex/test_add_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/demultiplex/test_create_sample_sheet.py` & `cg-29.8.2/tests/cli/demultiplex/test_create_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/demultiplex/test_demultiplex_flowcell.py` & `cg-29.8.2/tests/cli/demultiplex/test_demultiplex_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/demultiplex/test_finish_demux.py` & `cg-29.8.2/tests/cli/demultiplex/test_finish_demux.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/demultiplex/test_stats_command.py` & `cg-29.8.2/tests/cli/demultiplex/test_stats_command.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/demultiplex/test_validate_sample_sheet.py` & `cg-29.8.2/tests/cli/demultiplex/test_validate_sample_sheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/generate/report/conftest.py` & `cg-29.8.2/tests/cli/generate/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/generate/report/test_cli_delivery_report.py` & `cg-29.8.2/tests/cli/generate/report/test_cli_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/generate/report/test_utils.py` & `cg-29.8.2/tests/cli/generate/report/test_utils.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/generate/test_cli_base.py` & `cg-29.8.2/tests/cli/generate/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/get/test_cli_get.py` & `cg-29.8.2/tests/cli/get/test_cli_get.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/get/test_cli_get_analysis.py` & `cg-29.8.2/tests/cli/get/test_cli_get_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/get/test_cli_get_case.py` & `cg-29.8.2/tests/cli/get/test_cli_get_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/get/test_cli_get_flow_cell.py` & `cg-29.8.2/tests/cli/get/test_cli_get_flow_cell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/get/test_cli_get_sample.py` & `cg-29.8.2/tests/cli/get/test_cli_get_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/set/conftest.py` & `cg-29.8.2/tests/cli/set/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/set/test_cli_set_case.py` & `cg-29.8.2/tests/cli/set/test_cli_set_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/set/test_cli_set_cases.py` & `cg-29.8.2/tests/cli/set/test_cli_set_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/set/test_cli_set_flowcell.py` & `cg-29.8.2/tests/cli/set/test_cli_set_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/set/test_cli_set_list_keys.py` & `cg-29.8.2/tests/cli/set/test_cli_set_list_keys.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/set/test_cli_set_sample.py` & `cg-29.8.2/tests/cli/set/test_cli_set_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/set/test_cli_set_samples.py` & `cg-29.8.2/tests/cli/set/test_cli_set_samples.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/store/test_fastq.py` & `cg-29.8.2/tests/cli/store/test_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/test_base.py` & `cg-29.8.2/tests/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/test_clean.py` & `cg-29.8.2/tests/cli/test_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/test_cli_status_cases.py` & `cg-29.8.2/tests/cli/test_cli_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/conftest.py` & `cg-29.8.2/tests/cli/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_scout.py` & `cg-29.8.2/tests/cli/upload/test_cli_scout.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_auto.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_auto.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_delivery_report.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_fastq.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_genotype.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_genotype.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_gens.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_gens.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_nipt.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_nipt.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_nipt_ftp.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_nipt_ftp.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_nipt_statina.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_nipt_statina.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_observations.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/upload/test_cli_upload_vogue.py` & `cg-29.8.2/tests/cli/upload/test_cli_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/balsamic/conftest.py` & `cg-29.8.2/tests/cli/workflow/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py` & `cg-29.8.2/tests/cli/workflow/balsamic/test_cli_balsamic_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/balsamic/test_compound_commands.py` & `cg-29.8.2/tests/cli/workflow/balsamic/test_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/balsamic/test_link.py` & `cg-29.8.2/tests/cli/workflow/balsamic/test_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/balsamic/test_report_deliver.py` & `cg-29.8.2/tests/cli/workflow/balsamic/test_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/balsamic/test_run.py` & `cg-29.8.2/tests/cli/workflow/balsamic/test_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/balsamic/test_store_housekeeper.py` & `cg-29.8.2/tests/cli/workflow/balsamic/test_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/conftest.py` & `cg-29.8.2/tests/cli/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/fastq/test_fastq_base.py` & `cg-29.8.2/tests/cli/workflow/fastq/test_fastq_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/fluffy/conftest.py` & `cg-29.8.2/tests/cli/workflow/fluffy/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py` & `cg-29.8.2/tests/cli/workflow/fluffy/test_cli_create_samplesheet.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/fluffy/test_cli_link.py` & `cg-29.8.2/tests/cli/workflow/fluffy/test_cli_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/fluffy/test_cli_run.py` & `cg-29.8.2/tests/cli/workflow/fluffy/test_cli_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/fluffy/test_cli_start.py` & `cg-29.8.2/tests/cli/workflow/fluffy/test_cli_start.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/fluffy/test_cli_store.py` & `cg-29.8.2/tests/cli/workflow/fluffy/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/microsalt/conftest.py` & `cg-29.8.2/tests/cli/workflow/microsalt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py` & `cg-29.8.2/tests/cli/workflow/microsalt/snapshots/snap_test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/microsalt/test_microsalt_case_config.py` & `cg-29.8.2/tests/cli/workflow/microsalt/test_microsalt_case_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/microsalt/test_microsalt_run.py` & `cg-29.8.2/tests/cli/workflow/microsalt/test_microsalt_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/conftest.py` & `cg-29.8.2/tests/cli/workflow/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_base.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_run.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_dna_start.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_dna_start.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_rna_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_rna_link.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_rna_link.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_rna_run.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_rna_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/mip/test_cli_mip_store.py` & `cg-29.8.2/tests/cli/workflow/mip/test_cli_mip_store.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/rnafusion/conftest.py` & `cg-29.8.2/tests/cli/workflow/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py` & `cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py` & `cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_config_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py` & `cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_metrics_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py` & `cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_report_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py` & `cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_run.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py` & `cg-29.8.2/tests/cli/workflow/rnafusion/test_cli_rnafusion_store_housekeeper.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py` & `cg-29.8.2/tests/cli/workflow/taxprofiler/test_cli_taxprofiler_compound_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/test_cli_workflow.py` & `cg-29.8.2/tests/cli/workflow/test_cli_workflow.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/cli/workflow/test_cli_workflow_clean.py` & `cg-29.8.2/tests/cli/workflow/test_cli_workflow_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/conftest.py` & `cg-29.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml` & `cg-29.8.2/tests/fixtures/DEMUX/160219_D00410_0217_AHJKMYBCXX/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json` & `cg-29.8.2/tests/fixtures/analysis/microsalt/ACC11111_qc_fail/ACC11111_qc_fail.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json` & `cg-29.8.2/tests/fixtures/analysis/microsalt/ACC22222_qc_pass/ACC22222_qc_pass.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/analysis/rnafusion/multiqc_data.json` & `cg-29.8.2/tests/fixtures/analysis/rnafusion/multiqc_data.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/analysis/sample_coverage.bed` & `cg-29.8.2/tests/fixtures/analysis/sample_coverage.bed`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/balsamic/case/config.json` & `cg-29.8.2/tests/fixtures/apps/balsamic/case/config.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/balsamic/case/metadata.yml` & `cg-29.8.2/tests/fixtures/apps/balsamic/case/metadata.yml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml` & `cg-29.8.2/tests/fixtures/apps/balsamic/case/metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/crunchy/spring_metadata.json` & `cg-29.8.2/tests/fixtures/apps/crunchy/spring_metadata.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/201203_A00689_0200_AHVKJCDRXX/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Bcl2Fastq.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/SampleSheetS2_Dragen.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/211101_A00187_0615_AHLG5GDRXY/Unaligned/Reports/RunInfo.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs/fastq/fastq_run_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/ConversionStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/demultiplexed-runs-unfinished/201203_A00689_0200_AHVKJCDRXX/Unaligned/Stats/DemultiplexingStats.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/201203_A00689_0200_AHVKJCDRXX/RunParameters_different_index_cycles.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/HLG5GDRXY_demultiplex.stdout`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/211101_A00187_0615_AHLG5GDRXY/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/bcl2fastq/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/HVKJCDRXX_demultiplex.stderr`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/flowcell-runs/dragen/201203_A00689_0200_AHVKJCDRXX/RunParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/hiseq_run/runParameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/raw_lims_samples/raw_samplesheet_novaseq.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/runParameters_missing_flowcell_run_field.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml` & `cg-29.8.2/tests/fixtures/apps/demultiplexing/unknown_run_parameters.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/fluffy/SampleSheet.csv` & `cg-29.8.2/tests/fixtures/apps/fluffy/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/fluffy/deliverables.yaml` & `cg-29.8.2/tests/fixtures/apps/fluffy/deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/madeline/madeline.xml` & `cg-29.8.2/tests/fixtures/apps/madeline/madeline.xml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/case_metrics_deliverables.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/case_metrics_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/dna/store/case_config.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/dna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/dna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/dna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf` & `cg-29.8.2/tests/fixtures/apps/mip/dna/store/yellowhog_clinical_selected.vcf`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/rna/case_config.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/rna/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/rna/case_qc_sampleinfo.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/rna/store/bundle_data.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/rna/store/bundle_data.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/rna/store/case_config.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/rna/store/case_config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/rna/store/case_id_deliverables.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml` & `cg-29.8.2/tests/fixtures/apps/mip/rna/store/case_qc_sample_info.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/scout/643594.config.yaml` & `cg-29.8.2/tests/fixtures/apps/scout/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/scout/case_export.json` & `cg-29.8.2/tests/fixtures/apps/scout/case_export.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/scout/export_causatives.json` & `cg-29.8.2/tests/fixtures/apps/scout/export_causatives.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/scout/none_case_export.json` & `cg-29.8.2/tests/fixtures/apps/scout/none_case_export.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/scout/other_sex_case.json` & `cg-29.8.2/tests/fixtures/apps/scout/other_sex_case.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/scout/panel_export.bed` & `cg-29.8.2/tests/fixtures/apps/scout/panel_export.bed`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/apps/scout/panel_export.csv` & `cg-29.8.2/tests/fixtures/apps/scout/panel_export.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/balsamic.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/balsamic.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/fastq.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/fastq.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/metagenome.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/metagenome.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/microsalt.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/microsalt.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/mip.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/mip.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/mip_rna.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/mip_rna.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/rml.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/rml.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/cgweb_orders/sarscov2.json` & `cg-29.8.2/tests/fixtures/cgweb_orders/sarscov2.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/data/SampleSheet.csv` & `cg-29.8.2/tests/fixtures/data/SampleSheet.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/data/cgfixture.db` & `cg-29.8.2/tests/fixtures/data/cgfixture.db`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/data/hkstore.db` & `cg-29.8.2/tests/fixtures/data/hkstore.db`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/io/example_json.json` & `cg-29.8.2/tests/fixtures/io/example_json.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1508.27.balsamic.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1508.27.balsamic.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1508.27.balsamic_qc.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1508.27.balsamic_umi.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1508.27.fastq.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1508.27.fastq.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1508.27.mip.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1508.27.mip.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1508.27.mip_rna.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1508.27.mip_rna.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1603.11.microbial.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1603.11.microbial.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1604.15.rml.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1604.15.rml.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/1605.10.metagenome.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/1605.10.metagenome.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/2184.7.sarscov2.xlsx` & `cg-29.8.2/tests/fixtures/orderforms/2184.7.sarscov2.xlsx`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/NIPT-json.json` & `cg-29.8.2/tests/fixtures/orderforms/NIPT-json.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json` & `cg-29.8.2/tests/fixtures/orderforms/balsamic_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/orderforms/mip_uploaded_json_orderform.json` & `cg-29.8.2/tests/fixtures/orderforms/mip_uploaded_json_orderform.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/report/case_data.json` & `cg-29.8.2/tests/fixtures/report/case_data.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/report/lims_exported_samples.json` & `cg-29.8.2/tests/fixtures/report/lims_exported_samples.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/fixtures/report/lims_family.json` & `cg-29.8.2/tests/fixtures/report/lims_family.json`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/io/conftest.py` & `cg-29.8.2/tests/io/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/io/test_io_controller.py` & `cg-29.8.2/tests/io/test_io_controller.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/io/test_io_csv.py` & `cg-29.8.2/tests/io/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/io/test_io_json.py` & `cg-29.8.2/tests/io/test_io_json.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/io/test_io_yaml.py` & `cg-29.8.2/tests/io/test_io_yaml.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/archive/conftest.py` & `cg-29.8.2/tests/meta/archive/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/archive/test_archiving.py` & `cg-29.8.2/tests/meta/archive/test_archiving.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/backup/conftest.py` & `cg-29.8.2/tests/meta/backup/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/backup/test_meta_backup.py` & `cg-29.8.2/tests/meta/backup/test_meta_backup.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/backup/test_meta_pdc.py` & `cg-29.8.2/tests/meta/backup/test_meta_pdc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/clean/conftest.py` & `cg-29.8.2/tests/meta/clean/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/clean/test_clean_demultiplexed_runs.py` & `cg-29.8.2/tests/meta/clean/test_clean_demultiplexed_runs.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/clean/test_clean_flow_cell_run_directories.py` & `cg-29.8.2/tests/meta/clean/test_clean_flow_cell_run_directories.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/compress/conftest.py` & `cg-29.8.2/tests/meta/compress/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/compress/test_clean_fastq.py` & `cg-29.8.2/tests/meta/compress/test_clean_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/compress/test_compress_files.py` & `cg-29.8.2/tests/meta/compress/test_compress_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/compress/test_compress_meta_fastq.py` & `cg-29.8.2/tests/meta/compress/test_compress_meta_fastq.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/compress/test_decompress_spring_meta.py` & `cg-29.8.2/tests/meta/compress/test_decompress_spring_meta.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/compress/test_meta_compress_update_hk.py` & `cg-29.8.2/tests/meta/compress/test_meta_compress_update_hk.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/conftest.py` & `cg-29.8.2/tests/meta/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/deliver/conftest.py` & `cg-29.8.2/tests/meta/deliver/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/deliver/test_deliver_ticket.py` & `cg-29.8.2/tests/meta/deliver/test_deliver_ticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/deliver/test_delivery_api.py` & `cg-29.8.2/tests/meta/deliver/test_delivery_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/demultiplex/conftest.py` & `cg-29.8.2/tests/meta/demultiplex/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/demultiplex/test_delete_demultiplex_api.py` & `cg-29.8.2/tests/meta/demultiplex/test_delete_demultiplex_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/demultiplex/test_demux_post_processing.py` & `cg-29.8.2/tests/meta/demultiplex/test_demux_post_processing.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/demultiplex/test_rename_files.py` & `cg-29.8.2/tests/meta/demultiplex/test_rename_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/encryption/conftest.py` & `cg-29.8.2/tests/meta/encryption/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/encryption/test_encryption.py` & `cg-29.8.2/tests/meta/encryption/test_encryption.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/observations/conftest.py` & `cg-29.8.2/tests/meta/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/observations/test_meta_upload_observations.py` & `cg-29.8.2/tests/meta/observations/test_meta_upload_observations.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/conftest.py` & `cg-29.8.2/tests/meta/orders/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_PoolSubmitter_validate_order.py` & `cg-29.8.2/tests/meta/orders/test_PoolSubmitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py` & `cg-29.8.2/tests/meta/orders/test_SarsCov2Submitter_order_to_status.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_SarsCov2Submitter_store_order.py` & `cg-29.8.2/tests/meta/orders/test_SarsCov2Submitter_store_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_SarsCov2Submitter_validate_order.py` & `cg-29.8.2/tests/meta/orders/test_SarsCov2Submitter_validate_order.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_meta_orders_api.py` & `cg-29.8.2/tests/meta/orders/test_meta_orders_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_meta_orders_lims.py` & `cg-29.8.2/tests/meta/orders/test_meta_orders_lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_meta_orders_status.py` & `cg-29.8.2/tests/meta/orders/test_meta_orders_status.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/orders/test_ticket_handler.py` & `cg-29.8.2/tests/meta/orders/test_ticket_handler.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/report/conftest.py` & `cg-29.8.2/tests/meta/report/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/report/test_balsamic_api.py` & `cg-29.8.2/tests/meta/report/test_balsamic_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/report/test_field_validators.py` & `cg-29.8.2/tests/meta/report/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/report/test_mip_dna_api.py` & `cg-29.8.2/tests/meta/report/test_mip_dna_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/report/test_report_api.py` & `cg-29.8.2/tests/meta/report/test_report_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/rsync/conftest.py` & `cg-29.8.2/tests/meta/rsync/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/rsync/test_rsync.py` & `cg-29.8.2/tests/meta/rsync/test_rsync.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/test_invoice.py` & `cg-29.8.2/tests/meta/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/transfer/conftest.py` & `cg-29.8.2/tests/meta/transfer/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/transfer/test_external_data.py` & `cg-29.8.2/tests/meta/transfer/test_external_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/transfer/test_meta_transfer_flowcell.py` & `cg-29.8.2/tests/meta/transfer/test_meta_transfer_flowcell.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/transfer/test_meta_transfer_lims.py` & `cg-29.8.2/tests/meta/transfer/test_meta_transfer_lims.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/balsamic/test_balsamic.py` & `cg-29.8.2/tests/meta/upload/balsamic/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/conftest.py` & `cg-29.8.2/tests/meta/upload/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/gisaid/conftest.py` & `cg-29.8.2/tests/meta/upload/gisaid/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/gisaid/fixtures/four_samples.csv` & `cg-29.8.2/tests/meta/upload/gisaid/fixtures/four_samples.csv`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/mutacc/conftest.py` & `cg-29.8.2/tests/meta/upload/mutacc/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/mutacc/test_meta_upload_mutacc.py` & `cg-29.8.2/tests/meta/upload/mutacc/test_meta_upload_mutacc.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/nipt/conftest.py` & `cg-29.8.2/tests/meta/upload/nipt/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/nipt/test_nipt_upload_api.py` & `cg-29.8.2/tests/meta/upload/nipt/test_nipt_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/scout/conftest.py` & `cg-29.8.2/tests/meta/upload/scout/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/scout/test_generate_load_config.py` & `cg-29.8.2/tests/meta/upload/scout/test_generate_load_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/scout/test_meta_upload_scoutapi.py` & `cg-29.8.2/tests/meta/upload/scout/test_meta_upload_scoutapi.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py` & `cg-29.8.2/tests/meta/upload/scout/test_meta_upload_scoutapi_rna.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/scout/test_scout_config_builder.py` & `cg-29.8.2/tests/meta/upload/scout/test_scout_config_builder.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/test_meta_upload_coverage.py` & `cg-29.8.2/tests/meta/upload/test_meta_upload_coverage.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/test_upload_api.py` & `cg-29.8.2/tests/meta/upload/test_upload_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/test_upload_genotypes_api.py` & `cg-29.8.2/tests/meta/upload/test_upload_genotypes_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/vogue/conftest.py` & `cg-29.8.2/tests/meta/upload/vogue/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/upload/vogue/test_upload_vogue.py` & `cg-29.8.2/tests/meta/upload/vogue/test_upload_vogue.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/workflow/conftest.py` & `cg-29.8.2/tests/meta/workflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/workflow/test_analysis.py` & `cg-29.8.2/tests/meta/workflow/test_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/workflow/test_balsamic.py` & `cg-29.8.2/tests/meta/workflow/test_balsamic.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/workflow/test_microsalt.py` & `cg-29.8.2/tests/meta/workflow/test_microsalt.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/meta/workflow/test_prepare_fastq_api.py` & `cg-29.8.2/tests/meta/workflow/test_prepare_fastq_api.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/balsamic_analysis_mock.py` & `cg-29.8.2/tests/mocks/balsamic_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/crunchy.py` & `cg-29.8.2/tests/mocks/crunchy.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/hk_mock.py` & `cg-29.8.2/tests/mocks/hk_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/limsmock.py` & `cg-29.8.2/tests/mocks/limsmock.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/madeline.py` & `cg-29.8.2/tests/mocks/madeline.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/mip_analysis_mock.py` & `cg-29.8.2/tests/mocks/mip_analysis_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/osticket.py` & `cg-29.8.2/tests/mocks/osticket.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/process_mock.py` & `cg-29.8.2/tests/mocks/process_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/report.py` & `cg-29.8.2/tests/mocks/report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/scout.py` & `cg-29.8.2/tests/mocks/scout.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/store_model.py` & `cg-29.8.2/tests/mocks/store_model.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/mocks/tb_mock.py` & `cg-29.8.2/tests/mocks/tb_mock.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/balsamic/conftest.py` & `cg-29.8.2/tests/models/balsamic/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/balsamic/test_balsamic_analysis.py` & `cg-29.8.2/tests/models/balsamic/test_balsamic_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/conftest.py` & `cg-29.8.2/tests/models/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/demultiplexing/conftest.py` & `cg-29.8.2/tests/models/demultiplexing/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/demultiplexing/test_demux_results.py` & `cg-29.8.2/tests/models/demultiplexing/test_demux_results.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/demultiplexing/test_flowcell_model.py` & `cg-29.8.2/tests/models/demultiplexing/test_flowcell_model.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/demultiplexing/test_run_parameters.py` & `cg-29.8.2/tests/models/demultiplexing/test_run_parameters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/mip/conftest.py` & `cg-29.8.2/tests/models/mip/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/mip/test_mip_analysis.py` & `cg-29.8.2/tests/models/mip/test_mip_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/mip/test_mip_config.py` & `cg-29.8.2/tests/models/mip/test_mip_config.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/mip/test_mip_metrics_deliverables.py` & `cg-29.8.2/tests/models/mip/test_mip_metrics_deliverables.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/mip/test_mip_sample_info.py` & `cg-29.8.2/tests/models/mip/test_mip_sample_info.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/nextflow/conftest.py` & `cg-29.8.2/tests/models/nextflow/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/nextflow/test_nextflow_deliver.py` & `cg-29.8.2/tests/models/nextflow/test_nextflow_deliver.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/observations/conftest.py` & `cg-29.8.2/tests/models/observations/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/observations/test_observations_input_files.py` & `cg-29.8.2/tests/models/observations/test_observations_input_files.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/report/test_validators.py` & `cg-29.8.2/tests/models/report/test_validators.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/rnafusion/conftest.py` & `cg-29.8.2/tests/models/rnafusion/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/rnafusion/test_rnafusion_sample.py` & `cg-29.8.2/tests/models/rnafusion/test_rnafusion_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/test_cg_models.py` & `cg-29.8.2/tests/models/test_cg_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/test_compression_data.py` & `cg-29.8.2/tests/models/test_compression_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/test_file_data.py` & `cg-29.8.2/tests/models/test_file_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/models/test_flowcell_class.py` & `cg-29.8.2/tests/models/test_flowcell_class.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/server/conftest.py` & `cg-29.8.2/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/add/test_store_add_application_version.py` & `cg-29.8.2/tests/store/api/add/test_store_add_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/add/test_store_add_base.py` & `cg-29.8.2/tests/store/api/add/test_store_add_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/add/test_store_add_customer.py` & `cg-29.8.2/tests/store/api/add/test_store_add_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/add/test_store_add_flow_celll.py` & `cg-29.8.2/tests/store/api/add/test_store_add_flow_celll.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/conftest.py` & `cg-29.8.2/tests/store/api/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/delete/test_store_api_delete.py` & `cg-29.8.2/tests/store/api/delete/test_store_api_delete.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/find/test_find_basic_data.py` & `cg-29.8.2/tests/store/api/find/test_find_basic_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/find/test_find_basic_data_application_version.py` & `cg-29.8.2/tests/store/api/find/test_find_basic_data_application_version.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/find/test_find_business_data.py` & `cg-29.8.2/tests/store/api/find/test_find_business_data.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/find/test_find_business_data_analysis.py` & `cg-29.8.2/tests/store/api/find/test_find_business_data_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/find/test_find_business_data_case.py` & `cg-29.8.2/tests/store/api/find/test_find_business_data_case.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/find/test_find_business_data_sample.py` & `cg-29.8.2/tests/store/api/find/test_find_business_data_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_analyses_to_clean.py` & `cg-29.8.2/tests/store/api/status/test_analyses_to_clean.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_analyses_to_delivery_report.py` & `cg-29.8.2/tests/store/api/status/test_analyses_to_delivery_report.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_store_api_status.py` & `cg-29.8.2/tests/store/api/status/test_store_api_status.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_store_api_status_analysis.py` & `cg-29.8.2/tests/store/api/status/test_store_api_status_analysis.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_store_api_status_cases.py` & `cg-29.8.2/tests/store/api/status/test_store_api_status_cases.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_store_api_status_customer.py` & `cg-29.8.2/tests/store/api/status/test_store_api_status_customer.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_store_api_status_pool.py` & `cg-29.8.2/tests/store/api/status/test_store_api_status_pool.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/status/test_store_api_status_sample.py` & `cg-29.8.2/tests/store/api/status/test_store_api_status_sample.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/api/test_base.py` & `cg-29.8.2/tests/store/api/test_base.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/conftest.py` & `cg-29.8.2/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_analyses_filters.py` & `cg-29.8.2/tests/store/filters/test_status_analyses_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_application_filters.py` & `cg-29.8.2/tests/store/filters/test_status_application_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_application_version_filters.py` & `cg-29.8.2/tests/store/filters/test_status_application_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_bed_filters.py` & `cg-29.8.2/tests/store/filters/test_status_bed_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_bed_version_filters.py` & `cg-29.8.2/tests/store/filters/test_status_bed_version_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_case_sample_filters.py` & `cg-29.8.2/tests/store/filters/test_status_case_sample_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_cases_filters.py` & `cg-29.8.2/tests/store/filters/test_status_cases_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_collaboration_filters.py` & `cg-29.8.2/tests/store/filters/test_status_collaboration_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_customer_filters.py` & `cg-29.8.2/tests/store/filters/test_status_customer_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_flow_cell_filters.py` & `cg-29.8.2/tests/store/filters/test_status_flow_cell_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_invoice_filters.py` & `cg-29.8.2/tests/store/filters/test_status_invoice_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_organism_filters.py` & `cg-29.8.2/tests/store/filters/test_status_organism_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_panel_filters.py` & `cg-29.8.2/tests/store/filters/test_status_panel_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_pool_filters.py` & `cg-29.8.2/tests/store/filters/test_status_pool_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_samples_filters.py` & `cg-29.8.2/tests/store/filters/test_status_samples_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/filters/test_status_user_filters.py` & `cg-29.8.2/tests/store/filters/test_status_user_filters.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/test_delivery.py` & `cg-29.8.2/tests/store/test_delivery.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store/test_store_models.py` & `cg-29.8.2/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/store_helpers.py` & `cg-29.8.2/tests/store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/test_store_helpers.py` & `cg-29.8.2/tests/test_store_helpers.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/utils/conftest.py` & `cg-29.8.2/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/utils/test_commands.py` & `cg-29.8.2/tests/utils/test_commands.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/utils/test_date.py` & `cg-29.8.2/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/utils/test_dict.py` & `cg-29.8.2/tests/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/utils/test_dispatcher.py` & `cg-29.8.2/tests/utils/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cg-29.8.1/tests/utils/test_utils.py` & `cg-29.8.2/tests/utils/test_utils.py`

 * *Files identical despite different names*

