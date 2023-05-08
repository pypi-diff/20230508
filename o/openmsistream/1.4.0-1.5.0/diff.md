# Comparing `tmp/openmsistream-1.4.0.tar.gz` & `tmp/openmsistream-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmsistream-1.4.0.tar", last modified: Mon Apr 24 23:55:54 2023, max compression
+gzip compressed data, was "openmsistream-1.5.0.tar", last modified: Mon May  8 20:19:57 2023, max compression
```

## Comparing `openmsistream-1.4.0.tar` & `openmsistream-1.5.0.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-24 23:55:47.000000 openmsistream-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 23:55:47.000000 openmsistream-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-24 23:55:54.826432 openmsistream-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-24 23:55:47.000000 openmsistream-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.818432 openmsistream-1.4.0/openmsistream/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/actor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_download_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18319 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_upload_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/data_file_io/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/download_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/reproducer_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/upload_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/data_file_io/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/kafka_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test.config
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/prod.config
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test.config
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.822432 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17730 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/producible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/kafka_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/metadata_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/metadata_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_reproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/s3_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/s3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/services/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/services/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/examples/runnable_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/examples/script_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/install_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/linux_service_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/manage_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22468 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/service_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/services/windows_service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.826432 openmsistream-1.4.0/openmsistream/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21362 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/controlled_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/controlled_process_multi_threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/controlled_process_single_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    22465 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/dataclass_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/exception_tracking_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/has_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/has_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/provision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-24 23:55:47.000000 openmsistream-1.4.0/openmsistream/utilities/runnable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:55:54.818432 openmsistream-1.4.0/openmsistream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 23:55:54.000000 openmsistream-1.4.0/openmsistream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-24 23:55:47.000000 openmsistream-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-24 23:55:54.826432 openmsistream-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-24 23:55:47.000000 openmsistream-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.553995 openmsistream-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-08 20:19:51.000000 openmsistream-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-08 20:19:51.000000 openmsistream-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-08 20:19:57.553995 openmsistream-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-08 20:19:51.000000 openmsistream-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream/data_file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream/data_file_io/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_download_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31418 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_upload_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.541995 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.541995 openmsistream-1.5.0/openmsistream/data_file_io/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/download_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/reproducer_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/data_file_io/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.541995 openmsistream-1.5.0/openmsistream/kafka_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/prod.config
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/producible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/kafka_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.545995 openmsistream-1.5.0/openmsistream/metadata_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/metadata_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_reproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.549995 openmsistream-1.5.0/openmsistream/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/s3_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/s3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.549995 openmsistream-1.5.0/openmsistream/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.549995 openmsistream-1.5.0/openmsistream/services/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/examples/runnable_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/examples/script_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/install_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/linux_service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/manage_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/service_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/services/windows_service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.553995 openmsistream-1.5.0/openmsistream/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22161 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/controlled_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/controlled_process_multi_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/controlled_process_single_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/dataclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/exception_tracking_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/has_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/has_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/provision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-08 20:19:51.000000 openmsistream-1.5.0/openmsistream/utilities/runnable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:19:57.537995 openmsistream-1.5.0/openmsistream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 20:19:57.000000 openmsistream-1.5.0/openmsistream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 20:19:51.000000 openmsistream-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-08 20:19:57.553995 openmsistream-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-08 20:19:51.000000 openmsistream-1.5.0/setup.py
```

### Comparing `openmsistream-1.4.0/LICENSE` & `openmsistream-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/PKG-INFO` & `openmsistream-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.0.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.4.0/README.md` & `openmsistream-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # <div align="center"> OpenMSIStream </div>
-#### <div align="center">***v1.4.0***</div>
+#### <div align="center">***v1.5.0***</div>
 
 #### <div align="center">Maggie Eminizer<sup>1</sup>, Sam Tabrisky<sup>2,3,4</sup>, Amir Sharifzadeh<sup>1</sup>, Christopher DiMarco<sup>4</sup>, Jacob M. Diamond<sup>4,6</sup>, K.T. Ramesh<sup>4</sup>, Todd C. Hufnagel<sup>4,5,6</sup>, Tyrel M. McQueen<sup>4,5,7,8</sup>, David Elbert<sup>1,4</sup></div>
 
  <div align="center"><sup>1</sup> Institute for Data Intensive Engineering and Science (IDIES), The Johns Hopkins University, Baltimore, MD, USA </div>
  <div align="center"><sup>2</sup> Department of Biology, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>3</sup> Department of Computer Science, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>4</sup> Hopkins Extreme Materials Institute (HEMI), The Johns Hopkins University, Baltimore, MD, USA </div>
```

### Comparing `openmsistream-1.4.0/openmsistream/__init__.py` & `openmsistream-1.5.0/openmsistream/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
                 CDLL(str(fp))
         if len(fps) < 1:
             reason = f"{dll_dir} does not contain any librdkafka DLL files to preload!"
         if reason is not None:
             print(f"WARNING: Failed to preload librdkafka DLLs. Reason: {reason}")
         try:
             import confluent_kafka
-        except Exception as e:
+        except Exception as exc:
             errmsg = "ERROR: Preloading librdkafka DLLs ("
             errmsg += ", ".join([str(_) for _ in fps])
             errmsg += (
                 f"{errmsg}) did not allow confluent_kafka to be imported! "
                 f"Exception (will be re-raised): {traceback.format_exc()}"
             )
             print(errmsg)
-            raise e
+            raise exc
     _ = confluent_kafka.Producer  # appease pyflakes
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/__init__.py` & `openmsistream-1.5.0/openmsistream/data_file_io/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 """
 
 from .entity.data_file import DataFile
 from .entity.download_data_file import (
     DownloadDataFile,
     DownloadDataFileToDisk,
     DownloadDataFileToMemory,
+    DownloadDataFileToMemoryAndDisk,
 )
 from .entity.data_file_directory import DataFileDirectory
 from .entity.reproducer_message import ReproducerMessage
 
 __all__ = [
     "DataFile",
     "DownloadDataFile",
     "DownloadDataFileToDisk",
     "DownloadDataFileToMemory",
+    "DownloadDataFileToMemoryAndDisk",
     "DataFileDirectory",
     "ReproducerMessage",
 ]
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_chunk_handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         datafile_type = the type of datafile that the consumed messages will be used to create
             (must be a subclass of DownloadDataFile)
         """
         super().__init__(*args, **kwargs)
         self.datafile_type = datafile_type
         if not issubclass(self.datafile_type, DownloadDataFile):
             errmsg = (
-                "ERROR: DataFileChunkProcessor requires a datafile_type that is a subclass"
-                f" of DownloadDataFile but {self.datafile_type} was given!"
+                f"ERROR: {self.__class__.__name__} requires a datafile_type that is "
+                f"a subclass of DownloadDataFile but {self.datafile_type} was given!"
             )
             raise ValueError(errmsg)
         self.files_in_progress_by_path = {}
         self.locks_by_fp = {}
         self.recent_processed_filepaths = []
         self.n_processed_files = 0
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_download_directory.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_download_directory.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,35 +26,44 @@
         and Consumers
     :type config_path: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
     :type topic_name: str
     :param datafile_type: the type of data file that recognized files should be reconstructed as
         (must be a subclass of :class:`~.data_file_io.DownloadDataFileToDisk`)
     :type datafile_type: :class:`~.data_file_io.DownloadDataFileToDisk`, optional
+    :param filepath_regex: If given, only messages associated with files whose paths match
+        this regex will be consumed
+    :type filepath_regex: :type filepath_regex: :func:`re.compile` or None, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
         :class:`~.data_file_io.DownloadDataFileToDisk`
     """
 
     #################### PUBLIC FUNCTIONS ####################
 
     def __init__(
         self,
         dirpath,
         config_path,
         topic_name,
         datafile_type=DownloadDataFileToDisk,
+        filepath_regex=None,
         **kwargs,
     ):
         """
         datafile_type = the type of datafile that the consumed messages are from
         In this class datafile_type should be something that extends DownloadDataFileToDisk
         """
         super().__init__(
-            dirpath, config_path, topic_name, datafile_type=datafile_type, **kwargs
+            dirpath,
+            config_path,
+            topic_name,
+            datafile_type=datafile_type,
+            filepath_regex=filepath_regex,
+            **kwargs,
         )
         if not issubclass(self.datafile_type, DownloadDataFileToDisk):
             errmsg = (
                 "ERROR: DataFileDownloadDirectory requires a datafile_type that is a "
                 f"subclass of DownloadDataFileToDisk but {self.datafile_type} was given!"
             )
             self.logger.error(errmsg, exc_type=ValueError)
@@ -181,14 +190,15 @@
         args = [
             *superargs,
             "output_dir",
             "config",
             "topic_name",
             "update_seconds",
             "consumer_group_id",
+            "download_regex",
         ]
         kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
         return args, kwargs
 
     @classmethod
     def run_from_command_line(cls, args=None):
         """
@@ -205,14 +215,15 @@
         args = parser.parse_args(args=args)
         # make the download directory
         reconstructor_directory = cls(
             args.output_dir,
             args.config,
             args.topic_name,
             n_threads=args.n_threads,
+            filepath_regex=args.download_regex,
             consumer_group_id=args.consumer_group_id,
             update_secs=args.update_seconds,
             streamlevel=args.logger_stream_level,
             filelevel=args.logger_file_level,
         )
         # start the reconstructor running
         run_start = datetime.datetime.now()
@@ -238,17 +249,17 @@
                 f'{n_complete_files} file{" was" if n_complete_files==1 else "s were"} '
                 "successfully reconstructed"
             )
         else:
             msg += f" and {n_processed} messages were successfully processed"
         msg += (
             f" from {run_start} to {run_stop}\n"
-            f"Most recent completed files (up to {cls.N_RECENT_FILES}):"
+            f"Most recent completed files (up to {cls.N_RECENT_FILES}):\n\t"
         )
-        msg += "\n\t".join(complete_filepaths)
+        msg += "\n\t".join([str(filepath) for filepath in complete_filepaths])
         reconstructor_directory.logger.info(msg)
 
 
 def main(args=None):
     """
     Main method to run from command line
     """
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_handler.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,45 +10,67 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     from kafkacrypto.message import KafkaCryptoMessage
 from ...utilities.misc import populated_kwargs
 from ...utilities import Runnable
 from ..config import DATA_FILE_HANDLING_CONST
 from ..utilities import get_encrypted_message_timestamp_string
-from ..entity.download_data_file import DownloadDataFileToMemory
+from ..entity.download_data_file import (
+    DownloadDataFileToMemory,
+    DownloadDataFileToDisk,
+    DownloadDataFileToMemoryAndDisk,
+)
 from .data_file_chunk_handlers import DataFileChunkHandler
 
 
 class DataFileStreamHandler(DataFileChunkHandler, Runnable, ABC):
     """
     Generic base class for consuming file chunks into memory and then doing something
     once entire files are available
     """
 
+    LOG_SUBDIR_NAME = "LOGS"  # name of the directory that holds the logs
+
     def __init__(
-        self, *args, output_dir=None, datafile_type=DownloadDataFileToMemory, **kwargs
+        self, *args, output_dir=None, mode="memory", datafile_type=None, **kwargs
     ):
         """
         Constructor method
         """
         # make sure the directory for the output is set
         self._output_dir = (
             self._get_auto_output_dir() if output_dir is None else output_dir
         )
         if not self._output_dir.is_dir():
             self._output_dir.mkdir(parents=True)
-        kwargs = populated_kwargs(kwargs, {"logger_file": self._output_dir})
-        super().__init__(*args, datafile_type=datafile_type, **kwargs)
-        self.logger.info(f"Log files and output will be in {self._output_dir}")
-        if not issubclass(datafile_type, DownloadDataFileToMemory):
+        # create a subdirectory for the logs
+        self._logs_subdir = self._output_dir / self.LOG_SUBDIR_NAME
+        if not self._logs_subdir.is_dir():
+            self._logs_subdir.mkdir(parents=True)
+        # put the log file in the subdirectory
+        kwargs = populated_kwargs(kwargs, {"logger_file": self._logs_subdir})
+        # figure out or check the datafile type from the "mode" argument
+        if mode == "memory":
+            base_datafile_type = DownloadDataFileToMemory
+        elif mode == "disk":
+            base_datafile_type = DownloadDataFileToDisk
+        elif mode == "both":
+            base_datafile_type = DownloadDataFileToMemoryAndDisk
+        else:
+            raise ValueError(f"ERROR: unrecognized mode argument '{mode}'")
+        if not datafile_type:
+            datafile_type = base_datafile_type
+        if not issubclass(datafile_type, base_datafile_type):
             errmsg = (
                 f"ERROR: {self.__class__.__name__} requires a datafile_type that is a "
-                f"subclass of DownloadDataFileToMemory but {datafile_type} was given!"
+                f"subclass of {base_datafile_type} but {datafile_type} was given!"
             )
-            self.logger.error(errmsg, exc_type=ValueError)
+            raise ValueError(errmsg)
+        super().__init__(*args, datafile_type=datafile_type, **kwargs)
+        self.logger.info(f"Log files and output will be in {self._output_dir}")
         self.file_registry = None  # needs to be set in subclasses
 
     def _process_message(self, lock, msg, rootdir_to_set=None):
         """
         Parent class message processing function to check for:
             undecryptable messages (returns False)
             files where reconstruction is just in progress (returns True)
@@ -146,13 +168,13 @@
     @classmethod
     def _get_auto_output_dir(cls):
         return pathlib.Path() / f"{cls.__name__}_output"
 
     @classmethod
     def get_command_line_arguments(cls):
         superargs, superkwargs = super().get_command_line_arguments()
-        args = [*superargs, "config", "consumer_group_id", "update_seconds"]
+        args = [*superargs, "config", "consumer_group_id", "update_seconds", "mode"]
         kwargs = {
             **superkwargs,
             "optional_output_dir": cls._get_auto_output_dir(),
         }
         return args, kwargs
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_processor.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """A DataFileStreamHandler that triggers some arbitrary local code when full files are available"""
 
 # imports
 from abc import ABC, abstractmethod
-from ...utilities.misc import populated_kwargs
 from ..config import RUN_OPT_CONST, DATA_FILE_HANDLING_CONST
 from .data_file_chunk_handlers import DataFileChunkProcessor
 from .data_file_stream_handler import DataFileStreamHandler
 from .file_registry.stream_handler_registries import StreamProcessorRegistry
 
 
 class DataFileStreamProcessor(DataFileStreamHandler, DataFileChunkProcessor, ABC):
@@ -19,44 +18,40 @@
         and Consumers
     :type config_path: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
     :type topic_name: str
     :param output_dir: Path to the directory where the log and csv registry files should be kept
         (if None a default will be created in the current directory)
     :type output_dir: :class:`pathlib.Path`, optional
-    :param datafile_type: the type of data file that recognized files should be reconstructed as
-        (must be a subclass of :class:`~.data_file_io.DownloadDataFileToMemory`)
-    :type datafile_type: :class:`~.data_file_io.DownloadDataFileToMemory`, optional
+    :param mode: a string flag determining whether reconstructed data files should
+        have their contents stored only in "memory" (the default, and the fastest),
+        only on "disk" (in the output directory, to reduce the memory footprint),
+        or "both" (for flexibility in processing)
+    :type mode: str, optional
+    :param datafile_type: the type of data file that recognized files should be reconstructed as.
+        Default options are set automatically depending on the "mode" argument.
+        (must be a subclass of :class:`~.data_file_io.DownloadDataFile`)
+    :type datafile_type: :class:`~.data_file_io.DownloadDataFile`, optional
     :param n_threads: the number of threads/consumers to run
     :type n_threads: int, optional
     :param consumer_group_id: the group ID under which each consumer should be created
     :type consumer_group_id: str, optional
+    :param filepath_regex: If given, only messages associated with files whose paths match
+        this regex will be consumed
+    :type filepath_regex: :type filepath_regex: :func:`re.compile` or None, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
-        :class:`~.data_file_io.DownloadDataFileToMemory`
+        :class:`~.data_file_io.DownloadDataFileToMemory`, or more specific as determined
+        by the "mode" argument
     """
 
-    LOG_SUBDIR_NAME = "LOGS"
-
-    def __init__(self, config_file, topic_name, output_dir=None, **kwargs):
+    def __init__(self, config_file, topic_name, **kwargs):
         """
-        Constructor method
+        Constructor method (duplicated here for its function signature in the docs)
         """
-        # set the output directory
-        self._output_dir = (
-            self._get_auto_output_dir() if output_dir is None else output_dir
-        )
-        # create a subdirectory for the logs
-        self.__logs_subdir = self._output_dir / self.LOG_SUBDIR_NAME
-        if not self.__logs_subdir.is_dir():
-            self.__logs_subdir.mkdir(parents=True)
-        # put the log file in the subdirectory
-        kwargs = populated_kwargs(
-            kwargs, {"output_dir": self._output_dir, "logger_file": self.__logs_subdir}
-        )
         super().__init__(config_file, topic_name, **kwargs)
 
     def process_files_as_read(self):
         """
         Consumes messages and stores their data in memory.
         Uses several parallel threads to consume message and calls
         :func:`~_process_downloaded_data_file` for fully read files.
@@ -75,15 +70,15 @@
         msg = (
             f"Will process files from messages in the {self.topic_name} topic using "
             f'{self.n_threads} thread{"s" if self.n_threads>1 else ""}'
         )
         self.logger.info(msg)
         # set up the stream processor registry
         self.file_registry = StreamProcessorRegistry(
-            dirpath=self.__logs_subdir,
+            dirpath=self._logs_subdir,
             topic_name=self.topic_name,
             consumer_group_id=self.consumer_group_id,
             logger=self.logger,
         )
         # if there are files that need to be re-processed,
         # set the variables to re-read messages from those files
         if self.file_registry.rerun_file_key_regex is not None:
@@ -256,10 +251,10 @@
     def _on_shutdown(self):
         super()._on_shutdown()
         self.file_registry.consolidate_succeeded_files()
 
     @classmethod
     def get_command_line_arguments(cls):
         superargs, superkwargs = super().get_command_line_arguments()
-        args = [*superargs, "topic_name"]
+        args = [*superargs, "topic_name", "download_regex"]
         kwargs = {**superkwargs, "n_threads": RUN_OPT_CONST.N_DEFAULT_DOWNLOAD_THREADS}
         return args, kwargs
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_stream_reproducer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,38 @@
     :type consumer_topic_name: str
     :param producer_topic_name: Name of the topic to which the Producer should produce
         the processing results
     :type producer_topic_name: str
     :param output_dir: Path to the directory where the log and csv registry files should be kept
         (if None a default will be created in the current directory)
     :type output_dir: :class:`pathlib.Path`, optional
-    :param datafile_type: the type of data file that recognized files should be reconstructed as
-        (must be a subclass of :class:`~.data_file_io.DownloadDataFileToMemory`)
-    :type datafile_type: :class:`~.data_file_io.DownloadDataFileToMemory`, optional
+    :param mode: a string flag determining whether reconstructed data files should
+        have their contents stored only in "memory" (the default, and the fastest),
+        only on "disk" (in the output directory, to reduce the memory footprint),
+        or "both" (for flexibility in processing)
+    :type mode: str, optional
+    :param datafile_type: the type of data file that recognized files should be reconstructed as.
+        Default options are set automatically depending on the "mode" argument.
+        (must be a subclass of :class:`~.data_file_io.DownloadDataFile`)
+    :type datafile_type: :class:`~.data_file_io.DownloadDataFile`, optional
     :param n_producer_threads: the number of producers to run. The total number of
         producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_producer_threads: int, optional
     :param n_consumer_threads: the number of consumers to run. The total number of
         producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_consumer_threads: int, optional
     :param consumer_group_id: the group ID under which each consumer should be created
     :type consumer_group_id: str, optional
+    :param filepath_regex: If given, only messages associated with files whose paths match
+        this regex will be consumed
+    :type filepath_regex: :type filepath_regex: :func:`re.compile` or None, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
-        :class:`~.data_file_io.DownloadDataFileToMemory`
+        :class:`~.data_file_io.DownloadDataFileToMemory`, or more specific as determined
+        by the "mode" argument
     """
 
     def __init__(self, config_file, consumer_topic_name, producer_topic_name, **kwargs):
         """
         Constructor method signature duplicated above to display in Sphinx docs
         """
         super().__init__(config_file, consumer_topic_name, producer_topic_name, **kwargs)
@@ -79,15 +89,15 @@
             f'{"s" if self.n_consumer_threads>1 else ""} and produce their '
             f"processing results to the {self.producer_topic_name} topic using "
             f'{self.n_producer_threads} thread{"s" if self.n_producer_threads>1 else ""}'
         )
         self.logger.info(msg)
         # set up the stream reproducer registry
         self.file_registry = StreamReproducerRegistry(
-            dirpath=self._output_dir,
+            dirpath=self._logs_subdir,
             consumer_topic_name=self.consumer_topic_name,
             consumer_group_id=self.consumer_group_id,
             producer_topic_name=self.producer_topic_name,
             logger=self.logger,
         )
         # if there are files that need to be re-processed,
         # set the variables to re-read messages from those files
@@ -119,15 +129,14 @@
             kwargs_per_thread=run_worker_kwargs_per_thread,
         )
         # return the results of the processing
         return (
             self.n_msgs_read,
             self.n_msgs_processed,
             self.n_processed_files,
-            self.recent_processed_filepaths,
             self.n_results_produced_files,
             self.recent_results_produced,
         )
 
     def producer_callback(self, err, msg, prodid, filename, rel_filepath, n_total_chunks):
         """
         A reference to this method is given as the callback for each call to
@@ -364,10 +373,11 @@
         superargs, superkwargs = super().get_command_line_arguments()
         args = [
             *superargs,
             "consumer_topic_name",
             "producer_topic_name",
             "n_consumer_threads",
             "n_producer_threads",
+            "download_regex",
         ]
         kwargs = {**superkwargs}
         return args, kwargs
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/data_file_upload_directory.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/data_file_upload_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,33 +63,33 @@
         datafile_type=UploadDataFile,
         **kwargs,
     ):
         """
         Constructor method
         """
         # create a subdirectory for the logs
-        self.__logs_subdir = dirpath / self.LOG_SUBDIR_NAME
-        if not self.__logs_subdir.is_dir():
-            self.__logs_subdir.mkdir(parents=True)
+        self._logs_subdir = dirpath / self.LOG_SUBDIR_NAME
+        if not self._logs_subdir.is_dir():
+            self._logs_subdir.mkdir(parents=True)
         # put the log file in the subdirectory
-        kwargs = populated_kwargs(kwargs, {"logger_file": self.__logs_subdir})
+        kwargs = populated_kwargs(kwargs, {"logger_file": self._logs_subdir})
         super().__init__(dirpath, config_path, **kwargs)
         if not issubclass(datafile_type, UploadDataFile):
             errmsg = (
                 "ERROR: DataFileUploadDirectory requires a datafile_type that is a "
                 f"subclass of UploadDataFile but {datafile_type} was given!"
             )
             self.logger.error(errmsg, exc_type=ValueError)
         self.__datafile_type = datafile_type
         self.__wait_time = self.MIN_WAIT_TIME
         self.__lock = Lock()
         self.__observer = Observer(timeout=self.WATCHDOG_OBSERVER_TIMEOUT)
         self.__event_handler = UploadDirectoryEventHandler(
             upload_regex=upload_regex,
-            logs_subdir=self.__logs_subdir,
+            logs_subdir=self._logs_subdir,
             logger=self.logger,
         )
         self.__active_files_by_path = {}
         self.__status_message_files = {}
         self.__topic_name = None
         self.__chunk_size = None
         self.__file_registry = None
@@ -130,15 +130,15 @@
             f'Will upload {"files in" if upload_existing else "new files added to"}'
             f"{self.dirpath} to the {self.__topic_name} topic as "
             f"{self.__chunk_size}-byte chunks using {n_threads} threads"
         )
         self.logger.info(msg)
         # start up a file registry in the watched directory
         self.__file_registry = ProducerFileRegistry(
-            dirpath=self.__logs_subdir, topic_name=topic_name, logger=self.logger
+            dirpath=self._logs_subdir, topic_name=topic_name, logger=self.logger
         )
         # start the upload queue
         n_max_queue_items = int((1000000 * max_queue_size) / self.__chunk_size)
         self.__upload_queue = Queue(n_max_queue_items)
         # start the producers and upload threads
         for _ in range(n_threads):
             self.__producers.append(self.get_new_producer())
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,26 +116,30 @@
         ).lines
         for fp in self.completed_filepath_pattern.parent.glob(globpattern):
             if fp == self.completed_filepath_pattern:
                 continue
             added_file = DataclassTableReadOnly(
                 dataclass_type=RegistryLineCompleted, filepath=fp, logger=self.logger
             )
+            file_is_good = True
             for entry_line in added_file.lines:
                 if entry_line not in all_lines:
+                    self.logger.warning(f"missing line = {entry_line} in file {fp}")
                     warnmsg = (
                         "WARNING: failed to consolidate individual files into "
                         f"{self.completed_filepath_pattern}. Individual files will be "
                         "retained and should be manually concatenated. "
                         "Duplicate entries may be present."
                     )
                     self.logger.warning(warnmsg)
-            if fp in self.__completed_tables_by_path:
-                self.__completed_tables_by_path.pop(fp)
-            fp.unlink()
+                    file_is_good = False
+            if file_is_good:
+                if fp in self.__completed_tables_by_path:
+                    self.__completed_tables_by_path.pop(fp)
+                fp.unlink()
 
     def get_incomplete_filepaths_and_chunks(self):
         """
         Generate tuples of (rel_filepath, chunks to upload) for each file
         that has not yet been completely uploaded
         """
         for obj_address in self.__in_prog.obj_addresses:
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py` & `openmsistream-1.5.0/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/config.py` & `openmsistream-1.5.0/openmsistream/data_file_io/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file.py` & `openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file_chunk.py` & `openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_chunk.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/entity/data_file_directory.py` & `openmsistream-1.5.0/openmsistream/data_file_io/entity/data_file_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/entity/download_data_file.py` & `openmsistream-1.5.0/openmsistream/data_file_io/entity/download_data_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,25 +165,32 @@
     Class to represent a data file that will be reconstructed on disk
     using messages read from a topic
 
     :param filepath: Path to the file
     :type filepath: :class:`pathlib.Path`
     """
 
+    #################### CONSTANTS ####################
+
+    READ_BUFFER_SIZE = 4096
+
     #################### PROPERTIES ####################
 
     @property
     def check_file_hash(self):
         """
         Hash of the file contents as read from its current location on disk
         """
         check_file_hash = sha512()
         with open(self.full_filepath, "rb") as fp:
-            data = fp.read()
-        check_file_hash.update(data)
+            while True:
+                data = fp.read(self.READ_BUFFER_SIZE)
+                if not data:
+                    break
+                check_file_hash.update(data)
         return check_file_hash.digest()
 
     #################### PUBLIC FUNCTIONS ####################
 
     def __init__(self, filepath, *args, **kwargs):
         super().__init__(filepath, *args, **kwargs)
         # create the parent directory of the file if it doesn't exist yet
@@ -193,14 +200,18 @@
     def _on_add_chunk(self, dfc):
         """
         Add the data from a given file chunk to this file on disk
 
         :param dfc: the DataFileChunk object whose data should be added
         :type dfc: :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`
         """
+        try:
+            super()._on_add_chunk(dfc)
+        except NotImplementedError:
+            pass
         mode = "r+b" if self.full_filepath.is_file() else "w+b"
         with open(self.full_filepath, mode) as fp:
             fp.seek(dfc.chunk_offset_write)
             fp.write(dfc.data)
             fp.flush()
             os.fsync(fp.fileno())
             fp.close()
@@ -260,20 +271,63 @@
     def _on_add_chunk(self, dfc):
         """
         Add the data from a given file chunk to the dictionary of data by offset
 
         :param dfc: the DataFileChunk object whose data should be added
         :type dfc: :class:`~.data_file_io.entity.data_file_chunk.DataFileChunk`
         """
+        try:
+            super()._on_add_chunk(dfc)
+        except NotImplementedError:
+            pass
         self.__chunk_data_by_offset[dfc.chunk_offset_write] = dfc.data
 
     def __create_bytestring(self):
         """
         Makes all of the data held in the dictionary into a single bytestring
         """
         bytestring = b""
         for data in [
             self.__chunk_data_by_offset[offset]
             for offset in sorted(self.__chunk_data_by_offset.keys())
         ]:
             bytestring += data
         self.__bytestring = bytestring
+
+
+class DownloadDataFileToMemoryAndDisk(DownloadDataFileToMemory, DownloadDataFileToDisk):
+    """
+    A class for a file that should be written to disk as its messages are read
+    from a topic, but that should also have a bytestring created for it.
+
+    :param filepath: Path to the file
+    :type filepath: :class:`pathlib.Path`
+    """
+
+    @property
+    def check_file_hash(self):
+        """
+        Hash of the file contents as read from its current location on disk
+        and from the bytestring of the file stored in memory.
+        Raises an error if they don't match.
+        """
+        check_file_hash_memory = sha512()
+        check_file_hash_memory.update(self.bytestring)
+        check_file_hash_memory = check_file_hash_memory.digest()
+        check_file_hash_disk = sha512()
+        with open(self.full_filepath, "rb") as fp:
+            while True:
+                data = fp.read(self.READ_BUFFER_SIZE)
+                if not data:
+                    break
+                check_file_hash_disk.update(data)
+        check_file_hash_disk = check_file_hash_disk.digest()
+        if check_file_hash_disk != check_file_hash_memory:
+            errmsg = (
+                f"ERROR: hashes of file on disk and in memory are mismatched! "
+                f"On disk: {check_file_hash_disk}. In memory: {check_file_hash_memory}."
+            )
+            self.logger.error(errmsg, exc_type=ValueError)
+        return check_file_hash_disk
+
+    def __init__(self, filepath, *args, **kwargs):
+        super().__init__(filepath, *args, **kwargs)
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/entity/reproducer_message.py` & `openmsistream-1.5.0/openmsistream/data_file_io/entity/reproducer_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/entity/upload_data_file.py` & `openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py` & `openmsistream-1.5.0/openmsistream/data_file_io/entity/upload_directory_event_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     def __init__(self, upload_regex, logs_subdir, **other_kwargs):
         """
         Constructor method
         """
         super().__init__(**other_kwargs)
         # variables for determining files whose events should be dispatched
         self.__upload_regex = upload_regex
-        self.__logs_subdir = logs_subdir
-        self.__rootdir = self.__logs_subdir.parent
+        self._logs_subdir = logs_subdir
+        self.__rootdir = self._logs_subdir.parent
         # A thread lock
         self.__lock = RLock()
         # all currently active files
         self.__active_files_by_path = {}
 
     def get_new_files(self):
         """
@@ -99,15 +99,15 @@
         # only files count
         if not filepath.is_file():
             return False
         # must be relative to the upload directory
         if not filepath.is_relative_to(self.__rootdir):
             return False
         # must be outside the logs subdirectory
-        if self.__logs_subdir in filepath.parents:
+        if self._logs_subdir in filepath.parents:
             return False
         # name shouldn't start with '.'
         if filepath.name.startswith("."):
             return False
         # must match the given regex
         if self.__upload_regex.match(str(filepath.relative_to(self.__rootdir))):
             return True
```

### Comparing `openmsistream-1.4.0/openmsistream/data_file_io/utilities.py` & `openmsistream-1.5.0/openmsistream/data_file_io/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/__init__.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_file_parser.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/prod.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/prod.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_and_producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/consumer_group.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/consumer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_processor.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,41 +16,44 @@
     """
 
     CONSUMER_POLL_TIMEOUT = 0.050
     NO_MESSAGE_WAIT = (
         0.005  # how long to wait if consumer.get_next_message_value returns None
     )
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, filepath_regex=None, **kwargs):
         """
         Hang onto the number of messages read and processed
         """
         self.n_msgs_read = 0
         self.n_msgs_processed = 0
         super().__init__(*args, **kwargs)
         # set below to true to reset new consumers to their earliest offsets
         self.restart_at_beginning = False
         # set below to some regex to filter messages by their keys
         self.message_key_regex = None
-        # reset the regex after the consumer has filtered through previous messages
-        self.filter_new_messages = False
+        # reset the key regex after the consumer has filtered through previous messages
+        self.filter_new_message_keys = False
+        # set below to some regex to filter messages by filepath
+        self.filepath_regex = filepath_regex
         # hold onto the last consumed message to manually commit its offset on shutdown
         self.last_message = None
 
     def _run_worker(self):
         """
         Handle startup and shutdown of a thread-independent Consumer and
         serve individual messages to the _process_message function
         """
         # create the Consumer for this thread
         if self.alive:
             consumer = self.get_new_subscribed_consumer(
                 restart_at_beginning=self.restart_at_beginning,
                 message_key_regex=self.message_key_regex,
-                filter_new_messages=self.filter_new_messages,
+                filter_new_message_keys=self.filter_new_message_keys,
+                filepath_regex=self.filepath_regex,
             )
         if ("enable.auto.commit" not in consumer.configs.keys()) or (
             consumer.configs["enable.auto.commit"] is True
         ):
             warnmsg = (
                 "WARNING: enable.auto.commit has not been set to False for a Consumer "
                 "that will manually commit offsets. Missed or duplicate messages could result. "
```

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/controlled_message_reproducer.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     def __init__(
         self,
         config_path,
         consumer_topic_name,
         producer_topic_name,
         *,
+        filepath_regex=None,
         n_producer_threads=1,
         n_consumer_threads=RUN_CONST.DEFAULT_N_THREADS,
         **kwargs,
     ):
         """
         Hang onto the number of messages read, processed, and produced
         """
@@ -49,16 +50,18 @@
             n_threads=max(n_producer_threads, n_consumer_threads),
             **kwargs,
         )
         # set to true to reset new consumers to their earliest offsets
         self.restart_at_beginning = False
         # set to some regex to filter messages by their keys
         self.message_key_regex = None
-        # reset the regex after the consumer has filtered through previous messages
-        self.filter_new_messages = False
+        # reset the key regex after the consumer has filtered through previous messages
+        self.filter_new_message_keys = False
+        # set below to some regex to filter messages by filepath
+        self.filepath_regex = filepath_regex
         # hold onto the last consumed message to commit its offset on shutdown
         self.last_message = None
         self.producer_topic_name = producer_topic_name
         self.n_producer_threads = n_producer_threads
         self.n_consumer_threads = n_consumer_threads
         self.producer_message_queue = Queue()
 
@@ -128,15 +131,16 @@
         """
         Return the consumer and producer to use for a specific thread
         """
         if create_consumer:
             consumer = self.get_new_subscribed_consumer(
                 restart_at_beginning=self.restart_at_beginning,
                 message_key_regex=self.message_key_regex,
-                filter_new_messages=self.filter_new_messages,
+                filter_new_message_keys=self.filter_new_message_keys,
+                filepath_regex=self.filepath_regex,
             )
         else:
             consumer = None
         if create_producer:
             producer = self.get_new_producer()
         else:
             producer = None
```

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_consumer.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     warnings.simplefilter("ignore")
     from kafkacrypto import KafkaConsumer
 from ..utilities import LogOwner
 from ..utilities.misc import (
     raise_err_with_optional_logger,
     debug_msg_with_optional_logger,
 )
+from ..data_file_io.entity.data_file_chunk import DataFileChunk
 from .utilities import add_kwargs_to_configs, KCCommitOffsetDictKey, KCCommitOffset
 from .config_file_parser import KafkaConfigFileParser
 from .openmsistream_kafka_crypto import OpenMSIStreamKafkaCrypto
 from .serialization import CompoundDeserializer
 
 
 class OpenMSIStreamConsumer(LogOwner):
@@ -35,28 +36,34 @@
         that should be used to instantiate the Consumer. Only needed if `consumer_type` is
         :class:`kafkacrypto.KafkaConsumer`.
     :type kafkacrypto: :class:`~.kafka_wrapper.OpenMSIStreamKafkaCrypto`, optional
     :param message_key_regex: A regular expression to filter messages based on their keys.
         Only messages matching this regex will be returned by :func:`~get_next_message`.
         This parameter only has an effect if `restart_at_beginning` is true and a consumer group
         with the given ID has previously consumed messages from the topic, or if
-        `filter_new_messages` is True. Messages with keys that are not strings will always
+        `filter_new_message_keys` is True. Messages with keys that are not strings will always
         be consumed, logging warnings if they should be filtered.
     :type message_key_regex: :func:`re.compile` or None, optional
-    :param filter_new_messages: If False (the default) the `message_key_regex` will only be used
+    :param filter_new_message_keys: If False (the default) the `message_key_regex` will only be used
         to filter messages from before each partition's currently committed location.
         Useful if you want to process only some messages from earlier in the topic, but all new
         messages that have never been read. To filter every message read instead of just
         previously-consumed messages, set this to True.
-    :type filter_new_messages: bool, optional
+    :type filter_new_message_keys: bool, optional
     :param starting_offsets: A list of :class:`confluent_kafka.TopicPartition` objects listing
         the initial starting offsets for each partition in the topic for Consumers with this
-        group ID. If `filter_new_messages` is False, messages with offsets greater than or
+        group ID. If `filter_new_message_keys` is False, messages with offsets greater than or
         equal to these will NOT be filtered using `message_key_regex`.
     :type starting_offsets: list(:class:`confluent_kafka.TopicPartition`) or None, optional
+    :param filepath_regex: A regular expression to filter messages based on the path to the
+        file with which they're associated (relative to the "root" upload directory).
+        Only messages matching this regex will be returned by :func:`~get_next_message`.
+        Messages that cannot be deserialized to :class:`~DataFileChunk` objects will
+        always be consumed, logging warnings if they should be filtered.
+    :type filepath_regex: :func:`re.compile` or None, optional
     :param kwargs: Any extra keyword arguments are added to the configuration dict for the Consumer,
         with underscores in their names replaced by dots
     :type kwargs: dict
 
     :raises ValueError: if `consumer_type` is not :class:`confluent_kafka.DeserializingConsumer`
         or :class:`kafkacrypto.KafkaConsumer`
     :raises ValueError: if `consumer_type` is :class:`kafkacrypto.KafkaConsumer` and
@@ -65,16 +72,17 @@
 
     def __init__(
         self,
         consumer_type,
         configs,
         kafkacrypto=None,
         message_key_regex=None,
-        filter_new_messages=False,
+        filter_new_message_keys=False,
         starting_offsets=None,
+        filepath_regex=None,
         **kwargs,
     ):
         """
         Constructor method
         """
         super().__init__(**kwargs)
         if consumer_type == KafkaConsumer:
@@ -87,15 +95,16 @@
         elif consumer_type == DeserializingConsumer:
             self._consumer = consumer_type(configs)
         else:
             errmsg = f"ERROR: Unrecognized consumer type {consumer_type} for OpenMSIStreamConsumer!"
             self.logger.error(errmsg, exc_type=ValueError)
         self.configs = configs
         self.message_key_regex = message_key_regex
-        self.filter_new_messages = filter_new_messages
+        self.filter_new_message_keys = filter_new_message_keys
+        self.filepath_regex = filepath_regex
         self.__starting_offsets = starting_offsets
 
     @staticmethod
     def get_consumer_args_kwargs(
         config_file_path, logger=None, kafkacrypto=None, **kwargs
     ):
         """
@@ -307,36 +316,72 @@
         except Exception:
             pass
         finally:
             self.__kafkacrypto = None
 
     def _filter_message(self, msg):
         """
-        Checks a message's key against the regex and its offset against the starting offsets.
-        Returns None if a message should be skipped, otherwise returns the message.
+        Checks a message's key against the key regex, its filepath against the filepath regex,
+        and its offset against the starting offsets. Returns None if a message should be skipped,
+        otherwise returns the message.
         """
-        if (self.message_key_regex is not None) and (
-            self.filter_new_messages or self.message_consumed_before(msg)
+        if self._message_passes_key_filter(msg) and self._message_passes_filepath_filter(
+            msg
         ):
-            try:
-                msg_key = msg.key()  # from a regular Kafka Consumer
-            except TypeError:
-                msg_key = msg.key  # from KafkaCrypto
-            if not isinstance(msg_key, str):
-                warnmsg = (
-                    f"WARNING: found a message whose key ({msg_key}) is not a string, "
-                    "but which should be filtered using the key regex. "
-                    "This message will be consumed as though it successfully passed the filter."
-                )
-                self.logger.warning(warnmsg)
-                return msg
-            if self.message_key_regex.match(msg_key):
-                return msg
-            return None
-        return msg
+            return msg
+        return None
+
+    def _message_passes_key_filter(self, msg):
+        """
+        Returns True if a message should be consumed based on the key regex and False
+        if it should be skipped instead
+        """
+        if (self.message_key_regex is None) or not (
+            self.filter_new_message_keys or self.message_consumed_before(msg)
+        ):
+            return True
+        try:
+            msg_key = msg.key()  # from a regular Kafka Consumer
+        except TypeError:
+            msg_key = msg.key  # from KafkaCrypto
+        if not isinstance(msg_key, str):
+            warnmsg = (
+                f"WARNING: found a message whose key ({msg_key}) is not a string, "
+                "but which should be filtered using the key regex. "
+                "This message will be consumed as though it successfully passed the filter."
+            )
+            self.logger.warning(warnmsg)
+            return True
+        if self.message_key_regex.match(msg_key):
+            return True
+        return False
+
+    def _message_passes_filepath_filter(self, msg):
+        """
+        Returns True if a message should be consumed based on the filepath regex and False
+        if it should be skipped instead
+        """
+        if self.filepath_regex is None:
+            return True
+        try:
+            msg_value = msg.value()  # from a regular Kafka Consumer
+        except TypeError:
+            msg_value = msg.value  # from KafkaCrypto
+        if not isinstance(msg_value, DataFileChunk):
+            warnmsg = (
+                f"WARNING: found a message whose value ({msg_value}) is not a DataFileChunk, "
+                "but which should be filtered using the filepath regex. "
+                "This message will be consumed as though it successfully passed the filter."
+            )
+            self.logger.warning(warnmsg)
+            return True
+        rel_filepath = msg_value.relative_filepath
+        if self.filepath_regex.match(str(rel_filepath)):
+            return True
+        return False
 
     @methodtools.lru_cache()
     def message_consumed_before(self, msg):
         """
         Returns True if a message has an offset less than the starting offset
         for the topic/partition, False otherwise
         """
```

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/openmsistream_producer.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/openmsistream_producer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/producer_group.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/producible.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/producible.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/serialization.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/serialization.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/kafka_wrapper/utilities.py` & `openmsistream-1.5.0/openmsistream/kafka_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_message.py` & `openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/metadata_extraction/metadata_json_reproducer.py` & `openmsistream-1.5.0/openmsistream/metadata_extraction/metadata_json_reproducer.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,17 @@
         producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_producer_threads: int, optional
     :param n_consumer_threads: the number of consumers to run. The total number of
         producer/consumer threads started is `max(n_consumer_threads,n_producer_threads)`.
     :type n_consumer_threads: int, optional
     :param consumer_group_id: the group ID under which each consumer should be created
     :type consumer_group_id: str, optional
+    :param filepath_regex: If given, only messages associated with files whose paths match
+        this regex will be consumed
+    :type filepath_regex: :type filepath_regex: :func:`re.compile` or None, optional
 
     :raises ValueError: if `datafile_type` is not a subclass of
         :class:`~.data_file_io.DownloadDataFileToMemory`
     """
 
     def __init__(self, config_file, consumer_topic_name, producer_topic_name, **kwargs):
         """
@@ -107,14 +110,16 @@
             args.config,
             args.consumer_topic_name,
             args.producer_topic_name,
             consumer_group_id=args.consumer_group_id,
             n_consumer_threads=args.n_consumer_threads,
             n_producer_threads=args.n_producer_threads,
             output_dir=args.output_dir,
+            mode=args.mode,
+            filepath_regex=args.download_regex,
             update_secs=args.update_seconds,
             streamlevel=args.logger_stream_level,
             filelevel=args.logger_file_level,
         )
         # cls.bucket_name = args.bucket_name
         msg = (
             f"Listening to the {args.consumer_topic_name} topic for XRD CSV files to "
@@ -122,15 +127,15 @@
         )
         metadata_reproducer.logger.info(msg)
         (
             n_m_r,
             n_m_p,
             n_f_r,
             n_f_mp,
-            m_p_fns,
+            m_p_fps,
         ) = metadata_reproducer.produce_processing_results_for_files_as_read()
         metadata_reproducer.close()
         msg = ""
         if n_m_r > 0:
             msg += f'{n_m_r} total message{"s were" if n_m_r!=1 else " was"} consumed, '
         if n_m_p > 0:
             msg += f'{n_m_p} message{"s were" if n_m_p!=1 else " was"} successfully processed, '
@@ -144,9 +149,9 @@
         metadata_reproducer.logger.info(msg[:-2])
         if n_f_mp > 0:
             msg = (
                 f'{n_f_mp} file{"" if n_f_mp==1 else "s"} had json metadata produced '
                 f"to the {args.producer_topic_name} topic. "
                 f"Up to {cls.N_RECENT_FILES} most recent:\n\t"
             )
-            msg += "\n\t".join(m_p_fns)
+            msg += "\n\t".join([str(fp) for fp in m_p_fps])
             metadata_reproducer.logger.debug(msg)
```

### Comparing `openmsistream-1.4.0/openmsistream/s3_buckets/config_file_parser.py` & `openmsistream-1.5.0/openmsistream/s3_buckets/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/s3_buckets/s3_data_transfer.py` & `openmsistream-1.5.0/openmsistream/s3_buckets/s3_data_transfer.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,18 +12,24 @@
     def __init__(self, s3_config, *args, **kwargs):
         super().__init__(s3_config, *args, **kwargs)
 
     def transfer_object_stream(self, object_key, datafile):
         """
         Transfer the contents of a DataFile Consumed from chunks in a topic to an S3 bucket
         """
+        content = None
+        try:
+            content = datafile.bytestring
+        except AttributeError:
+            with open(datafile.full_filepath, "rb") as fp:
+                content = fp.read()
         file_name = str(datafile.filename)
         try:
             self.s3_client.put_object(
-                Body=datafile.bytestring,
+                Body=content,
                 Bucket=self.bucket_name,
                 Key=object_key,
                 # GrantRead=self.grant_read
             )
             msg = f"{file_name} successfully transferred into {self.bucket_name}/{object_key}"
             self.logger.debug(msg)
         except ClientError as err:
```

### Comparing `openmsistream-1.4.0/openmsistream/s3_buckets/s3_service.py` & `openmsistream-1.5.0/openmsistream/s3_buckets/s3_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py` & `openmsistream-1.5.0/openmsistream/s3_buckets/s3_transfer_stream_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     :param bucket_name: Name of the S3 bucket into which reconstructed files should be transferred
     :type bucket_name: str
     :param config_path: Path to the config file to use in defining the Broker connection
         and Consumers
     :type config_path: :class:`pathlib.Path`
     :param topic_name: Name of the topic to which the Consumers should be subscribed
     :type topic_name: str
+    :param filepath_regex: If given, only messages associated with files whose paths match
+        this regex will be consumed
+    :type filepath_regex: :type filepath_regex: :func:`re.compile` or None, optional
     """
 
     def __init__(self, bucket_name, config_path, topic_name, **kwargs):
         super().__init__(config_path, topic_name, **kwargs)
         parser = S3ConfigFileParser(config_path, logger=self.logger)
         self.__s3_config = parser.s3_configs
         self.__s3_config["bucket_name"] = bucket_name
@@ -111,15 +114,17 @@
         parser = cls.get_argument_parser()
         args = parser.parse_args(args=args)
         s3_stream_proc = cls(
             args.bucket_name,
             args.config,
             args.topic_name,
             output_dir=args.output_dir,
+            mode=args.mode,
             n_threads=args.n_threads,
+            filepath_regex=args.download_regex,
             update_secs=args.update_seconds,
             consumer_group_id=args.consumer_group_id,
             streamlevel=args.logger_stream_level,
             filelevel=args.logger_file_level,
         )
         # cls.bucket_name = args.bucket_name
         msg = (
```

### Comparing `openmsistream-1.4.0/openmsistream/services/config.py` & `openmsistream-1.5.0/openmsistream/services/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/services/examples/runnable_example.py` & `openmsistream-1.5.0/openmsistream/services/examples/runnable_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/services/examples/script_example.py` & `openmsistream-1.5.0/openmsistream/services/examples/script_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/services/install_service.py` & `openmsistream-1.5.0/openmsistream/services/install_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/services/linux_service_manager.py` & `openmsistream-1.5.0/openmsistream/services/linux_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/services/manage_service.py` & `openmsistream-1.5.0/openmsistream/services/manage_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/services/service_manager_base.py` & `openmsistream-1.5.0/openmsistream/services/service_manager_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,32 +303,32 @@
         write out the executable python file that the service will actually be running
         """
         error_log_path = (
             pathlib.Path().resolve()
             / f"{self.service_name}{SERVICE_CONST.ERROR_LOG_STEM}"
         )
         code = """\
-            if __name__=='__main__' :
-                try :"""
+            if __name__ == "__main__":
+                try:"""
         if self.service_dict["func_name"] is not None:
             code += f"""
                     from {self.service_dict['filepath']} import {self.service_dict['func_name']}
                     {self.service_dict['func_name']}({self.argslist})"""
         else:
             code += f"""
                     from {self.service_dict['filepath']} import {self.service_dict['class_name']}
                     {self.service_dict['class_name']}.run_from_command_line({self.argslist})"""
         code += f"""
-                except Exception :
+                except Exception:
                     import pathlib, traceback, datetime
                     output_filepath = pathlib.Path(r"{error_log_path}")
-                    with open(output_filepath,'a') as fp :"""
+                    with open(output_filepath, "a") as fp:"""
         code += r"""
                         timestamp = (datetime.datetime.now()).strftime("%Y-%m-%d at %H:%M:%S")
-                        fp.write(f'Error on {timestamp}. Exception:\n{traceback.format_exc()}')
+                        fp.write(f"Error on {timestamp}. Exception:\n{traceback.format_exc()}")
                     import sys
                     sys.exit(1)
         """
         if filepath is not None:
             warnmsg = (
                 f"WARNING: Services executable will be written to {filepath} "
                 f"instead of {self.exec_fp}"
```

### Comparing `openmsistream-1.4.0/openmsistream/services/utilities.py` & `openmsistream-1.5.0/openmsistream/services/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/services/windows_service_manager.py` & `openmsistream-1.5.0/openmsistream/services/windows_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/__init__.py` & `openmsistream-1.5.0/openmsistream/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/argument_parsing.py` & `openmsistream-1.5.0/openmsistream/utilities/argument_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 def detect_bucket_name(argstring):
     """
     detects if the bucket name contains invalid characters
     """
     if argstring is None:  # Then the argument wasn't given and nothing should be done
         return None
-    illegal_charcters = [
+    illegal_characters = [
         "#",
         "%",
         "&",
         "{",
         "}",
         "\\",
         "/",
@@ -89,16 +89,17 @@
         ":",
         "@",
         "+",
         "`",
         "|",
         "=",
     ]
-    if argstring in illegal_charcters:
-        raise RuntimeError(f"ERROR: Illegal characters in bucket_name {argstring}")
+    for illegal_character in illegal_characters:
+        if illegal_character in argstring:
+            raise RuntimeError(f"ERROR: Illegal characters in bucket_name {argstring}")
     return argstring
 
 
 def int_power_of_two(argval):
     """
     make sure a given value is a nonzero integer power of two (or can be converted to one)
     """
@@ -245,15 +246,22 @@
             },
         ],
         "upload_regex": [
             "optional",
             {
                 "default": RUN_OPT_CONST.DEFAULT_UPLOAD_REGEX,
                 "type": re.compile,
-                "help": "Only files matching this regular expression will be uploaded",
+                "help": "Only files with paths matching this regular expression will be uploaded",
+            },
+        ],
+        "download_regex": [
+            "optional",
+            {
+                "type": re.compile,
+                "help": "Only files with paths matching this regular expression will be uploaded",
             },
         ],
         "chunk_size": [
             "optional",
             {
                 "default": RUN_OPT_CONST.DEFAULT_CHUNK_SIZE,
                 "type": int_power_of_two,
@@ -281,14 +289,27 @@
                 "type": int,
                 "help": (
                     'Number of seconds between printing a "." to the console '
                     "to indicate the program is alive"
                 ),
             },
         ],
+        "mode": [
+            "optional",
+            {
+                "choices": ["memory", "disk", "both"],
+                "default": "memory",
+                "help": (
+                    "Choose whether files should be reconstructed in 'memory', "
+                    "on 'disk' (with the output directory as the root directory) "
+                    "or 'both' (giving access to the data bytestring, "
+                    "but also writing to disk)"
+                ),
+            },
+        ],
         "upload_existing": [
             "optional",
             {
                 "action": "store_true",
                 "help": (
                     "Add this flag to upload files already existing in addition to those "
                     "added to the directory after this code starts running (by default "
```

### Comparing `openmsistream-1.4.0/openmsistream/utilities/config.py` & `openmsistream-1.5.0/openmsistream/utilities/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/config_file_parser.py` & `openmsistream-1.5.0/openmsistream/utilities/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/controlled_process.py` & `openmsistream-1.5.0/openmsistream/utilities/controlled_process.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/controlled_process_multi_threaded.py` & `openmsistream-1.5.0/openmsistream/utilities/controlled_process_multi_threaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     """
     A class for running a group of processes in multiple threads until they're explicitly shut down.
 
     :param n_threads: the number of threads to use in the group of processes
     :type n_threads: int, optional
     """
 
+    # time in seconds to wait for threads to join in shutdown
+    SHUTDOWN_THREAD_TIMEOUT = 10
+
     def __init__(self, *args, n_threads=RUN_CONST.DEFAULT_N_THREADS, **kwargs):
         self.n_threads = n_threads
         super().__init__(*args, **kwargs)
         self.lock = Lock()
         self.__args_per_thread = []
         self.__kwargs_per_thread = {}
         self.__threads = []
@@ -88,15 +91,15 @@
 
     def _on_shutdown(self):
         """
         Join all of the running threads. Can override this method further in subclasses,
         just be sure to also call :func:`super()._on_shutdown()`.
         """
         for thread in self.__threads:
-            thread.join()
+            thread.join(self.SHUTDOWN_THREAD_TIMEOUT)
 
     @abstractmethod
     def _run_worker(self):
         """
         The function that will actually be run in multiple threads while the process is alive.
         Should include a "while self.alive" loop to keep it running.
```

### Comparing `openmsistream-1.4.0/openmsistream/utilities/controlled_process_single_thread.py` & `openmsistream-1.5.0/openmsistream/utilities/controlled_process_single_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/dataclass_table.py` & `openmsistream-1.5.0/openmsistream/utilities/dataclass_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         return self._entry_objs.values()
 
     @property
     def lines(self):
         """
         A list of all the text lines in the file
         """
-        return self._entry_lines.values()
+        return [line.strip() for line in self._entry_lines.values()]
 
 
 class DataclassTableAppendOnly(DataclassTableBase):
     """
     A class to work with an atomic csv file that's holding dataclass entries. Only includes
     methods to add lines to the file like a log and not to edit the objects themselves,
     which can be much more efficient.
```

### Comparing `openmsistream-1.4.0/openmsistream/utilities/exception_tracking_thread.py` & `openmsistream-1.5.0/openmsistream/utilities/exception_tracking_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/has_arguments.py` & `openmsistream-1.5.0/openmsistream/utilities/has_arguments.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/logging.py` & `openmsistream-1.5.0/openmsistream/utilities/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,22 @@
         Set the level of the underlying logger's streamhandler
 
         :param level: The level to set
         :type level: logging level int
         """
         self._streamhandler.setLevel(level)
 
+    def get_stream_level(self):
+        """
+        Get the current level of the underlying logger's streamhandler
+
+        :return: The integer level of the current streamhandler
+        """
+        return self._streamhandler.level
+
     def set_file_level(self, level):
         """
         Set the level of the underlying logger's filehandler
 
         :param level: The level to set
         :type level: logging level int
         """
```

### Comparing `openmsistream-1.4.0/openmsistream/utilities/misc.py` & `openmsistream-1.5.0/openmsistream/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/provision_wrapper.py` & `openmsistream-1.5.0/openmsistream/utilities/provision_wrapper.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream/utilities/runnable.py` & `openmsistream-1.5.0/openmsistream/utilities/runnable.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream.egg-info/PKG-INFO` & `openmsistream-1.5.0/openmsistream.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.4.0.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.0.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.4.0/openmsistream.egg-info/SOURCES.txt` & `openmsistream-1.5.0/openmsistream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/openmsistream.egg-info/entry_points.txt` & `openmsistream-1.5.0/openmsistream.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `openmsistream-1.4.0/setup.py` & `openmsistream-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # imports
 import setuptools
 
 # version tag
-version = "1.4.0"
+version = "1.5.0"
 
 long_description = ""
 with open("README.md", "r") as readme:
     for il, line in enumerate(readme.readlines(), start=1):
         if il >= 18:
             long_description += line
```

