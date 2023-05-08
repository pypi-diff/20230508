# Comparing `tmp/ekaros-0.1.7.tar.gz` & `tmp/ekaros-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekaros-0.1.7.tar", max compression
+gzip compressed data, was "ekaros-0.1.8.tar", max compression
```

## Comparing `ekaros-0.1.7.tar` & `ekaros-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1071 2023-04-26 19:07:51.621558 ekaros-0.1.7/LICENSE
--rw-r--r--   0        0        0     3345 2023-04-26 19:07:51.621558 ekaros-0.1.7/README.md
--rw-r--r--   0        0        0     2835 2023-04-26 19:08:24.203860 ekaros-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/__cli__.py
--rw-r--r--   0        0        0      887 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/__init__.py
--rw-r--r--   0        0        0       22 2023-04-26 19:08:24.143856 ekaros-0.1.7/src/ekaros/_version.py
--rw-r--r--   0        0        0        0 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/__init__.py
--rw-r--r--   0        0        0      220 2023-04-26 19:08:24.143856 ekaros-0.1.7/src/ekaros/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-26 19:07:51.621558 ekaros-0.1.7/src/ekaros/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/conf/task/__init__.yaml
--rw-r--r--   0        0        0      196 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/project.toml
--rw-r--r--   0        0        0        0 2023-04-26 19:07:51.625559 ekaros-0.1.7/src/ekaros/py.typed
--rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 ekaros-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 04:33:55.195780 ekaros-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1798 2023-05-08 04:33:55.195780 ekaros-0.1.8/README.md
+-rw-r--r--   0        0        0     2917 2023-05-08 04:34:18.899757 ekaros-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      287 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/__cli__.py
+-rw-r--r--   0        0        0      379 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-08 04:34:18.851757 ekaros-0.1.8/src/ekaros/_version.py
+-rw-r--r--   0        0        0        0 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/__init__.py
+-rw-r--r--   0        0        0      222 2023-05-08 04:34:18.851757 ekaros-0.1.8/src/ekaros/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      807 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      196 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/project.toml
+-rw-r--r--   0        0        0        0 2023-05-08 04:33:55.199780 ekaros-0.1.8/src/ekaros/py.typed
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 ekaros-0.1.8/PKG-INFO
```

### Comparing `ekaros-0.1.7/LICENSE` & `ekaros-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.7/pyproject.toml` & `ekaros-0.1.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 [tool.poetry]
 name = "ekaros"
-version = "0.1.7"
+version = "0.1.8"
 description = "A Python Library for Generative AI Art"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://ekaros.entelecheia.ai"
 repository = "https://github.com/entelecheia/ekaros"
 readme = "README.md"
 packages = [{ include = "ekaros", from = "src" }]
 
 [tool.poetry.scripts]
 ekaros = 'ekaros.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.20"
+hyfi = "^0.4.0"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
+
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
@@ -70,15 +76,14 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/ekaros/_version.py:__version__"
 version_pattern = 'src/ekaros/conf/about/__init__.yaml:version: "{version}"'
@@ -87,13 +92,14 @@
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
+build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `ekaros-0.1.7/src/ekaros/conf/dotenv/__init__.yaml` & `ekaros-0.1.8/src/ekaros/conf/dotenv/__init__.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # HYFI_VERBOSE:
 # NUM_WORKERS:
 # CACHED_PATH_CACHE_ROOT:
 
 # # Secrets
 # WANDB_API_KEY:
 # HUGGING_FACE_HUB_TOKEN:
+# OPENAI_API_KEY:
 # ECOS_API_KEY:
 # FRED_API_KEY:
 # NASDAQ_API_KEY:
 # HF_USER_ACCESS_TOKEN:
 # LABEL_STUDIO_USER_TOKEN:
 
 # # Environment variables for other packages
```

### Comparing `ekaros-0.1.7/src/ekaros/conf/hydra/help/help.yaml` & `ekaros-0.1.8/src/ekaros/conf/hydra/help/help.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # Configuration generated with overrides:
 #   $CONFIG : Generated config
 #
 template: |-
   ${hydra.help.header} 
   
-  author: ${about.author}
+  authors: ${about.authors}
   description: ${about.description}
 
   ${hydra.help.app_name} Command Line Interface for Hydra
 
   == Configuration groups ==
 
   Compose your configuration from those groups (task=task_name)
```

### Comparing `ekaros-0.1.7/src/ekaros/conf/mode/__init__.yaml` & `ekaros-0.1.8/src/ekaros/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.7/src/ekaros/conf/path/__default__.yaml` & `ekaros-0.1.8/src/ekaros/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `ekaros-0.1.7/src/ekaros/conf/path/__init__.yaml` & `ekaros-0.1.8/src/ekaros/conf/path/__init__.yaml`

 * *Files identical despite different names*

