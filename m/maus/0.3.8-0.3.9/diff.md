# Comparing `tmp/maus-0.3.8.tar.gz` & `tmp/maus-0.3.9.tar.gz`

## Comparing `maus-0.3.8.tar` & `maus-0.3.9.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 maus-0.3.8/.gitattributes
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 maus-0.3.8/.gitmodules
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 maus-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 maus-0.3.8/.readthedocs.yaml
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 maus-0.3.8/README.rst
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 maus-0.3.8/requirements.in
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 maus-0.3.8/requirements.txt
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 maus-0.3.8/tox.ini
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 maus-0.3.8/.github/dependabot.yml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 maus-0.3.8/.github/release-drafter.yml
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/docs.yml
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/integrationtests.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/release.yml
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 maus-0.3.8/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-build_executable.in
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-build_executable.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-docs.in
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-docs.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-integration_tests.in
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-integration_tests.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-json_schemas.in
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-test_packaging.in
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-test_packaging.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-unit_tests.in
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 maus-0.3.8/dev_requirements/requirements-unit_tests.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 maus-0.3.8/docs/Makefile
--rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 maus-0.3.8/docs/conf.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 maus-0.3.8/docs/index.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 maus-0.3.8/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.3.8/docs/_static/.gitkeep
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 maus-0.3.8/docs/_static/maus-favicon.png
--rw-r--r--   0        0        0    24553 2020-02-02 00:00:00.000000 maus-0.3.8/docs/_static/maus-logo.png
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 maus-0.3.8/docs/_static/maus-logo.svg
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 maus-0.3.8/docs/api/maus.models.rst
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 maus-0.3.8/docs/api/maus.reader.rst
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 maus-0.3.8/docs/api/maus.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 maus-0.3.8/docs/api/modules.rst
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 maus-0.3.8/json_schemas/DeepAnwendungshandbuchSchema.json
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 maus-0.3.8/json_schemas/README.md
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 maus-0.3.8/json_schemas/generate_json_schemas.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 maus-0.3.8/src/_maus_version.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/__init__.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/division_helper.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/edifact.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/maus_provider.py
--rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/mig_ahb_matching.py
--rw-r--r--   0        0        0    30525 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/navigation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/py.typed
--rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/transformation.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/models/__init__.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/models/anwendungshandbuch.py
--rw-r--r--   0        0        0    25221 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/models/edifact_components.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/models/message_implementation_guide.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/reader/__init__.py
--rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/reader/ahb_location_xml.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/reader/etree_element_helpers.py
--rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/reader/flat_ahb_reader.py
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/reader/mig_ahb_name_helpers.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/reader/mig_reader.py
--rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 maus-0.3.8/src/maus/reader/mig_xml_reader.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 maus-0.3.8/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 maus-0.3.8/LICENSE
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 maus-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 maus-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 maus-0.3.9/.gitattributes
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 maus-0.3.9/.gitmodules
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 maus-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 maus-0.3.9/.readthedocs.yaml
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 maus-0.3.9/README.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 maus-0.3.9/requirements.in
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 maus-0.3.9/requirements.txt
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 maus-0.3.9/tox.ini
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 maus-0.3.9/.github/dependabot.yml
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 maus-0.3.9/.github/release-drafter.yml
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/integrationtests.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/release.yml
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 maus-0.3.9/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-build_executable.in
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-build_executable.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-docs.in
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-docs.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-integration_tests.in
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-integration_tests.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-json_schemas.in
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-unit_tests.in
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 maus-0.3.9/dev_requirements/requirements-unit_tests.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 maus-0.3.9/docs/Makefile
+-rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 maus-0.3.9/docs/conf.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 maus-0.3.9/docs/index.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 maus-0.3.9/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.3.9/docs/_static/.gitkeep
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 maus-0.3.9/docs/_static/maus-favicon.png
+-rw-r--r--   0        0        0    24553 2020-02-02 00:00:00.000000 maus-0.3.9/docs/_static/maus-logo.png
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 maus-0.3.9/docs/_static/maus-logo.svg
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 maus-0.3.9/docs/api/maus.models.rst
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 maus-0.3.9/docs/api/maus.reader.rst
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 maus-0.3.9/docs/api/maus.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 maus-0.3.9/docs/api/modules.rst
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 maus-0.3.9/json_schemas/DeepAnwendungshandbuchSchema.json
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 maus-0.3.9/json_schemas/README.md
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 maus-0.3.9/json_schemas/generate_json_schemas.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 maus-0.3.9/src/_maus_version.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/division_helper.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/edifact.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/maus_provider.py
+-rw-r--r--   0        0        0    12088 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/mig_ahb_matching.py
+-rw-r--r--   0        0        0    30525 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/navigation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/py.typed
+-rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/transformation.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/models/__init__.py
+-rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/models/anwendungshandbuch.py
+-rw-r--r--   0        0        0    25221 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/models/edifact_components.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/models/message_implementation_guide.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/__init__.py
+-rw-r--r--   0        0        0     4921 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/ahb_location_xml.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/etree_element_helpers.py
+-rw-r--r--   0        0        0    13743 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/flat_ahb_reader.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/mig_ahb_name_helpers.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/mig_reader.py
+-rw-r--r--   0        0        0    11111 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/mig_xml_reader.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 maus-0.3.9/src/maus/reader/tree_to_sgh.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 maus-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 maus-0.3.9/LICENSE
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 maus-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 maus-0.3.9/PKG-INFO
```

### Comparing `maus-0.3.8/.pre-commit-config.yaml` & `maus-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.readthedocs.yaml` & `maus-0.3.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/README.rst` & `maus-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/tox.ini` & `maus-0.3.9/tox.ini`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/dependabot.yml` & `maus-0.3.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/codeql-analysis.yml` & `maus-0.3.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/coverage.yml` & `maus-0.3.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/docs.yml` & `maus-0.3.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/formatting.yml` & `maus-0.3.9/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/integrationtests.yml` & `maus-0.3.9/.github/workflows/integrationtests.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/packaging_test.yml` & `maus-0.3.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/pythonlint.yml` & `maus-0.3.9/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/release.yml` & `maus-0.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.github/workflows/unittests.yml` & `maus-0.3.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/dev_requirements/requirements-build_executable.txt` & `maus-0.3.9/dev_requirements/requirements-build_executable.txt`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/dev_requirements/requirements-docs.txt` & `maus-0.3.9/dev_requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/dev_requirements/requirements-test_packaging.txt` & `maus-0.3.9/dev_requirements/requirements-test_packaging.txt`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/dev_requirements/requirements-unit_tests.txt` & `maus-0.3.9/dev_requirements/requirements-unit_tests.txt`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/Makefile` & `maus-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/conf.py` & `maus-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/make.bat` & `maus-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/_static/maus-favicon.png` & `maus-0.3.9/docs/_static/maus-favicon.png`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/_static/maus-logo.png` & `maus-0.3.9/docs/_static/maus-logo.png`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/_static/maus-logo.svg` & `maus-0.3.9/docs/_static/maus-logo.svg`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/api/maus.models.rst` & `maus-0.3.9/docs/api/maus.models.rst`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/api/maus.reader.rst` & `maus-0.3.9/docs/api/maus.reader.rst`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/docs/api/maus.rst` & `maus-0.3.9/docs/api/maus.rst`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/json_schemas/DeepAnwendungshandbuchSchema.json` & `maus-0.3.9/json_schemas/DeepAnwendungshandbuchSchema.json`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/json_schemas/README.md` & `maus-0.3.9/json_schemas/README.md`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/json_schemas/generate_json_schemas.py` & `maus-0.3.9/json_schemas/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/__init__.py` & `maus-0.3.9/src/maus/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,40 @@
 from maus.reader.mig_xml_reader import MigXmlReader
 
 
 # pylint:disable=too-many-arguments
 @click.command()
 @click.version_option()
 @click.option(
-    "-fap", "--flat_ahb_path", type=click.Path(exists=True, path_type=Path), help="Path to the flat ahb json file"
+    "-fap",
+    "--flat_ahb_path",
+    type=click.Path(exists=True, path_type=Path),
+    help="Path to the flat ahb json file",
+    required=True,
+)
+@click.option(
+    "-sghp",
+    "--sgh_path",
+    type=click.Path(exists=True, path_type=Path),
+    help="Path to the sgh json file",
+    required=True,
+)
+@click.option(
+    "-tp",
+    "--template_path",
+    type=click.Path(exists=True, path_type=Path),
+    help="Path to the template file",
+    required=True,
+)
+@click.option(
+    "-cp",
+    "--check_path",
+    type=click.Path(exists=True, path_type=Path),
+    help="Path to the maus json file",
 )
-@click.option("-sghp", "--sgh_path", type=click.Path(exists=True, path_type=Path), help="Path to the sgh json file")
-@click.option("-tp", "--template_path", type=click.Path(exists=True, path_type=Path), help="Path to the template file")
-@click.option("-cp", "--check_path", type=click.Path(exists=True, path_type=Path), help="Path to the maus json file")
 @click.option(
     "-o",
     "--output_path",
     type=click.Path(dir_okay=False, file_okay=True, path_type=Path),
     help="Path to the output file",
 )
 # pylint:disable=no-value-for-parameter
@@ -36,30 +57,38 @@
     flat_ahb_path: Path,
     sgh_path: Path,
     template_path: Path,
     check_path: Path,
     output_path: Path,
 ):
     """
-    The main entry point for the maus command line interface
+    🐭 MAUS CLI is a standalone executable that generates .maus.json files from given input data
     """
 
+    if check_path is None and output_path is None or check_path is not None and output_path is not None:
+        # pylint:disable=line-too-long
+        click.secho(
+            "❌ You need to specify either the `output_path` or the `check_path` parameter. Please use --help to see more information.",
+            fg="red",
+        )
+        raise click.Abort()
+
     with open(flat_ahb_path, "r", encoding="utf-8") as flat_ahb_file:
         flat_ahb = FlatAnwendungshandbuchSchema().load(json.load(flat_ahb_file))
     with open(sgh_path, "r", encoding="utf-8") as sgh_file:
         sgh = SegmentGroupHierarchySchema().loads(sgh_file.read())
 
     mig_reader = MigXmlReader(template_path)
 
     # create new maus.json files
     maus = to_deep_ahb(flat_ahb, sgh, mig_reader)
 
     if output_path is not None and check_path is not None:
         click.secho("❌ You can only specify one of the output_path and maus_to_check_path parameters", fg="red")
-        click.Abort()  # pylint:disable=pointless-exception-statement
+        raise click.Abort()
 
     if output_path is not None:
         maus_dict = DeepAnwendungshandbuchSchema().dump(maus)
 
         with open(output_path, "w", encoding="utf-8") as maus_file:
             json.dump(maus_dict, maus_file, indent=2, ensure_ascii=False, sort_keys=True)
```

### Comparing `maus-0.3.8/src/maus/division_helper.py` & `maus-0.3.9/src/maus/division_helper.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/edifact.py` & `maus-0.3.9/src/maus/edifact.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/maus_provider.py` & `maus-0.3.9/src/maus/maus_provider.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/mig_ahb_matching.py` & `maus-0.3.9/src/maus/mig_ahb_matching.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/navigation.py` & `maus-0.3.9/src/maus/navigation.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/transformation.py` & `maus-0.3.9/src/maus/transformation.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/models/__init__.py` & `maus-0.3.9/src/maus/models/__init__.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/models/anwendungshandbuch.py` & `maus-0.3.9/src/maus/models/anwendungshandbuch.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/models/edifact_components.py` & `maus-0.3.9/src/maus/models/edifact_components.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/models/message_implementation_guide.py` & `maus-0.3.9/src/maus/models/message_implementation_guide.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/reader/ahb_location_xml.py` & `maus-0.3.9/src/maus/reader/ahb_location_xml.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/reader/etree_element_helpers.py` & `maus-0.3.9/src/maus/reader/etree_element_helpers.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/reader/flat_ahb_reader.py` & `maus-0.3.9/src/maus/reader/flat_ahb_reader.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/reader/mig_ahb_name_helpers.py` & `maus-0.3.9/src/maus/reader/mig_ahb_name_helpers.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/reader/mig_reader.py` & `maus-0.3.9/src/maus/reader/mig_reader.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/src/maus/reader/mig_xml_reader.py` & `maus-0.3.9/src/maus/reader/mig_xml_reader.py`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/.gitignore` & `maus-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/LICENSE` & `maus-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maus-0.3.8/pyproject.toml` & `maus-0.3.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,23 @@
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "attrs>=21.4.0",
     "marshmallow>=3.18.0",
     "more_itertools",
     "xmltodict",
-    "click"
+    "click",
+    "lark>=1.1.5"
     # add everything you add in requirements.in here
 ]
 dynamic = ["readme", "version"]
 
 [project.optional-dependencies]
-xml = ["lxml>=4.9.2", "xmltodict"]
+xml = ["lxml>=4.9.2", "xmltodict"] # for parsing the Hochfrequenz MIG templates
+tree = ["lark>=1.1.5"] # for parsing the Hochfrequenz .tree files
 
 [project.urls]
 Changelog = "https://github.com/Hochfrequenz/mig_ahb_utility_stack/releases"
 Homepage = "https://github.com/Hochfrequenz/mig_ahb_utility_stack"
 Documentation = "https://maus.readthedocs.io/en/latest/"
 
 # wird das tool als CLI script verwendet, dann muss hier der Name des Scripts angegeben werden
```

### Comparing `maus-0.3.8/PKG-INFO` & `maus-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maus
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python Library that consolidates Anwendungshandbücher (AHB) and Message Implementation Guides (MIG)
 Project-URL: Changelog, https://github.com/Hochfrequenz/mig_ahb_utility_stack/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/mig_ahb_utility_stack
 Project-URL: Documentation, https://maus.readthedocs.io/en/latest/
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
@@ -16,17 +16,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: attrs>=21.4.0
 Requires-Dist: click
+Requires-Dist: lark>=1.1.5
 Requires-Dist: marshmallow>=3.18.0
 Requires-Dist: more-itertools
 Requires-Dist: xmltodict
+Provides-Extra: tree
+Requires-Dist: lark>=1.1.5; extra == 'tree'
 Provides-Extra: xml
 Requires-Dist: lxml>=4.9.2; extra == 'xml'
 Requires-Dist: xmltodict; extra == 'xml'
 Description-Content-Type: text/x-rst
 
 MIG AHB Utility Stack (MAUS) 🐭
 ===============================
```

