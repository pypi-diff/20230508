# Comparing `tmp/pkilint-0.8.2.tar.gz` & `tmp/pkilint-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkilint-0.8.2.tar", last modified: Sat May  6 04:55:15 2023, max compression
+gzip compressed data, was "pkilint-0.8.3.tar", last modified: Mon May  8 20:14:59 2023, max compression
```

## Comparing `pkilint-0.8.2.tar` & `pkilint-0.8.3.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-06 04:55:05.000000 pkilint-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-06 04:55:15.417621 pkilint-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-06 04:55:05.000000 pkilint-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 04:55:05.000000 pkilint-0.8.2/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.409622 pkilint-0.8.2/pkilint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/adobe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/adobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/adobe/adobe_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/adobe/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/adobe/asn1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/convert_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_cabf_serverauth_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_pkix_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/cabf_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/servercert/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/servercert/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/asn1/ev_guidelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/servercert/servercert_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/cabf/smime/
--rw-r--r--   0 runner    (1001) docker     (123)     9554 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/cabf/smime/smime_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/etsi/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint/etsi/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/asn1/en_319_412_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/etsi/asn1/ts_119_495.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/iso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/iso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/iso/lei.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/itu/x520_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/msft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/msft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/msft/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/msft/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/msft/msft_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/certificate/certificate_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/crl/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/crl_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/crl_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/crl/crl_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/general_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/pkilint/pkix/ocsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_basic_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/pkix/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-06 04:55:05.000000 pkilint-0.8.2/pkilint/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.413622 pkilint-0.8.2/pkilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 04:55:15.000000 pkilint-0.8.2/pkilint.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-06 04:55:15.421622 pkilint-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 04:55:05.000000 pkilint-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/tests/integration_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/integration_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/integration_certificate/test_cabf_smime_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:15.417621 pkilint-0.8.2/tests/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/itu/test_bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/itu/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-06 04:55:05.000000 pkilint-0.8.2/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.426457 pkilint-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 20:14:49.000000 pkilint-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-08 20:14:59.426457 pkilint-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-08 20:14:49.000000 pkilint-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 20:14:49.000000 pkilint-0.8.3/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.410457 pkilint-0.8.3/pkilint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/adobe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/adobe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/adobe/adobe_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/adobe/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/adobe/asn1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/convert_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_cabf_serverauth_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_pkix_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/cabf/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/cabf/servercert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/cabf/servercert/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/asn1/ev_guidelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/cabf/smime/
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/etsi/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/etsi/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/asn1/en_319_412_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/asn1/ts_119_495.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/iso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/iso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/iso/lei.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/x520_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/msft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/msft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/msft/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/msft/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/msft/msft_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26221 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/crl_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/crl_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/crl_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/ocsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_basic_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-08 20:14:59.426457 pkilint-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 20:14:49.000000 pkilint-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.426457 pkilint-0.8.3/tests/integration_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/integration_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/integration_certificate/test_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/integration_certificate/test_pkix_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.426457 pkilint-0.8.3/tests/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/itu/test_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/itu/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/util.py
```

### Comparing `pkilint-0.8.2/LICENSE` & `pkilint-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/PKG-INFO` & `pkilint-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.2
+Version: 0.8.3
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.8.2/README.md` & `pkilint-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/adobe/adobe_validator.py` & `pkilint-0.8.3/pkilint/adobe/adobe_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/adobe/asn1/__init__.py` & `pkilint-0.8.3/pkilint/adobe/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/bin/convert_cert.py` & `pkilint-0.8.3/pkilint/bin/convert_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/bin/lint_cabf_serverauth_cert.py` & `pkilint-0.8.3/pkilint/bin/lint_cabf_serverauth_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/bin/lint_cabf_smime_cert.py` & `pkilint-0.8.3/pkilint/bin/lint_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/bin/lint_crl.py` & `pkilint-0.8.3/pkilint/bin/lint_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/bin/lint_ocsp_response.py` & `pkilint-0.8.3/pkilint/bin/lint_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/bin/lint_pkix_cert.py` & `pkilint-0.8.3/pkilint/bin/lint_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/bin/lint_pkix_signer_signee_cert_chain.py` & `pkilint-0.8.3/pkilint/bin/lint_pkix_signer_signee_cert_chain.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/__init__.py` & `pkilint-0.8.3/pkilint/cabf/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/cabf_constants.py` & `pkilint-0.8.3/pkilint/cabf/cabf_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/cabf_crl.py` & `pkilint-0.8.3/pkilint/cabf/cabf_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/cabf_extension.py` & `pkilint-0.8.3/pkilint/cabf/cabf_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/cabf_key.py` & `pkilint-0.8.3/pkilint/cabf/cabf_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/cabf_name.py` & `pkilint-0.8.3/pkilint/cabf/cabf_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/servercert/__init__.py` & `pkilint-0.8.3/pkilint/cabf/servercert/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/servercert/asn1/ev_guidelines.py` & `pkilint-0.8.3/pkilint/cabf/servercert/asn1/ev_guidelines.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/servercert/servercert_extension.py` & `pkilint-0.8.3/pkilint/cabf/servercert/servercert_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/servercert/servercert_key.py` & `pkilint-0.8.3/pkilint/cabf/servercert/servercert_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/servercert/servercert_name.py` & `pkilint-0.8.3/pkilint/cabf/servercert/servercert_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/smime/__init__.py` & `pkilint-0.8.3/pkilint/cabf/smime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 def create_extensions_validator_container(validation_level, generation):
     return certificate.create_extensions_validator_container(
         [
             smime_extension.RequiredPolicyIdentifierValidator(validation_level, generation),
             smime_extension.CertificatePoliciesPresenceValidator(),
             smime_extension.ExtendedKeyUsagePresenceValidator(),
-            smime_extension.KeyUsagePresenceValidator(),
+            smime_extension.CabfSmimeKeyUsagePresenceValidator(),
             cabf_extension.AuthorityInformationAccessPresenceValidator(
                 validation.ValidationFindingSeverity.WARNING
             ),
             cabf_extension.CrlDistributionPointPresenceValidator(),
             smime_extension.SubjectAlternativeNamePresenceValidator(),
             smime_extension.AllowedExtendedKeyUsageValidator(generation),
             smime_extension.AllowedKeyUsageValidator(generation),
```

### Comparing `pkilint-0.8.2/pkilint/cabf/smime/smime_constants.py` & `pkilint-0.8.3/pkilint/cabf/smime/smime_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/smime/smime_extension.py` & `pkilint-0.8.3/pkilint/cabf/smime/smime_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         super().__init__(
             extension_oid=rfc5280.id_ce_extKeyUsage,
             validation=self.VALIDATION_EKU_EXTENSION_ABSENT,
             pdu_class=rfc5280.Extensions
         )
 
 
-class KeyUsagePresenceValidator(extension.ExtensionPresenceValidator):
+class CabfSmimeKeyUsagePresenceValidator(extension.ExtensionPresenceValidator):
     VALIDATION_KU_EXTENSION_ABSENT = validation.ValidationFinding(
         validation.ValidationFindingSeverity.ERROR,
         'cabf.smime.key_usage_extension_missing'
     )
 
     def __init__(self):
         super().__init__(
```

### Comparing `pkilint-0.8.2/pkilint/cabf/smime/smime_key.py` & `pkilint-0.8.3/pkilint/cabf/smime/smime_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/cabf/smime/smime_name.py` & `pkilint-0.8.3/pkilint/cabf/smime/smime_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/document.py` & `pkilint-0.8.3/pkilint/document.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/etsi/__init__.py` & `pkilint-0.8.3/pkilint/etsi/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/etsi/asn1/en_319_412_5.py` & `pkilint-0.8.3/pkilint/etsi/asn1/en_319_412_5.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/etsi/asn1/ts_119_495.py` & `pkilint-0.8.3/pkilint/etsi/asn1/ts_119_495.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/iso/lei.py` & `pkilint-0.8.3/pkilint/iso/lei.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/itu/bitstring.py` & `pkilint-0.8.3/pkilint/itu/bitstring.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import binascii
-
 from pyasn1.codec.der.encoder import encode
 from pyasn1.type.univ import BitString
-from pyasn1_alt_modules import rfc5280
 
 from pkilint import validation
 
 
 class NamedBitStringMinimalEncodingValidator(validation.Validator):
     VALIDATION_BIT_STRING_NOT_MINIMALLY_ENCODED = validation.ValidationFinding(
         validation.ValidationFindingSeverity.ERROR,
@@ -23,15 +20,15 @@
     def validate(self, node):
         # extract values then re-encode
 
         asserted_values = ','.join((k for k in node.pdu.namedValues.keys() if has_named_bit(node, k)))
 
         encoded = encode(node.pdu)
 
-        new_encoded = encode(type(node.pdu)(asserted_values))
+        new_encoded = encode(type(node.pdu)(asserted_values), asn1Spec=node.pdu)
 
         if encoded != new_encoded:
             encoded_hex = encoded.hex()
             new_encoded_hex = new_encoded.hex()
 
             raise validation.ValidationFindingEncountered(
                 self.VALIDATION_BIT_STRING_NOT_MINIMALLY_ENCODED,
```

### Comparing `pkilint-0.8.2/pkilint/itu/string.py` & `pkilint-0.8.3/pkilint/itu/string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/itu/x520_name.py` & `pkilint-0.8.3/pkilint/itu/x520_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/loader.py` & `pkilint-0.8.3/pkilint/loader.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/msft/msft_name.py` & `pkilint-0.8.3/pkilint/msft/msft_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/__init__.py` & `pkilint-0.8.3/pkilint/pkix/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/algorithm.py` & `pkilint-0.8.3/pkilint/pkix/algorithm.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/certificate/__init__.py` & `pkilint-0.8.3/pkilint/pkix/certificate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import functools
 import logging
+from typing import Optional
 
 from cryptography import x509, exceptions
 from cryptography.hazmat.primitives.asymmetric import (
     padding, rsa, dsa, ec, ed25519, ed448
 )
 from pyasn1.codec.der.encoder import encode
 from pyasn1_alt_modules import rfc5280, rfc3739
 
-from pkilint import validation, pkix
+from pkilint import validation, pkix, document
 from pkilint.document import Document, ValueDecoder
 from pkilint.itu.bitstring import NamedBitStringMinimalEncodingValidator
 from pkilint.itu.string import PrintableStringConstraintValidator
 from pkilint.pkix import (extension, time, name,
                           create_name_validator_container, general_name, algorithm
                           )
 from pkilint.pkix.certificate import (
@@ -40,23 +41,26 @@
     @property
     def not_after(self):
         return time.parse_time_node(
             self.root.navigate('tbsCertificate.validity.notAfter')
         )
 
     @property
-    def is_ca(self):
+    def is_ca(self) -> Optional[bool]:
         ext_and_idx = self.get_extension_by_oid(rfc5280.id_ce_basicConstraints)
 
         if ext_and_idx is None:
             return False
 
         ext, _ = ext_and_idx
 
-        return bool(ext.navigate('extnValue.basicConstraints.cA').pdu)
+        try:
+            return bool(ext.navigate('extnValue.basicConstraints.cA').pdu)
+        except document.PDUNavigationFailedError:
+            return None
 
     @functools.cached_property
     def cryptography_object(self):
         return x509.load_der_x509_certificate(self.substrate)
 
     @functools.cached_property
     def is_self_issued(self):
@@ -294,15 +298,15 @@
                        certificate_extension.NameConstraintsValidator(),
                        certificate_extension.NameConstraintsGeneralSubtreeValidator(),
                        certificate_extension.AuthorityInformationAccessCriticalityValidator(),
                        certificate_extension.SubjectInformationAccessCriticalityValidator(),
                        certificate_extension.SubjectAlternativeNameCriticalityValidator(),
                        certificate_extension.SubjectDirectoryAttributesCriticalityValidator(),
                        certificate_extension.SmimeCapabilitiesCriticalityValidator(),
-                       extension.CrlDistributionPointExtensionEmptyValidator(),
+                       extension.DistributionPointValidator(),
                    ] + additional_validators,
         path='certificate.tbsCertificate.extensions'
     )
 
 
 def create_pkix_certificate_validator_container(
         decoding_validators, validators):
```

### Comparing `pkilint-0.8.2/pkilint/pkix/certificate/certificate_extension.py` & `pkilint-0.8.3/pkilint/pkix/certificate/certificate_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import NamedTuple, Set
 
 from pyasn1.type.univ import ObjectIdentifier
 from pyasn1_alt_modules import rfc5280, rfc4262
 
 from pkilint import validation
 from pkilint.itu.bitstring import has_named_bit
+from pkilint.pkix import extension
 from pkilint.pkix.extension import (get_criticality_from_decoded_node,
                                     ExtensionCriticalityValidator
                                     )
 
 CERTIFICATE_POLICY_QUALIFIER_MAPPINGS = {
     rfc5280.id_qt_cps: rfc5280.CPSuri(),
     rfc5280.id_qt_unotice: rfc5280.UserNotice(),
@@ -533,49 +534,28 @@
                         None
                     )
                 )
 
         return validation.ValidationResult(self, node, results)
 
 
-class KeyUsagePresenceValidator(validation.Validator):
+class KeyUsagePresenceValidator(extension.ExtensionPresenceValidator):
     VALIDATION_CA_NO_KU_EXTENSION = validation.ValidationFinding(
         validation.ValidationFindingSeverity.ERROR,
         'pkix.ca_certificate_no_ku_extension'
     )
 
-    VALIDATION_EE_NO_KU_EXTENSION = validation.ValidationFinding(
-        validation.ValidationFindingSeverity.WARNING,
-        'pkix.ee_certificate_no_ku_extension'
-    )
-
     def __init__(self):
         super().__init__(
-            pdu_class=rfc5280.KeyUsage,
-            validations=[
-                self.VALIDATION_CA_NO_KU_EXTENSION,
-                self.VALIDATION_EE_NO_KU_EXTENSION
-            ]
+            extension_oid=rfc5280.id_ce_keyUsage,
+            validation=self.VALIDATION_CA_NO_KU_EXTENSION,
+            pdu_class=rfc5280.Extensions,
+            predicate=lambda n: n.document.is_ca
         )
 
-    def validate(self, node):
-        is_ca = node.document.is_ca
-
-        ku_ext = node.document.get_extension_by_oid(rfc5280.id_ce_keyUsage)
-
-        if ku_ext is None:
-            if is_ca:
-                raise validation.ValidationFindingEncountered(
-                    self.VALIDATION_CA_NO_KU_EXTENSION
-                )
-            else:
-                raise validation.ValidationFindingEncountered(
-                    self.VALIDATION_EE_NO_KU_EXTENSION
-                )
-
 
 class KeyUsageCriticalityValidator(validation.Validator):
     VALIDATION_KU_NOT_CRITICAL = validation.ValidationFinding(
         validation.ValidationFindingSeverity.WARNING,
         'pkix.key_usage_extension_not_critical'
     )
```

### Comparing `pkilint-0.8.2/pkilint/pkix/certificate/certificate_key.py` & `pkilint-0.8.3/pkilint/pkix/certificate/certificate_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/certificate/certificate_name.py` & `pkilint-0.8.3/pkilint/pkix/certificate/certificate_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/certificate/certificate_validator.py` & `pkilint-0.8.3/pkilint/pkix/certificate/certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/certificate/certificate_validity.py` & `pkilint-0.8.3/pkilint/pkix/certificate/certificate_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/crl/__init__.py` & `pkilint-0.8.3/pkilint/pkix/crl/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/crl/crl_extension.py` & `pkilint-0.8.3/pkilint/pkix/crl/crl_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/crl/crl_validator.py` & `pkilint-0.8.3/pkilint/pkix/crl/crl_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/crl/crl_validity.py` & `pkilint-0.8.3/pkilint/pkix/crl/crl_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/extension.py` & `pkilint-0.8.3/pkilint/pkix/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,19 +233,19 @@
                     self.VALIDATION_AKI_NO_CERT_ISSUER, None
                 )
             )
 
         return validation.ValidationResult(self, node, results)
 
 
-class CrlDistributionPointExtensionEmptyValidator(validation.Validator):
-    VALIDATION_CRLDP_EMPTY = validation.ValidationFinding(
+class DistributionPointValidator(validation.Validator):
+    VALIDATION_DP_NO_NAME_OR_ISSUER = validation.ValidationFinding(
         validation.ValidationFindingSeverity.ERROR,
-        'pkix.crldp_distribution_point_empty'
+        'pkix.distribution_point_does_not_contain_name_or_issuer'
     )
 
     def __init__(self):
-        super().__init__(validations=[self.VALIDATION_CRLDP_EMPTY], pdu_class=rfc5280.DistributionPoint)
+        super().__init__(validations=[self.VALIDATION_DP_NO_NAME_OR_ISSUER], pdu_class=rfc5280.DistributionPoint)
 
     def validate(self, node):
-        if len(node.children) == 0:
-            raise validation.ValidationFindingEncountered(self.VALIDATION_CRLDP_EMPTY)
+        if 'distributionPoint' not in node.children and 'cRLIssuer' not in node.children:
+            raise validation.ValidationFindingEncountered(self.VALIDATION_DP_NO_NAME_OR_ISSUER)
```

### Comparing `pkilint-0.8.2/pkilint/pkix/general_name.py` & `pkilint-0.8.3/pkilint/pkix/general_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/name.py` & `pkilint-0.8.3/pkilint/pkix/name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/ocsp/__init__.py` & `pkilint-0.8.3/pkilint/pkix/ocsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_basic_response.py` & `pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_basic_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_response.py` & `pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/ocsp/ocsp_validity.py` & `pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/pkix/time.py` & `pkilint-0.8.3/pkilint/pkix/time.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/report.py` & `pkilint-0.8.3/pkilint/report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/util.py` & `pkilint-0.8.3/pkilint/util.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint/validation.py` & `pkilint-0.8.3/pkilint/validation.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/pkilint.egg-info/PKG-INFO` & `pkilint-0.8.3/pkilint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.2
+Version: 0.8.3
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.8.2/pkilint.egg-info/SOURCES.txt` & `pkilint-0.8.3/pkilint.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -79,10 +79,11 @@
 pkilint/pkix/ocsp/ocsp_basic_response.py
 pkilint/pkix/ocsp/ocsp_response.py
 pkilint/pkix/ocsp/ocsp_validity.py
 tests/__init__.py
 tests/util.py
 tests/integration_certificate/__init__.py
 tests/integration_certificate/test_cabf_smime_cert.py
+tests/integration_certificate/test_pkix_cert.py
 tests/itu/__init__.py
 tests/itu/test_bitstring.py
 tests/itu/test_string.py
```

### Comparing `pkilint-0.8.2/setup.cfg` & `pkilint-0.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/tests/integration_certificate/__init__.py` & `pkilint-0.8.3/tests/integration_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/tests/integration_certificate/test_cabf_smime_cert.py` & `pkilint-0.8.3/tests/integration_certificate/test_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/tests/itu/test_bitstring.py` & `pkilint-0.8.3/tests/itu/test_bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/tests/itu/test_string.py` & `pkilint-0.8.3/tests/itu/test_string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.2/tests/util.py` & `pkilint-0.8.3/tests/util.py`

 * *Files identical despite different names*

