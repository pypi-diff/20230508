# Comparing `tmp/finch_api-0.0.1.tar.gz` & `tmp/finch_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finch_api-0.0.1.tar", max compression
+gzip compressed data, was "finch_api-0.0.2.tar", max compression
```

## Comparing `finch_api-0.0.1.tar` & `finch_api-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,93 @@
--rw-r--r--   0        0        0      162 2022-12-22 21:59:12.339553 finch_api-0.0.1/README.md
--rw-r--r--   0        0        0     1374 2022-12-22 21:59:51.479258 finch_api-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       40 2022-12-22 21:59:12.339746 finch_api-0.0.1/src/finch/__init__.py
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 finch_api-0.0.1/setup.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 finch_api-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-05-08 18:28:19.703315 finch_api-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7347 2023-05-08 18:28:19.703315 finch_api-0.0.2/README.md
+-rw-r--r--   0        0        0     1872 2023-05-08 18:28:19.703315 finch_api-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1834 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/__init__.py
+-rw-r--r--   0        0        0    46017 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_base_exceptions.py
+-rw-r--r--   0        0        0    17885 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_client.py
+-rw-r--r--   0        0        0     1285 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_models.py
+-rw-r--r--   0        0        0     4781 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_qs.py
+-rw-r--r--   0        0        0      872 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_resource.py
+-rw-r--r--   0        0        0     3976 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_types.py
+-rw-r--r--   0        0        0     1277 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_utils/__init__.py
+-rw-r--r--   0        0        0     6701 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_utils/_utils.py
+-rw-r--r--   0        0        0      124 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/_version.py
+-rw-r--r--   0        0        0    10630 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/pagination.py
+-rw-r--r--   0        0        0        0 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/py.typed
+-rw-r--r--   0        0        0      321 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/__init__.py
+-rw-r--r--   0        0        0     4144 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/account.py
+-rw-r--r--   0        0        0      532 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/__init__.py
+-rw-r--r--   0        0        0     5758 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/applications.py
+-rw-r--r--   0        0        0     1409 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/ats.py
+-rw-r--r--   0        0        0     6058 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/candidates.py
+-rw-r--r--   0        0        0     5428 2023-05-08 18:28:19.703315 finch_api-0.0.2/src/finch/resources/ats/jobs.py
+-rw-r--r--   0        0        0     5532 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/ats/offers.py
+-rw-r--r--   0        0        0     2703 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/ats/stages.py
+-rw-r--r--   0        0        0      703 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/__init__.py
+-rw-r--r--   0        0        0      231 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/benefits/__init__.py
+-rw-r--r--   0        0        0    13700 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/benefits/benefits.py
+-rw-r--r--   0        0        0    13797 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/benefits/individuals.py
+-rw-r--r--   0        0        0     2021 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/company.py
+-rw-r--r--   0        0        0     4175 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/directory.py
+-rw-r--r--   0        0        0     1760 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/hris.py
+-rw-r--r--   0        0        0      262 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     4278 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0     4552 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/individuals/individuals.py
+-rw-r--r--   0        0        0     3963 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/pay_statements.py
+-rw-r--r--   0        0        0     4247 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/hris/payments.py
+-rw-r--r--   0        0        0     2256 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/resources/providers.py
+-rw-r--r--   0        0        0      416 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/__init__.py
+-rw-r--r--   0        0        0      572 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/application.py
+-rw-r--r--   0        0        0      361 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/application_list_params.py
+-rw-r--r--   0        0        0      726 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/candidate.py
+-rw-r--r--   0        0        0      355 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/candidate_list_params.py
+-rw-r--r--   0        0        0      889 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/job.py
+-rw-r--r--   0        0        0      337 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/job_list_params.py
+-rw-r--r--   0        0        0      474 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/offer.py
+-rw-r--r--   0        0        0      343 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/offer_list_params.py
+-rw-r--r--   0        0        0      362 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/ats/stage.py
+-rw-r--r--   0        0        0      266 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/disconnect_response.py
+-rw-r--r--   0        0        0     1761 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/__init__.py
+-rw-r--r--   0        0        0      902 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_create_params.py
+-rw-r--r--   0        0        0      220 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_frequency.py
+-rw-r--r--   0        0        0      598 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_type.py
+-rw-r--r--   0        0        0      278 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefit_update_params.py
+-rw-r--r--   0        0        0      784 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/enrolled_individual.py
+-rw-r--r--   0        0        0      969 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_benefit.py
+-rw-r--r--   0        0        0      424 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_enroll_many_params.py
+-rw-r--r--   0        0        0      259 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
+-rw-r--r--   0        0        0      398 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
+-rw-r--r--   0        0        0      329 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/individual_unenroll_params.py
+-rw-r--r--   0        0        0      647 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benefits/unenrolled_individual.py
+-rw-r--r--   0        0        0      415 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/benfit_contribution.py
+-rw-r--r--   0        0        0     2209 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/company.py
+-rw-r--r--   0        0        0      596 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/company_benefit.py
+-rw-r--r--   0        0        0      202 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/create_company_benefits_response.py
+-rw-r--r--   0        0        0      376 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/directory_list_individuals_params.py
+-rw-r--r--   0        0        0     1361 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual.py
+-rw-r--r--   0        0        0     1025 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual_in_directory.py
+-rw-r--r--   0        0        0      327 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual_response.py
+-rw-r--r--   0        0        0      480 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individual_retrieve_many_params.py
+-rw-r--r--   0        0        0      367 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     2985 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0      363 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/employment_data_response.py
+-rw-r--r--   0        0        0      703 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py
+-rw-r--r--   0        0        0     3320 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement.py
+-rw-r--r--   0        0        0      376 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement_response.py
+-rw-r--r--   0        0        0      438 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement_response_body.py
+-rw-r--r--   0        0        0      616 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/pay_statement_retrieve_many_params.py
+-rw-r--r--   0        0        0      791 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/payment.py
+-rw-r--r--   0        0        0      709 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/payment_list_params.py
+-rw-r--r--   0        0        0     1411 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/supported_benefit.py
+-rw-r--r--   0        0        0      200 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/hris/update_company_benefit_response.py
+-rw-r--r--   0        0        0      724 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/income.py
+-rw-r--r--   0        0        0      881 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/introspection.py
+-rw-r--r--   0        0        0      631 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/location.py
+-rw-r--r--   0        0        0      262 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/money.py
+-rw-r--r--   0        0        0      369 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/paging.py
+-rw-r--r--   0        0        0      959 2023-05-08 18:28:19.707315 finch_api-0.0.2/src/finch/types/provider.py
+-rw-r--r--   0        0        0     8245 1970-01-01 00:00:00.000000 finch_api-0.0.2/PKG-INFO
```

