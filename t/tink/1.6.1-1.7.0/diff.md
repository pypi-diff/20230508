# Comparing `tmp/tink-1.6.1.tar.gz` & `tmp/tink-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, from Unix
+gzip compressed data, was "tink-1.7.0.tar", last modified: Fri Aug 26 08:30:17 2022, max compression
```

## Comparing `tink-1.6.1.tar` & `tink-1.7.0.tar`

### file list

```diff
@@ -1,343 +1,345 @@
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/integration/
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/integration/gcpkms/
--rw-r-----   0 root         (0) root         (0)     3615 2021-08-10 08:41:24.000000 tink-1.6.1/tink/integration/gcpkms/_gcp_kms_aead_test.py
--rw-r-----   0 root         (0) root         (0)     2823 2020-10-15 19:17:20.000000 tink-1.6.1/tink/integration/gcpkms/_gcp_kms_client.py
--rw-r-----   0 root         (0) root         (0)     1986 2021-08-10 08:41:24.000000 tink-1.6.1/tink/integration/gcpkms/_gcp_kms_client_test.py
--rw-r-----   0 root         (0) root         (0)     1149 2020-10-15 19:17:20.000000 tink-1.6.1/tink/integration/gcpkms/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)      807 2020-10-15 19:17:20.000000 tink-1.6.1/tink/integration/gcpkms/__init__.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/integration/awskms/
--rw-r-----   0 root         (0) root         (0)     3052 2020-10-15 19:17:20.000000 tink-1.6.1/tink/integration/awskms/_aws_kms_client.py
--rw-r-----   0 root         (0) root         (0)     3116 2021-08-10 08:41:24.000000 tink-1.6.1/tink/integration/awskms/_aws_kms_aead_test.py
--rw-r-----   0 root         (0) root         (0)     1119 2020-10-15 19:17:20.000000 tink-1.6.1/tink/integration/awskms/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)      858 2021-08-10 08:41:24.000000 tink-1.6.1/tink/integration/awskms/__init__.py
--rw-r-----   0 root         (0) root         (0)     2187 2021-08-10 08:41:24.000000 tink-1.6.1/tink/integration/awskms/_aws_kms_client_test.py
--rw-r-----   0 root         (0) root         (0)      575 2021-08-10 08:41:24.000000 tink-1.6.1/tink/integration/__init__.py
--rw-r-----   0 root         (0) root         (0)    11612 2021-08-10 08:47:45.000000 tink-1.6.1/tink/_keyset_handle.py
--rw-r-----   0 root         (0) root         (0)     2124 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cleartext_keyset_handle_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/aead/
--rw-r-----   0 root         (0) root         (0)     2103 2020-10-15 19:17:20.000000 tink-1.6.1/tink/aead/_aead_key_manager.py
--rw-r-----   0 root         (0) root         (0)     2844 2020-10-15 19:17:20.000000 tink-1.6.1/tink/aead/_aead_wrapper.py
--rw-r-----   0 root         (0) root         (0)     6903 2021-08-10 08:41:24.000000 tink-1.6.1/tink/aead/_aead_key_templates.py
--rw-r-----   0 root         (0) root         (0)     6789 2021-08-10 08:41:24.000000 tink-1.6.1/tink/aead/_aead_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     5921 2021-08-10 08:41:24.000000 tink-1.6.1/tink/aead/_aead_key_templates_test.py
--rw-r-----   0 root         (0) root         (0)     3457 2020-10-15 19:17:20.000000 tink-1.6.1/tink/aead/_kms_envelope_aead.py
--rw-r-----   0 root         (0) root         (0)     3411 2021-08-10 08:41:24.000000 tink-1.6.1/tink/aead/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1093 2020-10-15 19:17:20.000000 tink-1.6.1/tink/aead/__init__.py
--rw-r-----   0 root         (0) root         (0)     2337 2020-10-15 19:17:20.000000 tink-1.6.1/tink/aead/_aead.py
--rw-r-----   0 root         (0) root         (0)     4958 2021-08-10 08:41:24.000000 tink-1.6.1/tink/aead/_kms_envelope_aead_test.py
--rw-r-----   0 root         (0) root         (0)     5150 2020-10-15 19:17:20.000000 tink-1.6.1/tink/aead/_aead_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)    13045 2021-08-10 08:47:45.000000 tink-1.6.1/tink/_keyset_handle_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/cc/
--rw-r-----   0 root         (0) root         (0)      902 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/cc_tink_config.cc
--rw-r-----   0 root         (0) root         (0)     1506 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/input_stream_adapter.h
--rw-r-----   0 root         (0) root         (0)     3305 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/python_input_stream.cc
--rw-r-----   0 root         (0) root         (0)     1773 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/output_stream_adapter.h
--rw-r-----   0 root         (0) root         (0)     3428 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/output_stream_adapter_test.cc
--rw-r-----   0 root         (0) root         (0)     1709 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/cc_streaming_aead_wrappers_test.cc
--rw-r-----   0 root         (0) root         (0)     6532 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/python_input_stream_test.cc
--rw-r-----   0 root         (0) root         (0)     2192 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/python_input_stream.h
--rw-r-----   0 root         (0) root         (0)    11260 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/test_util.h
--rw-r-----   0 root         (0) root         (0)     2223 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/python_output_stream.h
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/cc/pybind/
--rw-r-----   0 root         (0) root         (0)      994 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/cc_tink_config.cc
--rw-r-----   0 root         (0) root         (0)      966 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/cc_tink_config_test.py
--rw-r-----   0 root         (0) root         (0)     1026 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/input_stream_adapter.h
--rw-r-----   0 root         (0) root         (0)     2537 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_gcp_kms_client.cc
--rw-r-----   0 root         (0) root         (0)     1009 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/status_injector.h
--rw-r-----   0 root         (0) root         (0)     2153 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/mac.cc
--rw-r-----   0 root         (0) root         (0)     1141 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/import_helper.cc
--rw-r-----   0 root         (0) root         (0)     1447 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_fake_kms_client_testonly.cc
--rw-r-----   0 root         (0) root         (0)     1107 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_aws_kms_client.h
--rw-r-----   0 root         (0) root         (0)     2680 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/tink_bindings.cc
--rw-r-----   0 root         (0) root         (0)     1527 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/hybrid_decrypt.cc
--rw-r-----   0 root         (0) root         (0)      998 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/output_stream_adapter.h
--rw-r-----   0 root         (0) root         (0)     1063 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_fake_kms_client_testonly.h
--rw-r-----   0 root         (0) root         (0)     1961 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/public_key_sign.cc
--rw-r-----   0 root         (0) root         (0)     5680 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/python_file_object_adapter.cc
--rw-r-----   0 root         (0) root         (0)     1839 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/streaming_aead.cc
--rw-r-----   0 root         (0) root         (0)     1003 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/hybrid_encrypt.h
--rw-r-----   0 root         (0) root         (0)     2823 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/aead.cc
--rw-r-----   0 root         (0) root         (0)      958 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/status.h
--rw-r-----   0 root         (0) root         (0)     1008 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/streaming_aead.h
--rw-r-----   0 root         (0) root         (0)     1400 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/output_stream_adapter.cc
--rw-r-----   0 root         (0) root         (0)     4053 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/status.cc
--rw-r-----   0 root         (0) root         (0)      995 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_jwt_config.cc
--rw-r-----   0 root         (0) root         (0)     9047 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1049 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/python_file_object_adapter.h
--rw-r-----   0 root         (0) root         (0)      965 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/prf.h
--rw-r-----   0 root         (0) root         (0)     2269 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/cc_streaming_aead_wrappers.cc
--rw-r-----   0 root         (0) root         (0)     2512 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_aws_kms_client.cc
--rw-r-----   0 root         (0) root         (0)     1523 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/hybrid_encrypt.cc
--rw-r-----   0 root         (0) root         (0)    20616 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     3745 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_key_manager.cc
--rw-r-----   0 root         (0) root         (0)      969 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/aead.h
--rw-r-----   0 root         (0) root         (0)     1048 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_streaming_aead_wrappers.h
--rw-r-----   0 root         (0) root         (0)     3136 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/deterministic_aead.cc
--rw-r-----   0 root         (0) root         (0)     1013 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/public_key_verify.h
--rw-r-----   0 root         (0) root         (0)     1107 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_gcp_kms_client.h
--rw-r-----   0 root         (0) root         (0)     1304 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/input_stream_adapter.cc
--rw-r-----   0 root         (0) root         (0)     1001 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_tink_config.h
--rw-r-----   0 root         (0) root         (0)      997 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_jwt_config.h
--rw-r-----   0 root         (0) root         (0)     1350 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/status_utils.cc
--rw-r-----   0 root         (0) root         (0)     1615 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/prf.cc
--rw-r-----   0 root         (0) root         (0)     1019 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/deterministic_aead.h
--rw-r-----   0 root         (0) root         (0)     1002 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/cc_key_manager.h
--rw-r-----   0 root         (0) root         (0)      960 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/mac.h
--rw-r-----   0 root         (0) root         (0)     2068 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/public_key_verify.cc
--rw-r-----   0 root         (0) root         (0)      974 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/public_key_sign.h
--rw-r-----   0 root         (0) root         (0)     1205 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/import_helper.h
--rw-r-----   0 root         (0) root         (0)     6938 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/status_test.py
--rw-r-----   0 root         (0) root         (0)     6239 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/status_injector.cc
--rw-r-----   0 root         (0) root         (0)     1003 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/pybind/hybrid_decrypt.h
--rw-r-----   0 root         (0) root         (0)     5857 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/status_casters.h
--rw-r-----   0 root         (0) root         (0)     3643 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/pybind/status_utils.h
--rw-r-----   0 root         (0) root         (0)     1566 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/output_stream_adapter.cc
--rw-r-----   0 root         (0) root         (0)     7370 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/python_output_stream_test.cc
--rw-r-----   0 root         (0) root         (0)     2108 2021-08-10 08:45:24.000000 tink-1.6.1/tink/cc/cc_jwt_config.cc
--rw-r-----   0 root         (0) root         (0)     5738 2021-08-10 08:45:24.000000 tink-1.6.1/tink/cc/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1748 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/python_file_object_adapter.h
--rw-r-----   0 root         (0) root         (0)     2337 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/cc_streaming_aead_wrappers.cc
--rw-r-----   0 root         (0) root         (0)     4143 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/input_stream_adapter_test.cc
--rw-r-----   0 root         (0) root         (0)     2478 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/cc_streaming_aead_wrappers.h
--rw-r-----   0 root         (0) root         (0)     1451 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/input_stream_adapter.cc
--rw-r-----   0 root         (0) root         (0)      991 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/cc_tink_config.h
--rw-r-----   0 root         (0) root         (0)      987 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/cc_jwt_config.h
--rw-r-----   0 root         (0) root         (0)     4122 2021-08-10 08:41:24.000000 tink-1.6.1/tink/cc/python_output_stream.cc
--rw-r-----   0 root         (0) root         (0)     4383 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cc/cc_key_manager.h
--rw-r-----   0 root         (0) root         (0)     4989 2020-10-15 19:17:20.000000 tink-1.6.1/tink/_keyset_reader_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/daead/
--rw-r-----   0 root         (0) root         (0)     2666 2021-08-10 08:41:24.000000 tink-1.6.1/tink/daead/_deterministic_aead_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     1658 2020-10-15 19:17:20.000000 tink-1.6.1/tink/daead/_deterministic_aead_key_templates.py
--rw-r-----   0 root         (0) root         (0)     1957 2021-08-10 08:41:24.000000 tink-1.6.1/tink/daead/_deterministic_aead_key_templates_test.py
--rw-r-----   0 root         (0) root         (0)     3557 2020-10-15 19:17:20.000000 tink-1.6.1/tink/daead/_deterministic_aead_wrapper.py
--rw-r-----   0 root         (0) root         (0)     2270 2020-10-15 19:17:20.000000 tink-1.6.1/tink/daead/_deterministic_aead_key_manager.py
--rw-r-----   0 root         (0) root         (0)     6074 2020-10-15 19:17:20.000000 tink-1.6.1/tink/daead/_deterministic_aead_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)     2471 2021-08-10 08:41:24.000000 tink-1.6.1/tink/daead/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1070 2020-10-15 19:17:20.000000 tink-1.6.1/tink/daead/__init__.py
--rw-r-----   0 root         (0) root         (0)     2160 2020-10-15 19:17:20.000000 tink-1.6.1/tink/daead/_deterministic_aead.py
--rw-r-----   0 root         (0) root         (0)     1076 2021-08-10 08:41:24.000000 tink-1.6.1/tink/tink_config.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/testing/
--rw-r-----   0 root         (0) root         (0)     5613 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/bytes_io_test.py
--rw-r-----   0 root         (0) root         (0)     7016 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/keyset_builder_test.py
--rw-r-----   0 root         (0) root         (0)     2197 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/fake_kms_test.py
--rw-r-----   0 root         (0) root         (0)     1072 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/fake_kms.py
--rw-r-----   0 root         (0) root         (0)     2158 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)      575 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/__init__.py
--rw-r-----   0 root         (0) root         (0)     4542 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/keyset_builder.py
--rw-r-----   0 root         (0) root         (0)     5733 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/helper_test.py
--rw-r-----   0 root         (0) root         (0)     7256 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/helper.py
--rw-r-----   0 root         (0) root         (0)     3864 2021-08-10 08:41:24.000000 tink-1.6.1/tink/testing/bytes_io.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/signature/
--rw-r-----   0 root         (0) root         (0)     5421 2021-08-10 08:41:24.000000 tink-1.6.1/tink/signature/_signature_wrapper.py
--rw-r-----   0 root         (0) root         (0)     3043 2020-10-15 19:17:20.000000 tink-1.6.1/tink/signature/_signature_key_manager.py
--rw-r-----   0 root         (0) root         (0)     2859 2021-08-10 08:41:24.000000 tink-1.6.1/tink/signature/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1122 2020-10-15 19:17:20.000000 tink-1.6.1/tink/signature/__init__.py
--rw-r-----   0 root         (0) root         (0)     3192 2021-08-10 08:41:24.000000 tink-1.6.1/tink/signature/_signature_key_templates_test.py
--rw-r-----   0 root         (0) root         (0)     1709 2020-10-15 19:17:20.000000 tink-1.6.1/tink/signature/_public_key_verify.py
--rw-r-----   0 root         (0) root         (0)     1582 2020-10-15 19:17:20.000000 tink-1.6.1/tink/signature/_public_key_sign.py
--rw-r-----   0 root         (0) root         (0)     5995 2020-10-15 19:17:20.000000 tink-1.6.1/tink/signature/_signature_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)     5042 2020-10-15 19:17:20.000000 tink-1.6.1/tink/signature/_signature_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     5949 2020-10-15 19:17:20.000000 tink-1.6.1/tink/signature/_signature_key_templates.py
--rw-r-----   0 root         (0) root         (0)     4688 2020-10-15 19:17:20.000000 tink-1.6.1/tink/_keyset_writer_test.py
--rw-r-----   0 root         (0) root         (0)     3469 2021-08-10 08:41:24.000000 tink-1.6.1/tink/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1522 2021-08-10 08:47:45.000000 tink-1.6.1/tink/__init__.py
--rw-r-----   0 root         (0) root         (0)     1624 2020-10-15 19:17:20.000000 tink-1.6.1/tink/cleartext_keyset_handle.py
--rw-r-----   0 root         (0) root         (0)     3542 2020-10-15 19:17:20.000000 tink-1.6.1/tink/_keyset_writer.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/core/
--rw-r-----   0 root         (0) root         (0)     1651 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/_crypto_format.py
--rw-r-----   0 root         (0) root         (0)    10037 2021-08-10 08:41:24.000000 tink-1.6.1/tink/core/_primitive_set_test.py
--rw-r-----   0 root         (0) root         (0)     1961 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/_primitive_wrapper.py
--rw-r-----   0 root         (0) root         (0)     1405 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/_tink_error.py
--rw-r-----   0 root         (0) root         (0)     3767 2021-08-10 08:41:24.000000 tink-1.6.1/tink/core/_primitive_set.py
--rw-r-----   0 root         (0) root         (0)     2603 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1528 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/__init__.py
--rw-r-----   0 root         (0) root         (0)     9252 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/_registry.py
--rw-r-----   0 root         (0) root         (0)     2840 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/_crypto_format_test.py
--rw-r-----   0 root         (0) root         (0)    14588 2020-10-15 19:17:20.000000 tink-1.6.1/tink/core/_registry_test.py
--rw-r-----   0 root         (0) root         (0)     5445 2021-08-10 08:41:24.000000 tink-1.6.1/tink/core/_key_manager.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/
--rw-r-----   0 root         (0) root         (0)     6256 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/config_pb2.py
--rw-r-----   0 root         (0) root         (0)    11623 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/ecdsa_pb2.py
--rw-r-----   0 root         (0) root         (0)     4478 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_siv_pb2.py
--rw-r-----   0 root         (0) root         (0)     2529 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/ecdsa.proto
--rw-r-----   0 root         (0) root         (0)     1166 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/aes_siv.proto
--rw-r-----   0 root         (0) root         (0)     1596 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_gcm_hkdf_streaming.proto
--rw-r-----   0 root         (0) root         (0)     5215 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/kms_envelope_pb2.py
--rw-r-----   0 root         (0) root         (0)     6573 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/ed25519_pb2.py
--rw-r-----   0 root         (0) root         (0)     1561 2021-08-10 08:47:45.000000 tink-1.6.1/tink/proto/cached_dek_envelope.proto
--rw-r-----   0 root         (0) root         (0)     4363 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/xchacha20_poly1305_pb2.py
--rw-r-----   0 root         (0) root         (0)    15250 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/jwt_rsa_ssa_pss_pb2.py
--rw-r-----   0 root         (0) root         (0)    11673 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/jwt_ecdsa_pb2.py
--rw-r-----   0 root         (0) root         (0)     4592 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_gcm_siv_pb2.py
--rw-r-----   0 root         (0) root         (0)     1737 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/empty_pb2.py
--rw-r-----   0 root         (0) root         (0)     1439 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/jwt_hmac.proto
--rw-r-----   0 root         (0) root         (0)     3089 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/rsa_ssa_pss.proto
--rw-r-----   0 root         (0) root         (0)      897 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/empty.proto
--rw-r-----   0 root         (0) root         (0)     4478 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_gcm_pb2.py
--rw-r-----   0 root         (0) root         (0)     5465 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/cached_dek_envelope_pb2.py
--rw-r-----   0 root         (0) root         (0)     1199 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/chacha20_poly1305.proto
--rw-r-----   0 root         (0) root         (0)     1165 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_ctr.proto
--rw-r-----   0 root         (0) root         (0)     4614 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_cmac_prf_pb2.py
--rw-r-----   0 root         (0) root         (0)     1682 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/jwt_ecdsa.proto
--rw-r-----   0 root         (0) root         (0)     1385 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/kms_aead.proto
--rw-r-----   0 root         (0) root         (0)      932 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/test_proto.proto
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/testing/
--rw-r-----   0 root         (0) root         (0)    11791 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/testing/testing_api.proto
--rw-r-----   0 root         (0) root         (0)     7645 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/hkdf_prf_pb2.py
--rw-r-----   0 root         (0) root         (0)     1974 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/config.proto
--rw-r-----   0 root         (0) root         (0)     1191 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_gcm_siv.proto
--rw-r-----   0 root         (0) root         (0)     1510 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/common.proto
--rw-r-----   0 root         (0) root         (0)     1752 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/ed25519.proto
--rw-r-----   0 root         (0) root         (0)    21854 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/tink_pb2.py
--rw-r-----   0 root         (0) root         (0)     5337 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1252 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/hmac_prf.proto
--rw-r-----   0 root         (0) root         (0)      575 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/__init__.py
--rw-r-----   0 root         (0) root         (0)     6224 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_ctr_hmac_aead_pb2.py
--rw-r-----   0 root         (0) root         (0)     3872 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/chacha20_poly1305_pb2.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/experimental/
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/experimental/pqcrypto/
--rw-r-----   0 root         (0) root         (0)     3688 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/experimental/pqcrypto/cecpq2_aead_hkdf.proto
--rw-r-----   0 root         (0) root         (0)     1341 2021-08-10 08:47:45.000000 tink-1.6.1/tink/proto/experimental/pqcrypto/dilithium.proto
--rw-r-----   0 root         (0) root         (0)     7483 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/hmac_pb2.py
--rw-r-----   0 root         (0) root         (0)    13664 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/rsa_ssa_pss_pb2.py
--rw-r-----   0 root         (0) root         (0)     4393 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/cached_dek_aead_pb2.py
--rw-r-----   0 root         (0) root         (0)     1694 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_ctr_hmac_streaming.proto
--rw-r-----   0 root         (0) root         (0)    15421 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/jwt_rsa_ssa_pkcs1_pb2.py
--rw-r-----   0 root         (0) root         (0)     1797 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/hpke.proto
--rw-r-----   0 root         (0) root         (0)     6000 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/common_pb2.py
--rw-r-----   0 root         (0) root         (0)     2539 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/jwt_rsa_ssa_pss.proto
--rw-r-----   0 root         (0) root         (0)     1410 2021-08-10 08:47:45.000000 tink-1.6.1/tink/proto/cached_dek_aead.proto
--rw-r-----   0 root         (0) root         (0)     7324 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/tink.proto
--rw-r-----   0 root         (0) root         (0)     3568 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/ecies_aead_hkdf.proto
--rw-r-----   0 root         (0) root         (0)     9739 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_ctr_hmac_streaming_pb2.py
--rw-r-----   0 root         (0) root         (0)    15203 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/ecies_aead_hkdf_pb2.py
--rw-r-----   0 root         (0) root         (0)     1101 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/aes_cmac_prf.proto
--rw-r-----   0 root         (0) root         (0)     1292 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/prf_based_deriver.proto
--rw-r-----   0 root         (0) root         (0)     6429 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_ctr_pb2.py
--rw-r-----   0 root         (0) root         (0)     1173 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_cmac.proto
--rw-r-----   0 root         (0) root         (0)     4162 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/kms_aead_pb2.py
--rw-r-----   0 root         (0) root         (0)     9053 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/jwt_hmac_pb2.py
--rw-r-----   0 root         (0) root         (0)     6429 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_eax_pb2.py
--rw-r-----   0 root         (0) root         (0)     1584 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/kms_envelope.proto
--rw-r-----   0 root         (0) root         (0)    12753 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/rsa_ssa_pkcs1_pb2.py
--rw-r-----   0 root         (0) root         (0)     1251 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_ctr_hmac_aead.proto
--rw-r-----   0 root         (0) root         (0)     1254 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/hmac.proto
--rw-r-----   0 root         (0) root         (0)    12823 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/hpke_pb2.py
--rw-r-----   0 root         (0) root         (0)     1106 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/xchacha20_poly1305.proto
--rw-r-----   0 root         (0) root         (0)     1178 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_gcm.proto
--rw-r-----   0 root         (0) root         (0)     5326 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/test_proto_pb2.py
--rw-r-----   0 root         (0) root         (0)     1244 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/aes_eax.proto
--rw-r-----   0 root         (0) root         (0)     6471 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_cmac_pb2.py
--rw-r-----   0 root         (0) root         (0)     2551 2021-08-10 08:45:24.000000 tink-1.6.1/tink/proto/jwt_rsa_ssa_pkcs1.proto
--rw-r-----   0 root         (0) root         (0)     7588 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/prf_based_deriver_pb2.py
--rw-r-----   0 root         (0) root         (0)     7201 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/hmac_prf_pb2.py
--rw-r-----   0 root         (0) root         (0)     1295 2021-08-10 08:41:24.000000 tink-1.6.1/tink/proto/hkdf_prf.proto
--rw-r-----   0 root         (0) root         (0)     2775 2020-10-15 19:17:20.000000 tink-1.6.1/tink/proto/rsa_ssa_pkcs1.proto
--rw-r-----   0 root         (0) root         (0)     8969 2021-08-10 09:14:23.000000 tink-1.6.1/tink/proto/aes_gcm_hkdf_streaming_pb2.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/streaming_aead/
--rw-r-----   0 root         (0) root         (0)     4959 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_raw_streaming_aead.py
--rw-r-----   0 root         (0) root         (0)     4626 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead_test.py
--rw-r-----   0 root         (0) root         (0)     9070 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     3907 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_encrypting_stream_test.py
--rw-r-----   0 root         (0) root         (0)     5276 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_decrypting_stream.py
--rw-r-----   0 root         (0) root         (0)     2344 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_file_object_adapter.py
--rw-r-----   0 root         (0) root         (0)     3148 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead_key_manager.py
--rw-r-----   0 root         (0) root         (0)     4723 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead.py
--rw-r-----   0 root         (0) root         (0)     5269 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     6706 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead_wrapper.py
--rw-r-----   0 root         (0) root         (0)     1059 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/__init__.py
--rw-r-----   0 root         (0) root         (0)     3319 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_rewindable_input_stream.py
--rw-r-----   0 root         (0) root         (0)     6413 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_rewindable_input_stream_test.py
--rw-r-----   0 root         (0) root         (0)     3006 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_decrypting_stream_test.py
--rw-r-----   0 root         (0) root         (0)     9611 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)     5314 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead_key_templates.py
--rw-r-----   0 root         (0) root         (0)     4080 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_encrypting_stream.py
--rw-r-----   0 root         (0) root         (0)     4189 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_file_object_adapter_test.py
--rw-r-----   0 root         (0) root         (0)     4524 2021-08-10 08:41:24.000000 tink-1.6.1/tink/streaming_aead/_streaming_aead_key_templates_test.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/jwt/
--rw-r-----   0 root         (0) root         (0)    13199 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/_jwt_signature_key_manager.py
--rw-r-----   0 root         (0) root         (0)     3341 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/_jwt_mac.py
--rw-r-----   0 root         (0) root         (0)     7204 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/_jwt_mac_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)     2573 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_verified_jwt.py
--rw-r-----   0 root         (0) root         (0)     8887 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_hmac_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     7947 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_validator.py
--rw-r-----   0 root         (0) root         (0)    16505 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_format_test.py
--rw-r-----   0 root         (0) root         (0)     2267 2021-08-10 08:41:24.000000 tink-1.6.1/tink/jwt/_jwt_public_key_verify.py
--rw-r-----   0 root         (0) root         (0)     6371 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_key_templates_test.py
--rw-r-----   0 root         (0) root         (0)     7881 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_signature_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     5216 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/_jwt_hmac_key_manager.py
--rw-r-----   0 root         (0) root         (0)     7358 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_format.py
--rw-r-----   0 root         (0) root         (0)     6716 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     5822 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/__init__.py
--rw-r-----   0 root         (0) root         (0)    10764 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/_jwt_signature_wrappers_test.py
--rw-r-----   0 root         (0) root         (0)      682 2021-08-10 08:41:24.000000 tink-1.6.1/tink/jwt/_jwt_error.py
--rw-r-----   0 root         (0) root         (0)     7912 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_key_templates.py
--rw-r-----   0 root         (0) root         (0)    14930 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/_raw_jwt_test.py
--rw-r-----   0 root         (0) root         (0)    14981 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_validator_test.py
--rw-r-----   0 root         (0) root         (0)     7726 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_raw_jwt.py
--rw-r-----   0 root         (0) root         (0)     3478 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_mac_wrapper.py
--rw-r-----   0 root         (0) root         (0)     1885 2021-08-10 08:47:45.000000 tink-1.6.1/tink/jwt/_jwt_public_key_sign.py
--rw-r-----   0 root         (0) root         (0)     4150 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_verified_jwt_test.py
--rw-r-----   0 root         (0) root         (0)     4193 2021-08-10 08:45:24.000000 tink-1.6.1/tink/jwt/_jwt_signature_wrappers.py
--rw-r-----   0 root         (0) root         (0)     4318 2021-08-10 08:41:24.000000 tink-1.6.1/tink/tink_config_test.py
--rw-r-----   0 root         (0) root         (0)     2727 2021-08-10 08:41:24.000000 tink-1.6.1/tink/_keyset_reader.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/hybrid/
--rw-r-----   0 root         (0) root         (0)     3147 2021-08-10 08:41:24.000000 tink-1.6.1/tink/hybrid/_hybrid_key_templates.py
--rw-r-----   0 root         (0) root         (0)     2681 2020-10-15 19:17:20.000000 tink-1.6.1/tink/hybrid/_hybrid_encrypt.py
--rw-r-----   0 root         (0) root         (0)     6077 2020-10-15 19:17:20.000000 tink-1.6.1/tink/hybrid/_hybrid_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)     2697 2021-08-10 08:41:24.000000 tink-1.6.1/tink/hybrid/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     3896 2021-08-10 08:41:24.000000 tink-1.6.1/tink/hybrid/_hybrid_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     1083 2020-10-15 19:17:20.000000 tink-1.6.1/tink/hybrid/__init__.py
--rw-r-----   0 root         (0) root         (0)     4204 2020-10-15 19:17:20.000000 tink-1.6.1/tink/hybrid/_hybrid_wrapper.py
--rw-r-----   0 root         (0) root         (0)     3128 2021-08-10 08:41:24.000000 tink-1.6.1/tink/hybrid/_hybrid_key_templates_test.py
--rw-r-----   0 root         (0) root         (0)     2869 2020-10-15 19:17:20.000000 tink-1.6.1/tink/hybrid/_hybrid_key_manager.py
--rw-r-----   0 root         (0) root         (0)     2674 2020-10-15 19:17:20.000000 tink-1.6.1/tink/hybrid/_hybrid_decrypt.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/mac/
--rw-r-----   0 root         (0) root         (0)     5157 2020-10-15 19:17:20.000000 tink-1.6.1/tink/mac/_mac_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)     3032 2020-10-15 19:17:20.000000 tink-1.6.1/tink/mac/_mac_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)     1822 2020-10-15 19:17:20.000000 tink-1.6.1/tink/mac/_mac_key_manager.py
--rw-r-----   0 root         (0) root         (0)     2344 2021-08-10 08:41:24.000000 tink-1.6.1/tink/mac/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)      930 2020-10-15 19:17:20.000000 tink-1.6.1/tink/mac/__init__.py
--rw-r-----   0 root         (0) root         (0)     2343 2021-08-10 08:41:24.000000 tink-1.6.1/tink/mac/_mac_key_templates_test.py
--rw-r-----   0 root         (0) root         (0)     1902 2020-10-15 19:17:20.000000 tink-1.6.1/tink/mac/_mac.py
--rw-r-----   0 root         (0) root         (0)     3518 2021-08-10 08:41:24.000000 tink-1.6.1/tink/mac/_mac_wrapper.py
--rw-r-----   0 root         (0) root         (0)     2765 2020-10-15 19:17:20.000000 tink-1.6.1/tink/mac/_mac_key_templates.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink/prf/
--rw-r-----   0 root         (0) root         (0)     1876 2021-08-10 08:41:24.000000 tink-1.6.1/tink/prf/_prf_key_manager.py
--rw-r-----   0 root         (0) root         (0)     2089 2021-08-10 08:41:24.000000 tink-1.6.1/tink/prf/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     3912 2021-08-10 08:41:24.000000 tink-1.6.1/tink/prf/_prf_key_manager_test.py
--rw-r-----   0 root         (0) root         (0)      965 2020-10-15 19:17:20.000000 tink-1.6.1/tink/prf/__init__.py
--rw-r-----   0 root         (0) root         (0)     1994 2021-08-10 08:41:24.000000 tink-1.6.1/tink/prf/_prf_set_wrapper.py
--rw-r-----   0 root         (0) root         (0)     3346 2021-08-10 08:41:24.000000 tink-1.6.1/tink/prf/_prf_set.py
--rw-r-----   0 root         (0) root         (0)     2859 2021-08-10 08:41:24.000000 tink-1.6.1/tink/prf/_prf_set_wrapper_test.py
--rw-r-----   0 root         (0) root         (0)     3297 2021-08-10 08:41:24.000000 tink-1.6.1/tink/prf/_prf_key_templates.py
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tink.egg-info/
--rw-r-----   0 root         (0) root         (0)        1 2021-08-10 09:14:23.000000 tink-1.6.1/tink.egg-info/dependency_links.txt
--rw-r-----   0 root         (0) root         (0)       34 2021-08-10 09:14:23.000000 tink-1.6.1/tink.egg-info/top_level.txt
--rw-r-----   0 root         (0) root         (0)    10040 2021-08-10 09:14:23.000000 tink-1.6.1/tink.egg-info/SOURCES.txt
--rw-r-----   0 root         (0) root         (0)       21 2021-08-10 09:14:23.000000 tink-1.6.1/tink.egg-info/requires.txt
--rw-r-----   0 root         (0) root         (0)        1 2021-08-10 09:14:23.000000 tink-1.6.1/tink.egg-info/not-zip-safe
--rw-r-----   0 root         (0) root         (0)     1660 2021-08-10 09:14:23.000000 tink-1.6.1/tink.egg-info/PKG-INFO
--rw-r-----   0 root         (0) root         (0)      409 2020-10-15 19:17:20.000000 tink-1.6.1/MANIFEST.in
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tools/
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tools/build_defs/
--rw-r-----   0 root         (0) root         (0)     1919 2020-10-15 19:17:20.000000 tink-1.6.1/tools/build_defs/tink_python_rules.bzl
--rw-r-----   0 root         (0) root         (0)       76 2020-10-15 19:17:20.000000 tink-1.6.1/tools/build_defs/BUILD.bazel
-drwxr-x---   0 root         (0) root         (0)        0 2021-08-10 09:14:23.000000 tink-1.6.1/tools/distribution/
--rwxr-x---   0 root         (0) root         (0)     4452 2021-08-10 08:47:45.000000 tink-1.6.1/tools/distribution/create_release.sh
--rwxr-x---   0 root         (0) root         (0)     1837 2021-08-10 08:41:24.000000 tink-1.6.1/tools/distribution/test_linux_binary_wheels.sh
--rwxr-x---   0 root         (0) root         (0)     2912 2021-08-10 08:41:24.000000 tink-1.6.1/tools/distribution/build_linux_binary_wheels.sh
--rw-r-----   0 root         (0) root         (0)     1805 2021-08-10 08:41:24.000000 tink-1.6.1/tools/distribution/README.md
--rw-r-----   0 root         (0) root         (0)       76 2020-10-15 19:17:20.000000 tink-1.6.1/tools/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)     1447 2020-10-15 19:17:20.000000 tink-1.6.1/tink_py_deps.bzl
--rw-r-----   0 root         (0) root         (0)       21 2020-10-15 19:17:20.000000 tink-1.6.1/requirements.txt
--rw-r-----   0 root         (0) root         (0)      406 2020-10-15 19:17:20.000000 tink-1.6.1/tink_py_deps_init.bzl
--rw-r-----   0 root         (0) root         (0)       76 2021-08-10 08:41:24.000000 tink-1.6.1/VERSION
--rw-r-----   0 root         (0) root         (0)        0 2020-10-15 19:17:20.000000 tink-1.6.1/BUILD.bazel
--rw-r-----   0 root         (0) root         (0)    10254 2021-08-10 08:47:45.000000 tink-1.6.1/setup.py
--rw-r-----   0 root         (0) root         (0)       38 2021-08-10 09:14:23.000000 tink-1.6.1/setup.cfg
--rw-r-----   0 root         (0) root         (0)     1660 2021-08-10 09:14:23.000000 tink-1.6.1/PKG-INFO
--rw-r-----   0 root         (0) root         (0)      838 2020-10-15 19:17:20.000000 tink-1.6.1/WORKSPACE
--rw-r-----   0 root         (0) root         (0)     1043 2020-10-15 19:17:20.000000 tink-1.6.1/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.802082 tink-1.7.0/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-10 23:47:36.000000 tink-1.7.0/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      409 2022-08-10 23:47:36.000000 tink-1.7.0/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     1630 2022-08-26 08:30:17.802082 tink-1.7.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1033 2022-08-10 23:47:36.000000 tink-1.7.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)       76 2022-08-10 23:47:36.000000 tink-1.7.0/VERSION
+-rw-rw-r--   0 root         (0) root         (0)     1145 2022-08-11 02:05:40.000000 tink-1.7.0/WORKSPACE
+-rw-rw-r--   0 root         (0) root         (0)       25 2022-08-10 23:47:36.000000 tink-1.7.0/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       38 2022-08-26 08:30:17.806083 tink-1.7.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)    11007 2022-08-10 23:47:36.000000 tink-1.7.0/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.758078 tink-1.7.0/tink/
+-rw-rw-r--   0 root         (0) root         (0)     3847 2022-08-10 23:47:36.000000 tink-1.7.0/tink/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     1520 2022-08-10 23:47:36.000000 tink-1.7.0/tink/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11829 2022-08-10 23:47:36.000000 tink-1.7.0/tink/_keyset_handle.py
+-rw-rw-r--   0 root         (0) root         (0)    12888 2022-08-10 23:47:36.000000 tink-1.7.0/tink/_keyset_handle_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2497 2022-08-10 23:47:36.000000 tink-1.7.0/tink/_keyset_reader.py
+-rw-rw-r--   0 root         (0) root         (0)     4878 2022-08-10 23:47:36.000000 tink-1.7.0/tink/_keyset_reader_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2912 2022-08-10 23:47:36.000000 tink-1.7.0/tink/_keyset_writer.py
+-rw-rw-r--   0 root         (0) root         (0)     4531 2022-08-10 23:47:36.000000 tink-1.7.0/tink/_keyset_writer_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.762079 tink-1.7.0/tink/aead/
+-rw-rw-r--   0 root         (0) root         (0)     3268 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      937 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2133 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     1946 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_aead_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     6678 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_aead_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)    10166 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_aead_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     5270 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_aead_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2687 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_aead_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     4993 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_aead_wrapper_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3300 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_kms_envelope_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     4801 2022-08-10 23:47:36.000000 tink-1.7.0/tink/aead/_kms_envelope_aead_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.766079 tink-1.7.0/tink/cc/
+-rw-rw-r--   0 root         (0) root         (0)     6313 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      912 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_hpke_config.cc
+-rw-rw-r--   0 root         (0) root         (0)      964 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_hpke_config.h
+-rw-rw-r--   0 root         (0) root         (0)     2107 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_jwt_config.cc
+-rw-rw-r--   0 root         (0) root         (0)      986 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_jwt_config.h
+-rw-rw-r--   0 root         (0) root         (0)     4568 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_key_manager.h
+-rw-rw-r--   0 root         (0) root         (0)     2347 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_streaming_aead_wrappers.cc
+-rw-rw-r--   0 root         (0) root         (0)     2478 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_streaming_aead_wrappers.h
+-rw-rw-r--   0 root         (0) root         (0)     1729 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_streaming_aead_wrappers_test.cc
+-rw-rw-r--   0 root         (0) root         (0)     1083 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_tink_config.cc
+-rw-rw-r--   0 root         (0) root         (0)      968 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/cc_tink_config.h
+-rw-rw-r--   0 root         (0) root         (0)     1464 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/input_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1543 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/input_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     4136 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/input_stream_adapter_test.cc
+-rw-rw-r--   0 root         (0) root         (0)     1561 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/output_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1792 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/output_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     3492 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/output_stream_adapter_test.cc
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.770079 tink-1.7.0/tink/cc/pybind/
+-rw-rw-r--   0 root         (0) root         (0)     8056 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     3178 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/aead.cc
+-rw-rw-r--   0 root         (0) root         (0)      969 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/aead.h
+-rw-rw-r--   0 root         (0) root         (0)     2929 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_aws_kms_client.cc
+-rw-rw-r--   0 root         (0) root         (0)     1107 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_aws_kms_client.h
+-rw-rw-r--   0 root         (0) root         (0)     1697 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_fake_kms_client_testonly.cc
+-rw-rw-r--   0 root         (0) root         (0)     1063 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_fake_kms_client_testonly.h
+-rw-rw-r--   0 root         (0) root         (0)     2960 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_gcp_kms_client.cc
+-rw-rw-r--   0 root         (0) root         (0)     1107 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_gcp_kms_client.h
+-rw-rw-r--   0 root         (0) root         (0)     1264 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_hpke_config.cc
+-rw-rw-r--   0 root         (0) root         (0)     1003 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_hpke_config.h
+-rw-rw-r--   0 root         (0) root         (0)     1246 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_jwt_config.cc
+-rw-rw-r--   0 root         (0) root         (0)      997 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_jwt_config.h
+-rw-rw-r--   0 root         (0) root         (0)     3745 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_key_manager.cc
+-rw-rw-r--   0 root         (0) root         (0)     1002 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_key_manager.h
+-rw-rw-r--   0 root         (0) root         (0)    25593 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2800 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_streaming_aead_wrappers.cc
+-rw-rw-r--   0 root         (0) root         (0)     1048 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_streaming_aead_wrappers.h
+-rw-rw-r--   0 root         (0) root         (0)     1025 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_tink_config.cc
+-rw-rw-r--   0 root         (0) root         (0)     1001 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_tink_config.h
+-rw-rw-r--   0 root         (0) root         (0)      855 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/cc_tink_config_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3658 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/deterministic_aead.cc
+-rw-rw-r--   0 root         (0) root         (0)     1019 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/deterministic_aead.h
+-rw-rw-r--   0 root         (0) root         (0)     1821 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/hybrid_decrypt.cc
+-rw-rw-r--   0 root         (0) root         (0)     1003 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/hybrid_decrypt.h
+-rw-rw-r--   0 root         (0) root         (0)     1816 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/hybrid_encrypt.cc
+-rw-rw-r--   0 root         (0) root         (0)     1003 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/hybrid_encrypt.h
+-rw-rw-r--   0 root         (0) root         (0)     1141 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/import_helper.cc
+-rw-rw-r--   0 root         (0) root         (0)     1205 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/import_helper.h
+-rw-rw-r--   0 root         (0) root         (0)     2359 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/input_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1026 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/input_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     2515 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/mac.cc
+-rw-rw-r--   0 root         (0) root         (0)      960 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/mac.h
+-rw-rw-r--   0 root         (0) root         (0)     1829 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/output_stream_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1030 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/output_stream_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     1886 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/prf.cc
+-rw-rw-r--   0 root         (0) root         (0)      965 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/prf.h
+-rw-rw-r--   0 root         (0) root         (0)     2239 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/public_key_sign.cc
+-rw-rw-r--   0 root         (0) root         (0)     1006 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/public_key_sign.h
+-rw-rw-r--   0 root         (0) root         (0)     2329 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/public_key_verify.cc
+-rw-rw-r--   0 root         (0) root         (0)     1013 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/public_key_verify.h
+-rw-rw-r--   0 root         (0) root         (0)     4757 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/python_file_object_adapter.cc
+-rw-rw-r--   0 root         (0) root         (0)     1049 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/python_file_object_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     1882 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/streaming_aead.cc
+-rw-rw-r--   0 root         (0) root         (0)     1008 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/streaming_aead.h
+-rw-rw-r--   0 root         (0) root         (0)     2700 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/tink_bindings.cc
+-rw-rw-r--   0 root         (0) root         (0)     1425 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/pybind/tink_exception.h
+-rw-rw-r--   0 root         (0) root         (0)     1767 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/python_file_object_adapter.h
+-rw-rw-r--   0 root         (0) root         (0)     3353 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/python_input_stream.cc
+-rw-rw-r--   0 root         (0) root         (0)     2210 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/python_input_stream.h
+-rw-rw-r--   0 root         (0) root         (0)     6559 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/python_input_stream_test.cc
+-rw-rw-r--   0 root         (0) root         (0)     4123 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/python_output_stream.cc
+-rw-rw-r--   0 root         (0) root         (0)     2241 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/python_output_stream.h
+-rw-rw-r--   0 root         (0) root         (0)     7393 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/python_output_stream_test.cc
+-rw-rw-r--   0 root         (0) root         (0)    11511 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cc/test_util.h
+-rw-rw-r--   0 root         (0) root         (0)     1468 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cleartext_keyset_handle.py
+-rw-rw-r--   0 root         (0) root         (0)     2013 2022-08-10 23:47:36.000000 tink-1.7.0/tink/cleartext_keyset_handle_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.774080 tink-1.7.0/tink/core/
+-rw-rw-r--   0 root         (0) root         (0)     2575 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     1450 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1494 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_crypto_format.py
+-rw-rw-r--   0 root         (0) root         (0)     2729 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_crypto_format_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5259 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     3610 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_primitive_set.py
+-rw-rw-r--   0 root         (0) root         (0)     9880 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_primitive_set_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1766 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_primitive_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     9078 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_registry.py
+-rw-rw-r--   0 root         (0) root         (0)    14510 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_registry_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1302 2022-08-10 23:47:36.000000 tink-1.7.0/tink/core/_tink_error.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.774080 tink-1.7.0/tink/daead/
+-rw-rw-r--   0 root         (0) root         (0)     2343 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      914 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1956 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/_deterministic_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     2129 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/_deterministic_aead_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     2555 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/_deterministic_aead_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1820 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/_deterministic_aead_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     1624 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/_deterministic_aead_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3400 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/_deterministic_aead_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     5917 2022-08-10 23:47:36.000000 tink-1.7.0/tink/daead/_deterministic_aead_wrapper_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.778080 tink-1.7.0/tink/hybrid/
+-rw-rw-r--   0 root         (0) root         (0)     2710 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      927 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2470 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_decrypt.py
+-rw-rw-r--   0 root         (0) root         (0)     2477 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_encrypt.py
+-rw-rw-r--   0 root         (0) root         (0)     3669 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     8262 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5889 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3060 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4146 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     9752 2022-08-10 23:47:36.000000 tink-1.7.0/tink/hybrid/_hybrid_wrapper_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.778080 tink-1.7.0/tink/integration/
+-rw-rw-r--   0 root         (0) root         (0)      575 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/__init__.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.778080 tink-1.7.0/tink/integration/awskms/
+-rw-rw-r--   0 root         (0) root         (0)     1287 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/awskms/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      703 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/awskms/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2996 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/awskms/_aws_kms_aead_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2860 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/awskms/_aws_kms_client.py
+-rw-rw-r--   0 root         (0) root         (0)     2072 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/awskms/_aws_kms_client_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.778080 tink-1.7.0/tink/integration/gcpkms/
+-rw-rw-r--   0 root         (0) root         (0)     1146 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/gcpkms/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      697 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/gcpkms/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3459 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/gcpkms/_gcp_kms_aead_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2630 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/gcpkms/_gcp_kms_client.py
+-rw-rw-r--   0 root         (0) root         (0)     1878 2022-08-10 23:47:36.000000 tink-1.7.0/tink/integration/gcpkms/_gcp_kms_client_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.778080 tink-1.7.0/tink/internal/
+-rw-rw-r--   0 root         (0) root         (0)      504 2022-08-10 23:47:36.000000 tink-1.7.0/tink/internal/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      575 2022-08-10 23:47:36.000000 tink-1.7.0/tink/internal/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      918 2022-08-10 23:47:36.000000 tink-1.7.0/tink/internal/big_integer_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1578 2022-08-10 23:47:36.000000 tink-1.7.0/tink/internal/big_integer_util_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.782081 tink-1.7.0/tink/jwt/
+-rw-rw-r--   0 root         (0) root         (0)     7950 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     4228 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1789 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_json_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1839 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_json_util_test.py
+-rw-rw-r--   0 root         (0) root         (0)    12814 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwk_set_converter.py
+-rw-rw-r--   0 root         (0) root         (0)    37848 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwk_set_converter_test.py
+-rw-rw-r--   0 root         (0) root         (0)      682 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_error.py
+-rw-rw-r--   0 root         (0) root         (0)     7133 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_format.py
+-rw-rw-r--   0 root         (0) root         (0)    17449 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_format_test.py
+-rw-rw-r--   0 root         (0) root         (0)     5063 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_hmac_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)    12970 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_hmac_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     7622 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3975 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3153 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_mac.py
+-rw-rw-r--   0 root         (0) root         (0)     3344 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_mac_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)    10572 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_mac_wrapper_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1674 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_public_key_sign.py
+-rw-rw-r--   0 root         (0) root         (0)     2546 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_public_key_verify.py
+-rw-rw-r--   0 root         (0) root         (0)    13099 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_signature_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)    11632 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_signature_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4077 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_signature_wrappers.py
+-rw-rw-r--   0 root         (0) root         (0)    13424 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_signature_wrappers_test.py
+-rw-rw-r--   0 root         (0) root         (0)     8268 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_validator.py
+-rw-rw-r--   0 root         (0) root         (0)    14891 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_jwt_validator_test.py
+-rw-rw-r--   0 root         (0) root         (0)     9502 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_raw_jwt.py
+-rw-rw-r--   0 root         (0) root         (0)    15662 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_raw_jwt_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2910 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_verified_jwt.py
+-rw-rw-r--   0 root         (0) root         (0)     4149 2022-08-10 23:47:36.000000 tink-1.7.0/tink/jwt/_verified_jwt_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.786081 tink-1.7.0/tink/mac/
+-rw-rw-r--   0 root         (0) root         (0)     2216 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      774 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1698 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/_mac.py
+-rw-rw-r--   0 root         (0) root         (0)     1665 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/_mac_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     2921 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/_mac_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3396 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/_mac_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     2048 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/_mac_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3361 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/_mac_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     5000 2022-08-10 23:47:36.000000 tink-1.7.0/tink/mac/_mac_wrapper_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.786081 tink-1.7.0/tink/prf/
+-rw-rw-r--   0 root         (0) root         (0)     1961 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      809 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1720 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/_prf_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     3336 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/_prf_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3141 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/_prf_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3127 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/_prf_set.py
+-rw-rw-r--   0 root         (0) root         (0)     1838 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/_prf_set_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     2749 2022-08-10 23:47:36.000000 tink-1.7.0/tink/prf/_prf_set_wrapper_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.798082 tink-1.7.0/tink/proto/
+-rw-rw-r--   0 root         (0) root         (0)     5468 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      575 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1173 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_cmac.proto
+-rw-r--r--   0 root         (0) root         (0)     2663 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_cmac_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1101 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_cmac_prf.proto
+-rw-r--r--   0 root         (0) root         (0)     2140 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_cmac_prf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1165 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_ctr.proto
+-rw-rw-r--   0 root         (0) root         (0)     1251 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_ctr_hmac_aead.proto
+-rw-r--r--   0 root         (0) root         (0)     2686 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_ctr_hmac_aead_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1694 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_ctr_hmac_streaming.proto
+-rw-r--r--   0 root         (0) root         (0)     3635 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_ctr_hmac_streaming_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_ctr_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1244 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_eax.proto
+-rw-r--r--   0 root         (0) root         (0)     2637 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_eax_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2586 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_gcm.proto
+-rw-rw-r--   0 root         (0) root         (0)     1596 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_gcm_hkdf_streaming.proto
+-rw-r--r--   0 root         (0) root         (0)     3460 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_gcm_hkdf_streaming_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_gcm_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1191 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_gcm_siv.proto
+-rw-r--r--   0 root         (0) root         (0)     2125 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_gcm_siv_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1166 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/aes_siv.proto
+-rw-r--r--   0 root         (0) root         (0)     2033 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/aes_siv_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1409 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/cached_dek_aead.proto
+-rw-r--r--   0 root         (0) root         (0)     2232 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/cached_dek_aead_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1560 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/cached_dek_envelope.proto
+-rw-r--r--   0 root         (0) root         (0)     2614 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/cached_dek_envelope_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1199 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/chacha20_poly1305.proto
+-rw-r--r--   0 root         (0) root         (0)     2219 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/chacha20_poly1305_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1510 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/common.proto
+-rw-r--r--   0 root         (0) root         (0)     2403 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1974 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/config.proto
+-rw-r--r--   0 root         (0) root         (0)     2439 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/config_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2529 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/ecdsa.proto
+-rw-r--r--   0 root         (0) root         (0)     4099 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/ecdsa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     3568 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/ecies_aead_hkdf.proto
+-rw-r--r--   0 root         (0) root         (0)     5450 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/ecies_aead_hkdf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1752 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/ed25519.proto
+-rw-r--r--   0 root         (0) root         (0)     2783 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/ed25519_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      897 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/empty.proto
+-rw-r--r--   0 root         (0) root         (0)     1353 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/empty_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1295 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/hkdf_prf.proto
+-rw-r--r--   0 root         (0) root         (0)     2856 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/hkdf_prf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1254 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/hmac.proto
+-rw-r--r--   0 root         (0) root         (0)     2740 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/hmac_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1252 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/hmac_prf.proto
+-rw-r--r--   0 root         (0) root         (0)     2826 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/hmac_prf_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1891 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/hpke.proto
+-rw-r--r--   0 root         (0) root         (0)     4767 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/hpke_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1994 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/jwt_ecdsa.proto
+-rw-r--r--   0 root         (0) root         (0)     4109 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/jwt_ecdsa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1573 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/jwt_hmac.proto
+-rw-r--r--   0 root         (0) root         (0)     3291 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/jwt_hmac_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2732 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/jwt_rsa_ssa_pkcs1.proto
+-rw-r--r--   0 root         (0) root         (0)     4712 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/jwt_rsa_ssa_pkcs1_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2765 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/jwt_rsa_ssa_pss.proto
+-rw-r--r--   0 root         (0) root         (0)     4607 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/jwt_rsa_ssa_pss_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1385 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/kms_aead.proto
+-rw-r--r--   0 root         (0) root         (0)     2050 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/kms_aead_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1584 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/kms_envelope.proto
+-rw-r--r--   0 root         (0) root         (0)     2425 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/kms_envelope_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1292 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/prf_based_deriver.proto
+-rw-r--r--   0 root         (0) root         (0)     3224 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/prf_based_deriver_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2775 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/rsa_ssa_pkcs1.proto
+-rw-r--r--   0 root         (0) root         (0)     3987 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/rsa_ssa_pkcs1_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     3089 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/rsa_ssa_pss.proto
+-rw-r--r--   0 root         (0) root         (0)     4008 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/rsa_ssa_pss_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1076 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/test_proto.proto
+-rw-r--r--   0 root         (0) root         (0)     2653 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/test_proto_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     7230 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/tink.proto
+-rw-r--r--   0 root         (0) root         (0)     6552 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/tink_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     1106 2022-08-10 23:47:36.000000 tink-1.7.0/tink/proto/xchacha20_poly1305.proto
+-rw-r--r--   0 root         (0) root         (0)     2274 2022-08-10 23:49:06.000000 tink-1.7.0/tink/proto/xchacha20_poly1305_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      882 2022-08-10 23:47:36.000000 tink-1.7.0/tink/secret_key_access.py
+-rw-rw-r--   0 root         (0) root         (0)     1268 2022-08-10 23:47:36.000000 tink-1.7.0/tink/secret_key_access_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.798082 tink-1.7.0/tink/signature/
+-rw-rw-r--   0 root         (0) root         (0)     2338 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      966 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1380 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/_public_key_sign.py
+-rw-rw-r--   0 root         (0) root         (0)     1507 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/_public_key_verify.py
+-rw-rw-r--   0 root         (0) root         (0)     2887 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/_signature_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     4901 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/_signature_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     7852 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/_signature_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     5265 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/_signature_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     5885 2022-08-10 23:47:36.000000 tink-1.7.0/tink/signature/_signature_wrapper_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.802082 tink-1.7.0/tink/streaming_aead/
+-rw-rw-r--   0 root         (0) root         (0)     5311 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      904 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4767 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_decrypting_stream.py
+-rw-rw-r--   0 root         (0) root         (0)     2896 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_decrypting_stream_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3874 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_encrypting_stream.py
+-rw-rw-r--   0 root         (0) root         (0)     3778 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_encrypting_stream_test.py
+-rw-rw-r--   0 root         (0) root         (0)     2165 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_file_object_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     4079 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_file_object_adapter_test.py
+-rw-rw-r--   0 root         (0) root         (0)     3176 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_pybind11_python_file_object_adapter_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4756 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_raw_streaming_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     3109 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_rewindable_input_stream.py
+-rw-rw-r--   0 root         (0) root         (0)     6303 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_rewindable_input_stream_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4520 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead.py
+-rw-rw-r--   0 root         (0) root         (0)     2894 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead_key_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     8960 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead_key_manager_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6594 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead_key_templates.py
+-rw-rw-r--   0 root         (0) root         (0)     3569 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead_key_templates_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4470 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6490 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead_wrapper.py
+-rw-rw-r--   0 root         (0) root         (0)     9501 2022-08-10 23:47:36.000000 tink-1.7.0/tink/streaming_aead/_streaming_aead_wrapper_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.802082 tink-1.7.0/tink/testing/
+-rw-rw-r--   0 root         (0) root         (0)     2060 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)      575 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3518 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/bytes_io.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/bytes_io_test.py
+-rw-rw-r--   0 root         (0) root         (0)      916 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/fake_kms.py
+-rw-rw-r--   0 root         (0) root         (0)     2041 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/fake_kms_test.py
+-rw-rw-r--   0 root         (0) root         (0)     6601 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/helper.py
+-rw-rw-r--   0 root         (0) root         (0)     5409 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/helper_test.py
+-rw-rw-r--   0 root         (0) root         (0)     4487 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/keyset_builder.py
+-rw-rw-r--   0 root         (0) root         (0)     7016 2022-08-10 23:47:36.000000 tink-1.7.0/tink/testing/keyset_builder_test.py
+-rw-rw-r--   0 root         (0) root         (0)      965 2022-08-10 23:47:36.000000 tink-1.7.0/tink/tink_config.py
+-rw-rw-r--   0 root         (0) root         (0)     4207 2022-08-10 23:47:36.000000 tink-1.7.0/tink/tink_config_test.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.758078 tink-1.7.0/tink.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1630 2022-08-26 08:30:17.000000 tink-1.7.0/tink.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10124 2022-08-26 08:30:17.000000 tink-1.7.0/tink.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 08:30:17.000000 tink-1.7.0/tink.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-11 00:34:41.000000 tink-1.7.0/tink.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2022-08-26 08:30:17.000000 tink-1.7.0/tink.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2022-08-26 08:30:17.000000 tink-1.7.0/tink.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1414 2022-08-10 23:47:36.000000 tink-1.7.0/tink_py_deps.bzl
+-rw-rw-r--   0 root         (0) root         (0)      275 2022-08-10 23:47:36.000000 tink-1.7.0/tink_py_deps_init.bzl
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.802082 tink-1.7.0/tools/
+-rw-rw-r--   0 root         (0) root         (0)       76 2022-08-10 23:47:36.000000 tink-1.7.0/tools/BUILD.bazel
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.802082 tink-1.7.0/tools/build_defs/
+-rw-rw-r--   0 root         (0) root         (0)       76 2022-08-10 23:47:36.000000 tink-1.7.0/tools/build_defs/BUILD.bazel
+-rw-rw-r--   0 root         (0) root         (0)     1690 2022-08-10 23:47:36.000000 tink-1.7.0/tools/build_defs/tink_python_rules.bzl
+drwxrwxr-x   0 root         (0) root         (0)        0 2022-08-26 08:30:17.802082 tink-1.7.0/tools/distribution/
+-rw-rw-r--   0 root         (0) root         (0)     1819 2022-08-10 23:47:36.000000 tink-1.7.0/tools/distribution/README.md
+-rwxrwxr-x   0 root         (0) root         (0)     3094 2022-08-10 23:47:36.000000 tink-1.7.0/tools/distribution/build_linux_binary_wheels.sh
+-rwxrwxr-x   0 root         (0) root         (0)     5814 2022-08-26 08:07:04.000000 tink-1.7.0/tools/distribution/create_release.sh
+-rwxrwxr-x   0 root         (0) root         (0)     2160 2022-08-10 23:47:36.000000 tink-1.7.0/tools/distribution/test_linux_binary_wheels.sh
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tink-1.6.1/tink/integration/gcpkms/_gcp_kms_aead_test.py` & `tink-1.7.0/tink/integration/gcpkms/_gcp_kms_aead_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.integration.gcp_kms_aead."""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
 
 import os
 
 from absl.testing import absltest
 
 from tink import core
 from tink.integration import gcpkms
 from tink.testing import helper
 
-CREDENTIAL_PATH = os.path.join(helper.tink_root_path(),
-                               'testdata/credential.json')
+CREDENTIAL_PATH = os.path.join(helper.tink_py_testdata_path(),
+                               'gcp/credential.json')
 KEY_URI = 'gcp-kms://projects/tink-test-infrastructure/locations/global/keyRings/unit-and-integration-testing/cryptoKeys/aead-key'
 LOCAL_KEY_URI = 'gcp-kms://projects/tink-test-infrastructure/locations/europe-west1/keyRings/unit-and-integration-test/cryptoKeys/aead-key'
 BAD_KEY_URI = 'aws-kms://arn:aws:kms:us-east-2:235739564943:key/3ee50705-5a82-4f5b-9753-05c4f473922f'
 
 if 'TEST_SRCDIR' in os.environ:
   # Set root certificates for gRPC in Bazel Test which are needed on MacOS
   os.environ['GRPC_DEFAULT_SSL_ROOTS_FILE_PATH'] = os.path.join(
@@ -85,10 +82,8 @@
       tmp_ciphertext = list(ciphertext)
       tmp_ciphertext[byte_idx] ^= 1
       corrupted_ciphertext = bytes(tmp_ciphertext)
       with self.assertRaises(core.TinkError):
         aead.decrypt(corrupted_ciphertext, b'')
 
 if __name__ == '__main__':
-  # TODO(b/154273145): re-enable this.
-  pass
-  # absltest.main()
+  absltest.main()
```

### Comparing `tink-1.6.1/tink/integration/gcpkms/_gcp_kms_client.py` & `tink-1.7.0/tink/integration/gcpkms/_gcp_kms_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,36 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A client for Google Cloud KMS."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
-from typing import Text
-
 from tink import aead
 from tink import core
 from tink.cc.pybind import tink_bindings
 
 GCP_KEYURI_PREFIX = 'gcp-kms://'
 
 
-class GcpKmsClient(object):
+class GcpKmsClient:
   """Basic GCP client for AEAD."""
 
-  def __init__(self, key_uri: Text, credentials_path: Text):
+  def __init__(self, key_uri: str, credentials_path: str):
     """Creates a new GcpKmsClient that is bound to the key specified in 'key_uri'.
 
-    Uses the specifed credentials when communicating with the KMS. Either of
+    Uses the specified credentials when communicating with the KMS. Either of
     arguments can be empty.
 
     If 'key_uri' is empty, then the client is not bound to any particular key.
     If 'credential_path' is empty, then default credentials will be used.
 
     Args:
       key_uri: Text, URI of the key the client should be bound to.
@@ -54,27 +47,27 @@
       self._key_uri = key_uri
     else:
       raise core.TinkError
 
     # Use the C++ GCP KMS client
     self.cc_client = tink_bindings.GcpKmsClient(key_uri, credentials_path)
 
-  def does_support(self, key_uri: Text) -> bool:
+  def does_support(self, key_uri: str) -> bool:
     """Returns true iff this client supports KMS key specified in 'key_uri'.
 
     Args:
       key_uri: Text, URI of the key to be checked.
 
     Returns:
       A boolean value which is true if the key is supported and false otherwise.
     """
     return self.cc_client.does_support(key_uri)
 
   @core.use_tink_errors
-  def get_aead(self, key_uri: Text) -> aead.Aead:
+  def get_aead(self, key_uri: str) -> aead.Aead:
     """Returns an Aead-primitive backed by KMS key specified by 'key_uri'.
 
     Args:
       key_uri: Text, URI of the key which should be used.
 
     Returns:
       The AEAD object...
```

### Comparing `tink-1.6.1/tink/integration/gcpkms/_gcp_kms_client_test.py` & `tink-1.7.0/tink/integration/gcpkms/_gcp_kms_client_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.integration.gcp_kms_client."""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
 
 import os
 
 from absl.testing import absltest
 
 from tink.integration import gcpkms
 from tink.testing import helper
 
 
-CREDENTIAL_PATH = os.path.join(helper.tink_root_path(),
-                               'testdata/credential.json')
+CREDENTIAL_PATH = os.path.join(helper.tink_py_testdata_path(),
+                               'gcp/credential.json')
 
 
 class GcpKmsClientTest(absltest.TestCase):
 
   def test_client_generation(self):
     gcp_client = gcpkms.GcpKmsClient('', CREDENTIAL_PATH)
     self.assertNotEqual(gcp_client, None)
```

### Comparing `tink-1.6.1/tink/integration/gcpkms/BUILD.bazel` & `tink-1.7.0/tink/integration/gcpkms/BUILD.bazel`

 * *Files 15% similar despite different names*

```diff
@@ -12,43 +12,42 @@
         ":_gcp_kms_client",
     ],
 )
 
 py_library(
     name = "_gcp_kms_client",
     srcs = ["_gcp_kms_client.py"],
-    srcs_version =  "PY3",
+    srcs_version = "PY3",
     deps = [
         "//tink/aead",
-        "//tink/core",
         "//tink/cc/pybind:tink_bindings",
-    ]
+        "//tink/core",
+    ],
 )
 
 py_test(
     name = "_gcp_kms_client_test",
     srcs = ["_gcp_kms_client_test.py"],
-    srcs_version =  "PY3",
-    data = [
-        "@tink_base//testdata:credentials"
-    ],
+    data = ["//testdata/gcp:credentials"],
+    srcs_version = "PY3",
     deps = [
         ":gcpkms",
         "//tink/testing:helper",
         requirement("absl-py"),
-    ]
+    ],
 )
 
 py_test(
     name = "_gcp_kms_aead_test",
     srcs = ["_gcp_kms_aead_test.py"],
-    srcs_version =  "PY3",
     data = [
-        "@tink_base//testdata:credentials",
+        "//testdata/gcp:credentials",
         "@google_root_pem//file",
     ],
+    srcs_version = "PY3",
+    tags = ["manual"],
     deps = [
         ":gcpkms",
         "//tink/testing:helper",
         requirement("absl-py"),
-    ]
+    ],
 )
```

### Comparing `tink-1.6.1/tink/integration/gcpkms/__init__.py` & `tink-1.7.0/tink/mac/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright 2019 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Mac package."""
 
-"""GCP KMS package."""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
+from tink.mac import _mac
+from tink.mac import _mac_key_manager
+from tink.mac import _mac_key_templates as mac_key_templates
 
-from tink.integration.gcpkms import _gcp_kms_client
 
-GcpKmsClient = _gcp_kms_client.GcpKmsClient
+Mac = _mac.Mac
+register = _mac_key_manager.register
```

### Comparing `tink-1.6.1/tink/integration/awskms/_aws_kms_client.py` & `tink-1.7.0/tink/integration/awskms/_aws_kms_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A client for AWS KMS."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import re
 
-from typing import Text
 
 from tink import aead
 from tink import core
 from tink.cc.pybind import tink_bindings
 
 
-class AwsKmsClient(object):
+class AwsKmsClient:
   """Basic AWS client for AEAD."""
 
-  def __init__(self, key_uri: Text, credentials_path: Text):
+  def __init__(self, key_uri: str, credentials_path: str):
     """Creates a new AwsKmsClient that is bound to the key specified in 'key_uri'.
 
-    Uses the specifed credentials when communicating with the KMS. Either of
+    Uses the specified credentials when communicating with the KMS. Either of
     arguments can be empty.
 
     If 'key_uri' is empty, then the client is not bound to any particular key.
     If 'credential_path' is empty, then default credentials will be used.
     For more information on credentials and in which order they are loaded see
     https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html.
 
@@ -56,27 +50,27 @@
     elif match:
       self._key_uri = key_uri
     else:
       raise core.TinkError
 
     self.cc_client = tink_bindings.AwsKmsClient(key_uri, credentials_path)
 
-  def does_support(self, key_uri: Text) -> bool:
+  def does_support(self, key_uri: str) -> bool:
     """Returns true iff this client supports KMS key specified in 'key_uri'.
 
     Args:
       key_uri: Text, URI of the key to be checked.
 
     Returns: A boolean value which is true if the key is supported and false
       otherwise.
     """
     return self.cc_client.does_support(key_uri)
 
   @core.use_tink_errors
-  def get_aead(self, key_uri: Text) -> aead.Aead:
+  def get_aead(self, key_uri: str) -> aead.Aead:
     """Returns an Aead-primitive backed by KMS key specified by 'key_uri'.
 
     Args:
       key_uri: Text, URI of the key which should be used.
 
     Returns:
       An AEAD primitive which uses the specified key.
```

### Comparing `tink-1.6.1/tink/integration/awskms/_aws_kms_aead_test.py` & `tink-1.7.0/tink/integration/awskms/_aws_kms_aead_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.integration.aws_kms_aead."""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
 
 import os
 
 from absl.testing import absltest
 
 from tink import core
 from tink.integration import awskms
 from tink.testing import helper
 
-CREDENTIAL_PATH = os.path.join(helper.tink_root_path(),
-                               'testdata/aws_credentials_cc.txt')
-BAD_CREDENTIALS_PATH = os.path.join(helper.tink_root_path(),
-                                    'testdata/bad_aws_credentials_cc.txt')
+CREDENTIAL_PATH = os.path.join(helper.tink_py_testdata_path(),
+                               'aws/credentials.ini')
+BAD_CREDENTIALS_PATH = os.path.join(helper.tink_py_testdata_path(),
+                                    'aws/credentials_bad.ini')
 KEY_URI = 'aws-kms://arn:aws:kms:us-east-2:235739564943:key/3ee50705-5a82-4f5b-9753-05c4f473922f'
 BAD_KEY_URI = 'gcp-kms://projects/tink-test-infrastructure/locations/global/keyRings/unit-and-integration-testing/cryptoKeys/aead-key'
 
 
 class AwsKmsAeadTest(absltest.TestCase):
 
   def test_encrypt_decrypt(self):
```

### Comparing `tink-1.6.1/tink/integration/awskms/__init__.py` & `tink-1.7.0/tink/jwt/_jwt_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-# Copyright 2020 Google LLC
+# Copyright 2021 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Defines an Invalid JWT Error."""
 
-"""StreamingAead package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
+from tink import core
 
-from tink.integration.awskms import _aws_kms_client
 
-AwsKmsClient = _aws_kms_client.AwsKmsClient
+class JwtInvalidError(core.TinkError):
+  pass
```

### Comparing `tink-1.6.1/tink/integration/awskms/_aws_kms_client_test.py` & `tink-1.7.0/tink/integration/awskms/_aws_kms_client_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.integration.aws_kms_client."""
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
 
 import os
 
 from absl.testing import absltest
 
 from tink import core
 from tink.integration import awskms
 from tink.testing import helper
 
-CREDENTIAL_PATH = os.path.join(helper.tink_root_path(),
-                               'testdata/aws_credentials_cc.txt')
+CREDENTIAL_PATH = os.path.join(helper.tink_py_testdata_path(),
+                               'aws/credentials.ini')
 KEY_URI = 'aws-kms://arn:aws:kms:us-east-2:235739564943:key/3ee50705-5a82-4f5b-9753-05c4f473922f'
 BAD_KEY_URI = 'gcp-kms://projects/tink-test-infrastructure/locations/global/keyRings/unit-and-integration-testing/cryptoKeys/aead-key'
 
 
 class AwsKmsClientTest(absltest.TestCase):
 
   def test_client_generation(self):
```

### Comparing `tink-1.6.1/tink/integration/__init__.py` & `tink-1.7.0/tink/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/_keyset_handle.py` & `tink-1.7.0/tink/_keyset_handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,53 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module defines KeysetHandle."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import random
 
 from typing import Type, TypeVar
 
 from google.protobuf import message
 from tink.proto import tink_pb2
 from tink import _keyset_reader
 from tink import _keyset_writer
 from tink import aead
 from tink import core
+from tink import secret_key_access
 
 P = TypeVar('P')
 
 MAX_INT32 = 2147483647  # = 2^31 - 1
 
 
-class KeysetHandle(object):
+class PublicKeyAccess(core.KeyAccess):
+  pass
+
+
+# KeyAccess token that gives access to public keys.
+PUBLIC_KEY_ACCESS_TOKEN = PublicKeyAccess()
+
+
+def has_secret_key_access(token: core.KeyAccess) -> bool:
+  """Returns True if token is secret_key_access.TOKEN, and False otherwise."""
+  return isinstance(token, secret_key_access.SecretKeyAccess)
+
+
+class KeysetHandle:
   """A KeysetHandle provides abstracted access to Keyset.
 
   KeysetHandle limits the exposure of actual protocol buffers that hold
   sensitive key material. This class allows reading and writing encrypted
   keysets.
   """
```

### Comparing `tink-1.6.1/tink/cleartext_keyset_handle_test.py` & `tink-1.7.0/tink/cleartext_keyset_handle_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.cleartext_keyset_handle."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import io
 
 from absl.testing import absltest
 
 import tink
 from tink import cleartext_keyset_handle
 from tink import core
```

### Comparing `tink-1.6.1/tink/aead/_aead_key_manager.py` & `tink-1.7.0/tink/aead/_aead_key_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python wrapper of the wrapped C++ AEAD key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from tink import core
 from tink.aead import _aead
 from tink.aead import _aead_wrapper
 from tink.cc.pybind import tink_bindings
 
 
 class AeadCcToPyWrapper(_aead.Aead):
```

### Comparing `tink-1.6.1/tink/aead/_aead_wrapper.py` & `tink-1.7.0/tink/aead/_aead_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """AEAD wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from typing import Type
 from absl import logging
 
 from tink import core
 from tink.aead import _aead
```

### Comparing `tink-1.6.1/tink/aead/_aead_key_manager_test.py` & `tink-1.7.0/tink/aead/_aead_key_manager_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.aead_key_manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 from tink.proto import aes_ctr_hmac_aead_pb2
 from tink.proto import aes_eax_pb2
 from tink.proto import aes_gcm_pb2
 from tink.proto import aes_gcm_siv_pb2
 from tink.proto import common_pb2
```

### Comparing `tink-1.6.1/tink/aead/_aead_key_templates_test.py` & `tink-1.7.0/tink/aead/_aead_key_templates_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,121 +10,108 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.aead_key_templates."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 from tink.proto import aes_ctr_hmac_aead_pb2
 from tink.proto import aes_eax_pb2
 from tink.proto import aes_gcm_pb2
 from tink.proto import aes_gcm_siv_pb2
 from tink.proto import common_pb2
 from tink.proto import kms_aead_pb2
 from tink.proto import kms_envelope_pb2
 from tink.proto import tink_pb2
 from tink import aead
-from tink.testing import helper
 
 
 class AeadKeyTemplatesTest(parameterized.TestCase):
 
-  @parameterized.parameters([
-      ('AES128_EAX', aead.aead_key_templates.AES128_EAX),
-      ('AES256_EAX', aead.aead_key_templates.AES256_EAX),
-      ('AES128_GCM', aead.aead_key_templates.AES128_GCM),
-      ('AES256_GCM', aead.aead_key_templates.AES256_GCM),
-      ('AES128_GCM_SIV', aead.aead_key_templates.AES128_GCM_SIV),
-      ('AES256_GCM_SIV', aead.aead_key_templates.AES256_GCM_SIV),
-      ('AES128_CTR_HMAC_SHA256',
-       aead.aead_key_templates.AES128_CTR_HMAC_SHA256),
-      ('AES256_CTR_HMAC_SHA256',
-       aead.aead_key_templates.AES256_CTR_HMAC_SHA256),
-      ('XCHACHA20_POLY1305', aead.aead_key_templates.XCHACHA20_POLY1305)
-  ])
-  def test_template(self, template_name, template):
-    self.assertEqual(template,
-                     helper.template_from_testdata(template_name, 'aead'))
+  def test_create_kms_aead_key_template(self):
+    template = aead.aead_key_templates.create_kms_aead_key_template(
+        key_uri='fake://kek/uri')
+    self.assertEqual(template.type_url,
+                     'type.googleapis.com/google.crypto.tink.KmsAeadKey')
+    self.assertEqual(template.output_prefix_type, tink_pb2.RAW)
+    key_format = kms_aead_pb2.KmsAeadKeyFormat.FromString(template.value)
+    self.assertEqual(key_format.key_uri, 'fake://kek/uri')
+
+  def test_create_kms_envelope_aead_key_template(self):
+    template = aead.aead_key_templates.create_kms_envelope_aead_key_template(
+        kek_uri='fake://kek/uri',
+        dek_template=aead.aead_key_templates.AES128_GCM)
+    self.assertEqual(
+        template.type_url,
+        'type.googleapis.com/google.crypto.tink.KmsEnvelopeAeadKey')
+    self.assertEqual(template.output_prefix_type, tink_pb2.RAW)
+    key_format = kms_envelope_pb2.KmsEnvelopeAeadKeyFormat.FromString(
+        template.value)
+    self.assertEqual(key_format.kek_uri, 'fake://kek/uri')
+    self.assertEqual(key_format.dek_template.type_url,
+                     aead.aead_key_templates.AES128_GCM.type_url)
 
   def test_create_aes_eax_key_template(self):
     # Intentionally using 'weird' or invalid values for parameters,
     # to test that the function correctly puts them in the resulting template.
-    template = aead.aead_key_templates.create_aes_eax_key_template(
-        key_size=42, iv_size=72)
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = aead.aead_key_templates.create_aes_eax_key_template(
+          key_size=42, iv_size=72)
     self.assertEqual('type.googleapis.com/google.crypto.tink.AesEaxKey',
                      template.type_url)
     self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
     key_format = aes_eax_pb2.AesEaxKeyFormat.FromString(template.value)
     self.assertEqual(42, key_format.key_size)
     self.assertEqual(72, key_format.params.iv_size)
 
   def test_create_aes_gcm_key_template(self):
     # Intentionally using 'weird' or invalid values for parameters,
     # to test that the function correctly puts them in the resulting template.
-    template = aead.aead_key_templates.create_aes_gcm_key_template(key_size=42)
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = aead.aead_key_templates.create_aes_gcm_key_template(
+          key_size=42)
     self.assertEqual('type.googleapis.com/google.crypto.tink.AesGcmKey',
                      template.type_url)
     self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
     key_format = aes_gcm_pb2.AesGcmKeyFormat.FromString(template.value)
     self.assertEqual(42, key_format.key_size)
 
   def test_create_aes_gcm_siv_key_template(self):
-    template = aead.aead_key_templates.create_aes_gcm_siv_key_template(
-        key_size=42)
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = aead.aead_key_templates.create_aes_gcm_siv_key_template(
+          key_size=42)
     self.assertEqual('type.googleapis.com/google.crypto.tink.AesGcmSivKey',
                      template.type_url)
     self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
     key_format = aes_gcm_siv_pb2.AesGcmSivKeyFormat.FromString(template.value)
     self.assertEqual(42, key_format.key_size)
 
   def test_create_aes_ctr_hmac_aead_key_template(self):
     # Intentionally using 'weird' or invalid values for parameters,
     # to test that the function correctly puts them in the resulting template.
-    template = aead.aead_key_templates.create_aes_ctr_hmac_aead_key_template(
-        aes_key_size=34,
-        iv_size=93,
-        hmac_key_size=46,
-        tag_size=99,
-        hash_type=common_pb2.SHA1)
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = aead.aead_key_templates.create_aes_ctr_hmac_aead_key_template(
+          aes_key_size=34,
+          iv_size=93,
+          hmac_key_size=46,
+          tag_size=99,
+          hash_type=common_pb2.SHA1)
     self.assertEqual('type.googleapis.com/google.crypto.tink.AesCtrHmacAeadKey',
                      template.type_url)
     self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
     key_format = aes_ctr_hmac_aead_pb2.AesCtrHmacAeadKeyFormat.FromString(
         template.value)
     self.assertEqual(93, key_format.aes_ctr_key_format.params.iv_size)
     self.assertEqual(34, key_format.aes_ctr_key_format.key_size)
     self.assertEqual(common_pb2.SHA1, key_format.hmac_key_format.params.hash)
     self.assertEqual(99, key_format.hmac_key_format.params.tag_size)
     self.assertEqual(46, key_format.hmac_key_format.key_size)
 
-  def test_create_kms_aead_key_template(self):
-    template = aead.aead_key_templates.create_kms_aead_key_template(
-        key_uri='fake://kek/uri')
-    self.assertEqual(template.type_url,
-                     'type.googleapis.com/google.crypto.tink.KmsAeadKey')
-    self.assertEqual(template.output_prefix_type, tink_pb2.RAW)
-    key_format = kms_aead_pb2.KmsAeadKeyFormat.FromString(template.value)
-    self.assertEqual(key_format.key_uri, 'fake://kek/uri')
-
-  def test_create_kms_envelope_aead_key_template(self):
-    template = aead.aead_key_templates.create_kms_envelope_aead_key_template(
-        kek_uri='fake://kek/uri',
-        dek_template=aead.aead_key_templates.AES128_GCM)
-    self.assertEqual(
-        template.type_url,
-        'type.googleapis.com/google.crypto.tink.KmsEnvelopeAeadKey')
-    self.assertEqual(template.output_prefix_type, tink_pb2.RAW)
-    key_format = kms_envelope_pb2.KmsEnvelopeAeadKeyFormat.FromString(
-        template.value)
-    self.assertEqual(key_format.kek_uri, 'fake://kek/uri')
-    self.assertEqual(key_format.dek_template.type_url,
-                     aead.aead_key_templates.AES128_GCM.type_url)
-
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/aead/_kms_envelope_aead.py` & `tink-1.7.0/tink/aead/_kms_envelope_aead.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Module for envelope encryption with KMS."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import struct
 
 from tink.proto import tink_pb2
 from tink import core
 from tink.aead import _aead
```

### Comparing `tink-1.6.1/tink/aead/BUILD.bazel` & `tink-1.7.0/tink/aead/BUILD.bazel`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,14 @@
     ],
 )
 
 py_library(
     name = "_aead",
     srcs = ["_aead.py"],
     srcs_version = "PY3",
-    deps = [
-        requirement("six"),
-    ],
 )
 
 py_library(
     name = "_aead_key_manager",
     srcs = ["_aead_key_manager.py"],
     srcs_version = "PY3",
     deps = [
@@ -97,30 +94,26 @@
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_aead_key_templates_test",
     srcs = ["_aead_key_templates_test.py"],
-    data = [
-        "@tink_base//testdata/templates",
-    ],
     srcs_version = "PY3",
     deps = [
         ":aead",
         requirement("absl-py"),
         "//tink/proto:aes_ctr_hmac_aead_py_pb2",
         "//tink/proto:aes_eax_py_pb2",
         "//tink/proto:aes_gcm_py_pb2",
         "//tink/proto:aes_gcm_siv_py_pb2",
         "//tink/proto:common_py_pb2",
         "//tink/proto:kms_aead_py_pb2",
         "//tink/proto:kms_envelope_py_pb2",
         "//tink/proto:tink_py_pb2",
-        "//tink/testing:helper",
     ],
 )
 
 py_library(
     name = "_kms_envelope_aead",
     srcs = ["_kms_envelope_aead.py"],
     srcs_version = "PY3",
```

### Comparing `tink-1.6.1/tink/aead/__init__.py` & `tink-1.7.0/tink/aead/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Aead package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
 from tink.aead import _aead
 from tink.aead import _aead_key_manager
 from tink.aead import _aead_key_templates as aead_key_templates
 from tink.aead import _kms_envelope_aead
```

### Comparing `tink-1.6.1/tink/aead/_aead.py` & `tink-1.7.0/tink/aead/_aead.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,27 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module defines the interface for AEAD."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 
-# Special imports
-import six
-
 
-@six.add_metaclass(abc.ABCMeta)
-class Aead(object):
+class Aead(metaclass=abc.ABCMeta):
   """The interface for authenticated encryption with associated data.
 
   Implementations of this interface are secure against adaptive
   chosen ciphertext attacks.  Encryption with associated data ensures
   authenticity and integrity of that data, but not its secrecy.
   (see RFC 5116, https://tools.ietf.org/html/rfc5116)
   """
```

### Comparing `tink-1.6.1/tink/aead/_kms_envelope_aead_test.py` & `tink-1.7.0/tink/aead/_kms_envelope_aead_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.aead.aead."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import struct
 from absl.testing import absltest
 
 from tink.proto import aes_gcm_pb2
 import tink
 from tink import aead
 from tink import core
```

### Comparing `tink-1.6.1/tink/aead/_aead_wrapper_test.py` & `tink-1.7.0/tink/aead/_aead_wrapper_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.aead_wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 import tink
 from tink import aead
 from tink.testing import keyset_builder
```

### Comparing `tink-1.6.1/tink/_keyset_handle_test.py` & `tink-1.7.0/tink/_keyset_handle_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink._keyset_handle."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 
 from absl.testing import absltest
 from tink.proto import tink_pb2
 import tink
 from tink import aead
 from tink import core
```

### Comparing `tink-1.6.1/tink/cc/cc_tink_config.cc` & `tink-1.7.0/tink/cc/cc_hpke_config.cc`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019 Google LLC.
+// Copyright 2022 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -10,20 +10,22 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/cc/cc_tink_config.h"
+#include "tink/cc/cc_hpke_config.h"
 
-#include "tink/config/tink_config.h"
+#include <memory>
+
+#include "tink/hybrid/hpke_config.h"
 
 namespace crypto {
 namespace tink {
 
-util::Status CcTinkConfigRegister() {
-  return TinkConfig::Register();
+util::Status CcHpkeConfigRegister() {
+  return RegisterHpke();
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/input_stream_adapter.h` & `tink-1.7.0/tink/cc/input_stream_adapter.h`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #ifndef TINK_PYTHON_CC_INPUT_STREAM_ADAPTER_H_
 #define TINK_PYTHON_CC_INPUT_STREAM_ADAPTER_H_
 
 #include <memory>
+#include <string>
+#include <utility>
 
 #include "tink/input_stream.h"
 #include "tink/util/statusor.h"
 
 namespace crypto {
 namespace tink {
```

### Comparing `tink-1.6.1/tink/cc/python_input_stream.cc` & `tink-1.7.0/tink/cc/python_input_stream.cc`

 * *Files 6% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 #include "tink/cc/python_input_stream.h"
 
 #include <algorithm>
 #include <memory>
 #include <string>
 
 #include "absl/memory/memory.h"
+#include "absl/status/status.h"
+#include "absl/strings/match.h"
 #include "tink/input_stream.h"
 #include "tink/subtle/subtle_util.h"
 #include "tink/util/status.h"
 #include "tink/util/statusor.h"
 #include "tink/cc/python_file_object_adapter.h"
 
 namespace crypto {
 namespace tink {
 
 namespace {
 
 bool is_eof(const util::Status& status) {
-  return status.error_code() == util::error::UNKNOWN &&
-         status.error_message().find("EOFError") != std::string::npos;
+  return status.code() == absl::StatusCode::kUnknown &&
+         absl::StrContains(status.message(), "EOFError");
 }
 
 }  // namespace
 
 PythonInputStream::PythonInputStream(
     std::shared_ptr<PythonFileObjectAdapter> adapter, int buffer_size) {
   if (buffer_size <= 0) buffer_size = 128 * 1024;  // 128 KB
@@ -62,24 +64,24 @@
     *data = &buffer_[buffer_offset_];
     return count_in_buffer_;
   }
 
   // Read new bytes to buffer_.
   auto read_result = adapter_->Read(buffer_.size());
   if (is_eof(read_result.status())) {
-    return status_ = util::Status(util::error::OUT_OF_RANGE, "EOF");
-  } else if (read_result.status().error_code() == util::error::OUT_OF_RANGE) {
+    return status_ = util::Status(absl::StatusCode::kOutOfRange, "EOF");
+  } else if (read_result.status().code() == absl::StatusCode::kOutOfRange) {
     // We need to change the error code because for InputStream OUT_OF_RANGE
     // status always means EOF.
-    return status_ = util::Status(util::error::UNKNOWN,
-                                  read_result.status().error_message());
+    return status_ = util::Status(absl::StatusCode::kUnknown,
+                                  read_result.status().message());
   } else if (!read_result.ok()) {
     return status_ = read_result.status();
   }
-  std::string read_string = read_result.ValueOrDie();
+  std::string read_string = read_result.value();
   int count_read = read_string.length();
   buffer_.replace(0, count_read, read_string);
   buffer_offset_ = 0;
   count_backedup_ = 0;
   count_in_buffer_ = count_read;
   position_ += count_in_buffer_;
   *data = &buffer_[0];
```

### Comparing `tink-1.6.1/tink/cc/output_stream_adapter.h` & `tink-1.7.0/tink/cc/output_stream_adapter.h`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #ifndef TINK_PYTHON_CC_OUTPUT_STREAM_ADAPTER_H_
 #define TINK_PYTHON_CC_OUTPUT_STREAM_ADAPTER_H_
 
 #include <memory>
+#include <utility>
 
 #include "absl/strings/string_view.h"
 #include "tink/output_stream.h"
 #include "tink/util/status.h"
 #include "tink/util/statusor.h"
 
 namespace crypto {
```

### Comparing `tink-1.6.1/tink/cc/output_stream_adapter_test.cc` & `tink-1.7.0/tink/cc/output_stream_adapter_test.cc`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/output_stream_adapter.h"
 
 #include <algorithm>
 #include <sstream>
+#include <string>
+#include <utility>
 
 #include "gmock/gmock.h"
 #include "gtest/gtest.h"
 #include "absl/memory/memory.h"
+#include "absl/status/status.h"
 #include "tink/output_stream.h"
 #include "tink/subtle/random.h"
 #include "tink/util/ostream_output_stream.h"
 
 namespace crypto {
 namespace tink {
 namespace {
@@ -41,53 +44,54 @@
 }
 
 TEST(OutputStreamAdapterTest, Basic) {
   std::stringbuf* buffer_ref;
   auto adapter = GetOutputStreamAdapter(-1, &buffer_ref);
   auto write_result = adapter->Write("something");
   ASSERT_TRUE(write_result.status().ok());
-  EXPECT_EQ(write_result.ValueOrDie(), 9);
+  EXPECT_EQ(write_result.value(), 9);
   EXPECT_TRUE(adapter->Close().ok());
   EXPECT_EQ(buffer_ref->str(), "something");
 }
 
 TEST(OutputStreamAdapterTest, MultipleWrite) {
   std::stringbuf* buffer_ref;
   auto adapter = GetOutputStreamAdapter(-1, &buffer_ref);
   auto write_result = adapter->Write("something");
   ASSERT_TRUE(write_result.status().ok());
-  EXPECT_EQ(write_result.ValueOrDie(), 9);
+  EXPECT_EQ(write_result.value(), 9);
   write_result = adapter->Write("123");
   ASSERT_TRUE(write_result.status().ok());
-  EXPECT_EQ(write_result.ValueOrDie(), 3);
+  EXPECT_EQ(write_result.value(), 3);
   write_result = adapter->Write("456");
   ASSERT_TRUE(write_result.status().ok());
-  EXPECT_EQ(write_result.ValueOrDie(), 3);
+  EXPECT_EQ(write_result.value(), 3);
   EXPECT_TRUE(adapter->Close().ok());
   EXPECT_EQ(buffer_ref->str(), "something123456");
 }
 
 TEST(OutputStreamAdapterTest, WriteAfterClose) {
   std::stringbuf* buffer_ref;
   auto adapter = GetOutputStreamAdapter(-1, &buffer_ref);
   ASSERT_TRUE(adapter->Close().ok());
   auto status = adapter->Write("something").status();
-  EXPECT_EQ(status.error_code(), util::error::FAILED_PRECONDITION);
-  EXPECT_THAT(status.error_message(), testing::HasSubstr("Stream closed"));
+  EXPECT_EQ(status.code(), absl::StatusCode::kFailedPrecondition);
+  EXPECT_THAT(std::string(status.message()),
+              testing::HasSubstr("Stream closed"));
 }
 
 // In this test size of the OstreamOutputStream buffer is smaller than the
 // size of data to be written, so multiple calls to Next() will be needed.
 TEST(OutputStreamAdapterTest, MultipleNext) {
   std::stringbuf* buffer_ref;
   auto adapter = GetOutputStreamAdapter(10, &buffer_ref);
   std::string data = subtle::Random::GetRandomBytes(35);
   auto write_result = adapter->Write(data);
   ASSERT_TRUE(write_result.status().ok());
-  EXPECT_EQ(write_result.ValueOrDie(), 35);
+  EXPECT_EQ(write_result.value(), 35);
   EXPECT_TRUE(adapter->Close().ok());
   EXPECT_EQ(buffer_ref->str(), data);
 }
 
 }  // namespace
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/cc_streaming_aead_wrappers_test.cc` & `tink-1.7.0/tink/cc/cc_streaming_aead_wrappers_test.cc`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/cc_streaming_aead_wrappers.h"
 
+#include <utility>
+
 #include "gtest/gtest.h"
 #include "tink/cc/test_util.h"
 
 namespace crypto {
 namespace tink {
 namespace {
```

### Comparing `tink-1.6.1/tink/cc/python_input_stream_test.cc` & `tink-1.7.0/tink/cc/python_input_stream_test.cc`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,21 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/python_input_stream.h"
 
+#include <algorithm>
+#include <string>
+#include <utility>
+
 #include "gtest/gtest.h"
 #include "absl/memory/memory.h"
+#include "absl/status/status.h"
 #include "tink/subtle/random.h"
 #include "tink/cc/test_util.h"
 
 namespace crypto {
 namespace tink {
 namespace {
 
@@ -30,31 +35,30 @@
 // Returns the status of the last input_stream->Next()-operation.
 util::Status ReadTillEnd(PythonInputStream* input_stream,
                          std::string* contents) {
   contents->clear();
   const void* buffer;
   auto next_result = input_stream->Next(&buffer);
   while (next_result.ok()) {
-    contents->append(static_cast<const char*>(buffer),
-                     next_result.ValueOrDie());
+    contents->append(static_cast<const char*>(buffer), next_result.value());
     next_result = input_stream->Next(&buffer);
   }
   return next_result.status();
 }
 
 TEST(PythonInputStreamTest, testReadingStreams) {
   for (int stream_size : {0, 10, 100, 1000, 10000, 100000, 1000000}) {
     std::string contents = subtle::Random::GetRandomBytes(stream_size);
     auto input = absl::make_unique<test::TestReadableObject>(contents);
     EXPECT_EQ(stream_size, contents.size());
     auto input_stream = absl::make_unique<PythonInputStream>(std::move(input));
     std::string stream_contents;
     auto status = ReadTillEnd(input_stream.get(), &stream_contents);
-    EXPECT_EQ(util::error::OUT_OF_RANGE, status.error_code());
-    EXPECT_EQ("EOF", status.error_message());
+    EXPECT_EQ(absl::StatusCode::kOutOfRange, status.code());
+    EXPECT_EQ("EOF", status.message());
     EXPECT_EQ(contents, stream_contents);
   }
 }
 
 TEST(PythonInputStreamTest, testCustomBufferSizes) {
   int stream_size = 100000;
   for (int buffer_size : {1, 10, 100, 1000, 10000}) {
@@ -62,15 +66,15 @@
     auto input = absl::make_unique<test::TestReadableObject>(contents);
     EXPECT_EQ(stream_size, contents.size());
     auto input_stream =
         absl::make_unique<PythonInputStream>(std::move(input), buffer_size);
     const void* buffer;
     auto next_result = input_stream->Next(&buffer);
     EXPECT_TRUE(next_result.ok()) << next_result.status();
-    EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+    EXPECT_EQ(buffer_size, next_result.value());
     EXPECT_EQ(contents.substr(0, buffer_size),
               std::string(static_cast<const char*>(buffer), buffer_size));
   }
 }
 
 TEST(PythonInputStreamTest, testBackupAndPosition) {
   int stream_size = 100000;
@@ -82,30 +86,30 @@
 
   // Prepare the stream and do the first call to Next().
   auto input_stream =
       absl::make_unique<PythonInputStream>(std::move(input), buffer_size);
   EXPECT_EQ(0, input_stream->Position());
   auto next_result = input_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+  EXPECT_EQ(buffer_size, next_result.value());
   EXPECT_EQ(buffer_size, input_stream->Position());
   EXPECT_EQ(contents.substr(0, buffer_size),
             std::string(static_cast<const char*>(buffer), buffer_size));
 
   // BackUp several times, but in total fewer bytes than returned by Next().
   int total_backup_size = 0;
   for (auto backup_size : {0, 1, 5, 0, 10, 100, -42, 400, 20, -100}) {
     input_stream->BackUp(backup_size);
     total_backup_size += std::max(0, backup_size);
     EXPECT_EQ(buffer_size - total_backup_size, input_stream->Position());
   }
   // Call Next(), it should return exactly the backed up bytes.
   next_result = input_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(total_backup_size, next_result.ValueOrDie());
+  EXPECT_EQ(total_backup_size, next_result.value());
   EXPECT_EQ(buffer_size, input_stream->Position());
   EXPECT_EQ(contents.substr(buffer_size - total_backup_size, total_backup_size),
             std::string(static_cast<const char*>(buffer), total_backup_size));
 
   // BackUp() some bytes, again fewer than returned by Next().
   total_backup_size = 0;
   for (int backup_size : {0, 72, -94, 37, 82}) {
@@ -113,23 +117,23 @@
     total_backup_size += std::max(0, backup_size);
     EXPECT_EQ(buffer_size - total_backup_size, input_stream->Position());
   }
 
   // Call Next(), it should return exactly the backed up bytes.
   next_result = input_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(total_backup_size, next_result.ValueOrDie());
+  EXPECT_EQ(total_backup_size, next_result.value());
   EXPECT_EQ(buffer_size, input_stream->Position());
   EXPECT_EQ(contents.substr(buffer_size - total_backup_size, total_backup_size),
             std::string(static_cast<const char*>(buffer), total_backup_size));
 
   // Call Next() again, it should return the second block.
   next_result = input_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+  EXPECT_EQ(buffer_size, next_result.value());
   EXPECT_EQ(2 * buffer_size, input_stream->Position());
   EXPECT_EQ(contents.substr(buffer_size, buffer_size),
             std::string(static_cast<const char*>(buffer), buffer_size));
 
   // BackUp a few times, with total over the returned buffer_size.
   total_backup_size = 0;
   for (int backup_size :
@@ -139,15 +143,15 @@
                                  total_backup_size + std::max(0, backup_size));
     EXPECT_EQ(2 * buffer_size - total_backup_size, input_stream->Position());
   }
 
   // Call Next() again, it should return the second block.
   next_result = input_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+  EXPECT_EQ(buffer_size, next_result.value());
   EXPECT_EQ(2 * buffer_size, input_stream->Position());
   EXPECT_EQ(contents.substr(buffer_size, buffer_size),
             std::string(static_cast<const char*>(buffer), buffer_size));
 }
 
 }  // namespace
 }  // namespace tink
```

### Comparing `tink-1.6.1/tink/cc/python_input_stream.h` & `tink-1.7.0/tink/cc/python_input_stream.h`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #ifndef TINK_PYTHON_CC_PYTHON_INPUT_STREAM_H_
 #define TINK_PYTHON_CC_PYTHON_INPUT_STREAM_H_
 
 #include <memory>
+#include <string>
 
 #include "tink/input_stream.h"
 #include "tink/util/status.h"
 #include "tink/util/statusor.h"
 #include "tink/cc/python_file_object_adapter.h"
 
 namespace crypto {
```

### Comparing `tink-1.6.1/tink/cc/test_util.h` & `tink-1.7.0/tink/cc/test_util.h`

 * *Files 9% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #ifndef TINK_PYTHON_CC_TEST_UTIL_H_
 #define TINK_PYTHON_CC_TEST_UTIL_H_
 
-#include "tink/cc/python_file_object_adapter.h"
-#include "tink/streaming_aead.h"
+#include <algorithm>
+#include <string>
+#include <utility>
+
 #include "absl/base/thread_annotations.h"
+#include "absl/status/status.h"
 #include "absl/strings/str_cat.h"
 #include "absl/synchronization/mutex.h"
-
+#include "tink/streaming_aead.h"
+#include "tink/cc/python_file_object_adapter.h"
 
 namespace crypto {
 namespace tink {
 namespace test {
 
 // Writable PythonFileObjectAdapter for testing.
 class TestWritableObject : public PythonFileObjectAdapter {
@@ -35,15 +39,15 @@
     buffer_ += std::string(data);
     return data.size();
   }
 
   util::Status Close() override { return util::OkStatus(); }
 
   util::StatusOr<std::string> Read(int size) override {
-    return util::Status(util::error::UNIMPLEMENTED, "not readable");
+    return util::Status(absl::StatusCode::kUnimplemented, "not readable");
   }
 
   std::string* GetBuffer() { return &buffer_; }
 
  private:
   std::string buffer_;
 };
@@ -53,22 +57,22 @@
  public:
   explicit TestReadableObject(const std::string& data) {
     buffer_ = data;
     position_ = 0;
   }
 
   util::StatusOr<int> Write(absl::string_view data) override {
-    return util::Status(util::error::UNIMPLEMENTED, "not writable");
+    return util::Status(absl::StatusCode::kUnimplemented, "not writable");
   }
 
   util::Status Close() override { return util::OkStatus(); }
 
   util::StatusOr<std::string> Read(int size) override {
     if (position_ == buffer_.size() && size > 0) {
-      return util::Status(util::error::UNKNOWN, "EOFError");
+      return util::Status(absl::StatusCode::kUnknown, "EOFError");
     }
     int actual = std::min(size, static_cast<int>(buffer_.size() - position_));
     std::string to_return = buffer_.substr(position_, actual);
     position_ += actual;
     return to_return;
   }
 
@@ -86,34 +90,34 @@
  public:
   explicit DummyStreamingAead(absl::string_view streaming_aead_name)
       : streaming_aead_name_(streaming_aead_name) {}
 
   crypto::tink::util::StatusOr<std::unique_ptr<crypto::tink::OutputStream>>
   NewEncryptingStream(
       std::unique_ptr<crypto::tink::OutputStream> ciphertext_destination,
-      absl::string_view associated_data) override {
+      absl::string_view associated_data) const override {
     return {absl::make_unique<DummyEncryptingStream>(
         std::move(ciphertext_destination),
         absl::StrCat(streaming_aead_name_, associated_data))};
   }
 
   crypto::tink::util::StatusOr<std::unique_ptr<crypto::tink::InputStream>>
   NewDecryptingStream(
       std::unique_ptr<crypto::tink::InputStream> ciphertext_source,
-      absl::string_view associated_data) override {
+      absl::string_view associated_data) const override {
     return {absl::make_unique<DummyDecryptingStream>(
         std::move(ciphertext_source),
         absl::StrCat(streaming_aead_name_, associated_data))};
   }
 
   crypto::tink::util::StatusOr<
       std::unique_ptr<crypto::tink::RandomAccessStream>>
   NewDecryptingRandomAccessStream(
       std::unique_ptr<crypto::tink::RandomAccessStream> ciphertext_source,
-      absl::string_view associated_data) override {
+      absl::string_view associated_data) const override {
     return {absl::make_unique<DummyDecryptingRandomAccessStream>(
         std::move(ciphertext_source),
         absl::StrCat(streaming_aead_name_, associated_data))};
   }
 
   // Upon first call to Next() writes to 'ct_dest' the specifed 'header',
   // and subsequently forwards all methods calls to the corresponding
@@ -129,19 +133,20 @@
       if (!after_init_) {  // Try to initialize.
         after_init_ = true;
         auto next_result = ct_dest_->Next(data);
         if (!next_result.ok()) {
           status_ = next_result.status();
           return status_;
         }
-        if (next_result.ValueOrDie() < header_.size()) {
-          status_ = util::Status(util::error::INTERNAL, "Buffer too small");
+        if (next_result.value() < header_.size()) {
+          status_ =
+              util::Status(absl::StatusCode::kInternal, "Buffer too small");
         } else {
           memcpy(*data, header_.data(), static_cast<int>(header_.size()));
-          ct_dest_->BackUp(next_result.ValueOrDie() - header_.size());
+          ct_dest_->BackUp(next_result.value() - header_.size());
         }
       }
       if (!status_.ok()) return status_;
       return ct_dest_->Next(data);
     }
 
     void BackUp(int count) override {
@@ -158,15 +163,15 @@
       }
     }
     util::Status Close() override {
       if (!after_init_) {  // Call Next() to write the header to ct_dest_.
         void *buf;
         auto next_result = Next(&buf);
         if (next_result.ok()) {
-          BackUp(next_result.ValueOrDie());
+          BackUp(next_result.value());
         } else {
           status_ = next_result.status();
           return status_;
         }
       }
       return ct_dest_->Close();
     }
@@ -191,29 +196,30 @@
 
     crypto::tink::util::StatusOr<int> Next(const void** data) override {
       if (!after_init_) {  // Try to initialize.
         after_init_ = true;
         auto next_result = ct_source_->Next(data);
         if (!next_result.ok()) {
           status_ = next_result.status();
-          if (status_.error_code() == util::error::OUT_OF_RANGE) {
-            status_ = util::Status(
-                util::error::INVALID_ARGUMENT, "Could not read header");
+          if (status_.code() == absl::StatusCode::kOutOfRange) {
+            status_ = util::Status(absl::StatusCode::kInvalidArgument,
+                                   "Could not read header");
           }
           return status_;
         }
-        if (next_result.ValueOrDie() < exp_header_.size()) {
-          status_ = util::Status(util::error::INTERNAL, "Buffer too small");
+        if (next_result.value() < exp_header_.size()) {
+          status_ =
+              util::Status(absl::StatusCode::kInternal, "Buffer too small");
         } else if (memcmp((*data), exp_header_.data(),
                           static_cast<int>(exp_header_.size()))) {
-          status_ = util::Status(
-              util::error::INVALID_ARGUMENT, "Corrupted header");
+          status_ = util::Status(absl::StatusCode::kInvalidArgument,
+                                 "Corrupted header");
         }
         if (status_.ok()) {
-          ct_source_->BackUp(next_result.ValueOrDie() - exp_header_.size());
+          ct_source_->BackUp(next_result.value() - exp_header_.size());
         }
       }
       if (!status_.ok()) return status_;
       return ct_source_->Next(data);
     }
 
     void BackUp(int count) override {
@@ -244,57 +250,57 @@
   class DummyDecryptingRandomAccessStream :
       public crypto::tink::RandomAccessStream {
    public:
     DummyDecryptingRandomAccessStream(
         std::unique_ptr<crypto::tink::RandomAccessStream> ct_source,
         absl::string_view expected_header)
         : ct_source_(std::move(ct_source)), exp_header_(expected_header),
-          status_(util::Status(util::error::UNAVAILABLE, "not initialized")) {}
+          status_(util::Status(absl::StatusCode::kUnavailable,
+                               "not initialized")) {}
 
     crypto::tink::util::Status PRead(
         int64_t position, int count,
         crypto::tink::util::Buffer* dest_buffer) override {
       {  // Initialize, if not initialized yet.
         absl::MutexLock lock(&status_mutex_);
-        if (status_.error_code() == util::error::UNAVAILABLE) Initialize();
+        if (status_.code() == absl::StatusCode::kUnavailable) Initialize();
         if (!status_.ok()) return status_;
       }
       auto status = dest_buffer->set_size(0);
       if (!status.ok()) return status;
       return ct_source_->PRead(
           position + exp_header_.size(), count, dest_buffer);
     }
 
     util::StatusOr<int64_t> size() override {
       {  // Initialize, if not initialized yet.
         absl::MutexLock lock(&status_mutex_);
-        if (status_.error_code() == util::error::UNAVAILABLE) Initialize();
+        if (status_.code() == absl::StatusCode::kUnavailable) Initialize();
         if (!status_.ok()) return status_;
       }
       auto ct_size_result = ct_source_->size();
       if (!ct_size_result.ok()) return ct_size_result.status();
-      auto pt_size = ct_size_result.ValueOrDie() - exp_header_.size();
+      auto pt_size = ct_size_result.value() - exp_header_.size();
       if (pt_size >= 0) return pt_size;
-      return util::Status(util::error::UNAVAILABLE, "size not available");
+      return util::Status(absl::StatusCode::kUnavailable, "size not available");
     }
 
    private:
     void Initialize() ABSL_EXCLUSIVE_LOCKS_REQUIRED(status_mutex_) {
-      auto buf = std::move(
-          util::Buffer::New(exp_header_.size()).ValueOrDie());
+      auto buf = std::move(util::Buffer::New(exp_header_.size()).value());
       status_ = ct_source_->PRead(0, exp_header_.size(), buf.get());
       if (!status_.ok() &&
-          status_.error_code() != util::error::OUT_OF_RANGE) return;
+          status_.code() != absl::StatusCode::kOutOfRange) return;
       if (buf->size() < exp_header_.size()) {
-        status_ = util::Status(
-            util::error::INVALID_ARGUMENT, "Could not read header");
+        status_ = util::Status(absl::StatusCode::kInvalidArgument,
+                               "Could not read header");
       } else if (memcmp(buf->get_mem_block(), exp_header_.data(),
                         static_cast<int>(exp_header_.size()))) {
-        status_ = util::Status(
-            util::error::INVALID_ARGUMENT, "Corrupted header");
+        status_ = util::Status(absl::StatusCode::kInvalidArgument,
+                               "Corrupted header");
       }
     }
 
     std::unique_ptr<crypto::tink::RandomAccessStream> ct_source_;
     std::string exp_header_;
     mutable absl::Mutex status_mutex_;
     util::Status status_ ABSL_GUARDED_BY(status_mutex_);
```

### Comparing `tink-1.6.1/tink/cc/python_output_stream.h` & `tink-1.7.0/tink/cc/python_output_stream.h`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #ifndef TINK_PYTHON_CC_PYTHON_OUTPUT_STREAM_H_
 #define TINK_PYTHON_CC_PYTHON_OUTPUT_STREAM_H_
 
 #include <memory>
+#include <string>
 
 #include "tink/output_stream.h"
 #include "tink/util/status.h"
 #include "tink/util/statusor.h"
 #include "tink/cc/python_file_object_adapter.h"
 
 namespace crypto {
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_tink_config.cc` & `tink-1.7.0/tink/cc/pybind/cc_tink_config.cc`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/cc/cc_tink_config.h"
+#include "tink/cc/pybind/cc_tink_config.h"
 
-#include "tink/cc/pybind/status_casters.h"
+#include "pybind11/pybind11.h"
+#include "tink/cc/cc_tink_config.h"
 
 namespace crypto {
 namespace tink {
 
 void PybindRegisterCcTinkConfig(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_tink_config_test.py` & `tink-1.7.0/tink/cc/pybind/cc_tink_config_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.cc.pybind.cc_tink_config."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from tink.cc.pybind import tink_bindings
 
 
 class CcTinkConfigTest(absltest.TestCase):
 
   def test_register(self):
```

### Comparing `tink-1.6.1/tink/cc/pybind/input_stream_adapter.h` & `tink-1.7.0/tink/cc/pybind/input_stream_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/cc_gcp_kms_client.cc` & `tink-1.7.0/tink/cc/pybind/cc_gcp_kms_client.cc`

 * *Files 16% similar despite different names*

```diff
@@ -10,57 +10,70 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
+#include "tink/cc/pybind/cc_gcp_kms_client.h"
+
 #include "pybind11/pybind11.h"
 #include "tink/integration/gcpkms/gcp_kms_client.h"
 #include "tink/kms_clients.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 namespace integration {
 namespace gcpkms {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterCcGcpKmsClient(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   py::class_<GcpKmsClient>(m, "GcpKmsClient", "Wrapper for C++ GcpKMS.")
       .def(py::init(
           [](const std::string& key_uri, const std::string& credentials_path) {
             auto client_result = GcpKmsClient::New(key_uri, credentials_path);
             if (!client_result.ok()) {
               throw pybind11::value_error("Could not create client.");
             }
 
-            return std::move(client_result.ValueOrDie());
+            return std::move(client_result.value());
           }))
       .def(
           "does_support",
           [](const GcpKmsClient& self, const std::string& key_uri) -> bool {
             return self.DoesSupport(key_uri);
           },
           py::arg("key_uri"), "URI of the key to be checked.")
       .def(
           "get_aead",
-          [](const GcpKmsClient& self, const std::string& key_uri)
-              -> util::StatusOr<std::unique_ptr<Aead>> {
-            return self.GetAead(key_uri);
+          [](const GcpKmsClient& self,
+             const std::string& key_uri) -> std::unique_ptr<Aead> {
+            crypto::tink::util::StatusOr<std::unique_ptr<Aead>> aead_result =
+                self.GetAead(key_uri);
+            if (!aead_result.ok()) {
+              throw TinkException(aead_result.status());
+            }
+            return *std::move(aead_result);
           },
           py::arg("key_uri"), "URI of the key which should be used.")
       .def_static(
           "register_client",
           [](const std::string& key_uri,
-             const std::string& credentials_path) -> util::Status {
-            return GcpKmsClient::RegisterNewClient(key_uri, credentials_path);
+             const std::string& credentials_path) -> void {
+            crypto::tink::util::Status result =
+                GcpKmsClient::RegisterNewClient(key_uri, credentials_path);
+            if (!result.ok()) {
+              throw TinkException(result);
+            }
           },
           py::arg("key_uri"), "URI of the key which should be used.",
           py::arg("credentials_path"),
           "Path to the credentials for the client.");
 }
 
 }  // namespace gcpkms
```

### Comparing `tink-1.6.1/tink/cc/pybind/status_injector.h` & `tink-1.7.0/tink/cc/pybind/aead.h`

 * *Files 10% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
-
-#ifndef TINK_PYTHON_TINK_CC_PYBIND_STATUS_EXAMPLE_H_
-#define TINK_PYTHON_TINK_CC_PYBIND_STATUS_EXAMPLE_H_
+#ifndef TINK_PYTHON_TINK_CC_PYBIND_AEAD_H_
+#define TINK_PYTHON_TINK_CC_PYBIND_AEAD_H_
 
 #include "pybind11/pybind11.h"
 
-namespace pybind11 {
-namespace test {
+namespace crypto {
+namespace tink {
 
-void PybindRegisterStatusInjector(pybind11::module* m);
+void PybindRegisterAead(pybind11::module* module);
 
-}  // namespace test
-}  // namespace pybind11
+}  // namespace tink
+}  // namespace crypto
 
-#endif  // TINK_PYTHON_TINK_CC_PYBIND_STATUS_EXAMPLE_H_
+#endif  // TINK_PYTHON_TINK_CC_PYBIND_AEAD_H_
```

### Comparing `tink-1.6.1/tink/cc/pybind/mac.cc` & `tink-1.7.0/tink/cc/pybind/mac.cc`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,30 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/mac.h"
+#include "tink/cc/pybind/mac.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/mac.h"
 #include "tink/util/status.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using crypto::tink::util::StatusOr;
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterMac(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<Mac>(
@@ -34,28 +41,34 @@
       "Interface for MACs (Message Authentication Codes). "
       "This interface should be used for authentication only, and not for "
       "other purposes (e.g., it should not be used to generate pseudorandom "
       "bytes).")
 
       .def(
           "compute_mac",
-          [](const Mac& self,
-             const py::bytes& data) -> util::StatusOr<py::bytes> {
+          [](const Mac& self, const py::bytes& data) -> py::bytes {
             // TODO(b/145925674)
-            return self.ComputeMac(std::string(data));
+            StatusOr<std::string> result = self.ComputeMac(std::string(data));
+            if (!result.ok()) {
+              throw TinkException(result.status());
+            }
+            return *std::move(result);
           },
           py::arg("data"),
           "Computes and returns the message authentication code (MAC) for "
           "'data'.")
       .def(
           "verify_mac",
           [](const Mac& self, const py::bytes& mac,
-             const py::bytes& data) -> util::Status {
-            // TODO(b/145925674)
-            return self.VerifyMac(std::string(mac), std::string(data));
+             const py::bytes& data) -> void {
+            util::Status result =
+                self.VerifyMac(std::string(mac), std::string(data));
+            if (!result.ok()) {
+              throw TinkException(result);
+            }
           },
           py::arg("mac"), py::arg("data"),
           "Verifies if 'mac' is a correct authentication code (MAC) for "
           "'data'. "
           "Raises a StatusNotOk exception if the verification fails.");
 }
```

### Comparing `tink-1.6.1/tink/cc/pybind/import_helper.cc` & `tink-1.7.0/tink/cc/pybind/import_helper.cc`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/cc_fake_kms_client_testonly.cc` & `tink-1.7.0/tink/cc/pybind/cc_fake_kms_client_testonly.cc`

 * *Files 16% similar despite different names*

```diff
@@ -10,31 +10,42 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
+#include "tink/cc/pybind/cc_fake_kms_client_testonly.h"
+
+#include <string>
+#include <utility>
+
 #include "pybind11/pybind11.h"
 #include "tink/util/fake_kms_client.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 namespace test {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterCcFakeKmsClientTestonly(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
   m.def(
       "register_fake_kms_client_testonly",
       [](const std::string& key_uri,
-         const std::string& credentials_path) -> util::Status {
-        return FakeKmsClient::RegisterNewClient(key_uri, credentials_path);
+         const std::string& credentials_path) -> void {
+        crypto::tink::util::Status result =
+            FakeKmsClient::RegisterNewClient(key_uri, credentials_path);
+        if (!result.ok()) {
+          throw TinkException(result);
+        }
       },
       py::arg("key_uri"), "URI of the key which should be used.",
       py::arg("credentials_path"), "Path to the credentials for the client.");
 }
 
 }  // namespace test
 }  // namespace tink
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_aws_kms_client.h` & `tink-1.7.0/tink/cc/pybind/cc_aws_kms_client.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/tink_bindings.cc` & `tink-1.7.0/tink/cc/pybind/tink_bindings.cc`

 * *Files 8% similar despite different names*

```diff
@@ -17,55 +17,57 @@
 #include "pybind11/pybind11.h"
 #include "tink/aead.h"
 #include "tink/util/statusor.h"
 #include "tink/cc/pybind/aead.h"
 #include "tink/cc/pybind/cc_aws_kms_client.h"
 #include "tink/cc/pybind/cc_gcp_kms_client.h"
 #include "tink/cc/pybind/cc_fake_kms_client_testonly.h"
+#include "tink/cc/pybind/cc_hpke_config.h"
 #include "tink/cc/pybind/cc_jwt_config.h"
 #include "tink/cc/pybind/cc_key_manager.h"
 #include "tink/cc/pybind/cc_streaming_aead_wrappers.h"
 #include "tink/cc/pybind/cc_tink_config.h"
 #include "tink/cc/pybind/deterministic_aead.h"
 #include "tink/cc/pybind/hybrid_decrypt.h"
 #include "tink/cc/pybind/hybrid_encrypt.h"
 #include "tink/cc/pybind/input_stream_adapter.h"
 #include "tink/cc/pybind/mac.h"
 #include "tink/cc/pybind/output_stream_adapter.h"
 #include "tink/cc/pybind/prf.h"
 #include "tink/cc/pybind/public_key_sign.h"
 #include "tink/cc/pybind/public_key_verify.h"
 #include "tink/cc/pybind/python_file_object_adapter.h"
-#include "tink/cc/pybind/status.h"
-#include "tink/cc/pybind/status_casters.h"
 #include "tink/cc/pybind/streaming_aead.h"
-#include "tink/cc/pybind/status_injector.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
 PYBIND11_MODULE(tink_bindings, m) {
   integration::awskms::PybindRegisterCcAwsKmsClient(&m);
   integration::gcpkms::PybindRegisterCcGcpKmsClient(&m);
+  namespace py = pybind11;
+
+  py::register_exception<pybind11::google_tink::TinkException>(
+      m, "PythonTinkException");
   PybindRegisterCcStreamingAeadWrappers(&m);
   PybindRegisterAead(&m);
   PybindRegisterHybridEncrypt(&m);
   PybindRegisterCcTinkConfig(&m);
+  PybindRegisterCcHpkeConfig(&m);
   PybindRegisterCcJwtConfig(&m);
   PybindRegisterStreamingAead(&m);
   PybindRegisterDeterministicAead(&m);
   PybindRegisterPublicKeySign(&m);
   PybindRegisterMac(&m);
   test::PybindRegisterCcFakeKmsClientTestonly(&m);
   PybindRegisterPrf(&m);
-  pybind11::google_tink::PybindRegisterStatus(&m);
   PybindRegisterHybridDecrypt(&m);
   PybindRegisterOutputStreamAdapter(&m);
   PybindRegisterCcKeyManager(&m);
   PybindRegisterPythonFileObjectAdapter(&m);
   PybindRegisterInputStreamAdapter(&m);
   PybindRegisterPublicKeyVerify(&m);
-  pybind11::test::PybindRegisterStatusInjector(&m);
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/hybrid_decrypt.cc` & `tink-1.7.0/tink/cc/pybind/hybrid_decrypt.cc`

 * *Files 20% similar despite different names*

```diff
@@ -10,36 +10,46 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/hybrid_decrypt.h"
+#include "tink/cc/pybind/hybrid_decrypt.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/hybrid_decrypt.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterHybridDecrypt(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<HybridDecrypt>(m, "HybridDecrypt")
       .def(
           "decrypt",
           [](const HybridDecrypt& self, const py::bytes& ciphertext,
-             const py::bytes& context_info) -> util::StatusOr<py::bytes> {
+             const py::bytes& context_info) -> py::bytes {
             // TODO(b/145925674)
-            return self.Decrypt(std::string(ciphertext),
-                                std::string(context_info));
+            util::StatusOr<std::string> decrypt_result = self.Decrypt(
+                std::string(ciphertext), std::string(context_info));
+            if (!decrypt_result.ok()) {
+              throw TinkException(decrypt_result.status());
+            }
+            return *std::move(decrypt_result);
           },
           py::arg("ciphertext"), py::arg("context_info"));
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/output_stream_adapter.h` & `tink-1.7.0/tink/cc/pybind/output_stream_adapter.h`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 #ifndef TINK_PYTHON_TINK_CC_PYBIND_OUTPUT_STREAM_ADAPTER_H_
 #define TINK_PYTHON_TINK_CC_PYBIND_OUTPUT_STREAM_ADAPTER_H_
 
+#include "pybind11/pybind11.h"
+
 namespace crypto {
 namespace tink {
 
 void PybindRegisterOutputStreamAdapter(pybind11::module* m);
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_fake_kms_client_testonly.h` & `tink-1.7.0/tink/cc/pybind/cc_fake_kms_client_testonly.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/public_key_sign.cc` & `tink-1.7.0/tink/cc/pybind/public_key_sign.cc`

 * *Files 13% similar despite different names*

```diff
@@ -10,23 +10,29 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/public_key_sign.h"
+#include "tink/cc/pybind/public_key_sign.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/public_key_sign.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterPublicKeySign(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<PublicKeySign>(
       m, "PublicKeySign",
@@ -38,16 +44,20 @@
       "these interfaces are secure against adaptive chosen-message attacks. "
       "Signing data ensures the authenticity and the integrity of that data, "
       "but not its secrecy.")
 
       .def(
           "sign",
           [](const PublicKeySign& self,
-             const py::bytes& data) -> util::StatusOr<py::bytes> {
+             const py::bytes& data) -> py::bytes {
             // TODO(b/145925674)
-            return self.Sign(std::string(data));
+            util::StatusOr<std::string> result = self.Sign(std::string(data));
+            if (!result.ok()) {
+              throw TinkException(result.status());
+            }
+            return *std::move(result);
           },
           py::arg("data"), "Computes the signature for 'data'.");
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/python_file_object_adapter.cc` & `tink-1.7.0/tink/cc/pybind/python_file_object_adapter.cc`

 * *Files 26% similar despite different names*

```diff
@@ -10,110 +10,121 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/cc/python_file_object_adapter.h"
+#include "tink/cc/pybind/python_file_object_adapter.h"
+
+#include <string>
 
+#include "absl/status/status.h"
 #include "pybind11/pybind11.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/python_file_object_adapter.h"
 
 namespace crypto {
 namespace tink {
 
-// Defining PYBIND11_OVERLOAD macros here for now.
-// TODO(b/146426040): Use future macros for OSS absl::Status, StatusOr
-//                    when they become available.
-
-// Macro to populate pybind11 trampoline class virtual methods with a
-// util::Status return type. Converts all exceptions derived from
-// std::exception to a StatusNotOk return. std::abort is called for
-// all other exceptions, to ensure exceptions don't unwind through code
-// compiled with -fno-exceptions (or similar, depending on the platform).
-// Modeled after PYBIND11_OVERLOAD_INT defined in pybind11/pybind11.h.
-#define PYBIND11_OVERLOAD_PURE_STATUS_RETURN(cname, name, ...)            \
-  try {                                                                   \
-    pybind11::gil_scoped_acquire gil;                                     \
-    pybind11::function overload =                                         \
-        pybind11::get_overload(static_cast<const cname *>(this), name);   \
-    if (!overload) {                                                      \
-      return util::Status(util::error::UNIMPLEMENTED,                     \
-                          "No Python overload is defined for " name "."); \
-    }                                                                     \
-    overload(__VA_ARGS__); /* Ignoring return value. */                   \
-    return util::Status();                                                \
-  } catch (const std::exception &e) {                                     \
-    return util::Status(util::error::UNKNOWN, e.what());                  \
-  } catch (...) {                                                         \
-    std::abort();                                                         \
-  }
-
-// Macro to populate pybind11 trampoline class virtual methods with a
-// util::StatusOr return type. Converts all exceptions as described for
-// PYBIND11_OVERLOAD_PURE_STATUS_RETURN.
-#define PYBIND11_OVERLOAD_PURE_STATUSOR_RETURN(statusor_payload_type, cname, \
-                                               name, ...)                    \
-  try {                                                                      \
-    pybind11::gil_scoped_acquire gil;                                        \
-    pybind11::function overload =                                            \
-        pybind11::get_overload(static_cast<const cname *>(this), name);      \
-    if (!overload) {                                                         \
-      return util::Status(util::error::UNIMPLEMENTED,                        \
-                          "No Python overload is defined for " name ".");    \
-    }                                                                        \
-    auto o = overload(__VA_ARGS__);                                          \
-    return o.cast<statusor_payload_type>();                                  \
-  } catch (const std::exception &e) {                                        \
-    return util::Status(util::error::UNKNOWN, e.what());                     \
-  } catch (...) {                                                            \
-    std::abort();                                                            \
-  }
-
 class Pybind11PythonFileObjectAdapter : public PythonFileObjectAdapter {
  public:
   // Inherit the constructors.
   using PythonFileObjectAdapter::PythonFileObjectAdapter;
 
-  // Trampoline for each virtual member function:
+  // Trampoline for each virtual member function.
 
-  util::StatusOr<int> Write(absl::string_view data) override{
-      PYBIND11_OVERLOAD_PURE_STATUSOR_RETURN(
-          int, PythonFileObjectAdapter, "write",
-          pybind11::bytes(std::string(data)))}
+  // The implementations are modeled after PYBIND11_OVERLOAD_INT
+  // defined in pybind11/pybind11.h, and convert all exceptions derived from
+  // std::exception to a StatusNotOk return. std::abort is called for all other
+  // exceptions, to ensure exceptions don't unwind through code compiled with
+  // -fno-exceptions (or similar, depending on the platform).
+
+  util::StatusOr<int> Write(absl::string_view data) override {
+    try {
+      pybind11::gil_scoped_acquire gil;
+      pybind11::function overload = pybind11::get_overload(
+          static_cast<const PythonFileObjectAdapter *>(this), "write");
+      if (!overload) {
+        return util::Status(absl::StatusCode::kUnimplemented,
+                            "No Python overload is defined for write.");
+      }
+      auto o = overload(pybind11::bytes(std::string(data)));
+      return o.cast<int>();
+    } catch (const std::exception &e) {
+      return util::Status(absl::StatusCode::kUnknown, e.what());
+    } catch (...) {
+      std::abort();
+    }
+  }
 
-  util::Status Close() override{
-      PYBIND11_OVERLOAD_PURE_STATUS_RETURN(PythonFileObjectAdapter, "close")}
+  util::Status Close() override {
+    try {
+      pybind11::gil_scoped_acquire gil;
+      pybind11::function overload = pybind11::get_overload(
+          static_cast<const PythonFileObjectAdapter *>(this), "close");
+      if (!overload) {
+        return util::Status(absl::StatusCode::kUnimplemented,
+                            "No Python overload is defined for close.");
+      }
+      overload(); /* Ignoring return value. */
+      return util::Status();
+    } catch (const std::exception &e) {
+      return util::Status(absl::StatusCode::kUnknown, e.what());
+    } catch (...) {
+      std::abort();
+    }
+  }
 
   util::StatusOr<std::string> Read(int size) override {
-    PYBIND11_OVERLOAD_PURE_STATUSOR_RETURN(std::string, PythonFileObjectAdapter,
-                                           "read", size)
+    try {
+      pybind11::gil_scoped_acquire gil;
+      pybind11::function overload = pybind11::get_overload(
+          static_cast<const PythonFileObjectAdapter *>(this), "read");
+      if (!overload) {
+        return util::Status(absl::StatusCode::kUnimplemented,
+                            "No Python overload is defined for read.");
+      }
+      auto o = overload(size);
+      return o.cast<std::string>();
+    } catch (const std::exception &e) {
+      return util::Status(absl::StatusCode::kUnknown, e.what());
+    } catch (...) {
+      std::abort();
+    }
   }
 };
 
-void PybindRegisterPythonFileObjectAdapter(pybind11::module* module) {
+void PybindRegisterPythonFileObjectAdapter(pybind11::module *module) {
   namespace py = pybind11;
-  py::module& m = *module;
+  py::module &m = *module;
 
-  // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<PythonFileObjectAdapter, Pybind11PythonFileObjectAdapter,
              std::shared_ptr<PythonFileObjectAdapter>>(
       m, "PythonFileObjectAdapter")
       .def(py::init<>())
       .def(
           "write",
-          [](PythonFileObjectAdapter *self,
-             const py::bytes &data) -> util::StatusOr<int> {
-            return self->Write(std::string(data));  // TODO(b/145925674)
+          [](PythonFileObjectAdapter *self, const py::bytes &data) -> int {
+            /**
+             * This and the following methods are purely virtual, and should
+             * never be called. We use std::abort to decouple Python bindings
+             * from the C++ interface's usage of Status{,Or}, while still
+             * marking the method non-callable.
+             *
+             * For the explanation of why we need a helper `trampoline` class
+             * and the details of its implementation, please see the docs:
+             * https://pybind11.readthedocs.io/en/stable/advanced/classes.html#extended-trampoline-class-functionality
+             */
+            std::abort();
           },
           py::arg("data"))
-      .def("close", &PythonFileObjectAdapter::Close)
+      .def("close", [](PythonFileObjectAdapter *self) -> void { std::abort(); })
       .def(
           "read",
-          [](PythonFileObjectAdapter *self, int size)
-              -> util::StatusOr<py::bytes> { return self->Read(size); },
+          [](PythonFileObjectAdapter *self, int size) -> py::bytes {
+            std::abort();
+          },
           py::arg("size"));
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/streaming_aead.cc` & `tink-1.7.0/tink/cc/pybind/streaming_aead.cc`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/streaming_aead.h"
+#include "tink/cc/pybind/streaming_aead.h"
 
 #include "pybind11/pybind11.h"
+#include "tink/streaming_aead.h"
 
 namespace crypto {
 namespace tink {
 
 void PybindRegisterStreamingAead(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
```

### Comparing `tink-1.6.1/tink/cc/pybind/hybrid_encrypt.h` & `tink-1.7.0/tink/cc/pybind/hybrid_encrypt.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/aead.cc` & `tink-1.7.0/tink/cc/pybind/aead.cc`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,29 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/aead.h"
+#include "tink/cc/pybind/aead.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/aead.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterAead(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<Aead>(
       m, "Aead",
@@ -34,32 +40,39 @@
       "Implementations of this interface are secure against adaptive "
       "chosen ciphertext attacks.  Encryption with associated data ensures "
       "authenticity and integrity of that data, but not its secrecy. "
       "(see RFC 5116, https://tools.ietf.org/html/rfc5116)")
 
       .def(
           "encrypt",
-          [](const Aead& self, const py::bytes& plaintext,
-             const py::bytes& associated_data) -> util::StatusOr<py::bytes> {
-            // TODO(b/145925674)
-            return self.Encrypt(std::string(plaintext),
-                                std::string(associated_data));
+          [](const Aead &self, const py::bytes &plaintext,
+             const py::bytes &associated_data) -> py::bytes {
+            util::StatusOr<std::string> result = self.Encrypt(
+                std::string(plaintext), std::string(associated_data));
+            if (!result.ok()) {
+              throw TinkException(result.status());
+            }
+            return *std::move(result);
           },
           py::arg("plaintext"), py::arg("associated_data"),
           "Encrypts 'plaintext' with 'associated_data' as associated data, "
           "and returns the resulting ciphertext. "
           "The ciphertext allows for checking authenticity and integrity "
           "of the associated data, but does not guarantee its secrecy.")
       .def(
           "decrypt",
-          [](const Aead& self, const py::bytes& ciphertext,
-             const py::bytes& associated_data) -> util::StatusOr<py::bytes> {
+          [](const Aead &self, const py::bytes &ciphertext,
+             const py::bytes &associated_data) -> py::bytes {
             // TODO(b/145925674)
-            return self.Decrypt(std::string(ciphertext),
-                                std::string(associated_data));
+            util::StatusOr<std::string> result = self.Decrypt(
+                std::string(ciphertext), std::string(associated_data));
+            if (!result.ok()) {
+              throw TinkException(result.status());
+            }
+            return *std::move(result);
           },
           py::arg("ciphertext"), py::arg("associated_data"),
           "Decrypts 'ciphertext' with 'associated_data' as associated data, "
           "and returns the resulting plaintext. "
           "The decryption verifies the authenticity and integrity "
           "of the associated data, but there are no guarantees wrt. secrecy "
           "of that data.");
```

### Comparing `tink-1.6.1/tink/cc/pybind/status.h` & `tink-1.7.0/tink/cc/pybind/public_key_sign.h`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
-#ifndef TINK_PYTHON_TINK_CC_PYBIND_STATUS_H_
-#define TINK_PYTHON_TINK_CC_PYBIND_STATUS_H_
+#ifndef TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_SIGN_H_
+#define TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_SIGN_H_
 
-namespace pybind11 {
-namespace google_tink {
+#include "pybind11/pybind11.h"
 
-void PybindRegisterStatus(pybind11::module* m);
+namespace crypto {
+namespace tink {
 
-}  // namespace google_tink
-}  // namespace pybind11
+void PybindRegisterPublicKeySign(pybind11::module* m);
 
-#endif  // TINK_PYTHON_TINK_CC_PYBIND_STATUS_H_
+}  // namespace tink
+}  // namespace crypto
+
+#endif  // TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_SIGN_H_
```

### Comparing `tink-1.6.1/tink/cc/pybind/streaming_aead.h` & `tink-1.7.0/tink/cc/pybind/streaming_aead.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/output_stream_adapter.cc` & `tink-1.7.0/tink/cc/pybind/public_key_verify.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-// Copyright 2019 Google Inc.
+// Copyright 2020 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
-
-#include "tink/cc/output_stream_adapter.h"
-
+#ifndef TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_VERIFY_H_
+#define TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_VERIFY_H_
 #include "pybind11/pybind11.h"
-#include "tink/cc/pybind/status_casters.h"
 
 namespace crypto {
 namespace tink {
 
-void PybindRegisterOutputStreamAdapter(pybind11::module* module) {
-  namespace py = pybind11;
-  py::module& m = *module;
-
-  // TODO(b/146492561): Reduce the number of complicated lambdas.
-  py::class_<OutputStreamAdapter>(m, "OutputStreamAdapter")
-      .def(
-          "write",
-          [](OutputStreamAdapter* self,
-             const py::bytes& data) -> util::StatusOr<int64_t> {
-            return self->Write(std::string(data));
-          },
-          py::arg("data"))
-      .def("close", &OutputStreamAdapter::Close);
-}
+void PybindRegisterPublicKeyVerify(pybind11::module* m);
 
 }  // namespace tink
 }  // namespace crypto
+
+#endif  // TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_VERIFY_H_
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_jwt_config.cc` & `tink-1.7.0/tink/cc/cc_tink_config.cc`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019 Google Inc.
+// Copyright 2019 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -10,22 +10,27 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/cc/cc_jwt_config.h"
+#include "tink/cc/cc_tink_config.h"
 
-#include "tink/cc/pybind/status_casters.h"
+#include <utility>
+
+#include "tink/config/tink_config.h"
+#include "tink/util/status.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
-void PybindRegisterCcJwtConfig(pybind11::module* module) {
-  namespace py = pybind11;
-  py::module& m = *module;
-  m.def("register_jwt", CcJwtConfigRegister);
+void CcTinkConfigRegister() {
+  util::Status result = TinkConfig::Register();
+  if (!result.ok()) {
+    throw pybind11::google_tink::TinkException(result);
+  }
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/BUILD.bazel` & `tink-1.7.0/tink/cc/pybind/BUILD.bazel`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 tink_pybind_library(
     name = "cc_key_manager",
     srcs = ["cc_key_manager.cc"],
     hdrs = ["cc_key_manager.h"],
     deps = [
         ":import_helper",
-        ":status_casters",
         "//tink/cc:cc_key_manager",
         "@pybind11",
         "@tink_cc//:aead",
         "@tink_cc//:deterministic_aead",
         "@tink_cc//:hybrid_decrypt",
         "@tink_cc//:hybrid_encrypt",
         "@tink_cc//:mac",
@@ -50,173 +49,126 @@
         "//tink/proto:aes_eax_py_pb2",
         "//tink/proto:aes_siv_py_pb2",
         "//tink/proto:common_py_pb2",
         "//tink/proto:ecdsa_py_pb2",
         "//tink/proto:ecies_aead_hkdf_py_pb2",
         "//tink/proto:hmac_prf_py_pb2",
         "//tink/proto:hmac_py_pb2",
+        "//tink/proto:hpke_py_pb2",
         "//tink/proto:jwt_ecdsa_py_pb2",
         "//tink/proto:jwt_hmac_py_pb2",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 tink_pybind_library(
     name = "cc_tink_config",
     srcs = ["cc_tink_config.cc"],
     hdrs = ["cc_tink_config.h"],
     deps = [
-        ":status_casters",
         "//tink/cc:cc_tink_config",
         "@pybind11",
     ],
 )
 
 tink_pybind_library(
     name = "cc_jwt_config",
     srcs = ["cc_jwt_config.cc"],
     hdrs = ["cc_jwt_config.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "//tink/cc:cc_jwt_config",
         "@pybind11",
     ],
 )
 
+tink_pybind_library(
+    name = "cc_hpke_config",
+    srcs = ["cc_hpke_config.cc"],
+    hdrs = ["cc_hpke_config.h"],
+    deps = [
+        ":tink_exception",
+        "//tink/cc:cc_hpke_config",
+        "@pybind11",
+    ],
+)
+
 py_test(
     name = "cc_tink_config_test",
     srcs = ["cc_tink_config_test.py"],
     deps = [
         ":tink_bindings",
         requirement("absl-py"),
-        requirement("six"),
     ],
 )
 
 tink_pybind_library(
     name = "python_file_object_adapter",
     srcs = ["python_file_object_adapter.cc"],
     hdrs = ["python_file_object_adapter.h"],
     deps = [
-        ":status_casters",
         "//tink/cc:python_file_object_adapter",
         "@pybind11",
     ],
 )
 
 tink_pybind_library(
     name = "output_stream_adapter",
     srcs = ["output_stream_adapter.cc"],
     hdrs = ["output_stream_adapter.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "//tink/cc:output_stream_adapter",
         "@pybind11",
     ],
 )
 
 tink_pybind_library(
     name = "cc_streaming_aead_wrappers",
     srcs = ["cc_streaming_aead_wrappers.cc"],
     hdrs = ["cc_streaming_aead_wrappers.h"],
     deps = [
         ":import_helper",
-        ":status_casters",
+        ":tink_exception",
         "//tink/cc:cc_streaming_aead_wrappers",
         "@pybind11",
     ],
 )
 
 tink_pybind_library(
     name = "input_stream_adapter",
     srcs = ["input_stream_adapter.cc"],
     hdrs = ["input_stream_adapter.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "//tink/cc:input_stream_adapter",
         "@pybind11",
     ],
 )
 
 # Pybind11 Status, StatusOr casters and extension.
 
 tink_pybind_library(
-    name = "status_utils",
-    srcs = ["status_utils.cc"],
-    hdrs = ["status_utils.h"],
-    visibility = ["//visibility:private"],
-    deps = [
-        ":import_helper",
-        "@pybind11",
-        "@tink_cc//util:status",
-        "@tink_cc//util:statusor",
-    ],
-)
-
-tink_pybind_library(
-    name = "status_casters",
-    hdrs = ["status_casters.h"],
-    deps = [
-        ":status_utils",
-        "@pybind11",
-        "@tink_cc//util:status",
-        "@tink_cc//util:statusor",
-    ],
-)
-
-tink_pybind_library(
-    name = "status",
-    srcs = ["status.cc"],
-    hdrs = ["status.h"],
-    deps = [
-        ":status_utils",
-        "@pybind11",
-        "@tink_cc//util:status",
-    ],
-)
-
-tink_pybind_library(
-    name = "status_injector",
-    srcs = ["status_injector.cc"],
-    hdrs = ["status_injector.h"],
-    deps = [
-        ":status_casters",
-        "@pybind11",
-        "@tink_cc//util:status",
-    ],
-)
-
-py_test(
-    name = "status_test",
-    srcs = ["status_test.py"],
-    deps = [
-        ":tink_bindings",
-        requirement("absl-py"),
-        requirement("six"),
-    ],
-)
-
-tink_pybind_library(
     name = "aead",
     srcs = ["aead.cc"],
     hdrs = ["aead.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//:aead",
         "@tink_cc//util:statusor",
     ],
 )
 
 tink_pybind_library(
     name = "deterministic_aead",
     srcs = ["deterministic_aead.cc"],
     hdrs = ["deterministic_aead.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//:deterministic_aead",
         "@tink_cc//util:statusor",
     ],
 )
 
 tink_pybind_library(
@@ -230,112 +182,112 @@
 )
 
 tink_pybind_library(
     name = "hybrid_decrypt",
     srcs = ["hybrid_decrypt.cc"],
     hdrs = ["hybrid_decrypt.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//:hybrid_decrypt",
         "@tink_cc//util:statusor",
     ],
 )
 
 tink_pybind_library(
     name = "hybrid_encrypt",
     srcs = ["hybrid_encrypt.cc"],
     hdrs = ["hybrid_encrypt.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//:hybrid_encrypt",
         "@tink_cc//util:statusor",
     ],
 )
 
 tink_pybind_library(
     name = "mac",
     srcs = ["mac.cc"],
     hdrs = ["mac.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//:mac",
         "@tink_cc//util:status",
     ],
 )
 
 tink_pybind_library(
     name = "prf",
     srcs = ["prf.cc"],
     hdrs = ["prf.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//prf:prf_set",
         "@tink_cc//util:status",
     ],
 )
 
 tink_pybind_library(
     name = "public_key_sign",
     srcs = ["public_key_sign.cc"],
     hdrs = ["public_key_sign.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//:public_key_sign",
         "@tink_cc//util:statusor",
     ],
 )
 
 tink_pybind_library(
     name = "public_key_verify",
     srcs = ["public_key_verify.cc"],
     hdrs = ["public_key_verify.h"],
     deps = [
-        ":status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//:public_key_verify",
         "@tink_cc//util:status",
     ],
 )
 
 tink_pybind_library(
     name = "cc_gcp_kms_client",
     srcs = ["cc_gcp_kms_client.cc"],
     hdrs = ["cc_gcp_kms_client.h"],
     deps = [
+        ":tink_exception",
         "//tink/cc:output_stream_adapter",
-        "//tink/cc/pybind:status_casters",
         "@pybind11",
         "@tink_cc//:kms_clients",
-        "@tink_cc//integration/gcpkms:gcp_kms_client",
+        "@tink_cc_gcpkms//:gcp_kms_client",
     ],
 )
 
 tink_pybind_library(
     name = "cc_aws_kms_client",
     srcs = ["cc_aws_kms_client.cc"],
     hdrs = ["cc_aws_kms_client.h"],
     deps = [
+        ":tink_exception",
         "//tink/cc:output_stream_adapter",
-        "//tink/cc/pybind:status_casters",
         "@pybind11",
-        "@tink_cc//integration/awskms:aws_kms_client",
+        "@tink_cc_awskms//:aws_kms_client",
     ],
 )
 
 tink_pybind_library(
     name = "cc_fake_kms_client_testonly",
     srcs = ["cc_fake_kms_client_testonly.cc"],
     hdrs = ["cc_fake_kms_client_testonly.h"],
     deps = [
-        "//tink/cc/pybind:status_casters",
+        ":tink_exception",
         "@pybind11",
         "@tink_cc//util:fake_kms_client_pybind",
         "@tink_cc//util:statusor",
     ],
 )
 
 # To avoid getting multiple instances of KmsClients, ":aead" and
@@ -344,40 +296,44 @@
     name = "tink_bindings",
     srcs = ["tink_bindings.cc"],
     deps = [
         ":aead",
         ":cc_aws_kms_client",
         ":cc_fake_kms_client_testonly",
         ":cc_gcp_kms_client",
+        ":cc_hpke_config",
         ":cc_jwt_config",
         ":cc_key_manager",
         ":cc_streaming_aead_wrappers",
         ":cc_tink_config",
         ":deterministic_aead",
         ":hybrid_decrypt",
         ":hybrid_encrypt",
         ":input_stream_adapter",
         ":mac",
         ":output_stream_adapter",
         ":prf",
         ":public_key_sign",
         ":public_key_verify",
         ":python_file_object_adapter",
-        ":status",
-        ":status_casters",
-        ":status_injector",
         ":streaming_aead",
+        ":tink_exception",
         "@tink_cc//:aead",
         "@tink_cc//:deterministic_aead",
         "@tink_cc//:hybrid_decrypt",
         "@tink_cc//:hybrid_encrypt",
         "@tink_cc//:mac",
         "@tink_cc//:public_key_sign",
         "@tink_cc//:public_key_verify",
         "@tink_cc//:streaming_aead",
-        "@tink_cc//integration/awskms:aws_kms_client",
-        "@tink_cc//integration/gcpkms:gcp_kms_client",
         "@tink_cc//prf:prf_set",
         "@tink_cc//util:status",
         "@tink_cc//util:statusor",
     ],
 )
+
+tink_pybind_library(
+    name = "tink_exception",
+    hdrs = ["tink_exception.h"],
+    visibility = ["//tink/cc:__pkg__"],
+    deps = ["@tink_cc//util:status"],
+)
```

### Comparing `tink-1.6.1/tink/cc/pybind/python_file_object_adapter.h` & `tink-1.7.0/tink/cc/pybind/python_file_object_adapter.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/prf.h` & `tink-1.7.0/tink/cc/pybind/prf.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/cc_streaming_aead_wrappers.cc` & `tink-1.7.0/tink/cc/pybind/cc_streaming_aead_wrappers.cc`

 * *Files 25% similar despite different names*

```diff
@@ -10,49 +10,65 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/cc/cc_streaming_aead_wrappers.h"
+#include "tink/cc/pybind/cc_streaming_aead_wrappers.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/cc/cc_streaming_aead_wrappers.h"
 #include "tink/cc/pybind/import_helper.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterCcStreamingAeadWrappers(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   m.def(
       "new_cc_encrypting_stream",
       // TODO(b/145925674)
       [](StreamingAead* streaming_aead, const py::bytes& aad,
          std::shared_ptr<PythonFileObjectAdapter> ciphertext_destination)
-          -> util::StatusOr<std::unique_ptr<OutputStreamAdapter>> {
-        return NewCcEncryptingStream(streaming_aead, std::string(aad),
-                                     ciphertext_destination);
+          -> std::unique_ptr<OutputStreamAdapter> {
+        util::StatusOr<std::unique_ptr<OutputStreamAdapter>> result_stream =
+            NewCcEncryptingStream(streaming_aead, std::string(aad),
+                                  ciphertext_destination);
+        if (!result_stream.ok()) {
+          throw TinkException(result_stream.status());
+        }
+        return *std::move(result_stream);
       },
       py::arg("primitive"), py::arg("aad"), py::arg("destination"),
       // Keep destination alive at least as long as OutputStreamAdapter.
       py::keep_alive<0, 3>());
 
   m.def(
       "new_cc_decrypting_stream",
       // TODO(b/145925674)
       [](StreamingAead* streaming_aead, const py::bytes& aad,
          std::shared_ptr<PythonFileObjectAdapter> ciphertext_source)
-          -> util::StatusOr<std::unique_ptr<InputStreamAdapter>> {
-        return NewCcDecryptingStream(streaming_aead, std::string(aad),
-                                     ciphertext_source);
+          -> std::unique_ptr<InputStreamAdapter> {
+        util::StatusOr<std::unique_ptr<InputStreamAdapter>> result_stream =
+            NewCcDecryptingStream(streaming_aead, std::string(aad),
+                                  ciphertext_source);
+        if (!result_stream.ok()) {
+          throw TinkException(result_stream.status());
+        }
+        return *std::move(result_stream);
       },
       py::arg("primitive"), py::arg("aad"), py::arg("source"),
       // Keep source alive at least as long as InputStreamAdapter.
       py::keep_alive<0, 3>());
 }
 
 }  // namespace tink
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_aws_kms_client.cc` & `tink-1.7.0/tink/cc/pybind/cc_aws_kms_client.cc`

 * *Files 16% similar despite different names*

```diff
@@ -10,60 +10,68 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/integration/awskms/aws_kms_client.h"
+#include "tink/cc/pybind/cc_aws_kms_client.h"
 
 #include "pybind11/pybind11.h"
+#include "tink/integration/awskms/aws_kms_client.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
-
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 namespace integration {
 namespace awskms {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterCcAwsKmsClient(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
-  py::class_<AwsKmsClient>(
-      m, "AwsKmsClient",
-      "Wrapper for C++ AwsKMS."
-      )
-      .def(py::init([](const std::string& key_uri,
-                       const std::string& credentials_path) {
-        auto client_result = AwsKmsClient::New(key_uri, credentials_path);
-        if (!client_result.ok()) {
-          throw pybind11::value_error("Could not create client.");
-        }
-        return std::move(client_result.ValueOrDie());
-      }))
+  py::class_<AwsKmsClient>(m, "AwsKmsClient", "Wrapper for C++ AwsKMS.")
+      .def(py::init(
+          [](const std::string& key_uri, const std::string& credentials_path) {
+            auto client_result = AwsKmsClient::New(key_uri, credentials_path);
+            if (!client_result.ok()) {
+              throw pybind11::value_error("Could not create client.");
+            }
+            return std::move(client_result.value());
+          }))
       .def(
           "does_support",
           [](const AwsKmsClient& self, const std::string& key_uri) -> bool {
             return self.DoesSupport(key_uri);
           },
           py::arg("key_uri"), "URI of the key to be checked.")
       .def(
           "get_aead",
-          [](const AwsKmsClient& self, const std::string& key_uri) ->
-          util::StatusOr<std::unique_ptr<Aead>> {
-            return self.GetAead(key_uri);
+          [](const AwsKmsClient& self,
+             const std::string& key_uri) -> std::unique_ptr<Aead> {
+            crypto::tink::util::StatusOr<std::unique_ptr<Aead>> aead_result =
+                self.GetAead(key_uri);
+            if (!aead_result.ok()) {
+              throw TinkException(aead_result.status());
+            }
+            return *std::move(aead_result);
           },
           py::arg("key_uri"), "URI of the key which should be used.")
       .def_static(
           "register_client",
           [](const std::string& key_uri,
-             const std::string& credentials_path) -> util::Status {
-            return AwsKmsClient::RegisterNewClient(key_uri, credentials_path);
+             const std::string& credentials_path) -> void {
+            crypto::tink::util::Status result =
+                AwsKmsClient::RegisterNewClient(key_uri, credentials_path);
+            if (!result.ok()) {
+              throw TinkException(result);
+            }
           },
           py::arg("key_uri"), "URI of the key which should be used.",
           py::arg("credentials_path"),
           "Path to the credentials for the client.");
 }
 
 }  // namespace awskms
```

### Comparing `tink-1.6.1/tink/cc/pybind/hybrid_encrypt.cc` & `tink-1.7.0/tink/cc/pybind/hybrid_encrypt.cc`

 * *Files 18% similar despite different names*

```diff
@@ -10,35 +10,45 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/hybrid_encrypt.h"
+#include "tink/cc/pybind/hybrid_encrypt.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/hybrid_encrypt.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterHybridEncrypt(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<HybridEncrypt>(m, "HybridEncrypt")
       .def(
           "encrypt",
           [](const HybridEncrypt& self, const py::bytes& plaintext,
-             const py::bytes& context_info) -> util::StatusOr<py::bytes> {
+             const py::bytes& context_info) -> py::bytes {
             // TODO(b/145925674)
-            return self.Encrypt(std::string(plaintext),
-                                std::string(context_info));
+            util::StatusOr<std::string> encrypt_result =
+                self.Encrypt(std::string(plaintext), std::string(context_info));
+            if (!encrypt_result.ok()) {
+              throw TinkException(encrypt_result.status());
+            }
+            return *std::move(encrypt_result);
           },
           py::arg("plaintext"), py::arg("context_info"));
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_key_manager_test.py` & `tink-1.7.0/tink/cc/pybind/cc_key_manager_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,44 +10,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.cc.pybind.py_key_manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from typing import cast
 from absl.testing import absltest
+from absl.testing import parameterized
 from tink.proto import aes_eax_pb2
 from tink.proto import aes_siv_pb2
 from tink.proto import common_pb2
 from tink.proto import ecdsa_pb2
 from tink.proto import ecies_aead_hkdf_pb2
 from tink.proto import hmac_pb2
 from tink.proto import hmac_prf_pb2
+from tink.proto import hpke_pb2
 from tink.proto import jwt_ecdsa_pb2
 from tink.proto import jwt_hmac_pb2
 from tink.proto import tink_pb2
 from tink import aead
 from tink import hybrid
 from tink.cc.pybind import tink_bindings
 
 
 def setUpModule():
   tink_bindings.register()
   tink_bindings.register_jwt()
+  tink_bindings.register_hpke()
 
 
 class AeadKeyManagerTest(absltest.TestCase):
 
   def setUp(self):
-    super(AeadKeyManagerTest, self).setUp()
+    super().setUp()
     self.key_manager = tink_bindings.AeadKeyManager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.AesEaxKey')
 
   def new_aes_eax_key_template(self, iv_size, key_size):
     key_format = aes_eax_pb2.AesEaxKeyFormat()
     key_format.params.iv_size = iv_size
     key_format.key_size = key_size
@@ -69,15 +68,15 @@
     key = aes_eax_pb2.AesEaxKey.FromString(key_data.value)
     self.assertEqual(key.version, 0)
     self.assertEqual(key.params.iv_size, 12)
     self.assertLen(key.key_value, 16)
 
   def test_invalid_params_raise_exception(self):
     key_template = self.new_aes_eax_key_template(9, 16)
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       self.key_manager.new_key_data(key_template)
 
   def test_encrypt_decrypt(self):
     key_template = self.new_aes_eax_key_template(12, 16)
     key_data = self.key_manager.new_key_data(key_template)
 
     primitive = self.key_manager.primitive(key_data)
@@ -86,15 +85,15 @@
     ciphertext = primitive.encrypt(plaintext, associated_data)
     self.assertEqual(primitive.decrypt(ciphertext, associated_data), plaintext)
 
 
 class DeterministicAeadKeyManagerTest(absltest.TestCase):
 
   def setUp(self):
-    super(DeterministicAeadKeyManagerTest, self).setUp()
+    super().setUp()
     daead_key_manager = tink_bindings.DeterministicAeadKeyManager
     self.key_manager = daead_key_manager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.AesSivKey')
 
   def new_aes_siv_key_template(self, key_size):
     key_format = aes_siv_pb2.AesSivKeyFormat()
     key_format.key_size = key_size
@@ -115,15 +114,15 @@
     self.assertEqual(key_data.key_material_type, tink_pb2.KeyData.SYMMETRIC)
     key = aes_siv_pb2.AesSivKey.FromString(key_data.value)
     self.assertEqual(key.version, 0)
     self.assertLen(key.key_value, 64)
 
   def test_invalid_params_raise_exception(self):
     key_template = self.new_aes_siv_key_template(65)
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       self.key_manager.new_key_data(key_template)
 
   def test_encrypt_decrypt(self):
     key_template = self.new_aes_siv_key_template(64)
     key_data = self.key_manager.new_key_data(key_template)
 
     primitive = self.key_manager.primitive(key_data)
@@ -156,15 +155,15 @@
                      tink_pb2.KeyData.ASYMMETRIC_PRIVATE)
     key = ecies_aead_hkdf_pb2.EciesAeadHkdfPrivateKey.FromString(key_data.value)
     self.assertLen(key.key_value, 32)
     self.assertEqual(key.public_key.params.kem_params.curve_type,
                      common_pb2.NIST_P256)
 
   def test_new_key_data_invalid_params_raise_exception(self):
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk,
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
                                 'Unsupported elliptic curve'):
       self.hybrid_decrypt_key_manager().new_key_data(
           hybrid.hybrid_key_templates.create_ecies_aead_hkdf_key_template(
               curve_type=cast(common_pb2.EllipticCurveType, 100),  # invalid
               ec_point_format=common_pb2.UNCOMPRESSED,
               hash_type=common_pb2.SHA256,
               dem_key_template=aead.aead_key_templates.AES128_GCM)
@@ -185,23 +184,124 @@
 
   def test_decrypt_fails(self):
     decrypt_key_manager = self.hybrid_decrypt_key_manager()
     key_data = decrypt_key_manager.new_key_data(
         hybrid.hybrid_key_templates.ECIES_P256_HKDF_HMAC_SHA256_AES128_GCM
         .SerializeToString())
     hybrid_decrypt = decrypt_key_manager.primitive(key_data)
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk,
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
                                 'ciphertext too short'):
       hybrid_decrypt.decrypt(b'bad ciphertext', b'some context info')
 
 
+class HpkeKeyManagerTest(parameterized.TestCase):
+
+  def hybrid_decrypt_key_manager(self):
+    return tink_bindings.HybridDecryptKeyManager.from_cc_registry(
+        'type.googleapis.com/google.crypto.tink.HpkePrivateKey')
+
+  def hybrid_encrypt_key_manager(self):
+    return tink_bindings.HybridEncryptKeyManager.from_cc_registry(
+        'type.googleapis.com/google.crypto.tink.HpkePublicKey')
+
+  def test_new_key_data(self):
+    key_manager = self.hybrid_decrypt_key_manager()
+    key_data = tink_pb2.KeyData.FromString(
+        key_manager.new_key_data(
+            hybrid.hybrid_key_templates
+            .DHKEM_X25519_HKDF_SHA256_HKDF_SHA256_AES_128_GCM.SerializeToString(
+            )))
+    self.assertEqual(key_data.type_url, key_manager.key_type())
+    self.assertEqual(key_data.key_material_type,
+                     tink_pb2.KeyData.ASYMMETRIC_PRIVATE)
+    key = hpke_pb2.HpkePrivateKey.FromString(key_data.value)
+    self.assertLen(key.private_key, 32)  # HPKE 'Nsk' parameter length  = 32
+    self.assertEqual(key.public_key.params.kem,
+                     hpke_pb2.DHKEM_X25519_HKDF_SHA256)
+    self.assertEqual(key.public_key.params.kdf, hpke_pb2.HKDF_SHA256)
+    self.assertEqual(key.public_key.params.aead, hpke_pb2.AES_128_GCM)
+
+  def test_new_key_data_invalid_kem_raise_exception(self):
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
+                                'Invalid KEM param.'):
+      self.hybrid_decrypt_key_manager().new_key_data(
+          hybrid.hybrid_key_templates._create_hpke_key_template(
+              hpke_kem=hpke_pb2.KEM_UNKNOWN,
+              hpke_kdf=hpke_pb2.HKDF_SHA256,
+              hpke_aead=hpke_pb2.AES_128_GCM,
+              output_prefix_type=tink_pb2.TINK).SerializeToString())
+
+  def test_new_key_data_invalid_kdf_raise_exception(self):
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
+                                'Invalid KDF param.'):
+      self.hybrid_decrypt_key_manager().new_key_data(
+          hybrid.hybrid_key_templates._create_hpke_key_template(
+              hpke_kem=hpke_pb2.DHKEM_X25519_HKDF_SHA256,
+              hpke_kdf=hpke_pb2.KDF_UNKNOWN,
+              hpke_aead=hpke_pb2.AES_128_GCM,
+              output_prefix_type=tink_pb2.TINK).SerializeToString())
+
+  def test_new_key_data_invalid_aead_raise_exception(self):
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
+                                'Invalid AEAD param.'):
+      self.hybrid_decrypt_key_manager().new_key_data(
+          hybrid.hybrid_key_templates._create_hpke_key_template(
+              hpke_kem=hpke_pb2.DHKEM_X25519_HKDF_SHA256,
+              hpke_kdf=hpke_pb2.HKDF_SHA256,
+              hpke_aead=hpke_pb2.AEAD_UNKNOWN,
+              output_prefix_type=tink_pb2.TINK).SerializeToString())
+
+  def test_encrypt_decrypt(self):
+    decrypt_key_manager = self.hybrid_decrypt_key_manager()
+    encrypt_key_manager = self.hybrid_encrypt_key_manager()
+    key_data = decrypt_key_manager.new_key_data(
+        hybrid.hybrid_key_templates
+        .DHKEM_X25519_HKDF_SHA256_HKDF_SHA256_AES_128_GCM.SerializeToString())
+    public_key_data = decrypt_key_manager.public_key_data(key_data)
+    hybrid_encrypt = encrypt_key_manager.primitive(public_key_data)
+    ciphertext = hybrid_encrypt.encrypt(b'some plaintext', b'some context info')
+    hybrid_decrypt = decrypt_key_manager.primitive(key_data)
+    self.assertEqual(
+        hybrid_decrypt.decrypt(ciphertext, b'some context info'),
+        b'some plaintext')
+
+  @parameterized.parameters(
+      [tink_pb2.TINK, tink_pb2.RAW, tink_pb2.CRUNCHY, tink_pb2.LEGACY])
+  def test_encrypt_decrypt_by_prefix(self, prefix):
+    decrypt_key_manager = self.hybrid_decrypt_key_manager()
+    encrypt_key_manager = self.hybrid_encrypt_key_manager()
+    key_data = decrypt_key_manager.new_key_data(
+        hybrid.hybrid_key_templates._create_hpke_key_template(
+            hpke_kem=hpke_pb2.DHKEM_X25519_HKDF_SHA256,
+            hpke_kdf=hpke_pb2.HKDF_SHA256,
+            hpke_aead=hpke_pb2.AES_128_GCM,
+            output_prefix_type=prefix).SerializeToString())
+    public_key_data = decrypt_key_manager.public_key_data(key_data)
+    hybrid_encrypt = encrypt_key_manager.primitive(public_key_data)
+    ciphertext = hybrid_encrypt.encrypt(b'some plaintext', b'some context info')
+    hybrid_decrypt = decrypt_key_manager.primitive(key_data)
+    self.assertEqual(
+        hybrid_decrypt.decrypt(ciphertext, b'some context info'),
+        b'some plaintext')
+
+  def test_decrypt_fails(self):
+    decrypt_key_manager = self.hybrid_decrypt_key_manager()
+    key_data = decrypt_key_manager.new_key_data(
+        hybrid.hybrid_key_templates
+        .DHKEM_X25519_HKDF_SHA256_HKDF_SHA256_AES_128_GCM.SerializeToString())
+    hybrid_decrypt = decrypt_key_manager.primitive(key_data)
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
+                                'Ciphertext is too short.'):
+      hybrid_decrypt.decrypt(b'bad ciphertext', b'some context info')
+
+
 class MacKeyManagerTest(absltest.TestCase):
 
   def setUp(self):
-    super(MacKeyManagerTest, self).setUp()
+    super().setUp()
     self.key_manager = tink_bindings.MacKeyManager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.HmacKey')
 
   def new_hmac_key_template(self, hash_type, tag_size, key_size):
     key_format = hmac_pb2.HmacKeyFormat()
     key_format.params.hash = hash_type
     key_format.params.tag_size = tag_size
@@ -224,15 +324,15 @@
     self.assertEqual(key.version, 0)
     self.assertEqual(key.params.hash, common_pb2.SHA256)
     self.assertEqual(key.params.tag_size, 24)
     self.assertLen(key.key_value, 16)
 
   def test_invalid_params_raise_exception(self):
     key_template = self.new_hmac_key_template(common_pb2.SHA256, 9, 16)
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       self.key_manager.new_key_data(key_template)
 
   def test_mac_success(self):
     mac = self.key_manager.primitive(
         self.key_manager.new_key_data(
             self.new_hmac_key_template(common_pb2.SHA256, 24, 16)))
     data = b'data'
@@ -241,23 +341,23 @@
     # No exception raised.
     mac.verify_mac(tag, data)
 
   def test_mac_wrong(self):
     mac = self.key_manager.primitive(
         self.key_manager.new_key_data(
             self.new_hmac_key_template(common_pb2.SHA256, 16, 16)))
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk,
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
                                 'verification failed'):
       mac.verify_mac(b'0123456789ABCDEF', b'data')
 
 
 class JwtMacKeyManagerTest(absltest.TestCase):
 
   def setUp(self):
-    super(JwtMacKeyManagerTest, self).setUp()
+    super().setUp()
     self.key_manager = tink_bindings.MacKeyManager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.JwtHmacKey')
 
   def new_jwt_hmac_key_template(self, algorithm, key_size):
     key_format = jwt_hmac_pb2.JwtHmacKeyFormat()
     key_format.algorithm = algorithm
     key_format.key_size = key_size
@@ -278,15 +378,15 @@
     key = jwt_hmac_pb2.JwtHmacKey.FromString(key_data.value)
     self.assertEqual(key.version, 0)
     self.assertEqual(key.algorithm, jwt_hmac_pb2.HS256)
     self.assertLen(key.key_value, 32)
 
   def test_too_short_key_size_raises_exception(self):
     key_template = self.new_jwt_hmac_key_template(jwt_hmac_pb2.HS256, 31)
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       self.key_manager.new_key_data(key_template)
 
   def test_mac_success(self):
     mac = self.key_manager.primitive(
         self.key_manager.new_key_data(
             self.new_jwt_hmac_key_template(jwt_hmac_pb2.HS256, 32)))
     data = b'data'
@@ -295,23 +395,23 @@
     # No exception raised.
     mac.verify_mac(tag, data)
 
   def test_mac_wrong(self):
     mac = self.key_manager.primitive(
         self.key_manager.new_key_data(
             self.new_jwt_hmac_key_template(jwt_hmac_pb2.HS256, 32)))
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk,
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
                                 'verification failed'):
       mac.verify_mac(b'0123456789ABCDEF0123456789ABCDEF', b'data')
 
 
 class PrfKeyManagerTest(absltest.TestCase):
 
   def setUp(self):
-    super(PrfKeyManagerTest, self).setUp()
+    super().setUp()
     self.key_manager = tink_bindings.PrfKeyManager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.HmacPrfKey')
 
   def new_hmac_prf_key_template(self, hash_type, key_size):
     key_format = hmac_prf_pb2.HmacPrfKeyFormat()
     key_format.params.hash = hash_type
     key_format.key_size = key_size
@@ -335,15 +435,15 @@
     self.assertEqual(key.version, 0)
     self.assertEqual(key.params.hash, common_pb2.SHA256)
     self.assertLen(key.key_value, 16)
 
   def test_invalid_params_raise_exception(self):
     key_template = self.new_hmac_prf_key_template(
         hash_type=common_pb2.SHA256, key_size=7)
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       self.key_manager.new_key_data(key_template)
 
   def test_prf_success(self):
     prf = self.key_manager.primitive(
         self.key_manager.new_key_data(
             self.new_hmac_prf_key_template(
                 hash_type=common_pb2.SHA256, key_size=16)))
@@ -352,22 +452,22 @@
     self.assertEqual(prf.compute(b'input_data', output_length=31), output)
 
   def test_prf_bad_output_length(self):
     prf = self.key_manager.primitive(
         self.key_manager.new_key_data(
             self.new_hmac_prf_key_template(
                 hash_type=common_pb2.SHA256, key_size=16)))
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       _ = prf.compute(b'input_data', output_length=12345)
 
 
 class PublicKeySignVerifyKeyManagerTest(absltest.TestCase):
 
   def setUp(self):
-    super(PublicKeySignVerifyKeyManagerTest, self).setUp()
+    super().setUp()
     public_key_verify_manager = tink_bindings.PublicKeyVerifyKeyManager
     self.key_manager_verify = public_key_verify_manager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.EcdsaPublicKey')
     public_key_sign_manager = tink_bindings.PublicKeySignKeyManager
     self.key_manager_sign = public_key_sign_manager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.EcdsaPrivateKey')
 
@@ -408,15 +508,16 @@
     self.assertEqual(public_key.params.curve, common_pb2.NIST_P256)
     self.assertEqual(public_key.params.encoding, ecdsa_pb2.DER)
     self.assertLen(key.key_value, 32)
 
   def test_new_key_data_verify(self):
     key_template = self.new_ecdsa_key_template(
         common_pb2.SHA256, common_pb2.NIST_P256, ecdsa_pb2.DER, True)
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk, 'not supported'):
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
+                                'not supported'):
       self.key_manager_verify.new_key_data(key_template)
 
   def test_signature_success(self):
     priv_key = self.key_manager_sign.new_key_data(
         self.new_ecdsa_key_template(common_pb2.SHA256, common_pb2.NIST_P256,
                                     ecdsa_pb2.DER))
     pub_key = self.key_manager_sign.public_key_data(priv_key)
@@ -440,41 +541,42 @@
 
     signer = self.key_manager_sign.primitive(priv_key)
     verifier = self.key_manager_verify.primitive(pub_key)
 
     data = b'data'
     signature = signer.sign(data)
 
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk,
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
                                 'Signature is not valid'):
       verifier.verify(signature, b'wrongdata')
 
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk,
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
                                 'Signature is not valid'):
       verifier.verify(b'wrongsignature', data)
 
 
 class JwtPublicKeySignVerifyKeyManagerTest(absltest.TestCase):
 
   def setUp(self):
-    super(JwtPublicKeySignVerifyKeyManagerTest, self).setUp()
+    super().setUp()
     public_key_verify_manager = tink_bindings.PublicKeyVerifyKeyManager
     self.key_manager_verify = public_key_verify_manager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.JwtEcdsaPublicKey')
     public_key_sign_manager = tink_bindings.PublicKeySignKeyManager
     self.key_manager_sign = public_key_sign_manager.from_cc_registry(
         'type.googleapis.com/google.crypto.tink.JwtEcdsaPrivateKey')
 
   def test_new_key_data_verify_fails(self):
     key_format = jwt_ecdsa_pb2.JwtEcdsaKeyFormat(algorithm=jwt_ecdsa_pb2.ES256)
     key_template = tink_pb2.KeyTemplate()
     key_template.type_url = (
         'type.googleapis.com/google.crypto.tink.JwtEcdsaPublicKey')
     key_template.value = key_format.SerializeToString()
-    with self.assertRaisesRegex(tink_bindings.StatusNotOk, 'not supported'):
+    with self.assertRaisesRegex(tink_bindings.PythonTinkException,
+                                'not supported'):
       self.key_manager_verify.new_key_data(key_template.SerializeToString())
 
   def test_signature_success(self):
     key_format = jwt_ecdsa_pb2.JwtEcdsaKeyFormat(algorithm=jwt_ecdsa_pb2.ES256)
     key_template = tink_pb2.KeyTemplate()
     key_template.type_url = (
         'type.googleapis.com/google.crypto.tink.JwtEcdsaPrivateKey')
@@ -487,16 +589,16 @@
     verifier = self.key_manager_verify.primitive(pub_key)
     signer = self.key_manager_sign.primitive(priv_key)
 
     data = b'data'
     signature = signer.sign(data)
     verifier.verify(signature, data)
 
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       verifier.verify(signature, b'wrongdata')
 
-    with self.assertRaises(tink_bindings.StatusNotOk):
+    with self.assertRaises(tink_bindings.PythonTinkException):
       verifier.verify(b'wrongsignature', data)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_key_manager.cc` & `tink-1.7.0/tink/cc/pybind/cc_key_manager.cc`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/cc/cc_key_manager.h"
+#include "tink/cc/pybind/cc_key_manager.h"
 
 #include <memory>
 
 #include "pybind11/pybind11.h"
 #include "tink/aead.h"
 #include "tink/deterministic_aead.h"
 #include "tink/hybrid_decrypt.h"
 #include "tink/hybrid_encrypt.h"
 #include "tink/mac.h"
 #include "tink/prf/prf_set.h"
 #include "tink/public_key_sign.h"
 #include "tink/public_key_verify.h"
 #include "tink/streaming_aead.h"
+#include "tink/cc/cc_key_manager.h"
 #include "tink/cc/pybind/import_helper.h"
-#include "tink/cc/pybind/status_casters.h"
 
 namespace crypto {
 namespace tink {
 
 namespace py_thin_wrappers {
 
 template <typename PrimitiveType>
```

### Comparing `tink-1.6.1/tink/cc/pybind/aead.h` & `tink-1.7.0/tink/cc/pybind/hybrid_decrypt.h`

 * *Files 10% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
-#ifndef TINK_PYTHON_TINK_CC_PYBIND_AEAD_H_
-#define TINK_PYTHON_TINK_CC_PYBIND_AEAD_H_
+#ifndef TINK_PYTHON_TINK_CC_PYBIND_HYBRID_DECRYPT_H_
+#define TINK_PYTHON_TINK_CC_PYBIND_HYBRID_DECRYPT_H_
 
 #include "pybind11/pybind11.h"
 
 namespace crypto {
 namespace tink {
 
-void PybindRegisterAead(pybind11::module* module);
+void PybindRegisterHybridDecrypt(pybind11::module* m);
 
 }  // namespace tink
 }  // namespace crypto
 
-#endif  // TINK_PYTHON_TINK_CC_PYBIND_AEAD_H_
+#endif  // TINK_PYTHON_TINK_CC_PYBIND_HYBRID_DECRYPT_H_
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_streaming_aead_wrappers.h` & `tink-1.7.0/tink/cc/pybind/cc_streaming_aead_wrappers.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/deterministic_aead.cc` & `tink-1.7.0/tink/cc/pybind/deterministic_aead.cc`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,29 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/deterministic_aead.h"
+#include "tink/cc/pybind/deterministic_aead.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/deterministic_aead.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterDeterministicAead(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<DeterministicAead>(
       m, "DeterministicAead",
@@ -48,26 +54,36 @@
       "and integrity (the data has not been tampered with) of that data, but "
       "not ",
       "its secrecy. (see https://tools.ietf.org/html/rfc5116)")
 
       .def(
           "encrypt_deterministically",
           [](const DeterministicAead& self, const py::bytes& plaintext,
-             const py::bytes& associated_data) -> util::StatusOr<py::bytes> {
+             const py::bytes& associated_data) -> py::bytes {
             // TODO(b/145925674)
-            return self.EncryptDeterministically(std::string(plaintext),
-                                                 std::string(associated_data));
+            util::StatusOr<std::string> encrypt_result =
+                self.EncryptDeterministically(std::string(plaintext),
+                                              std::string(associated_data));
+            if (!encrypt_result.ok()) {
+              throw TinkException(encrypt_result.status());
+            }
+            return *std::move(encrypt_result);
           },
           py::arg("plaintext"), py::arg("associated_data"))
       .def(
           "decrypt_deterministically",
           [](const DeterministicAead& self, const py::bytes& ciphertext,
-             const py::bytes& associated_data) -> util::StatusOr<py::bytes> {
+             const py::bytes& associated_data) -> py::bytes {
             // TODO(b/145925674)
-            return self.DecryptDeterministically(std::string(ciphertext),
-                                                 std::string(associated_data));
+            util::StatusOr<std::string> decrypt_result =
+                self.DecryptDeterministically(std::string(ciphertext),
+                                              std::string(associated_data));
+            if (!decrypt_result.ok()) {
+              throw TinkException(decrypt_result.status());
+            }
+            return *std::move(decrypt_result);
           },
           py::arg("ciphertext"), py::arg("associated_data"));
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/public_key_verify.h` & `tink-1.7.0/tink/cc/cc_tink_config.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-// Copyright 2020 Google LLC
+// Copyright 2019 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
-#ifndef TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_VERIFY_H_
-#define TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_VERIFY_H_
-#include "pybind11/pybind11.h"
+
+#ifndef TINK_PYTHON_CC_CC_TINK_CONFIG_H_
+#define TINK_PYTHON_CC_CC_TINK_CONFIG_H_
+
+#include "tink/util/status.h"
+#include "tink/registry.h"
 
 namespace crypto {
 namespace tink {
 
-void PybindRegisterPublicKeyVerify(pybind11::module* m);
+void CcTinkConfigRegister();
 
 }  // namespace tink
 }  // namespace crypto
 
-#endif  // TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_VERIFY_H_
+#endif  // TINK_PYTHON_CC_CC_TINK_CONFIG_H_
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_gcp_kms_client.h` & `tink-1.7.0/tink/cc/pybind/cc_gcp_kms_client.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/input_stream_adapter.cc` & `tink-1.7.0/tink/cc/pybind/output_stream_adapter.cc`

 * *Files 18% similar despite different names*

```diff
@@ -9,32 +9,48 @@
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
+#include "tink/cc/pybind/output_stream_adapter.h"
 
-#include "tink/cc/input_stream_adapter.h"
+#include <algorithm>
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/output_stream_adapter.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
-void PybindRegisterInputStreamAdapter(pybind11::module* module) {
+using pybind11::google_tink::TinkException;
+
+void PybindRegisterOutputStreamAdapter(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
-
   // TODO(b/146492561): Reduce the number of complicated lambdas.
-  py::class_<InputStreamAdapter>(m, "InputStreamAdapter")
+  py::class_<OutputStreamAdapter>(m, "OutputStreamAdapter")
       .def(
-          "read",
-          [](InputStreamAdapter *self, int64_t size)
-              -> util::StatusOr<py::bytes> { return self->Read(size); },
-          py::arg("size"));
+          "write",
+          [](OutputStreamAdapter* self, const py::bytes& data) -> int64_t {
+            util::StatusOr<int64_t> result = self->Write(std::string(data));
+            if (!result.ok()) {
+              throw TinkException(result.status());
+            }
+            return *std::move(result);
+          },
+          py::arg("data"))
+      .def("close", [](OutputStreamAdapter* self) -> void {
+        util::Status result = self->Close();
+        if (!result.ok()) {
+          throw TinkException(result);
+        }
+      });
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/cc_tink_config.h` & `tink-1.7.0/tink/cc/pybind/cc_tink_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/cc_jwt_config.h` & `tink-1.7.0/tink/cc/pybind/cc_jwt_config.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/status_utils.cc` & `tink-1.7.0/tink/cc/pybind/cc_jwt_config.cc`

 * *Files 20% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/cc/pybind/status_utils.h"
+#include "tink/cc/pybind/cc_jwt_config.h"
 
-#include <pybind11/pybind11.h>
+#include <utility>
 
-#include "tink/cc/pybind/import_helper.h"
-
-namespace pybind11 {
-namespace google_tink {
-
-void ImportStatusModule() {
-  // This function is called each time a Status object is passed from
-  // C++ to Python or vice versa. While it is safe to call module::import
-  // on an already-imported module, this is a super simple optimization
-  // certain to cut out any overhead.
-  static bool imported_already = false;
-  if (!imported_already) {
-    // crypto::tink::ImportTinkPythonModule("python.tink.cc.pybind.status");
-    imported_already = true;
-  }
+#include "pybind11/pybind11.h"
+#include "tink/cc/cc_jwt_config.h"
+#include "tink/cc/pybind/tink_exception.h"
+
+namespace crypto {
+namespace tink {
+
+using pybind11::google_tink::TinkException;
+
+void PybindRegisterCcJwtConfig(pybind11::module* module) {
+  namespace py = pybind11;
+  py::module& m = *module;
+  m.def("register_jwt", []() -> void {
+    util::Status result = CcJwtConfigRegister();
+    if (!result.ok()) {
+      throw TinkException(result);
+    }
+  });
 }
 
-}  // namespace google_tink
-}  // namespace pybind11
+}  // namespace tink
+}  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/prf.cc` & `tink-1.7.0/tink/cc/pybind/prf.cc`

 * *Files 9% similar despite different names*

```diff
@@ -12,35 +12,46 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/pybind/prf.h"
 
+#include <algorithm>
+#include <string>
+#include <utility>
+
 #include "pybind11/pybind11.h"
 #include "tink/prf/prf_set.h"
 #include "tink/util/statusor.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterPrf(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   py::class_<Prf>(m, "Prf", "The interface for PRF.")
       // We only wrap PrfSet objects that contain a single PRF. Therefore, we
       // only need the function "compute_primary".
       .def(
           "compute",
           [](const Prf& self, const py::bytes& input_data,
-             size_t output_length) -> util::StatusOr<py::bytes> {
+             size_t output_length) -> py::bytes {
             // TODO(b/145925674)
-            return self.Compute(std::string(input_data), output_length);
+            util::StatusOr<std::string> result =
+                self.Compute(std::string(input_data), output_length);
+            if (!result.ok()) {
+              throw TinkException(result.status());
+            }
+            return *std::move(result);
           },
           py::arg("input_data"), py::arg("output_length"),
           "Computes the value of the primary (and only) PRF.");
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/deterministic_aead.h` & `tink-1.7.0/tink/cc/pybind/deterministic_aead.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/cc_key_manager.h` & `tink-1.7.0/tink/cc/pybind/cc_key_manager.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/mac.h` & `tink-1.7.0/tink/cc/pybind/mac.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/public_key_verify.cc` & `tink-1.7.0/tink/cc/pybind/public_key_verify.cc`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,29 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#include "tink/public_key_verify.h"
+#include "tink/cc/pybind/public_key_verify.h"
+
+#include <string>
+#include <utility>
 
 #include "pybind11/pybind11.h"
+#include "tink/public_key_verify.h"
 #include "tink/util/status.h"
-#include "tink/cc/pybind/status_casters.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 void PybindRegisterPublicKeyVerify(pybind11::module* module) {
   namespace py = pybind11;
   py::module& m = *module;
 
   // TODO(b/146492561): Reduce the number of complicated lambdas.
   py::class_<PublicKeyVerify>(
       m, "PublicKeyVerify",
@@ -38,17 +44,22 @@
       "these interfaces are secure against adaptive chosen-message attacks. "
       "Signing data ensures the authenticity and the integrity of that data, "
       "but not its secrecy.")
 
       .def(
           "verify",
           [](const PublicKeyVerify& self, const py::bytes& signature,
-             const py::bytes& data) -> util::Status {
+             const py::bytes& data) -> void {
             // TODO(b/145925674)
-            return self.Verify(std::string(signature), std::string(data));
+            util::Status result =
+                self.Verify(std::string(signature), std::string(data));
+            if (!result.ok()) {
+              throw TinkException(result);
+            }
+            return;
           },
           py::arg("signature"), py::arg("data"),
           "Verifies that signature is a digital signature for data.");
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/pybind/public_key_sign.h` & `tink-1.7.0/tink/cc/pybind/cc_hpke_config.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-// Copyright 2020 Google LLC
+// Copyright 2022 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
-#ifndef TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_SIGN_H_
-#define TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_SIGN_H_
+
+#ifndef TINK_PYTHON_TINK_CC_PYBIND_CC_HPKE_CONFIG_H_
+#define TINK_PYTHON_TINK_CC_PYBIND_CC_HPKE_CONFIG_H_
+
+#include "pybind11/pybind11.h"
 
 namespace crypto {
 namespace tink {
 
-void PybindRegisterPublicKeySign(pybind11::module* m);
+void PybindRegisterCcHpkeConfig(pybind11::module* m);
 
 }  // namespace tink
 }  // namespace crypto
 
-#endif  // TINK_PYTHON_TINK_CC_PYBIND_PUBLIC_KEY_SIGN_H_
+#endif  // TINK_PYTHON_TINK_CC_PYBIND_CC_HPKE_CONFIG_H_
```

### Comparing `tink-1.6.1/tink/cc/pybind/import_helper.h` & `tink-1.7.0/tink/cc/pybind/import_helper.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/pybind/hybrid_decrypt.h` & `tink-1.7.0/tink/proto/aes_cmac_prf.proto`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 // Copyright 2020 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
-//     http://www.apache.org/licenses/LICENSE-2.0
+//      http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
-///////////////////////////////////////////////////////////////////////////////
-#ifndef TINK_PYTHON_TINK_CC_PYBIND_HYBRID_DECRYPT_H_
-#define TINK_PYTHON_TINK_CC_PYBIND_HYBRID_DECRYPT_H_
+////////////////////////////////////////////////////////////////////////////////
 
-#include "pybind11/pybind11.h"
+syntax = "proto3";
 
-namespace crypto {
-namespace tink {
+package google.crypto.tink;
 
-void PybindRegisterHybridDecrypt(pybind11::module* m);
+option java_package = "com.google.crypto.tink.proto";
+option java_multiple_files = true;
+option go_package = "github.com/google/tink/proto/aes_cmac_prf_go_proto";
 
-}  // namespace tink
-}  // namespace crypto
+// key_type: type.googleapis.com/google.crypto.tink.AesCmacPrfKey
+message AesCmacPrfKey {
+  uint32 version = 1;
+  bytes key_value = 2;
+}
 
-#endif  // TINK_PYTHON_TINK_CC_PYBIND_HYBRID_DECRYPT_H_
+message AesCmacPrfKeyFormat {
+  uint32 version = 2;
+  uint32 key_size = 1;
+}
```

### Comparing `tink-1.6.1/tink/cc/output_stream_adapter.cc` & `tink-1.7.0/tink/cc/output_stream_adapter.cc`

 * *Files 19% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 util::StatusOr<int64_t> OutputStreamAdapter::Write(absl::string_view data) {
   void* buffer;
   int64_t written = 0;
   while (written < data.size()) {
     auto next_result = stream_->Next(&buffer);
     if (!next_result.ok()) return next_result.status();
-    int available = next_result.ValueOrDie();
+    int available = next_result.value();
     int write_count =
         std::min(available, static_cast<int>(data.size() - written));
     memcpy(buffer, data.data() + written, write_count);
     if (write_count < available) stream_->BackUp(available - write_count);
     written += write_count;
   }
   return written;
```

### Comparing `tink-1.6.1/tink/cc/python_output_stream_test.cc` & `tink-1.7.0/tink/cc/python_output_stream_test.cc`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/python_output_stream.h"
 
+#include <algorithm>
 #include <memory>
+#include <string>
+#include <utility>
 
 #include "gtest/gtest.h"
 #include "absl/memory/memory.h"
 #include "absl/strings/str_cat.h"
 #include "absl/strings/string_view.h"
 #include "tink/subtle/random.h"
 #include "tink/util/status.h"
@@ -40,15 +43,15 @@
   int pos = 0;
   int remaining = contents.length();
   int available_space = 0;
   int available_bytes = 0;
   while (remaining > 0) {
     auto next_result = output_stream->Next(&buffer);
     if (!next_result.ok()) return next_result.status();
-    available_space = next_result.ValueOrDie();
+    available_space = next_result.value();
     available_bytes = std::min(available_space, remaining);
     memcpy(buffer, contents.data() + pos, available_bytes);
     remaining -= available_bytes;
     pos += available_bytes;
   }
   if (available_space > available_bytes) {
     output_stream->BackUp(available_space - available_bytes);
@@ -79,15 +82,15 @@
     auto output = absl::make_unique<test::TestWritableObject>();
     std::string* output_buffer = output->GetBuffer();
     auto output_stream =
         absl::make_unique<PythonOutputStream>(std::move(output), buffer_size);
     void* buffer;
     auto next_result = output_stream->Next(&buffer);
     EXPECT_TRUE(next_result.ok()) << next_result.status();
-    EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+    EXPECT_EQ(buffer_size, next_result.value());
     output_stream->BackUp(buffer_size);
     auto status = WriteToStream(output_stream.get(), stream_contents);
     EXPECT_TRUE(status.ok()) << status;
     EXPECT_EQ(stream_size, output_buffer->size());
     EXPECT_EQ(stream_contents, *output_buffer);
   }
 }
@@ -102,51 +105,51 @@
 
   // Prepare the stream and do the first call to Next().
   auto output_stream =
       absl::make_unique<PythonOutputStream>(std::move(output), buffer_size);
   EXPECT_EQ(0, output_stream->Position());
   auto next_result = output_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+  EXPECT_EQ(buffer_size, next_result.value());
   EXPECT_EQ(buffer_size, output_stream->Position());
   std::memcpy(buffer, stream_contents.data(), buffer_size);
 
   // BackUp several times, but in total fewer bytes than returned by Next().
   int total_backup_size = 0;
   for (int backup_size : {0, 1, 5, 0, 10, 100, -42, 400, 20, -100}) {
     SCOPED_TRACE(absl::StrCat("backup_size = ", backup_size));
     output_stream->BackUp(backup_size);
     total_backup_size += std::max(backup_size, 0);
     EXPECT_EQ(buffer_size - total_backup_size, output_stream->Position());
   }
-  EXPECT_LT(total_backup_size, next_result.ValueOrDie());
+  EXPECT_LT(total_backup_size, next_result.value());
 
   // Call Next(), it should succeed.
   next_result = output_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
 
   // BackUp() some bytes, again fewer than returned by Next().
   total_backup_size = 0;
   for (int backup_size : {0, 72, -94, 37, 82}) {
     SCOPED_TRACE(absl::StrCat("backup_size = ", backup_size));
     output_stream->BackUp(backup_size);
     total_backup_size += std::max(0, backup_size);
     EXPECT_EQ(buffer_size - total_backup_size, output_stream->Position());
   }
-  EXPECT_LT(total_backup_size, next_result.ValueOrDie());
+  EXPECT_LT(total_backup_size, next_result.value());
 
   // Call Next(), it should succeed;
   next_result = output_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
 
   // Call Next() again, it should return a full block.
   auto prev_position = output_stream->Position();
   next_result = output_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+  EXPECT_EQ(buffer_size, next_result.value());
   EXPECT_EQ(prev_position + buffer_size, output_stream->Position());
   std::memcpy(buffer, stream_contents.data() + buffer_size, buffer_size);
 
   // BackUp a few times, with total over the returned buffer_size.
   total_backup_size = 0;
   for (int backup_size :
            {0, 72, -100, buffer_size / 2, 200, -25, buffer_size / 2, 42}) {
@@ -159,15 +162,15 @@
   }
   EXPECT_EQ(total_backup_size, buffer_size);
   EXPECT_EQ(prev_position, output_stream->Position());
 
   // Call Next() again, it should return a full block.
   next_result = output_stream->Next(&buffer);
   EXPECT_TRUE(next_result.ok()) << next_result.status();
-  EXPECT_EQ(buffer_size, next_result.ValueOrDie());
+  EXPECT_EQ(buffer_size, next_result.value());
   EXPECT_EQ(prev_position + buffer_size, output_stream->Position());
   std::memcpy(buffer, stream_contents.data() + buffer_size, buffer_size);
 
   // Write the remaining stream contents to stream.
   auto status = WriteToStream(
       output_stream.get(), stream_contents.substr(output_stream->Position()));
   EXPECT_TRUE(status.ok()) << status;
```

### Comparing `tink-1.6.1/tink/cc/cc_jwt_config.cc` & `tink-1.7.0/tink/cc/cc_jwt_config.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019 Google LLC.
+// Copyright 2019 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `tink-1.6.1/tink/cc/BUILD.bazel` & `tink-1.7.0/tink/cc/BUILD.bazel`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
+load("@tink_py//tools/build_defs:tink_python_rules.bzl", "tink_pybind_library")
+
 package(default_visibility = ["//:__subpackages__"])
 
 licenses(["notice"])
 
 cc_library(
     name = "cc_key_manager",
     hdrs = ["cc_key_manager.h"],
     include_prefix = "tink/cc",
     deps = [
+        "//tink/cc/pybind:tink_exception",
+        "@com_google_absl//absl/memory",
+        "@com_google_absl//absl/status",
+        "@com_google_absl//absl/strings",
         "@tink_cc",
         "@tink_cc//util:status",
         "@tink_cc//util:statusor",
     ],
 )
 
-cc_library(
+tink_pybind_library(
     name = "cc_tink_config",
     srcs = ["cc_tink_config.cc"],
     hdrs = ["cc_tink_config.h"],
     deps = [
+        "//tink/cc/pybind:tink_exception",
         "@tink_cc",
         "@tink_cc//config:tink_config",
         "@tink_cc//util:status",
     ],
 )
 
 cc_library(
@@ -38,14 +45,24 @@
         "@tink_cc//jwt/internal:raw_jwt_rsa_ssa_pss_sign_key_manager",
         "@tink_cc//jwt/internal:raw_jwt_rsa_ssa_pss_verify_key_manager",
         "@tink_cc//util:status",
     ],
 )
 
 cc_library(
+    name = "cc_hpke_config",
+    srcs = ["cc_hpke_config.cc"],
+    hdrs = ["cc_hpke_config.h"],
+    deps = [
+        "@tink_cc//hybrid:hpke_config",
+        "@tink_cc//util:status",
+    ],
+)
+
+cc_library(
     name = "python_file_object_adapter",
     hdrs = ["python_file_object_adapter.h"],
     include_prefix = "tink/cc",
     deps = [
         "@com_google_absl//absl/strings",
         "@tink_cc//util:status",
         "@tink_cc//util:statusor",
@@ -101,14 +118,15 @@
 cc_test(
     name = "output_stream_adapter_test",
     size = "small",
     srcs = ["output_stream_adapter_test.cc"],
     deps = [
         ":output_stream_adapter",
         "@com_google_absl//absl/memory",
+        "@com_google_absl//absl/status",
         "@com_google_googletest//:gtest_main",
         "@tink_cc//:output_stream",
         "@tink_cc//subtle:random",
         "@tink_cc//util:ostream_output_stream",
     ],
 )
 
@@ -158,17 +176,17 @@
 cc_library(
     name = "python_input_stream",
     srcs = ["python_input_stream.cc"],
     hdrs = ["python_input_stream.h"],
     include_prefix = "tink/cc",
     deps = [
         ":python_file_object_adapter",
-        "@com_google_absl//absl/base:core_headers",
         "@com_google_absl//absl/memory",
         "@com_google_absl//absl/strings",
+        "@com_google_absl//absl/status",
         "@tink_cc//:input_stream",
         "@tink_cc//subtle:subtle_util",
         "@tink_cc//util:status",
         "@tink_cc//util:statusor",
     ],
 )
 
@@ -176,14 +194,15 @@
     name = "python_input_stream_test",
     size = "medium",
     srcs = ["python_input_stream_test.cc"],
     deps = [
         ":python_input_stream",
         ":test_util",
         "@com_google_absl//absl/memory",
+        "@com_google_absl//absl/status",
         "@com_google_googletest//:gtest_main",
         "@tink_cc//subtle:random",
     ],
 )
 
 cc_library(
     name = "input_stream_adapter",
```

### Comparing `tink-1.6.1/tink/cc/python_file_object_adapter.h` & `tink-1.7.0/tink/cc/python_file_object_adapter.h`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #ifndef TINK_PYTHON_CC_PYTHON_FILE_OBJECT_ADAPTER_H_
 #define TINK_PYTHON_CC_PYTHON_FILE_OBJECT_ADAPTER_H_
 
+#include <string>
+
 #include "absl/strings/string_view.h"
 #include "tink/util/status.h"
 #include "tink/util/statusor.h"
 
 namespace crypto {
 namespace tink {
```

### Comparing `tink-1.6.1/tink/cc/cc_streaming_aead_wrappers.cc` & `tink-1.7.0/tink/cc/cc_streaming_aead_wrappers.cc`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/cc_streaming_aead_wrappers.h"
 
+#include <utility>
+
 #include "tink/input_stream.h"
 #include "tink/output_stream.h"
 
 namespace crypto {
 namespace tink {
 
 util::StatusOr<std::unique_ptr<OutputStreamAdapter>> NewCcEncryptingStream(
@@ -34,15 +36,15 @@
   auto result =
       streaming_aead->NewEncryptingStream(std::move(destination_os), aad);
   if (!result.ok()) {
     return result.status();
   }
 
   // Get an OutputStreamAdapter from the EncryptingStream
-  return absl::make_unique<OutputStreamAdapter>(std::move(result.ValueOrDie()));
+  return absl::make_unique<OutputStreamAdapter>(std::move(result.value()));
 }
 
 util::StatusOr<std::unique_ptr<InputStreamAdapter>> NewCcDecryptingStream(
     StreamingAead* streaming_aead, absl::string_view aad,
     std::shared_ptr<PythonFileObjectAdapter> ciphertext_source) {
   // Get a source InputStream from the source PythonFileObjectAdapter.
   std::unique_ptr<InputStream> source_os =
@@ -51,12 +53,12 @@
   // Get a DecryptingStream from the source InputStream.
   auto result = streaming_aead->NewDecryptingStream(std::move(source_os), aad);
   if (!result.ok()) {
     return result.status();
   }
 
   // Get an InputStreamAdapter from the DecryptingStream
-  return absl::make_unique<InputStreamAdapter>(std::move(result.ValueOrDie()));
+  return absl::make_unique<InputStreamAdapter>(std::move(result.value()));
 }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/input_stream_adapter_test.cc` & `tink-1.7.0/tink/cc/input_stream_adapter_test.cc`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/input_stream_adapter.h"
 
 #include <algorithm>
 #include <sstream>
+#include <string>
+#include <utility>
 
 #include "gtest/gtest.h"
 #include "absl/memory/memory.h"
 #include "tink/input_stream.h"
 #include "tink/subtle/random.h"
 #include "tink/util/istream_input_stream.h"
 
@@ -39,70 +41,70 @@
 }
 
 TEST(InputStreamAdapterTest, BasicRead) {
   std::string data = subtle::Random::GetRandomBytes(10);
   auto adapter = GetInputStreamAdapter(-1, data);
   auto read_result = adapter->Read(10);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data);
+  EXPECT_EQ(read_result.value(), data);
 }
 
 TEST(InputStreamAdapterTest, ReadEOFError) {
   std::string data = subtle::Random::GetRandomBytes(10);
   auto adapter = GetInputStreamAdapter(-1, data);
   auto read_result = adapter->Read(10);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data);
+  EXPECT_EQ(read_result.value(), data);
   read_result = adapter->Read(10);
-  EXPECT_EQ(read_result.status().error_code(), util::error::OUT_OF_RANGE);
+  EXPECT_EQ(read_result.status().code(), absl::StatusCode::kOutOfRange);
 }
 
 TEST(InputStreamAdapterTest, MultipleRead) {
   std::string data = subtle::Random::GetRandomBytes(15);
   auto adapter = GetInputStreamAdapter(-1, data);
   auto read_result = adapter->Read(5);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data.substr(0, 5));
+  EXPECT_EQ(read_result.value(), data.substr(0, 5));
   read_result = adapter->Read(5);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data.substr(5, 5));
+  EXPECT_EQ(read_result.value(), data.substr(5, 5));
   read_result = adapter->Read(5);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data.substr(10, 5));
+  EXPECT_EQ(read_result.value(), data.substr(10, 5));
 }
 
 // In this test size of the IstreamInputStream buffer is smaller than the
 // size of data to be read. Only one call to Next() is made and hence the output
 // is smaller.
 TEST(InputStreamAdapterTest, OnlyOneNext) {
   std::string data = subtle::Random::GetRandomBytes(40);
   auto adapter = GetInputStreamAdapter(10, data);
   auto read_result = adapter->Read(35);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data.substr(0, 10));
+  EXPECT_EQ(read_result.value(), data.substr(0, 10));
 }
 
 TEST(InputStreamAdapterTest, ReadLessThanAvailable) {
   std::string data = subtle::Random::GetRandomBytes(20);
   auto adapter = GetInputStreamAdapter(-1, data);
   auto read_result = adapter->Read(10);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data.substr(0, 10));
+  EXPECT_EQ(read_result.value(), data.substr(0, 10));
 }
 
 TEST(InputStreamAdapterTest, ReadMoreThanAvailable) {
   std::string data = subtle::Random::GetRandomBytes(20);
   auto adapter = GetInputStreamAdapter(-1, data);
   auto read_result = adapter->Read(30);
   ASSERT_TRUE(read_result.status().ok()) << read_result.status();
-  EXPECT_EQ(read_result.ValueOrDie(), data);
+  EXPECT_EQ(read_result.value(), data);
 }
 
 TEST(InputStreamAdapterTest, ReadFromEmptyStream) {
   auto adapter = GetInputStreamAdapter(-1, "");
   auto read_result = adapter->Read(10);
-  EXPECT_EQ(read_result.status().error_code(), util::error::OUT_OF_RANGE);
+  EXPECT_EQ(read_result.status().code(), absl::StatusCode::kOutOfRange);
 }
 
 }  // namespace
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/cc_streaming_aead_wrappers.h` & `tink-1.7.0/tink/cc/cc_streaming_aead_wrappers.h`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/cc/input_stream_adapter.cc` & `tink-1.7.0/tink/cc/input_stream_adapter.cc`

 * *Files 8% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #include "tink/cc/input_stream_adapter.h"
 
 #include <algorithm>
+#include <string>
 
 #include "absl/strings/str_cat.h"
 #include "absl/strings/string_view.h"
 #include "tink/util/status.h"
 #include "tink/util/statusor.h"
 
 namespace crypto {
 namespace tink {
 
 util::StatusOr<std::string> InputStreamAdapter::Read(int64_t size) {
   const void* buffer;
   auto next_result = stream_->Next(&buffer);
   if (!next_result.ok()) return next_result.status();
-  int available = next_result.ValueOrDie();
+  int available = next_result.value();
   int read_count =
       size < 0 ? available : std::min(static_cast<int64_t>(available), size);
   if (read_count < available) stream_->BackUp(available - read_count);
   return std::string(
       absl::string_view(static_cast<const char*>(buffer), read_count));
 }
```

### Comparing `tink-1.6.1/tink/cc/cc_tink_config.h` & `tink-1.7.0/tink/cc/cc_jwt_config.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019 Google LLC.
+// Copyright 2019 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -10,22 +10,22 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#ifndef TINK_PYTHON_CC_CC_TINK_CONFIG_H_
-#define TINK_PYTHON_CC_CC_TINK_CONFIG_H_
+#ifndef TINK_PYTHON_CC_CC_JWT_CONFIG_H_
+#define TINK_PYTHON_CC_CC_JWT_CONFIG_H_
 
 #include "tink/util/status.h"
 #include "tink/registry.h"
 
 namespace crypto {
 namespace tink {
 
-crypto::tink::util::Status CcTinkConfigRegister();
+crypto::tink::util::Status CcJwtConfigRegister();
 
 }  // namespace tink
 }  // namespace crypto
 
-#endif  // TINK_PYTHON_CC_CC_TINK_CONFIG_H_
+#endif  // TINK_PYTHON_CC_CC_JWT_CONFIG_H_
```

### Comparing `tink-1.6.1/tink/cc/cc_jwt_config.h` & `tink-1.7.0/tink/cc/cc_hpke_config.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019 Google LLC.
+// Copyright 2022 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -10,22 +10,21 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ///////////////////////////////////////////////////////////////////////////////
 
-#ifndef TINK_PYTHON_CC_CC_JWT_CONFIG_H_
-#define TINK_PYTHON_CC_CC_JWT_CONFIG_H_
+#ifndef TINK_PYTHON_TINK_CC_CC_HPKE_CONFIG_H_
+#define TINK_PYTHON_TINK_CC_CC_HPKE_CONFIG_H_
 
 #include "tink/util/status.h"
-#include "tink/registry.h"
 
 namespace crypto {
 namespace tink {
 
-crypto::tink::util::Status CcJwtConfigRegister();
+util::Status CcHpkeConfigRegister();
 
 }  // namespace tink
 }  // namespace crypto
 
-#endif  // TINK_PYTHON_CC_CC_JWT_CONFIG_H_
+#endif  // TINK_PYTHON_TINK_CC_CC_HPKE_CONFIG_H_
```

### Comparing `tink-1.6.1/tink/cc/python_output_stream.cc` & `tink-1.7.0/tink/cc/python_output_stream.cc`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
   // The available space might not span the entire buffer, as writing
   // may succeed only for a prefix of the buffer -- in this case the data still
   // to be written is shifted in the buffer and the remaining space is returned.
   auto write_result = adapter_->Write(buffer_);
   if (!write_result.ok()) return status_ = write_result.status();
 
   // Some data was written, so we can return some portion of buffer_.
-  int written = write_result.ValueOrDie();
+  int written = write_result.value();
   position_ += written;
   count_in_buffer_ = buffer_.size();
   buffer_offset_ = buffer_.size() - written;
   if (written < buffer_.size()) {
     // Only part of the data was written, shift the remaining data in buffer_.
     // Using memmove, as source and destination may overlap.
     std::memmove(&buffer_[0], &buffer_[written], buffer_offset_);
@@ -99,20 +99,21 @@
   if (count_in_buffer_ > 0) {
     // Try to write the remaining bytes.
     int written = 0;
     while (written < count_in_buffer_) {
       auto write_result = adapter_->Write(absl::string_view(buffer_).substr(
           written, count_in_buffer_ - written));
       if (!write_result.ok()) return write_result.status();
-      written += write_result.ValueOrDie();
+      written += write_result.value();
     }
   }
   status_ = adapter_->Close();
   if (!status_.ok()) return status_;
-  status_ = util::Status(util::error::FAILED_PRECONDITION, "Stream closed");
+  status_ =
+      util::Status(absl::StatusCode::kFailedPrecondition, "Stream closed");
   return util::OkStatus();
 }
 
 int64_t PythonOutputStream::Position() const { return position_; }
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/cc/cc_key_manager.h` & `tink-1.7.0/tink/cc/cc_key_manager.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2019 Google LLC.
+// Copyright 2019 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -14,102 +14,112 @@
 //
 ///////////////////////////////////////////////////////////////////////////////
 
 #ifndef TINK_PYTHON_CC_CC_KEY_MANAGER_H_
 #define TINK_PYTHON_CC_CC_KEY_MANAGER_H_
 
 #include <string>
+#include <utility>
 
 #include "absl/memory/memory.h"
+#include "absl/status/status.h"
 #include "absl/strings/str_cat.h"
 #include "pybind11/pybind11.h"
 #include "tink/key_manager.h"
 #include "tink/registry.h"
 #include "tink/util/status.h"
 #include "tink/util/statusor.h"
+#include "tink/cc/pybind/tink_exception.h"
 
 namespace crypto {
 namespace tink {
 
+using pybind11::google_tink::TinkException;
+
 /**
  * CcKeyManager is a thin wrapper of KeyManager in
  * third_party/tink/cc/key_manager.h
  * It only implements the methods currently needed in Python, and slightly
  * changes the interface to ease usage of pybind.
  */
 template<class P>
 class CcKeyManager {
  public:
   // Returns a key manager from the registry.
-  static util::StatusOr<std::unique_ptr<CcKeyManager<P>>> GetFromCcRegistry(
+  static std::unique_ptr<CcKeyManager<P>> GetFromCcRegistry(
       const std::string& type_url) {
     auto key_manager_result = Registry::get_key_manager<P>(type_url);
     if (!key_manager_result.ok()) {
-      return util::Status(util::error::FAILED_PRECONDITION,
-                          absl::StrCat("No manager for key type '", type_url,
-                                       "' found in the registry."));
+      throw TinkException(
+          util::Status(absl::StatusCode::kFailedPrecondition,
+                       absl::StrCat("No manager for key type '", type_url,
+                                    "' found in the registry.")));
     }
-    return absl::make_unique<CcKeyManager<P>>(
-        key_manager_result.ValueOrDie());
+    return absl::make_unique<CcKeyManager<P>>(key_manager_result.value());
   }
 
   explicit CcKeyManager(const KeyManager<P>* key_manager)
       : key_manager_(key_manager) {}
 
   // Constructs an instance of P for the given 'key_data'.
-  crypto::tink::util::StatusOr<std::unique_ptr<P>> GetPrimitive(
-      const std::string& serialized_key_data) {
+  std::unique_ptr<P> GetPrimitive(
+      const std::string& serialized_key_data) const {
     google::crypto::tink::KeyData key_data;
     key_data.ParseFromString(serialized_key_data);
-    return key_manager_->GetPrimitive(key_data);
+    util::StatusOr<std::unique_ptr<P>> result =
+        key_manager_->GetPrimitive(key_data);
+    if (!result.ok()) {
+      throw TinkException(result.status());
+    }
+    return *std::move(result);
   }
 
   // Creates a new random key, based on the specified 'key_format'.
-  crypto::tink::util::StatusOr<pybind11::bytes> NewKeyData(
-      const std::string& serialized_key_template) {
+  pybind11::bytes NewKeyData(const std::string& serialized_key_template) const {
     google::crypto::tink::KeyTemplate key_template;
     key_template.ParseFromString(serialized_key_template);
     if (key_manager_->get_key_type() != key_template.type_url()) {
-      return util::Status(util::error::INVALID_ARGUMENT,
-                          absl::StrCat("Key type '", key_template.type_url(),
-                                       "' is not supported by this manager."));
+      throw TinkException(
+          util::Status(absl::StatusCode::kInvalidArgument,
+                       absl::StrCat("Key type '", key_template.type_url(),
+                                    "' is not supported by this manager.")));
     }
 
     auto key_data =
         key_manager_->get_key_factory().NewKeyData(key_template.value());
     if (!key_data.ok()) {
-      return key_data.status();
+      throw TinkException(key_data.status());
     }
-    return pybind11::bytes(key_data.ValueOrDie()->SerializeAsString());
+    return pybind11::bytes(key_data.value()->SerializeAsString());
   }
 
   // Returns public key data extracted from the given private_key_data.
-  crypto::tink::util::StatusOr<pybind11::bytes>
-  GetPublicKeyData(const std::string& serialized_private_key_data) const {
+  pybind11::bytes GetPublicKeyData(
+      const std::string& serialized_private_key_data) const {
     const PrivateKeyFactory* factory = dynamic_cast<const PrivateKeyFactory*>(
         &key_manager_->get_key_factory());
     if (factory == nullptr) {
-      return util::Status(util::error::INVALID_ARGUMENT,
-                          absl::StrCat("KeyManager for type '",
-                                       key_manager_->get_key_type().c_str(),
-                                       "' does not have "
-                                       "a PrivateKeyFactory."));
+      throw TinkException(util::Status(
+          absl::StatusCode::kInvalidArgument,
+          absl::StrCat("KeyManager for type '", key_manager_->get_key_type(),
+                       "' does not have "
+                       "a PrivateKeyFactory.")));
     }
 
     google::crypto::tink::KeyData private_key_data;
     private_key_data.ParseFromString(serialized_private_key_data);
     auto result = factory->GetPublicKeyData(private_key_data.value());
     if (!result.ok()) {
-      return result.status();
+      throw TinkException(result.status());
     }
-    return pybind11::bytes(result.ValueOrDie()->SerializeAsString());
+    return pybind11::bytes(result.value()->SerializeAsString());
   }
 
   // Returns the type_url identifying the key type handled by this manager.
-  std::string KeyType() { return key_manager_->get_key_type(); }
+  std::string KeyType() const { return key_manager_->get_key_type(); }
 
  private:
   const KeyManager<P>* key_manager_;
 };
 
 }  // namespace tink
 }  // namespace crypto
```

### Comparing `tink-1.6.1/tink/_keyset_reader_test.py` & `tink-1.7.0/tink/_keyset_reader_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink._keyset_reader."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from typing import cast
 from absl.testing import absltest
 
 from tink.proto import tink_pb2
 import tink
 from tink import core
```

### Comparing `tink-1.6.1/tink/daead/_deterministic_aead_key_manager_test.py` & `tink-1.7.0/tink/daead/_deterministic_aead_key_manager_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.deterministic_aead_key_manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 
 from tink.proto import aes_siv_pb2
 from tink.proto import tink_pb2
 import tink
 from tink import core
 from tink import daead
```

### Comparing `tink-1.6.1/tink/daead/_deterministic_aead_key_templates.py` & `tink-1.7.0/tink/daead/_deterministic_aead_key_templates.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,31 +16,35 @@
 
 One can use these templates to generate a new tink_pb2.Keyset with
 tink_pb2.KeysetHandle. To generate a new keyset that contains a single
 tink_pb2.HmacKey, one can do:
 handle = keyset_handle.KeysetHandle(aead_key_templates.AES128_EAX).
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
+import warnings
 
 from tink.proto import aes_siv_pb2
 from tink.proto import tink_pb2
 
 
 _AES_SIV_KEY_TYPE_URL = 'type.googleapis.com/google.crypto.tink.AesSivKey'
 
 
-def create_aes_siv_key_template(key_size: int) -> tink_pb2.KeyTemplate:
+def _create_aes_siv_key_template(key_size: int) -> tink_pb2.KeyTemplate:
   """Creates an AES EAX KeyTemplate, and fills in its values."""
   key_format = aes_siv_pb2.AesSivKeyFormat()
   key_format.key_size = key_size
   key_template = tink_pb2.KeyTemplate()
   key_template.type_url = _AES_SIV_KEY_TYPE_URL
   key_template.output_prefix_type = tink_pb2.TINK
   key_template.value = key_format.SerializeToString()
   return key_template
 
 
-AES256_SIV = create_aes_siv_key_template(key_size=64)
+AES256_SIV = _create_aes_siv_key_template(key_size=64)
+
+
+# Deprecated. Use the predefined constant AES256_SIV instead.
+def create_aes_siv_key_template(key_size: int) -> tink_pb2.KeyTemplate:
+  warnings.warn('The "create_aes_siv_key_template" function is deprecated.',
+                DeprecationWarning, 2)
+  return _create_aes_siv_key_template(key_size)
```

### Comparing `tink-1.6.1/tink/daead/_deterministic_aead_key_templates_test.py` & `tink-1.7.0/tink/mac/_mac_key_templates_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,50 @@
-# Copyright 2019 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""Tests for tink.python.tink.deterministic_aead_key_templates."""
-
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
+"""Tests for tink.python.tink._mac_key_templates."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
-from tink.proto import aes_siv_pb2
+from tink.proto import common_pb2
+from tink.proto import hmac_pb2
 from tink.proto import tink_pb2
-from tink import daead
-from tink.testing import helper
-
+from tink import mac
 
-class DeterministicAeadKeyTemplatesTest(parameterized.TestCase):
 
-  @parameterized.parameters([
-      ('AES256_SIV', daead.deterministic_aead_key_templates.AES256_SIV),
-  ])
-  def test_template(self, template_name, template):
-    self.assertEqual(template,
-                     helper.template_from_testdata(template_name, 'daead'))
+class MacKeyTemplatesTest(parameterized.TestCase):
 
-  def test_create_aes_siv_key_template(self):
-    # Intentionally using 'weird' or invalid values for parameters,
+  def test_create_hmac_key_template(self):
+    # Intentionally using "weird" or invalid values for parameters,
     # to test that the function correctly puts them in the resulting template.
-    template = (daead.deterministic_aead_key_templates
-                .create_aes_siv_key_template(key_size=42))
-    self.assertEqual('type.googleapis.com/google.crypto.tink.AesSivKey',
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = mac.mac_key_templates.create_hmac_key_template(
+          key_size=42, tag_size=24, hash_type=common_pb2.SHA512)
+    self.assertEqual('type.googleapis.com/google.crypto.tink.HmacKey',
                      template.type_url)
     self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
-    key_format = aes_siv_pb2.AesSivKeyFormat()
-    key_format.ParseFromString(template.value)
+    key_format = hmac_pb2.HmacKeyFormat.FromString(template.value)
     self.assertEqual(42, key_format.key_size)
+    self.assertEqual(24, key_format.params.tag_size)
+    self.assertEqual(common_pb2.SHA512, key_format.params.hash)
+
+  def test_create_aes_cmac_key_template(self):
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = mac.mac_key_templates.create_aes_cmac_key_template(
+          key_size=42, tag_size=24)
+    self.assertEqual('type.googleapis.com/google.crypto.tink.AesCmacKey',
+                     template.type_url)
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/daead/_deterministic_aead_wrapper.py` & `tink-1.7.0/tink/daead/_deterministic_aead_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Deterministic AEAD wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from typing import Type
 from absl import logging
 
 from tink import core
 from tink.daead import _deterministic_aead
```

### Comparing `tink-1.6.1/tink/daead/_deterministic_aead_key_manager.py` & `tink-1.7.0/tink/daead/_deterministic_aead_key_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python wrapper of the wrapped C++ Deterministic AEAD key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.daead import _deterministic_aead
 from tink.daead import _deterministic_aead_wrapper
 
 
 class _DeterministicAeadCcToPyWrapper(_deterministic_aead.DeterministicAead):
@@ -41,15 +36,15 @@
   def decrypt_deterministically(self, ciphertext: bytes,
                                 associated_data: bytes) -> bytes:
     return self._deterministic_aead.decrypt_deterministically(
         ciphertext, associated_data)
 
 
 def register():
-  """Registers all Hybrid key managers and wrapper in the Python Registry."""
+  """Registers all deterministic AEAD key managers and the wrapper in the Python Registry."""
   tink_bindings.register()
 
   type_url = 'type.googleapis.com/google.crypto.tink.AesSivKey'
   key_manager = core.KeyManagerCcToPyWrapper(
       tink_bindings.DeterministicAeadKeyManager.from_cc_registry(type_url),
       _deterministic_aead.DeterministicAead, _DeterministicAeadCcToPyWrapper)
   core.Registry.register_key_manager(key_manager, new_key_allowed=True)
```

### Comparing `tink-1.6.1/tink/daead/_deterministic_aead_wrapper_test.py` & `tink-1.7.0/tink/daead/_deterministic_aead_wrapper_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.aead_wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 import tink
 from tink import daead
 from tink.testing import keyset_builder
```

### Comparing `tink-1.6.1/tink/daead/BUILD.bazel` & `tink-1.7.0/tink/daead/BUILD.bazel`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     ],
 )
 
 py_library(
     name = "_deterministic_aead",
     srcs = ["_deterministic_aead.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_deterministic_aead_key_manager",
     srcs = ["_deterministic_aead_key_manager.py"],
     srcs_version = "PY3",
     deps = [
@@ -60,24 +59,20 @@
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_deterministic_aead_key_templates_test",
     srcs = ["_deterministic_aead_key_templates_test.py"],
-    data = [
-        "@tink_base//testdata/templates",
-    ],
     srcs_version = "PY3",
     deps = [
         ":daead",
         requirement("absl-py"),
         "//tink/proto:aes_siv_py_pb2",
         "//tink/proto:tink_py_pb2",
-        "//tink/testing:helper",
     ],
 )
 
 py_library(
     name = "_deterministic_aead_wrapper",
     srcs = ["_deterministic_aead_wrapper.py"],
     srcs_version = "PY3",
```

### Comparing `tink-1.6.1/tink/daead/__init__.py` & `tink-1.7.0/tink/daead/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Deterministic aead package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
 from tink.daead import _deterministic_aead
 from tink.daead import _deterministic_aead_key_manager
 from tink.daead import _deterministic_aead_key_templates as deterministic_aead_key_templates
 
 
 DeterministicAead = _deterministic_aead.DeterministicAead
```

### Comparing `tink-1.6.1/tink/daead/_deterministic_aead.py` & `tink-1.7.0/tink/daead/_deterministic_aead.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,27 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module defines the interface for Deterministic AEAD."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 
-# Special imports
-import six
-
 
-@six.add_metaclass(abc.ABCMeta)
-class DeterministicAead(object):
+class DeterministicAead(metaclass=abc.ABCMeta):
   """Interface for Deterministic Authenticated Encryption with Associated Data.
 
   For why this interface is desirable and some of its use cases, see for
   example https://tools.ietf.org/html/rfc5297#section-1.3.
 
   Warning!
```

### Comparing `tink-1.6.1/tink/tink_config.py` & `tink-1.7.0/tink/tink_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Static methods for handling of Tink configurations."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from tink import aead
 from tink import daead
 from tink import hybrid
 from tink import mac
 from tink import prf
 from tink import signature
 from tink import streaming_aead
```

### Comparing `tink-1.6.1/tink/testing/bytes_io_test.py` & `tink-1.7.0/tink/testing/bytes_io_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,24 +7,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for tink.python.tink.util.bytes_io."""
-
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
+"""Tests for tink.python.tink.testing.bytes_io."""
 
 import io
 
 from absl.testing import absltest
+
 from tink.testing import bytes_io
 
 
 class BytesIoTest(absltest.TestCase):
 
   def test_close_success(self):
     f = bytes_io.BytesIOWithValueAfterClose()
```

### Comparing `tink-1.6.1/tink/testing/keyset_builder_test.py` & `tink-1.7.0/tink/testing/keyset_builder_test.py`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/testing/fake_kms_test.py` & `tink-1.7.0/tink/testing/fake_kms_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.testing._fake_kms."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from absl.testing import absltest
 import tink
 from tink import aead
 from tink.testing import fake_kms
 
 
 KEY_URI = (
```

### Comparing `tink-1.6.1/tink/testing/fake_kms.py` & `tink-1.7.0/tink/testing/fake_kms.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A client for Fake KMS."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from tink.cc.pybind import tink_bindings
 
 
 def register_client(key_uri=None, credentials_path=None) -> None:
   """Registers a fake KMS client."""
   if not key_uri:
     key_uri = ''
```

### Comparing `tink-1.6.1/tink/testing/BUILD.bazel` & `tink-1.7.0/tink/testing/BUILD.bazel`

 * *Files 6% similar despite different names*

```diff
@@ -20,43 +20,37 @@
         "//tink/signature",
     ],
 )
 
 py_test(
     name = "helper_test",
     srcs = ["helper_test.py"],
-    data = [
-        "@tink_base//testdata:credentials",
-        "@tink_base//testdata/templates",
-    ],
+    # This is used to check Tink Python testdata path.
+    data = ["//testdata/gcp:credentials"],
     srcs_version = "PY3",
     deps = [
         ":helper",
         requirement("absl-py"),
         "//tink/core",
     ],
 )
 
 py_library(
     name = "bytes_io",
     srcs = ["bytes_io.py"],
     srcs_version = "PY3",
-    deps = [
-        "//tink/cc/pybind:tink_bindings",
-    ],
 )
 
 py_test(
     name = "bytes_io_test",
     srcs = ["bytes_io_test.py"],
     srcs_version = "PY3",
     deps = [
         ":bytes_io",
         requirement("absl-py"),
-        requirement("six"),
     ],
 )
 
 py_library(
     name = "keyset_builder",
     testonly = 1,
     srcs = [
```

### Comparing `tink-1.6.1/tink/testing/__init__.py` & `tink-1.7.0/tink/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/testing/keyset_builder.py` & `tink-1.7.0/tink/testing/keyset_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python implementation of a KeysetBuilder."""
 
-# Placeholder for import for type annotations
-
 import io
 import random
 from tink.proto import tink_pb2
 import tink
 from tink import cleartext_keyset_handle
 
 _MAX_INT32 = 4294967295  # 2^32-1
@@ -45,15 +43,15 @@
 def legacy_template(template: tink_pb2.KeyTemplate) -> tink_pb2.KeyTemplate:
   template_copy = tink_pb2.KeyTemplate()
   template_copy.CopyFrom(template)
   template_copy.output_prefix_type = tink_pb2.LEGACY
   return template_copy
 
 
-class KeysetBuilder(object):
+class KeysetBuilder:
   """A KeysetBuilder provides convenience methods for managing Keysets.
 
   It provides methods for adding, disabling, enabling, or deleting keys.
   The validity of the keyset is checked when creating a keyset_handle.
   """
 
   def __init__(self, keyset_proto: tink_pb2.Keyset):
```

### Comparing `tink-1.6.1/tink/testing/helper_test.py` & `tink-1.7.0/tink/testing/helper_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,38 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.testing.helper."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import os
 
 from absl.testing import absltest
 from tink import core
 from tink.testing import helper
 
 
 class HelperTest(absltest.TestCase):
 
-  def test_tink_root_path(self):
-    path = os.path.join(helper.tink_root_path(), 'testdata/credential.json')
+  def test_tink_py_testdata_path(self):
+    path = os.path.join(helper.tink_py_testdata_path(), 'gcp/credential.json')
     with open(path, mode='rt') as f:
       credential_json = f.read()
     self.assertNotEmpty(credential_json)
 
-  def test_template_from_testdata(self):
-    template = helper.template_from_testdata('AES128_GCM', 'aead')
-    self.assertEqual(template.type_url,
-                     'type.googleapis.com/google.crypto.tink.AesGcmKey')
-
   def test_fake_mac_success(self):
     mac = helper.FakeMac('Name')
     mac_value = mac.compute_mac(b'data')
     mac.verify_mac(mac_value, b'data')
 
   def test_fake_mac_fail_wrong_data(self):
     mac = helper.FakeMac('Name')
```

### Comparing `tink-1.6.1/tink/testing/helper.py` & `tink-1.7.0/tink/testing/helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,107 +10,89 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This class implements helper functions for testing."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import os
-from typing import Text, Mapping, Optional
+from typing import Mapping
 
 from tink.proto import tink_pb2
 from tink import aead
 from tink import core
 from tink import daead
 from tink import hybrid
 from tink import mac
 from tink import prf
 from tink import signature as pk_signature
-from google.protobuf import text_format
 
+_RELATIVE_TESTDATA_PATH = 'tink_py/testdata'
 
-def tink_root_path() -> Text:
-  """Returns the path to the Tink root directory used for the test enviroment.
 
-     The path can be set in the TINK_SRC_PATH enviroment variable. If Bazel
-     is used the path is derived from the Bazel enviroment variables. If that
-     does not work, it generates the root path relative to the __file__ path.
-  """
-  root_paths = []
-  if 'TINK_SRC_PATH' in os.environ:
-    root_paths.append(os.environ['TINK_SRC_PATH'])
+def tink_py_testdata_path() -> str:
+  """Returns the path to the test data directory to be used for testing."""
+  # List of pairs <Env. variable, Path>.
+  testdata_paths = []
+  if 'TINK_PYTHON_ROOT_PATH' in os.environ:
+    testdata_paths.append(('TINK_PYTHON_ROOT_PATH',
+                           os.path.join(os.environ['TINK_PYTHON_ROOT_PATH'],
+                                        'testdata')))
   if 'TEST_SRCDIR' in os.environ:
-    # Bazel enviroment
-    root_paths.append(os.path.join(os.environ['TEST_SRCDIR'], 'tink_base'))
-    root_paths.append(os.path.join(os.environ['TEST_SRCDIR'],
-                                   'google3/third_party/tink'))
-  for root_path in root_paths:
-    # return the first root path that exists.
-    if os.path.exists(root_path):
-      return root_path
-  raise ValueError('Could not find path to Tink root directory. Make sure that '
-                   'TINK_SRC_PATH is set.')
-
-
-def template_from_testdata(
-    template_name: Text,
-    dir_name: Optional[Text] = None) -> tink_pb2.KeyTemplate:
-  """Reads a template from the testdata."""
-  if dir_name:
-    path = os.path.join(tink_root_path(), 'testdata/templates', dir_name,
-                        template_name)
-  else:
-    path = os.path.join(tink_root_path(), 'testdata/templates', template_name)
-  with open(path, mode='rt') as f:
-    data = f.read()
-  return text_format.Parse(data, tink_pb2.KeyTemplate())
-
-
-def fake_key(value: bytes = b'fakevalue',
-             type_url: Text = 'fakeurl',
-             key_material_type: tink_pb2.KeyData.KeyMaterialType = tink_pb2
-             .KeyData.SYMMETRIC,
-             key_id: int = 1234,
-             status: tink_pb2.KeyStatusType = tink_pb2.ENABLED,
-             output_prefix_type: tink_pb2.OutputPrefixType = tink_pb2.TINK
-            ) -> tink_pb2.Keyset.Key:
+    testdata_paths.append(('TEST_SRCDIR',
+                           os.path.join(os.environ['TEST_SRCDIR'],
+                                        _RELATIVE_TESTDATA_PATH)))
+  for env_variable, testdata_path in testdata_paths:
+    # Return the first path that is encountered.
+    if not os.path.exists(testdata_path):
+      raise FileNotFoundError(f'Variable {env_variable} is set but has an ' +
+                              f'invalid path {testdata_path}')
+    return testdata_path
+  raise ValueError('No path environment variable set among ' +
+                   'TINK_PYTHON_ROOT_PATH, TEST_SRCDIR')
+
+
+def fake_key(
+    value: bytes = b'fakevalue',
+    type_url: str = 'fakeurl',
+    key_material_type: tink_pb2.KeyData.KeyMaterialType = tink_pb2.KeyData
+    .SYMMETRIC,
+    key_id: int = 1234,
+    status: tink_pb2.KeyStatusType = tink_pb2.ENABLED,
+    output_prefix_type: tink_pb2.OutputPrefixType = tink_pb2.TINK
+) -> tink_pb2.Keyset.Key:
   """Returns a fake but valid key."""
   key = tink_pb2.Keyset.Key(
       key_id=key_id,
       status=status,
       output_prefix_type=output_prefix_type)
   key.key_data.type_url = type_url
   key.key_data.value = value
   key.key_data.key_material_type = key_material_type
   return key
 
 
 class FakeMac(mac.Mac):
   """A fake MAC implementation."""
 
-  def __init__(self, name: Text = 'FakeMac'):
+  def __init__(self, name: str = 'FakeMac'):
     self._name = name
 
   def compute_mac(self, data: bytes) -> bytes:
     return data + b'|' + self._name.encode()
 
   def verify_mac(self, mac_value: bytes, data: bytes) -> None:
     if mac_value != data + b'|' + self._name.encode():
       raise core.TinkError('invalid mac ' + mac_value.decode())
 
 
 class FakeAead(aead.Aead):
   """A fake AEAD implementation."""
 
-  def __init__(self, name: Text = 'FakeAead'):
+  def __init__(self, name: str = 'FakeAead'):
     self._name = name
 
   def encrypt(self, plaintext: bytes, associated_data: bytes) -> bytes:
     return plaintext + b'|' + associated_data + b'|' + self._name.encode()
 
   def decrypt(self, ciphertext: bytes, associated_data: bytes) -> bytes:
     data = ciphertext.split(b'|')
@@ -120,15 +102,15 @@
                            ciphertext.decode())
     return data[0]
 
 
 class FakeDeterministicAead(daead.DeterministicAead):
   """A fake Deterministic AEAD implementation."""
 
-  def __init__(self, name: Text = 'FakeDeterministicAead'):
+  def __init__(self, name: str = 'FakeDeterministicAead'):
     self._name = name
 
   def encrypt_deterministically(self, plaintext: bytes,
                                 associated_data: bytes) -> bytes:
     return plaintext + b'|' + associated_data + b'|' + self._name.encode()
 
   def decrypt_deterministically(self, ciphertext: bytes,
@@ -141,15 +123,15 @@
                            ciphertext.decode())
     return data[0]
 
 
 class FakeHybridDecrypt(hybrid.HybridDecrypt):
   """A fake HybridEncrypt implementation."""
 
-  def __init__(self, name: Text = 'Hybrid'):
+  def __init__(self, name: str = 'Hybrid'):
     self._name = name
 
   def decrypt(self, ciphertext: bytes, context_info: bytes) -> bytes:
     data = ciphertext.split(b'|')
     if (len(data) < 3 or
         data[1] != context_info or
         data[2] != self._name.encode()):
@@ -157,61 +139,61 @@
                            ciphertext.decode())
     return data[0]
 
 
 class FakeHybridEncrypt(hybrid.HybridEncrypt):
   """A fake HybridEncrypt implementation."""
 
-  def __init__(self, name: Text = 'Hybrid'):
+  def __init__(self, name: str = 'Hybrid'):
     self._name = name
 
   def encrypt(self, plaintext: bytes, context_info: bytes) -> bytes:
     return plaintext + b'|' + context_info + b'|' + self._name.encode()
 
 
 class FakePublicKeySign(pk_signature.PublicKeySign):
   """A fake PublicKeySign implementation."""
 
-  def __init__(self, name: Text = 'FakePublicKeySign'):
+  def __init__(self, name: str = 'FakePublicKeySign'):
     self._name = name
 
   def sign(self, data: bytes) -> bytes:
     return data + b'|' + self._name.encode()
 
 
 class FakePublicKeyVerify(pk_signature.PublicKeyVerify):
   """A fake PublicKeyVerify implementation."""
 
-  def __init__(self, name: Text = 'FakePublicKeyVerify'):
+  def __init__(self, name: str = 'FakePublicKeyVerify'):
     self._name = name
 
   def verify(self, signature: bytes, data: bytes):
     if signature != data + b'|' + self._name.encode():
       raise core.TinkError('invalid signature ' + signature.decode())
 
 
 class FakePrf(prf.Prf):
   """A fake Prf implementation."""
 
-  def __init__(self, name: Text = 'FakePrf'):
+  def __init__(self, name: str = 'FakePrf'):
     self._name = name
 
   def compute(self, input_data: bytes, output_length: int) -> bytes:
     if output_length > 32:
       raise core.TinkError('invalid output_length')
     output = (
         input_data + b'|' + self._name.encode() + b'|' +
         b''.join([b'*' for _ in range(output_length)]))
     return output[:output_length]
 
 
 class FakePrfSet(prf.PrfSet):
   """A fake PrfSet implementation that contains exactly one Prf."""
 
-  def __init__(self, name: Text = 'FakePrf'):
+  def __init__(self, name: str = 'FakePrf'):
     self._prf = FakePrf(name)
 
   def primary_id(self) -> int:
     return 0
 
   def all(self) -> Mapping[int, prf.Prf]:
     return {0: self._prf}
```

### Comparing `tink-1.6.1/tink/testing/bytes_io.py` & `tink-1.7.0/tink/testing/bytes_io.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,80 +16,75 @@
 This class can be used when an interface that writes to a stream and closes it
 in the end need to be transformed into a function that returns a value.
 
 An example is the implementation of normal AEAD encryption interface using
 the streaming AEAD encryption interface.
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import errno
 import io
 from typing import Optional
 
 
 class BytesIOWithValueAfterClose(io.BytesIO):
   """A BytesIO that lets you read the written value after close()."""
 
   def __init__(self, initial_bytes=None):
     self._finalvalue = None
     if initial_bytes:
-      super(BytesIOWithValueAfterClose, self).__init__(initial_bytes)
+      super().__init__(initial_bytes)
     else:
-      super(BytesIOWithValueAfterClose, self).__init__()
+      super().__init__()
 
   def close(self) -> None:
     if not self.closed:
       self._value_after_close = self.getvalue()
-    super(BytesIOWithValueAfterClose, self).close()
+    super().close()
 
   def value_after_close(self) -> bytes:
     if not self.closed:
       raise ValueError('call to value_after_close before close()')
     return self._value_after_close
 
 
 class SlowBytesIO(io.BytesIO):
   """A readable BytesIO that raised BlockingIOError on some calls to read."""
 
   def __init__(self, data: bytes, seekable: bool = False):
-    super(SlowBytesIO, self).__init__(data)
+    super().__init__(data)
     self._seekable = seekable
     self._state = -1
 
   def read(self, size: int = -1) -> bytes:
     if size > 0:
       self._state += 1
       if self._state > 10000000:
         raise AssertionError('too many read. Is there an infinite loop?')
       if self._state % 3 == 0:   # block on every third call.
         raise io.BlockingIOError(
             errno.EAGAIN,
             'write could not complete without blocking', 0)
       # read at most 5 bytes.
-      return super(SlowBytesIO, self).read(min(size, 5))
-    return super(SlowBytesIO, self).read(size)
+      return super().read(min(size, 5))
+    return super().read(size)
 
   def seek(self, pos: int, whence: int = 0) -> int:
     if self._seekable:
-      return super(SlowBytesIO, self).seek(pos, whence)
+      return super().seek(pos, whence)
     raise io.UnsupportedOperation('seek')
 
   def seekable(self)-> bool:
     return self._seekable
 
 
 class SlowReadableRawBytes(io.RawIOBase):
   """A readable io.RawIOBase stream that only sometimes returns data."""
 
   def __init__(self, data: bytes, seekable: bool = False):
-    super(SlowReadableRawBytes, self).__init__()
+    super().__init__()
     self._bytes_io = io.BytesIO(data)
     self._seekable = seekable
     self._state = -1
 
   def readinto(self, b: bytearray) -> Optional[int]:
     try:
       self._state += 1
```

### Comparing `tink-1.6.1/tink/signature/_signature_wrapper.py` & `tink-1.7.0/tink/signature/_signature_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Public Key Sign wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from typing import Type
 from absl import logging
 
 from tink.proto import tink_pb2
 from tink import core
 from tink.signature import _public_key_sign
 from tink.signature import _public_key_verify
```

### Comparing `tink-1.6.1/tink/signature/_signature_key_manager.py` & `tink-1.7.0/tink/signature/_signature_key_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python wrapper of the wrapped C++ Public Key Signature key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.signature import _public_key_sign
 from tink.signature import _public_key_verify
 from tink.signature import _signature_wrapper
```

### Comparing `tink-1.6.1/tink/signature/BUILD.bazel` & `tink-1.7.0/tink/signature/BUILD.bazel`

 * *Files 16% similar despite different names*

```diff
@@ -18,22 +18,20 @@
     ],
 )
 
 py_library(
     name = "_public_key_sign",
     srcs = ["_public_key_sign.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_public_key_verify",
     srcs = ["_public_key_verify.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_signature_key_manager",
     srcs = ["_signature_key_manager.py"],
     srcs_version = "PY3",
     deps = [
@@ -87,33 +85,15 @@
 )
 
 py_library(
     name = "_signature_key_templates",
     srcs = ["_signature_key_templates.py"],
     srcs_version = "PY3",
     deps = [
+        "//tink/internal:big_integer_util",
         "//tink/proto:common_py_pb2",
         "//tink/proto:ecdsa_py_pb2",
         "//tink/proto:rsa_ssa_pkcs1_py_pb2",
         "//tink/proto:rsa_ssa_pss_py_pb2",
         "//tink/proto:tink_py_pb2",
     ],
 )
-
-py_test(
-    name = "_signature_key_templates_test",
-    srcs = ["_signature_key_templates_test.py"],
-    data = [
-        "@tink_base//testdata/templates",
-    ],
-    srcs_version = "PY3",
-    deps = [
-        ":signature",
-        requirement("absl-py"),
-        "//tink/proto:common_py_pb2",
-        "//tink/proto:ecdsa_py_pb2",
-        "//tink/proto:rsa_ssa_pkcs1_py_pb2",
-        "//tink/proto:rsa_ssa_pss_py_pb2",
-        "//tink/proto:tink_py_pb2",
-        "//tink/testing:helper",
-    ],
-)
```

### Comparing `tink-1.6.1/tink/signature/__init__.py` & `tink-1.7.0/tink/signature/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Signature package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 
 from tink.signature import _public_key_sign
 from tink.signature import _public_key_verify
 from tink.signature import _signature_key_manager
 from tink.signature import _signature_key_templates as signature_key_templates
```

### Comparing `tink-1.6.1/tink/signature/_public_key_verify.py` & `tink-1.7.0/tink/signature/_public_key_verify.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,26 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Interface for PublicKeyVerify."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
-# Special imports
-import six
 
 
-@six.add_metaclass(abc.ABCMeta)
-class PublicKeyVerify(object):
+class PublicKeyVerify(metaclass=abc.ABCMeta):
   """Interface for public key verifying.
 
   Digital Signatures provide functionality of signing data and verification of
   the signatures. They are represented by a pair of primitives (interfaces)
   'PublicKeySign' for signing of data, and 'PublicKeyVerify' for verification
   of signatures. Implementations of these interfaces are secure against
   adaptive chosen-message attacks. Signing data ensures the authenticity and
```

### Comparing `tink-1.6.1/tink/signature/_public_key_sign.py` & `tink-1.7.0/tink/signature/_public_key_sign.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,26 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Interface for PublicKeySign."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
-# Special imports
-import six
 
 
-@six.add_metaclass(abc.ABCMeta)
-class PublicKeySign(object):
+class PublicKeySign(metaclass=abc.ABCMeta):
   """Interface for public key signing.
 
   Digital Signatures provide functionality of signing data and verification of
   the signatures. They are represented by a pair of primitives (interfaces)
   'PublicKeySign' for signing of data, and 'PublicKeyVerify' for verification
   of signatures. Implementations of these interfaces are secure against
   adaptive chosen-message attacks. Signing data ensures the authenticity and
```

### Comparing `tink-1.6.1/tink/signature/_signature_wrapper_test.py` & `tink-1.7.0/tink/signature/_signature_wrapper_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.public_key_sign_wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 
 import tink
 from tink import signature
 from tink.testing import keyset_builder
```

### Comparing `tink-1.6.1/tink/signature/_signature_key_manager_test.py` & `tink-1.7.0/tink/signature/_signature_key_manager_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink._signature_key_manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 
 from tink.proto import common_pb2
 from tink.proto import ecdsa_pb2
 from tink.proto import tink_pb2
 import tink
@@ -32,16 +27,18 @@
 def setUpModule():
   signature.register()
 
 
 class PublicKeySignKeyManagerTest(parameterized.TestCase):
 
   def test_new_key_data_ecdsa(self):
-    template = signature.signature_key_templates.create_ecdsa_key_template(
-        common_pb2.SHA256, common_pb2.NIST_P256, ecdsa_pb2.DER)
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = signature.signature_key_templates.create_ecdsa_key_template(
+          common_pb2.SHA256, common_pb2.NIST_P256, ecdsa_pb2.DER)
     key_manager = core.Registry.key_manager(template.type_url)
     key_data = key_manager.new_key_data(template)
     self.assertEqual(key_data.type_url, template.type_url)
     key = ecdsa_pb2.EcdsaPrivateKey()
     key.ParseFromString(key_data.value)
     public_key = key.public_key
     self.assertEqual(key.version, 0)
@@ -61,19 +58,18 @@
     template.type_url = 'type.googleapis.com/google.crypto.tink.EcdsaPublicKey'
     template.value = key_format.SerializeToString()
     with self.assertRaises(core.TinkError):
       tink.new_keyset_handle(template)
 
   @parameterized.parameters([
       signature.signature_key_templates.ECDSA_P256,
-      signature.signature_key_templates.ECDSA_P384,
       signature.signature_key_templates.ECDSA_P384_SHA384,
+      signature.signature_key_templates.ECDSA_P384_SHA512,
       signature.signature_key_templates.ECDSA_P521,
       signature.signature_key_templates.ECDSA_P256_IEEE_P1363,
-      signature.signature_key_templates.ECDSA_P384_IEEE_P1363,
       signature.signature_key_templates.ECDSA_P384_SHA384_IEEE_P1363,
       signature.signature_key_templates.ECDSA_P521_IEEE_P1363,
       signature.signature_key_templates.ED25519,
       signature.signature_key_templates.RSA_SSA_PKCS1_3072_SHA256_F4,
       signature.signature_key_templates.RSA_SSA_PKCS1_4096_SHA512_F4,
       signature.signature_key_templates.RSA_SSA_PSS_3072_SHA256_SHA256_32_F4,
       signature.signature_key_templates.RSA_SSA_PSS_4096_SHA512_SHA512_64_F4,
```

### Comparing `tink-1.6.1/tink/_keyset_writer_test.py` & `tink-1.7.0/tink/_keyset_writer_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink._keyset_writer."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 
 from typing import cast
 from absl.testing import absltest
 
 from tink.proto import tink_pb2
 import tink
```

### Comparing `tink-1.6.1/tink/BUILD.bazel` & `tink-1.7.0/tink/BUILD.bazel`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 py_library(
     name = "_keyset_handle",
     srcs = ["_keyset_handle.py"],
     srcs_version = "PY3",
     deps = [
         ":_keyset_reader",
         ":_keyset_writer",
+        ":secret_key_access",
         requirement("protobuf"),
         "//tink/aead",
         "//tink/core",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
@@ -59,15 +60,14 @@
 
 py_library(
     name = "_keyset_reader",
     srcs = ["_keyset_reader.py"],
     srcs_version = "PY3",
     deps = [
         requirement("protobuf"),
-        requirement("six"),
         "//tink/core",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_keyset_reader_test",
@@ -83,15 +83,14 @@
 
 py_library(
     name = "_keyset_writer",
     srcs = ["_keyset_writer.py"],
     srcs_version = "PY3",
     deps = [
         requirement("protobuf"),
-        requirement("six"),
         "//tink/core",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_keyset_writer_test",
@@ -135,14 +134,35 @@
         "//tink/prf",
         "//tink/signature",
         "//tink/streaming_aead",
     ],
 )
 
 py_library(
+    name = "secret_key_access",
+    srcs = ["secret_key_access.py"],
+    srcs_version = "PY3",
+    deps = [
+        "//tink/core",
+    ],
+)
+
+py_test(
+    name = "secret_key_access_test",
+    srcs = ["secret_key_access_test.py"],
+    python_version = "PY3",
+    srcs_version = "PY3",
+    deps = [
+        ":secret_key_access",
+        ":tink_python",
+        requirement("absl-py"),
+    ],
+)
+
+py_library(
     name = "cleartext_keyset_handle",
     srcs = ["cleartext_keyset_handle.py"],
     srcs_version = "PY3",
     visibility = ["//visibility:public"],
     deps = [
         ":tink_python",
         "//tink/proto:tink_py_pb2",
```

### Comparing `tink-1.6.1/tink/cleartext_keyset_handle.py` & `tink-1.7.0/tink/cleartext_keyset_handle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,18 +15,14 @@
 
 WARNING
 
 Reading or writing cleartext keysets is a bad practice, usage of this API
 should be restricted. Users can read encrypted keysets using
 tink.read_keyset_handle.
 """
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
 from tink.proto import tink_pb2
 import tink
 
 
 def from_keyset(keyset: tink_pb2.Keyset) -> tink.KeysetHandle:
   """Create a KeysetHandle from a keyset."""
```

### Comparing `tink-1.6.1/tink/_keyset_writer.py` & `tink-1.7.0/tink/_keyset_writer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,32 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Writes Keysets to file."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
-
 from typing import BinaryIO, TextIO
-# Special imports
-import six
 
 from google.protobuf import json_format
 from tink.proto import tink_pb2
 from tink import core
 
 
-@six.add_metaclass(abc.ABCMeta)
-class KeysetWriter(object):
+class KeysetWriter(metaclass=abc.ABCMeta):
   """Knows how to write keysets to some storage system."""
 
   @abc.abstractmethod
   def write(self, keyset: tink_pb2.Keyset) -> None:
     """Tries to write a tink_pb2.Keyset to some storage system."""
     raise NotImplementedError()
 
@@ -54,29 +45,21 @@
   def __init__(self, text_io_stream: TextIO):
     self._io_stream = text_io_stream
 
   def write(self, keyset: tink_pb2.Keyset) -> None:
     if not isinstance(keyset, tink_pb2.Keyset):
       raise core.TinkError('invalid keyset.')
     json_keyset = json_format.MessageToJson(keyset)
-    # TODO(b/141106504) Needed for python 2.7 compatibility. StringIO expects
-    # unicode, but MessageToJson outputs UTF-8.
-    if isinstance(json_keyset, bytes):
-      json_keyset = json_keyset.decode('utf-8')
     self._io_stream.write(json_keyset)
     self._io_stream.flush()
 
   def write_encrypted(self, encrypted_keyset: tink_pb2.EncryptedKeyset) -> None:
     if not isinstance(encrypted_keyset, tink_pb2.EncryptedKeyset):
       raise core.TinkError('invalid encrypted keyset.')
     json_keyset = json_format.MessageToJson(encrypted_keyset)
-    # TODO(b/141106504) Needed for python 2.7 compatibility. StringIO expects
-    # unicode, but MessageToJson outputs UTF-8.
-    if isinstance(json_keyset, bytes):
-      json_keyset = json_keyset.decode('utf-8')
     self._io_stream.write(json_keyset)
     self._io_stream.flush()
 
 
 class BinaryKeysetWriter(KeysetWriter):
   """Writes keysets in proto binary wire format to some storage system.
```

### Comparing `tink-1.6.1/tink/core/_crypto_format.py` & `tink-1.7.0/tink/core/_crypto_format.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Constants and convenience methods for the outputs handled by Tink."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import struct
 
 from tink.proto import tink_pb2
 from tink.core import _tink_error
 
 TINK_START_BYTE = b'\x01'
 LEGACY_START_BYTE = b'\x00'
```

### Comparing `tink-1.6.1/tink/core/_primitive_set_test.py` & `tink-1.7.0/tink/core/_primitive_set_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.core.primitive_set."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from absl.testing import absltest
 from tink.proto import tink_pb2
 from tink import aead
 from tink import core
 from tink import mac
 from tink.testing import helper
```

### Comparing `tink-1.6.1/tink/core/_primitive_wrapper.py` & `tink-1.7.0/tink/core/_primitive_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,33 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Basic interface for wrapping a primitive."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 from typing import Generic, Type, TypeVar
-# Special imports
-import six
 
 from tink.core import _primitive_set
 
 
 B = TypeVar('B')
 P = TypeVar('P')
 
 
-@six.add_metaclass(abc.ABCMeta)
-class PrimitiveWrapper(Generic[B, P]):
+class PrimitiveWrapper(Generic[B, P], metaclass=abc.ABCMeta):
   """Basic interface for wrapping a primitive.
 
   A PrimitiveSet can be wrapped by a single primitive in order to fulfill a
   cryptographic task. This is done by the PrimitiveWrapper. Whenever a new
   primitive type is added to Tink, the user should define a new PrimitiveWrapper
   and register it by calling registry.registerPrimitiveWrapper().
```

### Comparing `tink-1.6.1/tink/core/_tink_error.py` & `tink-1.7.0/tink/core/_tink_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,21 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module defines basic exceptions in Tink."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from tink.cc.pybind import tink_bindings
 
-KNOWN_STATUS_NOT_OK_TYPES = (tink_bindings.StatusNotOk,)
+KNOWN_STATUS_NOT_OK_TYPES = (tink_bindings.PythonTinkException,)
 
 
 def register_status_not_ok_type(status_not_ok_type):
   global KNOWN_STATUS_NOT_OK_TYPES
   if status_not_ok_type not in KNOWN_STATUS_NOT_OK_TYPES:
     assert issubclass(status_not_ok_type, Exception)
     KNOWN_STATUS_NOT_OK_TYPES += (status_not_ok_type,)
```

### Comparing `tink-1.6.1/tink/core/_primitive_set.py` & `tink-1.7.0/tink/core/_primitive_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A container class for a set of primitives."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import collections
 from typing import Generic, List, Type, TypeVar
 
 from tink.proto import tink_pb2
 from tink.core import _crypto_format
 from tink.core import _tink_error
```

### Comparing `tink-1.6.1/tink/core/BUILD.bazel` & `tink-1.7.0/tink/core/BUILD.bazel`

 * *Files 2% similar despite different names*

```diff
@@ -117,10 +117,9 @@
 
 py_library(
     name = "_primitive_wrapper",
     srcs = ["_primitive_wrapper.py"],
     srcs_version = "PY3",
     deps = [
         ":_primitive_set",
-        requirement("six"),
     ],
 )
```

### Comparing `tink-1.6.1/tink/core/__init__.py` & `tink-1.7.0/tink/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Core package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
 from tink.proto import tink_pb2
 from tink.core import _crypto_format
 from tink.core import _key_manager
 from tink.core import _primitive_set
 from tink.core import _primitive_wrapper
 from tink.core import _registry
@@ -39,7 +35,12 @@
 use_tink_errors = _tink_error.use_tink_errors
 
 new_primitive_set = _primitive_set.new_primitive_set
 PrimitiveSet = _primitive_set.PrimitiveSet
 PrimitiveWrapper = _primitive_wrapper.PrimitiveWrapper
 
 crypto_format = _crypto_format
+
+
+class KeyAccess:
+  """Base class for access tokens for Tink Keys."""
+  pass
```

### Comparing `tink-1.6.1/tink/core/_registry.py` & `tink-1.7.0/tink/core/_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,65 +10,60 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tink Registry."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
-from typing import Any, Text, Tuple, Type, TypeVar
+from typing import Any, Tuple, Type, TypeVar
 
 from tink.proto import tink_pb2
 from tink.core import _key_manager
 from tink.core import _primitive_set
 from tink.core import _primitive_wrapper
 from tink.core import _tink_error
 
 P = TypeVar('P')
 
 
-class Registry(object):
+class Registry:
   """A global container of key managers.
 
   Registry maps supported key types to a corresponding KeyManager object,
   which 'understands' the key type (i.e., the KeyManager can instantiate the
   primitive corresponding to given key, or can generate new keys of the
   supported key type). Keeping KeyManagers for all primitives in a single
   Registry (rather than having a separate KeyManager per primitive) enables
   modular construction of compound primitives from 'simple' ones,
   e.g., AES-CTR-HMAC AEAD encryption uses IND-CPA encryption and a MAC.
 
   Registry is initialized at startup, and is later used to instantiate
   primitives for given keys or keysets.
   """
 
-  _key_managers = {}  # type: dict[Text, Tuple[_key_manager.KeyManager, bool]]
+  _key_managers = {}  # type: dict[str, Tuple[_key_manager.KeyManager, bool]]
   _wrappers = {}  # type: dict[Type, _primitive_wrapper.PrimitiveWrapper]
 
   @classmethod
   def reset(cls) -> None:
     """Resets the registry."""
     cls._key_managers = {}
     cls._wrappers = {}
 
   @classmethod
   def _key_manager_internal(
-      cls, type_url: Text) -> Tuple[_key_manager.KeyManager, bool]:
+      cls, type_url: str) -> Tuple[_key_manager.KeyManager, bool]:
     """Returns a key manager, new_key_allowed pair for the given type_url."""
     if type_url not in cls._key_managers:
       raise _tink_error.TinkError(
           'No manager for type {} has been registered.'.format(type_url))
     return cls._key_managers[type_url]
 
   @classmethod
-  def key_manager(cls, type_url: Text) -> _key_manager.KeyManager:
+  def key_manager(cls, type_url: str) -> _key_manager.KeyManager:
     """Returns a key manager for the given type_url and primitive_class.
 
     Args:
       type_url: Key type string
 
     Returns:
       A KeyManager object
```

### Comparing `tink-1.6.1/tink/core/_crypto_format_test.py` & `tink-1.7.0/tink/core/_crypto_format_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.crypto_format."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from tink.proto import tink_pb2
 from tink import core
 
 
 def to_byte(c):
   # items in byte strings are of type str in Python v2.7 and int in v3.5
```

### Comparing `tink-1.6.1/tink/core/_registry_test.py` & `tink-1.7.0/tink/core/_registry_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,17 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.registry."""
 
-# Placeholder for import for type annotations
-
-from typing import cast, Mapping, Type, TypeVar, Text
+from typing import cast, Mapping, Type, TypeVar
 from absl.testing import absltest
 
 from tink.proto import tink_pb2
 
 from tink import aead
 from tink import core
 from tink import hybrid
@@ -32,53 +30,53 @@
 
 
 P = TypeVar('P')
 
 
 class DummyKeyManager(core.KeyManager[P]):
 
-  def __init__(self, type_url: Text, primitive_class: Type[P] = aead.Aead):
+  def __init__(self, type_url: str, primitive_class: Type[P] = aead.Aead):
     self._type_url = type_url
     self._primitive_class = primitive_class
 
   def primitive_class(self) -> Type[P]:
     return self._primitive_class
 
   def primitive(self, key_data: tink_pb2.KeyData) -> P:
     return helper.FakeAead()
 
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     return self._type_url
 
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     return tink_pb2.KeyData(type_url=key_template.type_url)
 
-  def does_support(self, type_url: Text) -> bool:
+  def does_support(self, type_url: str) -> bool:
     return self.key_type() == type_url
 
 
 class UnsupportedKeyManager(DummyKeyManager[P]):
 
-  def does_support(self, type_url: Text) -> bool:
+  def does_support(self, type_url: str) -> bool:
     return False
 
 
 class DummyPrivateKeyManager(core.PrivateKeyManager[hybrid.HybridDecrypt]):
 
-  def __init__(self, type_url: Text):
+  def __init__(self, type_url: str):
     self._type_url = type_url
 
   def primitive_class(self) -> Type[hybrid.HybridDecrypt]:
     return hybrid.HybridDecrypt
 
   def primitive(self, key_data: tink_pb2.KeyData) -> hybrid.HybridDecrypt:
     return helper.FakeHybridDecrypt()
 
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     return self._type_url
 
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     return tink_pb2.KeyData()
 
   def public_key_data(
@@ -177,15 +175,15 @@
             helper.fake_key(key_id=i, output_prefix_type=tink_pb2.RAW)))
   return mac_set
 
 
 class RegistryTest(absltest.TestCase):
 
   def setUp(self):
-    super(RegistryTest, self).setUp()
+    super().setUp()
     self.reg = core.Registry()
     self.reg.reset()
 
   def test_key_manager_no_exist(self):
     with self.assertRaises(core.TinkError):
       self.reg.key_manager('invalid')
```

### Comparing `tink-1.6.1/tink/core/_key_manager.py` & `tink-1.7.0/tink/core/_key_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module defines the basic types and abstract classes in Tink."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
 import abc
-from typing import Any, Generic, Text, Type, TypeVar
-import six
+from typing import Any, Generic, Type, TypeVar
 
 from tink.proto import tink_pb2
 from tink.core import _tink_error
 
 
 P = TypeVar('P')
 
 
-@six.add_metaclass(abc.ABCMeta)
-class KeyManager(Generic[P]):
+class KeyManager(Generic[P], metaclass=abc.ABCMeta):
   """Generates keys and provides primitives for the keys.
 
   A KeyManager "understands" keys of a specific key types: it can generate keys
   of a supported type and create primitives for supported keys.  A key type is
   identified by the global name of the protocol buffer that holds the
   corresponding key material, and is given by type_url-field of KeyData-protocol
   buffer.
@@ -55,15 +49,15 @@
       A primitive, for example an instance of Aead or Mac.
     Raises:
       tink.TinkError if getting the primitive fails.
     """
     raise NotImplementedError()
 
   @abc.abstractmethod
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     """Returns the type_url identifying the key type handled by this manager."""
     raise NotImplementedError()
 
   @abc.abstractmethod
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     """Generates a new random key, based on the specified key_template.
@@ -73,15 +67,15 @@
     Returns:
       A KeyData protocol buffer that contains the key.
     Raises:
       tink.TinkError if the key generation fails.
     """
     raise NotImplementedError()
 
-  def does_support(self, type_url: Text) -> bool:
+  def does_support(self, type_url: str) -> bool:
     return self.key_type() == type_url
 
 
 class PrivateKeyManager(KeyManager[P]):
   """Generates keys and provides primitives for the keys."""
 
   @abc.abstractmethod
@@ -114,15 +108,15 @@
     return self._primitive_class
 
   @_tink_error.use_tink_errors
   def primitive(self, key_data: tink_pb2.KeyData) -> P:
     return self._primitive_py_wrapper(
         self._cc_key_manager.primitive(key_data.SerializeToString()))
 
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     return self._cc_key_manager.key_type()
 
   @_tink_error.use_tink_errors
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     return tink_pb2.KeyData.FromString(
         self._cc_key_manager.new_key_data(key_template.SerializeToString()))
@@ -143,15 +137,15 @@
     return self._primitive_class
 
   @_tink_error.use_tink_errors
   def primitive(self, key_data: tink_pb2.KeyData) -> P:
     return self._primitive_py_wrapper(
         self._cc_key_manager.primitive(key_data.SerializeToString()))
 
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     return self._cc_key_manager.key_type()
 
   @_tink_error.use_tink_errors
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     return tink_pb2.KeyData.FromString(
         self._cc_key_manager.new_key_data(key_template.SerializeToString()))
```

### Comparing `tink-1.6.1/tink/proto/ecdsa.proto` & `tink-1.7.0/tink/proto/ecdsa.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/aes_siv.proto` & `tink-1.7.0/tink/proto/aes_siv.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/aes_gcm_hkdf_streaming.proto` & `tink-1.7.0/tink/proto/aes_gcm_hkdf_streaming.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/cached_dek_envelope.proto` & `tink-1.7.0/tink/proto/cached_dek_envelope.proto`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC.
+// Copyright 2021 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `tink-1.6.1/tink/proto/empty_pb2.py` & `tink-1.7.0/tink/proto/empty_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: tink/proto/empty.proto
-
+"""Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='tink/proto/empty.proto',
-  package='google.crypto.tink',
-  syntax='proto3',
-  serialized_options=b'\n\034com.google.crypto.tink.protoP\001Z+github.com/google/tink/proto/empty_go_proto',
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x16tink/proto/empty.proto\x12\x12google.crypto.tink\"\x07\n\x05\x45mptyBM\n\x1c\x63om.google.crypto.tink.protoP\x01Z+github.com/google/tink/proto/empty_go_protob\x06proto3'
-)
-
-
-
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16tink/proto/empty.proto\x12\x12google.crypto.tink\"\x07\n\x05\x45mptyBM\n\x1c\x63om.google.crypto.tink.protoP\x01Z+github.com/google/tink/proto/empty_go_protob\x06proto3')
 
-_EMPTY = _descriptor.Descriptor(
-  name='Empty',
-  full_name='google.crypto.tink.Empty',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=46,
-  serialized_end=53,
-)
 
-DESCRIPTOR.message_types_by_name['Empty'] = _EMPTY
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
+_EMPTY = DESCRIPTOR.message_types_by_name['Empty']
 Empty = _reflection.GeneratedProtocolMessageType('Empty', (_message.Message,), {
   'DESCRIPTOR' : _EMPTY,
   '__module__' : 'tink.proto.empty_pb2'
   # @@protoc_insertion_point(class_scope:google.crypto.tink.Empty)
   })
 _sym_db.RegisterMessage(Empty)
 
+if _descriptor._USE_C_DESCRIPTORS == False:
 
-DESCRIPTOR._options = None
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\034com.google.crypto.tink.protoP\001Z+github.com/google/tink/proto/empty_go_proto'
+  _EMPTY._serialized_start=46
+  _EMPTY._serialized_end=53
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tink-1.6.1/tink/proto/jwt_hmac.proto` & `tink-1.7.0/tink/proto/jwt_hmac.proto`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 
 package google.crypto.tink;
 
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
 option go_package = "github.com/google/tink/proto/jwt_hmac_go_proto";
 
+// See https://datatracker.ietf.org/doc/html/rfc7518#section-3.2
 enum JwtHmacAlgorithm {
   HS_UNKNOWN = 0;
-  HS256 = 1;
-  HS384 = 2;
-  HS512 = 3;
+  HS256 = 1;  // HMAC using SHA-256
+  HS384 = 2;  // HMAC using SHA-384
+  HS512 = 3;  // HMAC using SHA-512
 }
 
 // key_type: type.googleapis.com/google.crypto.tink.JwtHmacKey
 message JwtHmacKey {
   uint32 version = 1;
   JwtHmacAlgorithm algorithm = 2;
   bytes key_value = 3;
```

### Comparing `tink-1.6.1/tink/proto/rsa_ssa_pss.proto` & `tink-1.7.0/tink/proto/rsa_ssa_pss.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/empty.proto` & `tink-1.7.0/tink/proto/empty.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/chacha20_poly1305.proto` & `tink-1.7.0/tink/proto/chacha20_poly1305.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/aes_ctr.proto` & `tink-1.7.0/tink/proto/aes_ctr.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/jwt_ecdsa.proto` & `tink-1.7.0/tink/proto/jwt_ecdsa.proto`

 * *Files 16% similar despite different names*

```diff
@@ -18,25 +18,28 @@
 
 package google.crypto.tink;
 
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
 option go_package = "github.com/google/tink/proto/jwt_ecdsa_go_proto";
 
+// See https://datatracker.ietf.org/doc/html/rfc7518#section-3.4
 enum JwtEcdsaAlgorithm {
   ES_UNKNOWN = 0;
-  ES256 = 1;
-  ES384 = 2;
-  ES512 = 3;
+  ES256 = 1;  // ECDSA using P-256 and SHA-256
+  ES384 = 2;  // ECDSA using P-384 and SHA-384
+  ES512 = 3;  // ECDSA using P-521 and SHA-512
 }
 
 // key_type: type.googleapis.com/google.crypto.tink.JwtEcdsaPublicKey
 message JwtEcdsaPublicKey {
   uint32 version = 1;
   JwtEcdsaAlgorithm algorithm = 2;
+  // Affine coordinates of the public key in big-endian representation. The
+  // public key is a point (x, y) on the curve defined by algorithm.
   bytes x = 3;
   bytes y = 4;
 
   // Optional, custom kid header value to be used with "RAW" keys.
   // "TINK" keys with this value set will be rejected.
   message CustomKid {
     string value = 1;
```

### Comparing `tink-1.6.1/tink/proto/kms_aead.proto` & `tink-1.7.0/tink/proto/kms_aead.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/test_proto.proto` & `tink-1.7.0/tink/proto/xchacha20_poly1305.proto`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-// Copyright 2021 Google LLC
+// Copyright 2018 Google Inc.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ////////////////////////////////////////////////////////////////////////////////
+
 syntax = "proto3";
 
 package google.crypto.tink;
 
-message TestProto {
-  uint64 num = 1;
-  bytes str = 2;  // placeholder for ctype
+option java_package = "com.google.crypto.tink.proto";
+option java_multiple_files = true;
+option go_package = "github.com/google/tink/proto/xchacha20_poly1305_go_proto";
+
+message XChaCha20Poly1305KeyFormat {
+  uint32 version = 1;
 }
 
-message NestedTestProto {
-  TestProto a = 1;
-  TestProto b = 2;
-  uint64 num = 3;
-  bytes str = 4;  // placeholder for ctype
+// key_type: type.googleapis.com/google.crypto.tink.XChaCha20Poly1305Key
+message XChaCha20Poly1305Key {
+  uint32 version = 1;
+  bytes key_value = 3;
 }
```

### Comparing `tink-1.6.1/tink/proto/config.proto` & `tink-1.7.0/tink/proto/config.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/aes_gcm_siv.proto` & `tink-1.7.0/tink/proto/aes_gcm_siv.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/common.proto` & `tink-1.7.0/tink/proto/common.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/ed25519.proto` & `tink-1.7.0/tink/proto/ed25519.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/BUILD.bazel` & `tink-1.7.0/tink/proto/BUILD.bazel`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,22 @@
     deps = [
         ":common_py_pb2",
         ":tink_py_pb2",
     ],
 )
 
 py_proto_library(
+    name = "hpke_py_pb2",
+    srcs = [
+        "hpke.proto",
+    ],
+    visibility = ["//visibility:public"],
+)
+
+py_proto_library(
     name = "xchacha20_poly1305_py_pb2",
     srcs = [
         "xchacha20_poly1305.proto",
     ],
     visibility = ["//visibility:public"],
 )
```

### Comparing `tink-1.6.1/tink/proto/hmac_prf.proto` & `tink-1.7.0/tink/proto/hmac_prf.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/__init__.py` & `tink-1.7.0/tink/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/experimental/pqcrypto/cecpq2_aead_hkdf.proto` & `tink-1.7.0/tink/proto/ecies_aead_hkdf.proto`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,113 @@
-// Copyright 2021 Google LLC
+// Copyright 2017 Google Inc.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ////////////////////////////////////////////////////////////////////////////////
+
+// Definitions for Elliptic Curve Digital Signature Algorithm (ECDSA).
 syntax = "proto3";
 
 package google.crypto.tink;
 
-import "proto/common.proto";
-import "proto/tink.proto";
+import "tink/proto/common.proto";
+import "tink/proto/tink.proto";
 
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
-option go_package = "github.com/google/tink/proto/cecpq2_aead_hkdf_go_proto";
+option go_package = "github.com/google/tink/proto/ecies_aead_hkdf_go_proto";
 
-// Protos for keys for CECPQ2 with HKDF and AEAD encryption.
+// Protos for keys for ECIES with HKDF and AEAD encryption.
 //
 // These definitions follow loosely ECIES ISO 18033-2 standard
 // (Elliptic Curve Integrated Encryption Scheme, see
 // http://www.shoup.net/iso/std6.pdf), with but with some differences:
-//  * use of CECPQ2 as the KEM instead of ECC-only KEM
 //  * use of HKDF key derivation function (instead of KDF1 and KDF2) enabling
 //  the use
 //    of optional parameters to the key derivation function, which strenghten
 //    the overall security and allow for binding the key material to
 //    application-specific information (cf. RFC 5869,
 //    https://tools.ietf.org/html/rfc5869)
 //  * use of modern AEAD schemes rather than "manual composition" of symmetric
 //  encryption
 //    with message authentication codes (as in DEM1, DEM2, and DEM3 schemes of
 //    ISO 18033-2)
 //
-// CECPQ2-keys represent HybridEncryption resp. HybridDecryption primitives.
+// ECIES-keys represent HybridEncryption resp. HybridDecryption primitives.
 
 // Parameters of KEM (Key Encapsulation Mechanism)
-message Cecpq2HkdfKemParams {
+message EciesHkdfKemParams {
   // Required.
   EllipticCurveType curve_type = 1;
 
   // Required.
-  EcPointFormat ec_point_format = 2;
-
-  // Required.
-  HashType hkdf_hash_type = 3;
+  HashType hkdf_hash_type = 2;
 
   // Optional.
   bytes hkdf_salt = 11;
 }
 
 // Parameters of AEAD DEM (Data Encapsulation Mechanism).
-message Cecpq2AeadDemParams {
-  // Contains e.g. AesCtrHmacAeadKeyFormat or AesGcmKeyFormat.
+message EciesAeadDemParams {
   // Required.
+  // Contains an Aead or DeterministicAead key format (e.g:
+  // AesCtrHmacAeadKeyFormat, AesGcmKeyFormat or AesSivKeyFormat).
   KeyTemplate aead_dem = 2;
 }
 
-message Cecpq2AeadHkdfParams {
+message EciesAeadHkdfParams {
   // Key Encapsulation Mechanism.
   // Required.
-  Cecpq2HkdfKemParams kem_params = 1;
+  EciesHkdfKemParams kem_params = 1;
 
   // Data Encapsulation Mechanism.
   // Required.
-  Cecpq2AeadDemParams dem_params = 2;
-}
+  EciesAeadDemParams dem_params = 2;
 
-// Cecpq2AeadHkdfPublicKey represents HybridEncryption primitive.
-// key_type: type.googleapis.com/google.crypto.tink.Cecpq2AeadHkdfPublicKey
-message Cecpq2AeadHkdfPublicKey {
-  // Required.
-  uint32 version = 1;
+  // EC point format.
   // Required.
-  Cecpq2AeadHkdfParams params = 2;
+  EcPointFormat ec_point_format = 3;
+}
 
-  // X25519 public key: Affine coordinates of the public key in bigendian
-  // representation. The public key is a point (x, y) on the Curve25519.
+// EciesAeadHkdfPublicKey represents HybridEncryption primitive.
+// key_type: type.googleapis.com/google.crypto.tink.EciesAeadHkdfPublicKey
+message EciesAeadHkdfPublicKey {
   // Required.
-  bytes x25519_public_key_x = 3;
+  uint32 version = 1;
   // Required.
-  bytes x25519_public_key_y = 4;
+  EciesAeadHkdfParams params = 2;
 
-  // HRSS public key:
+  // Affine coordinates of the public key in bigendian representation.
+  // The public key is a point (x, y) on the curve defined by
+  // params.kem_params.curve. Required.
+  bytes x = 3;
   // Required.
-  bytes hrss_public_key_marshalled = 5;
+  bytes y = 4;
 }
 
-// Cecpq2KdfAeadPrivateKey represents HybridDecryption primitive.
-// key_type: type.googleapis.com/google.crypto.tink.Cecpq2AeadHkdfPrivateKey
-message Cecpq2AeadHkdfPrivateKey {
+// EciesKdfAeadPrivateKey represents HybridDecryption primitive.
+// key_type: type.googleapis.com/google.crypto.tink.EciesAeadHkdfPrivateKey
+message EciesAeadHkdfPrivateKey {
   // Required.
   uint32 version = 1;
 
   // Required.
-  Cecpq2AeadHkdfPublicKey public_key = 2;
-
-  // X25519 private key:
-  // Required.
-  bytes x25519_private_key = 3;  // Big integer in bigendian representation.
+  EciesAeadHkdfPublicKey public_key = 2;
 
-  // HRSS private key seed:
   // Required.
-  bytes hrss_private_key_seed = 4;
+  bytes key_value = 3;  // Big integer in bigendian representation.
 }
 
-message Cecpq2AeadHkdfKeyFormat {
+message EciesAeadHkdfKeyFormat {
   // Required.
-  Cecpq2AeadHkdfParams params = 1;
+  EciesAeadHkdfParams params = 1;
 }
```

### Comparing `tink-1.6.1/tink/proto/aes_ctr_hmac_streaming.proto` & `tink-1.7.0/tink/proto/aes_ctr_hmac_streaming.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/hpke.proto` & `tink-1.7.0/tink/proto/hmac.proto`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC
+// Copyright 2017 Google Inc.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -14,53 +14,30 @@
 //
 ////////////////////////////////////////////////////////////////////////////////
 
 syntax = "proto3";
 
 package google.crypto.tink;
 
+import "tink/proto/common.proto";
+
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
-option go_package = "github.com/google/tink/proto/hpke_proto";
-
-enum HpkeKem {
-  KEM_UNKNOWN = 0;
-  DHKEM_X25519_HKDF_SHA256 = 1;
-}
-
-enum HpkeKdf {
-  KDF_UNKNOWN = 0;
-  HKDF_SHA256 = 1;
-}
+option go_package = "github.com/google/tink/proto/hmac_go_proto";
 
-enum HpkeAead {
-  AEAD_UNKNOWN = 0;
-  AES_128_GCM = 1;
-  AES_256_GCM = 2;
-  CHACHA20_POLY1305 = 3;
-}
-
-message HpkeParams {
-  HpkeKem kem = 1;
-  HpkeKdf kdf = 2;
-  HpkeAead aead = 3;
-}
-
-message HpkePublicKey {
-  uint32 version = 1;
-  HpkeParams params = 2;
-  // KEM-encoding of public key (i.e., SerializePublicKey() ) as described in
-  // https://www.ietf.org/archive/id/draft-irtf-cfrg-hpke-09.html#name-cryptographic-dependencies.
-  bytes public_key = 3;
+message HmacParams {
+  HashType hash = 1;  // HashType is an enum.
+  uint32 tag_size = 2;
 }
 
-message HpkePrivateKey {
+// key_type: type.googleapis.com/google.crypto.tink.HmacKey
+message HmacKey {
   uint32 version = 1;
-  HpkePublicKey public_key = 2;
-  // KEM-encoding of private key (i.e., SerializePrivateKey() ) as described in
-  // https://www.ietf.org/archive/id/draft-irtf-cfrg-hpke-09.html#name-cryptographic-dependencies.
-  bytes private_key = 3;
+  HmacParams params = 2;
+  bytes key_value = 3;
 }
 
-message HpkeKeyFormat {
-  HpkeParams params = 1;
+message HmacKeyFormat {
+  HmacParams params = 1;
+  uint32 key_size = 2;
+  uint32 version = 3;
 }
```

### Comparing `tink-1.6.1/tink/proto/jwt_rsa_ssa_pss.proto` & `tink-1.7.0/tink/proto/jwt_rsa_ssa_pkcs1.proto`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2018 Google Inc.
+// Copyright 2020 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -16,67 +16,68 @@
 
 syntax = "proto3";
 
 package google.crypto.tink;
 
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
-option go_package = "github.com/google/tink/proto/jwt_rsa_ssa_pss_go_proto";
+option go_package = "github.com/google/tink/proto/rsa_ssa_pkcs1_go_proto";
 
-enum JwtRsaSsaPssAlgorithm {
-  PS_UNKNOWN = 0;
-  PS256 = 1;
-  PS384 = 2;
-  PS512 = 3;
+// See https://datatracker.ietf.org/doc/html/rfc7518#section-3.3
+enum JwtRsaSsaPkcs1Algorithm {
+  RS_UNKNOWN = 0;
+  RS256 = 1;  // RSASSA-PKCS1-v1_5 using SHA-256
+  RS384 = 2;  // RSASSA-PKCS1-v1_5 using SHA-384
+  RS512 = 3;  // RSASSA-PKCS1-v1_5 using SHA-512
 }
 
-// key_type: type.googleapis.com/google.crypto.tink.JwtRsaSsaPssPublicKey
-message JwtRsaSsaPssPublicKey {
+// key_type: type.googleapis.com/google.crypto.tink.JwtRsaSsaPkcs1PublicKey
+message JwtRsaSsaPkcs1PublicKey {
   uint32 version = 1;
-  JwtRsaSsaPssAlgorithm algorithm = 2;
+  JwtRsaSsaPkcs1Algorithm algorithm = 2;
   // Modulus.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes n = 3;
   // Public exponent.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes e = 4;
 
   // Optional, custom kid header value to be used with "RAW" keys.
   // "TINK" keys with this value set will be rejected.
   message CustomKid {
     string value = 1;
   }
   CustomKid custom_kid = 5;
 }
 
-// key_type: type.googleapis.com/google.crypto.tink.JwtRsaSsaPssPrivateKey
-message JwtRsaSsaPssPrivateKey {
+// key_type: type.googleapis.com/google.crypto.tink.RsaSsaPkcs1PrivateKey
+message JwtRsaSsaPkcs1PrivateKey {
   uint32 version = 1;
-  JwtRsaSsaPssPublicKey public_key = 2;
+  JwtRsaSsaPkcs1PublicKey public_key = 2;
   // Private exponent.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes d = 3;
 
   // The following parameters are used to optimize RSA signature computation.
   // The prime factor p of n.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes p = 4;
   // The prime factor q of n.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes q = 5;
   // d mod (p - 1).
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes dp = 6;
   // d mod (q - 1).
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes dq = 7;
   // Chinese Remainder Theorem coefficient q^(-1) mod p.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes crt = 8;
 }
 
-message JwtRsaSsaPssKeyFormat {
+message JwtRsaSsaPkcs1KeyFormat {
   uint32 version = 1;
-  JwtRsaSsaPssAlgorithm algorithm = 2;
+  JwtRsaSsaPkcs1Algorithm algorithm = 2;
   uint32 modulus_size_in_bits = 3;
   bytes public_exponent = 4;
 }
```

### Comparing `tink-1.6.1/tink/proto/cached_dek_aead.proto` & `tink-1.7.0/tink/proto/cached_dek_aead.proto`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2021 Google LLC.
+// Copyright 2021 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
```

### Comparing `tink-1.6.1/tink/proto/tink.proto` & `tink-1.7.0/tink/proto/tink.proto`

 * *Files 3% similar despite different names*

```diff
@@ -90,38 +90,37 @@
   TINK = 1;
   LEGACY = 2;
   RAW = 3;
   CRUNCHY = 4;
 }
 
 // Each *Key proto by convention contains a version field, which
-// identifies the version of implementation that can work with this key.
+// identifies the version of the key.
 //   message SomeInstantiationKey {
 //     uint32 version = 1;
 //     ...
 //   }
-// Version is a monotonic counter: each implementation of a primitive
-// has its associated "current version", which starts at 0 and is incremented
-// upon updates of the code/key proto.  A key with version n needs
-// an implementation version n or higher to work.
+// If a key type does not mention anything else, only version 0 is currently
+// specified. An implementation must only accept keys with versions it knows,
+// and must reject all keys with unknown version.
 
 // For public key primitives, the public and private keys are distinct entities
 // and represent distinct primitives.  However, by convention, the private key
 // of a public-key primitive contains the corresponding public key proto.
 
 // The actual *Key-proto is wrapped in a KeyData message, which in addition
 // to this serialized proto contains also type_url identifying the
 // definition of *Key-proto (as in KeyFormat-message), and some extra metadata
 // about the type key material.
 message KeyData {
   // Required.
   string type_url = 1;  // In format type.googleapis.com/packagename.messagename
   // Required.
   // Contains specific serialized *Key proto
-  bytes value = 2;  // placeholder for ctype
+  bytes value = 2;  // Placeholder for ctype.
   enum KeyMaterialType {
     UNKNOWN_KEYMATERIAL = 0;
     SYMMETRIC = 1;
     ASYMMETRIC_PRIVATE = 2;
     ASYMMETRIC_PUBLIC = 3;
     REMOTE = 4;  // points to a remote key, i.e., in a KMS.
   }
```

### Comparing `tink-1.6.1/tink/proto/aes_cmac_prf.proto` & `tink-1.7.0/tink/proto/hkdf_prf.proto`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2020 Google LLC
+// Copyright 2019 Google LLC
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -14,21 +14,31 @@
 //
 ////////////////////////////////////////////////////////////////////////////////
 
 syntax = "proto3";
 
 package google.crypto.tink;
 
+import "tink/proto/common.proto";
+
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
-option go_package = "github.com/google/tink/proto/aes_cmac_prf_go_proto";
+option go_package = "github.com/google/tink/proto/hkdf_prf_proto";
+
+message HkdfPrfParams {
+  HashType hash = 1;
+  // Salt, optional in RFC 5869. Using "" is equivalent to zeros of length up to
+  // the block length of the HMac.
+  bytes salt = 2;
+}
 
-// key_type: type.googleapis.com/google.crypto.tink.AesCmacPrfKey
-message AesCmacPrfKey {
+message HkdfPrfKey {
   uint32 version = 1;
-  bytes key_value = 2;
+  HkdfPrfParams params = 2;
+  bytes key_value = 3;
 }
 
-message AesCmacPrfKeyFormat {
-  uint32 version = 2;
-  uint32 key_size = 1;
+message HkdfPrfKeyFormat {
+  HkdfPrfParams params = 1;
+  uint32 key_size = 2;
+  uint32 version = 3;
 }
```

### Comparing `tink-1.6.1/tink/proto/prf_based_deriver.proto` & `tink-1.7.0/tink/proto/prf_based_deriver.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/aes_cmac.proto` & `tink-1.7.0/tink/proto/aes_cmac.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/kms_envelope.proto` & `tink-1.7.0/tink/proto/kms_envelope.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/aes_ctr_hmac_aead.proto` & `tink-1.7.0/tink/proto/aes_ctr_hmac_aead.proto`

 * *Files identical despite different names*

### Comparing `tink-1.6.1/tink/proto/aes_gcm.proto` & `tink-1.7.0/tink/proto/aes_eax.proto`

 * *Files 20% similar despite different names*

```diff
@@ -16,21 +16,26 @@
 
 syntax = "proto3";
 
 package google.crypto.tink;
 
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
-option go_package = "github.com/google/tink/proto/aes_gcm_go_proto";
+option go_package = "github.com/google/tink/proto/aes_eax_go_proto";
 
-// only allowing IV size in bytes = 12 and tag size in bytes = 16
-// Thus, accept no params.
-message AesGcmKeyFormat {
+// only allowing tag size in bytes = 16
+message AesEaxParams {
+  // possible value is 12 or 16 bytes.
+  uint32 iv_size = 1;
+}
+
+message AesEaxKeyFormat {
+  AesEaxParams params = 1;
   uint32 key_size = 2;
-  uint32 version = 3;
 }
 
-// key_type: type.googleapis.com/google.crypto.tink.AesGcmKey
-message AesGcmKey {
+// key_type: type.googleapis.com/google.crypto.tink.AesEaxKey
+message AesEaxKey {
   uint32 version = 1;
+  AesEaxParams params = 2;
   bytes key_value = 3;
 }
```

### Comparing `tink-1.6.1/tink/proto/jwt_rsa_ssa_pkcs1.proto` & `tink-1.7.0/tink/proto/rsa_ssa_pkcs1.proto`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-// Copyright 2020 Google LLC
+// Copyright 2018 Google Inc.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
 //
 //      http://www.apache.org/licenses/LICENSE-2.0
 //
@@ -10,73 +10,82 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ////////////////////////////////////////////////////////////////////////////////
 
+// Definitions for RSA SSA (Signature Schemes with Appendix) using PKCS1-v1_5
+// encoding (https://tools.ietf.org/html/rfc8017#section-8.2).
 syntax = "proto3";
 
 package google.crypto.tink;
 
+import "tink/proto/common.proto";
+
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
 option go_package = "github.com/google/tink/proto/rsa_ssa_pkcs1_go_proto";
 
-enum JwtRsaSsaPkcs1Algorithm {
-  RS_UNKNOWN = 0;
-  RS256 = 1;
-  RS384 = 2;
-  RS512 = 3;
+message RsaSsaPkcs1Params {
+  // Hash function used in computing hash of the signing message
+  // (see https://tools.ietf.org/html/rfc8017#section-9.2).
+  // Required.
+  HashType hash_type = 1;
 }
 
-// key_type: type.googleapis.com/google.crypto.tink.JwtRsaSsaPkcs1PublicKey
-message JwtRsaSsaPkcs1PublicKey {
+// key_type: type.googleapis.com/google.crypto.tink.RsaSsaPkcs1PublicKey
+message RsaSsaPkcs1PublicKey {
+  // Required.
   uint32 version = 1;
-  JwtRsaSsaPkcs1Algorithm algorithm = 2;
+  // Required.
+  RsaSsaPkcs1Params params = 2;
   // Modulus.
   // Unsigned big integer in bigendian representation.
   bytes n = 3;
   // Public exponent.
   // Unsigned big integer in bigendian representation.
   bytes e = 4;
-
-  // Optional, custom kid header value to be used with "RAW" keys.
-  // "TINK" keys with this value set will be rejected.
-  message CustomKid {
-    string value = 1;
-  }
-  CustomKid custom_kid = 5;
 }
 
 // key_type: type.googleapis.com/google.crypto.tink.RsaSsaPkcs1PrivateKey
-message JwtRsaSsaPkcs1PrivateKey {
+message RsaSsaPkcs1PrivateKey {
+  // Required.
   uint32 version = 1;
-  JwtRsaSsaPkcs1PublicKey public_key = 2;
+  // Required.
+  RsaSsaPkcs1PublicKey public_key = 2;
   // Private exponent.
   // Unsigned big integer in bigendian representation.
+  // Required.
   bytes d = 3;
 
   // The following parameters are used to optimize RSA signature computation.
   // The prime factor p of n.
   // Unsigned big integer in bigendian representation.
+  // Required.
   bytes p = 4;
   // The prime factor q of n.
   // Unsigned big integer in bigendian representation.
+  // Required.
   bytes q = 5;
   // d mod (p - 1).
   // Unsigned big integer in bigendian representation.
+  // Required.
   bytes dp = 6;
   // d mod (q - 1).
   // Unsigned big integer in bigendian representation.
+  // Required.
   bytes dq = 7;
   // Chinese Remainder Theorem coefficient q^(-1) mod p.
   // Unsigned big integer in bigendian representation.
+  // Required.
   bytes crt = 8;
 }
 
-message JwtRsaSsaPkcs1KeyFormat {
-  uint32 version = 1;
-  JwtRsaSsaPkcs1Algorithm algorithm = 2;
-  uint32 modulus_size_in_bits = 3;
-  bytes public_exponent = 4;
+message RsaSsaPkcs1KeyFormat {
+  // Required.
+  RsaSsaPkcs1Params params = 1;
+  // Required.
+  uint32 modulus_size_in_bits = 2;
+  // Required.
+  bytes public_exponent = 3;
 }
```

### Comparing `tink-1.6.1/tink/proto/rsa_ssa_pkcs1.proto` & `tink-1.7.0/tink/proto/jwt_rsa_ssa_pss.proto`

 * *Files 26% similar despite different names*

```diff
@@ -10,82 +10,74 @@
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.
 //
 ////////////////////////////////////////////////////////////////////////////////
 
-// Definitions for RSA SSA (Signature Schemes with Appendix) using PKCS1-v1_5
-// encoding (https://tools.ietf.org/html/rfc8017#section-8.2).
 syntax = "proto3";
 
 package google.crypto.tink;
 
-import "tink/proto/common.proto";
-
 option java_package = "com.google.crypto.tink.proto";
 option java_multiple_files = true;
-option go_package = "github.com/google/tink/proto/rsa_ssa_pkcs1_go_proto";
+option go_package = "github.com/google/tink/proto/jwt_rsa_ssa_pss_go_proto";
 
-message RsaSsaPkcs1Params {
-  // Hash function used in computing hash of the signing message
-  // (see https://tools.ietf.org/html/rfc8017#section-9.2).
-  // Required.
-  HashType hash_type = 1;
+// See https://datatracker.ietf.org/doc/html/rfc7518#section-3.5
+enum JwtRsaSsaPssAlgorithm {
+  PS_UNKNOWN = 0;
+  PS256 = 1;  // RSASSA-PSS using SHA-256 and MGF1 with SHA-256
+  PS384 = 2;  // RSASSA-PSS using SHA-384 and MGF1 with SHA-384
+  PS512 = 3;  // RSASSA-PSS using SHA-512 and MGF1 with SHA-512
 }
 
-// key_type: type.googleapis.com/google.crypto.tink.RsaSsaPkcs1PublicKey
-message RsaSsaPkcs1PublicKey {
-  // Required.
+// key_type: type.googleapis.com/google.crypto.tink.JwtRsaSsaPssPublicKey
+message JwtRsaSsaPssPublicKey {
   uint32 version = 1;
-  // Required.
-  RsaSsaPkcs1Params params = 2;
+  JwtRsaSsaPssAlgorithm algorithm = 2;
   // Modulus.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes n = 3;
   // Public exponent.
-  // Unsigned big integer in bigendian representation.
+  // Unsigned big integer in big-endian representation.
   bytes e = 4;
+
+  // Optional, custom kid header value to be used with "RAW" keys.
+  // "TINK" keys with this value set will be rejected.
+  message CustomKid {
+    string value = 1;
+  }
+  CustomKid custom_kid = 5;
 }
 
-// key_type: type.googleapis.com/google.crypto.tink.RsaSsaPkcs1PrivateKey
-message RsaSsaPkcs1PrivateKey {
-  // Required.
+// key_type: type.googleapis.com/google.crypto.tink.JwtRsaSsaPssPrivateKey
+message JwtRsaSsaPssPrivateKey {
   uint32 version = 1;
-  // Required.
-  RsaSsaPkcs1PublicKey public_key = 2;
+  JwtRsaSsaPssPublicKey public_key = 2;
   // Private exponent.
-  // Unsigned big integer in bigendian representation.
-  // Required.
+  // Unsigned big integer in big-endian representation.
   bytes d = 3;
 
   // The following parameters are used to optimize RSA signature computation.
   // The prime factor p of n.
-  // Unsigned big integer in bigendian representation.
-  // Required.
+  // Unsigned big integer in big-endian representation.
   bytes p = 4;
   // The prime factor q of n.
-  // Unsigned big integer in bigendian representation.
-  // Required.
+  // Unsigned big integer in big-endian representation.
   bytes q = 5;
   // d mod (p - 1).
-  // Unsigned big integer in bigendian representation.
-  // Required.
+  // Unsigned big integer in big-endian representation.
   bytes dp = 6;
   // d mod (q - 1).
-  // Unsigned big integer in bigendian representation.
-  // Required.
+  // Unsigned big integer in big-endian representation.
   bytes dq = 7;
   // Chinese Remainder Theorem coefficient q^(-1) mod p.
-  // Unsigned big integer in bigendian representation.
-  // Required.
+  // Unsigned big integer in big-endian representation.
   bytes crt = 8;
 }
 
-message RsaSsaPkcs1KeyFormat {
-  // Required.
-  RsaSsaPkcs1Params params = 1;
-  // Required.
-  uint32 modulus_size_in_bits = 2;
-  // Required.
-  bytes public_exponent = 3;
+message JwtRsaSsaPssKeyFormat {
+  uint32 version = 1;
+  JwtRsaSsaPssAlgorithm algorithm = 2;
+  uint32 modulus_size_in_bits = 3;
+  bytes public_exponent = 4;
 }
```

### Comparing `tink-1.6.1/tink/streaming_aead/_raw_streaming_aead.py` & `tink-1.7.0/tink/streaming_aead/_raw_streaming_aead.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,20 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module defines the 'raw' interface for Streaming AEAD."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 import io
 from typing import BinaryIO
 
-# Special imports
-import six
-
 
-@six.add_metaclass(abc.ABCMeta)
-class RawStreamingAead(object):
+class RawStreamingAead(metaclass=abc.ABCMeta):
   """Raw interface for streaming authenticated encryption with associated data.
 
   Streaming encryption is typically used for encrypting large plaintexts such
   as large files. This interface supports a streaming interface for symmetric
   encryption with authentication. The underlying encryption modes are selected
   so that partial plaintext can be obtained fast by decrypting and
   authenticating just a part of the ciphertext.
```

### Comparing `tink-1.6.1/tink/streaming_aead/_streaming_aead_test.py` & `tink-1.7.0/tink/streaming_aead/_streaming_aead_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.streaming_aead.streaming_aead."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 import os
 import tempfile
 
 from absl.testing import absltest
 
 import tink
```

### Comparing `tink-1.6.1/tink/streaming_aead/_streaming_aead_key_manager_test.py` & `tink-1.7.0/tink/streaming_aead/_streaming_aead_key_manager_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.streaming_aead_key_manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import io
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from tink.proto import aes_ctr_hmac_streaming_pb2
 from tink.proto import aes_gcm_hkdf_streaming_pb2
 from tink.proto import common_pb2
```

### Comparing `tink-1.6.1/tink/streaming_aead/_encrypting_stream_test.py` & `tink-1.7.0/tink/streaming_aead/_encrypting_stream_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # Copyright 2020 Google LLC
 #
-# Lint as: python3
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.streaming_aead.encrypting_stream."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import io
 from typing import cast
 
 from absl.testing import absltest
 
 from tink import core
 from tink import streaming_aead
```

### Comparing `tink-1.6.1/tink/streaming_aead/_decrypting_stream.py` & `tink-1.7.0/tink/streaming_aead/_decrypting_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A file-like object that decrypts the data it reads.
 
 It reads the ciphertext from a given other file-like object, and decrypts it.
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 from typing import BinaryIO
 
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.streaming_aead import _file_object_adapter
 
@@ -45,15 +40,15 @@
         will be obtained.
       ciphertext_source: A readable file-like object from which ciphertext bytes
         will be read.
       associated_data: The associated data to use for decryption.
       close_ciphertext_source: Whether ciphertext_source should be closed when
         close() is called.
     """
-    super(RawDecryptingStream, self).__init__()
+    super().__init__()
     self._ciphertext_source = ciphertext_source
     self._close_ciphertext_source = close_ciphertext_source
     if not ciphertext_source.readable():
       raise ValueError('ciphertext_source must be readable')
     cc_ciphertext_source = _file_object_adapter.FileObjectAdapter(
         ciphertext_source)
     self._input_stream_adapter = self._get_input_stream_adapter(
@@ -99,24 +94,16 @@
       # https://docs.python.org/3/library/io.html also mentions a
       # non-blocking mode, but according to https://bugs.python.org/issue13322
       # that mode is not properly implemented and not really used.
       while True:
         data = self._read_from_input_stream_adapter(size)
         if data:
           return data
-    except core.TinkError as e:
-      # We are checking if the exception was raised because of C++
-      # OUT_OF_RANGE status, which signals EOF.
-      wrapped_e = e.args[0]
-      if (isinstance(wrapped_e, tink_bindings.StatusNotOk) and
-          (wrapped_e.status.error_code() ==
-           tink_bindings.ErrorCode.OUT_OF_RANGE)):
-        return b''
-      else:
-        raise e
+    except tink_bindings.PythonTinkStreamFinishedException:
+      return b''
 
   def readinto(self, b: bytearray) -> int:
     """Read bytes into a pre-allocated bytes-like object b.
 
     Args:
       b: Bytes-like object to which data will be read.
 
@@ -134,15 +121,15 @@
 
   def close(self) -> None:
     """Close the stream. Has no effect on a closed stream."""
     if self.closed:  # pylint:disable=using-constant-test
       return
     if self._close_ciphertext_source:
       self._ciphertext_source.close()
-    super(RawDecryptingStream, self).close()
+    super().close()
 
   def readable(self) -> bool:
     """Return True if the stream can be read from."""
     return True
 
   def write(self, b: bytes) -> int:
     raise io.UnsupportedOperation()
```

### Comparing `tink-1.6.1/tink/streaming_aead/_file_object_adapter.py` & `tink-1.7.0/tink/streaming_aead/_file_object_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,31 +13,26 @@
 # limitations under the License.
 """FileObjectAdapter class.
 
 Used in conjunction with PythonOutputStream/PythonInputStream to allow a C++
 OutputStream/InputStream to interact with a Python file-like object.
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 from typing import BinaryIO
 
 from tink.cc.pybind import tink_bindings
 
 
 class FileObjectAdapter(tink_bindings.PythonFileObjectAdapter):
   """Adapts a Python file object for use in C++."""
 
   def __init__(self, file_object: BinaryIO):
     # Required to fix CLIF "Value invalidated due to capture by std::unique_ptr"
-    super(FileObjectAdapter, self).__init__()
+    super().__init__()
     self._file_object = file_object
 
   def write(self, data: bytes) -> int:
     """Writes to underlying file object and returns number of bytes written."""
     try:
       written = self._file_object.write(data)
       return 0 if written is None else written
```

### Comparing `tink-1.6.1/tink/streaming_aead/_streaming_aead_key_manager.py` & `tink-1.7.0/tink/streaming_aead/_streaming_aead_key_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python wrapper of the wrapped C++ Streaming AEAD key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
-from typing import Text, BinaryIO
-import six
+from typing import BinaryIO
 
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.streaming_aead import _decrypting_stream
 from tink.streaming_aead import _encrypting_stream
 from tink.streaming_aead import _raw_streaming_aead
 from tink.streaming_aead import _streaming_aead_wrapper
@@ -51,24 +45,22 @@
         self._cc_streaming_aead,
         ciphertext_source,
         associated_data,
         close_ciphertext_source=close_ciphertext_source)
 
 
 def from_cc_registry(
-    type_url: Text) -> core.KeyManager[_raw_streaming_aead.RawStreamingAead]:
+    type_url: str) -> core.KeyManager[_raw_streaming_aead.RawStreamingAead]:
   return core.KeyManagerCcToPyWrapper(
       tink_bindings.StreamingAeadKeyManager.from_cc_registry(type_url),
       _raw_streaming_aead.RawStreamingAead, _StreamingAeadCcToPyWrapper)
 
 
 def register() -> None:
   """Registers Streaming AEAD key managers and the wrapper in the Registry."""
-  if six.PY2:
-    raise NotImplementedError('StreamingAEAD requires Python 3.')
   tink_bindings.register()
   for ident in (
       'AesCtrHmacStreamingKey',
       'AesGcmHkdfStreamingKey',
   ):
     type_url = 'type.googleapis.com/google.crypto.tink.{}'.format(ident)
     key_manager = core.KeyManagerCcToPyWrapper(
```

### Comparing `tink-1.6.1/tink/streaming_aead/_streaming_aead.py` & `tink-1.7.0/tink/streaming_aead/_streaming_aead.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,28 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module defines the interface for Streaming AEAD."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 from typing import BinaryIO
 
-# Special imports
-import six
-
 
-@six.add_metaclass(abc.ABCMeta)
-class StreamingAead(object):
+class StreamingAead(metaclass=abc.ABCMeta):
   """The interface for streaming authenticated encryption with associated data.
 
   Streaming encryption is typically used for encrypting large plaintexts such
   as large files. This interface supports a streaming interface for symmetric
   encryption with authentication. The underlying encryption modes are selected
   so that partial plaintext can be obtained fast by decrypting and
   authenticating just a part of the ciphertext.
```

### Comparing `tink-1.6.1/tink/streaming_aead/BUILD.bazel` & `tink-1.7.0/tink/streaming_aead/BUILD.bazel`

 * *Files 18% similar despite different names*

```diff
@@ -64,34 +64,31 @@
     ],
 )
 
 py_library(
     name = "_raw_streaming_aead",
     srcs = ["_raw_streaming_aead.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_streaming_aead",
     srcs = ["_streaming_aead.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_streaming_aead_key_manager",
     srcs = ["_streaming_aead_key_manager.py"],
     srcs_version = "PY3",
     deps = [
         ":_decrypting_stream",
         ":_encrypting_stream",
         ":_raw_streaming_aead",
         ":_streaming_aead_wrapper",
-        requirement("six"),
         "//tink/cc/pybind:tink_bindings",
         "//tink/core",
     ],
 )
 
 py_test(
     name = "_streaming_aead_key_manager_test",
@@ -125,26 +122,22 @@
     ],
 )
 
 py_test(
     name = "_streaming_aead_key_templates_test",
     timeout = "short",
     srcs = ["_streaming_aead_key_templates_test.py"],
-    data = [
-        "@tink_base//testdata/templates",
-    ],
     srcs_version = "PY3",
     deps = [
         ":streaming_aead",
         requirement("absl-py"),
         "//tink/proto:aes_ctr_hmac_streaming_py_pb2",
         "//tink/proto:aes_gcm_hkdf_streaming_py_pb2",
         "//tink/proto:common_py_pb2",
         "//tink/proto:tink_py_pb2",
-        "//tink/testing:helper",
     ],
 )
 
 py_test(
     name = "_streaming_aead_test",
     timeout = "short",
     srcs = ["_streaming_aead_test.py"],
@@ -192,15 +185,14 @@
 py_test(
     name = "_rewindable_input_stream_test",
     srcs = ["_rewindable_input_stream_test.py"],
     srcs_version = "PY3",
     deps = [
         ":_rewindable_input_stream",
         requirement("absl-py"),
-        requirement("six"),
         "//tink/testing:bytes_io",
     ],
 )
 
 py_library(
     name = "_file_object_adapter",
     srcs = ["_file_object_adapter.py"],
@@ -213,10 +205,21 @@
 py_test(
     name = "_file_object_adapter_test",
     srcs = ["_file_object_adapter_test.py"],
     srcs_version = "PY3",
     deps = [
         ":_file_object_adapter",
         requirement("absl-py"),
-        requirement("six"),
+    ],
+)
+
+py_test(
+    name = "_pybind11_python_file_object_adapter_test",
+    timeout = "short",
+    srcs = ["_pybind11_python_file_object_adapter_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":streaming_aead",
+        requirement("absl-py"),
+        "//tink:tink_python",
     ],
 )
```

### Comparing `tink-1.6.1/tink/streaming_aead/_streaming_aead_wrapper.py` & `tink-1.7.0/tink/streaming_aead/_streaming_aead_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Streaming AEAD wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 from typing import cast, BinaryIO, Optional, Type
 
 from tink import core
 from tink.streaming_aead import _raw_streaming_aead
 from tink.streaming_aead import _rewindable_input_stream
 from tink.streaming_aead import _streaming_aead
@@ -41,15 +36,15 @@
 
     Args:
       primitive_set: The primitive set of StreamingAead primitives.
       ciphertext_source: A readable file-like object from which ciphertext bytes
         will be read.
       associated_data: The associated data to use for decryption.
     """
-    super(_DecryptingStreamWrapper, self).__init__()
+    super().__init__()
     if not ciphertext_source.readable():
       raise ValueError('ciphertext_source must be readable')
     self._ciphertext_source = _rewindable_input_stream.RewindableInputStream(
         ciphertext_source)
     self._associated_data = associated_data
     self._matching_stream = None
     self._remaining_primitives = [
@@ -126,15 +121,15 @@
     if self.closed:  # pylint:disable=using-constant-test
       return
     if self._matching_stream:
       self._matching_stream.close()
     if self._attempting_stream:
       self._attempting_stream.close()
     self._ciphertext_source.close()
-    super(_DecryptingStreamWrapper, self).close()
+    super().close()
 
   def readable(self) -> bool:
     return True
 
 
 class _WrappedStreamingAead(_streaming_aead.StreamingAead):
   """Implements StreamingAead by wrapping a set of RawStreamingAead."""
```

### Comparing `tink-1.6.1/tink/streaming_aead/__init__.py` & `tink-1.7.0/tink/streaming_aead/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """StreamingAead package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
 from tink.streaming_aead import _streaming_aead
 from tink.streaming_aead import _streaming_aead_key_manager
 from tink.streaming_aead import _streaming_aead_key_templates as streaming_aead_key_templates
 
 
 StreamingAead = _streaming_aead.StreamingAead
```

### Comparing `tink-1.6.1/tink/streaming_aead/_rewindable_input_stream.py` & `tink-1.7.0/tink/streaming_aead/_rewindable_input_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,31 +9,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A Raw Input stream wrapper that supports rewinding."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 from typing import Optional, BinaryIO
 
 
 class RewindableInputStream(io.RawIOBase):
   """Implements a readable io.RawIOBase wrapper that supports rewinding.
 
   The wrapped input_stream can either be a io.RawIOBase or io.BufferedIOBase.
   """
 
   def __init__(self, input_stream: BinaryIO):
-    super(RewindableInputStream, self).__init__()
+    super().__init__()
     if not input_stream.readable():
       raise ValueError('input_stream must be readable')
     self._input_stream = input_stream
     self._buffer = bytearray()
     self._pos = 0
     self._rewindable = True
 
@@ -89,8 +84,8 @@
     return True
 
   def close(self) -> None:
     """Close the stream and the wrapped input_stream."""
     if self.closed:  # pylint:disable=using-constant-test
       return
     self._input_stream.close()
-    super(RewindableInputStream, self).close()
+    super().close()
```

### Comparing `tink-1.6.1/tink/streaming_aead/_rewindable_input_stream_test.py` & `tink-1.7.0/tink/streaming_aead/_rewindable_input_stream_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.util.bytes_io."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import io
 import tempfile
 from typing import BinaryIO, cast
 from absl.testing import absltest
 from absl.testing import parameterized
 
 from tink.streaming_aead import _rewindable_input_stream
```

### Comparing `tink-1.6.1/tink/streaming_aead/_decrypting_stream_test.py` & `tink-1.7.0/tink/streaming_aead/_decrypting_stream_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.streaming_aead.decrypting_stream."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import io
 from typing import BinaryIO
 
 from absl.testing import absltest
 
 from tink import core
 from tink import streaming_aead
```

### Comparing `tink-1.6.1/tink/streaming_aead/_streaming_aead_wrapper_test.py` & `tink-1.7.0/tink/streaming_aead/_streaming_aead_wrapper_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.streaming_aead._streaming_aead_wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import io
 from typing import BinaryIO, cast
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import tink
 from tink import streaming_aead
```

### Comparing `tink-1.6.1/tink/streaming_aead/_streaming_aead_key_templates.py` & `tink-1.7.0/tink/streaming_aead/_streaming_aead_key_templates.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,33 +19,30 @@
 In the future, it will be possible to use these templates to generate a new
 tink_pb2.Keyset with tink_pb2.KeysetHandle. To generate a new keyset that
 contains a single aes_ctr_hmac_streaming_pb2.AesCtrHmacStreamingKey, one can do:
 handle = keyset_handle.KeysetHandle(
   streaming_aead_key_templates.AES256_CTR_HMAC_SHA256_4KB).
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
+import warnings
 
 from tink.proto import aes_ctr_hmac_streaming_pb2
 from tink.proto import aes_gcm_hkdf_streaming_pb2
 from tink.proto import common_pb2
 from tink.proto import tink_pb2
 
 _AES_GCM_HKDF_STREAMING_KEY_TYPE_URL = (
     'type.googleapis.com/google.crypto.tink.AesGcmHkdfStreamingKey')
 _AES_CTR_HMAC_STREAMING_KEY_TYPE_URL = (
     'type.googleapis.com/google.crypto.tink.AesCtrHmacStreamingKey')
 SEGMENT_SIZE_1MB = 1024 * 1024
 SEGMENT_SIZE_4KB = 4 * 1024
 
 
-def create_aes_gcm_hkdf_streaming_key_template(
+def _create_aes_gcm_hkdf_streaming_key_template(
     aes_key_size: int, hash_type: common_pb2.HashType, derived_key_size: int,
     ciphertext_segment_size: int) -> tink_pb2.KeyTemplate:
   """Creates an AES GCM HKDF Streaming KeyTemplate, and fills in its values."""
   key_format = aes_gcm_hkdf_streaming_pb2.AesGcmHkdfStreamingKeyFormat()
   key_format.key_size = aes_key_size
   key_format.params.hkdf_hash_type = hash_type
   key_format.params.derived_key_size = derived_key_size
@@ -54,15 +51,15 @@
   key_template = tink_pb2.KeyTemplate()
   key_template.value = key_format.SerializeToString()
   key_template.type_url = _AES_GCM_HKDF_STREAMING_KEY_TYPE_URL
   key_template.output_prefix_type = tink_pb2.RAW
   return key_template
 
 
-def create_aes_ctr_hmac_streaming_key_template(
+def _create_aes_ctr_hmac_streaming_key_template(
     aes_key_size: int, hkdf_hash_type: common_pb2.HashType,
     derived_key_size: int, mac_hash_type: common_pb2.HashType, tag_size: int,
     ciphertext_segment_size: int) -> tink_pb2.KeyTemplate:
   """Creates an AES CTR HMAC Streaming KeyTemplate, and fills in its values."""
   key_format = aes_ctr_hmac_streaming_pb2.AesCtrHmacStreamingKeyFormat()
   key_format.key_size = aes_key_size
 
@@ -76,63 +73,89 @@
   key_template = tink_pb2.KeyTemplate()
   key_template.value = key_format.SerializeToString()
   key_template.type_url = _AES_CTR_HMAC_STREAMING_KEY_TYPE_URL
   key_template.output_prefix_type = tink_pb2.RAW
   return key_template
 
 
-AES128_GCM_HKDF_4KB = create_aes_gcm_hkdf_streaming_key_template(
+AES128_GCM_HKDF_4KB = _create_aes_gcm_hkdf_streaming_key_template(
     aes_key_size=16,
     hash_type=common_pb2.HashType.SHA256,
     derived_key_size=16,
     ciphertext_segment_size=SEGMENT_SIZE_4KB)
 
-AES128_GCM_HKDF_1MB = create_aes_gcm_hkdf_streaming_key_template(
+AES128_GCM_HKDF_1MB = _create_aes_gcm_hkdf_streaming_key_template(
     aes_key_size=16,
     hash_type=common_pb2.HashType.SHA256,
     derived_key_size=16,
     ciphertext_segment_size=SEGMENT_SIZE_1MB)
 
-AES256_GCM_HKDF_4KB = create_aes_gcm_hkdf_streaming_key_template(
+AES256_GCM_HKDF_4KB = _create_aes_gcm_hkdf_streaming_key_template(
     aes_key_size=32,
     hash_type=common_pb2.HashType.SHA256,
     derived_key_size=32,
     ciphertext_segment_size=SEGMENT_SIZE_4KB)
 
-AES256_GCM_HKDF_1MB = create_aes_gcm_hkdf_streaming_key_template(
+AES256_GCM_HKDF_1MB = _create_aes_gcm_hkdf_streaming_key_template(
     aes_key_size=32,
     hash_type=common_pb2.HashType.SHA256,
     derived_key_size=32,
     ciphertext_segment_size=SEGMENT_SIZE_1MB)
 
-AES128_CTR_HMAC_SHA256_4KB = create_aes_ctr_hmac_streaming_key_template(
+AES128_CTR_HMAC_SHA256_4KB = _create_aes_ctr_hmac_streaming_key_template(
     aes_key_size=16,
     hkdf_hash_type=common_pb2.HashType.SHA256,
     derived_key_size=16,
     mac_hash_type=common_pb2.HashType.SHA256,
     tag_size=32,
     ciphertext_segment_size=SEGMENT_SIZE_4KB)
 
-AES128_CTR_HMAC_SHA256_1MB = create_aes_ctr_hmac_streaming_key_template(
+AES128_CTR_HMAC_SHA256_1MB = _create_aes_ctr_hmac_streaming_key_template(
     aes_key_size=16,
     hkdf_hash_type=common_pb2.HashType.SHA256,
     derived_key_size=16,
     mac_hash_type=common_pb2.HashType.SHA256,
     tag_size=32,
     ciphertext_segment_size=SEGMENT_SIZE_1MB)
 
-AES256_CTR_HMAC_SHA256_4KB = create_aes_ctr_hmac_streaming_key_template(
+AES256_CTR_HMAC_SHA256_4KB = _create_aes_ctr_hmac_streaming_key_template(
     aes_key_size=32,
     hkdf_hash_type=common_pb2.HashType.SHA256,
     derived_key_size=32,
     mac_hash_type=common_pb2.HashType.SHA256,
     tag_size=32,
     ciphertext_segment_size=SEGMENT_SIZE_4KB)
 
-AES256_CTR_HMAC_SHA256_1MB = create_aes_ctr_hmac_streaming_key_template(
+AES256_CTR_HMAC_SHA256_1MB = _create_aes_ctr_hmac_streaming_key_template(
     aes_key_size=32,
     hkdf_hash_type=common_pb2.HashType.SHA256,
     derived_key_size=32,
     mac_hash_type=common_pb2.HashType.SHA256,
     tag_size=32,
     ciphertext_segment_size=SEGMENT_SIZE_1MB)
 
+
+# Deprecated. Use the predefined constant templates above instead.
+def create_aes_gcm_hkdf_streaming_key_template(
+    aes_key_size: int, hash_type: common_pb2.HashType, derived_key_size: int,
+    ciphertext_segment_size: int) -> tink_pb2.KeyTemplate:
+  warnings.warn(
+      'The create_aes_gcm_hkdf_streaming_key_template function is deprecated.',
+      DeprecationWarning, 2)
+  return _create_aes_gcm_hkdf_streaming_key_template(aes_key_size, hash_type,
+                                                     derived_key_size,
+                                                     ciphertext_segment_size)
+
+
+# Deprecated. Use the predefined constant templates above instead.
+def create_aes_ctr_hmac_streaming_key_template(
+    aes_key_size: int, hkdf_hash_type: common_pb2.HashType,
+    derived_key_size: int, mac_hash_type: common_pb2.HashType, tag_size: int,
+    ciphertext_segment_size: int) -> tink_pb2.KeyTemplate:
+  warnings.warn(
+      'The create_aes_ctr_hmac_streaming_key_template function is deprecated.',
+      DeprecationWarning, 2)
+  return _create_aes_ctr_hmac_streaming_key_template(aes_key_size,
+                                                     hkdf_hash_type,
+                                                     derived_key_size,
+                                                     mac_hash_type, tag_size,
+                                                     ciphertext_segment_size)
```

### Comparing `tink-1.6.1/tink/streaming_aead/_encrypting_stream.py` & `tink-1.7.0/tink/streaming_aead/_encrypting_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,14 @@
 # limitations under the License.
 """A file-like object that encrypts data written to it.
 
 It writes the ciphertext to a given other file-like object, which can later be
 decrypted and read using a DecryptingStream wrapper.
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import io
 from typing import BinaryIO, Optional
 
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.streaming_aead import _file_object_adapter
 
@@ -55,15 +50,15 @@
       stream_aead: C++ StreamingAead primitive from which a C++ EncryptingStream
         will be obtained.
       ciphertext_destination: A writable file-like object to which ciphertext
         bytes will be written.
       associated_data: The associated data to use for encryption. This must
         match the associated_data used for decryption.
     """
-    super(RawEncryptingStream, self).__init__()
+    super().__init__()
     if not ciphertext_destination.writable():
       raise ValueError('ciphertext_destination must be writable')
     cc_ciphertext_destination = _file_object_adapter.FileObjectAdapter(
         ciphertext_destination)
     self._cc_encrypting_stream = _new_cc_encrypting_stream(
         stream_aead, associated_data, cc_ciphertext_destination)
 
@@ -103,12 +98,12 @@
 
   def close(self) -> None:
     """Flush and close the stream. Has no effect on a closed stream."""
     if self.closed:  # pylint:disable=using-constant-test
       return
     self.flush()
     self._close_cc_encrypting_stream()
-    super(RawEncryptingStream, self).close()
+    super().close()
 
   def writable(self) -> bool:
     """Return True if the stream supports writing."""
     return True
```

### Comparing `tink-1.6.1/tink/streaming_aead/_file_object_adapter_test.py` & `tink-1.7.0/tink/streaming_aead/_file_object_adapter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.util._file_object_adapter."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import io
 
 from absl.testing import absltest
 from absl.testing.absltest import mock
 
 from tink.streaming_aead import _file_object_adapter
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_signature_key_manager.py` & `tink-1.7.0/tink/jwt/_jwt_signature_key_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """JWT Signature key managers."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
-from typing import Any, Optional, Text, Type, Tuple, Callable
+from typing import Any, Optional, Type, Tuple, Callable
 
 from tink.proto import jwt_ecdsa_pb2
 from tink.proto import jwt_rsa_ssa_pkcs1_pb2
 from tink.proto import jwt_rsa_ssa_pss_pb2
 from tink.proto import tink_pb2
 from tink import core
 from tink.cc.pybind import tink_bindings
+from tink.jwt import _json_util
 from tink.jwt import _jwt_error
 from tink.jwt import _jwt_format
 from tink.jwt import _jwt_public_key_sign
 from tink.jwt import _jwt_public_key_verify
 from tink.jwt import _jwt_validator
 from tink.jwt import _raw_jwt
 from tink.jwt import _verified_jwt
@@ -61,84 +57,87 @@
     jwt_rsa_ssa_pss_pb2.PS512: 'PS512'
 }
 
 
 class _JwtPublicKeySign(_jwt_public_key_sign.JwtPublicKeySignInternal):
   """Implementation of JwtPublicKeySignInternal using a PublicKeySign."""
 
-  def __init__(self, cc_primitive: tink_bindings.PublicKeySign, algorithm: Text,
-               custom_kid: Text):
+  def __init__(self, cc_primitive: tink_bindings.PublicKeySign, algorithm: str,
+               custom_kid: str):
     self._public_key_sign = cc_primitive
     self._algorithm = algorithm
     self._custom_kid = custom_kid
 
   @core.use_tink_errors
   def _sign(self, data: bytes) -> bytes:
     return self._public_key_sign.sign(data)
 
   def sign_and_encode_with_kid(self, raw_jwt: _raw_jwt.RawJwt,
-                               kid: Optional[Text]) -> Text:
+                               kid: Optional[str]) -> str:
     """Computes a signature and encodes the token.
 
     Args:
       raw_jwt: The RawJwt token to be MACed and encoded.
       kid: Optional "kid" header value. It is set by the wrapper for keys with
         output prefix TINK, and it is None for output prefix RAW.
 
     Returns:
       The MACed token encoded in the JWS compact serialization format.
     Raises:
       tink.TinkError if the operation fails.
     """
-    type_header = raw_jwt.type_header() if raw_jwt.has_type_header() else None
     if self._custom_kid is not None:
       if kid is not None:
         raise _jwt_error.JwtInvalidError(
             'custom_kid must not be set for keys with output prefix type TINK')
       kid = self._custom_kid
-    unsigned = _jwt_format.create_unsigned_compact(self._algorithm, type_header,
-                                                   kid, raw_jwt.json_payload())
+    unsigned = _jwt_format.create_unsigned_compact(self._algorithm, kid,
+                                                   raw_jwt)
     return _jwt_format.create_signed_compact(unsigned, self._sign(unsigned))
 
 
-class _JwtPublicKeyVerify(_jwt_public_key_verify.JwtPublicKeyVerify):
+class _JwtPublicKeyVerify(_jwt_public_key_verify.JwtPublicKeyVerifyInternal):
   """Implementation of JwtPublicKeyVerify using a PublicKeyVerify."""
 
   def __init__(self, cc_primitive: tink_bindings.PublicKeyVerify,
-               algorithm: Text, custom_kid: Optional[Text]):
+               algorithm: str, custom_kid: Optional[str]):
     self._public_key_verify = cc_primitive
     self._algorithm = algorithm
     self._custom_kid = custom_kid
 
   @core.use_tink_errors
   def _verify(self, signature: bytes, data: bytes) -> None:
     self._public_key_verify.verify(signature, data)
 
-  def verify_and_decode(
-      self, compact: Text,
-      validator: _jwt_validator.JwtValidator) -> _verified_jwt.VerifiedJwt:
+  def verify_and_decode_with_kid(
+      self, compact: str, validator: _jwt_validator.JwtValidator,
+      kid: Optional[str]) -> _verified_jwt.VerifiedJwt:
     """Verifies, validates and decodes a signed compact JWT token."""
     parts = _jwt_format.split_signed_compact(compact)
     unsigned_compact, json_header, json_payload, signature = parts
     self._verify(signature, unsigned_compact)
-    header = _jwt_format.json_loads(json_header)
-    _jwt_format.validate_header(header, self._algorithm)
-    raw_jwt = _raw_jwt.RawJwt.from_json(
+    header = _json_util.json_loads(json_header)
+    _jwt_format.validate_header(
+        header=header,
+        algorithm=self._algorithm,
+        tink_kid=kid,
+        custom_kid=self._custom_kid)
+    raw_jwt = _raw_jwt.raw_jwt_from_json(
         _jwt_format.get_type_header(header), json_payload)
     _jwt_validator.validate(validator, raw_jwt)
     return _verified_jwt.VerifiedJwt._create(raw_jwt)  # pylint: disable=protected-access
 
 
 class _JwtPublicKeySignKeyManagerCcToPyWrapper(
     core.PrivateKeyManager[_jwt_public_key_sign.JwtPublicKeySignInternal]):
   """Converts a C++ sign key manager into a JwtPublicKeySignKeyManager."""
 
   def __init__(self, cc_key_manager: tink_bindings.PublicKeySignKeyManager,
                key_data_to_alg_kid: Callable[[tink_pb2.KeyData],
-                                             Tuple[Text, Optional[Text]]]):
+                                             Tuple[str, Optional[str]]]):
     self._cc_key_manager = cc_key_manager
     self._key_data_to_alg_kid = key_data_to_alg_kid
 
   def primitive_class(
       self) -> Type[_jwt_public_key_sign.JwtPublicKeySignInternal]:
     return _jwt_public_key_sign.JwtPublicKeySignInternal
 
@@ -146,15 +145,15 @@
   def primitive(
       self, key_data: tink_pb2.KeyData
   ) -> _jwt_public_key_sign.JwtPublicKeySignInternal:
     sign = self._cc_key_manager.primitive(key_data.SerializeToString())
     algorithm, custom_kid = self._key_data_to_alg_kid(key_data)
     return _JwtPublicKeySign(sign, algorithm, custom_kid)
 
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     return self._cc_key_manager.key_type()
 
   @core.use_tink_errors
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     return tink_pb2.KeyData.FromString(
         self._cc_key_manager.new_key_data(key_template.SerializeToString()))
@@ -162,117 +161,118 @@
   @core.use_tink_errors
   def public_key_data(self, key_data: tink_pb2.KeyData) -> tink_pb2.KeyData:
     return tink_pb2.KeyData.FromString(
         self._cc_key_manager.public_key_data(key_data.SerializeToString()))
 
 
 class _JwtPublicKeyVerifyKeyManagerCcToPyWrapper(
-    core.KeyManager[_jwt_public_key_verify.JwtPublicKeyVerify]):
+    core.KeyManager[_jwt_public_key_verify.JwtPublicKeyVerifyInternal]):
   """Converts a C++ verify key manager into a JwtPublicKeyVerifyKeyManager."""
 
   def __init__(self, cc_key_manager: tink_bindings.PublicKeyVerifyKeyManager,
                key_data_to_alg_kid: Callable[[tink_pb2.KeyData],
-                                             Tuple[Text, Optional[Text]]]):
+                                             Tuple[str, Optional[str]]]):
     self._cc_key_manager = cc_key_manager
     self._key_data_to_alg_kid = key_data_to_alg_kid
 
-  def primitive_class(self) -> Type[_jwt_public_key_verify.JwtPublicKeyVerify]:
-    return _jwt_public_key_verify.JwtPublicKeyVerify
+  def primitive_class(
+      self) -> Type[_jwt_public_key_verify.JwtPublicKeyVerifyInternal]:
+    return _jwt_public_key_verify.JwtPublicKeyVerifyInternal
 
   @core.use_tink_errors
   def primitive(
-      self,
-      key_data: tink_pb2.KeyData) -> _jwt_public_key_verify.JwtPublicKeyVerify:
+      self, key_data: tink_pb2.KeyData
+  ) -> _jwt_public_key_verify.JwtPublicKeyVerifyInternal:
     verify = self._cc_key_manager.primitive(key_data.SerializeToString())
     algorithm, custom_kid = self._key_data_to_alg_kid(key_data)
     return _JwtPublicKeyVerify(verify, algorithm, custom_kid)
 
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     return self._cc_key_manager.key_type()
 
   @core.use_tink_errors
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     return tink_pb2.KeyData.FromString(
         self._cc_key_manager.new_key_data(key_template.SerializeToString()))
 
 
-def _ecdsa_algorithm_text(algorithm: jwt_ecdsa_pb2.JwtEcdsaAlgorithm) -> Text:
+def _ecdsa_algorithm_text(algorithm: jwt_ecdsa_pb2.JwtEcdsaAlgorithm) -> str:
   if algorithm not in _ECDSA_ALGORITHM_TEXTS:
     raise _jwt_error.JwtInvalidError('Invalid algorithm')
   return _ECDSA_ALGORITHM_TEXTS[algorithm]
 
 
-def _get_custom_kid(public_key_proto: Any) -> Optional[Text]:
+def _get_custom_kid(public_key_proto: Any) -> Optional[str]:
   if public_key_proto.HasField('custom_kid'):
     return public_key_proto.custom_kid.value
   else:
     return None
 
 
 def _ecdsa_alg_kid_from_private_key_data(
-    key_data: tink_pb2.KeyData) -> Tuple[Text, Optional[Text]]:
+    key_data: tink_pb2.KeyData) -> Tuple[str, Optional[str]]:
   if key_data.type_url != _JWT_ECDSA_PRIVATE_KEY_TYPE:
     raise _jwt_error.JwtInvalidError('Invalid key data key type')
   key = jwt_ecdsa_pb2.JwtEcdsaPrivateKey.FromString(key_data.value)
   return (_ecdsa_algorithm_text(key.public_key.algorithm),
           _get_custom_kid(key.public_key))
 
 
 def _ecdsa_alg_kid_from_public_key_data(
-    key_data: tink_pb2.KeyData) -> Tuple[Text, Optional[Text]]:
+    key_data: tink_pb2.KeyData) -> Tuple[str, Optional[str]]:
   if key_data.type_url != _JWT_ECDSA_PUBLIC_KEY_TYPE:
     raise _jwt_error.JwtInvalidError('Invalid key data key type')
   key = jwt_ecdsa_pb2.JwtEcdsaPublicKey.FromString(key_data.value)
   return (_ecdsa_algorithm_text(key.algorithm), _get_custom_kid(key))
 
 
 def _rsa_ssa_pkcs1_algorithm_text(
-    algorithm: jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1Algorithm) -> Text:
+    algorithm: jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1Algorithm) -> str:
   if algorithm not in _RSA_SSA_PKCS1_ALGORITHM_TEXTS:
     raise _jwt_error.JwtInvalidError('Invalid algorithm')
   return _RSA_SSA_PKCS1_ALGORITHM_TEXTS[algorithm]
 
 
 def _rsa_ssa_pkcs1_alg_kid_from_private_key_data(
-    key_data: tink_pb2.KeyData) -> Tuple[Text, Optional[Text]]:
+    key_data: tink_pb2.KeyData) -> Tuple[str, Optional[str]]:
   if key_data.type_url != _JWT_RSA_SSA_PKCS1_PRIVATE_KEY_TYPE:
     raise _jwt_error.JwtInvalidError('Invalid key data key type')
   key = jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1PrivateKey.FromString(
       key_data.value)
   return (_rsa_ssa_pkcs1_algorithm_text(key.public_key.algorithm),
           _get_custom_kid(key.public_key))
 
 
 def _rsa_ssa_pkcs1_alg_kid_from_public_key_data(
-    key_data: tink_pb2.KeyData) -> Tuple[Text, Optional[Text]]:
+    key_data: tink_pb2.KeyData) -> Tuple[str, Optional[str]]:
   if key_data.type_url != _JWT_RSA_SSA_PKCS1_PUBLIC_KEY_TYPE:
     raise _jwt_error.JwtInvalidError('Invalid key data key type')
   key = jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1PublicKey.FromString(key_data.value)
   return (_rsa_ssa_pkcs1_algorithm_text(key.algorithm), _get_custom_kid(key))
 
 
 def _rsa_ssa_pss_algorithm_text(
-    algorithm: jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssAlgorithm) -> Text:
+    algorithm: jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssAlgorithm) -> str:
   if algorithm not in _RSA_SSA_PSS_ALGORITHM_TEXTS:
     raise _jwt_error.JwtInvalidError('Invalid algorithm')
   return _RSA_SSA_PSS_ALGORITHM_TEXTS[algorithm]
 
 
 def _rsa_ssa_pss_alg_kid_from_private_key_data(
-    key_data: tink_pb2.KeyData) -> Tuple[Text, Optional[Text]]:
+    key_data: tink_pb2.KeyData) -> Tuple[str, Optional[str]]:
   if key_data.type_url != _JWT_RSA_SSA_PSS_PRIVATE_KEY_TYPE:
     raise _jwt_error.JwtInvalidError('Invalid key data key type')
   key = jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssPrivateKey.FromString(key_data.value)
   return (_rsa_ssa_pss_algorithm_text(key.public_key.algorithm),
           _get_custom_kid(key.public_key))
 
 
 def _rsa_ssa_pss_alg_kid_from_public_key_data(
-    key_data: tink_pb2.KeyData) -> Tuple[Text, Optional[Text]]:
+    key_data: tink_pb2.KeyData) -> Tuple[str, Optional[str]]:
   if key_data.type_url != _JWT_RSA_SSA_PSS_PUBLIC_KEY_TYPE:
     raise _jwt_error.JwtInvalidError('Invalid key data key type')
   key = jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssPublicKey.FromString(key_data.value)
   return (_rsa_ssa_pss_algorithm_text(key.algorithm), _get_custom_kid(key))
 
 
 def register():
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_mac.py` & `tink-1.7.0/tink/jwt/_jwt_mac.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,54 +9,46 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Interface for JwtMac."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 
-from typing import Optional, Text
-
-import six
+from typing import Optional
 
 from tink.jwt import _jwt_validator
 from tink.jwt import _raw_jwt
 from tink.jwt import _verified_jwt
 
 
-@six.add_metaclass(abc.ABCMeta)
-class JwtMac(object):
+class JwtMac(metaclass=abc.ABCMeta):
   """Interface for authenticating and verifying JWT with JWS MAC.
 
   Sees RFC 7519 and RFC 7515. Security guarantees: similar to MAC.
   """
 
   @abc.abstractmethod
-  def compute_mac_and_encode(self, token: _raw_jwt.RawJwt) -> Text:
+  def compute_mac_and_encode(self, token: _raw_jwt.RawJwt) -> str:
     """Computes a MAC and encodes the token.
 
     Args:
       token: The RawJwt token to be MACed and encoded.
 
     Returns:
       The MACed token encoded in the JWS compact serialization format.
     Raises:
       tink.TinkError if the operation fails.
     """
     raise NotImplementedError()
 
   @abc.abstractmethod
   def verify_mac_and_decode(
-      self, compact: Text,
+      self, compact: str,
       validator: _jwt_validator.JwtValidator) -> _verified_jwt.VerifiedJwt:
     """Verifies, validates and decodes a MACed compact JWT token.
 
     The JWT is validated against the rules in validator. That is, every claim in
     validator must also be present in the JWT. For example, if validator
     contains an issuer (iss) claim, the JWT must contain an identical claim.
     The JWT can contain claims that are NOT in the validator, which are then
@@ -76,25 +68,24 @@
       A VerifiedJwt.
     Raises:
       tink.TinkError if the operation fails.
     """
     raise NotImplementedError()
 
 
-@six.add_metaclass(abc.ABCMeta)
-class JwtMacInternal(object):
+class JwtMacInternal(metaclass=abc.ABCMeta):
   """Internal interface for authenticating and verifying JWT with JWS MAC.
 
   "kid" is an optional value that is set by the wrapper for keys with output
-  prefix TINK, and it is set to None for output prefix RAW.
+  prefix TINK. It is set to None for output prefix RAW.
   """
 
   @abc.abstractmethod
   def compute_mac_and_encode_with_kid(self, token: _raw_jwt.RawJwt,
-                                      kid: Optional[Text]) -> Text:
+                                      kid: Optional[str]) -> str:
     raise NotImplementedError()
 
   @abc.abstractmethod
-  def verify_mac_and_decode(
-      self, compact: Text,
-      validator: _jwt_validator.JwtValidator) -> _verified_jwt.VerifiedJwt:
+  def verify_mac_and_decode_with_kid(
+      self, compact: str, validator: _jwt_validator.JwtValidator,
+      kid: Optional[str]) -> _verified_jwt.VerifiedJwt:
     raise NotImplementedError()
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_mac_wrapper_test.py` & `tink-1.7.0/tink/jwt/_jwt_mac_wrapper_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,51 +9,78 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.jwt._jwt_mac_wrapper."""
 
+import io
+
 from absl.testing import absltest
 from absl.testing import parameterized
 
+
 from tink.proto import jwt_hmac_pb2
 from tink.proto import tink_pb2
 import tink
+from tink import cleartext_keyset_handle
 from tink import jwt
+from tink.jwt import _json_util
 from tink.jwt import _jwt_format
 from tink.testing import keyset_builder
 
 
 def setUpModule():
   jwt.register_jwt_mac()
 
 
-def _create_jwt_hmac_template(
-    algorithm: jwt_hmac_pb2.JwtHmacAlgorithm, key_size: int,
-    output_prefix_type: tink_pb2.OutputPrefixType) -> tink_pb2.KeyTemplate:
-  key_format = jwt_hmac_pb2.JwtHmacKeyFormat(
-      algorithm=algorithm, key_size=key_size)
-  return tink_pb2.KeyTemplate(
-      type_url='type.googleapis.com/google.crypto.tink.JwtHmacKey',
-      value=key_format.SerializeToString(),
-      output_prefix_type=output_prefix_type)
-
-
-def jwt_hs256_tink_template() -> tink_pb2.KeyTemplate:
-  return _create_jwt_hmac_template(jwt_hmac_pb2.HS256, 32, tink_pb2.TINK)
+def _set_custom_kid(keyset_handle: tink.KeysetHandle,
+                    custom_kid: str) -> tink.KeysetHandle:
+  """Set the custom_kid field of the first key."""
+  buffer = io.BytesIO()
+  cleartext_keyset_handle.write(
+      tink.BinaryKeysetWriter(buffer), keyset_handle)
+  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  hmac_key = jwt_hmac_pb2.JwtHmacKey.FromString(keyset.key[0].key_data.value)
+  hmac_key.custom_kid.value = custom_kid
+  keyset.key[0].key_data.value = hmac_key.SerializeToString()
+  return cleartext_keyset_handle.from_keyset(keyset)
+
+
+def _change_key_id(keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
+  """Changes the key id of the first key and sets it primary."""
+  buffer = io.BytesIO()
+  cleartext_keyset_handle.write(
+      tink.BinaryKeysetWriter(buffer), keyset_handle)
+  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  # XOR the key id with an arbitrary 32-bit string to get a new key id.
+  new_key_id = keyset.key[0].key_id ^ 0xdeadbeef
+  keyset.key[0].key_id = new_key_id
+  keyset.primary_key_id = new_key_id
+  return cleartext_keyset_handle.from_keyset(keyset)
+
+
+def _change_output_prefix_to_tink(
+    keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
+  """Changes the output prefix type of the first key to TINK."""
+  buffer = io.BytesIO()
+  cleartext_keyset_handle.write(
+      tink.BinaryKeysetWriter(buffer), keyset_handle)
+  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  keyset.key[0].output_prefix_type = tink_pb2.TINK
+  return cleartext_keyset_handle.from_keyset(keyset)
 
 
 class JwtMacWrapperTest(parameterized.TestCase):
 
   @parameterized.parameters([
+      (jwt.raw_jwt_hs256_template(), jwt.raw_jwt_hs256_template()),
+      (jwt.raw_jwt_hs256_template(), jwt.jwt_hs256_template()),
+      (jwt.jwt_hs256_template(), jwt.raw_jwt_hs256_template()),
       (jwt.jwt_hs256_template(), jwt.jwt_hs256_template()),
-      (jwt.jwt_hs256_template(), jwt_hs256_tink_template()),
-      (jwt_hs256_tink_template(), jwt.jwt_hs256_template()),
-      (jwt_hs256_tink_template(), jwt_hs256_tink_template()),
   ])
   def test_key_rotation(self, old_key_tmpl, new_key_tmpl):
     builder = keyset_builder.new_keyset_builder()
     older_key_id = builder.add_new_key(old_key_tmpl)
 
     builder.set_primary_key(older_key_id)
     jwtmac1 = builder.keyset_handle().primitive(jwt.JwtMac)
@@ -112,65 +139,115 @@
     self.assertEqual(
         jwtmac2.verify_mac_and_decode(compact4, validator).issuer(), 'a')
     self.assertEqual(
         jwtmac3.verify_mac_and_decode(compact4, validator).issuer(), 'a')
     self.assertEqual(
         jwtmac4.verify_mac_and_decode(compact4, validator).issuer(), 'a')
 
-  def test_tink_output_prefix_type_encodes_a_kid_header(self):
-    keyset_handle = tink.new_keyset_handle(jwt_hs256_tink_template())
-    jwt_mac = keyset_handle.primitive(jwt.JwtMac)
+  def test_only_tink_output_prefix_type_encodes_a_kid_header(self):
+    handle = tink.new_keyset_handle(jwt.raw_jwt_hs256_template())
+    jwt_mac = handle.primitive(jwt.JwtMac)
+
+    tink_handle = _change_output_prefix_to_tink(handle)
+    tink_jwt_mac = tink_handle.primitive(jwt.JwtMac)
 
     raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
-    signed_compact = jwt_mac.compute_mac_and_encode(raw_jwt)
 
-    _, json_header, _, _ = _jwt_format.split_signed_compact(signed_compact)
-    header = _jwt_format.json_loads(json_header)
-    self.assertIn('kid', header)
+    token = jwt_mac.compute_mac_and_encode(raw_jwt)
+    token_with_kid = tink_jwt_mac.compute_mac_and_encode(raw_jwt)
 
-  def test_raw_output_prefix_type_encodes_a_custom_kid_header(self):
-    keyset_handle = tink.new_keyset_handle(jwt.raw_jwt_hs256_template())
+    _, header, _, _ = _jwt_format.split_signed_compact(token)
+    self.assertNotIn('kid', _json_util.json_loads(header))
 
-    # Add a custom kid to the key in keyset_handle
-    value = keyset_handle._keyset.key[0].key_data.value
-    hmac_key = jwt_hmac_pb2.JwtHmacKey.FromString(value)
-    hmac_key.custom_kid.value = 'my kid'
-    keyset_handle._keyset.key[0].key_data.value = hmac_key.SerializeToString()
+    _, header_with_kid, _, _ = _jwt_format.split_signed_compact(token_with_kid)
+    self.assertIn('kid', _json_util.json_loads(header_with_kid))
 
-    jwt_mac = keyset_handle.primitive(jwt.JwtMac)
+    validator = jwt.new_validator(
+        expected_issuer='issuer', allow_missing_expiration=True)
+    jwt_mac.verify_mac_and_decode(token, validator)
+    tink_jwt_mac.verify_mac_and_decode(token_with_kid, validator)
 
-    raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
-    signed_compact = jwt_mac.compute_mac_and_encode(raw_jwt)
+    # With output prefix type RAW, a kid header is ignored
+    jwt_mac.verify_mac_and_decode(token_with_kid, validator)
+    # With output prefix type TINK, a kid header is required.
+    with self.assertRaises(tink.TinkError):
+      tink_jwt_mac.verify_mac_and_decode(token, validator)
+
+    other_handle = _change_key_id(tink_handle)
+    other_jwt_mac = other_handle.primitive(jwt.JwtMac)
+    # A token with a wrong kid is rejected, even if the signature is ok.
+    with self.assertRaises(tink.TinkError):
+      other_jwt_mac.verify_mac_and_decode(token_with_kid, validator)
 
-    _, json_header, _, _ = _jwt_format.split_signed_compact(signed_compact)
-    header = _jwt_format.json_loads(json_header)
-    self.assertEqual(header['kid'], 'my kid')
+  def test_raw_output_prefix_type_encodes_a_custom_kid_header(self):
+    # normal HMAC jwt_mac with output prefix RAW
+    handle = tink.new_keyset_handle(jwt.raw_jwt_hs256_template())
+    raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
+    validator = jwt.new_validator(
+        expected_issuer='issuer', allow_missing_expiration=True)
 
-    # Now, change the output prefix type to TINK. This should fail.
-    keyset_handle._keyset.key[0].output_prefix_type = tink_pb2.TINK
+    jwt_mac = handle.primitive(jwt.JwtMac)
+    token = jwt_mac.compute_mac_and_encode(raw_jwt)
+    jwt_mac.verify_mac_and_decode(token, validator)
+
+    _, json_header, _, _ = _jwt_format.split_signed_compact(token)
+    self.assertNotIn('kid', _json_util.json_loads(json_header))
+
+    # HMAC jwt_mac with a custom_kid set
+    custom_kid_handle = _set_custom_kid(handle, custom_kid='my kid')
+    custom_kid_jwt_mac = custom_kid_handle.primitive(jwt.JwtMac)
+    token_with_kid = custom_kid_jwt_mac.compute_mac_and_encode(raw_jwt)
+    custom_kid_jwt_mac.verify_mac_and_decode(token_with_kid, validator)
+
+    _, header_with_kid, _, _ = _jwt_format.split_signed_compact(token_with_kid)
+    self.assertEqual(_json_util.json_loads(header_with_kid)['kid'], 'my kid')
+
+    # Even when custom_kid is set, its not required to be set in the header.
+    custom_kid_jwt_mac.verify_mac_and_decode(token, validator)
+    # An additional kid header is ignored.
+    jwt_mac.verify_mac_and_decode(token_with_kid, validator)
+
+    other_handle = _set_custom_kid(handle, custom_kid='other kid')
+    other_jwt_mac = other_handle.primitive(jwt.JwtMac)
+    with self.assertRaises(tink.TinkError):
+      # The custom_kid does not match the kid header.
+      other_jwt_mac.verify_mac_and_decode(
+          token_with_kid, validator)
+
+    tink_handle = _change_output_prefix_to_tink(custom_kid_handle)
+    tink_jwt_mac = tink_handle.primitive(jwt.JwtMac)
+    # having custom_kid set with output prefix TINK is not allowed
     with self.assertRaises(tink.TinkError):
-      tink_jwt_mac = keyset_handle.primitive(jwt.JwtMac)
       tink_jwt_mac.compute_mac_and_encode(raw_jwt)
+    with self.assertRaises(tink.TinkError):
+      tink_jwt_mac.verify_mac_and_decode(token, validator)
+    with self.assertRaises(tink.TinkError):
+      tink_jwt_mac.verify_mac_and_decode(token_with_kid, validator)
 
   def test_legacy_key_fails(self):
-    template = _create_jwt_hmac_template(jwt_hmac_pb2.HS256, 32,
-                                         tink_pb2.LEGACY)
+    template = keyset_builder.legacy_template(jwt.raw_jwt_hs256_template())
     builder = keyset_builder.new_keyset_builder()
     key_id = builder.add_new_key(template)
     builder.set_primary_key(key_id)
     handle = builder.keyset_handle()
     with self.assertRaises(tink.TinkError):
       handle.primitive(jwt.JwtMac)
 
   def test_legacy_non_primary_key_fails(self):
     builder = keyset_builder.new_keyset_builder()
-    old_template = _create_jwt_hmac_template(jwt_hmac_pb2.HS256, 32,
-                                             tink_pb2.LEGACY)
+    old_template = keyset_builder.legacy_template(jwt.raw_jwt_hs256_template())
     _ = builder.add_new_key(old_template)
     current_key_id = builder.add_new_key(jwt.jwt_hs256_template())
     builder.set_primary_key(current_key_id)
     handle = builder.keyset_handle()
     with self.assertRaises(tink.TinkError):
       handle.primitive(jwt.JwtMac)
 
+  def test_jwt_mac_from_keyset_without_primary_fails(self):
+    builder = keyset_builder.new_keyset_builder()
+    builder.add_new_key(jwt.raw_jwt_hs256_template())
+    with self.assertRaises(tink.TinkError):
+      builder.keyset_handle()
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/jwt/_verified_jwt.py` & `tink-1.7.0/tink/jwt/_verified_jwt.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 """The verified JSON Web Token (JWT)."""
 
 import datetime
 
-from typing import List, Set, Text
+from typing import List, Set
 
 from tink import core
 from tink.jwt import _raw_jwt
 
 
-class VerifiedJwt(object):
-  """A verified JSON Web Token (JWT).
+class VerifiedJwt:
+  """A decoded and verified JSON Web Token (JWT).
 
-  A VerifiedJwt is returned as the result of a sucessfully verification of a
-  MACed or signed compact JWT token.
+  A new instance of this class is returned as the result of a sucessfully
+  verification of a MACed or signed compact JWT.
+
+  It gives read-only access all payload claims and a subset of the headers. It
+  does not contain any headers that depend on the key, such as "alg" or "kid".
+  These headers are checked when the signature is verified and should not be
+  read by the user. This ensures that the key can be changed without any changes
+  to the user code.
   """
 
   def __new__(cls):
     raise core.TinkError('VerifiedJwt cannot be instantiated directly.')
 
   @classmethod
   def _create(cls, raw_jwt: _raw_jwt.RawJwt):
@@ -38,39 +44,39 @@
 
   def __init__(self, raw_jwt: _raw_jwt.RawJwt) -> None:
     self._raw_jwt = raw_jwt
 
   def has_type_header(self) -> bool:
     return self._raw_jwt.has_type_header()
 
-  def type_header(self) -> Text:
+  def type_header(self) -> str:
     return self._raw_jwt.type_header()
 
   def has_issuer(self) -> bool:
     return self._raw_jwt.has_issuer()
 
-  def issuer(self) -> Text:
+  def issuer(self) -> str:
     return self._raw_jwt.issuer()
 
   def has_subject(self) -> bool:
     return self._raw_jwt.has_subject()
 
-  def subject(self) -> Text:
+  def subject(self) -> str:
     return self._raw_jwt.subject()
 
   def has_audiences(self) -> bool:
     return self._raw_jwt.has_audiences()
 
-  def audiences(self) -> List[Text]:
+  def audiences(self) -> List[str]:
     return self._raw_jwt.audiences()
 
   def has_jwt_id(self) -> bool:
     return self._raw_jwt.has_jwt_id()
 
-  def jwt_id(self) -> Text:
+  def jwt_id(self) -> str:
     return self._raw_jwt.jwt_id()
 
   def has_expiration(self) -> bool:
     return self._raw_jwt.has_expiration()
 
   def expiration(self) -> datetime.datetime:
     return self._raw_jwt.expiration()
@@ -83,12 +89,12 @@
 
   def has_issued_at(self) -> bool:
     return self._raw_jwt.has_issued_at()
 
   def issued_at(self) -> datetime.datetime:
     return self._raw_jwt.issued_at()
 
-  def custom_claim_names(self) -> Set[Text]:
+  def custom_claim_names(self) -> Set[str]:
     return self._raw_jwt.custom_claim_names()
 
-  def custom_claim(self, name: Text) -> _raw_jwt.Claim:
+  def custom_claim(self, name: str) -> _raw_jwt.Claim:
     return self._raw_jwt.custom_claim(name)
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_validator.py` & `tink-1.7.0/tink/jwt/_jwt_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,127 +10,142 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 """The JwtValidator."""
 
 import datetime
 
-from typing import Optional, Text
+from typing import Optional
 from tink.jwt import _jwt_error
 from tink.jwt import _raw_jwt
 
 _MAX_CLOCK_SKEW = datetime.timedelta(minutes=10)
 
 
-class JwtValidator(object):
+class JwtValidator:
   """A JwtValidator defines how JSON Web Tokens (JWTs) should be validated.
 
     By default, the JwtValidator requires that a token has a valid expiration
-    claim, no issuer, no subject, and no audience claim. This can be changed
-    using the expect_... and  ignore_... arguments.
+    claim, no issuer and no audience claim. This can be changed using the
+    expect_... and  ignore_... arguments.
 
     If present, the JwtValidator also validates the not-before claim. The
     validation time can be changed using the fixed_now parameter. clock_skew can
     be set to allow a small leeway (not more than 10 minutes) to account for
     clock skew.
   """
 
   def __init__(self,
                *,
-               expected_type_header: Optional[Text],
-               expected_issuer: Optional[Text],
-               expected_subject: Optional[Text],
-               expected_audience: Optional[Text],
+               expected_type_header: Optional[str],
+               expected_issuer: Optional[str],
+               expected_audience: Optional[str],
                ignore_type_header: bool,
                ignore_issuer: bool,
-               ignore_subject: bool,
                ignore_audiences: bool,
                allow_missing_expiration: bool,
+               expect_issued_in_the_past: bool,
                clock_skew: Optional[datetime.timedelta],
                fixed_now: Optional[datetime.datetime]) -> None:
     if expected_type_header and ignore_type_header:
       raise ValueError(
           'expected_type_header and ignore_type_header cannot be used together')
     if expected_issuer and ignore_issuer:
       raise ValueError(
           'expected_issuer and ignore_issuer cannot be used together')
-    if expected_subject and ignore_subject:
-      raise ValueError(
-          'expected_subject and ignore_subject cannot be used together')
     if expected_audience and ignore_audiences:
       raise ValueError(
           'expected_audience and ignore_audiences cannot be used together')
     self._expected_type_header = expected_type_header
     self._expected_issuer = expected_issuer
-    self._expected_subject = expected_subject
     self._expected_audience = expected_audience
     self._ignore_type_header = ignore_type_header
     self._ignore_issuer = ignore_issuer
-    self._ignore_subject = ignore_subject
     self._ignore_audiences = ignore_audiences
     self._allow_missing_expiration = allow_missing_expiration
+    self._expect_issued_in_the_past = expect_issued_in_the_past
     if clock_skew:
       if clock_skew > _MAX_CLOCK_SKEW:
         raise ValueError('clock skew too large, max is 10 minutes')
       self._clock_skew = clock_skew
     else:
       self._clock_skew = datetime.timedelta()
     if fixed_now and not fixed_now.tzinfo:
       raise ValueError('fixed_now without tzinfo')
     self._fixed_now = fixed_now
 
   def has_expected_type_header(self) -> bool:
     return self._expected_type_header is not None
 
-  def expected_type_header(self) -> Text:
+  def expected_type_header(self) -> str:
     return self._expected_type_header
 
   def has_expected_issuer(self) -> bool:
     return self._expected_issuer is not None
 
-  def expected_issuer(self) -> Text:
+  def expected_issuer(self) -> str:
     return self._expected_issuer
 
-  def has_expected_subject(self) -> bool:
-    return self._expected_subject is not None
-
-  def expected_subject(self) -> Text:
-    return self._expected_subject
-
   def has_expected_audience(self) -> bool:
     return self._expected_audience is not None
 
-  def expected_audience(self) -> Text:
+  def expected_audience(self) -> str:
     return self._expected_audience
 
   def ignore_type_header(self) -> bool:
     return self._ignore_type_header
 
   def ignore_issuer(self) -> bool:
     return self._ignore_issuer
 
-  def ignore_subject(self) -> bool:
-    return self._ignore_subject
-
   def ignore_audiences(self) -> bool:
     return self._ignore_audiences
 
   def allow_missing_expiration(self) -> bool:
     return self._allow_missing_expiration
 
+  def expect_issued_in_the_past(self) -> bool:
+    return self._expect_issued_in_the_past
+
   def clock_skew(self) -> datetime.timedelta:
     return self._clock_skew
 
   def has_fixed_now(self) -> bool:
     return self._fixed_now is not None
 
   def fixed_now(self) -> datetime.datetime:
     return self._fixed_now
 
 
+def new_validator(
+    *,
+    expected_type_header: Optional[str] = None,
+    expected_issuer: Optional[str] = None,
+    expected_audience: Optional[str] = None,
+    ignore_type_header: bool = False,
+    ignore_issuer: bool = False,
+    ignore_audiences: bool = False,
+    allow_missing_expiration: bool = False,
+    expect_issued_in_the_past: bool = False,
+    clock_skew: Optional[datetime.timedelta] = None,
+    fixed_now: Optional[datetime.datetime] = None) -> JwtValidator:
+  """Creates a new JwtValidator."""
+  return JwtValidator(
+      expected_type_header=expected_type_header,
+      expected_issuer=expected_issuer,
+      expected_audience=expected_audience,
+      ignore_type_header=ignore_type_header,
+      ignore_issuer=ignore_issuer,
+      ignore_audiences=ignore_audiences,
+      allow_missing_expiration=allow_missing_expiration,
+      expect_issued_in_the_past=expect_issued_in_the_past,
+      clock_skew=clock_skew,
+      fixed_now=fixed_now)
+
+
 def validate(validator: JwtValidator, raw_jwt: _raw_jwt.RawJwt) -> None:
   """Validates a jwt.RawJwt and raises JwtInvalidError if it is invalid.
 
   This function is called by the JWT primitives and does not need to be called
   by the user.
 
   Args:
@@ -149,14 +164,21 @@
       raw_jwt.expiration() <= now - validator.clock_skew()):
     raise _jwt_error.JwtInvalidError('token has expired since %s' %
                                      raw_jwt.expiration())
   if (raw_jwt.has_not_before() and
       raw_jwt.not_before() > now + validator.clock_skew()):
     raise _jwt_error.JwtInvalidError('token cannot be used before %s' %
                                      raw_jwt.not_before())
+  if validator.expect_issued_in_the_past():
+    if not raw_jwt.has_issued_at():
+      raise _jwt_error.JwtInvalidError('token is missing iat claim')
+    if raw_jwt.issued_at() > now + validator.clock_skew():
+      raise _jwt_error.JwtInvalidError(
+          'token has a invalid iat claim in the future: %s' %
+          raw_jwt.issued_at())
   if validator.has_expected_type_header():
     if not raw_jwt.has_type_header():
       raise _jwt_error.JwtInvalidError(
           'invalid JWT; missing expected type header %s.' %
           validator.expected_type_header())
     if validator.expected_type_header() != raw_jwt.type_header():
       raise _jwt_error.JwtInvalidError(
@@ -175,27 +197,14 @@
       raise _jwt_error.JwtInvalidError(
           'invalid JWT; expected issuer %s, but got %s' %
           (validator.expected_issuer(), raw_jwt.issuer()))
   else:
     if raw_jwt.has_issuer() and not validator.ignore_issuer():
       raise _jwt_error.JwtInvalidError(
           'invalid JWT; token has issuer set, but validator not.')
-  if validator.has_expected_subject():
-    if not raw_jwt.has_subject():
-      raise _jwt_error.JwtInvalidError(
-          'invalid JWT; missing expected subject %s.' %
-          validator.expected_subject())
-    if validator.expected_subject() != raw_jwt.subject():
-      raise _jwt_error.JwtInvalidError(
-          'invalid JWT; expected subject %s, but got %s' %
-          (validator.expected_subject(), raw_jwt.subject()))
-  else:
-    if raw_jwt.has_subject() and not validator.ignore_subject():
-      raise _jwt_error.JwtInvalidError(
-          'invalid JWT; token has subject set, but validator not.')
   if validator.has_expected_audience():
     if (not raw_jwt.has_audiences() or
         validator.expected_audience() not in raw_jwt.audiences()):
       raise _jwt_error.JwtInvalidError(
           'invalid JWT; missing expected audience %s.' %
           validator.expected_audience())
   else:
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_format_test.py` & `tink-1.7.0/tink/jwt/_jwt_format_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,108 +12,95 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.jwt._jwt_format."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from tink.proto import tink_pb2
+from tink.jwt import _json_util
 from tink.jwt import _jwt_error
 from tink.jwt import _jwt_format
+from tink.jwt import _raw_jwt
 
 
 class JwtFormatTest(parameterized.TestCase):
 
   def test_base64_encode_decode_header_fixed_data(self):
     # Example from https://tools.ietf.org/html/rfc7519#section-3.1
     header = bytes([
         123, 34, 116, 121, 112, 34, 58, 34, 74, 87, 84, 34, 44, 13, 10, 32, 34,
         97, 108, 103, 34, 58, 34, 72, 83, 50, 53, 54, 34, 125
     ])
     encoded_header = b'eyJ0eXAiOiJKV1QiLA0KICJhbGciOiJIUzI1NiJ9'
-    self.assertEqual(_jwt_format._base64_encode(header), encoded_header)
-    self.assertEqual(_jwt_format._base64_decode(encoded_header), header)
+    self.assertEqual(_jwt_format.base64_encode(header), encoded_header)
+    self.assertEqual(_jwt_format.base64_decode(encoded_header), header)
 
   def test_base64_encode_decode_payload_fixed_data(self):
     # Example from https://tools.ietf.org/html/rfc7519#section-3.1
     payload = bytes([
         123, 34, 105, 115, 115, 34, 58, 34, 106, 111, 101, 34, 44, 13, 10, 32,
         34, 101, 120, 112, 34, 58, 49, 51, 48, 48, 56, 49, 57, 51, 56, 48, 44,
         13, 10, 32, 34, 104, 116, 116, 112, 58, 47, 47, 101, 120, 97, 109, 112,
         108, 101, 46, 99, 111, 109, 47, 105, 115, 95, 114, 111, 111, 116, 34,
         58, 116, 114, 117, 101, 125
     ])
     encoded_payload = (b'eyJpc3MiOiJqb2UiLA0KICJleHAiOjEzMDA4MTkzODAsDQogImh0'
                        b'dHA6Ly9leGFtcGxlLmNvbS9pc19yb290Ijp0cnVlfQ')
-    self.assertEqual(_jwt_format._base64_encode(payload), encoded_payload)
-    self.assertEqual(_jwt_format._base64_decode(encoded_payload), payload)
+    self.assertEqual(_jwt_format.base64_encode(payload), encoded_payload)
+    self.assertEqual(_jwt_format.base64_decode(encoded_payload), payload)
 
   def test_base64_decode_bad_format_raises_jwt_invalid_error(self):
     with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format._base64_decode(b'aeyJh')
+      _jwt_format.base64_decode(b'aeyJh')
 
   def test_base64_decode_fails_with_unknown_chars(self):
     self.assertNotEmpty(
-        _jwt_format._base64_decode(
+        _jwt_format.base64_decode(
             b'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_-')
     )
-    self.assertEqual(_jwt_format._base64_decode(b''), b'')
+    self.assertEqual(_jwt_format.base64_decode(b''), b'')
     with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format._base64_decode(b'[')
+      _jwt_format.base64_decode(b'[')
     with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format._base64_decode(b'@')
+      _jwt_format.base64_decode(b'@')
     with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format._base64_decode(b'/')
+      _jwt_format.base64_decode(b'/')
     with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format._base64_decode(b':')
+      _jwt_format.base64_decode(b':')
     with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format._base64_decode(b'{')
-
-  def test_json_loads_recursion(self):
-    num_recursions = 1000
-    recursive_json = ('{"a":' * num_recursions) + '""' + ('}' * num_recursions)
-    with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format.json_loads(recursive_json)
-
-  def test_json_loads_with_invalid_utf16(self):
-    with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format.json_loads(u'{"a":{"b":{"c":"\\uD834"}}}')
-    with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format.json_loads(u'{"\\uD834":"b"}')
-    with self.assertRaises(_jwt_error.JwtInvalidError):
-      _jwt_format.json_loads(u'{"a":["a":{"b":["c","\\uD834"]}]}')
+      _jwt_format.base64_decode(b'{')
 
   def test_decode_encode_header_hs256(self):
     # Example from https://tools.ietf.org/html/rfc7515#appendix-A.1
     encoded_header = b'eyJ0eXAiOiJKV1QiLA0KICJhbGciOiJIUzI1NiJ9'
     json_header = _jwt_format.decode_header(encoded_header)
-    header = _jwt_format.json_loads(json_header)
+    header = _json_util.json_loads(json_header)
     self.assertEqual(header['alg'], 'HS256')
     self.assertEqual(header['typ'], 'JWT')
     self.assertEqual(
         _jwt_format.decode_header(_jwt_format.encode_header(json_header)),
         json_header)
 
   def test_decode_encode_header_rs256(self):
     # Example from https://tools.ietf.org/html/rfc7515#appendix-A.2
     encoded_header = b'eyJhbGciOiJSUzI1NiJ9'
     json_header = _jwt_format.decode_header(encoded_header)
-    header = _jwt_format.json_loads(json_header)
+    header = _json_util.json_loads(json_header)
     self.assertEqual(header['alg'], 'RS256')
     self.assertEqual(
         _jwt_format.decode_header(_jwt_format.encode_header(json_header)),
         json_header)
 
   def test_encode_decode_header(self):
     encoded_header = _jwt_format.encode_header('{ "alg": "RS256"} ')
     json_header = _jwt_format.decode_header(encoded_header)
     self.assertEqual(json_header, '{ "alg": "RS256"} ')
 
   def test_decode_header_with_invalid_utf8(self):
-    encoded_header = _jwt_format._base64_encode(
-        b'{"alg":"RS256", "bad":"\xc2"}')
+    encoded_header = _jwt_format.base64_encode(b'{"alg":"RS256", "bad":"\xc2"}')
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.decode_header(encoded_header)
 
   def test_encode_header_with_utf16_surrogate(self):
     self.assertEqual(
         _jwt_format.encode_header('{"alg": "RS256", "a":"\U0001d11e"}'),
         b'eyJhbGciOiAiUlMyNTYiLCAiYSI6IvCdhJ4ifQ')
@@ -125,71 +112,100 @@
   @parameterized.parameters([
       'HS256', 'HS384', 'HS512', 'ES256', 'ES384', 'ES512', 'RS256', 'RS384',
       'RS384', 'RS512', 'PS256', 'PS384', 'PS512'
   ])
   def test_create_validate_header(self, algorithm):
     encoded_header = _jwt_format.create_header(algorithm, None, None)
     json_header = _jwt_format.decode_header(encoded_header)
-    header = _jwt_format.json_loads(json_header)
+    header = _json_util.json_loads(json_header)
     _jwt_format.validate_header(header, algorithm)
     self.assertIsNone(_jwt_format.get_type_header(header))
 
   def test_create_header_with_type(self):
     encoded_header = _jwt_format.create_header('HS256', 'typeHeader', None)
     json_header = _jwt_format.decode_header(encoded_header)
     self.assertEqual(json_header, '{"alg":"HS256","typ":"typeHeader"}')
-    header = _jwt_format.json_loads(json_header)
+    header = _json_util.json_loads(json_header)
     _jwt_format.validate_header(header, 'HS256')
     self.assertEqual(_jwt_format.get_type_header(header), 'typeHeader')
 
   def test_create_header_with_type_and_kid(self):
     encoded_header = _jwt_format.create_header('HS256', 'typeHeader', 'GsapRA')
     json_header = _jwt_format.decode_header(encoded_header)
     self.assertEqual(json_header,
                      '{"kid":"GsapRA","alg":"HS256","typ":"typeHeader"}')
-    header = _jwt_format.json_loads(json_header)
+    header = _json_util.json_loads(json_header)
     _jwt_format.validate_header(header, 'HS256')
     self.assertEqual(_jwt_format.get_type_header(header), 'typeHeader')
 
   def test_create_header_with_unknown_alg_fails(self):
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.create_header('unknown', None, None)
 
   def test_create_verify_different_algorithms_fails(self):
     encoded_header = _jwt_format.create_header('HS256', None, None)
     json_header = _jwt_format.decode_header(encoded_header)
-    header = _jwt_format.json_loads(json_header)
+    header = _json_util.json_loads(json_header)
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.validate_header(header, 'ES256')
 
   def test_verify_empty_header_fails(self):
-    header = _jwt_format.json_loads('{}')
+    header = _json_util.json_loads('{}')
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.validate_header(header, 'ES256')
 
   def test_validate_header_with_unknown_algorithm_fails(self):
-    header = _jwt_format.json_loads('{"alg":"HS123"}')
+    header = _json_util.json_loads('{"alg":"HS123"}')
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.validate_header(header, 'HS123')
 
   def test_validate_header_with_unknown_entry_success(self):
-    header = _jwt_format.json_loads('{"alg":"HS256","unknown":"header"}')
+    header = _json_util.json_loads('{"alg":"HS256","unknown":"header"}')
     _jwt_format.validate_header(header, 'HS256')
 
   def test_validate_header_ignores_typ(self):
-    header = _jwt_format.json_loads('{"alg":"HS256","typ":"unknown"}')
+    header = _json_util.json_loads('{"alg":"HS256","typ":"unknown"}')
     _jwt_format.validate_header(header, 'HS256')
 
   def test_validate_header_rejects_crit(self):
-    header = _jwt_format.json_loads(
+    header = _json_util.json_loads(
         '{"alg":"HS256","crit":["http://example.invalid/UNDEFINED"],'
         '"http://example.invalid/UNDEFINED":true}')
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.validate_header(header, 'HS256')
 
+  def test_validate_header_with_kid_success(self):
+    json_header = '{"kid":"GsapRA","alg":"HS256"}'
+    header = _json_util.json_loads(json_header)
+    _jwt_format.validate_header(header, 'HS256')
+    _jwt_format.validate_header(header, 'HS256', tink_kid='GsapRA')
+    _jwt_format.validate_header(header, 'HS256', custom_kid='GsapRA')
+    with self.assertRaises(_jwt_error.JwtInvalidError):
+      # fails because tink_kid and custom_kid must not be set at the same time.
+      _jwt_format.validate_header(
+          header, 'HS256', tink_kid='GsapRA', custom_kid='GsapRA')
+
+  def test_validate_header_with_other_kid_fails(self):
+    json_header = '{"kid":"GsapRA","alg":"HS256"}'
+    header = _json_util.json_loads(json_header)
+    _jwt_format.validate_header(header, 'HS256')
+    with self.assertRaises(_jwt_error.JwtInvalidError):
+      _jwt_format.validate_header(header, 'HS256', tink_kid='otherKid')
+    with self.assertRaises(_jwt_error.JwtInvalidError):
+      _jwt_format.validate_header(header, 'HS256', custom_kid='otherKid')
+
+  def test_validate_header_with_missing_kid_missing(self):
+    json_header = '{"alg":"HS256"}'
+    header = _json_util.json_loads(json_header)
+    with self.assertRaises(_jwt_error.JwtInvalidError):
+      # if tink_kid is set, a kid header is required.
+      _jwt_format.validate_header(header, 'HS256', tink_kid='GsapRA')
+    # if custom_kid is set, a kid header is *not* required.
+    _jwt_format.validate_header(header, 'HS256', custom_kid='GsapRA')
+
   def test_get_kid_success(self):
     key_id = 0x1ac6a944
     self.assertEqual(_jwt_format.get_kid(key_id, tink_pb2.TINK), 'GsapRA')
     self.assertIsNone(_jwt_format.get_kid(key_id, tink_pb2.RAW), None)
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.get_kid(key_id, tink_pb2.LEGACY)
 
@@ -202,28 +218,28 @@
       _jwt_format.get_kid(2**33, tink_pb2.TINK)
 
   def test_json_decode_encode_payload_fixed_data(self):
     # Example from https://tools.ietf.org/html/rfc7519#section-3.1
     encoded_payload = (b'eyJpc3MiOiJqb2UiLA0KICJleHAiOjEzMDA4MTkzODAsDQogImh0'
                        b'dHA6Ly9leGFtcGxlLmNvbS9pc19yb290Ijp0cnVlfQ')
     json_payload = _jwt_format.decode_payload(encoded_payload)
-    payload = _jwt_format.json_loads(json_payload)
+    payload = _json_util.json_loads(json_payload)
     self.assertEqual(payload['iss'], 'joe')
     self.assertEqual(payload['exp'], 1300819380)
     self.assertEqual(payload['http://example.com/is_root'], True)
     self.assertEqual(
         _jwt_format.decode_payload(_jwt_format.encode_payload(json_payload)),
         json_payload)
 
   def test_decode_encode_payload(self):
     # Example from https://tools.ietf.org/html/rfc7519#section-3.1
     encoded_payload = (b'eyJpc3MiOiJqb2UiLA0KICJleHAiOjEzMDA4MTkzODAsDQogImh0'
                        b'dHA6Ly9leGFtcGxlLmNvbS9pc19yb290Ijp0cnVlfQ')
     json_payload = _jwt_format.decode_payload(encoded_payload)
-    payload = _jwt_format.json_loads(json_payload)
+    payload = _json_util.json_loads(json_payload)
     self.assertEqual(payload['iss'], 'joe')
     self.assertEqual(payload['exp'], 1300819380)
     self.assertEqual(payload['http://example.com/is_root'], True)
     self.assertEqual(
         _jwt_format.decode_payload(_jwt_format.encode_payload(json_payload)),
         json_payload)
 
@@ -233,76 +249,76 @@
         b'eyJpc3MiOiLwnYSeIn0')
 
   def test_encode_payload_with_invalid_utf16(self):
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.encode_payload('{"iss":"\uD834"}')
 
   def test_create_unsigned_compact_success(self):
+    raw_jwt = _raw_jwt.raw_jwt_from_json(None, '{"iss":"joe"}')
     self.assertEqual(
-        _jwt_format.create_unsigned_compact('RS256', None, None,
-                                            '{"iss":"joe"}'),
+        _jwt_format.create_unsigned_compact('RS256', None, raw_jwt),
         b'eyJhbGciOiJSUzI1NiJ9.eyJpc3MiOiJqb2UifQ')
 
   def test_encode_decode_signature_success(self):
     signature = bytes([
         116, 24, 223, 180, 151, 153, 224, 37, 79, 250, 96, 125, 216, 173, 187,
         186, 22, 212, 37, 77, 105, 214, 191, 240, 91, 88, 5, 88, 83, 132, 141,
         121
     ])
     encoded = _jwt_format.encode_signature(signature)
     self.assertEqual(encoded, b'dBjftJeZ4CVP-mB92K27uhbUJU1p1r_wW1gFWFOEjXk')
     self.assertEqual(_jwt_format.decode_signature(encoded), signature)
 
   def test_signed_compact_create_split(self):
-    payload = '{"iss":"joe"}'
+    raw_jwt = _raw_jwt.raw_jwt_from_json('JWT', '{"iss":"joe"}')
     signature = _jwt_format.decode_signature(
         b'dBjftJeZ4CVP-mB92K27uhbUJU1p1r_wW1gFWFOEjXk')
     unsigned_compact = _jwt_format.create_unsigned_compact(
-        'RS256', 'JWT', None, payload)
+        'RS256', None, raw_jwt)
     signed_compact = _jwt_format.create_signed_compact(unsigned_compact,
                                                        signature)
     un_comp, hdr, pay, sig = _jwt_format.split_signed_compact(signed_compact)
 
     self.assertEqual(
         unsigned_compact,
         b'eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJqb2UifQ')
     self.assertEqual(
         signed_compact, 'eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.'
         'eyJpc3MiOiJqb2UifQ.dBjftJeZ4CVP-mB92K27uhbUJU1p1r_wW1gFWFOEjXk')
     self.assertEqual(un_comp, unsigned_compact)
     self.assertEqual(sig, signature)
     self.assertEqual(hdr, '{"alg":"RS256","typ":"JWT"}')
-    header = _jwt_format.json_loads(hdr)
+    header = _json_util.json_loads(hdr)
     _jwt_format.validate_header(header, 'RS256')
-    self.assertEqual(pay, payload)
+    self.assertEqual(pay, '{"iss":"joe"}')
     self.assertEqual(_jwt_format.get_type_header(header), 'JWT')
 
   def test_signed_compact_create_split_with_kid(self):
-    payload = '{"iss":"joe"}'
+    raw_jwt = _raw_jwt.raw_jwt_from_json(None, '{"iss":"joe"}')
     signature = _jwt_format.decode_signature(
         b'dBjftJeZ4CVP-mB92K27uhbUJU1p1r_wW1gFWFOEjXk')
     unsigned_compact = _jwt_format.create_unsigned_compact(
-        'RS256', None, 'AZxkm2U', payload)
+        'RS256', 'AZxkm2U', raw_jwt)
     signed_compact = _jwt_format.create_signed_compact(unsigned_compact,
                                                        signature)
     un_comp, hdr, pay, sig = _jwt_format.split_signed_compact(signed_compact)
 
     self.assertEqual(
         unsigned_compact,
         b'eyJraWQiOiJBWnhrbTJVIiwiYWxnIjoiUlMyNTYifQ.eyJpc3MiOiJqb2UifQ')
     self.assertEqual(
         signed_compact,
         'eyJraWQiOiJBWnhrbTJVIiwiYWxnIjoiUlMyNTYifQ.eyJpc3MiOiJqb2UifQ'
         '.dBjftJeZ4CVP-mB92K27uhbUJU1p1r_wW1gFWFOEjXk')
     self.assertEqual(un_comp, unsigned_compact)
     self.assertEqual(sig, signature)
     self.assertEqual(hdr, '{"kid":"AZxkm2U","alg":"RS256"}')
-    header = _jwt_format.json_loads(hdr)
+    header = _json_util.json_loads(hdr)
     _jwt_format.validate_header(header, 'RS256')
-    self.assertEqual(pay, payload)
+    self.assertEqual(pay, '{"iss":"joe"}')
     self.assertIsNone(_jwt_format.get_type_header(header))
 
   def test_split_empty_signed_compact(self):
     un_comp, hdr, pay, sig = _jwt_format.split_signed_compact('..')
     self.assertEqual(un_comp, b'.')
     self.assertEmpty(sig)
     self.assertEmpty(hdr)
@@ -348,16 +364,15 @@
       _jwt_format.split_signed_compact('e30.$e30.YWJj')
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.split_signed_compact('e30.e30.YWJj$')
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.split_signed_compact('e30.e30.YWJj\ud83c')
 
   def test_split_signed_compact_with_invalid_utf8_in_header(self):
-    encoded_header = _jwt_format._base64_encode(
-        b'{"alg":"RS256", "bad":"\xc2"}')
+    encoded_header = _jwt_format.base64_encode(b'{"alg":"RS256", "bad":"\xc2"}')
     token = (encoded_header + b'.e30.YWJj').decode('utf8')
     with self.assertRaises(_jwt_error.JwtInvalidError):
       _jwt_format.split_signed_compact(token)
 
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_public_key_verify.py` & `tink-1.7.0/tink/jwt/_jwt_public_key_verify.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,39 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Interface for JwtPublicKeyVerify."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 
-from typing import Text
-
-import six
+from typing import Optional
 
 from tink.jwt import _jwt_validator
 from tink.jwt import _verified_jwt
 
 
-@six.add_metaclass(abc.ABCMeta)
-class JwtPublicKeyVerify(object):
+class JwtPublicKeyVerify(metaclass=abc.ABCMeta):
   """Interface for verifying a signed JWT.
 
   Sees RFC 7519 and RFC 7515. Security guarantees: similar to PublicKeyVerify.
   """
 
   @abc.abstractmethod
   def verify_and_decode(
-      self, compact: Text,
+      self, compact: str,
       validator: _jwt_validator.JwtValidator) -> _verified_jwt.VerifiedJwt:
     """Verifies, validates and decodes a signed compact JWT token.
 
     The JWT is validated against the rules in validator. That is, every claim in
     validator must also be present in the JWT. For example, if validator
     contains an issuer (iss) claim, the JWT must contain an identical claim.
     The JWT can contain claims that are NOT in the validator, which are then
@@ -59,7 +51,21 @@
 
     Returns:
       A VerifiedJwt.
     Raises:
       tink.TinkError if the operation fails.
     """
     raise NotImplementedError()
+
+
+class JwtPublicKeyVerifyInternal(metaclass=abc.ABCMeta):
+  """Internal interface for creating a signed JWT.
+
+  "kid" is an optional value that is set by the wrapper for keys with output
+  prefix TINK. It is set to None for output prefix RAW.
+  """
+
+  @abc.abstractmethod
+  def verify_and_decode_with_kid(
+      self, compact: str, validator: _jwt_validator.JwtValidator,
+      kid: Optional[str]) -> _verified_jwt.VerifiedJwt:
+    raise NotImplementedError()
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_signature_key_manager_test.py` & `tink-1.7.0/tink/jwt/_jwt_signature_key_manager_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.jwt._jwt_signature_key_manager."""
 
 import datetime
 
-from typing import cast, Text
+from typing import cast
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
 from tink.proto import jwt_ecdsa_pb2
 from tink.proto import tink_pb2
 import tink
@@ -36,15 +36,15 @@
                                                 datetime.timezone.utc)
 
 
 def setUpModule():
   jwt.register_jwt_signature()
 
 
-def gen_compact(json_header: Text, json_payload: Text, raw_sign) -> Text:
+def gen_compact(json_header: str, json_payload: str, raw_sign) -> str:
   unsigned_compact = (
       _jwt_format.encode_header(json_header) + b'.' +
       _jwt_format.encode_payload(json_payload))
   signature = raw_sign.sign(unsigned_compact)
   return _jwt_format.create_signed_compact(unsigned_compact, signature)
 
 
@@ -90,20 +90,17 @@
       verify.verify_and_decode(signed_compact + '?', validator)
 
     # modified signature
     with self.assertRaises(tink.TinkError):
       verify.verify_and_decode(signed_compact + 'a', validator)
 
     # modified header
-    # TODO(juerg): Add better tests.
     with self.assertRaises(tink.TinkError):
       verify.verify_and_decode('a' + signed_compact, validator)
 
-    # TODO(juerg): Add tests with kid headers
-
   def test_create_sign_verify_with_type_header(self):
     handle = tink.new_keyset_handle(jwt.jwt_es256_template())
     sign = handle.primitive(jwt.JwtPublicKeySign)
     verify = handle.public_keyset_handle().primitive(jwt.JwtPublicKeyVerify)
     raw_jwt = jwt.new_raw_jwt(
         type_header='typeHeader', issuer='joe', without_expiration=True)
     signed_compact = sign.sign_and_encode(raw_jwt)
@@ -126,43 +123,123 @@
         jwt.JwtPublicKeyVerify)
     with self.assertRaises(tink.TinkError):
       other_verify.verify_and_decode(
           compact,
           jwt.new_validator(
               expected_issuer='issuer', allow_missing_expiration=True))
 
-  def test_bad_tokens_with_valid_signatures_fail(self):
-    handle = tink.new_keyset_handle(jwt.jwt_es256_template())
+  def test_weird_tokens_with_valid_signatures(self):
+    handle = tink.new_keyset_handle(jwt.raw_jwt_es256_template())
     sign = handle.primitive(jwt.JwtPublicKeySign)
-    # get the raw sign primitive, so that we can create correct signatures
+    # Get the internal PublicKeySign primitive to create valid signatures.
     wrapped = cast(_jwt_signature_wrappers._WrappedJwtPublicKeySign, sign)
     raw_sign = cast(_jwt_signature_key_manager._JwtPublicKeySign,
                     wrapped._primitive_set.primary().primitive)._public_key_sign
 
     verify = handle.public_keyset_handle().primitive(jwt.JwtPublicKeyVerify)
     validator = jwt.new_validator(
         expected_issuer='issuer', allow_missing_expiration=True)
 
-    valid_compact = gen_compact('{"alg":"ES256"}', '{"iss":"issuer"}', raw_sign)
-    verified_jwt = verify.verify_and_decode(valid_compact, validator)
+    # Normal token.
+    valid = gen_compact('{"alg":"ES256"}', '{"iss":"issuer"}', raw_sign)
+    verified_jwt = verify.verify_and_decode(valid, validator)
+    self.assertEqual(verified_jwt.issuer(), 'issuer')
+
+    # Token with unknown header is valid.
+    unknown_header = gen_compact('{"alg":"ES256","unknown_header":"abc"} \n ',
+                                 '{"iss":"issuer" }', raw_sign)
+    verified_jwt = verify.verify_and_decode(unknown_header, validator)
+    self.assertEqual(verified_jwt.issuer(), 'issuer')
+
+    # Token with unknown kid is valid, since primitives with output prefix type
+    # RAW ignore kid headers.
+    unknown_header = gen_compact('{"alg":"ES256","kid":"unknown"} \n ',
+                                 '{"iss":"issuer" }', raw_sign)
+    verified_jwt = verify.verify_and_decode(unknown_header, validator)
     self.assertEqual(verified_jwt.issuer(), 'issuer')
 
+    # Token with invalid alg header
     alg_invalid = gen_compact('{"alg":"ES384"}', '{"iss":"issuer"}', raw_sign)
     with self.assertRaises(tink.TinkError):
       verify.verify_and_decode(alg_invalid, validator)
 
+    # Token with empty header
+    empty_header = gen_compact('{}', '{"iss":"issuer"}', raw_sign)
+    with self.assertRaises(tink.TinkError):
+      verify.verify_and_decode(empty_header, validator)
+
+    # Token header is not valid JSON
     header_invalid = gen_compact('{"alg":"ES256"', '{"iss":"issuer"}', raw_sign)
     with self.assertRaises(tink.TinkError):
       verify.verify_and_decode(header_invalid, validator)
 
+    # Token payload is not valid JSON
     payload_invalid = gen_compact('{"alg":"ES256"}', '{"iss":"issuer"',
                                   raw_sign)
     with self.assertRaises(tink.TinkError):
       verify.verify_and_decode(payload_invalid, validator)
 
+    # Token with whitespace in header JSON string is valid.
+    whitespace_in_header = gen_compact(' {"alg":   \n  "ES256"} \n ',
+                                       '{"iss":"issuer" }', raw_sign)
+    verified_jwt = verify.verify_and_decode(whitespace_in_header, validator)
+    self.assertEqual(verified_jwt.issuer(), 'issuer')
+
+    # Token with whitespace in payload JSON string is valid.
+    whitespace_in_payload = gen_compact('{"alg":"ES256"}',
+                                        ' {"iss": \n"issuer" } \n', raw_sign)
+    verified_jwt = verify.verify_and_decode(whitespace_in_payload, validator)
+    self.assertEqual(verified_jwt.issuer(), 'issuer')
+
+    # Token with whitespace in base64-encoded header is invalid.
+    with_whitespace = (
+        _jwt_format.encode_header('{"alg":"ES256"}') + b' .' +
+        _jwt_format.encode_payload('{"iss":"issuer"}'))
+    token_with_whitespace = _jwt_format.create_signed_compact(
+        with_whitespace, raw_sign.sign(with_whitespace))
+    with self.assertRaises(tink.TinkError):
+      verify.verify_and_decode(token_with_whitespace, validator)
+
+    # Token with invalid character is invalid.
+    with_invalid_char = (
+        _jwt_format.encode_header('{"alg":"ES256"}') + b'.?' +
+        _jwt_format.encode_payload('{"iss":"issuer"}'))
+    token_with_invalid_char = _jwt_format.create_signed_compact(
+        with_invalid_char, raw_sign.sign(with_invalid_char))
+    with self.assertRaises(tink.TinkError):
+      verify.verify_and_decode(token_with_invalid_char, validator)
+
+    # Token with additional '.' is invalid.
+    with_dot = (
+        _jwt_format.encode_header('{"alg":"ES256"}') + b'.' +
+        _jwt_format.encode_payload('{"iss":"issuer"}') + b'.')
+    token_with_dot = _jwt_format.create_signed_compact(
+        with_dot, raw_sign.sign(with_dot))
+    with self.assertRaises(tink.TinkError):
+      verify.verify_and_decode(token_with_dot, validator)
+
+    # num_recursions has been chosen such that parsing of this token fails
+    # in all languages. We want to make sure that the algorithm does not
+    # hang or crash in this case, but only returns a parsing error.
+    num_recursions = 10000
+    rec_payload = ('{"a":' * num_recursions) + '""' + ('}' * num_recursions)
+    rec_token = gen_compact('{"alg":"ES256"}', rec_payload, raw_sign)
+    with self.assertRaises(tink.TinkError):
+      verify.verify_and_decode(
+          rec_token, validator=jwt.new_validator(allow_missing_expiration=True))
+
+    # test wrong types
+    with self.assertRaises(tink.TinkError):
+      verify.verify_and_decode(cast(str, None), validator)
+    with self.assertRaises(tink.TinkError):
+      verify.verify_and_decode(cast(str, 123), validator)
+    with self.assertRaises(tink.TinkError):
+      valid_bytes = valid.encode('utf8')
+      verify.verify_and_decode(cast(str, valid_bytes), validator)
+
   def test_create_ecdsa_handle_with_invalid_algorithm_fails(self):
     key_format = jwt_ecdsa_pb2.JwtEcdsaKeyFormat(
         algorithm=jwt_ecdsa_pb2.ES_UNKNOWN)
     template = tink_pb2.KeyTemplate(
         type_url='type.googleapis.com/google.crypto.tink.JwtEcdsaPrivateKey',
         value=key_format.SerializeToString(),
         output_prefix_type=tink_pb2.RAW)
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_hmac_key_manager.py` & `tink-1.7.0/tink/jwt/_jwt_hmac_key_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A JWT HMAC key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
-from typing import Optional, Text, Type
+from typing import Optional, Type
 
 from tink.proto import jwt_hmac_pb2
 from tink.proto import tink_pb2
 from tink import core
 from tink.cc.pybind import tink_bindings
+from tink.jwt import _json_util
 from tink.jwt import _jwt_error
 from tink.jwt import _jwt_format
 from tink.jwt import _jwt_mac
 from tink.jwt import _jwt_validator
 from tink.jwt import _raw_jwt
 from tink.jwt import _verified_jwt
 
@@ -39,66 +35,66 @@
     jwt_hmac_pb2.HS512: 'HS512'
 }
 
 
 class _JwtHmac(_jwt_mac.JwtMacInternal):
   """Interface for authenticating and verifying JWT with JWS MAC."""
 
-  def __init__(self, cc_mac: tink_bindings.Mac, algorithm: Text,
-               custom_kid: Optional[Text]):
+  def __init__(self, cc_mac: tink_bindings.Mac, algorithm: str,
+               custom_kid: Optional[str]):
     self._cc_mac = cc_mac
     self._algorithm = algorithm
     self._custom_kid = custom_kid
 
   @core.use_tink_errors
   def _compute_mac(self, data: bytes) -> bytes:
     return self._cc_mac.compute_mac(data)
 
   @core.use_tink_errors
   def _verify_mac(self, mac_value: bytes, data: bytes) -> None:
     self._cc_mac.verify_mac(mac_value, data)
 
   def compute_mac_and_encode_with_kid(self, raw_jwt: _raw_jwt.RawJwt,
-                                      kid: Optional[Text]) -> Text:
+                                      kid: Optional[str]) -> str:
     """Computes a MAC and encodes the token.
 
     Args:
       raw_jwt: The RawJwt token to be MACed and encoded.
       kid: Optional "kid" header value. It is set by the wrapper for keys with
         output prefix TINK, and it is None for output prefix RAW.
 
     Returns:
       The MACed token encoded in the JWS compact serialization format.
     Raises:
       tink.TinkError if the operation fails.
     """
-    if raw_jwt.has_type_header():
-      type_header = raw_jwt.type_header()
-    else:
-      type_header = None
     if self._custom_kid is not None:
       if kid is not None:
         raise _jwt_error.JwtInvalidError(
             'custom_kid must not be set for keys with output prefix type TINK')
       kid = self._custom_kid
-    unsigned = _jwt_format.create_unsigned_compact(self._algorithm, type_header,
-                                                   kid, raw_jwt.json_payload())
+    unsigned = _jwt_format.create_unsigned_compact(self._algorithm, kid,
+                                                   raw_jwt)
     return _jwt_format.create_signed_compact(unsigned,
                                              self._compute_mac(unsigned))
 
-  def verify_mac_and_decode(
-      self, compact: Text,
-      validator: _jwt_validator.JwtValidator) -> _verified_jwt.VerifiedJwt:
+  def verify_mac_and_decode_with_kid(
+      self, compact: str, validator: _jwt_validator.JwtValidator,
+      kid: Optional[str]) -> _verified_jwt.VerifiedJwt:
     """Verifies, validates and decodes a MACed compact JWT token."""
     parts = _jwt_format.split_signed_compact(compact)
     unsigned_compact, json_header, json_payload, mac = parts
     self._verify_mac(mac, unsigned_compact)
-    header = _jwt_format.json_loads(json_header)
-    _jwt_format.validate_header(header, self._algorithm)
-    raw_jwt = _raw_jwt.RawJwt.from_json(
+    header = _json_util.json_loads(json_header)
+    _jwt_format.validate_header(
+        header=header,
+        algorithm=self._algorithm,
+        tink_kid=kid,
+        custom_kid=self._custom_kid)
+    raw_jwt = _raw_jwt.raw_jwt_from_json(
         _jwt_format.get_type_header(header), json_payload)
     _jwt_validator.validate(validator, raw_jwt)
     return _verified_jwt.VerifiedJwt._create(raw_jwt)  # pylint: disable=protected-access
 
 
 class MacCcToPyJwtMacKeyManager(core.KeyManager[_jwt_mac.JwtMacInternal]):
   """Transforms C++ KeyManager into a Python KeyManager."""
@@ -119,15 +115,15 @@
     cc_mac = self._cc_key_manager.primitive(key_data.SerializeToString())
     if jwt_hmac_key.HasField('custom_kid'):
       custom_kid = jwt_hmac_key.custom_kid.value
     else:
       custom_kid = None
     return _JwtHmac(cc_mac, algorithm, custom_kid)
 
-  def key_type(self) -> Text:
+  def key_type(self) -> str:
     return self._cc_key_manager.key_type()
 
   @core.use_tink_errors
   def new_key_data(self,
                    key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyData:
     data = self._cc_key_manager.new_key_data(key_template.SerializeToString())
     return tink_pb2.KeyData.FromString(data)
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_format.py` & `tink-1.7.0/tink/jwt/_jwt_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Functions that help to serialize and deserialize from/to the JWT format."""
 
 import base64
 import binascii
-import json
 import struct
-from typing import Any, Optional, Text, Tuple
+from typing import Any, Optional, Tuple
 
 from tink.proto import tink_pb2
+from tink.jwt import _json_util
 from tink.jwt import _jwt_error
+from tink.jwt import _raw_jwt
 
 _VALID_ALGORITHMS = frozenset({
     'HS256', 'HS384', 'HS512', 'ES256', 'ES384', 'ES512', 'RS256', 'RS384',
     'RS384', 'RS512', 'PS256', 'PS384', 'PS512'
 })
 
 
-def _base64_encode(data: bytes) -> bytes:
+def base64_encode(data: bytes) -> bytes:
   """Does a URL-safe base64 encoding without padding."""
   return base64.urlsafe_b64encode(data).rstrip(b'=')
 
 
 def _is_valid_urlsafe_base64_char(c: int) -> bool:
   if c >= ord('a') and c <= ord('z'):
     return True
@@ -41,142 +42,111 @@
   if c >= ord('0') and c <= ord('9'):
     return True
   if c == ord('-') or c == ord('_'):
     return True
   return False
 
 
-def _base64_decode(encoded_data: bytes) -> bytes:
+def base64_decode(encoded_data: bytes) -> bytes:
   """Does a URL-safe base64 decoding without padding."""
   # base64.urlsafe_b64decode ignores all non-base64 chars. We don't want that.
   for c in encoded_data:
     if not _is_valid_urlsafe_base64_char(c):
-      raise _jwt_error.JwtInvalidError('invalid token')
+      raise _jwt_error.JwtInvalidError('invalid base64 encoding')
   # base64.urlsafe_b64decode requires padding, but does not mind too much
-  # padding. So we simply add the maximum ammount of padding needed.
+  # padding. So we simply add the maximum amount of padding needed.
   padded_encoded_data = encoded_data + b'==='
   try:
     return base64.urlsafe_b64decode(padded_encoded_data)
   except binascii.Error:
     # Throws when the length of encoded_data is (4*i + 1) for some i
-    raise _jwt_error.JwtInvalidError('invalid token')
-
-
-def json_dumps(json_data: Any) -> Text:
-  return json.dumps(json_data, separators=(',', ':'))
-
-
-def validate_all_strings(json_data: Any):
-  """Recursivly visits all strings and raises UnicodeEncodeError if invalid."""
-  if isinstance(json_data, str):
-    # We use encode('utf8') to validate that the string is valid.
-    json_data.encode('utf8')
-  if isinstance(json_data, list):
-    for item in json_data:
-      validate_all_strings(item)
-  if isinstance(json_data, dict):
-    for key, value in json_data.items():
-      key.encode('utf8')
-      validate_all_strings(value)
-
-
-def json_loads(json_text: Text) -> Any:
-  """Does the same as json.loads, but with some additinal validation."""
-  try:
-    json_data = json.loads(json_text)
-    validate_all_strings(json_data)
-    return json_data
-  except json.decoder.JSONDecodeError:
-    raise _jwt_error.JwtInvalidError('Failed to parse JSON string')
-  except RecursionError:
-    raise _jwt_error.JwtInvalidError(
-        'Failed to parse JSON string, too many recursions')
-  except UnicodeEncodeError:
-    raise _jwt_error.JwtInvalidError('invalid character')
+    raise _jwt_error.JwtInvalidError('invalid base64 encoding')
 
 
-def _validate_algorithm(algorithm: Text) -> None:
+def _validate_algorithm(algorithm: str) -> None:
   if algorithm not in _VALID_ALGORITHMS:
     raise _jwt_error.JwtInvalidError('Invalid algorithm %s' % algorithm)
 
 
-def encode_header(json_header: Text) -> bytes:
+def encode_header(json_header: str) -> bytes:
   try:
-    return _base64_encode(json_header.encode('utf8'))
+    return base64_encode(json_header.encode('utf8'))
   except UnicodeEncodeError:
     raise _jwt_error.JwtInvalidError('invalid token')
 
 
-def decode_header(encoded_header: bytes) -> Text:
+def decode_header(encoded_header: bytes) -> str:
   try:
-    return _base64_decode(encoded_header).decode('utf8')
+    return base64_decode(encoded_header).decode('utf8')
   except UnicodeDecodeError:
     raise _jwt_error.JwtInvalidError('invalid token')
 
 
-def encode_payload(json_payload: Text) -> bytes:
+def encode_payload(json_payload: str) -> bytes:
   """Encodes the payload into compact form."""
   try:
-    return _base64_encode(json_payload.encode('utf8'))
+    return base64_encode(json_payload.encode('utf8'))
   except UnicodeEncodeError:
     raise _jwt_error.JwtInvalidError('invalid token')
 
 
-def decode_payload(encoded_payload: bytes) -> Text:
+def decode_payload(encoded_payload: bytes) -> str:
   """Decodes the payload from compact form."""
   try:
-    return _base64_decode(encoded_payload).decode('utf8')
+    return base64_decode(encoded_payload).decode('utf8')
   except UnicodeDecodeError:
     raise _jwt_error.JwtInvalidError('invalid token')
 
 
 def encode_signature(signature: bytes) -> bytes:
   """Encodes the signature."""
-  return _base64_encode(signature)
+  return base64_encode(signature)
 
 
 def decode_signature(encoded_signature: bytes) -> bytes:
   """Decodes the signature."""
-  return _base64_decode(encoded_signature)
+  return base64_decode(encoded_signature)
 
 
-def create_header(algorithm: Text, type_header: Optional[Text],
-                  kid: Optional[Text]) -> bytes:
+def create_header(algorithm: str, type_header: Optional[str],
+                  kid: Optional[str]) -> bytes:
   _validate_algorithm(algorithm)
   header = {}
   if kid:
     header['kid'] = kid
   header['alg'] = algorithm
   if type_header:
     header['typ'] = type_header
-  return encode_header(json_dumps(header))
+  return encode_header(_json_util.json_dumps(header))
 
 
-def get_kid(key_id: int, prefix: tink_pb2.OutputPrefixType) -> Optional[Text]:
+def get_kid(key_id: int, prefix: tink_pb2.OutputPrefixType) -> Optional[str]:
   """Returns the encoded key_id, or None."""
   if prefix == tink_pb2.RAW:
     return None
   if prefix == tink_pb2.TINK:
     if key_id < 0 or key_id > 2**32:
       raise _jwt_error.JwtInvalidError('invalid key_id')
-    return _base64_encode(struct.pack('>L', key_id)).decode('utf8')
+    return base64_encode(struct.pack('>L', key_id)).decode('utf8')
   raise _jwt_error.JwtInvalidError('unexpected output prefix type')
 
 
-def split_signed_compact(
-    signed_compact: Text) -> Tuple[bytes, Text, Text, bytes]:
+def split_signed_compact(signed_compact: str) -> Tuple[bytes, str, str, bytes]:
   """Splits a signed compact into its parts.
 
   Args:
     signed_compact: A signed compact JWT.
+
   Returns:
     A (unsigned_compact, json_header, json_payload, signature_or_mac) tuple.
   Raises:
     _jwt_error.JwtInvalidError if it fails.
   """
+  if not isinstance(signed_compact, str):
+    raise _jwt_error.JwtInvalidError('invalid token: not a str')
   try:
     encoded = signed_compact.encode('utf8')
   except UnicodeEncodeError:
     raise _jwt_error.JwtInvalidError('invalid token')
   try:
     unsigned_compact, encoded_signature = encoded.rsplit(b'.', 1)
   except ValueError:
@@ -188,32 +158,51 @@
     raise _jwt_error.JwtInvalidError('invalid token')
 
   json_header = decode_header(encoded_header)
   json_payload = decode_payload(encoded_payload)
   return (unsigned_compact, json_header, json_payload, signature_or_mac)
 
 
-def validate_header(header: Any, algorithm: Text) -> None:
+def _validate_kid_header(header: Any, kid: str) -> None:
+  if header['kid'] != kid:
+    raise _jwt_error.JwtInvalidError('invalid kid header')
+
+
+def validate_header(header: Any,
+                    algorithm: str,
+                    tink_kid: Optional[str] = None,
+                    custom_kid: Optional[str] = None) -> None:
   """Parses the header and validates its values."""
   _validate_algorithm(algorithm)
   hdr_algorithm = header.get('alg', '')
   if hdr_algorithm.upper() != algorithm:
     raise _jwt_error.JwtInvalidError('Invalid algorithm; expected %s, got %s' %
                                      (algorithm, hdr_algorithm))
   if 'crit' in header:
     raise _jwt_error.JwtInvalidError(
         'all tokens with crit headers are rejected')
+  if tink_kid is not None and custom_kid is not None:
+    raise _jwt_error.JwtInvalidError('custom_kid can only be set for RAW keys')
+  if tink_kid is not None:
+    if 'kid' not in header:
+      # for output prefix type TINK, the kid header is required
+      raise _jwt_error.JwtInvalidError('missing kid in header')
+    _validate_kid_header(header, tink_kid)
+  if custom_kid is not None and 'kid' in header:
+    _validate_kid_header(header, custom_kid)
 
 
-def get_type_header(header: Any) -> Optional[Text]:
+def get_type_header(header: Any) -> Optional[str]:
   return header.get('typ', None)
 
 
-# TODO(juerg): Refactor this to create_unsigned_compact(algorithm, kid, raw_jwt)
-def create_unsigned_compact(algorithm: Text, typ_header: Optional[Text],
-                            kid: Optional[Text], json_payload: Text) -> bytes:
-  header = create_header(algorithm, typ_header, kid)
-  return header + b'.' + encode_payload(json_payload)
+def create_unsigned_compact(algorithm: str, kid: Optional[str],
+                            raw_jwt: _raw_jwt.RawJwt) -> bytes:
+  if raw_jwt.has_type_header():
+    header = create_header(algorithm, raw_jwt.type_header(), kid)
+  else:
+    header = create_header(algorithm, None, kid)
+  return header + b'.' + encode_payload(raw_jwt.json_payload())
 
 
-def create_signed_compact(unsigned_compact: bytes, signature: bytes) -> Text:
+def create_signed_compact(unsigned_compact: bytes, signature: bytes) -> str:
   return (unsigned_compact + b'.' + encode_signature(signature)).decode('utf8')
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_signature_wrappers_test.py` & `tink-1.7.0/tink/jwt/_jwt_signature_wrappers_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,70 +9,112 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink.jwt._jwt_signature_wrappers_test."""
 
+import io
+
+
 from absl.testing import absltest
 from absl.testing import parameterized
 
 from tink.proto import jwt_ecdsa_pb2
 from tink.proto import jwt_rsa_ssa_pkcs1_pb2
 from tink.proto import jwt_rsa_ssa_pss_pb2
 from tink.proto import tink_pb2
 import tink
+from tink import cleartext_keyset_handle
 from tink import jwt
+from tink.jwt import _json_util
 from tink.jwt import _jwt_format
+
 from tink.testing import keyset_builder
 
 
-def setUpModule():
-  jwt.register_jwt_signature()
+LONG_CUSTOM_KID = 'Lorem ipsum dolor sit amet, consectetur adipiscing elit'
 
 
-def _create_jwt_ecdsa_template(
-    algorithm: jwt_ecdsa_pb2.JwtEcdsaAlgorithm,
-    output_prefix_type: tink_pb2.OutputPrefixType) -> tink_pb2.KeyTemplate:
-  key_format = jwt_ecdsa_pb2.JwtEcdsaKeyFormat(algorithm=algorithm)
-  return tink_pb2.KeyTemplate(
-      type_url='type.googleapis.com/google.crypto.tink.JwtEcdsaPrivateKey',
-      value=key_format.SerializeToString(),
-      output_prefix_type=output_prefix_type)
+def setUpModule():
+  jwt.register_jwt_signature()
 
 
-def jwt_es256_tink_template():
-  return _create_jwt_ecdsa_template(jwt_ecdsa_pb2.ES256, tink_pb2.TINK)
+def _change_key_id(keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
+  """Changes the key id of the first key and makes it primary."""
+  buffer = io.BytesIO()
+  cleartext_keyset_handle.write(
+      tink.BinaryKeysetWriter(buffer), keyset_handle)
+  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  # XOR the key id with an arbitrary 32-bit string to get a new key id.
+  new_key_id = keyset.key[0].key_id ^ 0xdeadbeef
+  keyset.key[0].key_id = new_key_id
+  keyset.primary_key_id = new_key_id
+  return cleartext_keyset_handle.from_keyset(keyset)
+
+
+def _change_output_prefix_to_tink(
+    keyset_handle: tink.KeysetHandle) -> tink.KeysetHandle:
+  """Changes the output prefix type of the first key to TINK."""
+  buffer = io.BytesIO()
+  cleartext_keyset_handle.write(
+      tink.BinaryKeysetWriter(buffer), keyset_handle)
+  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  keyset.key[0].output_prefix_type = tink_pb2.TINK
+  return cleartext_keyset_handle.from_keyset(keyset)
+
+
+def _set_custom_kid(keyset_handle: tink.KeysetHandle,
+                    custom_kid: str) -> tink.KeysetHandle:
+  """Sets the custom_kid field of the first key."""
+  buffer = io.BytesIO()
+  cleartext_keyset_handle.write(
+      tink.BinaryKeysetWriter(buffer), keyset_handle)
+  keyset = tink_pb2.Keyset.FromString(buffer.getvalue())
+  if keyset.key[0].key_data.type_url.endswith('JwtEcdsaPrivateKey'):
+    jwt_ecdsa_key = jwt_ecdsa_pb2.JwtEcdsaPrivateKey.FromString(
+        keyset.key[0].key_data.value)
+    jwt_ecdsa_key.public_key.custom_kid.value = custom_kid
+    keyset.key[0].key_data.value = jwt_ecdsa_key.SerializeToString()
+  elif keyset.key[0].key_data.type_url.endswith('JwtRsaSsaPkcs1PrivateKey'):
+    rsa_key = jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1PrivateKey.FromString(
+        keyset.key[0].key_data.value)
+    rsa_key.public_key.custom_kid.value = custom_kid
+    keyset.key[0].key_data.value = rsa_key.SerializeToString()
+  elif keyset.key[0].key_data.type_url.endswith('JwtRsaSsaPssPrivateKey'):
+    rsa_key = jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssPrivateKey.FromString(
+        keyset.key[0].key_data.value)
+    rsa_key.public_key.custom_kid.value = custom_kid
+    keyset.key[0].key_data.value = rsa_key.SerializeToString()
+  else:
+    raise tink.TinkError('unknown key type')
+  return cleartext_keyset_handle.from_keyset(keyset)
 
 
 class JwtSignatureWrapperTest(parameterized.TestCase):
 
-  # TODO(juerg): Add tests with TINK templates
-
   def test_interesting_error(self):
     private_handle = tink.new_keyset_handle(jwt.jwt_es256_template())
     sign = private_handle.primitive(jwt.JwtPublicKeySign)
     verify = private_handle.public_keyset_handle().primitive(
         jwt.JwtPublicKeyVerify)
     raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
     compact = sign.sign_and_encode(raw_jwt)
     with self.assertRaisesRegex(jwt.JwtInvalidError,
                                 'invalid JWT; expected issuer'):
       verify.verify_and_decode(compact, jwt.new_validator(
           expected_issuer='unknown', allow_missing_expiration=True))
 
   @parameterized.parameters([
+      (jwt.raw_jwt_es256_template(), jwt.raw_jwt_es256_template()),
+      (jwt.raw_jwt_es256_template(), jwt.jwt_es256_template()),
+      (jwt.jwt_es256_template(), jwt.raw_jwt_es256_template()),
       (jwt.jwt_es256_template(), jwt.jwt_es256_template()),
-      (jwt.jwt_es256_template(), jwt_es256_tink_template()),
-      (jwt_es256_tink_template, jwt.jwt_es256_template()),
-      (jwt_es256_tink_template(), jwt_es256_tink_template()),
   ])
   def test_key_rotation(self, old_key_tmpl, new_key_tmpl):
-    old_key_tmpl = jwt.jwt_es256_template()
-    new_key_tmpl = jwt.jwt_es384_template()
     builder = keyset_builder.new_keyset_builder()
     older_key_id = builder.add_new_key(old_key_tmpl)
 
     builder.set_primary_key(older_key_id)
     handle1 = builder.keyset_handle()
     sign1 = handle1.primitive(jwt.JwtPublicKeySign)
     verify1 = handle1.public_keyset_handle().primitive(jwt.JwtPublicKeyVerify)
@@ -137,115 +179,136 @@
     self.assertEqual(
         verify2.verify_and_decode(compact4, validator).issuer(), 'a')
     self.assertEqual(
         verify3.verify_and_decode(compact4, validator).issuer(), 'a')
     self.assertEqual(
         verify4.verify_and_decode(compact4, validator).issuer(), 'a')
 
-  def test_tink_output_prefix_type_encodes_a_kid_header(self):
-    keyset_handle = tink.new_keyset_handle(jwt_es256_tink_template())
-    sign = keyset_handle.primitive(jwt.JwtPublicKeySign)
+  def test_only_tink_output_prefix_type_encodes_a_kid_header(self):
+    handle = tink.new_keyset_handle(jwt.raw_jwt_es256_template())
+    sign = handle.primitive(jwt.JwtPublicKeySign)
+    verify = handle.public_keyset_handle().primitive(jwt.JwtPublicKeyVerify)
+
+    tink_handle = _change_output_prefix_to_tink(handle)
+    tink_sign = tink_handle.primitive(jwt.JwtPublicKeySign)
+    tink_verify = tink_handle.public_keyset_handle().primitive(
+        jwt.JwtPublicKeyVerify)
 
     raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
-    signed_compact = sign.sign_and_encode(raw_jwt)
 
-    _, json_header, _, _ = _jwt_format.split_signed_compact(signed_compact)
-    header = _jwt_format.json_loads(json_header)
-    self.assertIn('kid', header)
-
-  def test_es256_key_with_custom_kid_header(self):
-    keyset_handle = tink.new_keyset_handle(jwt.raw_jwt_es256_template())
-
-    # Add a custom kid to the key in keyset_handle
-    value = keyset_handle._keyset.key[0].key_data.value
-    ecdsa_key = jwt_ecdsa_pb2.JwtEcdsaPrivateKey.FromString(value)
-    ecdsa_key.public_key.custom_kid.value = 'my kid'
-    keyset_handle._keyset.key[0].key_data.value = ecdsa_key.SerializeToString()
-    sign = keyset_handle.primitive(jwt.JwtPublicKeySign)
+    token = sign.sign_and_encode(raw_jwt)
+    token_with_kid = tink_sign.sign_and_encode(raw_jwt)
 
-    raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
-    signed_compact = sign.sign_and_encode(raw_jwt)
+    _, header, _, _ = _jwt_format.split_signed_compact(token)
+    self.assertNotIn('kid', _json_util.json_loads(header))
 
-    _, json_header, _, _ = _jwt_format.split_signed_compact(signed_compact)
-    header = _jwt_format.json_loads(json_header)
-    self.assertEqual(header['kid'], 'my kid')
+    _, header_with_kid, _, _ = _jwt_format.split_signed_compact(token_with_kid)
+    self.assertIn('kid', _json_util.json_loads(header_with_kid))
 
-    # Now, change the output prefix type to TINK. This should fail.
-    keyset_handle._keyset.key[0].output_prefix_type = tink_pb2.TINK
-    with self.assertRaises(tink.TinkError):
-      tink_sign = keyset_handle.primitive(jwt.JwtPublicKeySign)
-      tink_sign.sign_and_encode(raw_jwt)
+    validator = jwt.new_validator(
+        expected_issuer='issuer', allow_missing_expiration=True)
 
-  def test_rs256_key_with_custom_kid_header(self):
-    keyset_handle = tink.new_keyset_handle(jwt.raw_jwt_rs256_2048_f4_template())
+    verify.verify_and_decode(token, validator)
+    tink_verify.verify_and_decode(token_with_kid, validator)
 
-    # Add a custom kid to the key in keyset_handle
-    value = keyset_handle._keyset.key[0].key_data.value
-    pkcs1_key = jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1PrivateKey.FromString(value)
-    pkcs1_key.public_key.custom_kid.value = 'my kid'
-    keyset_handle._keyset.key[0].key_data.value = pkcs1_key.SerializeToString()
+    other_handle = _change_key_id(tink_handle)
+    other_verify = other_handle.public_keyset_handle().primitive(
+        jwt.JwtPublicKeyVerify)
 
-    sign = keyset_handle.primitive(jwt.JwtPublicKeySign)
+    verify.verify_and_decode(token_with_kid, validator)
+    # For output prefix type TINK, the kid header is required.
+    with self.assertRaises(tink.TinkError):
+      tink_verify.verify_and_decode(token, validator)
+    # This should fail because value of the kid header is wrong.
+    with self.assertRaises(tink.TinkError):
+      other_verify.verify_and_decode(token_with_kid, validator)
 
+  @parameterized.named_parameters([
+      ('JWT_ES256_RAW', jwt.raw_jwt_es256_template()),
+      ('JWT_RS256_RAW', jwt.raw_jwt_rs256_2048_f4_template()),
+      ('JWT_PS256_RAW', jwt.raw_jwt_ps256_3072_f4_template()),
+  ])
+  def test_raw_key_with_custom_kid_header(self, template):
+    # normal key with output prefix RAW
+    handle = tink.new_keyset_handle(template)
     raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
-    signed_compact = sign.sign_and_encode(raw_jwt)
-
-    _, json_header, _, _ = _jwt_format.split_signed_compact(signed_compact)
-    header = _jwt_format.json_loads(json_header)
-    self.assertEqual(header['kid'], 'my kid')
-
-    # Now, change the output prefix type to TINK. This should fail.
-    keyset_handle._keyset.key[0].output_prefix_type = tink_pb2.TINK
-    with self.assertRaises(tink.TinkError):
-      tink_sign = keyset_handle.primitive(jwt.JwtPublicKeySign)
-      tink_sign.sign_and_encode(raw_jwt)
+    validator = jwt.new_validator(
+        expected_issuer='issuer', allow_missing_expiration=True)
 
-  def test_ps256_key_with_a_custom_kid_header(self):
-    keyset_handle = tink.new_keyset_handle(jwt.raw_jwt_ps256_2048_f4_template())
+    sign = handle.primitive(jwt.JwtPublicKeySign)
+    token = sign.sign_and_encode(raw_jwt)
+    verify = handle.public_keyset_handle().primitive(jwt.JwtPublicKeyVerify)
+    verify.verify_and_decode(token, validator)
+
+    _, json_header, _, _ = _jwt_format.split_signed_compact(token)
+    self.assertNotIn('kid', _json_util.json_loads(json_header))
+
+    # key with a custom_kid set
+    custom_kid_handle = _set_custom_kid(handle, custom_kid=LONG_CUSTOM_KID)
+    custom_kid_sign = custom_kid_handle.primitive(jwt.JwtPublicKeySign)
+    token_with_kid = custom_kid_sign.sign_and_encode(raw_jwt)
+    custom_kid_verify = custom_kid_handle.public_keyset_handle().primitive(
+        jwt.JwtPublicKeyVerify)
+    custom_kid_verify.verify_and_decode(token_with_kid, validator)
 
-    # Add a custom kid to the key in keyset_handle
-    value = keyset_handle._keyset.key[0].key_data.value
-    pss_key = jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssPrivateKey.FromString(value)
-    pss_key.public_key.custom_kid.value = 'my kid'
-    keyset_handle._keyset.key[0].key_data.value = pss_key.SerializeToString()
+    _, header_with_kid, _, _ = _jwt_format.split_signed_compact(token_with_kid)
+    self.assertEqual(_json_util.json_loads(header_with_kid)['kid'],
+                     LONG_CUSTOM_KID)
 
-    sign = keyset_handle.primitive(jwt.JwtPublicKeySign)
+    # The primitive with a custom_kid set accepts tokens without kid header.
+    custom_kid_verify.verify_and_decode(token, validator)
 
-    raw_jwt = jwt.new_raw_jwt(issuer='issuer', without_expiration=True)
-    signed_compact = sign.sign_and_encode(raw_jwt)
+    # The primitive without a custom_kid set ignores the kid header.
+    verify.verify_and_decode(token_with_kid, validator)
 
-    _, json_header, _, _ = _jwt_format.split_signed_compact(signed_compact)
-    header = _jwt_format.json_loads(json_header)
-    self.assertEqual(header['kid'], 'my kid')
+    # key with a different custom_kid set
+    other_handle = _set_custom_kid(handle, custom_kid='other kid')
+    other_verify = other_handle.public_keyset_handle().primitive(
+        jwt.JwtPublicKeyVerify)
+    # Fails because the kid value do not match.
+    with self.assertRaises(tink.TinkError):
+      other_verify.verify_and_decode(token_with_kid, validator)
 
-    # Now, change the output prefix type to TINK. This should fail.
-    keyset_handle._keyset.key[0].output_prefix_type = tink_pb2.TINK
+    tink_handle = _change_output_prefix_to_tink(custom_kid_handle)
+    tink_sign = tink_handle.primitive(jwt.JwtPublicKeySign)
+    tink_verify = tink_handle.public_keyset_handle().primitive(
+        jwt.JwtPublicKeyVerify)
+    # Having custom_kid set with output prefix TINK is not allowed.
     with self.assertRaises(tink.TinkError):
-      tink_sign = keyset_handle.primitive(jwt.JwtPublicKeySign)
       tink_sign.sign_and_encode(raw_jwt)
+    with self.assertRaises(tink.TinkError):
+      tink_verify.verify_and_decode(token, validator)
+    with self.assertRaises(tink.TinkError):
+      tink_verify.verify_and_decode(token_with_kid, validator)
 
   def test_legacy_template_fails(self):
-    template = _create_jwt_ecdsa_template(jwt_ecdsa_pb2.ES256, tink_pb2.LEGACY)
+    template = keyset_builder.legacy_template(jwt.jwt_es256_template())
     builder = keyset_builder.new_keyset_builder()
     key_id = builder.add_new_key(template)
     builder.set_primary_key(key_id)
     handle = builder.keyset_handle()
     with self.assertRaises(tink.TinkError):
       handle.primitive(jwt.JwtPublicKeySign)
     with self.assertRaises(tink.TinkError):
       handle.public_keyset_handle().primitive(jwt.JwtPublicKeyVerify)
 
   def test_legacy_non_primary_key_fails(self):
     builder = keyset_builder.new_keyset_builder()
-    old_template = _create_jwt_ecdsa_template(jwt_ecdsa_pb2.ES256,
-                                              tink_pb2.LEGACY)
+    old_template = keyset_builder.legacy_template(jwt.jwt_es256_template())
     _ = builder.add_new_key(old_template)
     current_key_id = builder.add_new_key(jwt.jwt_es256_template())
     builder.set_primary_key(current_key_id)
     handle = builder.keyset_handle()
     with self.assertRaises(tink.TinkError):
       handle.primitive(jwt.JwtPublicKeySign)
     with self.assertRaises(tink.TinkError):
       handle.public_keyset_handle().primitive(jwt.JwtPublicKeyVerify)
 
+  def test_jwt_mac_from_keyset_without_primary_fails(self):
+    builder = keyset_builder.new_keyset_builder()
+    builder.add_new_key(jwt.jwt_es256_template())
+    with self.assertRaises(tink.TinkError):
+      builder.keyset_handle()
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_error.py` & `tink-1.7.0/tink/prf/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Copyright 2021 Google LLC
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Defines an Invalid JWT Error."""
+"""PrfSet package."""
 
-from tink import core
+from tink.prf import _prf_key_manager
+from tink.prf import _prf_key_templates as prf_key_templates
+from tink.prf import _prf_set
 
-
-class JwtInvalidError(core.TinkError):
-  pass
+Prf = _prf_set.Prf
+PrfSet = _prf_set.PrfSet
+register = _prf_key_manager.register
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_key_templates.py` & `tink-1.7.0/tink/jwt/_jwt_key_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 """Pre-generated JWT KeyTemplate."""
 
 from tink.proto import jwt_ecdsa_pb2
 from tink.proto import jwt_hmac_pb2
 from tink.proto import jwt_rsa_ssa_pkcs1_pb2
 from tink.proto import jwt_rsa_ssa_pss_pb2
 from tink.proto import tink_pb2
+from tink.internal import big_integer_util
 
 
 _F4 = 65537
 
-# TODO(juerg): Add TINK key templates.
-
 
 def _create_jwt_hmac_template(
     algorithm: jwt_hmac_pb2.JwtHmacAlgorithm, key_size: int,
     output_prefix_type: tink_pb2.OutputPrefixType) -> tink_pb2.KeyTemplate:
   key_format = jwt_hmac_pb2.JwtHmacKeyFormat(
       algorithm=algorithm, key_size=key_size)
   return tink_pb2.KeyTemplate(
@@ -42,48 +41,34 @@
       algorithm=algorithm)
   return tink_pb2.KeyTemplate(
       type_url='type.googleapis.com/google.crypto.tink.JwtEcdsaPrivateKey',
       value=key_format.SerializeToString(),
       output_prefix_type=output_prefix_type)
 
 
-# TODO(juerg): Move this function into a util lib.
-def _num_to_bytes(n: int) -> bytes:
-  """Converts a number to bytes."""
-  if n < 0:
-    raise OverflowError("number can't be negative")
-  if n == 0:
-    return b'\x00'
-  octets = bytearray()
-  while n:
-    octets.append(n % 256)
-    n //= 256
-  return bytes(octets[::-1])
-
-
 def _create_jwt_rsa_ssa_pkcs1_template(
     algorithm: jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1Algorithm, modulus_size: int,
     output_prefix_type: tink_pb2.OutputPrefixType) -> tink_pb2.KeyTemplate:
   key_format = jwt_rsa_ssa_pkcs1_pb2.JwtRsaSsaPkcs1KeyFormat(
       algorithm=algorithm,
       modulus_size_in_bits=modulus_size,
-      public_exponent=_num_to_bytes(_F4))
+      public_exponent=big_integer_util.num_to_bytes(_F4))
   return tink_pb2.KeyTemplate(
       type_url='type.googleapis.com/google.crypto.tink.JwtRsaSsaPkcs1PrivateKey',
       value=key_format.SerializeToString(),
       output_prefix_type=output_prefix_type)
 
 
 def _create_jwt_rsa_ssa_pss_template(
     algorithm: jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssAlgorithm, modulus_size: int,
     output_prefix_type: tink_pb2.OutputPrefixType) -> tink_pb2.KeyTemplate:
   key_format = jwt_rsa_ssa_pss_pb2.JwtRsaSsaPssKeyFormat(
       algorithm=algorithm,
       modulus_size_in_bits=modulus_size,
-      public_exponent=_num_to_bytes(_F4))
+      public_exponent=big_integer_util.num_to_bytes(_F4))
   return tink_pb2.KeyTemplate(
       type_url='type.googleapis.com/google.crypto.tink.JwtRsaSsaPssPrivateKey',
       value=key_format.SerializeToString(),
       output_prefix_type=output_prefix_type)
 
 
 # Hmac Templates
```

### Comparing `tink-1.6.1/tink/jwt/_raw_jwt_test.py` & `tink-1.7.0/tink/jwt/_raw_jwt_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 """Tests for tink.python.tink.jwt._raw_jwt."""
 
 import datetime
 import json
 
-from typing import cast, Dict, List, Text
+from typing import cast, Dict, List
 
 from absl.testing import absltest
 # from absl.testing import parameterized
 
 from tink import jwt
 
 ISSUED_AT_TIMESTAMP = 1582230020
@@ -90,22 +90,27 @@
     self.assertEqual(token.subject(), 'Subject')
 
   def test_jwt_id(self):
     token = jwt.new_raw_jwt(jwt_id='JWT ID', without_expiration=True)
     self.assertTrue(token.has_jwt_id())
     self.assertEqual(token.jwt_id(), 'JWT ID')
 
+  def test_audience(self):
+    token = jwt.new_raw_jwt(audience='bob', without_expiration=True)
+    self.assertTrue(token.has_audiences())
+    self.assertEqual(token.audiences(), ['bob'])
+
   def test_audiences(self):
     token = jwt.new_raw_jwt(audiences=['bob', 'eve'], without_expiration=True)
     self.assertTrue(token.has_audiences())
     self.assertEqual(token.audiences(), ['bob', 'eve'])
 
   def test_string_audiences(self):
     token = jwt.new_raw_jwt(
-        audiences=cast(List[Text], 'bob'), without_expiration=True)
+        audiences=cast(List[str], 'bob'), without_expiration=True)
     self.assertTrue(token.has_audiences())
     self.assertEqual(token.audiences(), ['bob'])
 
   def test_empty_audiences(self):
     with self.assertRaises(jwt.JwtInvalidError):
       jwt.new_raw_jwt(audiences=[], without_expiration=True)
 
@@ -257,14 +262,18 @@
             'amount': 1.5,
             'name': 'Peter',
             'null': None,
             'array': [1, None, 'Bob', 2.2, {'foo': 'bar'}],
             'object': {'one': {'two': 3}}
         })
 
+  def test_string_audience_payload(self):
+    token = jwt.new_raw_jwt(audience='bob', without_expiration=True)
+    self.assertEqual(json.loads(token.json_payload()), {'aud': 'bob'})
+
   def test_from_to_payload(self):
     payload = {
         'iss': 'Issuer',
         'sub': 'Subject',
         'jti': 'JWT ID',
         'aud': ['bob', 'eve'],
         'iat': ISSUED_AT_TIMESTAMP,
@@ -273,97 +282,109 @@
         'account_no': 1234,
         'amount': 1.5,
         'name': 'Peter',
         'null': None,
         'array': [1, None, 'Bob', 2.2, {'foo': 'bar'}],
         'object': {'one': {'two': 3}}
     }
-    token = jwt.RawJwt.from_json(None, json.dumps(payload))
+    token = jwt.RawJwt._from_json(None, json.dumps(payload))
     self.assertEqual(json.loads(token.json_payload()), payload)
 
   def test_exp_to_payload(self):
     expiration = datetime.datetime.fromtimestamp(2218027244,
                                                  datetime.timezone.utc)
     token = jwt.new_raw_jwt(expiration=expiration)
     self.assertEqual(token.json_payload(), '{"exp":2218027244}')
 
   def test_float_exp_to_payload(self):
     expiration = datetime.datetime.fromtimestamp(123.999, datetime.timezone.utc)
     token = jwt.new_raw_jwt(expiration=expiration)
     self.assertEqual(token.json_payload(), '{"exp":123}')
 
-  def test_from_to_payload_with_string_audience(self):
+  def test_from_to_payload_with_string_audience_perserves_string(self):
     payload = {
         'iss': 'Issuer',
         'aud': 'bob',
     }
-    token = jwt.RawJwt.from_json(None, json.dumps(payload))
+    token = jwt.RawJwt._from_json(None, json.dumps(payload))
+    expected = {
+        'iss': 'Issuer',
+        'aud': 'bob',
+    }
+    self.assertEqual(json.loads(token.json_payload()), expected)
+
+  def test_from_to_payload_with_list_audience_perserves_list(self):
+    payload = {
+        'iss': 'Issuer',
+        'aud': ['bob'],
+    }
+    token = jwt.RawJwt._from_json(None, json.dumps(payload))
     expected = {
         'iss': 'Issuer',
         'aud': ['bob'],
     }
     self.assertEqual(json.loads(token.json_payload()), expected)
 
   def test_from_payload_with_wrong_issuer_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"iss":123}')
+      jwt.RawJwt._from_json(None, '{"iss":123}')
 
   def test_from_payload_with_wrong_subject_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"sub":123}')
+      jwt.RawJwt._from_json(None, '{"sub":123}')
 
   def test_from_payload_with_wrong_jwt_id_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"jti":123}')
+      jwt.RawJwt._from_json(None, '{"jti":123}')
 
   def test_from_payload_with_wrong_expiration_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"exp":"123"}')
+      jwt.RawJwt._from_json(None, '{"exp":"123"}')
 
   def test_from_payload_with_wrong_issued_at_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"iat":"123"}')
+      jwt.RawJwt._from_json(None, '{"iat":"123"}')
 
   def test_from_payload_with_wrong_not_before_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"nbf":"123"}')
+      jwt.RawJwt._from_json(None, '{"nbf":"123"}')
 
   def test_from_payload_with_exp_expiration_success(self):
-    token = jwt.RawJwt.from_json(None, '{"exp":1e10}')
+    token = jwt.RawJwt._from_json(None, '{"exp":1e10}')
     self.assertEqual(
         token.expiration(),
         datetime.datetime.fromtimestamp(10000000000, datetime.timezone.utc))
 
   def test_from_payload_with_large_expiration_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"exp":1e30}')
+      jwt.RawJwt._from_json(None, '{"exp":1e30}')
 
   def test_from_payload_with_negative_expiration_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"exp":-1}')
+      jwt.RawJwt._from_json(None, '{"exp":-1}')
 
   def test_from_payload_with_infinity_expiration_fails(self):
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, '{"exp":Infinity}')
+      jwt.RawJwt._from_json(None, '{"exp":Infinity}')
 
   def test_from_payload_with_utf16_surrogate(self):
     # the json string contains "\uD834\uDD1E", which the JSON decoder decodes to
     # the G clef character (U+1D11E).
-    token = jwt.RawJwt.from_json(None, u'{"iss":"\\uD834\\uDD1E"}')
+    token = jwt.RawJwt._from_json(None, u'{"iss":"\\uD834\\uDD1E"}')
     self.assertEqual(token.issuer(), u'\U0001d11e')
 
   def test_from_payload_with_invalid_utf16(self):
     # the json string contains "\uD834", which gets decoded by the json decoder
     # into an invalid UTF16 character.
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, u'{"iss":"\\uD834"}')
+      jwt.RawJwt._from_json(None, u'{"iss":"\\uD834"}')
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, u'{"\\uD834":"issuer"}')
+      jwt.RawJwt._from_json(None, u'{"\\uD834":"issuer"}')
     with self.assertRaises(jwt.JwtInvalidError):
-      jwt.RawJwt.from_json(None, u'{"a":{"a":{"a":"\\uD834"}}}')
+      jwt.RawJwt._from_json(None, u'{"a":{"a":{"a":"\\uD834"}}}')
 
   def test_modification(self):
     audiences = ['alice', 'bob']
     my_claim = {'one': 'two'}
     custom_claims = {'my_claim': my_claim}
     token = jwt.new_raw_jwt(
         issuer='Issuer',
@@ -371,15 +392,15 @@
         custom_claims=custom_claims,
         without_expiration=True)
 
     # modify inputs and outputs of token
     audiences.append('eve')
     custom_claims['new_claim'] = 456
     my_claim['three'] = 4
-    output_claim = cast(Dict[Text, Text], token.custom_claim('my_claim'))
+    output_claim = cast(Dict[str, str], token.custom_claim('my_claim'))
     output_claim['three'] = 4  # pytype: disable=container-type-mismatch
 
     # modifications don't affect token.
     self.assertEqual(token.audiences(), ['alice', 'bob'])
     self.assertEqual(token.custom_claim_names(), {'my_claim'})
     self.assertEqual(token.custom_claim('my_claim'), {'one': 'two'})
     with self.assertRaises(KeyError):
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_validator_test.py` & `tink-1.7.0/tink/jwt/_jwt_validator_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,52 +23,45 @@
 
   def test_validator_getters(self):
     fixed_now = datetime.datetime.fromtimestamp(12345, datetime.timezone.utc)
     clock_skew = datetime.timedelta(minutes=1)
     validator = jwt.new_validator(
         expected_type_header='type_header',
         expected_issuer='issuer',
-        expected_subject='subject',
         expected_audience='audience',
         fixed_now=fixed_now,
         clock_skew=clock_skew)
     self.assertTrue(validator.has_expected_type_header())
     self.assertEqual(validator.expected_type_header(), 'type_header')
     self.assertTrue(validator.has_expected_issuer())
     self.assertEqual(validator.expected_issuer(), 'issuer')
-    self.assertTrue(validator.has_expected_subject())
-    self.assertEqual(validator.expected_subject(), 'subject')
     self.assertTrue(validator.has_expected_audience())
     self.assertEqual(validator.expected_audience(), 'audience')
     self.assertFalse(validator.allow_missing_expiration())
     self.assertFalse(validator.ignore_issuer())
-    self.assertFalse(validator.ignore_subject())
     self.assertFalse(validator.ignore_audiences())
     self.assertTrue(validator.has_fixed_now())
     self.assertEqual(validator.fixed_now(), fixed_now)
     self.assertEqual(validator.clock_skew(), clock_skew)
 
   def test_validator_ignore_getters(self):
     validator = jwt.new_validator(
         allow_missing_expiration=True,
         ignore_type_header=True,
         ignore_issuer=True,
-        ignore_subject=True,
         ignore_audiences=True)
     self.assertTrue(validator.allow_missing_expiration())
     self.assertTrue(validator.ignore_type_header())
     self.assertTrue(validator.ignore_issuer())
-    self.assertTrue(validator.ignore_subject())
     self.assertTrue(validator.ignore_audiences())
 
   def test_empty_validator_getters(self):
     validator = jwt.new_validator()
     self.assertFalse(validator.has_expected_type_header())
     self.assertFalse(validator.has_expected_issuer())
-    self.assertFalse(validator.has_expected_subject())
     self.assertFalse(validator.has_expected_audience())
     self.assertFalse(validator.has_fixed_now())
     self.assertFalse(validator.clock_skew(), datetime.timedelta())
 
   def test_too_much_clock_skew(self):
     with self.assertRaises(ValueError):
       jwt.new_validator(clock_skew=datetime.timedelta(minutes=20))
@@ -128,14 +121,59 @@
     in_one_minute = (datetime.datetime.now(tz=datetime.timezone.utc)
                      + datetime.timedelta(minutes=1))
     token = jwt.new_raw_jwt(not_before=in_one_minute, without_expiration=True)
     validator = jwt.new_validator(
         allow_missing_expiration=True, clock_skew=datetime.timedelta(minutes=2))
     _jwt_validator.validate(validator, token)
 
+  def test_validate_issued_at(self):
+    in_one_minute = (datetime.datetime.now(tz=datetime.timezone.utc)
+                     + datetime.timedelta(minutes=1))
+    one_minute_ago = (datetime.datetime.now(tz=datetime.timezone.utc)
+                      - datetime.timedelta(minutes=1))
+    token_with_issued_at_in_the_future = jwt.new_raw_jwt(
+        issued_at=in_one_minute, without_expiration=True)
+    token_with_issued_at_in_the_past = jwt.new_raw_jwt(
+        issued_at=one_minute_ago, without_expiration=True)
+    token_without_issued_at = jwt.new_raw_jwt(without_expiration=True)
+
+    validator = jwt.new_validator(allow_missing_expiration=True)
+    _jwt_validator.validate(validator, token_with_issued_at_in_the_future)
+    _jwt_validator.validate(validator, token_with_issued_at_in_the_past)
+    _jwt_validator.validate(validator, token_without_issued_at)
+
+    issued_at_validator = jwt.new_validator(
+        expect_issued_in_the_past=True, allow_missing_expiration=True)
+    with self.assertRaises(jwt.JwtInvalidError):
+      _jwt_validator.validate(issued_at_validator,
+                              token_with_issued_at_in_the_future)
+    _jwt_validator.validate(issued_at_validator,
+                            token_with_issued_at_in_the_past)
+    with self.assertRaises(jwt.JwtInvalidError):
+      _jwt_validator.validate(issued_at_validator, token_without_issued_at)
+
+  def test_validate_issued_at_with_clock_skew(self):
+    in_one_minute = (datetime.datetime.now(tz=datetime.timezone.utc)
+                     + datetime.timedelta(minutes=1))
+    token_one_minute_in_the_future = jwt.new_raw_jwt(
+        issued_at=in_one_minute, without_expiration=True)
+
+    validator_without_clock_skew = jwt.new_validator(
+        expect_issued_in_the_past=True, allow_missing_expiration=True)
+    with self.assertRaises(jwt.JwtInvalidError):
+      _jwt_validator.validate(validator_without_clock_skew,
+                              token_one_minute_in_the_future)
+
+    validator_with_clock_skew = jwt.new_validator(
+        expect_issued_in_the_past=True,
+        allow_missing_expiration=True,
+        clock_skew=datetime.timedelta(minutes=2))
+    _jwt_validator.validate(validator_with_clock_skew,
+                            token_one_minute_in_the_future)
+
   def test_requires_type_header_but_no_type_header_set_fails(self):
     token = jwt.new_raw_jwt(without_expiration=True)
     validator = jwt.new_validator(
         expected_type_header='type_header', allow_missing_expiration=True)
     with self.assertRaises(jwt.JwtInvalidError):
       _jwt_validator.validate(validator, token)
 
@@ -200,50 +238,14 @@
         ignore_issuer=True, allow_missing_expiration=True)
     token_without_issuer = jwt.new_raw_jwt(without_expiration=True)
     _jwt_validator.validate(validator, token_without_issuer)
     token_with_issuer = jwt.new_raw_jwt(
         issuer='issuer', without_expiration=True)
     _jwt_validator.validate(validator, token_with_issuer)
 
-  def test_requires_subject_but_no_subject_set_fails(self):
-    token = jwt.new_raw_jwt(without_expiration=True)
-    validator = jwt.new_validator(
-        expected_subject='subject', allow_missing_expiration=True)
-    with self.assertRaises(jwt.JwtInvalidError):
-      _jwt_validator.validate(validator, token)
-
-  def test_invalid_subject_fails(self):
-    token = jwt.new_raw_jwt(subject='unknown', without_expiration=True)
-    validator = jwt.new_validator(
-        expected_subject='subject', allow_missing_expiration=True)
-    with self.assertRaises(jwt.JwtInvalidError):
-      _jwt_validator.validate(validator, token)
-
-  def test_correct_subject_success(self):
-    token = jwt.new_raw_jwt(subject='subject', without_expiration=True)
-    validator = jwt.new_validator(
-        expected_subject='subject', allow_missing_expiration=True)
-    _jwt_validator.validate(validator, token)
-
-  def test_subject_in_token_but_not_in_validator_fails(self):
-    validator = jwt.new_validator(allow_missing_expiration=True)
-    token_with_subject = jwt.new_raw_jwt(
-        subject='subject', without_expiration=True)
-    with self.assertRaises(jwt.JwtInvalidError):
-      _jwt_validator.validate(validator, token_with_subject)
-
-  def test_ignore_subject_success(self):
-    validator = jwt.new_validator(
-        ignore_subject=True, allow_missing_expiration=True)
-    token_without_subject = jwt.new_raw_jwt(without_expiration=True)
-    _jwt_validator.validate(validator, token_without_subject)
-    token_with_subject = jwt.new_raw_jwt(
-        subject='subject', without_expiration=True)
-    _jwt_validator.validate(validator, token_with_subject)
-
   def test_requires_audience_but_no_audience_set_fails(self):
     token = jwt.new_raw_jwt(without_expiration=True)
     validator = jwt.new_validator(
         expected_audience='audience', allow_missing_expiration=True)
     with self.assertRaises(jwt.JwtInvalidError):
       _jwt_validator.validate(validator, token)
 
@@ -305,22 +307,14 @@
     fixed_now = datetime.datetime.fromtimestamp(12345, datetime.timezone.utc)
     validator = jwt.new_validator(fixed_now=fixed_now)
     expiration = fixed_now + datetime.timedelta(minutes=1)
     not_before = fixed_now - datetime.timedelta(minutes=1)
     token = jwt.new_raw_jwt(expiration=expiration, not_before=not_before)
     _jwt_validator.validate(validator, token)
 
-  def test_validators_with_expected_and_ignored_fail(self):
-    with self.assertRaises(ValueError):
-      jwt.new_validator(expected_issuer='a', ignore_issuer=True)
-    with self.assertRaises(ValueError):
-      jwt.new_validator(expected_subject='a', ignore_subject=True)
-    with self.assertRaises(ValueError):
-      jwt.new_validator(expected_audience='a', ignore_audiences=True)
-
   def test_invalid_clock_skew_fail(self):
     with self.assertRaises(ValueError):
       jwt.new_validator(clock_skew=datetime.timedelta(minutes=1000))
 
   def test_fixed_now_without_timezone_fail(self):
     with self.assertRaises(ValueError):
       jwt.new_validator(fixed_now=datetime.datetime.fromtimestamp(12345))
```

### Comparing `tink-1.6.1/tink/jwt/_raw_jwt.py` & `tink-1.7.0/tink/jwt/_raw_jwt.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,126 +12,132 @@
 # See the License for the specific language governing permissions and
 """The raw JSON Web Token (JWT)."""
 
 import copy
 import datetime
 import json
 
-from typing import cast, Mapping, Set, List, Dict, Optional, Text, Union, Any
+from typing import cast, Mapping, Set, List, Dict, Optional, Union, Any
 
 from tink import core
+from tink.jwt import _json_util
 from tink.jwt import _jwt_error
-from tink.jwt import _jwt_format
 
 _REGISTERED_NAMES = frozenset({'iss', 'sub', 'jti', 'aud', 'exp', 'nbf', 'iat'})
 
 _MAX_TIMESTAMP_VALUE = 253402300799  # 31 Dec 9999, 23:59:59 GMT
 
-Claim = Union[None, bool, int, float, Text, List[Any], Dict[Text, Any]]
+Claim = Union[None, bool, int, float, str, List[Any], Dict[str, Any]]
 
 
 def _from_datetime(t: datetime.datetime) -> int:
   if not t.tzinfo:
     raise _jwt_error.JwtInvalidError('datetime must have tzinfo')
   return int(t.timestamp())
 
 
 def _to_datetime(timestamp: float) -> datetime.datetime:
   return datetime.datetime.fromtimestamp(timestamp, datetime.timezone.utc)
 
 
-def _validate_custom_claim_name(name: Text) -> None:
+def _validate_custom_claim_name(name: str) -> None:
   if name in _REGISTERED_NAMES:
     raise _jwt_error.JwtInvalidError(
         'registered name %s cannot be custom claim name' % name)
 
 
-class RawJwt(object):
-  """A raw JSON Web Token (JWT).
+class RawJwt:
+  """An unencoded and unsigned JSON Web Token (JWT).
 
-  It can be signed to obtain a compact JWT. It is also used as a parse token
-  that has not yet been verified.
+  It contains all payload claims and a subset of the headers. It does not
+  contain any headers that depend on the key, such as "alg" or "kid", because
+  these headers are chosen when the token is signed and encoded, and should not
+  be chosen by the user. This ensures that the key can be changed without any
+  changes to the user code.
   """
 
   def __new__(cls):
     raise core.TinkError('RawJwt cannot be instantiated directly.')
 
-  def __init__(self, type_header: Optional[Text], payload: Dict[Text,
-                                                                Any]) -> None:
+  def __init__(self, type_header: Optional[str], payload: Dict[str,
+                                                               Any]) -> None:
     # No need to copy payload, because only create and from_json_payload
     # call this method.
     if not isinstance(payload, Dict):
       raise _jwt_error.JwtInvalidError('payload must be a dict')
     self._type_header = type_header
     self._payload = payload
     self._validate_string_claim('iss')
     self._validate_string_claim('sub')
     self._validate_string_claim('jti')
     self._validate_timestamp_claim('exp')
     self._validate_timestamp_claim('nbf')
     self._validate_timestamp_claim('iat')
     self._validate_audience_claim()
 
-  def _validate_string_claim(self, name: Text):
+  def _validate_string_claim(self, name: str):
     if name in self._payload:
-      if not isinstance(self._payload[name], Text):
+      if not isinstance(self._payload[name], str):
         raise _jwt_error.JwtInvalidError('claim %s must be a String' % name)
 
-  def _validate_timestamp_claim(self, name: Text):
+  def _validate_timestamp_claim(self, name: str):
     if name in self._payload:
       timestamp = self._payload[name]
       if not isinstance(timestamp, (int, float)):
         raise _jwt_error.JwtInvalidError('claim %s must be a Number' % name)
       if timestamp > _MAX_TIMESTAMP_VALUE or timestamp < 0:
         raise _jwt_error.JwtInvalidError(
             'timestamp of claim %s is out of range' % name)
 
   def _validate_audience_claim(self):
+    """The 'aud' claim must either be a string or a list of strings."""
     if 'aud' in self._payload:
       audiences = self._payload['aud']
-      if isinstance(audiences, Text):
-        self._payload['aud'] = [audiences]
+      if isinstance(audiences, str):
         return
       if not isinstance(audiences, list) or not audiences:
-        raise _jwt_error.JwtInvalidError('audiences must be a non-empty list')
-      if not all(isinstance(value, Text) for value in audiences):
-        raise _jwt_error.JwtInvalidError('audiences must only contain Text')
+        raise _jwt_error.JwtInvalidError('audiences cannot be an empty list')
+      if not all(isinstance(value, str) for value in audiences):
+        raise _jwt_error.JwtInvalidError('audiences must only contain strings')
 
   # TODO(juerg): Consider adding a raw_ prefix to all access methods
   def has_type_header(self) -> bool:
     return self._type_header is not None
 
-  def type_header(self) -> Text:
+  def type_header(self) -> str:
     if not self.has_type_header():
       raise KeyError('type header is not set')
     return self._type_header
 
   def has_issuer(self) -> bool:
     return 'iss' in self._payload
 
-  def issuer(self) -> Text:
-    return cast(Text, self._payload['iss'])
+  def issuer(self) -> str:
+    return cast(str, self._payload['iss'])
 
   def has_subject(self) -> bool:
     return 'sub' in self._payload
 
-  def subject(self) -> Text:
-    return cast(Text, self._payload['sub'])
+  def subject(self) -> str:
+    return cast(str, self._payload['sub'])
 
   def has_audiences(self) -> bool:
     return 'aud' in self._payload
 
-  def audiences(self) -> List[Text]:
-    return list(self._payload['aud'])
+  def audiences(self) -> List[str]:
+    aud = self._payload['aud']
+    if isinstance(aud, str):
+      return [aud]
+    return list(aud)
 
   def has_jwt_id(self) -> bool:
     return 'jti' in self._payload
 
-  def jwt_id(self) -> Text:
-    return cast(Text, self._payload['jti'])
+  def jwt_id(self) -> str:
+    return cast(str, self._payload['jti'])
 
   def has_expiration(self) -> bool:
     return 'exp' in self._payload
 
   def expiration(self) -> datetime.datetime:
     return _to_datetime(self._payload['exp'])
 
@@ -143,79 +149,117 @@
 
   def has_issued_at(self) -> bool:
     return 'iat' in self._payload
 
   def issued_at(self) -> datetime.datetime:
     return _to_datetime(self._payload['iat'])
 
-  def custom_claim_names(self) -> Set[Text]:
+  def custom_claim_names(self) -> Set[str]:
     return {n for n in self._payload.keys() if n not in _REGISTERED_NAMES}
 
-  def custom_claim(self, name: Text) -> Claim:
+  def custom_claim(self, name: str) -> Claim:
     _validate_custom_claim_name(name)
     value = self._payload[name]
     if isinstance(value, (list, dict)):
       return copy.deepcopy(value)
     else:
       return value
 
-  def json_payload(self) -> Text:
+  def json_payload(self) -> str:
     """Returns the payload encoded as JSON string."""
-    return _jwt_format.json_dumps(self._payload)
+    return _json_util.json_dumps(self._payload)
 
   @classmethod
   def create(cls,
              *,
-             type_header: Optional[Text] = None,
-             issuer: Optional[Text] = None,
-             subject: Optional[Text] = None,
-             audiences: Optional[List[Text]] = None,
-             jwt_id: Optional[Text] = None,
+             type_header: Optional[str] = None,
+             issuer: Optional[str] = None,
+             subject: Optional[str] = None,
+             audience: Optional[str] = None,
+             audiences: Optional[List[str]] = None,
+             jwt_id: Optional[str] = None,
              expiration: Optional[datetime.datetime] = None,
              without_expiration: Optional[bool] = None,
              not_before: Optional[datetime.datetime] = None,
              issued_at: Optional[datetime.datetime] = None,
-             custom_claims: Optional[Mapping[Text, Claim]] = None) -> 'RawJwt':
+             custom_claims: Optional[Mapping[str, Claim]] = None) -> 'RawJwt':
     """Create a new RawJwt instance."""
     if not expiration and not without_expiration:
       raise ValueError('either expiration or without_expiration must be set')
     if expiration and without_expiration:
       raise ValueError(
           'expiration and without_expiration cannot be set at the same time')
+    if audience is not None and audiences is not None:
+      raise _jwt_error.JwtInvalidError(
+          'audience and audiences cannot be set at the same time')
     payload = {}
     if issuer:
       payload['iss'] = issuer
     if subject:
       payload['sub'] = subject
     if jwt_id is not None:
       payload['jti'] = jwt_id
+    if audience is not None:
+      payload['aud'] = audience
     if audiences is not None:
       payload['aud'] = copy.copy(audiences)
     if expiration:
       payload['exp'] = _from_datetime(expiration)
     if not_before:
       payload['nbf'] = _from_datetime(not_before)
     if issued_at:
       payload['iat'] = _from_datetime(issued_at)
     if custom_claims:
       for name, value in custom_claims.items():
         _validate_custom_claim_name(name)
-        if not isinstance(name, Text):
+        if not isinstance(name, str):
           raise _jwt_error.JwtInvalidError('claim name must be Text')
-        if (value is None or isinstance(value, (bool, int, float, Text))):
+        if (value is None or isinstance(value, (bool, int, float, str))):
           payload[name] = value
         elif isinstance(value, list):
           payload[name] = json.loads(json.dumps(value))
         elif isinstance(value, dict):
           payload[name] = json.loads(json.dumps(value))
         else:
           raise _jwt_error.JwtInvalidError('claim %s has unknown type' % name)
     raw_jwt = object.__new__(cls)
     raw_jwt.__init__(type_header, payload)
     return raw_jwt
 
   @classmethod
-  def from_json(cls, type_header: Optional[Text], payload: Text) -> 'RawJwt':
+  def _from_json(cls, type_header: Optional[str], payload: str) -> 'RawJwt':
     """Creates a RawJwt from payload encoded as JSON string."""
     raw_jwt = object.__new__(cls)
-    raw_jwt.__init__(type_header, _jwt_format.json_loads(payload))
+    raw_jwt.__init__(type_header, _json_util.json_loads(payload))
     return raw_jwt
+
+
+def new_raw_jwt(*,
+                type_header: Optional[str] = None,
+                issuer: Optional[str] = None,
+                subject: Optional[str] = None,
+                audience: Optional[str] = None,
+                audiences: Optional[List[str]] = None,
+                jwt_id: Optional[str] = None,
+                expiration: Optional[datetime.datetime] = None,
+                without_expiration: bool = False,
+                not_before: Optional[datetime.datetime] = None,
+                issued_at: Optional[datetime.datetime] = None,
+                custom_claims: Optional[Mapping[str, Claim]] = None) -> RawJwt:
+  """Creates a new RawJwt."""
+  return RawJwt.create(
+      type_header=type_header,
+      issuer=issuer,
+      subject=subject,
+      audience=audience,
+      audiences=audiences,
+      jwt_id=jwt_id,
+      expiration=expiration,
+      without_expiration=without_expiration,
+      not_before=not_before,
+      issued_at=issued_at,
+      custom_claims=custom_claims)
+
+
+def raw_jwt_from_json(type_header: Optional[str], payload: str) -> RawJwt:
+  """Internal function used to verify JWT token."""
+  return RawJwt._from_json(type_header, payload)  # pylint: disable=protected-access
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_mac_wrapper.py` & `tink-1.7.0/tink/jwt/_jwt_mac_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python primitive set wrapper for the JwtMac primitive."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
-from typing import Optional, Text, Type
+from typing import Type
 
 from tink.proto import tink_pb2
 from tink import core
 from tink.jwt import _jwt_error
 from tink.jwt import _jwt_format
 from tink.jwt import _jwt_mac
 from tink.jwt import _jwt_validator
@@ -32,15 +27,15 @@
 
 class _WrappedJwtMac(_jwt_mac.JwtMac):
   """A wrapped JwtMac."""
 
   def __init__(self, pset: core.PrimitiveSet):
     self._primitive_set = pset
 
-  def compute_mac_and_encode(self, raw_jwt: _raw_jwt.RawJwt) -> Text:
+  def compute_mac_and_encode(self, raw_jwt: _raw_jwt.RawJwt) -> str:
     """Computes a MAC and encodes the token.
 
     Args:
       raw_jwt: The RawJwt token to be MACed and encoded.
 
     Returns:
       The MACed token encoded in the JWS compact serialization format.
@@ -48,15 +43,15 @@
       tink.TinkError if the operation fails.
     """
     primary = self._primitive_set.primary()
     kid = _jwt_format.get_kid(primary.key_id, primary.output_prefix_type)
     return primary.primitive.compute_mac_and_encode_with_kid(raw_jwt, kid)
 
   def verify_mac_and_decode(
-      self, compact: Text,
+      self, compact: str,
       validator: _jwt_validator.JwtValidator) -> _verified_jwt.VerifiedJwt:
     """Verifies, validates and decodes a MACed compact JWT token.
 
     Args:
       compact: A MACed token encoded in the JWS compact serialization format.
       validator: A JwtValidator that validates the token.
 
@@ -65,37 +60,38 @@
     Raises:
       tink.TinkError if the operation fails.
     """
     interesting_error = None
     for entries in self._primitive_set.all():
       for entry in entries:
         try:
-          return entry.primitive.verify_mac_and_decode(compact, validator)
+          kid = _jwt_format.get_kid(entry.key_id, entry.output_prefix_type)
+          return entry.primitive.verify_mac_and_decode_with_kid(
+              compact, validator, kid)
         except core.TinkError as e:
           if isinstance(e, _jwt_error.JwtInvalidError):
             interesting_error = e
           pass
     if interesting_error:
       raise interesting_error
     raise core.TinkError('invalid MAC')
 
 
 def _validate_primitive_set(pset: core.PrimitiveSet):
-  # TODO(juerg): also validate that there is a primary
   for entries in pset.all():
     for entry in entries:
       if (entry.output_prefix_type != tink_pb2.RAW and
           entry.output_prefix_type != tink_pb2.TINK):
         raise core.TinkError('unsupported OutputPrefixType')
 
 
 class _Wrapper(core.PrimitiveWrapper[_jwt_mac.JwtMacInternal, _jwt_mac.JwtMac]):
   """A wrapper for JwtMac."""
 
-  def wrap(self, pset: core.PrimitiveSet) -> Optional[_jwt_mac.JwtMac]:
+  def wrap(self, pset: core.PrimitiveSet) -> _jwt_mac.JwtMac:
     _validate_primitive_set(pset)
     return _WrappedJwtMac(pset)
 
   def primitive_class(self) -> Type[_jwt_mac.JwtMac]:
     return _jwt_mac.JwtMac
 
   def input_primitive_class(self) -> Type[_jwt_mac.JwtMacInternal]:
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_public_key_sign.py` & `tink-1.7.0/tink/jwt/_jwt_public_key_sign.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,54 +9,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Interface for JwtPublicKeySign."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
-from typing import Optional, Text
-
-import six
+from typing import Optional
 
 from tink.jwt import _raw_jwt
 
 
-@six.add_metaclass(abc.ABCMeta)
-class JwtPublicKeySign(object):
+class JwtPublicKeySign(metaclass=abc.ABCMeta):
   """Interface for creating a signed JWT.
 
   Sees RFC 7519 and RFC 7515. Security guarantees: similar to PublicKeySign.
   """
 
   @abc.abstractmethod
-  def sign_and_encode(self, raw_jwt: _raw_jwt.RawJwt) -> Text:
+  def sign_and_encode(self, raw_jwt: _raw_jwt.RawJwt) -> str:
     """Computes a signature and encodes the token.
 
     Args:
       raw_jwt: The RawJwt token to be signed and encoded.
 
     Returns:
       The signed token encoded in the JWS compact serialization format.
     Raises:
       tink.TinkError if the operation fails.
     """
     raise NotImplementedError()
 
 
-@six.add_metaclass(abc.ABCMeta)
-class JwtPublicKeySignInternal(object):
+class JwtPublicKeySignInternal(metaclass=abc.ABCMeta):
   """Internal interface for creating a signed JWT.
 
   "kid" is an optional value that is set by the wrapper for keys with output
   prefix TINK, and it is set to None for output prefix RAW.
   """
 
   @abc.abstractmethod
   def sign_and_encode_with_kid(self, token: _raw_jwt.RawJwt,
-                               kid: Optional[Text]) -> Text:
+                               kid: Optional[str]) -> str:
     raise NotImplementedError()
```

### Comparing `tink-1.6.1/tink/jwt/_verified_jwt_test.py` & `tink-1.7.0/tink/jwt/_verified_jwt_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 """Tests for tink.python.tink.jwt._verified_jwt."""
 
-
 import datetime
 
 from absl.testing import absltest
 from tink import jwt
 
 ISSUED_AT = datetime.datetime.fromtimestamp(1582230020, datetime.timezone.utc)
 NOT_BEFORE = datetime.datetime.fromtimestamp(1893553445, datetime.timezone.utc)
```

### Comparing `tink-1.6.1/tink/jwt/_jwt_signature_wrappers.py` & `tink-1.7.0/tink/jwt/_jwt_signature_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python primitive set wrapper for the JwtMac primitive."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
-from typing import Optional, Text, Type
+from typing import Type
 
 from tink.proto import tink_pb2
 from tink import core
 from tink.jwt import _jwt_error
 from tink.jwt import _jwt_format
 from tink.jwt import _jwt_public_key_sign
 from tink.jwt import _jwt_public_key_verify
@@ -33,86 +28,86 @@
 
 class _WrappedJwtPublicKeySign(_jwt_public_key_sign.JwtPublicKeySign):
   """A wrapped JwtPublicKeySign."""
 
   def __init__(self, pset: core.PrimitiveSet):
     self._primitive_set = pset
 
-  def sign_and_encode(self, raw_jwt: _raw_jwt.RawJwt) -> Text:
+  def sign_and_encode(self, raw_jwt: _raw_jwt.RawJwt) -> str:
     primary = self._primitive_set.primary()
     kid = _jwt_format.get_kid(primary.key_id, primary.output_prefix_type)
     return primary.primitive.sign_and_encode_with_kid(raw_jwt, kid)
 
 
 class _WrappedJwtPublicKeyVerify(_jwt_public_key_verify.JwtPublicKeyVerify):
   """A wrapped JwtPublicKeyVerify."""
 
   def __init__(self, pset: core.PrimitiveSet):
     self._primitive_set = pset
 
   def verify_and_decode(
-      self, compact: Text,
+      self, compact: str,
       validator: _jwt_validator.JwtValidator) -> _verified_jwt.VerifiedJwt:
     interesting_error = None
     for entries in self._primitive_set.all():
       for entry in entries:
         try:
-          return entry.primitive.verify_and_decode(compact, validator)
+          kid = _jwt_format.get_kid(entry.key_id, entry.output_prefix_type)
+          return entry.primitive.verify_and_decode_with_kid(
+              compact, validator, kid)
         except core.TinkError as e:
           if isinstance(e, _jwt_error.JwtInvalidError):
             interesting_error = e
           pass
     if interesting_error:
       raise interesting_error
     raise core.TinkError('invalid signature')
 
 
 def _validate_primitive_set(pset: core.PrimitiveSet):
-  # TODO(juerg): also validate that there is a primary
   for entries in pset.all():
     for entry in entries:
       if (entry.output_prefix_type != tink_pb2.RAW and
           entry.output_prefix_type != tink_pb2.TINK):
         raise core.TinkError('unsupported OutputPrefixType')
 
 
 class _JwtPublicKeySignWrapper(
     core.PrimitiveWrapper[_jwt_public_key_sign.JwtPublicKeySignInternal,
                           _jwt_public_key_sign.JwtPublicKeySign]):
   """A wrapper for JwtPublicKeySign."""
 
-  def wrap(
-      self, pset: core.PrimitiveSet
-  ) -> Optional[_jwt_public_key_sign.JwtPublicKeySign]:
+  def wrap(self,
+           pset: core.PrimitiveSet) -> _jwt_public_key_sign.JwtPublicKeySign:
     _validate_primitive_set(pset)
     return _WrappedJwtPublicKeySign(pset)
 
   def primitive_class(self) -> Type[_jwt_public_key_sign.JwtPublicKeySign]:
     return _jwt_public_key_sign.JwtPublicKeySign
 
   def input_primitive_class(
       self) -> Type[_jwt_public_key_sign.JwtPublicKeySignInternal]:
     return _jwt_public_key_sign.JwtPublicKeySignInternal
 
 
 class _JwtPublicKeyVerifyWrapper(
-    core.PrimitiveWrapper[_jwt_public_key_verify.JwtPublicKeyVerify,
+    core.PrimitiveWrapper[_jwt_public_key_verify.JwtPublicKeyVerifyInternal,
                           _jwt_public_key_verify.JwtPublicKeyVerify]):
   """A wrapper for JwtPublicKeyVerify."""
 
   def wrap(
-      self, pset: core.PrimitiveSet
-  ) -> Optional[_jwt_public_key_verify.JwtPublicKeyVerify]:
+      self,
+      pset: core.PrimitiveSet) -> _jwt_public_key_verify.JwtPublicKeyVerify:
     _validate_primitive_set(pset)
     return _WrappedJwtPublicKeyVerify(pset)
 
   def primitive_class(self) -> Type[_jwt_public_key_verify.JwtPublicKeyVerify]:
     return _jwt_public_key_verify.JwtPublicKeyVerify
 
   def input_primitive_class(
-      self) -> Type[_jwt_public_key_verify.JwtPublicKeyVerify]:
-    return _jwt_public_key_verify.JwtPublicKeyVerify
+      self) -> Type[_jwt_public_key_verify.JwtPublicKeyVerifyInternal]:
+    return _jwt_public_key_verify.JwtPublicKeyVerifyInternal
 
 
 def register():
   core.Registry.register_primitive_wrapper(_JwtPublicKeySignWrapper())
   core.Registry.register_primitive_wrapper(_JwtPublicKeyVerifyWrapper())
```

### Comparing `tink-1.6.1/tink/tink_config_test.py` & `tink-1.7.0/tink/tink_config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.tink_config."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 import os
 import tempfile
 
 from absl.testing import absltest
 
 import tink
 from tink import aead
```

### Comparing `tink-1.6.1/tink/_keyset_reader.py` & `tink-1.7.0/tink/_keyset_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,34 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Reads Keysets from file."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 
-from typing import Text
-# Special imports
-import six
-
-
-from tink.proto import tink_pb2
-from tink import core
 from google.protobuf import json_format
 from google.protobuf import message
+from tink.proto import tink_pb2
+from tink import core
 
 
-@six.add_metaclass(abc.ABCMeta)
-class KeysetReader(object):
+class KeysetReader(metaclass=abc.ABCMeta):
   """Reads a Keyset."""
 
   @abc.abstractmethod
   def read(self) -> tink_pb2.Keyset:
     """Reads and returns a (cleartext) tink_pb2.Keyset from its source."""
     raise NotImplementedError()
 
@@ -46,15 +35,15 @@
     """Reads and returns an tink_pb2.EncryptedKeyset from its source."""
     raise NotImplementedError()
 
 
 class JsonKeysetReader(KeysetReader):
   """Reads a JSON Keyset."""
 
-  def __init__(self, serialized_keyset: Text):
+  def __init__(self, serialized_keyset: str):
     self._serialized_keyset = serialized_keyset
 
   def read(self) -> tink_pb2.Keyset:
     try:
       return json_format.Parse(self._serialized_keyset, tink_pb2.Keyset())
     except json_format.ParseError as e:
       raise core.TinkError(e)
```

### Comparing `tink-1.6.1/tink/hybrid/_hybrid_key_templates.py` & `tink-1.7.0/tink/mac/_mac_key_templates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,83 @@
-# Copyright 2019 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-"""Pre-generated KeyTemplate for HybridEncryption.
+"""Pre-generated KeyTemplate for Mac.
 
 One can use these templates to generate a new tink_pb2.Keyset with
 tink_pb2.KeysetHandle. To generate a new keyset that contains a single
-tink_pb2.HmacKey, one can do:
+hmac_pb2.HmacKey, one can do:
 handle = keyset_handle.KeysetHandle(mac_key_templates.HMAC_SHA256_128BITTAG).
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
+import warnings
 
+from tink.proto import aes_cmac_pb2
 from tink.proto import common_pb2
-from tink.proto import ecies_aead_hkdf_pb2
+from tink.proto import hmac_pb2
 from tink.proto import tink_pb2
-from tink import aead
 
 
-def create_ecies_aead_hkdf_key_template(
-    curve_type: common_pb2.EllipticCurveType,
-    ec_point_format: common_pb2.EcPointFormat,
-    hash_type: common_pb2.HashType,
-    dem_key_template: tink_pb2.KeyTemplate) -> tink_pb2.KeyTemplate:
+def _create_hmac_key_template(
+    key_size: int, tag_size: int,
+    hash_type: common_pb2.HashType) -> tink_pb2.KeyTemplate:
   """Creates a HMAC KeyTemplate, and fills in its values."""
-  key_format = ecies_aead_hkdf_pb2.EciesAeadHkdfKeyFormat()
-  key_format.params.kem_params.curve_type = curve_type
-  key_format.params.kem_params.hkdf_hash_type = hash_type
-  key_format.params.dem_params.aead_dem.CopyFrom(dem_key_template)
-  key_format.params.ec_point_format = ec_point_format
+  key_format = hmac_pb2.HmacKeyFormat()
+  key_format.params.hash = hash_type
+  key_format.params.tag_size = tag_size
+  key_format.key_size = key_size
+  key_template = tink_pb2.KeyTemplate()
+  key_template.value = key_format.SerializeToString()
+  key_template.type_url = 'type.googleapis.com/google.crypto.tink.HmacKey'
+  key_template.output_prefix_type = tink_pb2.TINK
+  return key_template
+
 
+def _create_aes_cmac_key_template(key_size: int,
+                                  tag_size: int) -> tink_pb2.KeyTemplate:
+  """"Creates an AES-CMAC KeyTemplate, and fills in its values."""
+  key_format = aes_cmac_pb2.AesCmacKeyFormat()
+  key_format.key_size = key_size
+  key_format.params.tag_size = tag_size
   key_template = tink_pb2.KeyTemplate()
-  key_template.type_url = (
-      'type.googleapis.com/google.crypto.tink.EciesAeadHkdfPrivateKey')
   key_template.value = key_format.SerializeToString()
+  key_template.type_url = 'type.googleapis.com/google.crypto.tink.AesCmacKey'
   key_template.output_prefix_type = tink_pb2.TINK
   return key_template
 
 
-ECIES_P256_HKDF_HMAC_SHA256_AES128_GCM = create_ecies_aead_hkdf_key_template(
-    curve_type=common_pb2.NIST_P256,
-    ec_point_format=common_pb2.UNCOMPRESSED,
-    hash_type=common_pb2.SHA256,
-    dem_key_template=aead.aead_key_templates.AES128_GCM)
-
-ECIES_P256_COMPRESSED_HKDF_HMAC_SHA256_AES128_GCM = create_ecies_aead_hkdf_key_template(
-    curve_type=common_pb2.NIST_P256,
-    ec_point_format=common_pb2.COMPRESSED,
-    hash_type=common_pb2.SHA256,
-    dem_key_template=aead.aead_key_templates.AES128_GCM)
-
-ECIES_P256_HKDF_HMAC_SHA256_AES128_CTR_HMAC_SHA256 = (
-    create_ecies_aead_hkdf_key_template(
-        curve_type=common_pb2.NIST_P256,
-        ec_point_format=common_pb2.UNCOMPRESSED,
-        hash_type=common_pb2.SHA256,
-        dem_key_template=aead.aead_key_templates.AES128_CTR_HMAC_SHA256))
-
-ECIES_P256_COMPRESSED_HKDF_HMAC_SHA256_AES128_CTR_HMAC_SHA256 = (
-    create_ecies_aead_hkdf_key_template(
-        curve_type=common_pb2.NIST_P256,
-        ec_point_format=common_pb2.COMPRESSED,
-        hash_type=common_pb2.SHA256,
-        dem_key_template=aead.aead_key_templates.AES128_CTR_HMAC_SHA256))
+AES_CMAC = _create_aes_cmac_key_template(key_size=32, tag_size=16)
+HMAC_SHA256_128BITTAG = _create_hmac_key_template(
+    key_size=32, tag_size=16, hash_type=common_pb2.SHA256)
+HMAC_SHA256_256BITTAG = _create_hmac_key_template(
+    key_size=32, tag_size=32, hash_type=common_pb2.SHA256)
+HMAC_SHA512_256BITTAG = _create_hmac_key_template(
+    key_size=64, tag_size=32, hash_type=common_pb2.SHA512)
+HMAC_SHA512_512BITTAG = _create_hmac_key_template(
+    key_size=64, tag_size=64, hash_type=common_pb2.SHA512)
+
+
+# Deprecated. Use the predefined constant templates above instead.
+def create_hmac_key_template(
+    key_size: int, tag_size: int,
+    hash_type: common_pb2.HashType) -> tink_pb2.KeyTemplate:
+  warnings.warn('The "create_hmac_key_template" function is deprecated.',
+                DeprecationWarning, 2)
+  return _create_hmac_key_template(key_size, tag_size, hash_type)
+
+
+# Deprecated. Use the predefined constant templates above instead.
+def create_aes_cmac_key_template(key_size: int,
+                                 tag_size: int) -> tink_pb2.KeyTemplate:
+  warnings.warn('The "create_hmac_key_template" function is deprecated.',
+                DeprecationWarning, 2)
+  return _create_aes_cmac_key_template(key_size, tag_size)
```

### Comparing `tink-1.6.1/tink/hybrid/_hybrid_encrypt.py` & `tink-1.7.0/tink/hybrid/_hybrid_decrypt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,28 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""This module defines the interface for HybridEncrypt."""
-
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
+"""This module defines the interface for HybridDecrypt."""
 
 import abc
 
-# Special imports
-import six
-
 
-@six.add_metaclass(abc.ABCMeta)
-class HybridEncrypt(object):
-  """The interface for hybrid encryption.
+class HybridDecrypt(metaclass=abc.ABCMeta):
+  """The interface for hybrid decryption.
 
   Implementations of this interface are secure against adaptive
   chosen ciphertext attacks.  In addition to 'plaintext' the
   encryption takes an extra parameter 'context_info', which usually
   is public data implicit from the context, but should be bound to
   the resulting ciphertext: upon decryption the ciphertext allows for
   checking the integrity of 'context_info' (but there are no
@@ -55,10 +46,10 @@
   - use 'context_info' as "associated data"-input for the employed
     AEAD symmetric encryption (cf. https://tools.ietf.org/html/rfc5116).
   - use 'context_info' as "CtxInfo"-input for HKDF (if the implementation uses
     HKDF as key derivation function, cf. https://tools.ietf.org/html/rfc5869).
   """
 
   @abc.abstractmethod
-  def encrypt(self, plaintext: bytes, context_info: bytes) -> bytes:
-    """Encrypts plaintext binding context_info to the resulting ciphertext."""
+  def decrypt(self, ciphertext: bytes, context_info: bytes) -> bytes:
+    """Decrypts ciphertext verifying the integrity of context_info."""
     raise NotImplementedError()
```

### Comparing `tink-1.6.1/tink/hybrid/BUILD.bazel` & `tink-1.7.0/tink/hybrid/BUILD.bazel`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,20 @@
     ],
 )
 
 py_library(
     name = "_hybrid_decrypt",
     srcs = ["_hybrid_decrypt.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_hybrid_encrypt",
     srcs = ["_hybrid_encrypt.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_hybrid_key_manager",
     srcs = ["_hybrid_key_manager.py"],
     srcs_version = "PY3",
     deps = [
@@ -54,14 +52,15 @@
         ":hybrid",
         requirement("absl-py"),
         "//tink:tink_python",
         "//tink/aead",
         "//tink/core",
         "//tink/proto:common_py_pb2",
         "//tink/proto:ecies_aead_hkdf_py_pb2",
+        "//tink/proto:hpke_py_pb2",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_library(
     name = "_hybrid_wrapper",
     srcs = ["_hybrid_wrapper.py"],
@@ -77,42 +76,42 @@
 py_test(
     name = "_hybrid_wrapper_test",
     srcs = ["_hybrid_wrapper_test.py"],
     srcs_version = "PY3",
     deps = [
         ":hybrid",
         requirement("absl-py"),
+        "//tink:cleartext_keyset_handle",
         "//tink:tink_python",
         "//tink/proto:tink_py_pb2",
         "//tink/testing:keyset_builder",
     ],
 )
 
 py_library(
     name = "_hybrid_key_templates",
     srcs = ["_hybrid_key_templates.py"],
     srcs_version = "PY3",
     deps = [
         "//tink/aead",
+        "//tink/daead",
         "//tink/proto:common_py_pb2",
         "//tink/proto:ecies_aead_hkdf_py_pb2",
+        "//tink/proto:hpke_py_pb2",
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_hybrid_key_templates_test",
     srcs = ["_hybrid_key_templates_test.py"],
-    data = [
-        "@tink_base//testdata/templates",
-    ],
     srcs_version = "PY3",
     deps = [
         ":hybrid",
         requirement("absl-py"),
         "//tink/aead",
         "//tink/proto:common_py_pb2",
         "//tink/proto:ecies_aead_hkdf_py_pb2",
+        "//tink/proto:hpke_py_pb2",
         "//tink/proto:tink_py_pb2",
-        "//tink/testing:helper",
     ],
 )
```

### Comparing `tink-1.6.1/tink/hybrid/__init__.py` & `tink-1.7.0/tink/hybrid/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Hybrid package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
 from tink.hybrid import _hybrid_decrypt
 from tink.hybrid import _hybrid_encrypt
 from tink.hybrid import _hybrid_key_manager
 from tink.hybrid import _hybrid_key_templates as hybrid_key_templates
```

### Comparing `tink-1.6.1/tink/hybrid/_hybrid_wrapper.py` & `tink-1.7.0/tink/hybrid/_hybrid_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """HybridDecrypt wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from typing import Type
 from absl import logging
 
 from tink import core
 from tink.hybrid import _hybrid_decrypt
 from tink.hybrid import _hybrid_encrypt
 
@@ -79,14 +74,16 @@
 class _WrappedHybridEncrypt(_hybrid_encrypt.HybridEncrypt):
   """Implements HybridEncrypt for a set of HybridEncrypt primitives."""
 
   def __init__(self, pset: core.PrimitiveSet):
     self._primitive_set = pset
 
   def encrypt(self, plaintext: bytes, context_info: bytes) -> bytes:
+    if not self._primitive_set.primary():
+      raise core.TinkError('keyset without primary key')
     primary = self._primitive_set.primary()
     return primary.identifier + primary.primitive.encrypt(
         plaintext, context_info)
 
 
 class HybridEncryptWrapper(core.PrimitiveWrapper[_hybrid_encrypt.HybridEncrypt,
                                                  _hybrid_encrypt.HybridEncrypt]
```

### Comparing `tink-1.6.1/tink/hybrid/_hybrid_key_templates_test.py` & `tink-1.7.0/tink/hybrid/_hybrid_key_templates_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,56 +10,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.hybrid_key_templates."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 from tink.proto import common_pb2
 from tink.proto import ecies_aead_hkdf_pb2
+from tink.proto import hpke_pb2
 from tink.proto import tink_pb2
 from tink import aead
 from tink import hybrid
-from tink.testing import helper
 
 
 class HybridKeyTemplatesTest(parameterized.TestCase):
 
-  @parameterized.parameters([
-      ('ECIES_P256_HKDF_HMAC_SHA256_AES128_GCM',
-       hybrid.hybrid_key_templates.ECIES_P256_HKDF_HMAC_SHA256_AES128_GCM),
-      ('ECIES_P256_COMPRESSED_HKDF_HMAC_SHA256_AES128_GCM',
-       hybrid.hybrid_key_templates
-       .ECIES_P256_COMPRESSED_HKDF_HMAC_SHA256_AES128_GCM),
-      ('ECIES_P256_HKDF_HMAC_SHA256_AES128_CTR_HMAC_SHA256',
-       hybrid.hybrid_key_templates
-       .ECIES_P256_HKDF_HMAC_SHA256_AES128_CTR_HMAC_SHA256),
-      ('ECIES_P256_COMPRESSED_HKDF_HMAC_SHA256_AES128_CTR_HMAC_SHA256',
-       hybrid.hybrid_key_templates
-       .ECIES_P256_COMPRESSED_HKDF_HMAC_SHA256_AES128_CTR_HMAC_SHA256)
-
-  ])
-  def test_template(self, template_name, template):
-    self.assertEqual(template,
-                     helper.template_from_testdata(template_name, 'hybrid'))
-
   def test_create_aes_eax_key_template(self):
     # Intentionally using 'weird' or invalid values for parameters,
     # to test that the function correctly puts them in the resulting template.
-    template = hybrid.hybrid_key_templates.create_ecies_aead_hkdf_key_template(
-        curve_type=common_pb2.NIST_P521,
-        ec_point_format=common_pb2.DO_NOT_USE_CRUNCHY_UNCOMPRESSED,
-        hash_type=common_pb2.SHA1,
-        dem_key_template=aead.aead_key_templates.AES256_EAX)
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = (
+          hybrid.hybrid_key_templates.create_ecies_aead_hkdf_key_template(
+              curve_type=common_pb2.NIST_P521,
+              ec_point_format=common_pb2.DO_NOT_USE_CRUNCHY_UNCOMPRESSED,
+              hash_type=common_pb2.SHA1,
+              dem_key_template=aead.aead_key_templates.AES256_EAX))
     self.assertEqual(
         'type.googleapis.com/google.crypto.tink.EciesAeadHkdfPrivateKey',
         template.type_url)
     self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
     key_format = ecies_aead_hkdf_pb2.EciesAeadHkdfKeyFormat.FromString(
         template.value)
     self.assertEqual(key_format.params.kem_params.curve_type,
@@ -67,10 +48,24 @@
     self.assertEqual(key_format.params.kem_params.hkdf_hash_type,
                      common_pb2.SHA1)
     self.assertEqual(key_format.params.ec_point_format,
                      common_pb2.DO_NOT_USE_CRUNCHY_UNCOMPRESSED)
     self.assertEqual(key_format.params.dem_params.aead_dem,
                      aead.aead_key_templates.AES256_EAX)
 
+  def test_create_hpke_key_template(self):
+    template = hybrid.hybrid_key_templates._create_hpke_key_template(
+        hpke_kem=hpke_pb2.DHKEM_X25519_HKDF_SHA256,
+        hpke_kdf=hpke_pb2.HKDF_SHA256,
+        hpke_aead=hpke_pb2.AES_128_GCM,
+        output_prefix_type=tink_pb2.TINK)
+    self.assertEqual('type.googleapis.com/google.crypto.tink.HpkePrivateKey',
+                     template.type_url)
+    self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
+    key_format = hpke_pb2.HpkeKeyFormat.FromString(template.value)
+    self.assertEqual(key_format.params.kem, hpke_pb2.DHKEM_X25519_HKDF_SHA256)
+    self.assertEqual(key_format.params.kdf, hpke_pb2.HKDF_SHA256)
+    self.assertEqual(key_format.params.aead, hpke_pb2.AES_128_GCM)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/hybrid/_hybrid_key_manager.py` & `tink-1.7.0/tink/hybrid/_hybrid_key_manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python wrapper of the wrapped C++ Hybrid En- and Decryption key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.hybrid import _hybrid_decrypt
 from tink.hybrid import _hybrid_encrypt
 from tink.hybrid import _hybrid_wrapper
 
 
@@ -47,25 +42,48 @@
   def encrypt(self, plaintext: bytes, context_info: bytes) -> bytes:
     return self._hybrid_encrypt.encrypt(plaintext, context_info)
 
 
 def register():
   """Registers all Hybrid key managers and wrapper in the Python Registry."""
   tink_bindings.register()
+  tink_bindings.register_hpke()
+
+  # Register primitive wrappers.
+  core.Registry.register_primitive_wrapper(
+      _hybrid_wrapper.HybridDecryptWrapper())
+  core.Registry.register_primitive_wrapper(
+      _hybrid_wrapper.HybridEncryptWrapper())
 
+  # Register ECIES-AEAD-HKDF key managers.
   decrypt_type_url = (
       'type.googleapis.com/google.crypto.tink.EciesAeadHkdfPrivateKey')
   decrypt_key_manager = core.PrivateKeyManagerCcToPyWrapper(
       tink_bindings.HybridDecryptKeyManager.from_cc_registry(decrypt_type_url),
       _hybrid_decrypt.HybridDecrypt, _HybridDecryptCcToPyWrapper)
   core.Registry.register_key_manager(decrypt_key_manager, new_key_allowed=True)
-  core.Registry.register_primitive_wrapper(
-      _hybrid_wrapper.HybridDecryptWrapper())
 
   encrypt_type_url = (
       'type.googleapis.com/google.crypto.tink.EciesAeadHkdfPublicKey')
   encrypt_key_manager = core.KeyManagerCcToPyWrapper(
       tink_bindings.HybridEncryptKeyManager.from_cc_registry(encrypt_type_url),
       _hybrid_encrypt.HybridEncrypt, _HybridEncryptCcToPyWrapper)
   core.Registry.register_key_manager(encrypt_key_manager, new_key_allowed=True)
-  core.Registry.register_primitive_wrapper(
-      _hybrid_wrapper.HybridEncryptWrapper())
+
+  # Register HPKE key managers.
+  hpke_decrypt_type_url = (
+      'type.googleapis.com/google.crypto.tink.HpkePrivateKey')
+  hpke_decrypt_key_manager = core.PrivateKeyManagerCcToPyWrapper(
+      tink_bindings.HybridDecryptKeyManager.from_cc_registry(
+          hpke_decrypt_type_url), _hybrid_decrypt.HybridDecrypt,
+      _HybridDecryptCcToPyWrapper)
+  core.Registry.register_key_manager(
+      hpke_decrypt_key_manager, new_key_allowed=True)
+
+  hpke_encrypt_type_url = (
+      'type.googleapis.com/google.crypto.tink.HpkePublicKey')
+  hpke_encrypt_key_manager = core.KeyManagerCcToPyWrapper(
+      tink_bindings.HybridEncryptKeyManager.from_cc_registry(
+          hpke_encrypt_type_url), _hybrid_encrypt.HybridEncrypt,
+      _HybridEncryptCcToPyWrapper)
+  core.Registry.register_key_manager(
+      hpke_encrypt_key_manager, new_key_allowed=True)
```

### Comparing `tink-1.6.1/tink/hybrid/_hybrid_decrypt.py` & `tink-1.7.0/tink/hybrid/_hybrid_encrypt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,28 @@
-# Copyright 2019 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""This module defines the interface for HybridDecrypt."""
-
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
+"""This module defines the interface for HybridEncrypt."""
 
 import abc
 
-# Special imports
-import six
-
 
-@six.add_metaclass(abc.ABCMeta)
-class HybridDecrypt(object):
-  """The interface for hybrid decryption.
+class HybridEncrypt(metaclass=abc.ABCMeta):
+  """The interface for hybrid encryption.
 
   Implementations of this interface are secure against adaptive
   chosen ciphertext attacks.  In addition to 'plaintext' the
   encryption takes an extra parameter 'context_info', which usually
   is public data implicit from the context, but should be bound to
   the resulting ciphertext: upon decryption the ciphertext allows for
   checking the integrity of 'context_info' (but there are no
@@ -55,10 +46,10 @@
   - use 'context_info' as "associated data"-input for the employed
     AEAD symmetric encryption (cf. https://tools.ietf.org/html/rfc5116).
   - use 'context_info' as "CtxInfo"-input for HKDF (if the implementation uses
     HKDF as key derivation function, cf. https://tools.ietf.org/html/rfc5869).
   """
 
   @abc.abstractmethod
-  def decrypt(self, ciphertext: bytes, context_info: bytes) -> bytes:
-    """Decrypts ciphertext verifying the integrity of context_info."""
+  def encrypt(self, plaintext: bytes, context_info: bytes) -> bytes:
+    """Encrypts plaintext binding context_info to the resulting ciphertext."""
     raise NotImplementedError()
```

### Comparing `tink-1.6.1/tink/mac/_mac_wrapper_test.py` & `tink-1.7.0/tink/mac/_mac_wrapper_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink._mac_wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 import tink
 from tink import mac
 from tink.testing import keyset_builder
```

### Comparing `tink-1.6.1/tink/mac/_mac_key_manager_test.py` & `tink-1.7.0/tink/mac/_mac_key_manager_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for tink.python.tink._mac_key_manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 
 from tink.proto import common_pb2
 from tink.proto import hmac_pb2
 
 import tink
```

### Comparing `tink-1.6.1/tink/mac/_mac_key_manager.py` & `tink-1.7.0/tink/mac/_mac_key_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Python wrapper of the wrapped C++ MAC key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.mac import _mac
 from tink.mac import _mac_wrapper
 
 
 class _MacCcToPyWrapper(_mac.Mac):
```

### Comparing `tink-1.6.1/tink/mac/BUILD.bazel` & `tink-1.7.0/tink/mac/BUILD.bazel`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     ],
 )
 
 py_library(
     name = "_mac",
     srcs = ["_mac.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_mac_key_manager",
     srcs = ["_mac_key_manager.py"],
     srcs_version = "PY3",
     deps = [
@@ -88,20 +87,16 @@
         "//tink/proto:tink_py_pb2",
     ],
 )
 
 py_test(
     name = "_mac_key_templates_test",
     srcs = ["_mac_key_templates_test.py"],
-    data = [
-        "@tink_base//testdata/templates",
-    ],
     srcs_version = "PY3",
     deps = [
         ":mac",
         requirement("absl-py"),
         "//tink/proto:common_py_pb2",
         "//tink/proto:hmac_py_pb2",
         "//tink/proto:tink_py_pb2",
-        "//tink/testing:helper",
     ],
 )
```

### Comparing `tink-1.6.1/tink/mac/__init__.py` & `tink-1.7.0/tink/integration/awskms/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Mac package."""
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
 
-from tink.mac import _mac
-from tink.mac import _mac_key_manager
-from tink.mac import _mac_key_templates as mac_key_templates
+"""StreamingAead package."""
 
+from tink.integration.awskms import _aws_kms_client
 
-Mac = _mac.Mac
-register = _mac_key_manager.register
+AwsKmsClient = _aws_kms_client.AwsKmsClient
```

### Comparing `tink-1.6.1/tink/mac/_mac_key_templates_test.py` & `tink-1.7.0/tink/daead/_deterministic_aead_key_templates_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,42 @@
-# Copyright 2020 Google LLC.
+# Copyright 2019 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for tink.python.tink._mac_key_templates."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
+"""Tests for tink.python.tink.deterministic_aead_key_templates."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
-from tink.proto import common_pb2
-from tink.proto import hmac_pb2
+from tink.proto import aes_siv_pb2
 from tink.proto import tink_pb2
-from tink import mac
-from tink.testing import helper
+from tink import daead
 
 
-class MacKeyTemplatesTest(parameterized.TestCase):
+class DeterministicAeadKeyTemplatesTest(parameterized.TestCase):
 
-  @parameterized.parameters([
-      ('AES_CMAC', mac.mac_key_templates.AES_CMAC),
-      ('HMAC_SHA256_128BITTAG', mac.mac_key_templates.HMAC_SHA256_128BITTAG),
-      ('HMAC_SHA256_256BITTAG', mac.mac_key_templates.HMAC_SHA256_256BITTAG),
-      ('HMAC_SHA512_256BITTAG', mac.mac_key_templates.HMAC_SHA512_256BITTAG),
-      ('HMAC_SHA512_512BITTAG', mac.mac_key_templates.HMAC_SHA512_512BITTAG)
-  ])
-  def test_template(self, template_name, template):
-    self.assertEqual(template,
-                     helper.template_from_testdata(template_name, 'mac'))
-
-  def test_create_hmac_key_template(self):
-    # Intentionally using "weird" or invalid values for parameters,
+  def test_create_aes_siv_key_template(self):
+    # Intentionally using 'weird' or invalid values for parameters,
     # to test that the function correctly puts them in the resulting template.
-    template = mac.mac_key_templates.create_hmac_key_template(
-        key_size=42, tag_size=24, hash_type=common_pb2.SHA512)
-    self.assertEqual('type.googleapis.com/google.crypto.tink.HmacKey',
+    template = None
+    with self.assertWarns(DeprecationWarning):
+      template = (
+          daead.deterministic_aead_key_templates.create_aes_siv_key_template(
+              key_size=42))
+    self.assertEqual('type.googleapis.com/google.crypto.tink.AesSivKey',
                      template.type_url)
     self.assertEqual(tink_pb2.TINK, template.output_prefix_type)
-    key_format = hmac_pb2.HmacKeyFormat.FromString(template.value)
+    key_format = aes_siv_pb2.AesSivKeyFormat()
+    key_format.ParseFromString(template.value)
     self.assertEqual(42, key_format.key_size)
-    self.assertEqual(24, key_format.params.tag_size)
-    self.assertEqual(common_pb2.SHA512, key_format.params.hash)
-
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tink-1.6.1/tink/mac/_mac_wrapper.py` & `tink-1.7.0/tink/mac/_mac_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """MAC wrapper.
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from typing import Type
 from absl import logging
 
 
 from tink.proto import tink_pb2
 from tink import core
 from tink.mac import _mac
```

### Comparing `tink-1.6.1/tink/mac/_mac_key_templates.py` & `tink-1.7.0/tink/prf/_prf_key_templates.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,81 @@
-# Copyright 2020 Google LLC.
+# Copyright 2020 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Pre-generated KeyTemplate for Mac.
+
+"""Pre-generated KeyTemplate for Aead.
 
 One can use these templates to generate a new tink_pb2.Keyset with
 tink_pb2.KeysetHandle. To generate a new keyset that contains a single
-hmac_pb2.HmacKey, one can do:
-handle = keyset_handle.KeysetHandle(mac_key_templates.HMAC_SHA256_128BITTAG).
+aes_eax_pb2.AesEaxKey, one can do:
+handle = keyset_handle.KeysetHandle(aead_key_templates.AES128_EAX).
 """
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
-from tink.proto import aes_cmac_pb2
+from tink.proto import aes_cmac_prf_pb2
 from tink.proto import common_pb2
-from tink.proto import hmac_pb2
+from tink.proto import hkdf_prf_pb2
+from tink.proto import hmac_prf_pb2
 from tink.proto import tink_pb2
 
+_AES_CMAC_PRF_KEY_TYPE_URL = (
+    'type.googleapis.com/google.crypto.tink.AesCmacPrfKey')
+_HMAC_PRF_KEY_TYPE_URL = 'type.googleapis.com/google.crypto.tink.HmacPrfKey'
+_HKDF_PRF_KEY_TYPE_URL = 'type.googleapis.com/google.crypto.tink.HkdfPrfKey'
+
+
+def _create_aes_cmac_key_template(key_size: int) -> tink_pb2.KeyTemplate:
+  """Creates an AES CMAC PRF KeyTemplate, and fills in its values."""
+  key_format = aes_cmac_prf_pb2.AesCmacPrfKeyFormat()
+  key_format.key_size = key_size
+  key_format.version = 0
+  key_template = tink_pb2.KeyTemplate()
+  key_template.value = key_format.SerializeToString()
+  key_template.type_url = _AES_CMAC_PRF_KEY_TYPE_URL
+  key_template.output_prefix_type = tink_pb2.RAW
+  return key_template
+
 
-def create_hmac_key_template(
-    key_size: int, tag_size: int,
-    hash_type: common_pb2.HashType) -> tink_pb2.KeyTemplate:
-  """Creates a HMAC KeyTemplate, and fills in its values."""
-  key_format = hmac_pb2.HmacKeyFormat()
+def _create_hmac_key_template(
+    key_size: int, hash_type: common_pb2.HashType) -> tink_pb2.KeyTemplate:
+  """Creates an HMAC PRF KeyTemplate, and fills in its values."""
+  key_format = hmac_prf_pb2.HmacPrfKeyFormat()
   key_format.params.hash = hash_type
-  key_format.params.tag_size = tag_size
   key_format.key_size = key_size
+  key_format.version = 0
   key_template = tink_pb2.KeyTemplate()
   key_template.value = key_format.SerializeToString()
-  key_template.type_url = 'type.googleapis.com/google.crypto.tink.HmacKey'
-  key_template.output_prefix_type = tink_pb2.TINK
+  key_template.type_url = _HMAC_PRF_KEY_TYPE_URL
+  key_template.output_prefix_type = tink_pb2.RAW
   return key_template
 
 
-def create_aes_cmac_key_template(
-    key_size: int, tag_size: int) -> tink_pb2.KeyTemplate:
-  """"Creates an AES-CMAC KeyTemplate, and fills in its values."""
-  key_format = aes_cmac_pb2.AesCmacKeyFormat()
+def _create_hkdf_key_template(
+    key_size: int, hash_type: common_pb2.HashType) -> tink_pb2.KeyTemplate:
+  """Creates an HKDF PRF KeyTemplate, and fills in its values."""
+  key_format = hkdf_prf_pb2.HkdfPrfKeyFormat()
+  key_format.params.hash = hash_type
   key_format.key_size = key_size
-  key_format.params.tag_size = tag_size
+  key_format.version = 0
   key_template = tink_pb2.KeyTemplate()
   key_template.value = key_format.SerializeToString()
-  key_template.type_url = 'type.googleapis.com/google.crypto.tink.AesCmacKey'
-  key_template.output_prefix_type = tink_pb2.TINK
+  key_template.type_url = _HKDF_PRF_KEY_TYPE_URL
+  key_template.output_prefix_type = tink_pb2.RAW
   return key_template
 
 
-AES_CMAC = create_aes_cmac_key_template(key_size=32, tag_size=16)
-HMAC_SHA256_128BITTAG = create_hmac_key_template(
-    key_size=32, tag_size=16, hash_type=common_pb2.SHA256)
-HMAC_SHA256_256BITTAG = create_hmac_key_template(
-    key_size=32, tag_size=32, hash_type=common_pb2.SHA256)
-HMAC_SHA512_256BITTAG = create_hmac_key_template(
-    key_size=64, tag_size=32, hash_type=common_pb2.SHA512)
-HMAC_SHA512_512BITTAG = create_hmac_key_template(
-    key_size=64, tag_size=64, hash_type=common_pb2.SHA512)
+AES_CMAC = _create_aes_cmac_key_template(key_size=32)
+HMAC_SHA256 = _create_hmac_key_template(
+    key_size=32, hash_type=common_pb2.SHA256)
+HMAC_SHA512 = _create_hmac_key_template(
+    key_size=64, hash_type=common_pb2.SHA512)
+HKDF_SHA256 = _create_hkdf_key_template(
+    key_size=32, hash_type=common_pb2.SHA256)
```

### Comparing `tink-1.6.1/tink/prf/_prf_key_manager.py` & `tink-1.7.0/tink/prf/_prf_key_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,19 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Python wrapper of the wrapped C++ PRF Set key manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from tink import core
 from tink.cc.pybind import tink_bindings
 from tink.prf import _prf_set
 from tink.prf import _prf_set_wrapper
 
 
 class PrfCcToPyWrapper(_prf_set.Prf):
```

### Comparing `tink-1.6.1/tink/prf/BUILD.bazel` & `tink-1.7.0/tink/prf/BUILD.bazel`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     ],
 )
 
 py_library(
     name = "_prf_set",
     srcs = ["_prf_set.py"],
     srcs_version = "PY3",
-    deps = [requirement("six")],
 )
 
 py_library(
     name = "_prf_key_manager",
     srcs = ["_prf_key_manager.py"],
     srcs_version = "PY3",
     deps = [
@@ -35,28 +34,24 @@
         "//tink/core",
     ],
 )
 
 py_test(
     name = "_prf_key_manager_test",
     srcs = ["_prf_key_manager_test.py"],
-    data = [
-        "@tink_base//testdata/templates",
-    ],
     srcs_version = "PY3",
     deps = [
         ":prf",
         requirement("absl-py"),
         "//tink:tink_python",
         "//tink/core",
         "//tink/proto:common_py_pb2",
         "//tink/proto:hkdf_prf_py_pb2",
         "//tink/proto:hmac_prf_py_pb2",
         "//tink/proto:tink_py_pb2",
-        "//tink/testing:helper",
     ],
 )
 
 py_library(
     name = "_prf_set_wrapper",
     srcs = ["_prf_set_wrapper.py"],
     srcs_version = "PY3",
```

### Comparing `tink-1.6.1/tink/prf/_prf_key_manager_test.py` & `tink-1.7.0/tink/prf/_prf_key_manager_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,45 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.prf.prf_set_key_manager."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 from absl.testing import parameterized
 from tink.proto import common_pb2
 from tink.proto import hmac_prf_pb2
 from tink.proto import tink_pb2
 import tink
 from tink import core
 from tink import prf
-from tink.testing import helper
 
 
 def setUpModule():
   prf.register()
 
 
 class PrfKeyManagerTest(parameterized.TestCase):
 
-  @parameterized.parameters([
-      ('AES_CMAC_PRF', prf.prf_key_templates.AES_CMAC),
-      ('HMAC_PRF_SHA256', prf.prf_key_templates.HMAC_SHA256),
-      ('HMAC_PRF_SHA512', prf.prf_key_templates.HMAC_SHA512),
-      ('HKDF_PRF_SHA256', prf.prf_key_templates.HKDF_SHA256)
-  ])
-  def test_template(self, template_name, template):
-    self.assertEqual(template,
-                     helper.template_from_testdata(template_name, 'prf'))
-
   def test_new_key_data_success(self):
     key_template = prf.prf_key_templates._create_hmac_key_template(
         key_size=32, hash_type=common_pb2.SHA256)
     key_manager = core.Registry.key_manager(key_template.type_url)
     key_data = key_manager.new_key_data(key_template)
     self.assertEqual(key_data.type_url, key_template.type_url)
     self.assertEqual(key_data.key_material_type, tink_pb2.KeyData.SYMMETRIC)
```

### Comparing `tink-1.6.1/tink/prf/_prf_set_wrapper.py` & `tink-1.7.0/tink/prf/_prf_set_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """PrfSet wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 from typing import Type, Mapping
 from tink import core
 from tink.prf import _prf_set
 
 
 class _WrappedPrfSet(_prf_set.PrfSet):
   """Implements PrfSet for a set of PrfSet primitives."""
```

### Comparing `tink-1.6.1/tink/prf/_prf_set.py` & `tink-1.7.0/tink/prf/_prf_set.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,27 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module defines the interface for PrfSet."""
 
-from __future__ import absolute_import
-from __future__ import division
-# Placeholder for import for type annotations
-from __future__ import print_function
-
 import abc
 from typing import Mapping
-# Special imports
-import six
 
 
-@six.add_metaclass(abc.ABCMeta)
-class Prf(object):
+class Prf(metaclass=abc.ABCMeta):
   """An element of a pseudo random function family, selected by a key.
 
   The PRF interface is an abstraction for an element of a pseudo random function
   family, selected by a key. It has the following properties:
 
   - It is deterministic: Prf.compute(input, length) will always return the same
     output if the same key is used. Prf.compute(input, length1) will be a prefix
@@ -63,16 +55,15 @@
 
     Returns:
       the first output_length bytes of the PRF.
     """
     raise NotImplementedError()
 
 
-@six.add_metaclass(abc.ABCMeta)
-class PrfSet(object):
+class PrfSet(metaclass=abc.ABCMeta):
   """A Tink Keyset can be converted into a set of PRFs using this primitive.
 
   Every key in the keyset corresponds to a PRF in the PrfSet. Every PRF in the
   set is given an ID, which is the same ID as the key id in the Keyset.
   """
 
   @abc.abstractmethod
```

### Comparing `tink-1.6.1/tink/prf/_prf_set_wrapper_test.py` & `tink-1.7.0/tink/prf/_prf_set_wrapper_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for tink.python.tink.aead_wrapper."""
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
 from absl.testing import absltest
 import tink
 from tink import prf
 from tink.testing import keyset_builder
 
 
 TEMPLATE = prf.prf_key_templates.HMAC_SHA256
```

### Comparing `tink-1.6.1/tink.egg-info/SOURCES.txt` & `tink-1.7.0/tink.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 tink/_keyset_handle_test.py
 tink/_keyset_reader.py
 tink/_keyset_reader_test.py
 tink/_keyset_writer.py
 tink/_keyset_writer_test.py
 tink/cleartext_keyset_handle.py
 tink/cleartext_keyset_handle_test.py
+tink/secret_key_access.py
+tink/secret_key_access_test.py
 tink/tink_config.py
 tink/tink_config_test.py
 tink.egg-info/PKG-INFO
 tink.egg-info/SOURCES.txt
 tink.egg-info/dependency_links.txt
 tink.egg-info/not-zip-safe
 tink.egg-info/requires.txt
@@ -33,14 +35,16 @@
 tink/aead/_aead_key_templates.py
 tink/aead/_aead_key_templates_test.py
 tink/aead/_aead_wrapper.py
 tink/aead/_aead_wrapper_test.py
 tink/aead/_kms_envelope_aead.py
 tink/aead/_kms_envelope_aead_test.py
 tink/cc/BUILD.bazel
+tink/cc/cc_hpke_config.cc
+tink/cc/cc_hpke_config.h
 tink/cc/cc_jwt_config.cc
 tink/cc/cc_jwt_config.h
 tink/cc/cc_key_manager.h
 tink/cc/cc_streaming_aead_wrappers.cc
 tink/cc/cc_streaming_aead_wrappers.h
 tink/cc/cc_streaming_aead_wrappers_test.cc
 tink/cc/cc_tink_config.cc
@@ -64,14 +68,16 @@
 tink/cc/pybind/aead.h
 tink/cc/pybind/cc_aws_kms_client.cc
 tink/cc/pybind/cc_aws_kms_client.h
 tink/cc/pybind/cc_fake_kms_client_testonly.cc
 tink/cc/pybind/cc_fake_kms_client_testonly.h
 tink/cc/pybind/cc_gcp_kms_client.cc
 tink/cc/pybind/cc_gcp_kms_client.h
+tink/cc/pybind/cc_hpke_config.cc
+tink/cc/pybind/cc_hpke_config.h
 tink/cc/pybind/cc_jwt_config.cc
 tink/cc/pybind/cc_jwt_config.h
 tink/cc/pybind/cc_key_manager.cc
 tink/cc/pybind/cc_key_manager.h
 tink/cc/pybind/cc_key_manager_test.py
 tink/cc/pybind/cc_streaming_aead_wrappers.cc
 tink/cc/pybind/cc_streaming_aead_wrappers.h
@@ -96,25 +102,18 @@
 tink/cc/pybind/prf.h
 tink/cc/pybind/public_key_sign.cc
 tink/cc/pybind/public_key_sign.h
 tink/cc/pybind/public_key_verify.cc
 tink/cc/pybind/public_key_verify.h
 tink/cc/pybind/python_file_object_adapter.cc
 tink/cc/pybind/python_file_object_adapter.h
-tink/cc/pybind/status.cc
-tink/cc/pybind/status.h
-tink/cc/pybind/status_casters.h
-tink/cc/pybind/status_injector.cc
-tink/cc/pybind/status_injector.h
-tink/cc/pybind/status_test.py
-tink/cc/pybind/status_utils.cc
-tink/cc/pybind/status_utils.h
 tink/cc/pybind/streaming_aead.cc
 tink/cc/pybind/streaming_aead.h
 tink/cc/pybind/tink_bindings.cc
+tink/cc/pybind/tink_exception.h
 tink/core/BUILD.bazel
 tink/core/__init__.py
 tink/core/_crypto_format.py
 tink/core/_crypto_format_test.py
 tink/core/_key_manager.py
 tink/core/_primitive_set.py
 tink/core/_primitive_set_test.py
@@ -148,16 +147,24 @@
 tink/integration/awskms/_aws_kms_client.py
 tink/integration/awskms/_aws_kms_client_test.py
 tink/integration/gcpkms/BUILD.bazel
 tink/integration/gcpkms/__init__.py
 tink/integration/gcpkms/_gcp_kms_aead_test.py
 tink/integration/gcpkms/_gcp_kms_client.py
 tink/integration/gcpkms/_gcp_kms_client_test.py
+tink/internal/BUILD.bazel
+tink/internal/__init__.py
+tink/internal/big_integer_util.py
+tink/internal/big_integer_util_test.py
 tink/jwt/BUILD.bazel
 tink/jwt/__init__.py
+tink/jwt/_json_util.py
+tink/jwt/_json_util_test.py
+tink/jwt/_jwk_set_converter.py
+tink/jwt/_jwk_set_converter_test.py
 tink/jwt/_jwt_error.py
 tink/jwt/_jwt_format.py
 tink/jwt/_jwt_format_test.py
 tink/jwt/_jwt_hmac_key_manager.py
 tink/jwt/_jwt_hmac_key_manager_test.py
 tink/jwt/_jwt_key_templates.py
 tink/jwt/_jwt_key_templates_test.py
@@ -261,35 +268,32 @@
 tink/proto/rsa_ssa_pss_pb2.py
 tink/proto/test_proto.proto
 tink/proto/test_proto_pb2.py
 tink/proto/tink.proto
 tink/proto/tink_pb2.py
 tink/proto/xchacha20_poly1305.proto
 tink/proto/xchacha20_poly1305_pb2.py
-tink/proto/experimental/pqcrypto/cecpq2_aead_hkdf.proto
-tink/proto/experimental/pqcrypto/dilithium.proto
-tink/proto/testing/testing_api.proto
 tink/signature/BUILD.bazel
 tink/signature/__init__.py
 tink/signature/_public_key_sign.py
 tink/signature/_public_key_verify.py
 tink/signature/_signature_key_manager.py
 tink/signature/_signature_key_manager_test.py
 tink/signature/_signature_key_templates.py
-tink/signature/_signature_key_templates_test.py
 tink/signature/_signature_wrapper.py
 tink/signature/_signature_wrapper_test.py
 tink/streaming_aead/BUILD.bazel
 tink/streaming_aead/__init__.py
 tink/streaming_aead/_decrypting_stream.py
 tink/streaming_aead/_decrypting_stream_test.py
 tink/streaming_aead/_encrypting_stream.py
 tink/streaming_aead/_encrypting_stream_test.py
 tink/streaming_aead/_file_object_adapter.py
 tink/streaming_aead/_file_object_adapter_test.py
+tink/streaming_aead/_pybind11_python_file_object_adapter_test.py
 tink/streaming_aead/_raw_streaming_aead.py
 tink/streaming_aead/_rewindable_input_stream.py
 tink/streaming_aead/_rewindable_input_stream_test.py
 tink/streaming_aead/_streaming_aead.py
 tink/streaming_aead/_streaming_aead_key_manager.py
 tink/streaming_aead/_streaming_aead_key_manager_test.py
 tink/streaming_aead/_streaming_aead_key_templates.py
```

### Comparing `tink-1.6.1/tink.egg-info/PKG-INFO` & `tink-1.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tink
-Version: 1.6.1
+Version: 1.7.0
 Summary: A multi-language, cross-platform library that provides cryptographic APIs that are secure, easy to use correctly, and hard(er) to misuse.
 Home-page: https://github.com/google/tink
 Author: Tink Developers
 Author-email: tink-users@googlegroups.com
 License: Apache 2.0
 Keywords: tink cryptography
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 
 # Tink
@@ -27,15 +26,12 @@
 It reduces common crypto pitfalls with user-centered design, careful
 implementation and code reviews, and extensive testing. At Google, Tink is
 already being used to secure data of many products such as AdMob, Google Pay,
 Google Assistant, Firebase, the Android Search App, etc.
 
 ## Documentation
 
-For an overview of using Tink in Python, see the
-[Python HOW-TO](../docs/PYTHON-HOWTO.md).
+For an overview of using Tink in Python, see https://developers.google.com/tink.
 
 In addition, there are illustrative [examples of using Tink
 Python](https://github.com/google/tink/tree/master/examples/python/) which can
 used as a jumping off point.
-
-
```

### Comparing `tink-1.6.1/tools/build_defs/tink_python_rules.bzl` & `tink-1.7.0/tools/build_defs/tink_python_rules.bzl`

 * *Files 6% similar despite different names*

```diff
@@ -10,50 +10,41 @@
         deps = []):
     """
     Pybind Extension for Tink.
 
     Creates Bazel targets for a pybind module:
     - A py_library with the taret name
     - A cc_binary with the target name.so
-    - A cc_library with the target name_cc
 
     Args:
       name: name of the target
       srcs: source files corresponding to the target
       hdrs: header files corresponding to the target
       copts: flags for the compiler
       linkopts: flags for the linker
       features: features enabled for Bazel
       deps: dependencies of the target
 
     Returns:
       A py_library target.
     """
     shared_lib_name = name + ".so"
-    cc_library_name = name + "_cc"
     native.cc_binary(
         name = shared_lib_name,
         linkshared = 1,
         linkstatic = 1,
         srcs = srcs + hdrs,
         copts = copts + ["-fvisibility=hidden"],
         linkopts = linkopts + select({
             "@pybind11//:osx": [],
             "//conditions:default": ["-Wl,-Bsymbolic"],
         }),
         features = features,
         deps = deps,
     )
-    native.cc_library(
-        name = cc_library_name,
-        srcs = srcs,
-        hdrs = hdrs,
-        deps = deps,
-        alwayslink = True,
-    )
 
     # Extract Python targets from deps
     pybind_deps = [dep[:-3] for dep in deps if dep.endswith("_cc")]
     native.py_library(
         name = name,
         data = [shared_lib_name],
         deps = pybind_deps,
```

### Comparing `tink-1.6.1/tools/distribution/test_linux_binary_wheels.sh` & `tink-1.7.0/tools/distribution/test_linux_binary_wheels.sh`

 * *Files 8% similar despite different names*

```diff
@@ -17,34 +17,42 @@
 
 set -euo pipefail
 
 # The following assoicative array contains:
 #   ["<Python version>"]="<python tag>-<abi tag>"
 # where:
 #   <Python version> = language version, e.g "3.7"
-#   <python tag-<abi tag> = tags as specified in in PEP 491, e.g. "cp37-37m"
+#   <python tag>, <abi tag> = as defined at
+#       https://packaging.python.org/en/latest/specifications/, e.g. "cp37-37m"
 declare -A PYTHON_VERSIONS
 PYTHON_VERSIONS["3.7"]="cp37-cp37m"
 PYTHON_VERSIONS["3.8"]="cp38-cp38"
 PYTHON_VERSIONS["3.9"]="cp39-cp39"
+PYTHON_VERSIONS["3.10"]="cp310-cp310"
 readonly -A PYTHON_VERSIONS
 
-export TINK_SRC_PATH="/tmp/tink"
+# This is a compressed tag set as specified at
+# https://peps.python.org/pep-0425/#compressed-tag-sets
+#
+# Keep in sync with the output of the auditwheel tool.
+readonly PLATFORM_TAG_SET="manylinux_2_17_x86_64.manylinux2014_x86_64"
+
+export TINK_PYTHON_ROOT_PATH="${PWD}"
 
 # Required to fix https://github.com/pypa/manylinux/issues/357.
 export LD_LIBRARY_PATH="/usr/local/lib"
 
 # This link is required on CentOS, as curl used in the AWS SDK looks for the
 # certificates in this location. Removing this line will cause the AWS KMS tests
 # to fail.
 ln -s /etc/ssl/certs/ca-bundle.trust.crt /etc/ssl/certs/ca-certificates.crt
 
 for v in "${!PYTHON_VERSIONS[@]}"; do
   (
     # Executing in a subshell to make the PATH modification temporary.
     export PATH="${PATH}:/opt/python/${PYTHON_VERSIONS[$v]}/bin"
 
-    pip3 install release/*-"${PYTHON_VERSIONS[$v]}"-manylinux2014_x86_64.whl
+    pip3 install release/*-"${PYTHON_VERSIONS[$v]}"-"${PLATFORM_TAG_SET}".whl
     find tink/ -not -path "*cc/pybind*" -type f -name "*_test.py" -print0 \
       | xargs -0 -n1 python3
   )
 done
```

### Comparing `tink-1.6.1/tools/distribution/build_linux_binary_wheels.sh` & `tink-1.7.0/tools/distribution/build_linux_binary_wheels.sh`

 * *Files 10% similar despite different names*

```diff
@@ -21,38 +21,42 @@
 
 set -euo pipefail
 
 # The following assoicative array contains:
 #   ["<Python version>"]="<python tag>-<abi tag>"
 # where:
 #   <Python version> = language version, e.g "3.7"
-#   <python tag-<abi tag> = tags as specified in in PEP 491, e.g. "cp37-37m"
+#   <python tag>, <abi tag> = as defined at
+#       https://packaging.python.org/en/latest/specifications/, e.g. "cp37-37m"
 declare -A PYTHON_VERSIONS
 PYTHON_VERSIONS["3.7"]="cp37-cp37m"
 PYTHON_VERSIONS["3.8"]="cp38-cp38"
 PYTHON_VERSIONS["3.9"]="cp39-cp39"
+PYTHON_VERSIONS["3.10"]="cp310-cp310"
 readonly -A PYTHON_VERSIONS
 
-readonly BAZEL_VERSION='3.7.2'
-readonly PROTOC_VERSION='3.14.0'
+export TINK_PYTHON_ROOT_PATH="${PWD}"
+
+readonly BAZEL_VERSION="$(cat ${TINK_PYTHON_ROOT_PATH}/.bazelversion)"
+readonly PROTOC_VERSION="3.19.3"
 
 # Get dependencies which are needed for building Tink.
 
 # Install Bazel. Needed for building C++ extensions.
 curl -OL "https://github.com/bazelbuild/bazel/releases/download/${BAZEL_VERSION}/bazel-${BAZEL_VERSION}-installer-linux-x86_64.sh"
 chmod +x "bazel-${BAZEL_VERSION}-installer-linux-x86_64.sh"
 ./"bazel-${BAZEL_VERSION}-installer-linux-x86_64.sh"
 
 # Install protoc. Needed for protocol buffer compilation.
 PROTOC_ZIP="protoc-${PROTOC_VERSION}-linux-x86_64.zip"
 curl -OL "https://github.com/protocolbuffers/protobuf/releases/download/v${PROTOC_VERSION}/${PROTOC_ZIP}"
 unzip -o "${PROTOC_ZIP}" -d /usr/local bin/protoc
 
 # Setup required for Tink.
-export TINK_PYTHON_SETUPTOOLS_OVERRIDE_BASE_PATH="/tmp/tink"
+export TINK_PYTHON_SETUPTOOLS_OVERRIDE_BASE_PATH="${TINK_PYTHON_ROOT_PATH}/.."
 
 # Workaround for grpc which expects a python2 installation, which is not present
 # in the manylinux2014 container. Cannot be an empty string, otherwise Bazel
 # will fail.
 export PYTHON2_BIN_PATH="non_existent_file"
 export PYTHON2_LIB_PATH="non_existent_file"
```

### Comparing `tink-1.6.1/tools/distribution/README.md` & `tink-1.7.0/tools/distribution/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 
 ## Building the release
 
 In order to generate a release run `./tools/distribution/create_release.sh` from
 the `python/` folder. Note that this requires [Docker](https://www.docker.com)
 to be installed, as it makes use of the
 [pypa images](https://github.com/pypa/manylinux) to build
-[PEP 599](https://www.python.org/dev/peps/pep-0599/) conform wheels.
+[PEP 599](https://www.python.org/dev/peps/pep-0599/) conformant wheels.
 
 This will carry out the following three steps:
 
 *   Create binary wheels in a Docker container for Linux.
 *   Create a source distribution of the Python package.
 *   Run automatic tests against the packages created.
 
 The resulting packages of this process will be stored in `python/release` and
 can be distributed. The binary wheels can be installed on Linux without
 Bazel/protoc being available. Currently this supports building binary wheels
 for:
 
-*   manylinux2014_x86_64: Python 3.7, 3.8
+*   manylinux2014_x86_64: Python 3.7, 3.8, 3.9, 3.10
 
 The binary wheels are tested inside a Docker container with the corresponding
 Python versions.
 
 The source distribution still needs to compile the C++ bindings, which requires
 Bazel, protoc and the Tink repository to be available. The path to the Tink
 repository can be set with `TINK_PYTHON_SETUPTOOLS_OVERRIDE_BASE_PATH`. The
-source distribution is tested on the machine which the script is run.
+source distribution is tested on the machine where the script is run.
 
 ## Publishing the release
 
 The output generated in the previous step can directly be used for upload to
 PyPI. It is recommended to first upload it to the
 [test repository](https://test.pypi.org):
```

### Comparing `tink-1.6.1/tink_py_deps.bzl` & `tink-1.7.0/tink_py_deps.bzl`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
 
 def tink_py_deps():
     """ Loads dependencies of Python Tink.
     """
 
     if not native.existing_rule("rules_python"):
-        # Commit from 2020-03-05
+        # Release from 2022-01-05
         http_archive(
             name = "rules_python",
-            strip_prefix = "rules_python-748aa53d7701e71101dfd15d800e100f6ff8e5d1",
-            url = "https://github.com/bazelbuild/rules_python/archive/748aa53d7701e71101dfd15d800e100f6ff8e5d1.zip",
-            sha256 = "d3e40ca3b7e00b72d2b1585e0b3396bcce50f0fc692e2b7c91d8b0dc471e3eaf",
+            sha256 = "a30abdfc7126d497a7698c29c46ea9901c6392d6ed315171a6df5ce433aa4502",
+            strip_prefix = "rules_python-0.6.0",
+            url = "https://github.com/bazelbuild/rules_python/archive/0.6.0.tar.gz",
         )
 
     if not native.existing_rule("pybind11"):
+        # Commit from 2021-12-28
         http_archive(
             name = "pybind11",
             build_file = "@pybind11_bazel//:pybind11.BUILD",
-            strip_prefix = "pybind11-2.4.3",
-            urls = ["https://github.com/pybind/pybind11/archive/v2.4.3.tar.gz"],
-            sha256 = "1eed57bc6863190e35637290f97a20c81cfe4d9090ac0a24f3bbf08f265eb71d",
+            strip_prefix = "pybind11-2.9.0",
+            urls = ["https://github.com/pybind/pybind11/archive/v2.9.0.tar.gz"],
+            sha256 = "057fb68dafd972bc13afb855f3b0d8cf0fa1a78ef053e815d9af79be7ff567cb",
         )
 
     if not native.existing_rule("pybind11_bazel"):
-        # Commit from 2020-04-09
+        # Commit from 2021-01-05
         http_archive(
             name = "pybind11_bazel",
-            strip_prefix = "pybind11_bazel-34206c29f891dbd5f6f5face7b91664c2ff7185c",
-            url = "https://github.com/pybind/pybind11_bazel/archive/34206c29f891dbd5f6f5face7b91664c2ff7185c.zip",
-            sha256 = "8d0b776ea5b67891f8585989d54aa34869fc12f14bf33f1dc7459458dd222e95",
+            strip_prefix = "pybind11_bazel-72cbbf1fbc830e487e3012862b7b720001b70672",
+            url = "https://github.com/pybind/pybind11_bazel/archive/72cbbf1fbc830e487e3012862b7b720001b70672.zip",
+            sha256 = "fec6281e4109115c5157ca720b8fe20c8f655f773172290b03f57353c11869c2",
         )
```

### Comparing `tink-1.6.1/setup.py` & `tink-1.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         Instead of providing a URL of an archive of the current master branch,
         instead link to an archive that correspond with the tagged version (e.g.
         for creating release artifacts).
 
   Args:
     workspace_content: The original tink/python WORKSPACE.
   Returns:
-    The workspace_content using http_archive for tink_base and tink_cc.
+    The workspace_content using http_archive for tink_cc.
   """
 
   if 'TINK_PYTHON_SETUPTOOLS_OVERRIDE_BASE_PATH' in os.environ:
     base_path = os.environ['TINK_PYTHON_SETUPTOOLS_OVERRIDE_BASE_PATH']
     return _patch_with_local_path(workspace_content, base_path)
 
   if 'TINK_PYTHON_SETUPTOOLS_TAGGED_VERSION' in os.environ:
@@ -137,70 +137,94 @@
   return _patch_with_http_archive(workspace_content,
                                   'master.zip', 'tink-master')
 
 
 def _patch_with_local_path(workspace_content, base_path):
   """Replaces the base paths in the local_repository() rules."""
 
-  workspace_content = re.sub(r'(?<="tink_base",\n    path = ").*(?=\n)',
-                             base_path + '",  # Modified by setup.py',
-                             workspace_content)
   workspace_content = re.sub(r'(?<="tink_cc",\n    path = ").*(?=\n)',
                              base_path + '/cc",  # Modified by setup.py',
                              workspace_content)
+  workspace_content = re.sub(
+      r'(?<="tink_cc_awskms",\n    path = ").*(?=\n)',
+      base_path + '/cc/integration/awskms",  # Modified by setup.py',
+      workspace_content)
+  workspace_content = re.sub(
+      r'(?<="tink_cc_gcpkms",\n    path = ").*(?=\n)',
+      base_path + '/cc/integration/gcpkms",  # Modified by setup.py',
+      workspace_content)
   return workspace_content
 
 
 def _patch_with_http_archive(workspace_content, filename, prefix):
   """Replaces local_repository() rules with http_archive() rules."""
 
   workspace_lines = workspace_content.split('\n')
   http_archive_load = ('load("@bazel_tools//tools/build_defs/repo:http.bzl", '
                        '"http_archive")')
   workspace_content = '\n'.join([workspace_lines[0], http_archive_load] +
                                 workspace_lines[1:])
 
-  base = textwrap.dedent(
+  cc = textwrap.dedent(
       '''\
       local_repository(
-          name = "tink_base",
-          path = "..",
+          name = "tink_cc",
+          path = "../cc",
       )
       ''')
 
-  cc = textwrap.dedent(
+  cc_awskms = textwrap.dedent(
       '''\
       local_repository(
-          name = "tink_cc",
-          path = "../cc",
+          name = "tink_cc_awskms",
+          path = "../cc/integration/awskms",
       )
       ''')
 
-  base_patched = textwrap.dedent(
+  cc_gcpkms = textwrap.dedent(
+      '''\
+      local_repository(
+          name = "tink_cc_gcpkms",
+          path = "../cc/integration/gcpkms",
+      )
+      ''')
+
+  cc_patched = textwrap.dedent(
       '''\
       # Modified by setup.py
       http_archive(
-          name = "tink_base",
+          name = "tink_cc",
           urls = ["https://github.com/google/tink/archive/{}"],
-          strip_prefix = "{}/",
+          strip_prefix = "{}/cc",
       )
       '''.format(filename, prefix))
 
-  cc_patched = textwrap.dedent(
+  cc_awskms_patched = textwrap.dedent(
       '''\
       # Modified by setup.py
       http_archive(
-          name = "tink_cc",
+          name = "tink_cc_awskms",
           urls = ["https://github.com/google/tink/archive/{}"],
-          strip_prefix = "{}/cc",
+          strip_prefix = "{}/cc/integration/awskms",
+      )
+      '''.format(filename, prefix))
+
+  cc_gcpkms_patched = textwrap.dedent(
+      '''\
+      # Modified by setup.py
+      http_archive(
+          name = "tink_cc_gcpkms",
+          urls = ["https://github.com/google/tink/archive/{}"],
+          strip_prefix = "{}/cc/integration/gcpkms",
       )
       '''.format(filename, prefix))
 
-  workspace_content = workspace_content.replace(base, base_patched)
   workspace_content = workspace_content.replace(cc, cc_patched)
+  workspace_content = workspace_content.replace(cc_awskms, cc_awskms_patched)
+  workspace_content = workspace_content.replace(cc_gcpkms, cc_gcpkms_patched)
   return workspace_content
 
 
 class BazelExtension(setuptools.Extension):
   """A C/C++ extension that is defined as a Bazel BUILD target."""
 
   def __init__(self, bazel_target, target_name=''):
@@ -223,15 +247,15 @@
 
   def run(self):
     for ext in self.extensions:
       self.bazel_build(ext)
     build_ext.build_ext.run(self)
 
   def bazel_build(self, ext):
-    # Change WORKSPACE to include tink_base and tink_cc from an archive
+    # Change WORKSPACE to include tink_cc from an archive
     with open('WORKSPACE', 'r') as f:
       workspace_contents = f.read()
     with open('WORKSPACE', 'w') as f:
       f.write(_patch_workspace(workspace_contents))
 
     if not os.path.exists(self.build_temp):
       os.makedirs(self.build_temp)
```

### Comparing `tink-1.6.1/PKG-INFO` & `tink-1.7.0/tink.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: tink
-Version: 1.6.1
+Version: 1.7.0
 Summary: A multi-language, cross-platform library that provides cryptographic APIs that are secure, easy to use correctly, and hard(er) to misuse.
 Home-page: https://github.com/google/tink
 Author: Tink Developers
 Author-email: tink-users@googlegroups.com
 License: Apache 2.0
 Keywords: tink cryptography
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 
 # Tink
@@ -27,15 +26,12 @@
 It reduces common crypto pitfalls with user-centered design, careful
 implementation and code reviews, and extensive testing. At Google, Tink is
 already being used to secure data of many products such as AdMob, Google Pay,
 Google Assistant, Firebase, the Android Search App, etc.
 
 ## Documentation
 
-For an overview of using Tink in Python, see the
-[Python HOW-TO](../docs/PYTHON-HOWTO.md).
+For an overview of using Tink in Python, see https://developers.google.com/tink.
 
 In addition, there are illustrative [examples of using Tink
 Python](https://github.com/google/tink/tree/master/examples/python/) which can
 used as a jumping off point.
-
-
```

### Comparing `tink-1.6.1/WORKSPACE` & `tink-1.7.0/WORKSPACE`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,46 @@
 workspace(name = "tink_py")
 
 local_repository(
-    name = "tink_base",
-    path = "..",
+    name = "tink_cc",
+    path = "/tmp/tink/python/../cc",  # Modified by setup.py
 )
 
 local_repository(
-    name = "tink_cc",
-    path = "../cc",
+    name = "tink_cc_awskms",
+    path = "/tmp/tink/python/../cc/integration/awskms",  # Modified by setup.py
+)
+
+local_repository(
+    name = "tink_cc_gcpkms",
+    path = "/tmp/tink/python/../cc/integration/gcpkms",  # Modified by setup.py
 )
 
 # Need to load rules_python earlier as proto uses an older version which is
 # incompatible with our Python implementation will load
 load("@tink_py//:tink_py_deps.bzl", "tink_py_deps")
+
 tink_py_deps()
 
 load("@tink_py//:tink_py_deps_init.bzl", "tink_py_deps_init")
-tink_py_deps_init("tink_py")
-
-load("@tink_py_pip_deps//:requirements.bzl", "pip_install")
-pip_install()
-
-load("@tink_base//:tink_base_deps.bzl", "tink_base_deps")
-tink_base_deps()
 
-load("@tink_base//:tink_base_deps_init.bzl", "tink_base_deps_init")
-tink_base_deps_init()
+tink_py_deps_init("tink_py")
 
 load("@tink_cc//:tink_cc_deps.bzl", "tink_cc_deps")
+
 tink_cc_deps()
 
 load("@tink_cc//:tink_cc_deps_init.bzl", "tink_cc_deps_init")
+
 tink_cc_deps_init()
+
+load("@tink_cc_awskms//:tink_cc_awskms_deps.bzl", "tink_cc_awskms_deps")
+
+tink_cc_awskms_deps()
+
+load("@tink_cc_gcpkms//:tink_cc_gcpkms_deps.bzl", "tink_cc_gcpkms_deps")
+
+tink_cc_gcpkms_deps()
+
+load("@tink_cc_gcpkms//:tink_cc_gcpkms_deps_init.bzl", "tink_cc_gcpkms_deps_init")
+
+tink_cc_gcpkms_deps_init()
```

### Comparing `tink-1.6.1/README.md` & `tink-1.7.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -11,13 +11,12 @@
 It reduces common crypto pitfalls with user-centered design, careful
 implementation and code reviews, and extensive testing. At Google, Tink is
 already being used to secure data of many products such as AdMob, Google Pay,
 Google Assistant, Firebase, the Android Search App, etc.
 
 ## Documentation
 
-For an overview of using Tink in Python, see the
-[Python HOW-TO](../docs/PYTHON-HOWTO.md).
+For an overview of using Tink in Python, see https://developers.google.com/tink.
 
 In addition, there are illustrative [examples of using Tink
 Python](https://github.com/google/tink/tree/master/examples/python/) which can
 used as a jumping off point.
```

