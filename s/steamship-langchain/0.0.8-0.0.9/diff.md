# Comparing `tmp/steamship-langchain-0.0.8.tar.gz` & `tmp/steamship-langchain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamship-langchain-0.0.8.tar", last modified: Wed Feb  8 06:43:13 2023, max compression
+gzip compressed data, was "steamship-langchain-0.0.9.tar", last modified: Wed Feb  8 22:18:51 2023, max compression
```

## Comparing `steamship-langchain-0.0.8.tar` & `steamship-langchain-0.0.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.581509 steamship-langchain-0.0.8/
--rw-r--r--   0 dougreid   (501) staff       (20)      493 2022-12-30 20:00:12.000000 steamship-langchain-0.0.8/.flake8
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.563053 steamship-langchain-0.0.8/.github/
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.568670 steamship-langchain-0.0.8/.github/workflows/
--rw-r--r--   0 dougreid   (501) staff       (20)     1521 2023-01-06 23:46:37.000000 steamship-langchain-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 dougreid   (501) staff       (20)     2353 2023-01-06 23:46:37.000000 steamship-langchain-0.0.8/.github/workflows/test-main.yml
--rw-r--r--   0 dougreid   (501) staff       (20)     1198 2023-02-06 23:15:34.000000 steamship-langchain-0.0.8/.gitignore
--rw-r--r--   0 dougreid   (501) staff       (20)     2227 2022-12-30 20:00:12.000000 steamship-langchain-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 dougreid   (501) staff       (20)      273 2022-12-30 20:04:44.000000 steamship-langchain-0.0.8/AUTHORS.rst
--rw-r--r--   0 dougreid   (501) staff       (20)     3606 2023-02-05 23:51:50.000000 steamship-langchain-0.0.8/DEVELOPING.md
--rw-r--r--   0 dougreid   (501) staff       (20)     1082 2022-12-30 20:04:44.000000 steamship-langchain-0.0.8/LICENSE
--rw-r--r--   0 dougreid   (501) staff       (20)    13889 2023-02-08 06:43:13.581257 steamship-langchain-0.0.8/PKG-INFO
--rw-r--r--   0 dougreid   (501) staff       (20)    13628 2023-02-08 06:36:03.000000 steamship-langchain-0.0.8/README.md
--rw-r--r--   0 dougreid   (501) staff       (20)      656 2023-02-05 23:53:24.000000 steamship-langchain-0.0.8/TESTING.md
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.564124 steamship-langchain-0.0.8/examples/
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.568960 steamship-langchain-0.0.8/examples/chatbot/
--rw-r--r--   0 dougreid   (501) staff       (20)     1370 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/chatbot/README.md
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.569372 steamship-langchain-0.0.8/examples/chatbot/client/
--rw-r--r--   0 dougreid   (501) staff       (20)     1821 2023-02-06 23:20:55.000000 steamship-langchain-0.0.8/examples/chatbot/client/client.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.570645 steamship-langchain-0.0.8/examples/chatbot/server/
--rw-r--r--   0 dougreid   (501) staff       (20)     1350 2023-02-08 06:36:03.000000 steamship-langchain-0.0.8/examples/chatbot/server/api.py
--rw-r--r--   0 dougreid   (501) staff       (20)     1561 2023-02-06 22:39:02.000000 steamship-langchain-0.0.8/examples/chatbot/server/prompt.py
--rw-r--r--   0 dougreid   (501) staff       (20)       19 2023-02-08 06:01:03.000000 steamship-langchain-0.0.8/examples/chatbot/server/requirements.txt
--rw-r--r--   0 dougreid   (501) staff       (20)      631 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/chatbot/server/steamship.json
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.570849 steamship-langchain-0.0.8/examples/greeting/
--rw-r--r--   0 dougreid   (501) staff       (20)     1386 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/greeting/README.md
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.571104 steamship-langchain-0.0.8/examples/greeting/client/
--rw-r--r--   0 dougreid   (501) staff       (20)      642 2023-02-07 06:31:11.000000 steamship-langchain-0.0.8/examples/greeting/client/client.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.571781 steamship-langchain-0.0.8/examples/greeting/server/
--rw-r--r--   0 dougreid   (501) staff       (20)      636 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/greeting/server/api.py
--rw-r--r--   0 dougreid   (501) staff       (20)       19 2023-02-06 21:53:19.000000 steamship-langchain-0.0.8/examples/greeting/server/requirements.txt
--rw-r--r--   0 dougreid   (501) staff       (20)      652 2023-02-07 06:32:13.000000 steamship-langchain-0.0.8/examples/greeting/server/steamship.json
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.572367 steamship-langchain-0.0.8/examples/qa_with_sources/
--rw-r--r--   0 dougreid   (501) staff       (20)     1516 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/qa_with_sources/README.md
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.572884 steamship-langchain-0.0.8/examples/qa_with_sources/client/
--rw-r--r--   0 dougreid   (501) staff       (20)     2199 2023-02-07 09:25:37.000000 steamship-langchain-0.0.8/examples/qa_with_sources/client/client.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.573753 steamship-langchain-0.0.8/examples/qa_with_sources/server/
--rw-r--r--   0 dougreid   (501) staff       (20)     2795 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/qa_with_sources/server/api.py
--rw-r--r--   0 dougreid   (501) staff       (20)       19 2023-02-07 08:36:35.000000 steamship-langchain-0.0.8/examples/qa_with_sources/server/requirements.txt
--rw-r--r--   0 dougreid   (501) staff       (20)      602 2023-02-07 08:37:41.000000 steamship-langchain-0.0.8/examples/qa_with_sources/server/steamship.json
--rw-r--r--   0 dougreid   (501) staff       (20)    45779 2023-02-07 08:42:31.000000 steamship-langchain-0.0.8/examples/qa_with_sources/state-of-the-union-2022.txt
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.574036 steamship-langchain-0.0.8/examples/self-ask-with-search/
--rw-r--r--   0 dougreid   (501) staff       (20)     1395 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/self-ask-with-search/README.md
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.574317 steamship-langchain-0.0.8/examples/self-ask-with-search/client/
--rw-r--r--   0 dougreid   (501) staff       (20)     1337 2023-02-06 23:27:34.000000 steamship-langchain-0.0.8/examples/self-ask-with-search/client/client.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.575227 steamship-langchain-0.0.8/examples/self-ask-with-search/server/
--rw-r--r--   0 dougreid   (501) staff       (20)     1202 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/self-ask-with-search/server/api.py
--rw-r--r--   0 dougreid   (501) staff       (20)       19 2023-02-06 21:53:19.000000 steamship-langchain-0.0.8/examples/self-ask-with-search/server/requirements.txt
--rw-r--r--   0 dougreid   (501) staff       (20)      657 2023-02-06 23:05:14.000000 steamship-langchain-0.0.8/examples/self-ask-with-search/server/steamship.json
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.575500 steamship-langchain-0.0.8/examples/summarize-audio/
--rw-r--r--   0 dougreid   (501) staff       (20)     1935 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/summarize-audio/README.md
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.575716 steamship-langchain-0.0.8/examples/summarize-audio/client/
--rw-r--r--   0 dougreid   (501) staff       (20)     2055 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/summarize-audio/client/client.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.576349 steamship-langchain-0.0.8/examples/summarize-audio/server/
--rw-r--r--   0 dougreid   (501) staff       (20)     1567 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/summarize-audio/server/api.py
--rw-r--r--   0 dougreid   (501) staff       (20)       19 2023-02-06 21:53:19.000000 steamship-langchain-0.0.8/examples/summarize-audio/server/requirements.txt
--rw-r--r--   0 dougreid   (501) staff       (20)      679 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/examples/summarize-audio/server/steamship.json
--rw-r--r--   0 dougreid   (501) staff       (20)     1860 2023-02-04 02:07:36.000000 steamship-langchain-0.0.8/pyproject.toml
--rw-r--r--   0 dougreid   (501) staff       (20)     1172 2023-01-25 22:01:10.000000 steamship-langchain-0.0.8/requirements.dev.txt
--rw-r--r--   0 dougreid   (501) staff       (20)       51 2023-02-07 09:25:18.000000 steamship-langchain-0.0.8/requirements.txt
--rw-r--r--   0 dougreid   (501) staff       (20)       38 2023-02-08 06:43:13.581563 steamship-langchain-0.0.8/setup.cfg
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.564721 steamship-langchain-0.0.8/src/
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.576517 steamship-langchain-0.0.8/src/steamship_langchain/
--rw-r--r--   0 dougreid   (501) staff       (20)        0 2023-02-03 22:39:51.000000 steamship-langchain-0.0.8/src/steamship_langchain/__init__.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.577606 steamship-langchain-0.0.8/src/steamship_langchain/cache/
--rw-r--r--   0 dougreid   (501) staff       (20)      226 2023-02-03 23:10:28.000000 steamship-langchain-0.0.8/src/steamship_langchain/cache/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)     2953 2023-02-07 07:49:10.000000 steamship-langchain-0.0.8/src/steamship_langchain/cache/cache.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.578010 steamship-langchain-0.0.8/src/steamship_langchain/llms/
--rw-r--r--   0 dougreid   (501) staff       (20)      152 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/src/steamship_langchain/llms/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)     4608 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/src/steamship_langchain/llms/openai.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.578378 steamship-langchain-0.0.8/src/steamship_langchain/memory/
--rw-r--r--   0 dougreid   (501) staff       (20)      317 2023-02-08 06:36:03.000000 steamship-langchain-0.0.8/src/steamship_langchain/memory/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)     4563 2023-02-08 06:36:03.000000 steamship-langchain-0.0.8/src/steamship_langchain/memory/conversation_memory.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.578837 steamship-langchain-0.0.8/src/steamship_langchain/tools/
--rw-r--r--   0 dougreid   (501) staff       (20)      172 2023-02-04 02:12:55.000000 steamship-langchain-0.0.8/src/steamship_langchain/tools/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)     2128 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/src/steamship_langchain/tools/search_tool.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.577207 steamship-langchain-0.0.8/src/steamship_langchain.egg-info/
--rw-r--r--   0 dougreid   (501) staff       (20)    13889 2023-02-08 06:43:13.000000 steamship-langchain-0.0.8/src/steamship_langchain.egg-info/PKG-INFO
--rw-r--r--   0 dougreid   (501) staff       (20)     2240 2023-02-08 06:43:13.000000 steamship-langchain-0.0.8/src/steamship_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 dougreid   (501) staff       (20)        1 2023-02-08 06:43:13.000000 steamship-langchain-0.0.8/src/steamship_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 dougreid   (501) staff       (20)       52 2023-02-08 06:43:13.000000 steamship-langchain-0.0.8/src/steamship_langchain.egg-info/requires.txt
--rw-r--r--   0 dougreid   (501) staff       (20)       20 2023-02-08 06:43:13.000000 steamship-langchain-0.0.8/src/steamship_langchain.egg-info/top_level.txt
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.579032 steamship-langchain-0.0.8/tests/
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.579429 steamship-langchain-0.0.8/tests/cache/
--rw-r--r--   0 dougreid   (501) staff       (20)        0 2023-02-03 22:45:49.000000 steamship-langchain-0.0.8/tests/cache/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)     1276 2023-02-04 02:13:08.000000 steamship-langchain-0.0.8/tests/cache/test_cache.py
--rw-r--r--   0 dougreid   (501) staff       (20)      420 2023-02-05 23:49:10.000000 steamship-langchain-0.0.8/tests/conftest.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.579778 steamship-langchain-0.0.8/tests/llms/
--rw-r--r--   0 dougreid   (501) staff       (20)        0 2023-02-03 22:46:23.000000 steamship-langchain-0.0.8/tests/llms/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)     2324 2023-02-08 06:35:59.000000 steamship-langchain-0.0.8/tests/llms/test_openai.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.580061 steamship-langchain-0.0.8/tests/memory/
--rw-r--r--   0 dougreid   (501) staff       (20)        0 2023-02-03 22:46:36.000000 steamship-langchain-0.0.8/tests/memory/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)     6248 2023-02-08 06:36:03.000000 steamship-langchain-0.0.8/tests/memory/test_conversation_memory.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.580337 steamship-langchain-0.0.8/tests/tools/
--rw-r--r--   0 dougreid   (501) staff       (20)        0 2023-02-03 22:47:09.000000 steamship-langchain-0.0.8/tests/tools/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)      371 2023-02-04 02:13:08.000000 steamship-langchain-0.0.8/tests/tools/test_search_tool.py
-drwxr-xr-x   0 dougreid   (501) staff       (20)        0 2023-02-08 06:43:13.580884 steamship-langchain-0.0.8/tests/utils/
--rw-r--r--   0 dougreid   (501) staff       (20)        0 2023-02-03 22:50:55.000000 steamship-langchain-0.0.8/tests/utils/__init__.py
--rw-r--r--   0 dougreid   (501) staff       (20)      358 2023-02-07 21:21:05.000000 steamship-langchain-0.0.8/tests/utils/client.py
--rw-r--r--   0 dougreid   (501) staff       (20)      731 2023-02-05 23:54:08.000000 steamship-langchain-0.0.8/tests/utils/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.988333 steamship-langchain-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/.github/workflows/test-main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/DEVELOPING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/TESTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.988333 steamship-langchain-0.0.9/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/chatbot/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/chatbot/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/chatbot/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/chatbot/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/chatbot/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/chatbot/server/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/chatbot/server/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/chatbot/server/steamship.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/greeting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/greeting/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/greeting/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/greeting/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/greeting/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/greeting/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/greeting/server/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/greeting/server/steamship.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/qa_with_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/qa_with_sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.992333 steamship-langchain-0.0.9/examples/qa_with_sources/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/qa_with_sources/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/examples/qa_with_sources/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/qa_with_sources/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/qa_with_sources/server/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/qa_with_sources/server/steamship.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/qa_with_sources/state-of-the-union-2022.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/examples/self-ask-with-search/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/self-ask-with-search/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/examples/self-ask-with-search/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/self-ask-with-search/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/examples/self-ask-with-search/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/self-ask-with-search/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/self-ask-with-search/server/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/self-ask-with-search/server/steamship.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/examples/summarize-audio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/summarize-audio/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/examples/summarize-audio/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/summarize-audio/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/examples/summarize-audio/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/summarize-audio/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/summarize-audio/server/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/examples/summarize-audio/server/steamship.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.988333 steamship-langchain-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/src/steamship_langchain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/src/steamship_langchain/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/src/steamship_langchain/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/llms/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/src/steamship_langchain/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/memory/conversation_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/src/steamship_langchain/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/src/steamship_langchain/tools/search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/src/steamship_langchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-02-08 22:18:50.000000 steamship-langchain-0.0.9/src/steamship_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-02-08 22:18:50.000000 steamship-langchain-0.0.9/src/steamship_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 22:18:50.000000 steamship-langchain-0.0.9/src/steamship_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-08 22:18:50.000000 steamship-langchain-0.0.9/src/steamship_langchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-08 22:18:50.000000 steamship-langchain-0.0.9/src/steamship_langchain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:50.996333 steamship-langchain-0.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/tests/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/cache/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/tests/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/llms/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/tests/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/memory/test_conversation_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/tools/test_search_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:51.000333 steamship-langchain-0.0.9/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-08 22:18:39.000000 steamship-langchain-0.0.9/tests/utils/fixtures.py
```

### Comparing `steamship-langchain-0.0.8/.github/workflows/python-publish.yml` & `steamship-langchain-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/.github/workflows/test-main.yml` & `steamship-langchain-0.0.9/.github/workflows/test-main.yml`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/.gitignore` & `steamship-langchain-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/.pre-commit-config.yaml` & `steamship-langchain-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/DEVELOPING.md` & `steamship-langchain-0.0.9/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/LICENSE` & `steamship-langchain-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/PKG-INFO` & `steamship-langchain-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamship-langchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: The fastest way to deploy a production langchain API.
 Project-URL: Homepage, https://steamship.com/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # Steamship Python Client Library For LangChain (🦜️🔗)
@@ -32,15 +32,15 @@
 ```commandline
 pip install steamship-langchain
 ```
 
 ## Adapters
 
 Initial support is offered for the following (with more to follow soon):
-- LLMS
+- LLMs
   - An adapter is provided for Steamship's OpenAI integration (`steamship_langchain.llms.OpenAI`)
   - An adapter is provided for *caching* LLM calls, via Steamship's Key-Value store (`SteamshipCache`) 
 - Tools
   - Search:
     - An adapter is provided for Steamship's SERPAPI integration (`SteamshipSERP`)
 - Memory
   - Two adapters that provide persistent conversation memory:
```

### Comparing `steamship-langchain-0.0.8/README.md` & `steamship-langchain-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ```commandline
 pip install steamship-langchain
 ```
 
 ## Adapters
 
 Initial support is offered for the following (with more to follow soon):
-- LLMS
+- LLMs
   - An adapter is provided for Steamship's OpenAI integration (`steamship_langchain.llms.OpenAI`)
   - An adapter is provided for *caching* LLM calls, via Steamship's Key-Value store (`SteamshipCache`) 
 - Tools
   - Search:
     - An adapter is provided for Steamship's SERPAPI integration (`SteamshipSERP`)
 - Memory
   - Two adapters that provide persistent conversation memory:
```

### Comparing `steamship-langchain-0.0.8/TESTING.md` & `steamship-langchain-0.0.9/TESTING.md`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/chatbot/README.md` & `steamship-langchain-0.0.9/examples/chatbot/README.md`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/chatbot/client/client.py` & `steamship-langchain-0.0.9/examples/chatbot/client/client.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/chatbot/server/api.py` & `steamship-langchain-0.0.9/examples/chatbot/server/api.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/chatbot/server/prompt.py` & `steamship-langchain-0.0.9/examples/chatbot/server/prompt.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/chatbot/server/steamship.json` & `steamship-langchain-0.0.9/examples/chatbot/server/steamship.json`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/greeting/README.md` & `steamship-langchain-0.0.9/examples/greeting/README.md`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/greeting/client/client.py` & `steamship-langchain-0.0.9/examples/greeting/client/client.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/greeting/server/api.py` & `steamship-langchain-0.0.9/examples/greeting/server/api.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/greeting/server/steamship.json` & `steamship-langchain-0.0.9/examples/greeting/server/steamship.json`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/qa_with_sources/README.md` & `steamship-langchain-0.0.9/examples/qa_with_sources/README.md`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/qa_with_sources/client/client.py` & `steamship-langchain-0.0.9/examples/qa_with_sources/client/client.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/qa_with_sources/server/api.py` & `steamship-langchain-0.0.9/examples/qa_with_sources/server/api.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/qa_with_sources/server/steamship.json` & `steamship-langchain-0.0.9/examples/qa_with_sources/server/steamship.json`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/qa_with_sources/state-of-the-union-2022.txt` & `steamship-langchain-0.0.9/examples/qa_with_sources/state-of-the-union-2022.txt`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/self-ask-with-search/README.md` & `steamship-langchain-0.0.9/examples/self-ask-with-search/README.md`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/self-ask-with-search/client/client.py` & `steamship-langchain-0.0.9/examples/self-ask-with-search/client/client.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/self-ask-with-search/server/api.py` & `steamship-langchain-0.0.9/examples/self-ask-with-search/server/api.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/self-ask-with-search/server/steamship.json` & `steamship-langchain-0.0.9/examples/self-ask-with-search/server/steamship.json`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/summarize-audio/README.md` & `steamship-langchain-0.0.9/examples/summarize-audio/README.md`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/summarize-audio/client/client.py` & `steamship-langchain-0.0.9/examples/summarize-audio/client/client.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/summarize-audio/server/api.py` & `steamship-langchain-0.0.9/examples/summarize-audio/server/api.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/examples/summarize-audio/server/steamship.json` & `steamship-langchain-0.0.9/examples/summarize-audio/server/steamship.json`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/pyproject.toml` & `steamship-langchain-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/requirements.dev.txt` & `steamship-langchain-0.0.9/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/src/steamship_langchain/cache/cache.py` & `steamship-langchain-0.0.9/src/steamship_langchain/cache/cache.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/src/steamship_langchain/llms/openai.py` & `steamship-langchain-0.0.9/src/steamship_langchain/llms/openai.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     client: Steamship
     plugin_handle: str = Field(default="gpt-3", const=True)
     batch_size: int = Field(default=20)
     temperature: float = 0.8
     max_words: int = 256
     n: int = 1
     best_of: int = 1
+    batch_task_timeout_seconds: int = 10 * 60  # 10 minute limit on generation tasks
 
     @property
     def _llm_type(self) -> str:
         return f"steamship-{self.plugin_handle}"
 
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
@@ -102,15 +103,17 @@
         for prompt in prompts:
             blocks.append(Block(text=prompt))
 
         generations = []
         try:
             prompt_file = File.create(client=self.client, blocks=blocks)
             task = llm_plugin.tag(doc=prompt_file)
-            task.wait()  # TODO(douglas-reid): put in timeout, based on configuration
+            # the llm_plugin handles retries and backoff. this wait()
+            # will allow for that to happen.
+            task.wait(max_timeout_s=self.batch_task_timeout_seconds)
             generation_file = task.output.file
 
             for text_block in generation_file.blocks:
                 for block_tag in text_block.tags:
                     if block_tag.kind == TagKind.GENERATION:
                         generation = block_tag.value[TagValueKey.STRING_VALUE]
                         generations.append(Generation(generation))
```

### Comparing `steamship-langchain-0.0.8/src/steamship_langchain/memory/conversation_memory.py` & `steamship-langchain-0.0.9/src/steamship_langchain/memory/conversation_memory.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/src/steamship_langchain/tools/search_tool.py` & `steamship-langchain-0.0.9/src/steamship_langchain/tools/search_tool.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/src/steamship_langchain.egg-info/PKG-INFO` & `steamship-langchain-0.0.9/src/steamship_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamship-langchain
-Version: 0.0.8
+Version: 0.0.9
 Summary: The fastest way to deploy a production langchain API.
 Project-URL: Homepage, https://steamship.com/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # Steamship Python Client Library For LangChain (🦜️🔗)
@@ -32,15 +32,15 @@
 ```commandline
 pip install steamship-langchain
 ```
 
 ## Adapters
 
 Initial support is offered for the following (with more to follow soon):
-- LLMS
+- LLMs
   - An adapter is provided for Steamship's OpenAI integration (`steamship_langchain.llms.OpenAI`)
   - An adapter is provided for *caching* LLM calls, via Steamship's Key-Value store (`SteamshipCache`) 
 - Tools
   - Search:
     - An adapter is provided for Steamship's SERPAPI integration (`SteamshipSERP`)
 - Memory
   - Two adapters that provide persistent conversation memory:
```

### Comparing `steamship-langchain-0.0.8/src/steamship_langchain.egg-info/SOURCES.txt` & `steamship-langchain-0.0.9/src/steamship_langchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/tests/cache/test_cache.py` & `steamship-langchain-0.0.9/tests/cache/test_cache.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/tests/llms/test_openai.py` & `steamship-langchain-0.0.9/tests/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/tests/memory/test_conversation_memory.py` & `steamship-langchain-0.0.9/tests/memory/test_conversation_memory.py`

 * *Files identical despite different names*

### Comparing `steamship-langchain-0.0.8/tests/utils/fixtures.py` & `steamship-langchain-0.0.9/tests/utils/fixtures.py`

 * *Files identical despite different names*

