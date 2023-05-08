# Comparing `tmp/gene-normalizer-0.2.8.tar.gz` & `tmp/gene-normalizer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene-normalizer-0.2.8.tar", last modified: Tue Feb  7 13:16:13 2023, max compression
+gzip compressed data, was "gene-normalizer-0.2.9.tar", last modified: Tue Apr 18 17:39:50 2023, max compression
```

## Comparing `gene-normalizer-0.2.8.tar` & `gene-normalizer-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:16:13.030080 gene-normalizer-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-02-07 13:16:13.030080 gene-normalizer-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:16:13.030080 gene-normalizer-0.2.8/gene/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:16:13.030080 gene-normalizer-0.2.8/gene/etl/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/ensembl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/hgnc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:16:13.030080 gene-normalizer-0.2.8/gene/etl/vrs_locations/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/vrs_locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/vrs_locations/chromosome_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/etl/vrs_locations/sequence_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    28765 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    31404 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/gene/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 13:16:13.030080 gene-normalizer-0.2.8/gene_normalizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-02-07 13:16:12.000000 gene-normalizer-0.2.8/gene_normalizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-02-07 13:16:12.000000 gene-normalizer-0.2.8/gene_normalizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 13:16:12.000000 gene-normalizer-0.2.8/gene_normalizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 13:16:12.000000 gene-normalizer-0.2.8/gene_normalizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-07 13:16:12.000000 gene-normalizer-0.2.8/gene_normalizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 13:16:12.000000 gene-normalizer-0.2.8/gene_normalizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-02-07 13:16:13.030080 gene-normalizer-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-07 13:16:02.000000 gene-normalizer-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.966632 gene-normalizer-0.2.9/gene/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/gene/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20417 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/gene/database/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/postgresql/add_fkeys.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/postgresql/add_indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/postgresql/create_record_lookup_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/postgresql/create_tables_query.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/postgresql/drop_fkeys.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/postgresql/drop_indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/database/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/gene/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/ensembl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/hgnc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/ncbi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/gene/etl/vrs_locations/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/vrs_locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/vrs_locations/chromosome_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/etl/vrs_locations/sequence_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31395 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/gene/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/gene_normalizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-18 17:39:50.000000 gene-normalizer-0.2.9/gene_normalizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-18 17:39:50.000000 gene-normalizer-0.2.9/gene_normalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:39:50.000000 gene-normalizer-0.2.9/gene_normalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 17:39:50.000000 gene-normalizer-0.2.9/gene_normalizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:39:50.000000 gene-normalizer-0.2.9/gene_normalizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 17:39:50.000000 gene-normalizer-0.2.9/gene_normalizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 17:39:50.000000 gene-normalizer-0.2.9/gene_normalizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-18 17:39:50.970632 gene-normalizer-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-18 17:39:44.000000 gene-normalizer-0.2.9/setup.py
```

### Comparing `gene-normalizer-0.2.8/LICENSE` & `gene-normalizer-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.2.8/PKG-INFO` & `gene-normalizer-0.2.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gene-normalizer
-Version: 0.2.8
+Version: 0.2.9
 Summary: VICC normalization routine for genes
 Home-page: https://github.com/cancervariants/gene-normalization
 Author: VICC
 Author-email: help@cancervariants.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -17,40 +17,28 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
 
-# Gene Normalization
+# Gene Normalizer
 Services and guidelines for normalizing gene terms
 
-Installing with pip:
+## Installation
+
+The Normalizer is available via PyPI:
 
 ```commandline
 pip install gene[dev]
 ```
 
 The `[dev]` argument tells pip to install packages to fulfill the dependencies of the `gene.etl` package.
 
-## Developer instructions
-Following are sections include instructions specifically for developers.
-
-### Installation
-For a development install, we recommend using Pipenv. See the
-[pipenv docs](https://pipenv-fork.readthedocs.io/en/latest/#install-pipenv-today)
-for direction on installing pipenv in your compute environment.
-
-Once installed, from the project root dir, just run:
-
-```commandline
-pipenv shell
-pipenv lock && pipenv sync
-pipenv install --dev
-```
+### External requirements
 
 Gene Normalization relies on [SeqRepo](https://github.com/biocommons/biocommons.seqrepo) data, which you must download yourself.
 
 From the _root_ directory:
 ```
 pip install seqrepo
 sudo mkdir /usr/local/share/seqrepo
@@ -61,109 +49,130 @@
 If you get an error similar to the one below:
 ```
 PermissionError: [Error 13] Permission denied: '/usr/local/share/seqrepo/2021-01-29._fkuefgd' -> '/usr/local/share/seqrepo/2021-01-29'
 ```
 
 You will want to do the following:\
 (*Might not be ._fkuefgd, so replace with your error message path*)
+
 ```console
 sudo mv /usr/local/share/seqrepo/2021-01-29._fkuefgd /usr/local/share/seqrepo/2021-01-29
-exit
 ```
 
-### Deploying DynamoDB Locally
+Use the `SEQREPO_ROOT_DIR` environment variable to set the path of an already existing SeqRepo directory. The default is `/usr/local/share/seqrepo/latest`.
 
-We use Amazon DynamoDB for our database. To deploy locally, follow [these instructions](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html).
+### Database Initialization
 
-### Init coding style tests
+The Normalizer supports two data storage options:
 
-Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
+* [DynamoDB](https://aws.amazon.com/dynamodb), a NoSQL service provided by AWS. This is our preferred storage solution. In addition to cloud deployment, Amazon also provides a tool for local service, which can be installed [here](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html). Once downloaded, you can start service by running `java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb` in a terminal (add a `-port <VALUE>` option to use a different port)
+* [PostgreSQL](https://www.postgresql.org/), a well-known relational database technology. Once starting the Postgres server process, [ensure that a database is created](https://www.postgresql.org/docs/current/sql-createdatabase.html) (we typically name ours `gene_normalizer`).
 
-We use [pre-commit](https://pre-commit.com/#usage) to run conformance tests.
+By default, the Gene Normalizer expects to find a DynamoDB instance listening at `http://localhost:8000`. Alternative locations can be specified in two ways:
 
-This ensures:
+The first way is to set the `--db_url` option to the URL endpoint.
 
-* Check code style
-* Check for added large files
-* Detect AWS Credentials
-* Detect Private Key
+```commandline
+gene_update --update_all --db_url="http://localhost:8001"
+```
 
-Before first commit run:
+The second way is to set the `GENE_NORM_DB_URL` environment variable to the URL endpoint.
+```commandline
+export GENE_NORM_DB_URL="http://localhost:8001"
+```
+
+To use a PostgreSQL instance instead of DynamoDB, provide a PostgreSQL connection URL instead, e.g.
 
 ```commandline
-pre-commit install
+export GENE_NORM_DB_URL="postgresql://postgres@localhost:5432/gene_normalizer"
 ```
 
+### Adding and refreshing data
 
-### Running unit tests
+Use the `gene_update` command in a shell to update the database.
 
-By default, tests will employ an existing DynamoDB database. For test environments where this is unavailable (e.g. in CI), the `GENE_TEST` environment variable can be set to initialize a local DynamoDB instance with miniature versions of input data files before tests are executed.
+#### Update source(s)
+
+The normalizer currently pulls data from [HGNC](https://www.genenames.org/), [Ensembl](https://useast.ensembl.org/index.html), and [NCBI](https://www.ncbi.nlm.nih.gov/gene/).
+
+To update one source, simply set `--normalizer` to the source you wish to update. The normalizer will check to see if local source data is up-to-date, acquire the most recent data if not, and use it to populate the database.
+
+For example, run the following to acquire the latest HGNC data if necessary, and update the HGNC gene records in the normalizer database:
 
 ```commandline
-export GENE_TEST=true
+gene_update --normalizer="hgnc"
 ```
 
-Running unit tests is as easy as pytest.
+To update multiple sources, you can use the `--normalizer` option with the source names separated by spaces.
+
+#### Update all sources
+
+To update all sources, use the `--update_all` flag:
 
 ```commandline
-pipenv run pytest
+gene_update --update_all
 ```
 
-### Updating the gene normalization database
+### Starting the gene normalization service
 
-Before you use the CLI to update the database, run the following in a separate terminal to start a local DynamoDB service on `port 8000`:
+Once the Gene Normalizer database has been loaded, from the project root, run the following:
 
-```
-java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
+```commandline
+uvicorn gene.main:app --reload
 ```
 
-To change the port, simply add `-port value`.
+Next, view the OpenAPI docs on your local machine:
 
-#### Update source(s)
-The sources we currently use are: HGNC, Ensembl, and NCBI.
+http://127.0.0.1:8000/gene
+
+## Developer instructions
+The following sections include instructions specifically for developers.
 
-To update one source, simply set `--normalizer` to the source you wish to update.
+### Installation
+For a development install, we recommend using Pipenv. See the
+[pipenv docs](https://pipenv-fork.readthedocs.io/en/latest/#install-pipenv-today)
+for direction on installing pipenv in your compute environment.
 
-From the project root, run the following to update the HGNC source:
+Once installed, clone the repo and initialize the environment:
 
 ```commandline
-python3 -m gene.cli --normalizer="hgnc"
+git clone https://github.com/cancervariants/gene-normalization
+cd gene-normalization
+pipenv shell
+pipenv update
+pipenv install --dev
 ```
 
-To update multiple sources, you can use the `--normalizer` flag with the source names separated by spaces.
+### Init coding style tests
 
-#### Update all sources
+Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
 
-To update all sources, use the `--update_all` flag.
+We use [pre-commit](https://pre-commit.com/#usage) to run conformance tests.
 
-From the project root, run the following to update all sources:
+This ensures:
 
-```commandline
-python3 -m gene.cli --update_all
-```
+* Check code style
+* Check for added large files
+* Detect AWS Credentials
+* Detect Private Key
 
-#### Specifying the database URL endpoint
-The default URL endpoint is `http://localhost:8000`.
-There are two different ways to specify the database URL endpoint.
+Before first commit run:
 
-The first way is to set the `--db_url` flag to the URL endpoint.
 ```commandline
-python3 -m gene.cli --update_all --db_url="http://localhost:8001"
+pre-commit install
 ```
 
-The second way is to set the `GENE_NORM_DB_URL` to the URL endpoint.
-```commandline
-export GENE_NORM_DB_URL="http://localhost:8001"
-python3 -m gene.cli --update_all
-```
+### Running unit tests
+
+By default, tests will employ an existing database. For test environments where this is unavailable (e.g. in CI), the `GENE_TEST` environment variable can be set to initialize a local DynamoDB instance with miniature versions of input data files before tests are executed.
 
-### Starting the gene normalization service
-From the project root, run the following:
 ```commandline
- uvicorn gene.main:app --reload
+export GENE_TEST=true
 ```
 
-Next, view the OpenAPI docs on your local machine:
+Running unit tests is as easy as pytest.
 
-http://127.0.0.1:8000/gene
+```commandline
+pipenv run pytest
+```
```

### Comparing `gene-normalizer-0.2.8/README.md` & `gene-normalizer-0.2.9/gene_normalizer.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,44 @@
+Metadata-Version: 2.1
+Name: gene-normalizer
+Version: 0.2.9
+Summary: VICC normalization routine for genes
+Home-page: https://github.com/cancervariants/gene-normalization
+Author: VICC
+Author-email: help@cancervariants.org
+License: MIT
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
 
-# Gene Normalization
+# Gene Normalizer
 Services and guidelines for normalizing gene terms
 
-Installing with pip:
+## Installation
+
+The Normalizer is available via PyPI:
 
 ```commandline
 pip install gene[dev]
 ```
 
 The `[dev]` argument tells pip to install packages to fulfill the dependencies of the `gene.etl` package.
 
-## Developer instructions
-Following are sections include instructions specifically for developers.
-
-### Installation
-For a development install, we recommend using Pipenv. See the
-[pipenv docs](https://pipenv-fork.readthedocs.io/en/latest/#install-pipenv-today)
-for direction on installing pipenv in your compute environment.
-
-Once installed, from the project root dir, just run:
-
-```commandline
-pipenv shell
-pipenv lock && pipenv sync
-pipenv install --dev
-```
+### External requirements
 
 Gene Normalization relies on [SeqRepo](https://github.com/biocommons/biocommons.seqrepo) data, which you must download yourself.
 
 From the _root_ directory:
 ```
 pip install seqrepo
 sudo mkdir /usr/local/share/seqrepo
@@ -40,107 +49,130 @@
 If you get an error similar to the one below:
 ```
 PermissionError: [Error 13] Permission denied: '/usr/local/share/seqrepo/2021-01-29._fkuefgd' -> '/usr/local/share/seqrepo/2021-01-29'
 ```
 
 You will want to do the following:\
 (*Might not be ._fkuefgd, so replace with your error message path*)
+
 ```console
 sudo mv /usr/local/share/seqrepo/2021-01-29._fkuefgd /usr/local/share/seqrepo/2021-01-29
-exit
 ```
 
-### Deploying DynamoDB Locally
+Use the `SEQREPO_ROOT_DIR` environment variable to set the path of an already existing SeqRepo directory. The default is `/usr/local/share/seqrepo/latest`.
 
-We use Amazon DynamoDB for our database. To deploy locally, follow [these instructions](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html).
+### Database Initialization
 
-### Init coding style tests
+The Normalizer supports two data storage options:
 
-Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
+* [DynamoDB](https://aws.amazon.com/dynamodb), a NoSQL service provided by AWS. This is our preferred storage solution. In addition to cloud deployment, Amazon also provides a tool for local service, which can be installed [here](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html). Once downloaded, you can start service by running `java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb` in a terminal (add a `-port <VALUE>` option to use a different port)
+* [PostgreSQL](https://www.postgresql.org/), a well-known relational database technology. Once starting the Postgres server process, [ensure that a database is created](https://www.postgresql.org/docs/current/sql-createdatabase.html) (we typically name ours `gene_normalizer`).
 
-We use [pre-commit](https://pre-commit.com/#usage) to run conformance tests.
+By default, the Gene Normalizer expects to find a DynamoDB instance listening at `http://localhost:8000`. Alternative locations can be specified in two ways:
 
-This ensures:
+The first way is to set the `--db_url` option to the URL endpoint.
 
-* Check code style
-* Check for added large files
-* Detect AWS Credentials
-* Detect Private Key
+```commandline
+gene_update --update_all --db_url="http://localhost:8001"
+```
 
-Before first commit run:
+The second way is to set the `GENE_NORM_DB_URL` environment variable to the URL endpoint.
+```commandline
+export GENE_NORM_DB_URL="http://localhost:8001"
+```
+
+To use a PostgreSQL instance instead of DynamoDB, provide a PostgreSQL connection URL instead, e.g.
 
 ```commandline
-pre-commit install
+export GENE_NORM_DB_URL="postgresql://postgres@localhost:5432/gene_normalizer"
 ```
 
+### Adding and refreshing data
 
-### Running unit tests
+Use the `gene_update` command in a shell to update the database.
+
+#### Update source(s)
+
+The normalizer currently pulls data from [HGNC](https://www.genenames.org/), [Ensembl](https://useast.ensembl.org/index.html), and [NCBI](https://www.ncbi.nlm.nih.gov/gene/).
 
-By default, tests will employ an existing DynamoDB database. For test environments where this is unavailable (e.g. in CI), the `GENE_TEST` environment variable can be set to initialize a local DynamoDB instance with miniature versions of input data files before tests are executed.
+To update one source, simply set `--normalizer` to the source you wish to update. The normalizer will check to see if local source data is up-to-date, acquire the most recent data if not, and use it to populate the database.
+
+For example, run the following to acquire the latest HGNC data if necessary, and update the HGNC gene records in the normalizer database:
 
 ```commandline
-export GENE_TEST=true
+gene_update --normalizer="hgnc"
 ```
 
-Running unit tests is as easy as pytest.
+To update multiple sources, you can use the `--normalizer` option with the source names separated by spaces.
+
+#### Update all sources
+
+To update all sources, use the `--update_all` flag:
 
 ```commandline
-pipenv run pytest
+gene_update --update_all
 ```
 
-### Updating the gene normalization database
+### Starting the gene normalization service
 
-Before you use the CLI to update the database, run the following in a separate terminal to start a local DynamoDB service on `port 8000`:
+Once the Gene Normalizer database has been loaded, from the project root, run the following:
 
-```
-java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
+```commandline
+uvicorn gene.main:app --reload
 ```
 
-To change the port, simply add `-port value`.
+Next, view the OpenAPI docs on your local machine:
 
-#### Update source(s)
-The sources we currently use are: HGNC, Ensembl, and NCBI.
+http://127.0.0.1:8000/gene
+
+## Developer instructions
+The following sections include instructions specifically for developers.
 
-To update one source, simply set `--normalizer` to the source you wish to update.
+### Installation
+For a development install, we recommend using Pipenv. See the
+[pipenv docs](https://pipenv-fork.readthedocs.io/en/latest/#install-pipenv-today)
+for direction on installing pipenv in your compute environment.
 
-From the project root, run the following to update the HGNC source:
+Once installed, clone the repo and initialize the environment:
 
 ```commandline
-python3 -m gene.cli --normalizer="hgnc"
+git clone https://github.com/cancervariants/gene-normalization
+cd gene-normalization
+pipenv shell
+pipenv update
+pipenv install --dev
 ```
 
-To update multiple sources, you can use the `--normalizer` flag with the source names separated by spaces.
+### Init coding style tests
 
-#### Update all sources
+Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
+
+We use [pre-commit](https://pre-commit.com/#usage) to run conformance tests.
+
+This ensures:
 
-To update all sources, use the `--update_all` flag.
+* Check code style
+* Check for added large files
+* Detect AWS Credentials
+* Detect Private Key
 
-From the project root, run the following to update all sources:
+Before first commit run:
 
 ```commandline
-python3 -m gene.cli --update_all
+pre-commit install
 ```
 
-#### Specifying the database URL endpoint
-The default URL endpoint is `http://localhost:8000`.
-There are two different ways to specify the database URL endpoint.
+### Running unit tests
+
+By default, tests will employ an existing database. For test environments where this is unavailable (e.g. in CI), the `GENE_TEST` environment variable can be set to initialize a local DynamoDB instance with miniature versions of input data files before tests are executed.
 
-The first way is to set the `--db_url` flag to the URL endpoint.
 ```commandline
-python3 -m gene.cli --update_all --db_url="http://localhost:8001"
+export GENE_TEST=true
 ```
 
-The second way is to set the `GENE_NORM_DB_URL` to the URL endpoint.
-```commandline
-export GENE_NORM_DB_URL="http://localhost:8001"
-python3 -m gene.cli --update_all
-```
+Running unit tests is as easy as pytest.
 
-### Starting the gene normalization service
-From the project root, run the following:
 ```commandline
- uvicorn gene.main:app --reload
+pipenv run pytest
 ```
 
-Next, view the OpenAPI docs on your local machine:
 
-http://127.0.0.1:8000/gene
```

### Comparing `gene-normalizer-0.2.8/gene/__init__.py` & `gene-normalizer-0.2.9/gene/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,28 +19,27 @@
 logging.getLogger("botocore").setLevel(logging.INFO)
 logging.getLogger("urllib3").setLevel(logging.INFO)
 logging.getLogger("python_jsonschema_objects").setLevel(logging.INFO)
 logging.getLogger("biocommons.seqrepo.seqaliasdb.seqaliasdb").setLevel(logging.INFO)
 logging.getLogger("biocommons.seqrepo.fastadir.fastadir").setLevel(logging.INFO)
 
 
-SEQREPO_DATA_PATH = environ.get("SEQREPO_DATA_PATH",
-                                "/usr/local/share/seqrepo/latest")
+SEQREPO_ROOT_DIR = environ.get("SEQREPO_ROOT_DIR", "/usr/local/share/seqrepo/latest")
 
 
 class DownloadException(Exception):
     """Exception for failures relating to source file downloads."""
 
     def __init__(self, *args, **kwargs):
         """Initialize exception."""
         super().__init__(*args, **kwargs)
 
 
-from gene.schemas import SourceName, NamespacePrefix, SourceIDAfterNamespace, ItemTypes  # noqa: E402, E501
-ITEM_TYPES = {k.lower(): v.value for k, v in ItemTypes.__members__.items()}
+from gene.schemas import SourceName, NamespacePrefix, SourceIDAfterNamespace, RefType  # noqa: E402, E501
+ITEM_TYPES = {k.lower(): v.value for k, v in RefType.__members__.items()}
 
 # Sources we import directly (HGNC, Ensembl, NCBI)
 SOURCES = {source.value.lower(): source.value
            for source in SourceName.__members__.values()}
 
 # Set of sources we import directly
 XREF_SOURCES = {src.lower() for src in SourceName.__members__}
```

### Comparing `gene-normalizer-0.2.8/gene/cli.py` & `gene-normalizer-0.2.9/gene/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,243 +1,214 @@
 """This module provides a CLI util to make updates to normalizer database."""
+from collections.abc import Collection
 import logging
-from os import environ
+import os
+from pathlib import Path
 from timeit import default_timer as timer
+from typing import List, Optional
 
 import click
-from botocore.exceptions import ClientError
-from boto3.dynamodb.conditions import Key
 
 from gene import SOURCES
-from gene.database import Database, confirm_aws_db_use, SKIP_AWS_DB_ENV_NAME, \
-    VALID_AWS_ENV_NAMES, AWS_ENV_VAR_NAME
+from gene.database import AbstractDatabase, DatabaseReadException, \
+    DatabaseWriteException
+from gene.database import create_db
+from gene.database.database import DatabaseException
 from gene.etl import NCBI, HGNC, Ensembl  # noqa: F401
 from gene.etl.merge import Merge
 from gene.schemas import SourceName
 
 
 logger = logging.getLogger('gene')
 logger.setLevel(logging.DEBUG)
 
 
-class CLI:
-    """Class for updating the normalizer database via Click"""
-
-    @staticmethod
-    @click.command()
-    @click.option(
-        '--normalizer',
-        help="The normalizer(s) you wish to update separated by spaces."
-    )
-    @click.option(
-        '--aws_instance',
-        is_flag=True,
-        help="Using AWS DynamodDB instance."
-    )
-    @click.option(
-        '--db_url',
-        help="URL endpoint for the application database."
-    )
-    @click.option(
-        '--update_all',
-        is_flag=True,
-        help='Update all normalizer sources.'
-    )
-    @click.option(
-        '--update_merged',
-        is_flag=True,
-        help='Update concepts for normalize endpoint from accepted sources.'
-    )
-    def update_normalizer_db(normalizer, aws_instance, db_url, update_all,
-                             update_merged):
-        """Update selected normalizer source(s) in the gene database."""
-        # If SKIP_AWS_CONFIRMATION is accidentally set, we should verify that the
-        # aws instance should actually be used
-        invalid_aws_msg = f"{AWS_ENV_VAR_NAME} must be set to one of {VALID_AWS_ENV_NAMES}"  # noqa: E501
-        aws_env_var_set = False
-        if AWS_ENV_VAR_NAME in environ:
-            aws_env_var_set = True
-            assert environ[AWS_ENV_VAR_NAME] in VALID_AWS_ENV_NAMES, invalid_aws_msg
-            confirm_aws_db_use(environ[AWS_ENV_VAR_NAME].upper())
-
-        if aws_env_var_set or aws_instance:
-            assert AWS_ENV_VAR_NAME in environ, invalid_aws_msg
-            environ[SKIP_AWS_DB_ENV_NAME] = "true"  # this is already checked above
-            db: Database = Database()
-        else:
-            if db_url:
-                endpoint_url = db_url
-            elif 'GENE_NORM_DB_URL' in environ.keys():
-                endpoint_url = environ['GENE_NORM_DB_URL']
-            else:
-                endpoint_url = 'http://localhost:8000'
-            db: Database = Database(db_url=endpoint_url)
-
-        if update_all:
-            normalizers = [src for src in SOURCES]
-            CLI()._update_normalizers(normalizers, db, update_merged)
-        elif not normalizer:
-            if update_merged:
-                CLI()._load_merge(db, [])
-            else:
-                CLI()._help_msg()
+@click.command()
+@click.option("--data_url", help="URL to data dump")
+@click.option("--db_url", help="URL endpoint for the application database.")
+def update_from_remote(data_url: Optional[str], db_url: str) -> None:
+    """Update data from remotely-hosted DB dump. By default, fetches from latest
+    available dump on VICC S3 bucket; specific URLs can be provided instead by
+    command line option or GENE_NORM_REMOTE_DB_URL environment variable.
+
+    \f
+    :param data_url: user-specified location to pull DB dump from
+    :param db_url: URL to normalizer database
+    """  # noqa: D301
+    if not click.confirm("Are you sure you want to overwrite existing data?"):
+        click.get_current_context().exit()
+    if not data_url:
+        data_url = os.environ.get("GENE_NORM_REMOTE_DB_URL")
+    db = create_db(db_url, False)
+    try:
+        db.load_from_remote(data_url)
+    except NotImplementedError:
+        click.echo(f"Error: Fetching remote data dump not supported for {db.__class__.__name__}")  # noqa: E501
+        click.get_current_context().exit(1)
+    except DatabaseException as e:
+        click.echo(f"Encountered exception during update: {str(e)}")
+        click.get_current_context().exit(1)
+
+
+@click.command()
+@click.option(
+    "--output_directory", "-o",
+    help="Output location to write to",
+    type=click.Path(exists=True, path_type=Path)
+)
+@click.option("--db_url", help="URL endpoint for the application database.")
+def dump_database(output_directory: Path, db_url: str):
+    """Dump data from database into file.
+
+    \f
+    :param output_directory: path to existing directory
+    :param db_url: URL to normalizer database
+    """  # noqa: D301
+    if not output_directory:
+        output_directory = Path(".")
+
+    db = create_db(db_url, False)
+    try:
+        db.export_db(output_directory)
+    except NotImplementedError:
+        click.echo(f"Error: Dumping data to file not supported for {db.__class__.__name__}")  # noqa: E501
+        click.get_current_context().exit(1)
+    except DatabaseException as e:
+        click.echo(f"Encountered exception during update: {str(e)}")
+        click.get_current_context().exit(1)
+
+
+def _update_normalizers(
+    normalizers: Collection[SourceName], db: AbstractDatabase, update_merged: bool
+) -> None:
+    """Update selected normalizer sources."""
+    processed_ids = list()
+    for n in normalizers:
+        delete_time = _delete_source(n, db)
+        _load_source(n, db, delete_time, processed_ids)
+
+    if update_merged:
+        _load_merge(db, processed_ids)
+
+
+def _delete_source(n: SourceName, db: AbstractDatabase) -> float:
+    """Delete individual source data."""
+    msg = f"Deleting {n.value}..."
+    click.echo(f"\n{msg}")
+    logger.info(msg)
+    start_delete = timer()
+    db.delete_source(n)
+    end_delete = timer()
+    delete_time = end_delete - start_delete
+    msg = f"Deleted {n.value} in {delete_time:.5f} seconds."
+    click.echo(f"{msg}\n")
+    logger.info(msg)
+    return delete_time
+
+
+def _load_source(
+    n: SourceName, db: AbstractDatabase, delete_time: float, processed_ids: List[str]
+) -> None:
+    """Load individual source data."""
+    msg = f"Loading {n.value}..."
+    click.echo(msg)
+    logger.info(msg)
+    start_load = timer()
+
+    # used to get source class name from string
+    SourceClass = eval(n.value)
+
+    source = SourceClass(database=db)
+    processed_ids += source.perform_etl()
+    end_load = timer()
+    load_time = end_load - start_load
+    msg = f"Loaded {n.value} in {load_time:.5f} seconds."
+    click.echo(msg)
+    logger.info(msg)
+    msg = f"Total time for {n.value}: {(delete_time + load_time):.5f} seconds."
+    click.echo(msg)
+    logger.info(msg)
+
+
+def _delete_normalized_data(database):
+    """Delete normalized concepts"""
+    click.echo("\nDeleting normalized records...")
+    start_delete = timer()
+    try:
+        database.delete_normalized_concepts()
+    except (DatabaseReadException, DatabaseWriteException) as e:
+        click.echo(f"Encountered exception during normalized data deletion: {e}")
+    end_delete = timer()
+    delete_time = end_delete - start_delete
+    click.echo(f"Deleted normalized records in {delete_time:.5f} seconds.")
+
+
+def _load_merge(db, processed_ids):
+    """Load merged concepts"""
+    start = timer()
+    _delete_normalized_data(db)
+    if not processed_ids:
+        processed_ids = db.get_all_concept_ids()
+    merge = Merge(database=db)
+    click.echo("Constructing normalized records...")
+    merge.create_merged_concepts(processed_ids)
+    end = timer()
+    click.echo(f"Merged concept generation completed in "
+               f"{(end - start):.5f} seconds")
+
+
+@click.command()
+@click.option(
+    '--normalizer',
+    help="The normalizer(s) you wish to update separated by spaces."
+)
+@click.option(
+    '--aws_instance',
+    is_flag=True,
+    help="Using AWS DynamodDB instance."
+)
+@click.option(
+    '--db_url',
+    help="URL endpoint for the application database."
+)
+@click.option(
+    '--update_all',
+    is_flag=True,
+    help='Update all normalizer sources.'
+)
+@click.option(
+    '--update_merged',
+    is_flag=True,
+    help='Update concepts for normalize endpoint from accepted sources.'
+)
+def update_normalizer_db(normalizer, aws_instance, db_url, update_all,
+                         update_merged):
+    """Update selected normalizer source(s) in the gene database."""
+    db = create_db(db_url, aws_instance)
+
+    if update_all:
+        _update_normalizers(list(SourceName), db, update_merged)
+    elif not normalizer:
+        if update_merged:
+            _load_merge(db, [])
         else:
-            normalizers = normalizer.lower().split()
+            ctx = click.get_current_context()
+            click.echo("Must either enter 1 or more sources, or use `--update_all` parameter")  # noqa: E501
+            click.echo(ctx.get_help())
+            ctx.exit()
+    else:
+        normalizers = normalizer.lower().split()
+
+        if len(normalizers) == 0:
+            raise Exception("Must enter a normalizer")
 
-            if len(normalizers) == 0:
-                raise Exception("Must enter a normalizer")
+        non_sources = set(normalizers) - set(SOURCES)
 
-            non_sources = set(normalizers) - {src for src in SOURCES}
-
-            if len(non_sources) != 0:
-                raise Exception(f"Not valid source(s): {non_sources}")
-
-            CLI()._update_normalizers(normalizers, db, update_merged)
-
-    @staticmethod
-    def _help_msg():
-        """Display help message."""
-        ctx = click.get_current_context()
-        click.echo("Must either enter 1 or more sources, or use `--update_all` parameter")  # noqa: E501
-        click.echo(ctx.get_help())
-        ctx.exit()
-
-    @staticmethod
-    def _update_normalizers(normalizers, db, update_merged):
-        """Update selected normalizer sources."""
-        processed_ids = list()
-        for n in normalizers:
-            delete_time = CLI()._delete_source(n, db)
-            CLI()._load_source(n, db, delete_time, processed_ids)
-
-        if update_merged:
-            CLI()._load_merge(db, processed_ids)
+        if len(non_sources) != 0:
+            raise Exception(f"Not valid source(s): {non_sources}")
 
-    @staticmethod
-    def _delete_source(n, db):
-        """Delete individual source data."""
-        msg = f"Deleting {n}..."
-        click.echo(f"\n{msg}")
-        logger.info(msg)
-        start_delete = timer()
-        CLI()._delete_data(n, db)
-        end_delete = timer()
-        delete_time = end_delete - start_delete
-        msg = f"Deleted {n} in {delete_time:.5f} seconds."
-        click.echo(f"{msg}\n")
-        logger.info(msg)
-        return delete_time
-
-    @staticmethod
-    def _load_source(n, db, delete_time, processed_ids):
-        """Load individual source data."""
-        msg = f"Loading {n}..."
-        click.echo(msg)
-        logger.info(msg)
-        start_load = timer()
-
-        # used to get source class name from string
-        SOURCES_CLASS = \
-            {s.value.lower(): eval(s.value) for s in SourceName.__members__.values()}
-
-        source = SOURCES_CLASS[n](database=db)
-        processed_ids += source.perform_etl()
-        end_load = timer()
-        load_time = end_load - start_load
-        msg = f"Loaded {n} in {load_time:.5f} seconds."
-        click.echo(msg)
-        logger.info(msg)
-        msg = f"Total time for {n}: {(delete_time + load_time):.5f} seconds."
-        click.echo(msg)
-        logger.info(msg)
-
-    @staticmethod
-    def _load_merge(db, processed_ids):
-        """Load merged concepts"""
-        start = timer()
-        if not processed_ids:
-            CLI()._delete_normalized_data(db)
-            processed_ids = db.get_ids_for_merge()
-        merge = Merge(database=db)
-        click.echo("Constructing normalized records...")
-        merge.create_merged_concepts(processed_ids)
-        end = timer()
-        click.echo(f"Merged concept generation completed in "
-                   f"{(end - start):.5f} seconds")
-
-    @staticmethod
-    def _delete_normalized_data(database):
-        """Delete normalized concepts"""
-        click.echo("\nDeleting normalized records...")
-        start_delete = timer()
-        try:
-            while True:
-                with database.genes.batch_writer(
-                        overwrite_by_pkeys=['label_and_type', 'concept_id']) \
-                        as batch:
-                    response = database.genes.query(
-                        IndexName='item_type_index',
-                        KeyConditionExpression=Key('item_type').eq('merger'),
-                    )
-                    records = response['Items']
-                    if not records:
-                        break
-                    for record in records:
-                        batch.delete_item(Key={
-                            'label_and_type': record['label_and_type'],
-                            'concept_id': record['concept_id']
-                        })
-        except ClientError as e:
-            click.echo(e.response['Error']['Message'])
-        end_delete = timer()
-        delete_time = end_delete - start_delete
-        click.echo(f"Deleted normalized records in {delete_time:.5f} seconds.")
-
-    @staticmethod
-    def _delete_data(source, database):
-        """Delete a source's data from dynamodb table."""
-        # Delete source's metadata
-        try:
-            metadata = database.metadata.query(
-                KeyConditionExpression=Key(
-                    'src_name').eq(SourceName[f"{source.upper()}"].value)
-            )
-            if metadata['Items']:
-                database.metadata.delete_item(
-                    Key={'src_name': metadata['Items'][0]['src_name']},
-                    ConditionExpression="src_name = :src",
-                    ExpressionAttributeValues={
-                        ':src': SourceName[f"{source.upper()}"].value}
-                )
-        except ClientError as e:
-            click.echo(e.response['Error']['Message'])
-
-        # Delete source's data from genes table
-        try:
-            while True:
-                response = database.genes.query(
-                    IndexName='src_index',
-                    KeyConditionExpression=Key('src_name').eq(
-                        SourceName[f"{source.upper()}"].value)
-                )
-
-                records = response['Items']
-                if not records:
-                    break
-
-                with database.genes.batch_writer(
-                        overwrite_by_pkeys=['label_and_type', 'concept_id']) \
-                        as batch:
-
-                    for record in records:
-                        batch.delete_item(
-                            Key={
-                                'label_and_type': record['label_and_type'],
-                                'concept_id': record['concept_id']
-                            }
-                        )
-        except ClientError as e:
-            click.echo(e.response['Error']['Message'])
+        sources_to_update = {SourceName(SOURCES[s]) for s in normalizers}
+        _update_normalizers(sources_to_update, db, update_merged)
 
 
 if __name__ == '__main__':
-    CLI().update_normalizer_db()
+    update_normalizer_db()
```

### Comparing `gene-normalizer-0.2.8/gene/database.py` & `gene-normalizer-0.2.9/gene/database/dynamodb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,44 @@
-"""This module creates the database."""
-from enum import Enum
-import sys
+"""Provide DynamoDB client."""
+import atexit
 import logging
 from os import environ
-from typing import List, Optional, Dict, Any, Set
-
+from pathlib import Path
+import sys
+from typing import Any, Dict, List, Optional, Set, Union
 import boto3
-import click
 from boto3.dynamodb.conditions import Key
 from botocore.exceptions import ClientError
 
-from gene import PREFIX_LOOKUP
-
+import click
+from gene import ITEM_TYPES, PREFIX_LOOKUP
+from gene.database.database import AWS_ENV_VAR_NAME, SKIP_AWS_DB_ENV_NAME, \
+    VALID_AWS_ENV_NAMES, AbstractDatabase, AwsEnvName, DatabaseException, \
+    DatabaseReadException, DatabaseWriteException, confirm_aws_db_use
+from gene.schemas import RefType, SourceMeta, SourceName
 
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 
-# can be set to either `Dev`, `Staging`, or `Prod`
-# ONLY set when wanting to access aws instance
-AWS_ENV_VAR_NAME = "GENE_NORM_ENV"
-
-# Set to "true" if want to skip db confirmation check. Should ONLY be used for
-# deployment needs
-SKIP_AWS_DB_ENV_NAME = "SKIP_AWS_CONFIRMATION"
-
-
-class AwsEnvName(str, Enum):
-    """AWS environment name that is being used"""
-
-    DEVELOPMENT = "Dev"
-    STAGING = "Staging"
-    PRODUCTION = "Prod"
-
-
-VALID_AWS_ENV_NAMES = {v.value for v in AwsEnvName.__members__.values()}
-
-
-def confirm_aws_db_use(env_name: str) -> None:
-    """Check to ensure that AWS instance should actually be used."""
-    if click.confirm(f"Are you sure you want to use the AWS {env_name} database?",
-                     default=False):
-        click.echo(f"***GENE AWS {env_name.upper()} DATABASE IN USE***")
-    else:
-        click.echo("Exiting.")
-        sys.exit()
-
-
-class DatabaseException(Exception):
-    """Create custom class for handling database exceptions"""
-
-    pass
-
 
-class Database:
-    """The database class."""
+class DynamoDbDatabase(AbstractDatabase):
+    """Database class employing DynamoDB."""
 
-    def __init__(self, db_url: str = '', region_name: str = 'us-east-2'):
+    def __init__(self, db_url: Optional[str] = None, **db_args):
         """Initialize Database class.
 
         :param str db_url: URL endpoint for DynamoDB source
-        :param str region_name: default AWS region
+        :Keyword Arguments:
+            * region_name: AWS region (defaults to "us-east-2")
         """
         gene_concepts_table = "gene_concepts"  # default
         gene_metadata_table = "gene_metadata"  # default
+
+        region_name = db_args.get("region_name", "us-east-2")
+
         if AWS_ENV_VAR_NAME in environ:
             if "GENE_TEST" in environ:
                 raise DatabaseException(f"Cannot have both GENE_TEST and {AWS_ENV_VAR_NAME} set.")  # noqa: E501
 
             aws_env = environ[AWS_ENV_VAR_NAME]
             if aws_env not in VALID_AWS_ENV_NAMES:
                 raise DatabaseException(f"{AWS_ENV_VAR_NAME} must be one of {VALID_AWS_ENV_NAMES}")  # noqa: E501
@@ -97,41 +69,46 @@
 
         self.dynamodb = boto3.resource('dynamodb', **boto_params)
         self.dynamodb_client = boto3.client('dynamodb', **boto_params)
 
         # Only create tables for local instance
         envs_do_not_create_tables = {AWS_ENV_VAR_NAME, "GENE_TEST"}
         if not set(envs_do_not_create_tables) & set(environ):
-            self.create_db_tables()
+            self.initialize_db()
 
         self.genes = self.dynamodb.Table(gene_concepts_table)
         self.metadata = self.dynamodb.Table(gene_metadata_table)
         self.batch = self.genes.batch_writer()
-        self.cached_sources = {}
+        self._cached_sources = {}
+        atexit.register(self.close_connection)
 
-    def _get_table_names(self) -> List[str]:
+    def list_tables(self) -> List[str]:
         """Return names of tables in database.
 
         :return: Table names in DynamoDB
         """
         return self.dynamodb_client.list_tables()['TableNames']
 
-    def delete_all_db_tables(self) -> None:
-        """Delete all tables from database."""
-        existing_tables = self._get_table_names()
+    def drop_db(self) -> None:
+        """Delete all tables from database. Requires manual confirmation.
+
+        :raise DatabaseWriteException: if called in a protected setting with
+            confirmation silenced.
+        """
+        try:
+            if not self._check_delete_okay():
+                return
+        except DatabaseWriteException as e:
+            raise e
+
+        existing_tables = self.list_tables()
         for table_name in existing_tables:
             self.dynamodb.Table(table_name).delete()
 
-    def create_db_tables(self) -> None:
-        """Create gene_concepts and gene_metadata tables."""
-        existing_tables = self._get_table_names()
-        self.create_genes_table(existing_tables)
-        self.create_meta_data_table(existing_tables)
-
-    def create_genes_table(self, existing_tables: List[str]):
+    def _create_genes_table(self, existing_tables: List[str]):
         """Create Genes table if non-existent.
 
         :param List[str] existing_tables: table names already in DB
         """
         table_name = 'gene_concepts'
         if table_name not in existing_tables:
             self.dynamodb.create_table(
@@ -201,15 +178,15 @@
                 ],
                 ProvisionedThroughput={
                     'ReadCapacityUnits': 10,
                     'WriteCapacityUnits': 10
                 }
             )
 
-    def create_meta_data_table(self, existing_tables: List[str]):
+    def _create_meta_data_table(self, existing_tables: List[str]) -> None:
         """Create MetaData table if non-existent.
 
         :param List[str] existing_tables: table names already in DB
         """
         table_name = 'gene_metadata'
         if table_name not in existing_tables:
             self.dynamodb.create_table(
@@ -228,24 +205,44 @@
                 ],
                 ProvisionedThroughput={
                     'ReadCapacityUnits': 10,
                     'WriteCapacityUnits': 10
                 }
             )
 
+    def initialize_db(self) -> None:
+        """Create gene_concepts and gene_metadata tables."""
+        existing_tables = self.list_tables()
+        self._create_genes_table(existing_tables)
+        self._create_meta_data_table(existing_tables)
+
+    def get_source_metadata(self, src_name: Union[str, SourceName]) -> Dict:
+        """Get license, versioning, data lookup, etc information for a source.
+
+        :param src_name: name of the source to get data for
+        """
+        if isinstance(src_name, SourceName):
+            src_name = src_name.value
+        if src_name in self._cached_sources:
+            return self._cached_sources[src_name]
+        else:
+            metadata = self.metadata.get_item(Key={"src_name": src_name}).get("Item")
+            self._cached_sources[src_name] = metadata
+            return metadata
+
     def get_record_by_id(self, concept_id: str,
                          case_sensitive: bool = True,
                          merge: bool = False) -> Optional[Dict]:
         """Fetch record corresponding to provided concept ID
         :param str concept_id: concept ID for gene record
-        :param bool case_sensitive: if true, performs exact lookup, which is
-            more efficient. Otherwise, performs filter operation, which
-            doesn't require correct casing.
-        :param bool merge: if true, look for merged record; look for identity
-            record otherwise.
+        :param bool case_sensitive: if true, performs exact lookup, which is more
+        efficient. Otherwise, performs filter operation, which doesn't require correct
+        casing.
+        :param bool merge: if true, look for merged record; look for identity record
+        otherwise.
         :return: complete gene record, if match is found; None otherwise
         """
         try:
             if merge:
                 pk = f'{concept_id.lower()}##merger'
             else:
                 pk = f'{concept_id.lower()}##identity'
@@ -254,44 +251,45 @@
                     'label_and_type': pk,
                     'concept_id': concept_id
                 })
                 return match['Item']
             else:
                 exp = Key('label_and_type').eq(pk)
                 response = self.genes.query(KeyConditionExpression=exp)
-                return response['Items'][0]
+                record = response['Items'][0]
+                del record["label_and_type"]
+                return record
         except ClientError as e:
             logger.error(f"boto3 client error on get_records_by_id for "
                          f"search term {concept_id}: "
                          f"{e.response['Error']['Message']}")
             return None
         except (KeyError, IndexError):  # record doesn't exist
             return None
 
-    def get_records_by_type(self, query: str,
-                            match_type: str) -> List[Dict]:
-        """Retrieve records for given query and match type.
-        :param query: string to match against
-        :param str match_type: type of match to look for. Should be one
-            of {"symbol", "prev_symbol", "alias", "xref", "associated_with"}
-            (use `get_record_by_id` for concept ID lookup)
-        :return: list of matching records. Empty if lookup fails.
+    def get_refs_by_type(self, search_term: str, ref_type: RefType) -> List[str]:
+        """Retrieve concept IDs for records matching the user's query. Other methods
+        are responsible for actually retrieving full records.
+
+        :param search_term: string to match against
+        :param ref_type: type of match to look for.
+        :return: list of associated concept IDs. Empty if lookup fails.
         """
-        pk = f'{query}##{match_type.lower()}'
-        filter_exp = Key('label_and_type').eq(pk)
+        pk = f"{search_term}##{ref_type.value.lower()}"
+        filter_exp = Key("label_and_type").eq(pk)
         try:
             matches = self.genes.query(KeyConditionExpression=filter_exp)
-            return matches.get('Items', None)
+            return [m["concept_id"] for m in matches.get("Items", None)]
         except ClientError as e:
-            logger.error(f"boto3 client error on get_records_by_type for "
-                         f"search term {query}: "
+            logger.error(f"boto3 client error on get_refs_by_type for "
+                         f"search term {search_term}: "
                          f"{e.response['Error']['Message']}")
             return []
 
-    def get_ids_for_merge(self) -> Set[str]:
+    def get_all_concept_ids(self) -> Set[str]:
         """Retrieve concept IDs for use in generating normalized records.
 
         :return: List of concept IDs as strings.
         """
         last_evaluated_key = None
         concept_ids = []
         params = {
@@ -308,75 +306,212 @@
             for record in records:
                 concept_ids.append(record['concept_id'])
             last_evaluated_key = response.get('LastEvaluatedKey')
             if not last_evaluated_key:
                 break
         return set(concept_ids)
 
-    def add_record(self, record: Dict, record_type: str = "identity"):
+    def add_source_metadata(self, src_name: SourceName, metadata: SourceMeta) -> None:
+        """Add new source metadata entry.
+
+        :param src_name: name of source
+        :param data: known source attributes
+        :raise DatabaseWriteException: if write fails
+        """
+        metadata_item = metadata.dict()
+        metadata_item["src_name"] = src_name.value
+        try:
+            self.metadata.put_item(Item=metadata_item)
+        except ClientError as e:
+            raise DatabaseWriteException(e)
+
+    def add_record(self, record: Dict, src_name: SourceName) -> None:
         """Add new record to database.
+
         :param Dict record: record to upload
-        :param str record_type: type of record (either 'identity' or 'merger')
+        :param SourceName src_name: name of source for record
         """
-        id_prefix = record['concept_id'].split(':')[0].lower()
-        record['src_name'] = PREFIX_LOOKUP[id_prefix]
-        label_and_type = f'{record["concept_id"].lower()}##{record_type}'
-        record['label_and_type'] = label_and_type
-        record['item_type'] = record_type
+        concept_id = record["concept_id"]
+        record["src_name"] = src_name.value
+        label_and_type = f"{concept_id.lower()}##identity"
+        record["label_and_type"] = label_and_type
+        record["item_type"] = "identity"
         try:
-            self.genes.put_item(
-                Item=record,
-                ConditionExpression='attribute_not_exists(concept_id) AND attribute_not_exists(label_and_type)'  # noqa: E501
-            )
+            self.batch.put_item(Item=record)
         except ClientError as e:
             logger.error("boto3 client error on add_record for "
-                         f"{record['concept_id']}: "
-                         f"{e.response['Error']['Message']}")
+                         f"{concept_id}: {e.response['Error']['Message']}")
+        for attr_type, item_type in ITEM_TYPES.items():
+            if attr_type in record:
+                value = record.get(attr_type)
+                if not value:
+                    continue
+                if isinstance(value, str):
+                    items = [value.lower()]
+                else:
+                    items = {item.lower() for item in value}
+                for item in items:
+                    self._add_ref_record(
+                        item, record["concept_id"], item_type, src_name
+                    )
+
+    def add_merged_record(self, record: Dict) -> None:
+        """Add merged record to database.
+
+        :param record: merged record to add
+        """
+        concept_id = record["concept_id"]
+        id_prefix = concept_id.split(":")[0].lower()
+        record["src_name"] = PREFIX_LOOKUP[id_prefix]
+        label_and_type = f"{concept_id.lower()}##merger"
+        record["label_and_type"] = label_and_type
+        record["item_type"] = "merger"
+        try:
+            self.batch.put_item(Item=record)
+        except ClientError as e:
+            logger.error("boto3 client error on add_record for "
+                         f"{concept_id}: {e.response['Error']['Message']}")
 
-    def add_ref_record(self, term: str, concept_id: str, ref_type: str):
+    def _add_ref_record(self, term: str, concept_id: str, ref_type: str,
+                        src_name: SourceName) -> None:
         """Add auxiliary/reference record to database.
+
         :param str term: referent term
         :param str concept_id: concept ID to refer to
         :param str ref_type: one of {'alias', 'label', 'xref',
             'associated_with'}
+        :param src_name: name of source for record
         """
-        label_and_type = f'{term.lower()}##{ref_type}'
-        src_name = PREFIX_LOOKUP[concept_id.split(':')[0].lower()]
+        label_and_type = f"{term.lower()}##{ref_type}"
         record = {
-            'label_and_type': label_and_type,
-            'concept_id': concept_id.lower(),
-            'src_name': src_name,
-            'item_type': ref_type,
+            "label_and_type": label_and_type,
+            "concept_id": concept_id.lower(),
+            "src_name": src_name.value,
+            "item_type": ref_type,
         }
         try:
             self.batch.put_item(Item=record)
         except ClientError as e:
             logger.error(f"boto3 client error adding reference {term} for "
                          f"{concept_id} with match type {ref_type}: "
                          f"{e.response['Error']['Message']}")
 
-    def update_record(self, concept_id: str, field: str, new_value: Any,
-                      item_type: str = 'identity'):
-        """Update the field of an individual record to a new value.
-        :param str concept_id: record to update
-        :param str field: name of field to update
-        :param str new_value: new value
-        :param str item_type: record type, one of {'identity', 'merger'}
+    def update_merge_ref(self, concept_id: str, merge_ref: Any) -> None:
+        """Update the merged record reference of an individual record to a new value.
+
+        :param concept_id: record to update
+        :param merge_ref: new ref value
+        :raise DatabaseWriteException: if attempting to update non-existent record
         """
+        label_and_type = f"{concept_id.lower()}##identity"
         key = {
-            'label_and_type': f'{concept_id.lower()}##{item_type}',
-            'concept_id': concept_id
+            "label_and_type": label_and_type,
+            "concept_id": concept_id
         }
-        update_expression = f"set {field}=:r"
-        update_values = {':r': new_value}
+        update_expression = "set merge_ref=:r"
+        update_values = {':r': merge_ref.lower()}
+        condition_expression = "attribute_exists(label_and_type)"
         try:
             self.genes.update_item(Key=key,
                                    UpdateExpression=update_expression,
-                                   ExpressionAttributeValues=update_values)
+                                   ExpressionAttributeValues=update_values,
+                                   ConditionExpression=condition_expression)
         except ClientError as e:
-            logger.error(f"boto3 client error in `database.update_record()`: "
-                         f"{e.response['Error']['Message']}")
+            code = e.response.get("Error", {}).get("Code")
+            if code == "ConditionalCheckFailedException":
+                raise DatabaseWriteException(
+                    f"No such record exists for keys {label_and_type}, {concept_id}"
+                )
+            else:
+                logger.error(f"boto3 client error in `database.update_record()`: "
+                             f"{e.response['Error']['Message']}")
 
-    def flush_batch(self):
-        """Flush internal batch_writer."""
+    def delete_normalized_concepts(self) -> None:
+        """Remove merged records from the database. Use when performing a new update
+        of normalized data.
+
+        :raise DatabaseReadException: if DB client requires separate read calls and
+            encounters a failure in the process
+        :raise DatabaseWriteException: if deletion call fails
+        """
+        while True:
+            with self.genes.batch_writer(
+                overwrite_by_pkeys=["label_and_type", "concept_id"]
+            ) as batch:
+                try:
+                    response = self.genes.query(
+                        IndexName="item_type_index",
+                        KeyConditionExpression=Key("item_type").eq("merger"),
+                    )
+                except ClientError as e:
+                    raise DatabaseReadException(e)
+                records = response["Items"]
+                if not records:
+                    break
+                for record in records:
+                    batch.delete_item(Key={
+                        "label_and_type": record["label_and_type"],
+                        "concept_id": record["concept_id"]
+                    })
+
+    def delete_source(self, src_name: SourceName) -> None:
+        """Delete all data for a source. Use when updating source data.
+
+        :param src_name: name of source to delete
+        :raise DatabaseReadException: if DB client requires separate read calls and
+            encounters a failure in the process
+        :raise DatabaseWriteException: if deletion call fails
+        """
+        while True:
+            try:
+                response = self.genes.query(
+                    IndexName="src_index",
+                    KeyConditionExpression=Key("src_name").eq(
+                        src_name.value
+                    )
+                )
+            except ClientError as e:
+                raise DatabaseReadException(e)
+            records = response["Items"]
+            if not records:
+                break
+            with self.genes.batch_writer(
+                overwrite_by_pkeys=["label_and_type", "concept_id"]
+            ) as batch:
+                for record in records:
+                    try:
+                        batch.delete_item(Key={
+                            "label_and_type": record["label_and_type"],
+                            "concept_id": record["concept_id"]
+                        })
+                    except ClientError as e:
+                        raise DatabaseWriteException(e)
+
+        try:
+            self.metadata.delete_item(Key={
+                "src_name": src_name.value
+            })
+        except ClientError as e:
+            raise DatabaseWriteException(e)
+
+    def complete_write_transaction(self) -> None:
+        """Conclude transaction or batch writing if relevant."""
         self.batch.__exit__(*sys.exc_info())
         self.batch = self.genes.batch_writer()
+
+    def close_connection(self) -> None:
+        """Perform any manual connection closure procedures if necessary."""
+        self.batch.__exit__(*sys.exc_info())
+
+    def load_from_remote(self, url: Optional[str] = None) -> None:
+        """Load DB from remote dump. Not available for DynamoDB database backend.
+
+        :param url: remote location to retrieve gzipped dump file from
+        """
+        raise NotImplementedError
+
+    def export_db(self, export_location: Path) -> None:
+        """Dump DB to specified location. Not available for DynamoDB database backend.
+
+        :param export_location: path to save DB dump at
+        """
+        raise NotImplementedError
```

### Comparing `gene-normalizer-0.2.8/gene/etl/base.py` & `gene-normalizer-0.2.9/gene/etl/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """A base class for extraction, transformation, and loading of data."""
 from abc import ABC, abstractmethod
 from typing import Optional, List
-from gene.database import Database
-from gene import PREFIX_LOOKUP, ITEM_TYPES, SEQREPO_DATA_PATH
+from gene.database import AbstractDatabase
+from gene import ITEM_TYPES, SEQREPO_ROOT_DIR
 from biocommons.seqrepo import SeqRepo
 from pathlib import Path
 from ftplib import FTP
 import gzip
 import shutil
 from os import remove
 from dateutil import parser
 import datetime
 import logging
 import pydantic
-from gene.schemas import Gene, MatchType
+from gene.schemas import Gene, MatchType, SourceName
 
 logger = logging.getLogger('gene')
 logger.setLevel(logging.DEBUG)
 
 
 class Base(ABC):
     """The ETL base class."""
 
-    def __init__(self, database: Database, host: str, data_dir: str,
+    def __init__(self, database: AbstractDatabase, host: str, data_dir: str,
                  src_data_dir: Path,
-                 seqrepo_dir=SEQREPO_DATA_PATH,
+                 seqrepo_dir=SEQREPO_ROOT_DIR,
                  *args, **kwargs) -> None:
         """Instantiate Base class.
 
-        :param Database database: DynamoDB database
+        :param AbstractDatabase database: database instance
         :param str host: Hostname of FTP site
         :param str data_dir: Data directory of FTP site to look at
         :param Path src_data_dir: Data directory for source
         :param Path seqrepo_dir: Path to seqrepo directory
         """
+        self._src_name = SourceName(self.__class__.__name__)
         self._database = database
         self._host = host
         self._data_dir = data_dir
         self.src_data_dir = src_data_dir
         self._processed_ids = list()
         self.seqrepo = self.get_seqrepo(seqrepo_dir)
 
     @abstractmethod
     def perform_etl(self) -> List[str]:
-        """Extract, Transform, and Load data into DynamoDB database.
+        """Extract, Transform, and Load data into database.
 
         :return: Concept IDs of concepts successfully loaded
         """
         raise NotImplementedError
 
     @abstractmethod
     def _extract_data(self, *args, **kwargs) -> None:
@@ -57,76 +58,50 @@
     @abstractmethod
     def _transform_data(self, *args, **kwargs) -> None:
         """Transform data to model."""
         raise NotImplementedError
 
     @abstractmethod
     def _add_meta(self, *args, **kwargs) -> None:
-        """Add source meta to DynamoDB table."""
+        """Add source meta to database source info."""
         raise NotImplementedError
 
     def _create_data_directory(self):
         """Create data directory for source."""
         self.src_data_dir.mkdir(exist_ok=True, parents=True)
 
-    def _load_meta(self, db, metadata, source_name) -> None:
-        """Load source metadata into database.
-
-        :param Database db: DynamoDB Database
-        :param SourceMeta metadata: Source's metadata
-        :param str source_name: Source to load metadata for
-        """
-        db.metadata.put_item(Item={
-            'src_name': source_name,
-            'data_license': metadata.data_license,
-            'data_license_url': metadata.data_license_url,
-            'version': metadata.version,
-            'data_url': metadata.data_url,
-            'rdp_url': metadata.rdp_url,
-            'data_license_attributes': metadata.data_license_attributes,
-            'genome_assemblies': metadata.genome_assemblies
-        })
-
-    def _load_gene(self, gene, batch) -> None:
-        """Load a gene record into database.
+    def _load_gene(self, gene) -> None:
+        """Load a gene record into database. This method takes responsibility for:
+         * validating structure correctness
+         * removing duplicates from list-like fields
+         * removing empty fields
 
         :param dict gene: Gene record
-        :param BatchWriter batch: Object to write data to DynamoDB
         """
         try:
             assert Gene(match_type=MatchType.NO_MATCH, **gene)
         except pydantic.error_wrappers.ValidationError as e:
             logger.warning(f"Unable to load {gene} due to validation error: "
                            f"{e}")
         else:
-            concept_id = gene['concept_id'].lower()
-            gene['label_and_type'] = f"{concept_id}##identity"
-            gene['src_name'] = \
-                PREFIX_LOOKUP[gene['concept_id'].split(':')[0].lower()]
+            concept_id = gene['concept_id']
+            gene['label_and_type'] = f"{concept_id.lower()}##identity"
+            gene["src_name"] = self._src_name.value
             gene['item_type'] = 'identity'
 
-            for attr_type, item_type in ITEM_TYPES.items():
+            for attr_type in ITEM_TYPES:
                 if attr_type in gene:
                     value = gene[attr_type]
-                    if value is not None and value != []:
-                        if isinstance(value, str):
-                            items = [value.lower()]
-                        else:
-                            gene[attr_type] = list(set(value))
-                            items = {item.lower() for item in value}
-                        for item in items:
-                            batch.put_item(Item={
-                                'label_and_type': f"{item}##{item_type}",
-                                'concept_id': concept_id,
-                                'src_name': gene['src_name'],
-                                'item_type': item_type
-                            })
-                    else:
+                    if value is None or value == []:
                         del gene[attr_type]
-            batch.put_item(Item=gene)
+                    elif isinstance(value, str):
+                        continue
+                    gene[attr_type] = list(set(value))
+
+            self._database.add_record(gene, self._src_name)
             self._processed_ids.append(concept_id)
 
     def _ftp_download(self, host: str, data_dir: str, fn: str,
                       source_dir: Path,
                       data_fn: str) -> Optional[str]:
         """Download data file from FTP site.
```

### Comparing `gene-normalizer-0.2.8/gene/etl/ensembl.py` & `gene-normalizer-0.2.9/gene/etl/ensembl.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,39 +4,37 @@
 from ftplib import FTP
 
 import gffutils
 
 from .base import Base
 from gene import APP_ROOT
 from gene.schemas import SourceName, NamespacePrefix, Strand, SourceMeta
-from gene.database import Database
+from gene.database import AbstractDatabase
 from gene.etl.vrs_locations import SequenceLocation
 
 
 logger = logging.getLogger("gene")
 logger.setLevel(logging.DEBUG)
 
 
 class Ensembl(Base):
     """ETL the Ensembl source into the normalized database."""
 
-    def __init__(self, database: Database, host="ftp.ensembl.org",
+    def __init__(self, database: AbstractDatabase, host="ftp.ensembl.org",
                  data_dir="pub/current_gff3/homo_sapiens/",
                  src_data_dir=APP_ROOT / "data" / "ensembl") -> None:
         """Initialize Ensembl ETL class.
 
-        :param Database database: DynamoDB database
+        :param AbstractDatabase database: DynamoDB database
         :param str host: FTP host name
         :param str data_dir: FTP data directory to use
         :param Path src_data_dir: Data directory for Ensembl
         """
         super().__init__(database, host, data_dir, src_data_dir)
         self._sequence_location = SequenceLocation()
-        self._host = host
-        self._data_dir = data_dir
         self._version = None
         self._fn = None
         self._data_url = None
         self._assembly = None
 
     def _download_data(self) -> None:
         """Download latest Ensembl GFF3 data file."""
@@ -51,15 +49,15 @@
             for f in files:
                 match = regex.match(f)
                 if match:
                     resp = match.groupdict()
                     self._assembly = resp["assembly"]
                     self._version = resp["version"]
                     self._fn = f
-                    self._data_url = f"ftp://{self._host}/{self._data_dir}{self._fn}"
+                    self._data_url = f"ftp://{self._host}/{self._data_dir}{self._fn}"  # noqa: E501
                     new_fn = f"ensembl_{self._version}.gff3"
                     if not (self.src_data_dir / new_fn).exists():
                         self._ftp_download_file(ftp, self._fn, self.src_data_dir,
                                                 new_fn)
                         logger.info(f"Successfully downloaded Ensembl {self._version}"
                                     f" data.")
                     else:
@@ -85,23 +83,22 @@
         # Get accession numbers
         accession_numbers = dict()
         for item in db.features_of_type("scaffold"):
             accession_numbers[item[0]] = item[8]["Alias"][-1]
         for item in db.features_of_type("chromosome"):
             accession_numbers[item[0]] = item[8]["Alias"][-1]
 
-        with self._database.genes.batch_writer() as batch:
-            for f in db.all_features():
-                if f.attributes.get("ID"):
-                    f_id = f.attributes.get("ID")[0].split(":")[0]
-                    if f_id == "gene":
-                        gene = \
-                            self._add_gene(f, self.seqrepo, accession_numbers)
-                        if gene:
-                            self._load_gene(gene, batch)
+        for f in db.all_features():
+            if f.attributes.get("ID"):
+                f_id = f.attributes.get("ID")[0].split(":")[0]
+                if f_id == "gene":
+                    gene = \
+                        self._add_gene(f, self.seqrepo, accession_numbers)
+                    if gene:
+                        self._load_gene(gene)
         logger.info("Successfully transformed Ensembl.")
 
     def _add_gene(self, f, sr, accession_numbers):
         """Create a transformed gene record.
 
         :param gffutils.feature.Feature f: A gene from the data
         :param SeqRepo sr: Access to the seqrepo
@@ -211,15 +208,15 @@
 
         :return: Concept IDs of concepts successfully loaded
         """
         self._download_data()
         self._extract_data()
         self._add_meta()
         self._transform_data()
-        self._database.flush_batch()
+        self._database.complete_write_transaction()
         return self._processed_ids
 
     def _add_meta(self, *args, **kwargs):
         """Add Ensembl metadata."""
         metadata = SourceMeta(
             data_license="custom",
             data_license_url="https://useast.ensembl.org/info/about"
@@ -231,21 +228,8 @@
                 "non_commercial": False,
                 "share_alike": False,
                 "attribution": False
             },
             genome_assemblies=[self._assembly]
         )
 
-        self._database.metadata.put_item(
-            Item={
-                "src_name": SourceName.ENSEMBL.value,
-                "data_license": metadata.data_license,
-                "data_license_url": metadata.data_license_url,
-                "version": metadata.version,
-                "data_url": metadata.data_url,
-                "rdp_url": metadata.rdp_url,
-                "data_license_attributes": metadata.data_license_attributes,
-                "genome_assemblies": metadata.genome_assemblies
-            }
-        )
-
-        self._load_meta(self._database, metadata, SourceName.ENSEMBL.value)
+        self._database.add_source_metadata(self._src_name, metadata)
```

### Comparing `gene-normalizer-0.2.8/gene/etl/hgnc.py` & `gene-normalizer-0.2.9/gene/etl/hgnc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """This module defines the HGNC ETL methods."""
 import logging
 import json
 import shutil
 import re
 
 from gene import APP_ROOT, PREFIX_LOOKUP
-from gene.database import Database
+from gene.database import AbstractDatabase
 from gene.schemas import SourceName, SymbolStatus, NamespacePrefix, \
     SourceMeta, Annotation, Chromosome
 from gene.etl.base import Base
 from gene.etl.vrs_locations import ChromosomeLocation
 
 logger = logging.getLogger('gene')
 logger.setLevel(logging.DEBUG)
 
 
 class HGNC(Base):
     """ETL the HGNC source into the normalized database."""
 
     def __init__(self,
-                 database: Database,
+                 database: AbstractDatabase,
                  host='ftp.ebi.ac.uk',
                  data_dir='pub/databases/genenames/hgnc/json/',
                  src_data_dir=APP_ROOT / 'data' / 'hgnc',
                  fn='hgnc_complete_set.json'
                  ):
         """Initialize HGNC ETL class.
 
-        :param Database database: DynamoDB database
+        :param AbstractDatabase database: DynamoDB database
         :param str host: FTP host name
         :param str data_dir: FTP data directory to use
         :param Path src_data_dir: Data directory for HGNC
         :param str fn: Data file to download
         """
         super().__init__(database, host, data_dir, src_data_dir)
         self._chromosome_location = ChromosomeLocation()
@@ -62,44 +62,42 @@
         """Transform the HGNC source."""
         logger.info('Transforming HGNC...')
         with open(self._data_src, 'r') as f:
             data = json.load(f)
 
         records = data['response']['docs']
 
-        with self._database.genes.batch_writer() as batch:
-            for r in records:
-                gene = dict()
-                gene['concept_id'] = r['hgnc_id'].lower()
-                gene['label_and_type'] = \
-                    f"{gene['concept_id']}##identity"
-                gene['item_type'] = 'identity'
-                gene['symbol'] = r['symbol']
-                gene['label'] = r['name']
-                gene['src_name'] = SourceName.HGNC.value
-                if r['status']:
-                    if r['status'] == 'Approved':
-                        gene['symbol_status'] = \
-                            SymbolStatus.APPROVED.value
-                    elif r['status'] == 'Entry Withdrawn':
-                        gene['symbol_status'] =\
-                            SymbolStatus.WITHDRAWN.value
-                gene['src_name'] = SourceName.HGNC.value
-
-                # store alias, xref, associated_with, prev_symbols, location
-                self._get_aliases(r, gene)
-                self._get_xrefs_associated_with(r, gene)
-                if 'prev_symbol' in r:
-                    self._get_previous_symbols(r, gene)
-                if 'location' in r:
-                    self._get_location(r, gene)
-                if "locus_type" in r:
-                    gene["gene_type"] = r["locus_type"]
-                self._load_gene(gene, batch)
-        logger.info('Successfully transformed HGNC.')
+        for r in records:
+            gene = dict()
+            gene["concept_id"] = r["hgnc_id"].lower()
+            gene["label_and_type"] = f"{gene['concept_id']}##identity"
+            gene["item_type"] = "identity"
+            gene["symbol"] = r["symbol"]
+            gene["label"] = r["name"]
+            gene["src_name"] = SourceName.HGNC.value
+            if r["status"]:
+                if r["status"] == "Approved":
+                    gene["symbol_status"] = \
+                        SymbolStatus.APPROVED.value
+                elif r["status"] == "Entry Withdrawn":
+                    gene["symbol_status"] =\
+                        SymbolStatus.WITHDRAWN.value
+            gene["src_name"] = SourceName.HGNC.value
+
+            # store alias, xref, associated_with, prev_symbols, location
+            self._get_aliases(r, gene)
+            self._get_xrefs_associated_with(r, gene)
+            if "prev_symbol" in r:
+                self._get_previous_symbols(r, gene)
+            if "location" in r:
+                self._get_location(r, gene)
+            if "locus_type" in r:
+                gene["gene_type"] = r["locus_type"]
+                self._load_gene(gene)
+        logger.info("Successfully transformed HGNC.")
 
     def _get_aliases(self, r, gene):
         """Store aliases in a gene record.
 
         :param dict r: A gene record in the HGNC data file
         :param dict gene: A transformed gene record
         """
@@ -252,16 +250,15 @@
         if arm_match:
             # Location gives arm and sub / sub band
             arm_ix = arm_match.start()
             location['chr'] = loc[:arm_ix]
 
             if '-' in loc:
                 # Location gives both start and end
-                self._chromosome_location.set_interval_range(loc,
-                                                             arm_ix, location)
+                self._chromosome_location.set_interval_range(loc, arm_ix, location)
             else:
                 # Location only gives start
                 start = loc[arm_ix:]
                 location['start'] = start
                 location['end'] = start
         else:
             # Only gives chromosome
@@ -272,27 +269,26 @@
 
         :return: Concept IDs of concepts successfully loaded
         """
         self._download_data()
         self._extract_data()
         self._add_meta()
         self._transform_data()
-        self._database.flush_batch()
+        self._database.complete_write_transaction()
         return self._processed_ids
 
-    def _add_meta(self, *args, **kwargs):
+    def _add_meta(self) -> None:
         """Add HGNC metadata to the gene_metadata table."""
         metadata = SourceMeta(
             data_license='custom',
             data_license_url='https://www.genenames.org/about/',
             version=self._version,
             data_url=self._data_url,
             rdp_url=None,
             data_license_attributes={
                 'non_commercial': False,
                 'share_alike': False,
                 'attribution': False
             },
             genome_assemblies=[]
         )
-
-        self._load_meta(self._database, metadata, SourceName.HGNC.value)
+        self._database.add_source_metadata(SourceName.HGNC, metadata)
```

### Comparing `gene-normalizer-0.2.8/gene/etl/merge.py` & `gene-normalizer-0.2.9/gene/etl/merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Create concept groups and merged records."""
-from gene.database import Database
+from gene.database import AbstractDatabase
+from gene.database.database import DatabaseWriteException
 from gene.schemas import SourcePriority, GeneTypeFieldName
-from typing import Set, Dict
+from typing import Optional, Set, Dict
 from timeit import default_timer as timer
 import logging
 
 
 logger = logging.getLogger("gene")
 logger.setLevel(logging.DEBUG)
 
 
 class Merge:
     """Handles record merging."""
 
-    def __init__(self, database: Database):
+    def __init__(self, database: AbstractDatabase):
         """Initialize Merge instance.
         :param Database database: db instance to use for record retrieval
             and creation.
         """
         self._database = database
         self._groups = {}  # dict keying concept IDs to group Sets
 
@@ -45,49 +46,57 @@
         start = timer()
         for record_id, group in self._groups.items():
             if record_id in uploaded_ids:
                 continue
             merged_record = self._generate_merged_record(group)
 
             # add group merger item to DB
-            self._database.add_record(merged_record, 'merger')
+            self._database.add_merged_record(merged_record)
 
             # add updated references
             for concept_id in group:
-                if not self._database.get_record_by_id(concept_id, False):
-                    logger.error(f"Updating nonexistent record: {concept_id} "
-                                 f"for {merged_record['label_and_type']}")
-                else:
-                    merge_ref = merged_record['concept_id'].lower()
-                    self._database.update_record(concept_id, 'merge_ref',
-                                                 merge_ref)
+                merge_ref = merged_record["concept_id"]
+                try:
+                    self._database.update_merge_ref(concept_id, merge_ref)
+                except DatabaseWriteException as dw:
+                    if str(dw).startswith("No such record exists"):
+                        logger.error(f"Updating nonexistent record: {concept_id} "
+                                     f"for merge ref to {merge_ref}")
+                    else:
+                        logger.error(str(dw))
             uploaded_ids |= group
+        self._database.complete_write_transaction()
         logger.info('Merged concept generation successful.')
         end = timer()
         logger.debug(f'Generated and added concepts in {end - start} seconds')
 
     def _create_record_id_set(self, record_id: str,
-                              observed_id_set: Set = set()) -> Set[str]:
+                              observed_id_set: Optional[Set] = None) -> Set[str]:
         """Create concept ID group for an individual record ID.
         :param str record_id: concept ID for record to build group from
         :return: set of related identifiers pertaining to a common concept.
         """
+        if observed_id_set is None:
+            observed_id_set = set()
+
         if record_id in self._groups:
             return self._groups[record_id]
         else:
             db_record = self._database.get_record_by_id(record_id)
             if not db_record:
                 logger.warning(f"Record ID set creator could not resolve "
                                f"lookup for {record_id} in ID set: "
                                f"{observed_id_set}")
                 return observed_id_set - {record_id}
 
-            local_id_set = set(db_record.get('xrefs', []))
-            if not local_id_set:
-                return observed_id_set | {db_record['concept_id']}
+            record_xrefs = db_record.get("xrefs")
+            if not record_xrefs:
+                return observed_id_set | {db_record["concept_id"]}
+            else:
+                local_id_set = set(record_xrefs)
             merged_id_set = {record_id} | observed_id_set
             for local_record_id in local_id_set - observed_id_set:
                 merged_id_set |= self._create_record_id_set(local_record_id,
                                                             merged_id_set)
             return merged_id_set
 
     def _generate_merged_record(self, record_id_set: Set[str]) -> Dict:
@@ -157,11 +166,9 @@
                                    "ensembl_biotype"]:
             field_value = merged_attrs[field]
             if field_value:
                 merged_attrs[field] = list(field_value)
             else:
                 del merged_attrs[field]
 
-        merged_attrs['label_and_type'] = \
-            f'{merged_attrs["concept_id"].lower()}##merger'
         merged_attrs['item_type'] = 'merger'
         return merged_attrs
```

### Comparing `gene-normalizer-0.2.8/gene/etl/ncbi.py` & `gene-normalizer-0.2.9/gene/etl/ncbi.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 import csv
 from datetime import datetime
 import re
 
 import gffutils
 
 from gene import APP_ROOT, PREFIX_LOOKUP
-from gene.database import Database
+from gene.database import AbstractDatabase
 from gene.schemas import SourceMeta, SourceName, NamespacePrefix, Annotation, \
     Chromosome, SymbolStatus
 from gene.etl.base import Base
 from gene.etl.vrs_locations import SequenceLocation, ChromosomeLocation
 
 
 logger = logging.getLogger('gene')
 logger.setLevel(logging.DEBUG)
 
 
 class NCBI(Base):
     """ETL class for NCBI source"""
 
     def __init__(self,
-                 database: Database,
+                 database: AbstractDatabase,
                  host='ftp.ncbi.nlm.nih.gov',
                  data_dir='gene/DATA/',
                  src_data_dir=APP_ROOT / 'data' / 'ncbi'):
         """Construct the NCBI ETL instance.
 
-        :param Database database: gene database for adding new data
+        :param AbstractDatabase database: gene database for adding new data
         :param str host: FTP host name
         :param str data_dir: FTP data directory to use
         :param Path src_data_dir: Data directory for NCBI
         """
         super().__init__(database, host, data_dir, src_data_dir)
         self._sequence_location = SequenceLocation()
         self._chromosome_location = ChromosomeLocation()
@@ -44,16 +44,17 @@
 
     def perform_etl(self):
         """Perform ETL methods.
 
         :return: Concept IDs of concepts successfully loaded
         """
         self._extract_data()
+        self._add_meta()
         self._transform_data()
-        self._database.flush_batch()
+        self._database.complete_write_transaction()
         return self._processed_ids
 
     def _download_data(self):
         """Download NCBI info, history, and GRCh38 files.
 
         :param str ncbi_dir: The NCBI data directory
         """
@@ -65,15 +66,16 @@
         self._ftp_download(self._host, data_dir, fn, self.src_data_dir, data_fn)
         logger.info('Successfully downloaded NCBI gene_info.')
 
         # Download history
         fn = f'ncbi_history_{self._date_today}.tsv'
         data_fn = 'gene_history.gz'
         logger.info('Downloading NCBI gene_history...')
-        self._ftp_download(self._host, self._data_dir, fn, self.src_data_dir, data_fn)
+        self._ftp_download(self._host, self._data_dir, fn, self.src_data_dir,
+                           data_fn)
         logger.info('Successfully downloaded NCBI gene_history.')
 
         # Download gff
         self._download_gff()
 
     def _download_gff(self) -> None:
         """Download latest gff data"""
@@ -144,34 +146,31 @@
         :return: A dictionary of a gene's previous symbols
         """
         # get symbol history
         history_file = open(self._history_src, 'r')
         history = csv.reader(history_file, delimiter='\t')
         next(history)
         prev_symbols = {}
-        with self._database.genes.batch_writer() as batch:
-            for row in history:
-                # Only interested in rows that have homo sapiens tax id
-                if row[0] == '9606':
-                    if row[1] != '-':
-                        gene_id = row[1]
-                        if gene_id in prev_symbols.keys():
-                            prev_symbols[gene_id].append(row[3])
-                        else:
-                            prev_symbols[gene_id] = [row[3]]
+        for row in history:
+            # Only interested in rows that have homo sapiens tax id
+            if row[0] == "9606":
+                if row[1] != "-":
+                    gene_id = row[1]
+                    if gene_id in prev_symbols.keys():
+                        prev_symbols[gene_id].append(row[3])
                     else:
-                        # Load discontinued genes
-                        params = {
-                            'concept_id':
-                                f'{NamespacePrefix.NCBI.value.lower()}:'
-                                f'{row[2]}',
-                            'symbol': row[3],
-                            'symbol_status': SymbolStatus.DISCONTINUED.value
-                        }
-                        self._load_gene(params, batch)
+                        prev_symbols[gene_id] = [row[3]]
+                else:
+                    # Load discontinued genes
+                    params = {
+                        "concept_id": f"{NamespacePrefix.NCBI.value}:{row[2]}",
+                        "symbol": row[3],
+                        "symbol_status": SymbolStatus.DISCONTINUED.value
+                    }
+                    self._load_gene(params)
         history_file.close()
         return prev_symbols
 
     def _add_xrefs_associated_with(self, val, params):
         """Add xrefs and associated_with refs to a transformed gene.
 
         :param list val: A list of source ids for a given gene
@@ -525,30 +524,28 @@
             location['chr'] = loc[:centromere_ix].strip()
             location['start'] = "cen"
             location['end'] = "cen"
 
     def _transform_data(self):
         """Modify data and pass to loading functions."""
         logger.info('Transforming NCBI...')
-        self._add_meta()
         prev_symbols = self._get_prev_symbols()
         info_genes = self._get_gene_info(prev_symbols)
 
         # create db for gff file
         db = gffutils.create_db(str(self._gff_src),
                                 dbfn=":memory:",
                                 force=True,
                                 merge_strategy="create_unique",
                                 keep_order=True)
 
         self._get_gene_gff(db, info_genes, self.seqrepo)
 
-        with self._database.genes.batch_writer() as batch:
-            for gene in info_genes.keys():
-                self._load_gene(info_genes[gene], batch)
+        for gene in info_genes.keys():
+            self._load_gene(info_genes[gene])
         logger.info('Successfully transformed NCBI.')
 
     def _add_meta(self):
         """Load metadata"""
         metadata = SourceMeta(
             data_license="custom",
             data_license_url="https://www.ncbi.nlm.nih.gov/home/"
@@ -560,8 +557,8 @@
                 'non_commercial': False,
                 'share_alike': False,
                 'attribution': False
             },
             genome_assemblies=[self._assembly]
         )
 
-        self._load_meta(self._database, metadata, SourceName.NCBI.value)
+        self._database.add_source_metadata(SourceName.NCBI, metadata)
```

### Comparing `gene-normalizer-0.2.8/gene/etl/vrs_locations/chromosome_location.py` & `gene-normalizer-0.2.9/gene/etl/vrs_locations/chromosome_location.py`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.2.8/gene/etl/vrs_locations/sequence_location.py` & `gene-normalizer-0.2.9/gene/etl/vrs_locations/sequence_location.py`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.2.8/gene/main.py` & `gene-normalizer-0.2.9/gene/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Main application for FastAPI"""
 from fastapi import FastAPI, HTTPException, Query
 from fastapi.openapi.utils import get_openapi
 from typing import Optional
 from gene import __version__
+from gene.database import create_db
 from gene.query import QueryHandler, InvalidParameterException
 from gene.schemas import SearchService, NormalizeService, \
     UnmergedNormalizationService
 import html
 
 
-query_handler = QueryHandler()
+db = create_db()
+query_handler = QueryHandler(db)
+
 app = FastAPI(
     docs_url="/gene",
     openapi_url="/gene/openapi.json",
     swagger_ui_parameters={"tryItOutEnabled": True}
 )
```

### Comparing `gene-normalizer-0.2.8/gene/query.py` & `gene-normalizer-0.2.9/gene/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """This module provides methods for handling queries."""
 import re
-from typing import List, Dict, Set, Any, TypeVar, Callable, Optional
+from typing import List, Dict, Set, Any, Tuple, TypeVar, Callable, Optional
 from urllib.parse import quote
 from datetime import datetime
 
 from ga4gh.vrsatile.pydantic.core_models import Extension
 from ga4gh.vrsatile.pydantic.vrs_models import VRSTypes
 from ga4gh.vrsatile.pydantic.vrsatile_models import GeneDescriptor
-from botocore.exceptions import ClientError
-from boto3.dynamodb.conditions import Key
 from ga4gh.vrs import models
 from ga4gh.core import ga4gh_identify
 
 from gene import logger
 from gene import NAMESPACE_LOOKUP, PREFIX_LOOKUP, ITEM_TYPES
 from gene.version import __version__
-from gene.database import Database
-from gene.schemas import BaseGene, Gene, SourceMeta, MatchType, SourceName, \
-    ServiceMeta, SourcePriority, NormalizeService, SearchService, \
+from gene.database import AbstractDatabase, DatabaseReadException
+from gene.schemas import BaseGene, Gene, NamespacePrefix, RefType, MatchType, \
+    SourceName, ServiceMeta, SourcePriority, NormalizeService, SearchService, \
     GeneTypeFieldName, UnmergedNormalizationService, MatchesNormalized, \
     BaseNormalizationService
 
 
 NormService = TypeVar("NormService", bound=BaseNormalizationService)
 
 
@@ -32,21 +30,17 @@
 
 
 class QueryHandler:
     """Class for normalizer management. Stores reference to database instance
     and normalizes query input.
     """
 
-    def __init__(self, db_url: str = '', db_region: str = 'us-east-2'):
-        """Initialize QueryHandler instance.
-
-        :param str db_url: URL to database source.
-        :param str db_region: AWS default region.
-        """
-        self.db = Database(db_url=db_url, region_name=db_region)
+    def __init__(self, database: AbstractDatabase) -> None:
+        """Initialize QueryHandler instance."""
+        self.db = database
 
     @staticmethod
     def emit_warnings(query_str: str) -> List:
         """Emit warnings if query contains non breaking space characters.
 
         :param str query_str: query string
         :return: List of warnings
@@ -61,32 +55,14 @@
                 }
             ]
             logger.warning(
                 f'Query ({query_str}) contains non-breaking space characters.'
             )
         return warnings
 
-    def fetch_meta(self, src_name: str) -> SourceMeta:
-        """Fetch metadata for src_name.
-
-        :param str src_name: name of source to get metadata for
-        :return: SourceMeta object containing source metadata
-        """
-        if src_name in self.db.cached_sources.keys():
-            return self.db.cached_sources[src_name]
-        else:
-            try:
-                db_response = self.db.metadata.get_item(Key={'src_name':
-                                                             src_name})
-                response = SourceMeta(**db_response['Item'])
-                self.db.cached_sources[src_name] = response
-                return response
-            except ClientError as e:
-                logger.error(e.response['Error']['Message'])
-
     @staticmethod
     def _transform_sequence_location(loc: Dict) -> models.SequenceLocation:
         """Transform a sequence location to VRS sequence location
 
         :param Dict loc: Sequence location
         :return: VRS sequence location
         """
@@ -112,99 +88,112 @@
     def _transform_location(self, loc: Dict) -> Dict:
         """Transform a sequence/chromosome location to VRS sequence/chromosome location
 
         :param Dict loc: Sequence or Chromosome location
         :return: VRS sequence or chromosome location represented as a dictionary
         """
         if loc["type"] == VRSTypes.SEQUENCE_LOCATION:
-            loc = self._transform_sequence_location(loc)
+            transformed_loc = self._transform_sequence_location(loc)
         else:
-            loc = self._transform_chromosome_location(loc)
-        loc.id = ga4gh_identify(loc)
-        return loc.as_dict()
+            transformed_loc = self._transform_chromosome_location(loc)
+        transformed_loc.id = ga4gh_identify(transformed_loc)
+        return transformed_loc.as_dict()
 
     def _transform_locations(self, record: Dict) -> Dict:
         """Transform gene locations to VRS Chromosome/Sequence Locations
 
         :param Dict record: original record
         :return: record with transformed locations attributes, if applicable
         """
         record_locations = list()
         if "locations" in record:
             for loc in record["locations"]:
                 record_locations.append(self._transform_location(loc))
         record["locations"] = record_locations
         return record
 
+    def _get_src_name(self, concept_id: str) -> SourceName:
+        """Get source name enum from ID.
+
+        :param concept_id: candidate concept ID string to check
+        :return: SourceName option
+        :raise: ValueError if unrecognized ID provided
+        """
+        if concept_id.startswith(NamespacePrefix.ENSEMBL.value):
+            return SourceName.ENSEMBL
+        elif concept_id.startswith(NamespacePrefix.NCBI.value):
+            return SourceName.NCBI
+        elif concept_id.startswith(NamespacePrefix.HGNC.value):
+            return SourceName.HGNC
+        else:
+            raise ValueError("Invalid or unrecognized concept ID provided")
+
     def add_record(self,
                    response: Dict[str, Dict],
                    item: Dict,
-                   match_type: MatchType) -> (Dict, str):
+                   match_type: MatchType):
         """Add individual record (i.e. Item in DynamoDB) to response object
 
         :param Dict[str, Dict] response: in-progress response object to return
             to client
         :param Dict item: Item retrieved from DynamoDB
         :param MatchType match_type: match type for query
-        :return: Tuple containing updated response object, and string
-            containing name of the source of the match
         """
-        del item['label_and_type']
-        # DynamoDB Numbers get converted to Decimal
         item = self._transform_locations(item)
         item["match_type"] = match_type
         gene = Gene(**item)
-        src_name = item['src_name']
+        src_name = item["src_name"]
 
         matches = response['source_matches']
         if src_name not in matches.keys():
             pass
         elif matches[src_name] is None:
             matches[src_name] = {
                 'records': [gene],
-                'source_meta_': self.fetch_meta(src_name)
+                'source_meta_': self.db.get_source_metadata(src_name)
             }
         else:
             matches[src_name]['records'].append(gene)
 
-        return response, src_name
-
     def fetch_record(self, response: Dict[str, Dict], concept_id: str,
                      match_type: MatchType) -> None:
         """Add fetched record to response
 
         :param Dict[str, Dict] response: in-progress response object to return
             to client.
         :param str concept_id: Concept id to fetch record for.
             Should be all lower-case.
         :param MatchType match_type: match type for record
         """
         try:
-            pk = f'{concept_id}##identity'
-            filter_exp = Key('label_and_type').eq(pk)
-            result = self.db.genes.query(KeyConditionExpression=filter_exp)
-            match = result['Items'][0]
-            self.add_record(response, match, match_type)
-        except ClientError as e:
-            logger.error(e.response['Error']['Message'])
+            match = self.db.get_record_by_id(concept_id, case_sensitive=False)
+        except DatabaseReadException as e:
+            logger.error(
+                f"Encountered DatabaseReadException looking up {concept_id}: {e}"
+            )
+        else:
+            if match:
+                self.add_record(response, match, match_type)
+            else:
+                logger.error(f"Unable to find expected record for {concept_id} matching as {match_type}")  # noqa: E501
 
     def post_process_resp(self, resp: Dict) -> Dict:
         """Fill all empty source_matches slots with NO_MATCH results and
         sort source records by descending `match_type`.
 
         :param Dict resp: incoming response object
         :return: response object with empty source slots filled with
                 NO_MATCH results and corresponding source metadata
         """
         for src_name in resp['source_matches'].keys():
             if resp['source_matches'][src_name] is None:
                 resp['source_matches'][src_name] = {
                     'match_type': MatchType.NO_MATCH,
                     'records': [],
-                    'source_meta_': self.fetch_meta(src_name)
+                    'source_meta_': self.db.get_source_metadata(src_name)
                 }
             else:
                 records = resp['source_matches'][src_name]['records']
                 if len(records) > 1:
                     records = sorted(
                         records, key=lambda k: k.match_type, reverse=True)
         return resp
@@ -226,47 +215,43 @@
         }
         if query == '':
             return self.post_process_resp(resp)
         query_l = query.lower()
 
         queries = list()
         if [p for p in PREFIX_LOOKUP.keys() if query_l.startswith(p)]:
-            pk = f'{query_l}##identity'
-            queries.append(pk)
+            queries.append((query_l, "identity"))
 
         for prefix in [p for p in NAMESPACE_LOOKUP.keys() if
                        query_l.startswith(p)]:
-            pk = f'{NAMESPACE_LOOKUP[prefix].lower()}:{query_l}##identity'
-            queries.append(pk)
+            term = f"{NAMESPACE_LOOKUP[prefix].lower()}:{query_l}"
+            queries.append((term, "identity"))
 
         for match in ITEM_TYPES.values():
-            pk = f'{query_l}##{match}'
-            queries.append(pk)
+            queries.append((query_l, match))
 
         matched_concept_ids = list()
-        for q in queries:
+        for term, item_type in queries:
             try:
-                query_resp = self.db.genes.query(
-                    KeyConditionExpression=Key('label_and_type').eq(q)
-                )
-                for record in query_resp['Items']:
-                    concept_id = record['concept_id']
-                    if concept_id in matched_concept_ids:
-                        continue
-                    else:
-                        if record['item_type'] == "identity":
-                            self.add_record(resp, record, MatchType.CONCEPT_ID)
-                        else:
-                            self.fetch_record(
-                                resp, concept_id,
-                                MatchType[record['item_type'].upper()])
-                        matched_concept_ids.append(concept_id)
+                if item_type == "identity":
+                    record = self.db.get_record_by_id(term, False)
+                    if record and record['concept_id'] not in matched_concept_ids:
+                        self.add_record(resp, record, MatchType.CONCEPT_ID)
+                else:
+                    refs = self.db.get_refs_by_type(term, RefType(item_type))
+                    for ref in refs:
+                        if ref not in matched_concept_ids:
+                            self.fetch_record(resp, ref, MatchType[item_type.upper()])
+                            matched_concept_ids.append(ref)
 
-            except ClientError as e:
-                logger.error(e.response['Error']['Message'])
+            except DatabaseReadException as e:
+                logger.error(
+                    f"Encountered DatabaseReadException looking up {item_type}"
+                    f" {term}: {e}"
+                )
                 continue
 
         # remaining sources get no match
         return self.post_process_resp(resp)
 
     def response_list(self, query: str, sources: Set[str]) -> Dict:
         """Return response as list, where the first key-value in each item
@@ -318,15 +303,15 @@
             provided, or if invalid source names are given.
         :return: SearchService class containing all matches found in sources.
         """
         possible_sources = {name.value.lower(): name.value for name in
                             SourceName.__members__.values()}
         sources = dict()
         for k, v in possible_sources.items():
-            if self.db.metadata.get_item(Key={'src_name': v}).get('Item'):
+            if self.db.get_source_metadata(v):
                 sources[k] = v
 
         if not incl and not excl:
             query_sources = set(sources.values())
         elif incl and excl:
             detail = "Cannot request both source inclusions and exclusions."
             raise InvalidParameterException(detail)
@@ -377,15 +362,15 @@
         gene_descr = response.gene_descriptor
         xrefs = gene_descr.xrefs or []  # type: ignore
         ids = [gene_descr.gene] + xrefs  # type: ignore
         for concept_id in ids:
             prefix = concept_id.split(':')[0]
             src_name = PREFIX_LOOKUP[prefix.lower()]
             if src_name not in sources_meta:
-                sources_meta[src_name] = self.fetch_meta(src_name)
+                sources_meta[src_name] = self.db.get_source_metadata(src_name)
         response.source_meta_ = sources_meta
         return response
 
     def _add_alt_matches(self, response: NormService, record: Dict,
                          possible_concepts: List[str]) -> NormService:
         """Add alternate matches warning to response object
 
@@ -501,15 +486,15 @@
 
         response.gene_descriptor = GeneDescriptor(**params)
         response = self._add_merged_meta(response)
         response.match_type = match_type
         return response
 
     @staticmethod
-    def _record_order(record: Dict) -> (int, str):
+    def _record_order(record: Dict) -> Tuple[int, str]:
         """Construct priority order for matching. Only called by sort().
 
         :param Dict record: individual record item in iterable to sort
         :return: tuple with rank value and concept ID
         """
         src = record['src_name'].upper()
         source_rank = SourcePriority[src]
@@ -580,29 +565,19 @@
                 return response
             else:
                 return callback(response, merge, match_type, possible_concepts)
         else:
             # record is sole member of concept group
             return callback(response, record, match_type, possible_concepts)
 
-    def _get_matches_by_type(self, query: str, match_type: str) -> List[Dict]:
-        """Get matches list for match tier.
-        :param str query: user-provided query
-        :param str match_type: keyword of match type to check
-        :return: List of records matching the query and match level
-        """
-        matching_refs = self.db.get_records_by_type(query, match_type)
-        matching_records = [self.db.get_record_by_id(m["concept_id"], False)
-                            for m in matching_refs]
-        return sorted(matching_records, key=self._record_order)  # type: ignore
-
     def _perform_normalized_lookup(
         self, response: NormService, query: str, response_builder: Callable
     ) -> NormService:
         """Retrieve normalized concept, for use in normalization endpoints
+
         :param NormService response: in-progress response object
         :param str query: user-provided query
         :param Callable response_builder: response constructor callback method
         :return: completed service response object
         """
         if query == "":
             return response
@@ -615,34 +590,32 @@
 
         # check concept ID match
         record = self.db.get_record_by_id(query_str, case_sensitive=False)
         if record:
             return self._resolve_merge(response, record, MatchType.CONCEPT_ID,
                                        response_builder)
 
-        for match_type in ITEM_TYPES.values():
+        for match_type in RefType:
             # get matches list for match tier
-            matching_refs = self.db.get_records_by_type(query_str, match_type)
+            matching_refs = self.db.get_refs_by_type(query_str, match_type)
             matching_records = \
-                [self.db.get_record_by_id(m['concept_id'], False)
-                 for m in matching_refs]
+                [self.db.get_record_by_id(ref, False) for ref in matching_refs]
             matching_records.sort(key=self._record_order)  # type: ignore
 
             if len(matching_refs) > 1:
-                possible_concepts = \
-                    [ref["concept_id"] for ref in matching_refs]
+                possible_concepts = [ref for ref in matching_refs]
             else:
                 possible_concepts = None
 
             # attempt merge ref resolution until successful
             for match in matching_records:
                 assert match is not None
                 record = self.db.get_record_by_id(match["concept_id"], False)
                 if record:
-                    match_type_value = MatchType[match_type.upper()]
+                    match_type_value = MatchType[match_type.value.upper()]
                     return self._resolve_merge(
                         response, record, match_type_value,
                         response_builder, possible_concepts
                     )
         return response
 
     def _add_normalized_records(
@@ -658,33 +631,35 @@
         :param Optional[List[str]] possible_concepts: other possible results
         :return: Completed response object
         """
         response.match_type = match_type
         response.normalized_concept_id = normalized_record["concept_id"]
         if normalized_record["item_type"] == "identity":
             record_source = SourceName[normalized_record["src_name"].upper()]
+            meta = self.db.get_source_metadata(record_source.value)
             response.source_matches[record_source] = MatchesNormalized(
                 records=[BaseGene(**self._transform_locations(normalized_record))],
-                source_meta_=self.fetch_meta(record_source.value)
+                source_meta_=meta  # type: ignore
             )
         else:
             concept_ids = [normalized_record["concept_id"]] + \
                 normalized_record.get("xrefs", [])
             for concept_id in concept_ids:
                 record = self.db.get_record_by_id(concept_id, case_sensitive=False)
                 if not record:
                     continue
                 record_source = SourceName[record["src_name"].upper()]
                 gene = BaseGene(**self._transform_locations(record))
                 if record_source in response.source_matches:
                     response.source_matches[record_source].records.append(gene)
                 else:
+                    meta = self.db.get_source_metadata(record_source.value)
                     response.source_matches[record_source] = MatchesNormalized(
                         records=[gene],
-                        source_meta_=self.fetch_meta(record_source.value)
+                        source_meta_=meta,  # type: ignore
                     )
         if possible_concepts:
             response = self._add_alt_matches(response, normalized_record,
                                              possible_concepts)
         return response
 
     def normalize_unmerged(self, query: str) -> UnmergedNormalizationService:
```

### Comparing `gene-normalizer-0.2.8/gene/schemas.py` & `gene-normalizer-0.2.9/gene/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,16 +204,16 @@
     """Define constraints for data license attributes."""
 
     non_commercial: StrictBool
     share_alike: StrictBool
     attribution: StrictBool
 
 
-class ItemTypes(str, Enum):
-    """Item types used in DynamoDB."""
+class RefType(str, Enum):
+    """Reference item types."""
 
     # Must be in descending MatchType order.
     SYMBOL = 'symbol'
     PREVIOUS_SYMBOLS = 'prev_symbol'
     ALIASES = 'alias'
     XREFS = 'xref'
     ASSOCIATED_WITH = 'associated_with'
```

### Comparing `gene-normalizer-0.2.8/setup.cfg` & `gene-normalizer-0.2.9/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -30,19 +30,29 @@
 	ga4gh.vrsatile.pydantic >= 0.1.0.dev7
 	ga4gh.vrs >= 0.9.0.dev0
 tests_require = 
 	pytest
 	pytest-cov
 	mock
 
+[options.package_data]
+gene = 
+	database/postgresql/*
+
+[options.entry_points]
+console_scripts = 
+	gene_norm_update = gene.cli:update_normalizer_db
+	gene_norm_update_remote = gene.cli:update_from_remote
+	gene_norm_dump = gene.cli:dump_database
+
 [options.extras_require]
 dev = 
+	psycopg[binary]
 	gffutils
 	biocommons.seqrepo
-	psycopg2-binary
 	pytest
 	pre-commit
 	flake8
 	flake8-docstrings
 	pytest-cov
 	mock
 	ipykernel
```

