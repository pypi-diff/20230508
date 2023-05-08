# Comparing `tmp/ncbi-datasets-pylib-9.0.0.tar.gz` & `tmp/ncbi-datasets-pylib-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ncbi-datasets-pylib-9.0.0.tar", last modified: Thu Oct  1 20:00:42 2020, max compression
+gzip compressed data, was "dist/ncbi-datasets-pylib-9.1.0.tar", last modified: Fri Oct  9 11:40:29 2020, max compression
```

## Comparing `ncbi-datasets-pylib-9.0.0.tar` & `ncbi-datasets-pylib-9.1.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)      965 2020-10-01 19:59:53.000000 ncbi-datasets-pylib-9.0.0/LICENSE.md
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2964 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/PKG-INFO
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2282 2020-10-01 19:59:53.000000 ncbi-datasets-pylib-9.0.0/README.md
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)      220 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/requirements.txt
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)      580 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/setup.cfg
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       76 2020-10-01 19:59:53.000000 ncbi-datasets-pylib-9.0.0/setup.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/__init__.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/__init__.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6392 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/__init__.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)      234 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    76591 2020-10-01 19:59:55.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/gene_api.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    65857 2020-10-01 19:59:57.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/genome_api.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    56667 2020-10-01 19:59:58.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/virus_api.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    26247 2020-10-01 19:59:58.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api_client.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2737 2020-10-01 20:00:22.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/bio_dataset.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/components/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/components/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     1956 2020-10-01 20:00:22.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/components/sequence.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    12529 2020-10-01 19:59:58.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/configuration.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3797 2020-10-01 19:59:58.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/exceptions.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5816 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2964 2020-10-01 19:59:59.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/assembly_dataset_request_resolution.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3573 2020-10-01 19:59:59.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/assembly_metadata_request_accessions.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     9450 2020-10-01 19:59:59.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/datasetsv1alpha1_error.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6458 2020-10-01 20:00:01.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/download_summary_dehydrated.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5357 2020-10-01 20:00:01.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/download_summary_hydrated.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2903 2020-10-01 20:00:02.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_assembly_error_code.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3346 2020-10-01 20:00:02.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_gene_error_code.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4420 2020-10-01 20:00:03.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_replaced_id.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2882 2020-10-01 20:00:03.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_virus_error_code.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5320 2020-10-01 20:00:04.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gatewayruntime_error.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2961 2020-10-01 20:00:04.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_fasta.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4240 2020-10-01 20:00:04.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_sort.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3017 2020-10-01 20:00:05.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_sort_direction.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3036 2020-10-01 20:00:05.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_sort_field.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4194 2020-10-01 20:00:05.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_symbols_for_taxon.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3251 2020-10-01 20:00:05.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_descriptor_gene_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2908 2020-10-01 20:00:06.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_descriptor_rna_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3052 2020-10-01 20:00:06.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/genomic_region_genomic_region_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3547 2020-10-01 20:00:06.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/micro_bigge_dataset_request_element_flank_config.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4043 2020-10-01 20:00:07.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_count_by_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2928 2020-10-01 20:00:07.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_count_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4084 2020-10-01 20:00:08.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_counts.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3974 2020-10-01 20:00:08.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_rank_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4331 2020-10-01 20:00:08.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/protobuf_any.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6221 2020-10-01 20:00:09.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/runtime_stream_error.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4120 2020-10-01 20:00:09.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/sci_name_and_ids_sci_name_and_id.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4279 2020-10-01 20:00:10.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/stream_result_of_v1alpha1_tabular_output.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3079 2020-10-01 20:00:10.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/transcript_transcript_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     7698 2020-10-01 20:00:11.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4386 2020-10-01 20:00:11.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_file.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3136 2020-10-01 20:00:12.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3085 2020-10-01 20:00:12.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_virus_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5385 2020-10-01 20:00:13.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_availability.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    12678 2020-10-01 20:00:13.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptor.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4808 2020-10-01 20:00:13.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4664 2020-10-01 20:00:14.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_filter.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3032 2020-10-01 20:00:14.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_request_content_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     9964 2020-10-01 20:00:14.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_request.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4256 2020-10-01 20:00:15.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_match.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5265 2020-10-01 20:00:15.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2962 2020-10-01 20:00:15.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata_request_content_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     8614 2020-10-01 20:00:16.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_download_summary.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     8485 2020-10-01 20:00:16.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2942 2020-10-01 20:00:17.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request_content_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    20198 2020-10-01 20:00:17.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_descriptor.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4183 2020-10-01 20:00:17.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_descriptors.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4095 2020-10-01 20:00:17.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_match.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5089 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_metadata.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4201 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_genomic_region.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4865 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_mature_peptide.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3365 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_message.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3176 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_micro_bigge_dataset_request_file_type.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4268 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_nomenclature_authority.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    19688 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_organism.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2873 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_orientation.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     7208 2020-10-01 20:00:18.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_protein.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5394 2020-10-01 20:00:19.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_range.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3663 2020-10-01 20:00:19.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_sci_name_and_ids.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4256 2020-10-01 20:00:20.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_seq_range_set.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3339 2020-10-01 20:00:20.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_tabular_output.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     9186 2020-10-01 20:00:21.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_transcript.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3846 2020-10-01 20:00:21.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_virus_table_field.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/package/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/package/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     7886 2020-10-01 20:00:23.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/package/dataset.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/reports/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/reports/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4525 2020-10-01 20:00:24.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/reports/report_reader.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    12328 2020-10-01 20:00:21.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/rest.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/utils/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/utils/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)      107 2020-10-01 20:00:25.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/utils/utils.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    10690 2020-10-01 20:00:26.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/catalog_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-01 20:00:29.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/catalog_pb2_grpc.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)   186715 2020-10-01 20:00:29.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/datasets_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-01 20:00:30.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/datasets_pb2_grpc.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    16107 2020-10-01 20:00:30.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    48120 2020-10-01 20:00:30.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2_grpc.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    41994 2020-10-01 20:00:32.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/assembly_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-01 20:00:32.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/assembly_pb2_grpc.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6250 2020-10-01 20:00:32.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/common_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-01 20:00:33.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/common_pb2_grpc.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    35580 2020-10-01 20:00:33.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/gene_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-01 20:00:33.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/gene_pb2_grpc.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/microbigge/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/microbigge/__init__.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    27597 2020-10-01 20:00:33.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/microbigge/microbigge_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-01 20:00:33.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/microbigge/microbigge_pb2_grpc.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)    43712 2020-10-01 20:00:33.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/virus_pb2.py
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-01 20:00:34.000000 ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/virus_pb2_grpc.py
-drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2964 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/PKG-INFO
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5559 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/SOURCES.txt
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        1 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/dependency_links.txt
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        1 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/not-zip-safe
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)      215 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/requires.txt
--rw-r--r--   0 tomcat   (11236) tomcat   (13030)        5 2020-10-01 20:00:42.000000 ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/top_level.txt
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)      965 2020-10-09 11:40:07.000000 ncbi-datasets-pylib-9.1.0/LICENSE.md
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2964 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/PKG-INFO
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2282 2020-10-09 11:40:07.000000 ncbi-datasets-pylib-9.1.0/README.md
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)      220 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/requirements.txt
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)      580 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/setup.cfg
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       76 2020-10-09 11:40:07.000000 ncbi-datasets-pylib-9.1.0/setup.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/__init__.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/__init__.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6392 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/__init__.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)      234 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    76591 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/gene_api.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    65857 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/genome_api.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    56667 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/virus_api.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    26247 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api_client.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2737 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/bio_dataset.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/components/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/components/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     1956 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/components/sequence.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    12529 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/configuration.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3797 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/exceptions.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5816 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2964 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/assembly_dataset_request_resolution.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3573 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/assembly_metadata_request_accessions.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     9450 2020-10-09 11:40:08.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/datasetsv1alpha1_error.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6458 2020-10-09 11:40:09.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/download_summary_dehydrated.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5357 2020-10-09 11:40:09.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/download_summary_hydrated.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2903 2020-10-09 11:40:09.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_assembly_error_code.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3346 2020-10-09 11:40:09.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_gene_error_code.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4420 2020-10-09 11:40:09.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_replaced_id.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2882 2020-10-09 11:40:09.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_virus_error_code.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5320 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gatewayruntime_error.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2961 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_fasta.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4240 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_sort.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3017 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_sort_direction.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3036 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_sort_field.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4194 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_symbols_for_taxon.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3251 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_descriptor_gene_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2908 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_descriptor_rna_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3052 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/genomic_region_genomic_region_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3547 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/micro_bigge_dataset_request_element_flank_config.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4043 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_count_by_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2928 2020-10-09 11:40:10.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_count_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4084 2020-10-09 11:40:11.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_counts.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3974 2020-10-09 11:40:11.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_rank_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4331 2020-10-09 11:40:11.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/protobuf_any.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6221 2020-10-09 11:40:11.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/runtime_stream_error.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4120 2020-10-09 11:40:11.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/sci_name_and_ids_sci_name_and_id.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4279 2020-10-09 11:40:11.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/stream_result_of_v1alpha1_tabular_output.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3079 2020-10-09 11:40:12.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/transcript_transcript_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     7698 2020-10-09 11:40:12.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4386 2020-10-09 11:40:12.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_file.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3136 2020-10-09 11:40:12.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3085 2020-10-09 11:40:13.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_virus_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5385 2020-10-09 11:40:13.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_availability.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    12678 2020-10-09 11:40:13.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptor.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4808 2020-10-09 11:40:13.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4664 2020-10-09 11:40:13.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_filter.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3032 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_request_content_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     9964 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_request.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4256 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_match.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5265 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2962 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata_request_content_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     8614 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_download_summary.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     8485 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2942 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request_content_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    20198 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_descriptor.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4183 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_descriptors.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4095 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_match.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5089 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_metadata.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4201 2020-10-09 11:40:14.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_genomic_region.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4865 2020-10-09 11:40:15.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_mature_peptide.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3365 2020-10-09 11:40:15.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_message.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3176 2020-10-09 11:40:15.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_micro_bigge_dataset_request_file_type.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4268 2020-10-09 11:40:15.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_nomenclature_authority.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    19688 2020-10-09 11:40:15.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_organism.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2873 2020-10-09 11:40:15.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_orientation.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     7208 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_protein.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5394 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_range.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3663 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_sci_name_and_ids.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4256 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_seq_range_set.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3339 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_tabular_output.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     9186 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_transcript.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     3846 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_virus_table_field.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/package/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/package/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     7887 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/package/dataset.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/reports/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/reports/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     4525 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/reports/report_reader.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    12328 2020-10-09 11:40:16.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/rest.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/utils/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/utils/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)      107 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/utils/utils.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    10690 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/catalog_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/catalog_pb2_grpc.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)   186715 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/datasets_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/datasets_pb2_grpc.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    16107 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    48120 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2_grpc.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    39931 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/assembly_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/assembly_pb2_grpc.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     6250 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/common_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/common_pb2_grpc.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    35580 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/gene_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-09 11:40:17.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/gene_pb2_grpc.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/microbigge/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/microbigge/__init__.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    27597 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/microbigge/microbigge_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/microbigge/microbigge_pb2_grpc.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)    43712 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/virus_pb2.py
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)       83 2020-10-09 11:40:18.000000 ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/virus_pb2_grpc.py
+drwxr-xr-x   0 tomcat   (11236) tomcat   (13030)        0 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     2964 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/PKG-INFO
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)     5559 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/SOURCES.txt
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        1 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/dependency_links.txt
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        1 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/not-zip-safe
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)      215 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/requires.txt
+-rw-r--r--   0 tomcat   (11236) tomcat   (13030)        5 2020-10-09 11:40:29.000000 ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/top_level.txt
```

### Comparing `ncbi-datasets-pylib-9.0.0/LICENSE.md` & `ncbi-datasets-pylib-9.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/PKG-INFO` & `ncbi-datasets-pylib-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbi-datasets-pylib
-Version: 9.0.0
+Version: 9.1.0
 Summary: Easily gather data from across NCBI databases
 Home-page: https://www.ncbi.nlm.nih.gov/datasets
 Maintainer: NCBI
 Maintainer-email: info@ncbi.nlm.nih.gov
 License: Public Domain
 Description: # Welcome to NCBI Datasets
```

### Comparing `ncbi-datasets-pylib-9.0.0/README.md` & `ncbi-datasets-pylib-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/setup.cfg` & `ncbi-datasets-pylib-9.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 	src/**/*
 
 [bdist_wheel]
 universal = true
 
 [auto-version]
 type = fixed
-value = v9.0.0
+value = v9.1.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/__init__.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/gene_api.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/gene_api.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/genome_api.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/genome_api.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api/virus_api.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api/virus_api.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/api_client.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/api_client.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/bio_dataset.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/bio_dataset.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/components/sequence.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/components/sequence.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/configuration.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/configuration.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/exceptions.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/exceptions.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/__init__.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/assembly_dataset_request_resolution.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/assembly_dataset_request_resolution.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/assembly_metadata_request_accessions.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/assembly_metadata_request_accessions.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/datasetsv1alpha1_error.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/datasetsv1alpha1_error.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/download_summary_dehydrated.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/download_summary_dehydrated.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/download_summary_hydrated.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/download_summary_hydrated.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_assembly_error_code.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_assembly_error_code.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_gene_error_code.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_gene_error_code.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_replaced_id.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_replaced_id.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/error_virus_error_code.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/error_virus_error_code.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gatewayruntime_error.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gatewayruntime_error.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_fasta.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_fasta.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_sort.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_sort.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_sort_direction.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_sort_direction.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_sort_field.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_sort_field.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_dataset_request_symbols_for_taxon.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_dataset_request_symbols_for_taxon.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_descriptor_gene_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_descriptor_gene_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/gene_descriptor_rna_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/gene_descriptor_rna_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/genomic_region_genomic_region_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/genomic_region_genomic_region_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/micro_bigge_dataset_request_element_flank_config.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/micro_bigge_dataset_request_element_flank_config.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_count_by_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_count_by_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_count_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_count_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_counts.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_counts.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/organism_rank_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/organism_rank_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/protobuf_any.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/runtime_stream_error.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/runtime_stream_error.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/sci_name_and_ids_sci_name_and_id.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/sci_name_and_ids_sci_name_and_id.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/stream_result_of_v1alpha1_tabular_output.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/stream_result_of_v1alpha1_tabular_output.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/transcript_transcript_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/transcript_transcript_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_file.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_file.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_assembly_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_annotation_for_virus_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_annotation_for_virus_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_availability.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_availability.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptor.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptor.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_filter.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_filter.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_request_content_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_descriptors_request_content_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_request.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_dataset_request.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_match.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_match.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata_request_content_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_assembly_metadata_request_content_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_download_summary.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_download_summary.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request_content_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_dataset_request_content_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_descriptor.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_descriptor.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_descriptors.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_descriptors.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_match.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_match.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_gene_metadata.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_gene_metadata.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_genomic_region.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_genomic_region.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_mature_peptide.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_mature_peptide.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_message.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_message.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_micro_bigge_dataset_request_file_type.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_micro_bigge_dataset_request_file_type.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_nomenclature_authority.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_nomenclature_authority.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_organism.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_organism.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_orientation.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_orientation.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_protein.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_protein.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_range.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_range.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_sci_name_and_ids.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_sci_name_and_ids.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_seq_range_set.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_seq_range_set.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_tabular_output.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_tabular_output.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_transcript.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_transcript.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/models/v1alpha1_virus_table_field.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/models/v1alpha1_virus_table_field.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/package/dataset.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/package/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,44 @@
+import contextlib
 import json
 import logging
 import os
+from typing import Any, Dict
 import zipfile
-import contextlib
 
 from ncbi.datasets.reports.report_reader import DatasetsReportReader
 import ncbi.datasets.v1alpha1.reports.assembly_pb2 as assembly_report_pb2
 import ncbi.datasets.v1alpha1.reports.gene_pb2 as gene_report_pb2
 
 logger = logging.getLogger()
 
 
-def GetDatasetFromFile(zip_file_or_directory, dataset_type):  # pylint:disable=invalid-name
+def GetDatasetFromFile(zip_file_or_directory, dataset_type: str):  # pylint:disable=invalid-name
     if dataset_type == 'ASSEMBLY':
         return AssemblyDataset(zip_file_or_directory)
     elif dataset_type == 'GENE':
         return GeneDataset(zip_file_or_directory)
     elif dataset_type == 'VIRUS':
         return VirusDataset(zip_file_or_directory)
     raise ValueError(dataset_type)
 
 
-def _get_files_of_type(elt, file_type, results):
+def _get_files_of_type(elt: Dict[str, Any], file_type, results):
     if isinstance(elt, dict):
         for k, v in elt.items():
             if k == 'files' and isinstance(v, list):
                 results.extend([f['filePath'] for f in v if f['fileType'] == file_type])
             else:
                 _get_files_of_type(v, file_type, results)
     elif isinstance(elt, list):
         for v in elt:
             _get_files_of_type(v, file_type, results)
 
 
-def _get_file_types(elt, results):
+def _get_file_types(elt: Dict[str, Any], results):
     if isinstance(elt, dict):
         for k, v in elt.items():
             if k == 'files' and isinstance(v, list):
                 results.update([f['fileType'] for f in v])
             else:
                 _get_file_types(v, results)
     elif isinstance(elt, list):
@@ -54,15 +55,14 @@
     def __init__(self, zipfile_or_directory):
         self.report_reader = DatasetsReportReader()
         # Zip file object - is 'None' if dataset is not stored in a zip file
         self.dataset_zip = None
         # Top-level directory for files. If data is stored in a zip file this is the data
         # directory in the zip file (ncbi_dataset/data), otherwise it's the full data directory path.
         self.dataset_dir = None
-        self._dataset_catalog = {}
 
         if os.path.isdir(zipfile_or_directory):
             self.dataset_dir = os.path.join(zipfile_or_directory, 'data')
         elif os.path.isfile(zipfile_or_directory):
             try:
                 self.dataset_zip = zipfile.ZipFile(zipfile_or_directory)
                 self.dataset_dir = 'ncbi_dataset/data'
@@ -76,25 +76,23 @@
         return bool(self.dataset_zip)
 
     # Return top-level data directory
     def get_file_root_dir(self):
         return self.dataset_dir
 
     # return json catalog from zip file
-    def get_catalog(self):
-        if self._dataset_catalog:
-            return self._dataset_catalog
-
+    def get_catalog(self) -> Dict[str, Any]:
+        dataset_catalog: Dict[str, Any]
         catalog_file = self.get_file_content('dataset_catalog.json')
         if catalog_file:
             try:
-                self._dataset_catalog = json.loads(catalog_file)
+                dataset_catalog = json.loads(catalog_file)
             except json.JSONDecodeError as e:
                 logger.error('Error decoding dataset_catalog file to json: %s', e)
-        return self._dataset_catalog
+        return dataset_catalog
 
     # return names of all files of type 'file_type', eg. 'PROTEIN_FASTA'
     def get_file_names_by_type(self, file_type):
         results = []
         catalog = self.get_catalog()
         _get_files_of_type(catalog, file_type, results)
         return results
```

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/reports/report_reader.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/reports/report_reader.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/rest.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/rest.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/catalog_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/datasets_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/datasets_pb2.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2_grpc.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/datasets_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/assembly_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/assembly_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='ncbi/datasets/v1alpha1/reports/assembly.proto',
   package='ncbi.datasets.v1alpha1.reports',
   syntax='proto3',
   serialized_options=b'Z\036ncbi/datasets/v1alpha1/reports\370\001\001',
-  serialized_pb=b'\n-ncbi/datasets/v1alpha1/reports/assembly.proto\x12\x1encbi.datasets.v1alpha1.reports\"\xcb\x04\n\x12\x41ssemblyDataReport\x12\x13\n\x0b\x63ommon_name\x18\x01 \x01(\t\x12\x14\n\x0cspecies_name\x18\x02 \x01(\t\x12\r\n\x05\x62reed\x18\x03 \x01(\t\x12\x10\n\x08\x63ultivar\x18\x04 \x01(\t\x12\x0f\n\x07\x65\x63otype\x18\x05 \x01(\t\x12\x0f\n\x07isolate\x18\x06 \x01(\t\x12\x0b\n\x03sex\x18\x07 \x01(\t\x12\x0e\n\x06strain\x18\x08 \x01(\t\x12\x0e\n\x06tax_id\x18\t \x01(\r\x12\x43\n\rassembly_info\x18\n \x01(\x0b\x32,.ncbi.datasets.v1alpha1.reports.AssemblyInfo\x12\x45\n\x0e\x61ssembly_stats\x18\x0b \x01(\x0b\x32-.ncbi.datasets.v1alpha1.reports.AssemblyStats\x12\x45\n\x0eorganelle_info\x18\x0c \x03(\x0b\x32-.ncbi.datasets.v1alpha1.reports.OrganelleInfo\x12G\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32..ncbi.datasets.v1alpha1.reports.AnnotationInfo\x12\x39\n\x08wgs_info\x18\x0e \x01(\x0b\x32\'.ncbi.datasets.v1alpha1.reports.WGSInfo\x12\x43\n\rsequence_info\x18\x0f \x03(\x0b\x32,.ncbi.datasets.v1alpha1.reports.SequenceInfo\"\x9a\x01\n\x0eSequenceReport\x12\x43\n\rassembly_info\x18\x01 \x01(\x0b\x32,.ncbi.datasets.v1alpha1.reports.AssemblyInfo\x12\x43\n\rsequence_info\x18\x02 \x03(\x0b\x32,.ncbi.datasets.v1alpha1.reports.SequenceInfo\"\xa6\x02\n\x0c\x41ssemblyInfo\x12\x16\n\x0e\x61ssembly_level\x18\x01 \x01(\t\x12\x15\n\rassembly_name\x18\x02 \x01(\t\x12\x15\n\rassembly_type\x18\x03 \x01(\t\x12\x12\n\nbioproject\x18\x04 \x01(\t\x12\x17\n\x0fsubmission_date\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x18\n\x10genbank_assm_acc\x18\x07 \x01(\t\x12\x11\n\tsubmitter\x18\x08 \x01(\t\x12\x17\n\x0frefseq_category\x18\t \x01(\t\x12\x17\n\x0frefseq_assm_acc\x18\n \x01(\t\x12\x16\n\x0eucsc_assm_name\x18\x0b \x01(\t\x12\x17\n\x0flinked_assembly\x18\x0c \x01(\t\"\xcb\x02\n\rAssemblyStats\x12#\n\x1btotal_number_of_chromosomes\x18\x01 \x01(\r\x12\x1d\n\x15total_sequence_length\x18\x02 \x01(\x04\x12\x1d\n\x15total_ungapped_length\x18\x03 \x01(\x04\x12\x19\n\x11number_of_contigs\x18\x04 \x01(\r\x12\x12\n\ncontig_n50\x18\x05 \x01(\r\x12\x12\n\ncontig_l50\x18\x06 \x01(\r\x12\x1b\n\x13number_of_scaffolds\x18\x07 \x01(\r\x12\x14\n\x0cscaffold_n50\x18\x08 \x01(\r\x12\x14\n\x0cscaffold_l50\x18\t \x01(\r\x12$\n\x1cgaps_between_scaffolds_count\x18\n \x01(\r\x12%\n\x1dnumber_of_component_sequences\x18\x0b \x01(\r\"\x98\x01\n\rOrganelleInfo\x12\x15\n\rassembly_name\x18\x01 \x01(\t\x12\x1a\n\x12infraspecific_name\x18\x02 \x01(\t\x12\x12\n\nbioproject\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x18\n\x10total_seq_length\x18\x05 \x01(\x04\x12\x11\n\tsubmitter\x18\x06 \x01(\t\"\x80\x02\n\x0cSequenceInfo\x12\x15\n\rsequence_name\x18\x01 \x01(\t\x12\x15\n\rsequence_role\x18\x02 \x01(\t\x12\x10\n\x08\x63hr_name\x18\x03 \x01(\t\x12\x17\n\x0fucsc_style_name\x18\x04 \x01(\t\x12\x12\n\nsort_order\x18\x05 \x01(\r\x12\'\n\x1f\x61ssigned_molecule_location_type\x18\x06 \x01(\t\x12\x18\n\x10refseq_accession\x18\x07 \x01(\t\x12\x15\n\rassembly_unit\x18\x08 \x01(\t\x12\x0e\n\x06length\x18\t \x01(\r\x12\x19\n\x11genbank_accession\x18\n \x01(\t\"\x96\x01\n\x0e\x41nnotationInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x14\n\x0crelease_date\x18\x03 \x01(\t\x12\x12\n\nreport_url\x18\x04 \x01(\t\x12<\n\x05stats\x18\x05 \x01(\x0b\x32-.ncbi.datasets.v1alpha1.reports.FeatureCounts\"P\n\rFeatureCounts\x12?\n\x0bgene_counts\x18\x01 \x01(\x0b\x32*.ncbi.datasets.v1alpha1.reports.GeneCounts\"j\n\nGeneCounts\x12\r\n\x05total\x18\x01 \x01(\r\x12\x16\n\x0eprotein_coding\x18\x02 \x01(\r\x12\x12\n\nnon_coding\x18\x03 \x01(\r\x12\x12\n\npseudogene\x18\x04 \x01(\r\x12\r\n\x05other\x18\x05 \x01(\r\"Y\n\x07WGSInfo\x12\x1d\n\x15wgs_project_accession\x18\x01 \x01(\t\x12\x16\n\x0emaster_wgs_url\x18\x02 \x01(\t\x12\x17\n\x0fwgs_contigs_url\x18\x03 \x01(\tB#Z\x1encbi/datasets/v1alpha1/reports\xf8\x01\x01\x62\x06proto3'
+  serialized_pb=b'\n-ncbi/datasets/v1alpha1/reports/assembly.proto\x12\x1encbi.datasets.v1alpha1.reports\"\x86\x04\n\x12\x41ssemblyDataReport\x12\x13\n\x0b\x63ommon_name\x18\x01 \x01(\t\x12\x14\n\x0cspecies_name\x18\x02 \x01(\t\x12\r\n\x05\x62reed\x18\x03 \x01(\t\x12\x10\n\x08\x63ultivar\x18\x04 \x01(\t\x12\x0f\n\x07\x65\x63otype\x18\x05 \x01(\t\x12\x0f\n\x07isolate\x18\x06 \x01(\t\x12\x0b\n\x03sex\x18\x07 \x01(\t\x12\x0e\n\x06strain\x18\x08 \x01(\t\x12\x0e\n\x06tax_id\x18\t \x01(\r\x12\x43\n\rassembly_info\x18\n \x01(\x0b\x32,.ncbi.datasets.v1alpha1.reports.AssemblyInfo\x12\x45\n\x0e\x61ssembly_stats\x18\x0b \x01(\x0b\x32-.ncbi.datasets.v1alpha1.reports.AssemblyStats\x12\x45\n\x0eorganelle_info\x18\x0c \x03(\x0b\x32-.ncbi.datasets.v1alpha1.reports.OrganelleInfo\x12G\n\x0f\x61nnotation_info\x18\r \x01(\x0b\x32..ncbi.datasets.v1alpha1.reports.AnnotationInfo\x12\x39\n\x08wgs_info\x18\x0e \x01(\x0b\x32\'.ncbi.datasets.v1alpha1.reports.WGSInfo\"U\n\x0eSequenceReport\x12\x43\n\rsequence_info\x18\x01 \x03(\x0b\x32,.ncbi.datasets.v1alpha1.reports.SequenceInfo\"\xa6\x02\n\x0c\x41ssemblyInfo\x12\x16\n\x0e\x61ssembly_level\x18\x01 \x01(\t\x12\x15\n\rassembly_name\x18\x02 \x01(\t\x12\x15\n\rassembly_type\x18\x03 \x01(\t\x12\x12\n\nbioproject\x18\x04 \x01(\t\x12\x17\n\x0fsubmission_date\x18\x05 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x18\n\x10genbank_assm_acc\x18\x07 \x01(\t\x12\x11\n\tsubmitter\x18\x08 \x01(\t\x12\x17\n\x0frefseq_category\x18\t \x01(\t\x12\x17\n\x0frefseq_assm_acc\x18\n \x01(\t\x12\x16\n\x0eucsc_assm_name\x18\x0b \x01(\t\x12\x17\n\x0flinked_assembly\x18\x0c \x01(\t\"\xcb\x02\n\rAssemblyStats\x12#\n\x1btotal_number_of_chromosomes\x18\x01 \x01(\r\x12\x1d\n\x15total_sequence_length\x18\x02 \x01(\x04\x12\x1d\n\x15total_ungapped_length\x18\x03 \x01(\x04\x12\x19\n\x11number_of_contigs\x18\x04 \x01(\r\x12\x12\n\ncontig_n50\x18\x05 \x01(\r\x12\x12\n\ncontig_l50\x18\x06 \x01(\r\x12\x1b\n\x13number_of_scaffolds\x18\x07 \x01(\r\x12\x14\n\x0cscaffold_n50\x18\x08 \x01(\r\x12\x14\n\x0cscaffold_l50\x18\t \x01(\r\x12$\n\x1cgaps_between_scaffolds_count\x18\n \x01(\r\x12%\n\x1dnumber_of_component_sequences\x18\x0b \x01(\r\"\x98\x01\n\rOrganelleInfo\x12\x15\n\rassembly_name\x18\x01 \x01(\t\x12\x1a\n\x12infraspecific_name\x18\x02 \x01(\t\x12\x12\n\nbioproject\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x18\n\x10total_seq_length\x18\x05 \x01(\x04\x12\x11\n\tsubmitter\x18\x06 \x01(\t\"\xd2\x01\n\x0cSequenceInfo\x12\x10\n\x08\x63hr_name\x18\x03 \x01(\t\x12\x17\n\x0fucsc_style_name\x18\x04 \x01(\t\x12\x12\n\nsort_order\x18\x05 \x01(\r\x12\'\n\x1f\x61ssigned_molecule_location_type\x18\x06 \x01(\t\x12\x18\n\x10refseq_accession\x18\x07 \x01(\t\x12\x15\n\rassembly_unit\x18\x08 \x01(\t\x12\x0e\n\x06length\x18\t \x01(\r\x12\x19\n\x11genbank_accession\x18\n \x01(\t\"\x96\x01\n\x0e\x41nnotationInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x14\n\x0crelease_date\x18\x03 \x01(\t\x12\x12\n\nreport_url\x18\x04 \x01(\t\x12<\n\x05stats\x18\x05 \x01(\x0b\x32-.ncbi.datasets.v1alpha1.reports.FeatureCounts\"P\n\rFeatureCounts\x12?\n\x0bgene_counts\x18\x01 \x01(\x0b\x32*.ncbi.datasets.v1alpha1.reports.GeneCounts\"j\n\nGeneCounts\x12\r\n\x05total\x18\x01 \x01(\r\x12\x16\n\x0eprotein_coding\x18\x02 \x01(\r\x12\x12\n\nnon_coding\x18\x03 \x01(\r\x12\x12\n\npseudogene\x18\x04 \x01(\r\x12\r\n\x05other\x18\x05 \x01(\r\"Y\n\x07WGSInfo\x12\x1d\n\x15wgs_project_accession\x18\x01 \x01(\t\x12\x16\n\x0emaster_wgs_url\x18\x02 \x01(\t\x12\x17\n\x0fwgs_contigs_url\x18\x03 \x01(\tB#Z\x1encbi/datasets/v1alpha1/reports\xf8\x01\x01\x62\x06proto3'
 )
 
 
 
 
 _ASSEMBLYDATAREPORT = _descriptor.Descriptor(
   name='AssemblyDataReport',
@@ -125,55 +125,41 @@
     _descriptor.FieldDescriptor(
       name='wgs_info', full_name='ncbi.datasets.v1alpha1.reports.AssemblyDataReport.wgs_info', index=13,
       number=14, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='sequence_info', full_name='ncbi.datasets.v1alpha1.reports.AssemblyDataReport.sequence_info', index=14,
-      number=15, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=82,
-  serialized_end=669,
+  serialized_end=600,
 )
 
 
 _SEQUENCEREPORT = _descriptor.Descriptor(
   name='SequenceReport',
   full_name='ncbi.datasets.v1alpha1.reports.SequenceReport',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='assembly_info', full_name='ncbi.datasets.v1alpha1.reports.SequenceReport.assembly_info', index=0,
-      number=1, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='sequence_info', full_name='ncbi.datasets.v1alpha1.reports.SequenceReport.sequence_info', index=1,
-      number=2, type=11, cpp_type=10, label=3,
+      name='sequence_info', full_name='ncbi.datasets.v1alpha1.reports.SequenceReport.sequence_info', index=0,
+      number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
@@ -182,16 +168,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=672,
-  serialized_end=826,
+  serialized_start=602,
+  serialized_end=687,
 )
 
 
 _ASSEMBLYINFO = _descriptor.Descriptor(
   name='AssemblyInfo',
   full_name='ncbi.datasets.v1alpha1.reports.AssemblyInfo',
   filename=None,
@@ -290,16 +276,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=829,
-  serialized_end=1123,
+  serialized_start=690,
+  serialized_end=984,
 )
 
 
 _ASSEMBLYSTATS = _descriptor.Descriptor(
   name='AssemblyStats',
   full_name='ncbi.datasets.v1alpha1.reports.AssemblyStats',
   filename=None,
@@ -391,16 +377,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1126,
-  serialized_end=1457,
+  serialized_start=987,
+  serialized_end=1318,
 )
 
 
 _ORGANELLEINFO = _descriptor.Descriptor(
   name='OrganelleInfo',
   full_name='ncbi.datasets.v1alpha1.reports.OrganelleInfo',
   filename=None,
@@ -457,91 +443,77 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1460,
-  serialized_end=1612,
+  serialized_start=1321,
+  serialized_end=1473,
 )
 
 
 _SEQUENCEINFO = _descriptor.Descriptor(
   name='SequenceInfo',
   full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
     _descriptor.FieldDescriptor(
-      name='sequence_name', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.sequence_name', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='sequence_role', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.sequence_role', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR),
-    _descriptor.FieldDescriptor(
-      name='chr_name', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.chr_name', index=2,
+      name='chr_name', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.chr_name', index=0,
       number=3, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='ucsc_style_name', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.ucsc_style_name', index=3,
+      name='ucsc_style_name', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.ucsc_style_name', index=1,
       number=4, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='sort_order', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.sort_order', index=4,
+      name='sort_order', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.sort_order', index=2,
       number=5, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='assigned_molecule_location_type', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.assigned_molecule_location_type', index=5,
+      name='assigned_molecule_location_type', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.assigned_molecule_location_type', index=3,
       number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='refseq_accession', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.refseq_accession', index=6,
+      name='refseq_accession', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.refseq_accession', index=4,
       number=7, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='assembly_unit', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.assembly_unit', index=7,
+      name='assembly_unit', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.assembly_unit', index=5,
       number=8, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='length', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.length', index=8,
+      name='length', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.length', index=6,
       number=9, type=13, cpp_type=3, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
     _descriptor.FieldDescriptor(
-      name='genbank_accession', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.genbank_accession', index=9,
+      name='genbank_accession', full_name='ncbi.datasets.v1alpha1.reports.SequenceInfo.genbank_accession', index=7,
       number=10, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
@@ -551,16 +523,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1615,
-  serialized_end=1871,
+  serialized_start=1476,
+  serialized_end=1686,
 )
 
 
 _ANNOTATIONINFO = _descriptor.Descriptor(
   name='AnnotationInfo',
   full_name='ncbi.datasets.v1alpha1.reports.AnnotationInfo',
   filename=None,
@@ -610,16 +582,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1874,
-  serialized_end=2024,
+  serialized_start=1689,
+  serialized_end=1839,
 )
 
 
 _FEATURECOUNTS = _descriptor.Descriptor(
   name='FeatureCounts',
   full_name='ncbi.datasets.v1alpha1.reports.FeatureCounts',
   filename=None,
@@ -641,16 +613,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2026,
-  serialized_end=2106,
+  serialized_start=1841,
+  serialized_end=1921,
 )
 
 
 _GENECOUNTS = _descriptor.Descriptor(
   name='GeneCounts',
   full_name='ncbi.datasets.v1alpha1.reports.GeneCounts',
   filename=None,
@@ -700,16 +672,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2108,
-  serialized_end=2214,
+  serialized_start=1923,
+  serialized_end=2029,
 )
 
 
 _WGSINFO = _descriptor.Descriptor(
   name='WGSInfo',
   full_name='ncbi.datasets.v1alpha1.reports.WGSInfo',
   filename=None,
@@ -745,25 +717,23 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2216,
-  serialized_end=2305,
+  serialized_start=2031,
+  serialized_end=2120,
 )
 
 _ASSEMBLYDATAREPORT.fields_by_name['assembly_info'].message_type = _ASSEMBLYINFO
 _ASSEMBLYDATAREPORT.fields_by_name['assembly_stats'].message_type = _ASSEMBLYSTATS
 _ASSEMBLYDATAREPORT.fields_by_name['organelle_info'].message_type = _ORGANELLEINFO
 _ASSEMBLYDATAREPORT.fields_by_name['annotation_info'].message_type = _ANNOTATIONINFO
 _ASSEMBLYDATAREPORT.fields_by_name['wgs_info'].message_type = _WGSINFO
-_ASSEMBLYDATAREPORT.fields_by_name['sequence_info'].message_type = _SEQUENCEINFO
-_SEQUENCEREPORT.fields_by_name['assembly_info'].message_type = _ASSEMBLYINFO
 _SEQUENCEREPORT.fields_by_name['sequence_info'].message_type = _SEQUENCEINFO
 _ANNOTATIONINFO.fields_by_name['stats'].message_type = _FEATURECOUNTS
 _FEATURECOUNTS.fields_by_name['gene_counts'].message_type = _GENECOUNTS
 DESCRIPTOR.message_types_by_name['AssemblyDataReport'] = _ASSEMBLYDATAREPORT
 DESCRIPTOR.message_types_by_name['SequenceReport'] = _SEQUENCEREPORT
 DESCRIPTOR.message_types_by_name['AssemblyInfo'] = _ASSEMBLYINFO
 DESCRIPTOR.message_types_by_name['AssemblyStats'] = _ASSEMBLYSTATS
```

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/common_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/gene_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/gene_pb2.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/microbigge/microbigge_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/microbigge/microbigge_pb2.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi/datasets/v1alpha1/reports/virus_pb2.py` & `ncbi-datasets-pylib-9.1.0/src/ncbi/datasets/v1alpha1/reports/virus_pb2.py`

 * *Files identical despite different names*

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/PKG-INFO` & `ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbi-datasets-pylib
-Version: 9.0.0
+Version: 9.1.0
 Summary: Easily gather data from across NCBI databases
 Home-page: https://www.ncbi.nlm.nih.gov/datasets
 Maintainer: NCBI
 Maintainer-email: info@ncbi.nlm.nih.gov
 License: Public Domain
 Description: # Welcome to NCBI Datasets
```

### Comparing `ncbi-datasets-pylib-9.0.0/src/ncbi_datasets_pylib.egg-info/SOURCES.txt` & `ncbi-datasets-pylib-9.1.0/src/ncbi_datasets_pylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

