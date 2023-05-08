# Comparing `tmp/fschat-0.2.6.tar.gz` & `tmp/fschat-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.6.tar", last modified: Mon May  8 09:50:28 2023, max compression
+gzip compressed data, was "fschat-0.2.7.tar", last modified: Mon May  8 14:34:56 2023, max compression
```

## Comparing `fschat-0.2.6.tar` & `fschat-0.2.7.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 09:50:28.063382 fschat-0.2.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15049 2023-05-08 09:41:45.000000 fschat-0.2.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.055382 fschat-0.2.6/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2023-05-08 09:42:14.000000 fschat-0.2.6/fastchat/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.055382 fschat-0.2.6/fastchat/client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/client/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/client/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14198 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.055382 fschat-0.2.6/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3502 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.059382 fschat-0.2.6/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3017 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.059382 fschat-0.2.6/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:14:01.000000 fschat-0.2.6/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-05-08 06:48:06.000000 fschat-0.2.6/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/model/apply_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/model/chatglm_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/make_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14980 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/model_adapter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2772 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/model_registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/model/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      950 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/rwkv_model.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.059382 fschat-0.2.6/fastchat/protocol/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1655 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/protocol/chat_completion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10203 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/api_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11456 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5497 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11809 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14370 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_block_arena_anony.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14209 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_block_arena_named.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20281 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6239 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_web_server_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7980 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10911 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/model_worker.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fastchat/serve/monitor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5413 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/basic_stats.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5116 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/clean_battle_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8275 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/elo_analysis.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6919 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/monitor.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2401 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8670 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/train/train.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14619 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/train/train_flant5.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6393 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-05-08 09:42:47.000000 fschat-0.2.6/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-08 09:50:28.063382 fschat-0.2.6/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.7/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 14:34:56.836340 fschat-0.2.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15049 2023-05-08 10:26:52.000000 fschat-0.2.7/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-05-08 14:31:24.000000 fschat-0.2.7/fastchat/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4067 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/client/openai_api_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14198 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-05-05 11:09:54.000000 fschat-0.2.7/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-05-05 11:09:54.000000 fschat-0.2.7/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-05 11:09:54.000000 fschat-0.2.7/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.7/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.7/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3447 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.828340 fschat-0.2.7/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3023 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-05-08 06:48:06.000000 fschat-0.2.7/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/model/apply_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1222 2023-05-08 14:31:24.000000 fschat-0.2.7/fastchat/model/chatglm_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/make_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14980 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/model_adapter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2772 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/model_registry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/model/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      996 2023-05-08 14:31:24.000000 fschat-0.2.7/fastchat/model/rwkv_model.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/protocol/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/protocol/openai_api_protocol.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11456 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5497 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11809 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14370 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/gradio_block_arena_anony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14209 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/gradio_block_arena_named.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20317 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6239 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/gradio_web_server_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1796 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7980 2023-05-08 14:15:06.000000 fschat-0.2.7/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10911 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/model_worker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.832340 fschat-0.2.7/fastchat/serve/monitor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5413 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/basic_stats.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5116 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/clean_battle_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8275 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/elo_analysis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6919 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/serve/monitor/monitor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12369 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/openai_api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.7/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2442 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8670 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/train/train.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14619 2023-05-08 10:26:52.000000 fschat-0.2.7/fastchat/train/train_flant5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.7/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7107 2023-05-08 13:48:50.000000 fschat-0.2.7/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2047 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-08 14:34:56.000000 fschat-0.2.7/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-05-08 14:31:24.000000 fschat-0.2.7/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-08 14:34:56.836340 fschat-0.2.7/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 14:34:56.836340 fschat-0.2.7/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-05-08 13:54:24.000000 fschat-0.2.7/tests/test_openai_client.py
```

### Comparing `fschat-0.2.6/LICENSE` & `fschat-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/PKG-INFO` & `fschat-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.6
+Version: 0.2.7
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.6 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.7 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
 [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
```

### Comparing `fschat-0.2.6/README.md` & `fschat-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/client/api.py` & `fschat-0.2.7/fastchat/client/openai_api_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,122 @@
-from typing import Dict, List, Optional
 import asyncio
+import json
 import os
+from typing import AsyncGenerator, Dict, List, Optional, Generator, Union
 
 import httpx
-from fastchat.protocol.chat_completion import (
+
+from fastchat.utils import iter_over_async
+from fastchat.protocol.openai_api_protocol import (
     ChatCompletionRequest,
     ChatCompletionResponse,
+    ChatCompletionStreamResponse,
 )
 
-_BASE_URL = "http://localhost:8000"
 
-if os.environ.get("FASTCHAT_BASE_URL"):
-    _BASE_URL = os.environ.get("FASTCHAT_BASE_URL")
+_BASE_URL = os.environ.get("FASTCHAT_API_BASE_URL", "http://localhost:8000")
 
 
 def set_baseurl(base_url: str):
     global _BASE_URL
     _BASE_URL = base_url
 
 
 class ChatCompletionClient:
     def __init__(self, base_url: str):
         self.base_url = base_url
 
     async def request_completion(
         self, request: ChatCompletionRequest, timeout: Optional[float] = None
     ) -> ChatCompletionResponse:
+        """
+        Create chat completion request
+        :param request: The request data
+        :param timeout: The timeout of the request
+        :returns: Compleation stream
+        """
         async with httpx.AsyncClient() as client:
             response = await client.post(
                 f"{self.base_url}/v1/chat/completions",
                 json=request.dict(),
                 timeout=timeout,
             )
             response.raise_for_status()
             return ChatCompletionResponse.parse_obj(response.json())
 
+    async def request_completion_stream(
+        self, request: ChatCompletionRequest, timeout: Optional[float] = None
+    ) -> AsyncGenerator:
+        """
+        Create chat completion as a stream
+        :param request: The request data
+        :param timeout: The timeout of the request
+        :returns: Compleation stream
+        """
+        async with httpx.AsyncClient() as client:
+            async with client.stream(
+                "POST",
+                f"{self.base_url}/v1/chat/completions",
+                json=request.dict(),
+                timeout=timeout,
+            ) as response:
+                async for chunk in response.aiter_text():
+                    if not chunk:
+                        continue
+                    for line in chunk.split("\n"):
+                        if not line:
+                            continue
+                        yield ChatCompletionStreamResponse.parse_obj(json.loads(line))
+
 
 class ChatCompletion:
     OBJECT_NAME = "chat.completions"
 
     @classmethod
-    def create(cls, *args, **kwargs) -> ChatCompletionResponse:
+    def create(cls, *args, **kwargs) -> Union[ChatCompletionResponse, Generator]:
         """Creates a new chat completion for the provided messages and parameters.
 
         See `acreate` for more details.
         """
-        return asyncio.run(cls.acreate(*args, **kwargs))
+        if kwargs.get("stream"):
+            try:
+                loop = asyncio.get_event_loop()
+            except RuntimeError as e:
+                if str(e).startswith('There is no current event loop in thread'):
+                    loop = asyncio.new_event_loop()
+                    asyncio.set_event_loop(loop)
+                else:
+                    raise
+            async_gen = cls.acreate(*args, **kwargs)
+            async_gen_after_start = loop.run_until_complete(async_gen)
+            sync_gen = iter_over_async(async_gen_after_start, loop)
+            return sync_gen
+        else:
+            return asyncio.run(cls.acreate(*args, **kwargs))
 
     @classmethod
     async def acreate(
         cls,
         model: str,
         messages: List[Dict[str, str]],
         temperature: Optional[float] = 0.7,
         n: int = 1,
         max_tokens: Optional[int] = None,
         stop: Optional[str] = None,
         timeout: Optional[float] = None,
-    ) -> ChatCompletionResponse:
+        stream: Optional[bool] = False,
+    ):
         """Creates a new chat completion for the provided messages and parameters."""
         request = ChatCompletionRequest(
             model=model,
             messages=messages,
             temperature=temperature,
             n=n,
             max_tokens=max_tokens,
             stop=stop,
+            stream=stream,
         )
         client = ChatCompletionClient(_BASE_URL)
-        response = await client.request_completion(request, timeout=timeout)
-        return response
+        if stream:
+            return client.request_completion_stream(request, timeout=timeout)
+        else:
+            return await client.request_completion(request, timeout=timeout)
```

### Comparing `fschat-0.2.6/fastchat/conversation.py` & `fschat-0.2.7/fastchat/conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/data/clean_sharegpt.py` & `fschat-0.2.7/fastchat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/data/hardcoded_questions.py` & `fschat-0.2.7/fastchat/data/hardcoded_questions.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/data/inspect.py` & `fschat-0.2.7/fastchat/data/inspect.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/data/merge.py` & `fschat-0.2.7/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/data/optional_clean.py` & `fschat-0.2.7/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/data/sample.py` & `fschat-0.2.7/fastchat/data/sample.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/data/split_long_conversation.py` & `fschat-0.2.7/fastchat/data/split_long_conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from concurrent.futures import ProcessPoolExecutor
 import json
 from typing import Dict, Sequence, Optional
 
 import transformers
 from tqdm import tqdm
 
-from fastchat import conversation as conversation_lib
-
 
 def make_sample(sample, start_idx, end_idx):
     assert (end_idx - start_idx) % 2 == 0
     return {
         "id": sample["id"] + "_" + str(start_idx),
         "conversations": sample["conversations"][start_idx:end_idx],
     }
```

### Comparing `fschat-0.2.6/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.7/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.7/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/eval/get_model_answer.py` & `fschat-0.2.7/fastchat/eval/get_model_answer.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 import os
 import json
 from tqdm import tqdm
 import shortuuid
 import ray
 
-from fastchat import get_conversation_template
+from fastchat.model import get_conversation_template
 
 
 def run_eval(model_path, model_id, question_file, answer_file, num_gpus):
     # split question file into num_gpus files
     ques_jsons = []
     with open(os.path.expanduser(question_file), "r") as ques_file:
         for line in ques_file:
```

### Comparing `fschat-0.2.6/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.7/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/apply_delta.py` & `fschat-0.2.7/fastchat/model/apply_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/apply_lora.py` & `fschat-0.2.7/fastchat/model/apply_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/compression.py` & `fschat-0.2.7/fastchat/model/compression.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/convert_fp16.py` & `fschat-0.2.7/fastchat/model/convert_fp16.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/make_delta.py` & `fschat-0.2.7/fastchat/model/make_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/model_adapter.py` & `fschat-0.2.7/fastchat/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/model_registry.py` & `fschat-0.2.7/fastchat/model/model_registry.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/model/monkey_patch_non_inplace.py` & `fschat-0.2.7/fastchat/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/protocol/chat_completion.py` & `fschat-0.2.7/fastchat/protocol/openai_api_protocol.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import time
 
 import shortuuid
 from pydantic import BaseModel, Field
 
 
 class ChatCompletionRequest(BaseModel):
-    # TODO: support streaming, stop with a list of text etc.
+    # TODO: support stop with a list of text etc.
     model: str
     messages: List[Dict[str, str]]
     temperature: Optional[float] = 0.7
     n: int = 1
     max_tokens: Optional[int] = None
     stop: Optional[str] = None
+    stream: Optional[bool] = None
 
 
 class ChatMessage(BaseModel):
     role: str
     content: str
 
 
@@ -27,28 +28,47 @@
     finish_reason: str
 
 
 class ChatCompletionResponse(BaseModel):
     id: str = Field(default_factory=shortuuid.random)
     object: str = "chat.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
+    model: str
     choices: List[ChatCompletionResponseChoice]
-    usage: Optional[Dict[str, int]] = None
+    usage: Dict[str, int]
+
+
+class DeltaMessage(BaseModel):
+    content: str
+
+
+class ChatCompletionResponseStreamChoice(BaseModel):
+    index: int
+    delta: DeltaMessage
+    finish_reason: Optional[str]
+
+
+class ChatCompletionStreamResponse(BaseModel):
+    id: str = Field(default_factory=shortuuid.random)
+    object: str = "chat.completion.chunk"
+    created: int = Field(default_factory=lambda: int(time.time()))
+    model: str
+    choices: List[ChatCompletionResponseStreamChoice]
 
 
 class EmbeddingsRequest(BaseModel):
     model: str
     input: str
 
 
 class EmbeddingsResponse(BaseModel):
-    object: str = "lists"
+    object: str = "list"
     data: List[Dict[str, Any]]
     model: str
-    usage: Optional[Dict[str, int]] = None
+    usage: Dict[str, int]
 
 
 class CompletionRequest(BaseModel):
     model: str
     prompt: str
     suffix: Optional[str] = None
     temperature: Optional[float] = 0.7
@@ -62,8 +82,8 @@
 
 class CompletionResponse(BaseModel):
     id: str = Field(default_factory=shortuuid.random)
     object: str = "text_completion"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
     choices: List[Dict[str, Any]]
-    usage: Optional[Dict[str, int]] = None
+    usage: Dict[str, int]
```

### Comparing `fschat-0.2.6/fastchat/serve/api_server.py` & `fschat-0.2.7/fastchat/serve/openai_api_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 """A server that provides OpenAI-compatible RESTful APIs. It supports:
 
 - Chat Completions. (Reference: https://platform.openai.com/docs/api-reference/chat)
 - Completions. (Reference: https://platform.openai.com/docs/api-reference/completions)
 - Embeddings. (Reference: https://platform.openai.com/docs/api-reference/embeddings)
 
 Usage:
-python3 -m fastchat.serve.api_server
+python3 -m fastchat.serve.openai_api_server
 """
 import asyncio
 import argparse
+import asyncio
 import json
 import logging
+import os
 from typing import Union, Dict, List, Any
 
 import fastapi
 from fastapi.middleware.cors import CORSMiddleware
+from fastapi.responses import StreamingResponse
 import httpx
 import uvicorn
 from pydantic import BaseSettings
 
-from fastchat.protocol.chat_completion import (
+from fastchat.constants import WORKER_API_TIMEOUT
+from fastchat.model.model_adapter import get_conversation_template
+from fastchat.protocol.openai_api_protocol import (
     ChatCompletionRequest,
     ChatCompletionResponse,
+    ChatCompletionStreamResponse,
     ChatMessage,
     ChatCompletionResponseChoice,
+    ChatCompletionResponseStreamChoice,
+    DeltaMessage,
     CompletionRequest,
     CompletionResponse,
     EmbeddingsRequest,
     EmbeddingsResponse,
 )
-from fastchat.model.model_adapter import get_conversation_template
 
 logger = logging.getLogger(__name__)
 
 
 class AppSettings(BaseSettings):
     # The address of the model controller.
     controller_address: str = "http://localhost:21001"
@@ -49,31 +56,36 @@
 async def show_available_models():
     controller_address = app_settings.controller_address
     async with httpx.AsyncClient() as client:
         ret = await client.post(controller_address + "/refresh_all_workers")
         ret = await client.post(controller_address + "/list_models")
     models = ret.json()["models"]
     models.sort()
-    return {"data": [{"id": m} for m in models], "object": "list"}
+    return {"data": [{"id": m, "object": "model"} for m in models],
+            "object": "list"}
 
 
 @app.post("/v1/chat/completions")
 async def create_chat_completion(request: ChatCompletionRequest):
     """Creates a completion for the chat message"""
     gen_params = get_gen_params(
         request.model,
         request.messages,
         temperature=request.temperature,
         max_tokens=request.max_tokens,
         echo=False,
         stop=request.stop,
     )
+    if request.stream:
+        response_stream = chat_completion_stream(
+            request.model, gen_params, request.n)
+        return StreamingResponse(response_stream, media_type="text/event-stream")
 
+    # TODO: batch the requests
     choices = []
-    # TODO: batch the requests. maybe not necessary if using CacheFlow worker
     chat_completions = []
     for i in range(request.n):
         content = asyncio.create_task(chat_completion(request.model, gen_params))
         chat_completions.append(content)
 
     for i, content_task in enumerate(chat_completions):
         content = await content_task
@@ -83,20 +95,20 @@
                 message=ChatMessage(role="assistant", content=content),
                 # TODO: support other finish_reason
                 finish_reason="stop",
             )
         )
 
     # TODO: support usage field
-    # "usage": {
-    #     "prompt_tokens": 9,
-    #     "completion_tokens": 12,
-    #     "total_tokens": 21
-    # }
-    return ChatCompletionResponse(choices=choices)
+    usage = {
+        "prompt_tokens": -1,
+        "completion_tokens": -1,
+        "total_tokens": -1,
+    }
+    return ChatCompletionResponse(model=request.model, choices=choices, usage=usage)
 
 
 def get_gen_params(
     model_name: str,
     messages: List[Dict[str, str]],
     *,
     temperature: float,
@@ -138,35 +150,96 @@
         "stop": conv.stop_str,
         "stop_token_ids": conv.stop_token_ids,
     }
     logger.debug(f"==== request ====\n{gen_params}")
     return gen_params
 
 
-async def chat_completion(model_name: str, gen_params: Dict[str, Any]):
+async def _get_worker_address(model_name: str, client: httpx.AsyncClient) -> str:
+    """
+    Get worker address based on the requested model
+
+    :param model_name: The worker's model name
+    :param client: The httpx client to use
+    :return: Worker address from the controller
+    :raises: :class:`ValueError`: No available worker for requested model
+    """
     controller_address = app_settings.controller_address
+
+    ret = await client.post(
+        controller_address + "/get_worker_address", json={"model": model_name}
+    )
+    worker_addr = ret.json()["address"]
+    # No available worker
+    if worker_addr == "":
+        raise ValueError(f"No available worker for {model_name}")
+
+    logger.debug(f"model_name: {model_name}, worker_addr: {worker_addr}")
+    return worker_addr
+
+
+async def chat_completion_stream(model_name: str, gen_params: Dict[str, Any], n: int):
     async with httpx.AsyncClient() as client:
-        ret = await client.post(
-            controller_address + "/get_worker_address", json={"model": model_name}
-        )
-        worker_addr = ret.json()["address"]
-        # No available worker
-        if worker_addr == "":
-            raise ValueError(f"No available worker for {model_name}")
+        worker_addr = await _get_worker_address(model_name, client)
+        delimiter = b"\0"
+ 
+        for idx in range(n):
+            delta_position = 0
+            response = ChatCompletionStreamResponse(
+                model=model_name,
+                choices=[
+                    ChatCompletionResponseStreamChoice(
+                        index=idx,
+                        delta=DeltaMessage(content=""),
+                        finish_reason=None,
+                    )
+                ]
+            )
+
+            async with client.stream(
+                "POST",
+                worker_addr + "/worker_generate_stream",
+                headers=headers,
+                json=gen_params,
+                timeout=WORKER_API_TIMEOUT,
+            ) as post_response:
+                # TODO: begins with a single delta containing the role and a null finish reason
+                async for raw_chunk in post_response.aiter_raw():
+                    for chunk in raw_chunk.split(delimiter):
+                        if not chunk:
+                            continue
+                        data = json.loads(chunk.decode())
+                        if data["error_code"] == 0:
+                            last_delta_position = delta_position
+                            output = data["text"].strip()
+                            delta_position = len(output)
+                            delta_diff = delta_position - last_delta_position
+                            if delta_diff > 0:
+                                delta = output[last_delta_position:]
+                                response.choices[0].delta.content = delta
+                                yield json.dumps(response.dict())
+
+                # Streaming the finishing token
+                response.choices[0].delta.content = ""
+                response.choices[0].finish_reason = "stop"
+                yield json.dumps(response.dict())
 
-        logger.debug(f"model_name: {model_name}, worker_addr: {worker_addr}")
+
+async def chat_completion(model_name: str, gen_params: Dict[str, Any]):
+    async with httpx.AsyncClient() as client:
+        worker_addr = await _get_worker_address(model_name, client)
 
         output = ""
         delimiter = b"\0"
         async with client.stream(
             "POST",
             worker_addr + "/worker_generate_stream",
             headers=headers,
             json=gen_params,
-            timeout=20,
+            timeout=WORKER_API_TIMEOUT,
         ) as response:
             content = await response.aread()
 
         for chunk in content.split(delimiter):
             if not chunk:
                 continue
             data = json.loads(chunk.decode())
@@ -213,47 +286,35 @@
         },
     )
 
 
 async def generate_completion(payload: Dict[str, Any]):
     controller_address = app_settings.controller_address
     async with httpx.AsyncClient() as client:
-        ret = await client.post(
-            controller_address + "/get_worker_address", json={"model": payload["model"]}
-        )
-        worker_addr = ret.json()["address"]
-        # No available worker
-        if worker_addr == "":
-            raise ValueError(f"No available worker for {payload['model']}")
-
-        logger.debug(f"model_name: {payload['model']}, worker_addr: {worker_addr}")
+        worker_addr = await _get_worker_address(payload["model"], client)
 
         response = await client.post(
             worker_addr + "/worker_generate_completion",
             headers=headers,
             json=payload,
-            timeout=20,
+            timeout=WORKER_API_TIMEOUT,
         )
         completion = response.json()
         return completion
 
 
 @app.post("/v1/create_embeddings")
 async def create_embeddings(request: EmbeddingsRequest):
     """Creates embeddings for the text"""
+    payload = {
+        "model": request.model,
+        "input": request.input,
+    }
 
-    def generate_embeddings_payload(model_name: str, input: str):
-        payload = {
-            "model": model_name,
-            "input": input,
-        }
-        return payload
-
-    embeddings_payload = generate_embeddings_payload(request.model, request.input)
-    embedding = await get_embedding(embeddings_payload)
+    embedding = await get_embedding(payload)
     embedding = json.loads(embedding)
     data = [{"object": "embedding", "embedding": embedding["embedding"], "index": 0}]
     return EmbeddingsResponse(
         data=data,
         model=request.model,
         usage={
             "prompt_tokens": embedding["token_num"],
@@ -262,36 +323,29 @@
     )
 
 
 async def get_embedding(payload: Dict[str, Any]):
     controller_address = app_settings.controller_address
     model_name = payload["model"]
     async with httpx.AsyncClient() as client:
-        ret = await client.post(
-            controller_address + "/get_worker_address", json={"model": model_name}
-        )
-        worker_addr = ret.json()["address"]
-        if worker_addr == "":
-            raise ValueError(f"No available worker for {model_name}")
-
-        logger.debug(f"model_name: {model_name}, worker_addr: {worker_addr}")
+        worker_addr = await _get_worker_address(model_name, client)
 
         response = await client.post(
             worker_addr + "/worker_get_embeddings",
             headers=headers,
             json=payload,
-            timeout=20,
+            timeout=WORKER_API_TIMEOUT,
         )
         embedding = response.json()
         return embedding
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
-        description="FastChat ChatGPT-compatible Restful API server."
+        description="FastChat ChatGPT-Compatible RESTful API server."
     )
     parser.add_argument("--host", type=str, default="localhost", help="host name")
     parser.add_argument("--port", type=int, default=8000, help="port number")
     parser.add_argument(
         "--controller-address", type=str, default="http://localhost:21001"
     )
     parser.add_argument(
```

### Comparing `fschat-0.2.6/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.7/fastchat/serve/cacheflow_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/cli.py` & `fschat-0.2.7/fastchat/serve/cli.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/controller.py` & `fschat-0.2.7/fastchat/serve/controller.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/gradio_block_arena_anony.py` & `fschat-0.2.7/fastchat/serve/gradio_block_arena_anony.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/gradio_block_arena_named.py` & `fschat-0.2.7/fastchat/serve/gradio_block_arena_named.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/gradio_css.py` & `fschat-0.2.7/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/gradio_patch.py` & `fschat-0.2.7/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/gradio_web_server.py` & `fschat-0.2.7/fastchat/serve/gradio_web_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 import uuid
 
 import gradio as gr
 import requests
 
 from fastchat.conversation import SeparatorStyle
-from fastchat.constants import LOGDIR
+from fastchat.constants import LOGDIR, WORKER_API_TIMEOUT
 from fastchat.model.model_adapter import get_conversation_template
 from fastchat.model.model_registry import model_info
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_css import code_highlight_css
 from fastchat.utils import (
     build_logger,
     server_error_msg,
@@ -245,15 +245,15 @@
 
     # Stream output
     response = requests.post(
         worker_addr + "/worker_generate_stream",
         headers=headers,
         json=gen_params,
         stream=True,
-        timeout=20,
+        timeout=WORKER_API_TIMEOUT,
     )
     for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
         if chunk:
             data = json.loads(chunk.decode())
             yield data
```

### Comparing `fschat-0.2.6/fastchat/serve/gradio_web_server_multi.py` & `fschat-0.2.7/fastchat/serve/gradio_web_server_multi.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/huggingface_api.py` & `fschat-0.2.7/fastchat/serve/huggingface_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 import argparse
 import json
 
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
-from fastchat import load_model, get_conversation_template, add_model_args
+from fastchat.model import load_model, get_conversation_template, add_model_args
 
 
 @torch.inference_mode()
 def main(args):
     model, tokenizer = load_model(
         args.model_path,
         args.device,
```

### Comparing `fschat-0.2.6/fastchat/serve/inference.py` & `fschat-0.2.7/fastchat/serve/inference.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/model_worker.py` & `fschat-0.2.7/fastchat/serve/model_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/monitor/basic_stats.py` & `fschat-0.2.7/fastchat/serve/monitor/basic_stats.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/monitor/clean_battle_data.py` & `fschat-0.2.7/fastchat/serve/monitor/clean_battle_data.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/monitor/elo_analysis.py` & `fschat-0.2.7/fastchat/serve/monitor/elo_analysis.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/monitor/monitor.py` & `fschat-0.2.7/fastchat/serve/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/register_worker.py` & `fschat-0.2.7/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/serve/test_message.py` & `fschat-0.2.7/fastchat/serve/test_message.py`

 * *Files 16% similar despite different names*

```diff
@@ -48,21 +48,22 @@
         worker_addr + "/worker_generate_stream",
         headers=headers,
         json=gen_params,
         stream=True,
     )
 
     print(f"{conv.roles[0]}: {args.message}")
-    for chunk in response.iter_lines(
-        chunk_size=8192, decode_unicode=False, delimiter=b"\0"
-    ):
+    print(f"{conv.roles[1]}: ", end="")
+    prev = 0
+    for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
         if chunk:
-            data = json.loads(chunk.decode("utf-8"))
+            data = json.loads(chunk.decode())
             output = data["text"].strip()
-            print(f"{conv.roles[1]}: {output}", end="\r")
+            print(output[prev:], end="", flush=True)
+            prev = len(output)
     print("")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--controller-address", type=str, default="http://localhost:21001"
```

### Comparing `fschat-0.2.6/fastchat/serve/test_throughput.py` & `fschat-0.2.7/fastchat/serve/test_throughput.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.7/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/train/train.py` & `fschat-0.2.7/fastchat/train/train.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/train/train_flant5.py` & `fschat-0.2.7/fastchat/train/train_flant5.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/train/train_lora.py` & `fschat-0.2.7/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.6/fastchat/utils.py` & `fschat-0.2.7/fastchat/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from asyncio import AbstractEventLoop
+import json
 import logging
 import logging.handlers
 import os
+import platform
 import sys
-import json
+from typing import AsyncGenerator, Generator
 import warnings
-import platform
 
 import requests
 import torch
 
 from fastchat.constants import LOGDIR
 
 server_error_msg = (
@@ -193,7 +195,33 @@
 function() {
     const params = new URLSearchParams(window.location.search);
     url_params = Object.fromEntries(params);
     console.log("url_params", url_params);
     return url_params;
     }
 """
+
+
+def iter_over_async(
+    async_gen: AsyncGenerator, event_loop: AbstractEventLoop
+) -> Generator:
+    """
+    Convert async generator to sync generator
+
+    :param async_gen: the AsyncGenerator to convert
+    :param event_loop: the event loop to run on
+    :returns: Sync generator
+    """
+    ait = async_gen.__aiter__()
+
+    async def get_next():
+        try:
+            obj = await ait.__anext__()
+            return False, obj
+        except StopAsyncIteration:
+            return True, None
+
+    while True:
+        done, obj = event_loop.run_until_complete(get_next())
+        if done:
+            break
+        yield obj
```

### Comparing `fschat-0.2.6/fschat.egg-info/PKG-INFO` & `fschat-0.2.7/fschat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.6
+Version: 0.2.7
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.6 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.7 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
 [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
```

### Comparing `fschat-0.2.6/fschat.egg-info/SOURCES.txt` & `fschat-0.2.7/fschat.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 README.md
 pyproject.toml
 fastchat/__init__.py
 fastchat/constants.py
 fastchat/conversation.py
 fastchat/utils.py
 fastchat/client/__init__.py
-fastchat/client/api.py
-fastchat/client/test_client.py
+fastchat/client/openai_api_client.py
 fastchat/data/__init__.py
 fastchat/data/clean_sharegpt.py
 fastchat/data/hardcoded_questions.py
 fastchat/data/inspect.py
 fastchat/data/merge.py
 fastchat/data/optional_clean.py
 fastchat/data/pretty_json.py
@@ -28,29 +27,29 @@
 fastchat/model/compression.py
 fastchat/model/convert_fp16.py
 fastchat/model/make_delta.py
 fastchat/model/model_adapter.py
 fastchat/model/model_registry.py
 fastchat/model/monkey_patch_non_inplace.py
 fastchat/model/rwkv_model.py
-fastchat/protocol/chat_completion.py
+fastchat/protocol/openai_api_protocol.py
 fastchat/serve/__init__.py
-fastchat/serve/api_server.py
 fastchat/serve/cacheflow_worker.py
 fastchat/serve/cli.py
 fastchat/serve/controller.py
 fastchat/serve/gradio_block_arena_anony.py
 fastchat/serve/gradio_block_arena_named.py
 fastchat/serve/gradio_css.py
 fastchat/serve/gradio_patch.py
 fastchat/serve/gradio_web_server.py
 fastchat/serve/gradio_web_server_multi.py
 fastchat/serve/huggingface_api.py
 fastchat/serve/inference.py
 fastchat/serve/model_worker.py
+fastchat/serve/openai_api_server.py
 fastchat/serve/register_worker.py
 fastchat/serve/test_message.py
 fastchat/serve/test_throughput.py
 fastchat/serve/monitor/basic_stats.py
 fastchat/serve/monitor/clean_battle_data.py
 fastchat/serve/monitor/elo_analysis.py
 fastchat/serve/monitor/monitor.py
@@ -59,8 +58,9 @@
 fastchat/train/train_flant5.py
 fastchat/train/train_lora.py
 fastchat/train/train_mem.py
 fschat.egg-info/PKG-INFO
 fschat.egg-info/SOURCES.txt
 fschat.egg-info/dependency_links.txt
 fschat.egg-info/requires.txt
-fschat.egg-info/top_level.txt
+fschat.egg-info/top_level.txt
+tests/test_openai_client.py
```

### Comparing `fschat-0.2.6/pyproject.toml` & `fschat-0.2.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.6"
+version = "0.2.7"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
     "accelerate", "fastapi", "gradio==3.23", "httpx", "markdown2[all]", "nh3", "numpy",
     "prompt_toolkit>=3.0.0", "pydantic", "requests", "rich>=10.0.0", "sentencepiece",
     "shortuuid", "shortuuid", "tokenizers>=0.12.1", "torch",
-    "transformers>=4.28.0,<4.29.0", "uvicorn", "wandb"
+    "transformers>=4.28.0,<4.29.0", "uvicorn", "wandb",
 ]
 
 [project.optional-dependencies]
 dev = ["black==23.3.0", "pylint==2.8.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/lm-sys/fastchat"
```

