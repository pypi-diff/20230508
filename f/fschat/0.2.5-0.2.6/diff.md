# Comparing `tmp/fschat-0.2.5.tar.gz` & `tmp/fschat-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fschat-0.2.5.tar", last modified: Sun Apr 30 01:50:56 2023, max compression
+gzip compressed data, was "fschat-0.2.6.tar", last modified: Mon May  8 09:50:28 2023, max compression
```

## Comparing `fschat-0.2.5.tar` & `fschat-0.2.6.tar`

### file list

```diff
@@ -1,212 +1,79 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.209236 fschat-0.2.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15090 2023-04-30 01:50:56.205236 fschat-0.2.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14596 2023-04-30 01:50:41.000000 fschat-0.2.5/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2023-04-30 01:50:41.000000 fschat-0.2.5/fastchat/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/client/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/client/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/client/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/client/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10621 2023-04-30 01:40:10.000000 fschat-0.2.5/fastchat/conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/data/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/data/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1946 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/alpaca-converter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/clean_sharegpt.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/hardcoded_questions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/inspect.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/data/merge.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/optional_clean.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/data/pretty_json.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/data/sample.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3502 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/data/split_long_conversation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/eval/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/eval/eval_gpt_review.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/eval/generate_webpage_data_from_table.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3036 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/eval/get_model_answer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/eval/qa_baseline_gpt35.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:14:01.000000 fschat-0.2.5/fastchat/model/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/model/apply_delta.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/model/apply_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/model/convert_fp16.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1849 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/model/make_delta.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.197236 fschat-0.2.5/fastchat/protocol/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      855 2023-04-30 00:44:53.000000 fschat-0.2.5/fastchat/protocol/chat_completion.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.201236 fschat-0.2.5/fastchat/serve/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/serve/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6165 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11455 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/cacheflow_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5330 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6921 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/compression.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10058 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/controller.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13439 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_block_arena_anony.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13063 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_block_arena_named.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_css.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17943 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/gradio_web_server.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5205 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/gradio_web_server_multi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1877 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/huggingface_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13703 2023-04-30 01:40:10.000000 fschat-0.2.5/fastchat/serve/inference.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7474 2023-04-30 01:40:08.000000 fschat-0.2.5/fastchat/serve/model_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/monkey_patch_non_inplace.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.5/fastchat/serve/register_worker.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      930 2023-04-30 01:40:10.000000 fschat-0.2.5/fastchat/serve/rwkv_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/serve_chatglm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2430 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/test_message.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/serve/test_throughput.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.201236 fschat-0.2.5/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/llama_flash_attn_monkey_patch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8637 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14838 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train_flant5.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train_lora.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/train/train_mem.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5407 2023-04-30 00:47:10.000000 fschat-0.2.5/fastchat/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/fschat.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15090 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3424 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       27 2023-04-30 01:50:56.000000 fschat-0.2.5/fschat.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1143 2023-04-30 01:50:41.000000 fschat-0.2.5/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-30 01:50:56.209236 fschat-0.2.5/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/latest-run/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/latest-run/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8667 2023-04-29 11:02:46.000000 fschat-0.2.5/wandb/latest-run/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8305 2023-04-23 12:16:11.000000 fschat-0.2.5/wandb/run-20230423_121605-oewau9jn/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8235 2023-04-23 12:33:09.000000 fschat-0.2.5/wandb/run-20230423_123304-94p1mndo/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8252 2023-04-23 12:33:55.000000 fschat-0.2.5/wandb/run-20230423_123350-racn42nr/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.185236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8026 2023-04-23 12:44:12.000000 fschat-0.2.5/wandb/run-20230423_124407-xpczkc0l/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8027 2023-04-23 12:45:40.000000 fschat-0.2.5/wandb/run-20230423_124535-pleqc6uj/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8050 2023-04-23 12:47:12.000000 fschat-0.2.5/wandb/run-20230423_124706-32z1z18w/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8065 2023-04-23 12:48:16.000000 fschat-0.2.5/wandb/run-20230423_124811-w9ghf3r5/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8150 2023-04-23 12:49:50.000000 fschat-0.2.5/wandb/run-20230423_124945-tir0cmzd/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8172 2023-04-23 12:50:49.000000 fschat-0.2.5/wandb/run-20230423_125044-gt2auh7h/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8177 2023-04-23 12:51:43.000000 fschat-0.2.5/wandb/run-20230423_125138-ppb0mitq/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8217 2023-04-23 12:53:11.000000 fschat-0.2.5/wandb/run-20230423_125306-qlqhal9y/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:15:57.000000 fschat-0.2.5/wandb/run-20230423_131552-4ohibdhq/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:17:37.000000 fschat-0.2.5/wandb/run-20230423_131732-om16fnx6/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.189236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8485 2023-04-23 13:22:26.000000 fschat-0.2.5/wandb/run-20230423_132221-qaa4eh88/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:28:07.000000 fschat-0.2.5/wandb/run-20230425_092801-9vh8lrpr/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:28:26.000000 fschat-0.2.5/wandb/run-20230425_092821-byzh59pu/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2023-04-25 09:29:26.000000 fschat-0.2.5/wandb/run-20230425_092921-b2h0ajxd/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8722 2023-04-25 09:30:15.000000 fschat-0.2.5/wandb/run-20230425_093010-q4zph69x/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:31:04.000000 fschat-0.2.5/wandb/run-20230425_093059-7cyyktqp/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8728 2023-04-25 09:32:09.000000 fschat-0.2.5/wandb/run-20230425_093204-iz6wis38/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8657 2023-04-25 09:47:01.000000 fschat-0.2.5/wandb/run-20230425_094656-skoa23zu/files/code/fastchat/train/train.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.193236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/fastchat/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-30 01:50:56.205236 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/fastchat/train/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8667 2023-04-29 11:02:46.000000 fschat-0.2.5/wandb/run-20230429_110237-twh9tcpx/files/code/fastchat/train/train.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-04-03 18:06:47.000000 fschat-0.2.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 09:50:28.063382 fschat-0.2.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15049 2023-05-08 09:41:45.000000 fschat-0.2.6/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.055382 fschat-0.2.6/fastchat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2023-05-08 09:42:14.000000 fschat-0.2.6/fastchat/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.055382 fschat-0.2.6/fastchat/client/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      105 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/client/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2104 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/client/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      701 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/client/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14198 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.055382 fschat-0.2.6/fastchat/data/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/data/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6095 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/clean_sharegpt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6018 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/hardcoded_questions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      934 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/inspect.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      649 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/data/merge.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2711 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/data/optional_clean.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      475 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/data/pretty_json.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1005 2023-04-30 00:44:53.000000 fschat-0.2.6/fastchat/data/sample.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3502 2023-05-05 11:09:54.000000 fschat-0.2.6/fastchat/data/split_long_conversation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.059382 fschat-0.2.6/fastchat/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5257 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/eval/eval_gpt_review.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3776 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/eval/generate_webpage_data_from_table.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3017 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/eval/get_model_answer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2420 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/eval/qa_baseline_gpt35.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.059382 fschat-0.2.6/fastchat/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-27 21:14:01.000000 fschat-0.2.6/fastchat/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5999 2023-05-08 06:48:06.000000 fschat-0.2.6/fastchat/model/apply_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1564 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/model/apply_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      987 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/model/chatglm_model.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/compression.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      846 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/model/convert_fp16.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/make_delta.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14980 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/model_adapter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2772 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/model_registry.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4163 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/model/monkey_patch_non_inplace.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      950 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/model/rwkv_model.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.059382 fschat-0.2.6/fastchat/protocol/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1655 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/protocol/chat_completion.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fastchat/serve/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/serve/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10203 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11456 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/cacheflow_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5497 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/serve/cli.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11809 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/controller.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14370 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_block_arena_anony.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14209 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_block_arena_named.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2714 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/serve/gradio_css.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7386 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/serve/gradio_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20281 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_web_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6239 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/gradio_web_server_multi.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/huggingface_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7980 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/inference.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10911 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/model_worker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fastchat/serve/monitor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5413 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/basic_stats.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5116 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/clean_battle_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8275 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/elo_analysis.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6919 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/serve/monitor/monitor.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-04-17 02:09:54.000000 fschat-0.2.6/fastchat/serve/register_worker.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2401 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/serve/test_message.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/serve/test_throughput.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fastchat/train/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4053 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/train/llama_flash_attn_monkey_patch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8670 2023-05-08 06:53:27.000000 fschat-0.2.6/fastchat/train/train.py
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    14619 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/train/train_flant5.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4958 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/train/train_lora.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      354 2023-04-30 00:47:10.000000 fschat-0.2.6/fastchat/train/train_mem.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6393 2023-05-08 09:41:45.000000 fschat-0.2.6/fastchat/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-08 09:50:28.063382 fschat-0.2.6/fschat.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15543 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      253 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-08 09:50:28.000000 fschat-0.2.6/fschat.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-05-08 09:42:47.000000 fschat-0.2.6/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-08 09:50:28.063382 fschat-0.2.6/setup.cfg
```

### Comparing `fschat-0.2.5/LICENSE` & `fschat-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/PKG-INFO` & `fschat-0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: fschat
-Version: 0.2.5
+Version: 0.2.6
 Summary: An open platform for training, serving, and evaluating large language model based chatbots.
 Project-URL: Homepage, https://github.com/lm-sys/fastchat
 Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # FastChat
-| [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
+| [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) |
 
-An open platform for training, serving, and evaluating large language model based chatbots.
-
-## Release
-<p align="center">
-<a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
-</p>
-
-- 🔥 We released **FastChat-T5** compatible with commercial usage. Checkout [weights](#fastchat-t5).
-
-- 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
+FastChat is an open platform for training, serving, and evaluating large language model based chatbots. The core features include:
+- The weights, training code, and evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5).
+- A distributed multi-model serving system with Web UI and OpenAI-Compatible RESTful APIs.
+
+## News
+- [2023/05] 🔥 We introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
+- [2023/04] We released **FastChat-T5** compatible with commercial usage. Check out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org).
+- [2023/03] We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
 ## Contents
 - [Install](#install)
 - [Model Weights](#model-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
@@ -64,38 +62,40 @@
 ```
 
 ## Model Weights
 ### Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
-1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
+1. Get the original LLaMA weights in the Hugging Face format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 #### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
+Replace `/path/to/*` with the real paths.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-7b \
-    --target-model-path /output/path/to/vicuna-7b \
+    --target-model-path /path/to/output/vicuna-7b \
     --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
 #### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
+Replace `/path/to/*` with the real paths.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-13b \
-    --target-model-path /output/path/to/vicuna-13b \
+    --target-model-path /path/to/output/vicuna-13b \
     --delta-path lmsys/vicuna-13b-delta-v1.1
 ```
 
 #### Old weights
 See [docs/vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of weights and their differences.
 
 #### Low CPU Memory Conversion
@@ -117,24 +117,26 @@
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
 #### Supported Models
 The following models are tested:
 - Vicuna, Alpaca, LLaMA, Koala
 - [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
+- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
-- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
+Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
 
 #### Multiple GPUs
 You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
@@ -163,32 +165,38 @@
 Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
 ```
 
 In addition to that, you can add `--cpu-offloading` to commands above to offload weights that don't fit on your GPU onto the CPU memory. This requires 8-bit compression to be enabled and the bitsandbytes package to be installed, which is only available on linux operating systems.
 
+#### More Platforms
+
+- [MLC LLM](https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs and web browsers via Vulkan, Metal, CUDA and WebGPU.
+
 ## Serving with Web GUI
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_gui.png" width="70%"></a>
 
-To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
+To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. You can learn more about the architecture [here](docs/server_arch.md).
+
+Here are the commands to follow in your terminal:
 
 #### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
-#### Launch the model worker
+#### Launch the model worker(s)
 ```bash
 python3 -m fastchat.serve.model_worker --model-path /path/to/model/weights
 ```
-Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
+Wait until the process finishes loading the model and you see "Uvicorn running on ...". The model worker will register itself to the controller .
 
 To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
 python3 -m fastchat.serve.test_message --model-name vicuna-7b
 ```
 You will see a short output.
 
@@ -196,88 +204,36 @@
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
 This is the user interface that users will interact with.
 
 By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
+If the models do not show up, try to reboot the gradio web server.
 
-
-## API
-
-### Huggingface Generation APIs
-See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py)
-
-### OpenAI-compatible RESTful APIs & SDK
-
-(Experimental. We will keep improving the API and SDK.)
-
-#### Chat Completion
-
-Reference: https://platform.openai.com/docs/api-reference/chat/create
-
-Some features/compatibilities to be implemented:
-
-- [ ] streaming
-- [ ] support of some parameters like `top_p`, `presence_penalty`
-- [ ] proper error handling (e.g. model not found)
-- [ ] the return value in the client SDK could be used like a dict
-
-
-**RESTful API Server**
-
-First, launch the controller
-
-```bash
-python3 -m fastchat.serve.controller
+#### (Optional): Advanced Features
+- You can register multiple model workers to a single controller, which can be used for serving a single model with higher throughput or serving multiple models at the same time. When doing so, please allocate different GPUs and ports for different model workers.
 ```
-
-Then, launch the model worker(s)
-
-```bash
-python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights
+# worker 0
+CUDA_VISIBLE_DEVICES=0 python3 -m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --controller http://localhost:21001 --port 31000 --worker http://localhost:31000
+# worker 1
+CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --port 31001 --worker http://localhost:31001
 ```
-
-Finally, launch the RESTful API server
-
+- You can also launch a multi-tab gradio server, which includes the Chatbot Arena tabs.
 ```bash
-export FASTCHAT_CONTROLLER_URL=http://localhost:21001
-python3 -m fastchat.serve.api --host localhost --port 8000
+python3 -m fastchat.serve.gradio_web_server_multi
 ```
 
-Test the API server
-
-```bash
-curl http://localhost:8000/v1/chat/completions \
-  -H "Content-Type: application/json" \
-  -d '{
-    "model": "vicuna-7b-v1.1",
-    "messages": [{"role": "user", "content": "Hello!"}]
-  }'
-```
-
-**Client SDK**
-
-Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://localhost:8000`), you can use the following code to send a request to the API server:
-
-```python
-import os
-from fastchat import client
-
-client.set_baseurl(os.getenv("FASTCHAT_BASEURL"))
-
-completion = client.ChatCompletion.create(
-  model="vicuna-7b-v1.1",
-  messages=[
-    {"role": "user", "content": "Hello!"}
-  ]
-)
+## API
+### OpenAI-Compatible RESTful APIs & SDK
+FastChat provides OpenAI-Compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+See [docs/openai_api.md](docs/openai_api.md).
 
-print(completion.choices[0].message)
-```
+### Hugging Face Generation APIs
+See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py).
 
 ## Evaluation
 
 Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ### Pipeline Steps
```

#### html2text {}

```diff
@@ -1,144 +1,151 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.5 Summary: An open platform for
+Metadata-Version: 2.1 Name: fschat Version: 0.2.6 Summary: An open platform for
 training, serving, and evaluating large language model based chatbots. Project-
 URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
 https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # FastChat | [Demo](https://chat.lmsys.org/) |
-[Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) |
-[Twitter](https://twitter.com/lmsysorg) | An open platform for training,
-serving, and evaluating large language model based chatbots. ## Release
-                           [assets/vicuna_logo.jpeg]
-- ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
-[weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
-Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
-vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
-## Contents - [Install](#install) - [Model Weights](#model-weights) -
-[Inference with Command Line Interface](#inference-with-command-line-interface)
-- [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
-(#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
-```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
-repository and navigate to the FastChat folder ```bash git clone https://
-github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
-```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
-upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Model Weights ###
-Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
-weights to comply with the LLaMA model license. You can add our delta to the
-original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
-original LLaMA weights in the huggingface format by following the instructions
-[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
-the following scripts to get Vicuna weights by applying our delta. They will
-automatically download delta weights from our Hugging Face [account](https://
-huggingface.co/lmsys). **NOTE**: Weights v1.1 are only compatible with
-```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
-packages accordingly. If you follow the above commands to do a fresh install,
-then you should get all the correct versions. #### Vicuna-7B This conversion
-command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
-section below if you do not have enough memory. ```bash python3 -
+dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
+[**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
+h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) | FastChat is an open
+platform for training, serving, and evaluating large language model based
+chatbots. The core features include: - The weights, training code, and
+evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5). - A
+distributed multi-model serving system with Web UI and OpenAI-Compatible
+RESTful APIs. ## News - [2023/05] ð¥ We introduced **Chatbot Arena** for
+battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-
+03-arena) and [demo](https://arena.lmsys.org). - [2023/04] We released
+**FastChat-T5** compatible with commercial usage. Check out the [weights]
+(#fastchat-t5) and [demo](https://chat.lmsys.org). - [2023/03] We released
+**Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**.
+Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://
+chat.lmsys.org). [assets/demo_narrow.gif] ## Contents - [Install](#install) -
+[Model Weights](#model-weights) - [Inference with Command Line Interface]
+(#inference-with-command-line-interface) - [Serving with Web GUI](#serving-
+with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
+tuning) ## Install ### Method 1: With pip ```bash pip3 install fschat ``` ###
+Method 2: From source 1. Clone this repository and navigate to the FastChat
+folder ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ```
+If you are running on Mac: ```bash brew install rust cmake ``` 2. Install
+Package ```bash pip3 install --upgrade pip # enable PEP 660 support pip3
+install -e . ``` ## Model Weights ### Vicuna Weights We release [Vicuna](https:
+//vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
+license. You can add our delta to the original LLaMA weights to obtain the
+Vicuna weights. Instructions: 1. Get the original LLaMA weights in the Hugging
+Face format by following the instructions [here](https://huggingface.co/docs/
+transformers/main/model_doc/llama). 2. Use the following scripts to get Vicuna
+weights by applying our delta. They will automatically download delta weights
+from our Hugging Face [account](https://huggingface.co/lmsys). **NOTE**:
+Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat
+>= 0.2.0``. Please update your local packages accordingly. If you follow the
+above commands to do a fresh install, then you should get all the correct
+versions. #### Vicuna-7B This conversion command needs around 30 GB of CPU RAM.
+See the "Low CPU Memory Conversion" section below if you do not have enough
+memory. Replace `/path/to/*` with the real paths. ```bash python3 -
 m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
-model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
+model-path /path/to/output/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
 ``` #### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
 the "Low CPU Memory Conversion" section below if you do not have enough memory.
-```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
-llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
-lmsys/vicuna-13b-delta-v1.1 ``` #### Old weights See [docs/
-vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of
-weights and their differences. #### Low CPU Memory Conversion You can try these
-methods to reduce the CPU RAM requirement of weight conversion. 1. Append `--
-low-cpu-mem` to the commands above, which will split large weight files into
-smaller ones and use the disk as temporary storage. This can keep the peak
-memory at less than 16GB. 2. Create a large swap file and rely on the operating
-system to automatically utilize the disk as virtual memory. ### FastChat-T5
-Simply run the line below to start chatting. It will automatically download the
-weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-
-v1.0). ```bash python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-
-v1.0 ``` ## Inference with Command Line Interface (Experimental Feature: You
-can specify `--style rich` to enable rich text output and better text streaming
-quality for some non-ASCII content. This may not work properly on certain
-terminals.) [assets/screenshot_cli.png] #### Supported Models The following
-models are tested: - Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0]
-(https://huggingface.co/lmsys/fastchat-t5) - [databricks/dolly-v2-12b](https://
+Replace `/path/to/*` with the real paths. ```bash python3 -
+m fastchat.model.apply_delta \ --base-model-path /path/to/llama-13b \ --target-
+model-path /path/to/output/vicuna-13b \ --delta-path lmsys/vicuna-13b-delta-
+v1.1 ``` #### Old weights See [docs/vicuna_weights_version.md](docs/
+vicuna_weights_version.md) for all versions of weights and their differences.
+#### Low CPU Memory Conversion You can try these methods to reduce the CPU RAM
+requirement of weight conversion. 1. Append `--low-cpu-mem` to the commands
+above, which will split large weight files into smaller ones and use the disk
+as temporary storage. This can keep the peak memory at less than 16GB. 2.
+Create a large swap file and rely on the operating system to automatically
+utilize the disk as virtual memory. ### FastChat-T5 Simply run the line below
+to start chatting. It will automatically download the weights from a Hugging
+Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). ```bash python3
+-m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0 ``` ## Inference
+with Command Line Interface (Experimental Feature: You can specify `--style
+rich` to enable rich text output and better text streaming quality for some
+non-ASCII content. This may not work properly on certain terminals.) [assets/
+screenshot_cli.png] #### Supported Models The following models are tested: -
+Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0](https://
+huggingface.co/lmsys/fastchat-t5) - [BlinkDL/RWKV-4-Raven](https://
+huggingface.co/BlinkDL/rwkv-4-raven) - [databricks/dolly-v2-12b](https://
 huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
 12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
 baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
-[BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven) -
 [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
 stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
-chatglm-6b) #### Single GPU The command below requires around 28GB of GPU
-memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough
-Memory" section below if you do not have enough memory. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights ``` #### Multiple GPUs
-You can use model parallelism to aggregate GPU memory from multiple GPUs on the
-same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
-weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and does not
-require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around
-30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/model/weights --device cpu ``` #### Metal Backend (Mac Computers
-with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU acceleration
-on Mac computers (requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit
-compression. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
-weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook
-with 1 - 2 words / second. #### No Enough Memory If you do not have enough
-memory, you can enable 8-bit compression by adding `--load-8bit` to commands
-above. This can reduce memory usage by around half with slightly degraded model
-quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
-8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ```
-python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
-``` In addition to that, you can add `--cpu-offloading` to commands above to
-offload weights that don't fit on your GPU onto the CPU memory. This requires
-8-bit compression to be enabled and the bitsandbytes package to be installed,
-which is only available on linux operating systems. ## Serving with Web GUI
+chatglm-6b) - [FreedomIntelligence/phoenix-inst-chat-7b](https://
+huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) #### Single GPU The
+command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU
+memory for Vicuna-7B. See the "No Enough Memory" section below if you do not
+have enough memory. Replace `/path/to/model/weights` with the a local folder or
+a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+model/weights ``` #### Multiple GPUs You can use model parallelism to aggregate
+GPU memory from multiple GPUs on the same machine. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
+CPU Only This runs on the CPU only and does not require GPU. It requires around
+60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
+2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
+8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
+No Enough Memory If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
+addition to that, you can add `--cpu-offloading` to commands above to offload
+weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
+compression to be enabled and the bitsandbytes package to be installed, which
+is only available on linux operating systems. #### More Platforms - [MLC LLM]
+(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
+tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
+and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
 [assets/screenshot_gui.png] To serve using the web UI, you need three main
 components: web servers that interface with users, model workers that host one
 or more models, and a controller to coordinate the webserver and model workers.
-Here are the commands to follow in your terminal: #### Launch the controller
-```bash python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker ```bash python3 -
+You can learn more about the architecture [here](docs/server_arch.md). Here are
+the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
-...". You can launch multiple model workers to serve multiple models
-concurrently. The model worker will connect to the controller automatically. To
-ensure that your model worker is connected to your controller properly, send a
-test message using the following command: ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-7b ``` You will see a short
-output. #### Launch the Gradio web server ```bash python3 -
-m fastchat.serve.gradio_web_server ``` This is the user interface that users
-will interact with. By following these steps, you will be able to serve your
-models using the web UI. You can open your browser and chat with a model now.
-## API ### Huggingface Generation APIs See [fastchat/serve/huggingface_api.py]
-(fastchat/serve/huggingface_api.py) ### OpenAI-compatible RESTful APIs & SDK
-(Experimental. We will keep improving the API and SDK.) #### Chat Completion
-Reference: https://platform.openai.com/docs/api-reference/chat/create Some
-features/compatibilities to be implemented: - [ ] streaming - [ ] support of
-some parameters like `top_p`, `presence_penalty` - [ ] proper error handling
-(e.g. model not found) - [ ] the return value in the client SDK could be used
-like a dict **RESTful API Server** First, launch the controller ```bash python3
--m fastchat.serve.controller ``` Then, launch the model worker(s) ```bash
-python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-
-path /path/to/vicuna/weights ``` Finally, launch the RESTful API server ```bash
-export FASTCHAT_CONTROLLER_URL=http://localhost:21001 python3 -
-m fastchat.serve.api --host localhost --port 8000 ``` Test the API server
-```bash curl http://localhost:8000/v1/chat/completions \ -H "Content-Type:
-application/json" \ -d '{ "model": "vicuna-7b-v1.1", "messages": [{"role":
-"user", "content": "Hello!"}] }' ``` **Client SDK** Assuming environment
-variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://
-localhost:8000`), you can use the following code to send a request to the API
-server: ```python import os from fastchat import client client.set_baseurl
-(os.getenv("FASTCHAT_BASEURL")) completion = client.ChatCompletion.create
-( model="vicuna-7b-v1.1", messages=[ {"role": "user", "content": "Hello!"} ] )
-print(completion.choices[0].message) ``` ## Evaluation Our AI-enhanced
-evaluation pipeline is based on GPT-4. This section provides a high-level
-summary of the pipeline. For detailed instructions, please refer to the
-[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
-answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
-specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
-models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
-automatically. This step can also be performed manually if the GPT-4 API is not
-available to you. 3. Generate visualization data: Run
+...". The model worker will register itself to the controller . To ensure that
+your model worker is connected to your controller properly, send a test message
+using the following command: ```bash python3 -m fastchat.serve.test_message --
+model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
+web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
+user interface that users will interact with. By following these steps, you
+will be able to serve your models using the web UI. You can open your browser
+and chat with a model now. If the models do not show up, try to reboot the
+gradio web server. #### (Optional): Advanced Features - You can register
+multiple model workers to a single controller, which can be used for serving a
+single model with higher throughput or serving multiple models at the same
+time. When doing so, please allocate different GPUs and ports for different
+model workers. ``` # worker 0 CUDA_VISIBLE_DEVICES=0 python3 -
+m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --
+controller http://localhost:21001 --port 31000 --worker http://localhost:31000
+# worker 1 CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --
+model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --
+port 31001 --worker http://localhost:31001 ``` - You can also launch a multi-
+tab gradio server, which includes the Chatbot Arena tabs. ```bash python3 -
+m fastchat.serve.gradio_web_server_multi ``` ## API ### OpenAI-Compatible
+RESTful APIs & SDK FastChat provides OpenAI-Compatible APIs for its supported
+models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+See [docs/openai_api.md](docs/openai_api.md). ### Hugging Face Generation APIs
+See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py). ##
+Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
+provides a high-level summary of the pipeline. For detailed instructions,
+please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
+Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
+ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
+Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
+reviews automatically. This step can also be performed manually if the GPT-
+4 API is not available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.5/README.md` & `fschat-0.2.6/fschat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,31 @@
-# FastChat
-| [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
-
-An open platform for training, serving, and evaluating large language model based chatbots.
-
-## Release
-<p align="center">
-<a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
-</p>
+Metadata-Version: 2.1
+Name: fschat
+Version: 0.2.6
+Summary: An open platform for training, serving, and evaluating large language model based chatbots.
+Project-URL: Homepage, https://github.com/lm-sys/fastchat
+Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
-- 🔥 We released **FastChat-T5** compatible with commercial usage. Checkout [weights](#fastchat-t5).
+# FastChat
+| [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) |
 
-- 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
+FastChat is an open platform for training, serving, and evaluating large language model based chatbots. The core features include:
+- The weights, training code, and evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5).
+- A distributed multi-model serving system with Web UI and OpenAI-Compatible RESTful APIs.
+
+## News
+- [2023/05] 🔥 We introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
+- [2023/04] We released **FastChat-T5** compatible with commercial usage. Check out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org).
+- [2023/03] We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
 ## Contents
 - [Install](#install)
 - [Model Weights](#model-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
@@ -51,38 +62,40 @@
 ```
 
 ## Model Weights
 ### Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
-1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
+1. Get the original LLaMA weights in the Hugging Face format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 #### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
+Replace `/path/to/*` with the real paths.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-7b \
-    --target-model-path /output/path/to/vicuna-7b \
+    --target-model-path /path/to/output/vicuna-7b \
     --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
 #### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
+Replace `/path/to/*` with the real paths.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-13b \
-    --target-model-path /output/path/to/vicuna-13b \
+    --target-model-path /path/to/output/vicuna-13b \
     --delta-path lmsys/vicuna-13b-delta-v1.1
 ```
 
 #### Old weights
 See [docs/vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of weights and their differences.
 
 #### Low CPU Memory Conversion
@@ -104,24 +117,26 @@
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
 #### Supported Models
 The following models are tested:
 - Vicuna, Alpaca, LLaMA, Koala
 - [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
+- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
-- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
+Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
 
 #### Multiple GPUs
 You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
@@ -150,32 +165,38 @@
 Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
 ```
 
 In addition to that, you can add `--cpu-offloading` to commands above to offload weights that don't fit on your GPU onto the CPU memory. This requires 8-bit compression to be enabled and the bitsandbytes package to be installed, which is only available on linux operating systems.
 
+#### More Platforms
+
+- [MLC LLM](https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs and web browsers via Vulkan, Metal, CUDA and WebGPU.
+
 ## Serving with Web GUI
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_gui.png" width="70%"></a>
 
-To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
+To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. You can learn more about the architecture [here](docs/server_arch.md).
+
+Here are the commands to follow in your terminal:
 
 #### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
-#### Launch the model worker
+#### Launch the model worker(s)
 ```bash
 python3 -m fastchat.serve.model_worker --model-path /path/to/model/weights
 ```
-Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
+Wait until the process finishes loading the model and you see "Uvicorn running on ...". The model worker will register itself to the controller .
 
 To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
 python3 -m fastchat.serve.test_message --model-name vicuna-7b
 ```
 You will see a short output.
 
@@ -183,88 +204,36 @@
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
 This is the user interface that users will interact with.
 
 By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
+If the models do not show up, try to reboot the gradio web server.
 
-
-## API
-
-### Huggingface Generation APIs
-See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py)
-
-### OpenAI-compatible RESTful APIs & SDK
-
-(Experimental. We will keep improving the API and SDK.)
-
-#### Chat Completion
-
-Reference: https://platform.openai.com/docs/api-reference/chat/create
-
-Some features/compatibilities to be implemented:
-
-- [ ] streaming
-- [ ] support of some parameters like `top_p`, `presence_penalty`
-- [ ] proper error handling (e.g. model not found)
-- [ ] the return value in the client SDK could be used like a dict
-
-
-**RESTful API Server**
-
-First, launch the controller
-
-```bash
-python3 -m fastchat.serve.controller
+#### (Optional): Advanced Features
+- You can register multiple model workers to a single controller, which can be used for serving a single model with higher throughput or serving multiple models at the same time. When doing so, please allocate different GPUs and ports for different model workers.
 ```
-
-Then, launch the model worker(s)
-
-```bash
-python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights
+# worker 0
+CUDA_VISIBLE_DEVICES=0 python3 -m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --controller http://localhost:21001 --port 31000 --worker http://localhost:31000
+# worker 1
+CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --port 31001 --worker http://localhost:31001
 ```
-
-Finally, launch the RESTful API server
-
+- You can also launch a multi-tab gradio server, which includes the Chatbot Arena tabs.
 ```bash
-export FASTCHAT_CONTROLLER_URL=http://localhost:21001
-python3 -m fastchat.serve.api --host localhost --port 8000
+python3 -m fastchat.serve.gradio_web_server_multi
 ```
 
-Test the API server
-
-```bash
-curl http://localhost:8000/v1/chat/completions \
-  -H "Content-Type: application/json" \
-  -d '{
-    "model": "vicuna-7b-v1.1",
-    "messages": [{"role": "user", "content": "Hello!"}]
-  }'
-```
-
-**Client SDK**
-
-Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://localhost:8000`), you can use the following code to send a request to the API server:
-
-```python
-import os
-from fastchat import client
-
-client.set_baseurl(os.getenv("FASTCHAT_BASEURL"))
-
-completion = client.ChatCompletion.create(
-  model="vicuna-7b-v1.1",
-  messages=[
-    {"role": "user", "content": "Hello!"}
-  ]
-)
+## API
+### OpenAI-Compatible RESTful APIs & SDK
+FastChat provides OpenAI-Compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+See [docs/openai_api.md](docs/openai_api.md).
 
-print(completion.choices[0].message)
-```
+### Hugging Face Generation APIs
+See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py).
 
 ## Evaluation
 
 Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ### Pipeline Steps
```

#### html2text {}

```diff
@@ -1,138 +1,151 @@
-# FastChat | [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org)
-| [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/
-lmsysorg) | An open platform for training, serving, and evaluating large
-language model based chatbots. ## Release
-                           [assets/vicuna_logo.jpeg]
-- ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
-[weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
-Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
-vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
-## Contents - [Install](#install) - [Model Weights](#model-weights) -
-[Inference with Command Line Interface](#inference-with-command-line-interface)
-- [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
-(#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
-```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
-repository and navigate to the FastChat folder ```bash git clone https://
-github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
-```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
-upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Model Weights ###
-Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
-weights to comply with the LLaMA model license. You can add our delta to the
-original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
-original LLaMA weights in the huggingface format by following the instructions
-[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
-the following scripts to get Vicuna weights by applying our delta. They will
-automatically download delta weights from our Hugging Face [account](https://
-huggingface.co/lmsys). **NOTE**: Weights v1.1 are only compatible with
-```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
-packages accordingly. If you follow the above commands to do a fresh install,
-then you should get all the correct versions. #### Vicuna-7B This conversion
-command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
-section below if you do not have enough memory. ```bash python3 -
+Metadata-Version: 2.1 Name: fschat Version: 0.2.6 Summary: An open platform for
+training, serving, and evaluating large language model based chatbots. Project-
+URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
+https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+dev License-File: LICENSE # FastChat | [**Demo**](https://chat.lmsys.org/) |
+[**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/
+h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) | FastChat is an open
+platform for training, serving, and evaluating large language model based
+chatbots. The core features include: - The weights, training code, and
+evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5). - A
+distributed multi-model serving system with Web UI and OpenAI-Compatible
+RESTful APIs. ## News - [2023/05] ð¥ We introduced **Chatbot Arena** for
+battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-
+03-arena) and [demo](https://arena.lmsys.org). - [2023/04] We released
+**FastChat-T5** compatible with commercial usage. Check out the [weights]
+(#fastchat-t5) and [demo](https://chat.lmsys.org). - [2023/03] We released
+**Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**.
+Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://
+chat.lmsys.org). [assets/demo_narrow.gif] ## Contents - [Install](#install) -
+[Model Weights](#model-weights) - [Inference with Command Line Interface]
+(#inference-with-command-line-interface) - [Serving with Web GUI](#serving-
+with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-tuning](#fine-
+tuning) ## Install ### Method 1: With pip ```bash pip3 install fschat ``` ###
+Method 2: From source 1. Clone this repository and navigate to the FastChat
+folder ```bash git clone https://github.com/lm-sys/FastChat.git cd FastChat ```
+If you are running on Mac: ```bash brew install rust cmake ``` 2. Install
+Package ```bash pip3 install --upgrade pip # enable PEP 660 support pip3
+install -e . ``` ## Model Weights ### Vicuna Weights We release [Vicuna](https:
+//vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model
+license. You can add our delta to the original LLaMA weights to obtain the
+Vicuna weights. Instructions: 1. Get the original LLaMA weights in the Hugging
+Face format by following the instructions [here](https://huggingface.co/docs/
+transformers/main/model_doc/llama). 2. Use the following scripts to get Vicuna
+weights by applying our delta. They will automatically download delta weights
+from our Hugging Face [account](https://huggingface.co/lmsys). **NOTE**:
+Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat
+>= 0.2.0``. Please update your local packages accordingly. If you follow the
+above commands to do a fresh install, then you should get all the correct
+versions. #### Vicuna-7B This conversion command needs around 30 GB of CPU RAM.
+See the "Low CPU Memory Conversion" section below if you do not have enough
+memory. Replace `/path/to/*` with the real paths. ```bash python3 -
 m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
-model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
+model-path /path/to/output/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
 ``` #### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
 the "Low CPU Memory Conversion" section below if you do not have enough memory.
-```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
-llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
-lmsys/vicuna-13b-delta-v1.1 ``` #### Old weights See [docs/
-vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of
-weights and their differences. #### Low CPU Memory Conversion You can try these
-methods to reduce the CPU RAM requirement of weight conversion. 1. Append `--
-low-cpu-mem` to the commands above, which will split large weight files into
-smaller ones and use the disk as temporary storage. This can keep the peak
-memory at less than 16GB. 2. Create a large swap file and rely on the operating
-system to automatically utilize the disk as virtual memory. ### FastChat-T5
-Simply run the line below to start chatting. It will automatically download the
-weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-
-v1.0). ```bash python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-
-v1.0 ``` ## Inference with Command Line Interface (Experimental Feature: You
-can specify `--style rich` to enable rich text output and better text streaming
-quality for some non-ASCII content. This may not work properly on certain
-terminals.) [assets/screenshot_cli.png] #### Supported Models The following
-models are tested: - Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0]
-(https://huggingface.co/lmsys/fastchat-t5) - [databricks/dolly-v2-12b](https://
+Replace `/path/to/*` with the real paths. ```bash python3 -
+m fastchat.model.apply_delta \ --base-model-path /path/to/llama-13b \ --target-
+model-path /path/to/output/vicuna-13b \ --delta-path lmsys/vicuna-13b-delta-
+v1.1 ``` #### Old weights See [docs/vicuna_weights_version.md](docs/
+vicuna_weights_version.md) for all versions of weights and their differences.
+#### Low CPU Memory Conversion You can try these methods to reduce the CPU RAM
+requirement of weight conversion. 1. Append `--low-cpu-mem` to the commands
+above, which will split large weight files into smaller ones and use the disk
+as temporary storage. This can keep the peak memory at less than 16GB. 2.
+Create a large swap file and rely on the operating system to automatically
+utilize the disk as virtual memory. ### FastChat-T5 Simply run the line below
+to start chatting. It will automatically download the weights from a Hugging
+Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0). ```bash python3
+-m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-v1.0 ``` ## Inference
+with Command Line Interface (Experimental Feature: You can specify `--style
+rich` to enable rich text output and better text streaming quality for some
+non-ASCII content. This may not work properly on certain terminals.) [assets/
+screenshot_cli.png] #### Supported Models The following models are tested: -
+Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0](https://
+huggingface.co/lmsys/fastchat-t5) - [BlinkDL/RWKV-4-Raven](https://
+huggingface.co/BlinkDL/rwkv-4-raven) - [databricks/dolly-v2-12b](https://
 huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
 12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
 baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
-[BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven) -
 [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
 stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
-chatglm-6b) #### Single GPU The command below requires around 28GB of GPU
-memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough
-Memory" section below if you do not have enough memory. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights ``` #### Multiple GPUs
-You can use model parallelism to aggregate GPU memory from multiple GPUs on the
-same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
-weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and does not
-require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around
-30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/model/weights --device cpu ``` #### Metal Backend (Mac Computers
-with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU acceleration
-on Mac computers (requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit
-compression. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
-weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook
-with 1 - 2 words / second. #### No Enough Memory If you do not have enough
-memory, you can enable 8-bit compression by adding `--load-8bit` to commands
-above. This can reduce memory usage by around half with slightly degraded model
-quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
-8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ```
-python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
-``` In addition to that, you can add `--cpu-offloading` to commands above to
-offload weights that don't fit on your GPU onto the CPU memory. This requires
-8-bit compression to be enabled and the bitsandbytes package to be installed,
-which is only available on linux operating systems. ## Serving with Web GUI
+chatglm-6b) - [FreedomIntelligence/phoenix-inst-chat-7b](https://
+huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) #### Single GPU The
+command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU
+memory for Vicuna-7B. See the "No Enough Memory" section below if you do not
+have enough memory. Replace `/path/to/model/weights` with the a local folder or
+a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+model/weights ``` #### Multiple GPUs You can use model parallelism to aggregate
+GPU memory from multiple GPUs on the same machine. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
+CPU Only This runs on the CPU only and does not require GPU. It requires around
+60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
+2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
+8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
+No Enough Memory If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
+addition to that, you can add `--cpu-offloading` to commands above to offload
+weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
+compression to be enabled and the bitsandbytes package to be installed, which
+is only available on linux operating systems. #### More Platforms - [MLC LLM]
+(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
+tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
+and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
 [assets/screenshot_gui.png] To serve using the web UI, you need three main
 components: web servers that interface with users, model workers that host one
 or more models, and a controller to coordinate the webserver and model workers.
-Here are the commands to follow in your terminal: #### Launch the controller
-```bash python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker ```bash python3 -
+You can learn more about the architecture [here](docs/server_arch.md). Here are
+the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
-...". You can launch multiple model workers to serve multiple models
-concurrently. The model worker will connect to the controller automatically. To
-ensure that your model worker is connected to your controller properly, send a
-test message using the following command: ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-7b ``` You will see a short
-output. #### Launch the Gradio web server ```bash python3 -
-m fastchat.serve.gradio_web_server ``` This is the user interface that users
-will interact with. By following these steps, you will be able to serve your
-models using the web UI. You can open your browser and chat with a model now.
-## API ### Huggingface Generation APIs See [fastchat/serve/huggingface_api.py]
-(fastchat/serve/huggingface_api.py) ### OpenAI-compatible RESTful APIs & SDK
-(Experimental. We will keep improving the API and SDK.) #### Chat Completion
-Reference: https://platform.openai.com/docs/api-reference/chat/create Some
-features/compatibilities to be implemented: - [ ] streaming - [ ] support of
-some parameters like `top_p`, `presence_penalty` - [ ] proper error handling
-(e.g. model not found) - [ ] the return value in the client SDK could be used
-like a dict **RESTful API Server** First, launch the controller ```bash python3
--m fastchat.serve.controller ``` Then, launch the model worker(s) ```bash
-python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-
-path /path/to/vicuna/weights ``` Finally, launch the RESTful API server ```bash
-export FASTCHAT_CONTROLLER_URL=http://localhost:21001 python3 -
-m fastchat.serve.api --host localhost --port 8000 ``` Test the API server
-```bash curl http://localhost:8000/v1/chat/completions \ -H "Content-Type:
-application/json" \ -d '{ "model": "vicuna-7b-v1.1", "messages": [{"role":
-"user", "content": "Hello!"}] }' ``` **Client SDK** Assuming environment
-variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://
-localhost:8000`), you can use the following code to send a request to the API
-server: ```python import os from fastchat import client client.set_baseurl
-(os.getenv("FASTCHAT_BASEURL")) completion = client.ChatCompletion.create
-( model="vicuna-7b-v1.1", messages=[ {"role": "user", "content": "Hello!"} ] )
-print(completion.choices[0].message) ``` ## Evaluation Our AI-enhanced
-evaluation pipeline is based on GPT-4. This section provides a high-level
-summary of the pipeline. For detailed instructions, please refer to the
-[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
-answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
-specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
-models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
-automatically. This step can also be performed manually if the GPT-4 API is not
-available to you. 3. Generate visualization data: Run
+...". The model worker will register itself to the controller . To ensure that
+your model worker is connected to your controller properly, send a test message
+using the following command: ```bash python3 -m fastchat.serve.test_message --
+model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
+web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
+user interface that users will interact with. By following these steps, you
+will be able to serve your models using the web UI. You can open your browser
+and chat with a model now. If the models do not show up, try to reboot the
+gradio web server. #### (Optional): Advanced Features - You can register
+multiple model workers to a single controller, which can be used for serving a
+single model with higher throughput or serving multiple models at the same
+time. When doing so, please allocate different GPUs and ports for different
+model workers. ``` # worker 0 CUDA_VISIBLE_DEVICES=0 python3 -
+m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --
+controller http://localhost:21001 --port 31000 --worker http://localhost:31000
+# worker 1 CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --
+model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --
+port 31001 --worker http://localhost:31001 ``` - You can also launch a multi-
+tab gradio server, which includes the Chatbot Arena tabs. ```bash python3 -
+m fastchat.serve.gradio_web_server_multi ``` ## API ### OpenAI-Compatible
+RESTful APIs & SDK FastChat provides OpenAI-Compatible APIs for its supported
+models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+See [docs/openai_api.md](docs/openai_api.md). ### Hugging Face Generation APIs
+See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py). ##
+Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
+provides a high-level summary of the pipeline. For detailed instructions,
+please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
+Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
+ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
+Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
+reviews automatically. This step can also be performed manually if the GPT-
+4 API is not available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.5/fastchat/client/api.py` & `fschat-0.2.6/fastchat/client/api.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/client/test_client.py` & `fschat-0.2.6/fastchat/client/test_client.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/conversation.py` & `fschat-0.2.6/fastchat/conversation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 """
 Conversation prompt templates.
 """
 
 import dataclasses
 from enum import auto, Enum
-from typing import List, Tuple, Any
+from typing import List, Tuple, Any, Dict
 
 
 class SeparatorStyle(Enum):
-    """Different separator style."""
+    """Separator styles."""
 
     ADD_COLON_SINGLE = auto()
     ADD_COLON_TWO = auto()
     NO_COLON_SINGLE = auto()
     BAIZE = auto()
     DOLLY = auto()
     RWKV = auto()
+    PHOENIX = auto()
 
 
 @dataclasses.dataclass
 class Conversation:
     """A class that keeps all conversation history."""
 
+    # The name of this template
+    name: str
+    # System prompts
     system: str
+    # Two roles
     roles: List[str]
+    # All messages
     messages: List[List[str]]
     # Offset of few shot examples
     offset: int
-    # Separator
+    # Separators
     sep_style: SeparatorStyle
     sep: str
     sep2: str = None
     # Stop criteria (the default one is EOS token)
     stop_str: str = None
+    # Stops generation if meeting any token in this list
     stop_token_ids: List[int] = None
 
     # Used for the state in the gradio servers.
     # TODO(lmzheng): refactor this
     conv_id: Any = None
     skip_next: bool = False
     model_name: str = None
 
-    def get_prompt(self):
+    def get_prompt(self) -> str:
+        """Get the prompt for generation."""
         if self.sep_style == SeparatorStyle.ADD_COLON_SINGLE:
             ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + message + self.sep
                 else:
                     ret += role + ":"
@@ -86,36 +94,63 @@
                 else:
                     ret += role + ":\n"
             return ret
         elif self.sep_style == SeparatorStyle.RWKV:
             ret = self.system
             for i, (role, message) in enumerate(self.messages):
                 if message:
-                    ret += role + ": " + message.replace('\r\n','\n').replace('\n\n','\n')
+                    ret += (
+                        role
+                        + ": "
+                        + message.replace("\r\n", "\n").replace("\n\n", "\n")
+                    )
                     ret += "\n\n"
                 else:
                     ret += role + ":"
             return ret
+        elif self.sep_style == SeparatorStyle.PHOENIX:
+            ret = self.system
+            for role, message in self.messages:
+                if message:
+                    ret += role + ": " + "<s>" + message + "</s>"
+                else:
+                    ret += role + ": " + "<s>"
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.sep_style}")
 
-    def append_message(self, role, message):
+    def append_message(self, role: str, message: str):
+        """Append a new message."""
         self.messages.append([role, message])
 
     def to_gradio_chatbot(self):
+        """Convert the history to gradio chatbot format"""
         ret = []
         for i, (role, msg) in enumerate(self.messages[self.offset :]):
             if i % 2 == 0:
                 ret.append([msg, None])
             else:
                 ret[-1][-1] = msg
         return ret
 
+    def to_openai_api_messages(self):
+        """Convert the conversation to OpenAI chat completion format."""
+        ret = [{"role": "system", "content": self.system}]
+
+        for i, (_, msg) in enumerate(self.messages[self.offset :]):
+            if i % 2 == 0:
+                ret.append({"role": "user", "content": msg})
+            else:
+                if msg is not None:
+                    ret.append({"role": "assistant", "content": msg})
+        return ret
+
     def copy(self):
         return Conversation(
+            name=self.name,
             system=self.system,
             roles=self.roles,
             messages=[[x, y] for x, y in self.messages],
             offset=self.offset,
             sep_style=self.sep_style,
             sep=self.sep,
             sep2=self.sep2,
@@ -123,178 +158,250 @@
             stop_token_ids=self.stop_token_ids,
             conv_id=self.conv_id,
             model_name=self.model_name,
         )
 
     def dict(self):
         return {
+            "name": self.name,
             "system": self.system,
             "roles": self.roles,
             "messages": self.messages,
             "offset": self.offset,
             "conv_id": self.conv_id,
             "model_name": self.model_name,
         }
 
 
+# A global registry for all conversation templates
+conv_templates: Dict[str, Conversation] = {}
+
+
+def register_conv_template(template: Conversation, override: bool = False):
+    """Register a new conversation template."""
+    if not override:
+        assert template.name not in conv_templates, f"{name} has been registered."
+    conv_templates[template.name] = template
+
+
+def get_conv_template(name: str) -> Conversation:
+    """Get a conversation template."""
+    return conv_templates[name].copy()
+
+
 # A template with one conversation example
-conv_one_shot = Conversation(
-    system="A chat between a curious human and an artificial intelligence assistant. "
-    "The assistant gives helpful, detailed, and polite answers to the human's questions.",
-    roles=("Human", "Assistant"),
-    messages=(
-        (
-            "Human",
-            "What are the key differences between renewable and non-renewable energy sources?",
+register_conv_template(
+    Conversation(
+        name="one_shot",
+        system="A chat between a curious human and an artificial intelligence assistant. "
+        "The assistant gives helpful, detailed, and polite answers to the human's questions.",
+        roles=("Human", "Assistant"),
+        messages=(
+            (
+                "Human",
+                "What are the key differences between renewable and non-renewable energy sources?",
+            ),
+            (
+                "Assistant",
+                "Renewable energy sources are those that can be replenished naturally in a relatively "
+                "short amount of time, such as solar, wind, hydro, geothermal, and biomass. "
+                "Non-renewable energy sources, on the other hand, are finite and will eventually be "
+                "depleted, such as coal, oil, and natural gas. Here are some key differences between "
+                "renewable and non-renewable energy sources:\n"
+                "1. Availability: Renewable energy sources are virtually inexhaustible, while non-renewable "
+                "energy sources are finite and will eventually run out.\n"
+                "2. Environmental impact: Renewable energy sources have a much lower environmental impact "
+                "than non-renewable sources, which can lead to air and water pollution, greenhouse gas emissions, "
+                "and other negative effects.\n"
+                "3. Cost: Renewable energy sources can be more expensive to initially set up, but they typically "
+                "have lower operational costs than non-renewable sources.\n"
+                "4. Reliability: Renewable energy sources are often more reliable and can be used in more remote "
+                "locations than non-renewable sources.\n"
+                "5. Flexibility: Renewable energy sources are often more flexible and can be adapted to different "
+                "situations and needs, while non-renewable sources are more rigid and inflexible.\n"
+                "6. Sustainability: Renewable energy sources are more sustainable over the long term, while "
+                "non-renewable sources are not, and their depletion can lead to economic and social instability.",
+            ),
         ),
-        (
-            "Assistant",
-            "Renewable energy sources are those that can be replenished naturally in a relatively "
-            "short amount of time, such as solar, wind, hydro, geothermal, and biomass. "
-            "Non-renewable energy sources, on the other hand, are finite and will eventually be "
-            "depleted, such as coal, oil, and natural gas. Here are some key differences between "
-            "renewable and non-renewable energy sources:\n"
-            "1. Availability: Renewable energy sources are virtually inexhaustible, while non-renewable "
-            "energy sources are finite and will eventually run out.\n"
-            "2. Environmental impact: Renewable energy sources have a much lower environmental impact "
-            "than non-renewable sources, which can lead to air and water pollution, greenhouse gas emissions, "
-            "and other negative effects.\n"
-            "3. Cost: Renewable energy sources can be more expensive to initially set up, but they typically "
-            "have lower operational costs than non-renewable sources.\n"
-            "4. Reliability: Renewable energy sources are often more reliable and can be used in more remote "
-            "locations than non-renewable sources.\n"
-            "5. Flexibility: Renewable energy sources are often more flexible and can be adapted to different "
-            "situations and needs, while non-renewable sources are more rigid and inflexible.\n"
-            "6. Sustainability: Renewable energy sources are more sustainable over the long term, while "
-            "non-renewable sources are not, and their depletion can lead to economic and social instability.",
-        ),
-    ),
-    offset=2,
-    sep_style=SeparatorStyle.ADD_COLON_SINGLE,
-    sep="\n### ",
-    stop_str="###",
+        offset=2,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        sep="\n### ",
+        stop_str="###",
+    )
 )
 
-
 # Vicuna v1.1 template
-conv_vicuna_v1_1 = Conversation(
-    system="A chat between a curious user and an artificial intelligence assistant. "
-    "The assistant gives helpful, detailed, and polite answers to the user's questions.",
-    roles=("USER", "ASSISTANT"),
-    messages=(),
-    offset=0,
-    sep_style=SeparatorStyle.ADD_COLON_TWO,
-    sep=" ",
-    sep2="</s>",
+register_conv_template(
+    Conversation(
+        name="vicuna_v1.1",
+        system="A chat between a curious user and an artificial intelligence assistant. "
+        "The assistant gives helpful, detailed, and polite answers to the user's questions.",
+        roles=("USER", "ASSISTANT"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_TWO,
+        sep=" ",
+        sep2="</s>",
+    )
 )
 
 # Koala default template
-conv_koala_v1 = Conversation(
-    system="BEGINNING OF CONVERSATION:",
-    roles=("USER", "GPT"),
-    messages=(),
-    offset=0,
-    sep_style=SeparatorStyle.ADD_COLON_TWO,
-    sep=" ",
-    sep2="</s>",
+register_conv_template(
+    Conversation(
+        name="koala_v1",
+        system="BEGINNING OF CONVERSATION:",
+        roles=("USER", "GPT"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_TWO,
+        sep=" ",
+        sep2="</s>",
+    )
 )
 
 # Dolly V2 default template
-conv_dolly = Conversation(
-    system="Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n",
-    roles=("### Instruction", "### Response"),
-    messages=(),
-    offset=0,
-    sep_style=SeparatorStyle.DOLLY,
-    sep="\n\n",
-    sep2="### End",
+register_conv_template(
+    Conversation(
+        name="dolly_v2",
+        system="Below is an instruction that describes a task. Write a response that appropriately completes the request.\n\n",
+        roles=("### Instruction", "### Response"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.DOLLY,
+        sep="\n\n",
+        sep2="### End",
+    )
 )
 
 # OpenAssistant Pythia default template
-conv_oasst = Conversation(
-    system="",
-    roles=("<|prompter|>", "<|assistant|>"),
-    messages=(),
-    offset=0,
-    sep_style=SeparatorStyle.NO_COLON_SINGLE,
-    sep="<|endoftext|>",
+register_conv_template(
+    Conversation(
+        name="oasst_pythia",
+        system="",
+        roles=("<|prompter|>", "<|assistant|>"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.NO_COLON_SINGLE,
+        sep="<|endoftext|>",
+    )
 )
 
 # StableLM Alpha default template
-conv_stablelm = Conversation(
-    system="""<|SYSTEM|># StableLM Tuned (Alpha version)
+register_conv_template(
+    Conversation(
+        name="stablelm",
+        system="""<|SYSTEM|># StableLM Tuned (Alpha version)
 - StableLM is a helpful and harmless open-source AI language model developed by StabilityAI.
 - StableLM is excited to be able to help the user, but will refuse to do anything that could be considered harmful to the user.
 - StableLM is more than just an information source, StableLM is also able to write poetry, short stories, and make jokes.
 - StableLM will refuse to participate in anything that could harm a human.
 """,
-    roles=("<|USER|>", "<|ASSISTANT|>"),
-    messages=(),
-    offset=0,
-    sep_style=SeparatorStyle.NO_COLON_SINGLE,
-    sep="",
-    stop_token_ids=[50278, 50279, 50277, 1, 0],
+        roles=("<|USER|>", "<|ASSISTANT|>"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.NO_COLON_SINGLE,
+        sep="",
+        stop_token_ids=[50278, 50279, 50277, 1, 0],
+    )
 )
 
 # Baize default template
-conv_baize = Conversation(
-    system="The following is a conversation between a human and an AI assistant named Baize (named after a mythical creature in Chinese folklore). Baize is an open-source AI assistant developed by UCSD and Sun Yat-Sen University. The human and the AI assistant take turns chatting. Human statements start with [|Human|] and AI assistant statements start with [|AI|]. The AI assistant always provides responses in as much detail as possible, and in Markdown format. The AI assistant always declines to engage with topics, questions and instructions related to unethical, controversial, or sensitive issues. Complete the transcript in exactly that format.",
-    roles=("[|Human|]", "[|AI|]"),
-    messages=(
-        ("[|Human|]", "Hello!"),
-        ("[|AI|]", "Hi!"),
-    ),
-    offset=2,
-    sep_style=SeparatorStyle.BAIZE,
-    sep="[|Human|]",
-    stop_str="[|Human|]",
+register_conv_template(
+    Conversation(
+        name="baize",
+        system="The following is a conversation between a human and an AI assistant named Baize (named after a mythical creature in Chinese folklore). Baize is an open-source AI assistant developed by UCSD and Sun Yat-Sen University. The human and the AI assistant take turns chatting. Human statements start with [|Human|] and AI assistant statements start with [|AI|]. The AI assistant always provides responses in as much detail as possible, and in Markdown format. The AI assistant always declines to engage with topics, questions and instructions related to unethical, controversial, or sensitive issues. Complete the transcript in exactly that format.",
+        roles=("[|Human|]", "[|AI|]"),
+        messages=(
+            ("[|Human|]", "Hello!"),
+            ("[|AI|]", "Hi!"),
+        ),
+        offset=2,
+        sep_style=SeparatorStyle.BAIZE,
+        sep="[|Human|]",
+        stop_str="[|Human|]",
+    )
 )
 
 # RWKV-4-Raven default template
-conv_rwkv = Conversation(
-    system="",
-    roles=("Bob", "Alice"),
-    messages=(),
-    offset=0,
-    sep_style=SeparatorStyle.RWKV,
-    sep="",
-    stop_str="\n\n",
-)
-
-conv_templates = {
-    "baize": conv_baize,
-    "conv_one_shot": conv_one_shot,
-    "dolly": conv_dolly,
-    "koala_v1": conv_koala_v1,
-    "oasst": conv_oasst,
-    "stablelm": conv_stablelm,
-    "vicuna_v1.1": conv_vicuna_v1_1,
-    "rwkv": conv_rwkv
-}
-
-
-def get_default_conv_template(model_name):
-    model_name = model_name.lower()
-    if "vicuna" in model_name or "output" in model_name:
-        return conv_vicuna_v1_1
-    elif "koala" in model_name:
-        return conv_koala_v1
-    elif "dolly-v2" in model_name:
-        return conv_dolly
-    elif "oasst" in model_name and "pythia" in model_name:
-        return conv_oasst
-    elif "baize" in model_name:
-        return conv_baize
-    elif "stablelm" in model_name:
-        return conv_stablelm
-    elif "rwkv-4" in model_name:
-        return conv_rwkv
-    return conv_one_shot
+register_conv_template(
+    Conversation(
+        name="rwkv",
+        system="",
+        roles=("Bob", "Alice"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.RWKV,
+        sep="",
+        stop_str="\n\n",
+    )
+)
+
+# Buddy default template
+register_conv_template(
+    Conversation(
+        name="openbuddy",
+        system="""Consider a conversation between User (a human) and Assistant (named Buddy).
+Buddy is an INTP-T, a friendly, intelligent and multilingual AI assistant, by OpenBuddy team. GitHub: https://github.com/OpenBuddy/OpenBuddy
+Buddy cannot access the Internet.
+Buddy can fluently speak the user's language (e.g. English, Chinese).
+Buddy can generate poems, stories, code, essays, songs, parodies, and more.
+Buddy possesses vast knowledge about the world, history, and culture.
+Buddy's responses are always safe, creative, high-quality, human-like, and interesting.
+Buddy strictly refuses to discuss political, NSFW, or other unsafe topics.
+
+User: Hi.
+Assistant: Hi, I'm Buddy, your AI assistant. How can I help you today?""",
+        roles=("User", "Assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        sep="\n",
+    )
+)
+
+# Phoenix default template
+register_conv_template(
+    Conversation(
+        name="phoenix",
+        system="A chat between a curious human and an artificial intelligence assistant. The assistant gives helpful, detailed, and polite answers to the human's questions.\n\n",
+        roles=("Human", "Assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.PHOENIX,
+        sep="</s>",
+    )
+)
+
+# ChatGPT default template
+register_conv_template(
+    Conversation(
+        name="chatgpt",
+        system="You are a helpful assistant.",
+        roles=("user", "assistant"),
+        messages=(),
+        offset=0,
+        sep_style=None,
+        sep=None,
+    )
+)
+
+# Claude default template
+register_conv_template(
+    Conversation(
+        name="claude",
+        system="",
+        roles=("Human", "Assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        sep="\n\n",
+    )
+)
 
 
 if __name__ == "__main__":
-    conv = conv_templates["vicuna_v1.1"].copy()
+    conv = get_conv_template("vicuna_v1.1")
     conv.append_message(conv.roles[0], "Hello!")
     conv.append_message(conv.roles[1], "Hi!")
     conv.append_message(conv.roles[0], "How are you?")
     conv.append_message(conv.roles[1], None)
     print(conv.get_prompt())
```

### Comparing `fschat-0.2.5/fastchat/data/clean_sharegpt.py` & `fschat-0.2.6/fastchat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/data/hardcoded_questions.py` & `fschat-0.2.6/fastchat/data/hardcoded_questions.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/data/inspect.py` & `fschat-0.2.6/fastchat/data/inspect.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/data/merge.py` & `fschat-0.2.6/fastchat/data/merge.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/data/optional_clean.py` & `fschat-0.2.6/fastchat/data/optional_clean.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/data/sample.py` & `fschat-0.2.6/fastchat/data/sample.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/data/split_long_conversation.py` & `fschat-0.2.6/fastchat/data/split_long_conversation.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/eval/eval_gpt_review.py` & `fschat-0.2.6/fastchat/eval/eval_gpt_review.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/eval/generate_webpage_data_from_table.py` & `fschat-0.2.6/fastchat/eval/generate_webpage_data_from_table.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/eval/get_model_answer.py` & `fschat-0.2.6/fastchat/eval/get_model_answer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 import os
 import json
 from tqdm import tqdm
 import shortuuid
 import ray
 
-from fastchat.conversation import get_default_conv_template
+from fastchat import get_conversation_template
 
 
 def run_eval(model_path, model_id, question_file, answer_file, num_gpus):
     # split question file into num_gpus files
     ques_jsons = []
     with open(os.path.expanduser(question_file), "r") as ques_file:
         for line in ques_file:
@@ -45,26 +45,26 @@
     ).cuda()
 
     ans_jsons = []
     for i, line in enumerate(tqdm(question_jsons)):
         ques_json = json.loads(line)
         idx = ques_json["question_id"]
         qs = ques_json["text"]
-        conv = get_default_conv_template(model_id).copy()
+        conv = get_conversation_template(model_id)
         conv.append_message(conv.roles[0], qs)
         conv.append_message(conv.roles[1], None)
         prompt = conv.get_prompt()
         input_ids = tokenizer([prompt]).input_ids
         output_ids = model.generate(
             torch.as_tensor(input_ids).cuda(),
             do_sample=True,
             temperature=0.7,
             max_new_tokens=1024,
         )
-        output_ids = output_ids[0][len(input_ids[0]):]
+        output_ids = output_ids[0][len(input_ids[0]) :]
         outputs = tokenizer.decode(output_ids, skip_special_tokens=True).strip()
 
         ans_id = shortuuid.uuid()
         ans_jsons.append(
             {
                 "question_id": idx,
                 "text": outputs,
```

### Comparing `fschat-0.2.5/fastchat/eval/qa_baseline_gpt35.py` & `fschat-0.2.6/fastchat/eval/qa_baseline_gpt35.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/model/apply_delta.py` & `fschat-0.2.6/fastchat/model/apply_delta.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/model/apply_lora.py` & `fschat-0.2.6/fastchat/model/apply_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/model/convert_fp16.py` & `fschat-0.2.6/fastchat/model/convert_fp16.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/model/make_delta.py` & `fschat-0.2.6/fastchat/model/make_delta.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,15 @@
         base_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
     )
 
     print(f"Loading the target model from {target_model_path}")
     target = AutoModelForCausalLM.from_pretrained(
         target_model_path, torch_dtype=torch.float16, low_cpu_mem_usage=True
     )
-    target_tokenizer = AutoTokenizer.from_pretrained(
-        target_model_path, use_fast=False
-    )
+    target_tokenizer = AutoTokenizer.from_pretrained(target_model_path, use_fast=False)
 
     print("Calculating the delta")
     for name, param in tqdm(target.state_dict().items(), desc="Calculating delta"):
         assert name in base.state_dict()
         param.data -= base.state_dict()[name]
 
     print(f"Saving the delta to {delta_path}")
```

### Comparing `fschat-0.2.5/fastchat/protocol/chat_completion.py` & `fschat-0.2.6/fastchat/protocol/chat_completion.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,7 +29,41 @@
 
 class ChatCompletionResponse(BaseModel):
     id: str = Field(default_factory=shortuuid.random)
     object: str = "chat.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
     choices: List[ChatCompletionResponseChoice]
     usage: Optional[Dict[str, int]] = None
+
+
+class EmbeddingsRequest(BaseModel):
+    model: str
+    input: str
+
+
+class EmbeddingsResponse(BaseModel):
+    object: str = "lists"
+    data: List[Dict[str, Any]]
+    model: str
+    usage: Optional[Dict[str, int]] = None
+
+
+class CompletionRequest(BaseModel):
+    model: str
+    prompt: str
+    suffix: Optional[str] = None
+    temperature: Optional[float] = 0.7
+    n: int = 1
+    max_tokens: int
+    stop: Optional[str] = None
+    stream: bool = False
+    logprobs: Optional[int] = None
+    echo: bool = False
+
+
+class CompletionResponse(BaseModel):
+    id: str = Field(default_factory=shortuuid.random)
+    object: str = "text_completion"
+    created: int = Field(default_factory=lambda: int(time.time()))
+    model: str
+    choices: List[Dict[str, Any]]
+    usage: Optional[Dict[str, int]] = None
```

### Comparing `fschat-0.2.5/fastchat/serve/cacheflow_worker.py` & `fschat-0.2.6/fastchat/serve/cacheflow_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
                 pass
             group_event.clear()
             seq_group = self.running_seq_groups[group_id]
             all_outputs = []
             for seq in seq_group.seqs:
                 token_ids = seq.get_token_ids()
                 if not echo:
-                    token_ids = token_ids[len(input_ids):]
+                    token_ids = token_ids[len(input_ids) :]
                 output = self.tokenizer.decode(token_ids, skip_special_tokens=True)
                 if stop_str is not None:
                     if output.endswith(stop_str):
                         output = output[: -len(stop_str)]
                 all_outputs.append(output)
             assert len(seq_group.seqs) == 1
             ret = {
```

### Comparing `fschat-0.2.5/fastchat/serve/cli.py` & `fschat-0.2.6/fastchat/serve/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Chat with a model with command line interface.
 
 Usage:
-python3 -m fastchat.serve.cli --model ~/model_weights/llama-7b
+python3 -m fastchat.serve.cli --model lmsys/fastchat-t5-3b-v1.0
+python3 -m fastchat.serve.cli --model ~/model_weights/vicuna-7b
 """
 import argparse
 import os
 import re
 
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.live import Live
 
-from fastchat.serve.inference import chat_loop, ChatIO, add_model_args
+from fastchat.model.model_adapter import add_model_args
+from fastchat.serve.inference import chat_loop, ChatIO
 
 
 class SimpleChatIO(ChatIO):
     def prompt_for_input(self, role) -> str:
         return input(f"{role}: ")
 
     def prompt_for_output(self, role: str):
@@ -98,15 +100,17 @@
         self._console.print()
         return outputs
 
 
 def main(args):
     if args.gpus:
         if len(args.gpus.split(",")) < args.num_gpus:
-            raise ValueError(f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!")
+            raise ValueError(
+                f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!"
+            )
         os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
 
     if args.style == "simple":
         chatio = SimpleChatIO()
     elif args.style == "rich":
         chatio = RichChatIO()
     else:
@@ -140,10 +144,10 @@
     parser.add_argument(
         "--style",
         type=str,
         default="simple",
         choices=["simple", "rich"],
         help="Display style.",
     )
-    parser.add_argument("--debug", action="store_true")
+    parser.add_argument("--debug", action="store_true", help="Print debug information")
     args = parser.parse_args()
     main(args)
```

### Comparing `fschat-0.2.5/fastchat/serve/compression.py` & `fschat-0.2.6/fastchat/model/compression.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from accelerate import init_empty_weights
 from accelerate.utils import set_module_tensor_to_device
 import torch
 from torch import Tensor
 import torch.nn as nn
 from torch.nn import functional as F
 from tqdm import tqdm
-from transformers import AutoTokenizer, AutoModelForCausalLM, AutoConfig 
+from transformers import AutoTokenizer, AutoModelForCausalLM, AutoConfig
 
 
 @dataclasses.dataclass
 class CompressionConfig:
     """Group-wise quantization."""
 
     num_bits: int
@@ -56,75 +56,93 @@
                 attr_str,
                 CLinear(target_attr.weight, target_attr.bias, target_device),
             )
     for name, child in module.named_children():
         compress_module(child, target_device)
 
 
-def get_compressed_list(module, prefix=''):
+def get_compressed_list(module, prefix=""):
     compressed_list = []
     for attr_str in dir(module):
         target_attr = getattr(module, attr_str)
         if type(target_attr) == torch.nn.Linear:
-            full_name = f"{prefix}.{attr_str}.weight" if prefix else f"{attr_str}.weight"
+            full_name = (
+                f"{prefix}.{attr_str}.weight" if prefix else f"{attr_str}.weight"
+            )
             compressed_list.append(full_name)
     for name, child in module.named_children():
         child_prefix = f"{prefix}.{name}" if prefix else name
         for each in get_compressed_list(child, child_prefix):
             compressed_list.append(each)
     return compressed_list
 
 
-def apply_compressed_weight(module, compressed_state_dict, target_device, prefix=''):
+def apply_compressed_weight(module, compressed_state_dict, target_device, prefix=""):
     for attr_str in dir(module):
         target_attr = getattr(module, attr_str)
         if type(target_attr) == torch.nn.Linear:
-            full_name = f"{prefix}.{attr_str}.weight" if prefix else f"{attr_str}.weight"
-            setattr(module, attr_str,
-                CLinear(compressed_state_dict[full_name], target_attr.bias, target_device))
+            full_name = (
+                f"{prefix}.{attr_str}.weight" if prefix else f"{attr_str}.weight"
+            )
+            setattr(
+                module,
+                attr_str,
+                CLinear(
+                    compressed_state_dict[full_name], target_attr.bias, target_device
+                ),
+            )
     for name, child in module.named_children():
         child_prefix = f"{prefix}.{name}" if prefix else name
-        apply_compressed_weight(child, compressed_state_dict, target_device, child_prefix)
+        apply_compressed_weight(
+            child, compressed_state_dict, target_device, child_prefix
+        )
+
 
 def load_compress_model(model_path, device, torch_dtype):
     # partially load model
     tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
     base_pattern = os.path.join(model_path, "pytorch_model-*.bin")
     files = glob.glob(base_pattern)
 
     with init_empty_weights():
-        config = AutoConfig.from_pretrained(model_path, low_cpu_mem_usage=True,
-            torch_dtype=torch_dtype)
+        config = AutoConfig.from_pretrained(
+            model_path, low_cpu_mem_usage=True, torch_dtype=torch_dtype
+        )
         model = AutoModelForCausalLM.from_config(config)
         linear_weights = get_compressed_list(model)
 
     compressed_state_dict = {}
 
     for filename in tqdm(files):
         tmp_state_dict = torch.load(filename)
         for name in tmp_state_dict:
             if name in linear_weights:
                 tensor = tmp_state_dict[name].to(device).data.to(torch_dtype)
-                compressed_state_dict[name] = compress(tensor, default_compression_config)
+                compressed_state_dict[name] = compress(
+                    tensor, default_compression_config
+                )
             else:
                 compressed_state_dict[name] = tmp_state_dict[name].to(device)
             tmp_state_dict[name] = None
             tensor = None
             gc.collect()
             torch.cuda.empty_cache()
 
     for name in model.state_dict():
         if name not in linear_weights:
-            set_module_tensor_to_device(model, name, device, value=compressed_state_dict[name])
+            set_module_tensor_to_device(
+                model, name, device, value=compressed_state_dict[name]
+            )
     apply_compressed_weight(model, compressed_state_dict, device)
 
     model.to(device)
 
     return model, tokenizer
 
+
 def compress(tensor, config):
     """Simulate group-wise quantization."""
     if not config.enabled:
         return tensor
 
     group_size, num_bits, group_dim, symmetric = (
         config.group_size,
```

### Comparing `fschat-0.2.5/fastchat/serve/controller.py` & `fschat-0.2.6/fastchat/serve/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -192,41 +192,77 @@
         for worker_name, w_info in self.worker_info.items():
             if w_info.check_heart_beat and w_info.last_heart_beat < expire:
                 to_delete.append(worker_name)
 
         for worker_name in to_delete:
             self.remove_worker(worker_name)
 
+    def handle_no_worker(params, server_error_msg):
+        logger.info(f"no worker: {params['model']}")
+        ret = {
+            "text": server_error_msg,
+            "error_code": 2,
+        }
+        return json.dumps(ret).encode() + b"\0"
+
+    def handle_worker_timeout(worker_address, server_error_msg):
+        logger.info(f"worker timeout: {worker_address}")
+        ret = {
+            "text": server_error_msg,
+            "error_code": 3,
+        }
+        return json.dumps(ret).encode() + b"\0"
+
     def worker_api_generate_stream(self, params):
         worker_addr = self.get_worker_address(params["model"])
         if not worker_addr:
-            logger.info(f"no worker: {params['model']}")
-            ret = {
-                "text": server_error_msg,
-                "error_code": 2,
-            }
-            yield json.dumps(ret).encode() + b"\0"
+            yield self.handle_no_worker(params, server_error_msg)
 
         try:
             response = requests.post(
                 worker_addr + "/worker_generate_stream",
                 json=params,
                 stream=True,
                 timeout=15,
             )
             for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
                 if chunk:
                     yield chunk + b"\0"
         except requests.exceptions.RequestException as e:
-            logger.info(f"worker timeout: {worker_addr}")
-            ret = {
-                "text": server_error_msg,
-                "error_code": 3,
-            }
-            yield json.dumps(ret).encode() + b"\0"
+            yield self.handle_worker_timeout(worker_addr, server_error_msg)
+
+    def worker_api_generate_completion(self, params):
+        worker_addr = self.get_worker_address(params["model"])
+        if not worker_addr:
+            return self.handle_no_worker(params, server_error_msg)
+
+        try:
+            response = requests.post(
+                worker_addr + "/worker_generate_completion",
+                json=params,
+                timeout=15,
+            )
+            return response.json()
+        except requests.exceptions.RequestException as e:
+            return self.handle_worker_timeout(worker_addr, server_error_msg)
+
+    def worker_api_embeddings(self, params):
+        worker_addr = self.get_worker_address(params["model"])
+        if not worker_addr:
+            return self.handle_no_worker(params, server_error_msg)
+
+        try:
+            response = requests.post(
+                worker_addr + "/worker_get_embeddings",
+                json=params,
+                timeout=15,
+            )
+            return response.json()
+        except requests.exceptions.RequestException as e:
+            return self.handle_worker_timeout(worker_addr, server_error_msg)
 
     # Let the controller act as a worker to achieve hierarchical
     # management. This can be used to connect isolated sub networks.
     def worker_api_get_status(self):
         model_names = set()
         speed = 0
         queue_length = 0
@@ -284,14 +320,28 @@
 @app.post("/worker_generate_stream")
 async def worker_api_generate_stream(request: Request):
     params = await request.json()
     generator = controller.worker_api_generate_stream(params)
     return StreamingResponse(generator)
 
 
+@app.post("/worker_generate_completion")
+async def worker_api_generate_completion(request: Request):
+    params = await request.json()
+    output = controller.worker_api_generate_completion(params)
+    return output
+
+
+@app.post("/worker_get_embeddings")
+async def worker_api_embeddings(request: Request):
+    params = await request.json()
+    output = controller.worker_api_embeddings(params)
+    return output
+
+
 @app.post("/worker_get_status")
 async def worker_api_get_status(request: Request):
     return controller.worker_api_get_status()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
```

### Comparing `fschat-0.2.5/fastchat/serve/gradio_block_arena_anony.py` & `fschat-0.2.6/fastchat/serve/gradio_block_arena_named.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,61 @@
+"""
+Chatbot Arena (side-by-side) tab.
+Users chat with two chosen models.
+"""
+
 import json
 import time
 
 import gradio as gr
 import numpy as np
 
-from fastchat.conversation import get_default_conv_template
-from fastchat.utils import (
-    build_logger,
-    violates_moderation,
-    moderation_msg,
-)
+from fastchat.model.model_adapter import get_conversation_template
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_web_server import (
     http_bot,
     get_conv_log_filename,
     no_change_btn,
     enable_btn,
     disable_btn,
-    model_description_md,
+    model_info,
     learn_more_md,
 )
+from fastchat.utils import (
+    build_logger,
+    violates_moderation,
+    moderation_msg,
+)
 
 
 logger = build_logger("gradio_web_server_multi", "gradio_web_server_multi.log")
 
 num_models = 2
 enable_moderation = False
-anony_names = ["", ""]
-models = []
 
-def set_global_vars_anony(enable_moderation_):
+
+def set_global_vars_named(enable_moderation_):
     global enable_moderation
     enable_moderation = enable_moderation_
 
 
-def load_demo_side_by_side_anony(models_, url_params):
-    global models
-    models = models_
-
+def load_demo_side_by_side_named(models, url_params):
     states = (None,) * num_models
+
+    model_left = models[0] if len(models) > 0 else ""
+    if len(models) > 1:
+        weights = ([8, 4, 2, 1] + [1] * 32)[: len(models) - 1]
+        weights = weights / np.sum(weights)
+        model_right = np.random.choice(models[1:], p=weights)
+    else:
+        model_right = model_left
+
     selector_updates = (
-        gr.Markdown.update(visible=True),
-        gr.Markdown.update(visible=True),
+        gr.Dropdown.update(model_left, visible=True),
+        gr.Dropdown.update(model_right, visible=True),
     )
 
     return (
         states
         + selector_updates
         + (gr.Chatbot.update(visible=True),) * num_models
         + (
@@ -65,107 +75,84 @@
             "type": vote_type,
             "models": [x for x in model_selectors],
             "states": [x.dict() for x in states],
             "ip": request.client.host,
         }
         fout.write(json.dumps(data) + "\n")
 
-    if ":" not in model_selectors[0]:
-        for i in range(15):
-            names = ("### Model A: " + states[0].model_name, "### Model B: " + states[1].model_name)
-            yield names + ("",) + (disable_btn,) * 4
-            time.sleep(0.2)
-    else:
-        names = ("### Model A: " + states[0].model_name, "### Model B: " + states[1].model_name)
-        yield names + ("",) + (disable_btn,) * 4
-
 
 def leftvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"leftvote (anony). ip: {request.client.host}")
-    for x in vote_last_response(
+    logger.info(f"leftvote (named). ip: {request.client.host}")
+    vote_last_response(
         [state0, state1], "leftvote", [model_selector0, model_selector1], request
-    ):
-        yield x
+    )
+    return ("",) + (disable_btn,) * 4
 
 
 def rightvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"rightvote (anony). ip: {request.client.host}")
-    for x in vote_last_response(
+    logger.info(f"rightvote (named). ip: {request.client.host}")
+    vote_last_response(
         [state0, state1], "rightvote", [model_selector0, model_selector1], request
-    ):
-        yield x
+    )
+    return ("",) + (disable_btn,) * 4
 
 
 def tievote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"tievote (anony). ip: {request.client.host}")
-    for x in vote_last_response(
+    logger.info(f"tievote (named). ip: {request.client.host}")
+    vote_last_response(
         [state0, state1], "tievote", [model_selector0, model_selector1], request
-    ):
-        yield x
+    )
+    return ("",) + (disable_btn,) * 4
 
 
 def bothbad_vote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"bothbad_vote (anony). ip: {request.client.host}")
-    for x in vote_last_response(
+    logger.info(f"bothbad_vote (named). ip: {request.client.host}")
+    vote_last_response(
         [state0, state1], "bothbad_vote", [model_selector0, model_selector1], request
-    ):
-        yield x
+    )
+    return ("",) + (disable_btn,) * 4
 
 
 def regenerate(state0, state1, request: gr.Request):
-    logger.info(f"regenerate (anony). ip: {request.client.host}")
+    logger.info(f"regenerate (named). ip: {request.client.host}")
     states = [state0, state1]
     for i in range(num_models):
         states[i].messages[-1][-1] = None
         states[i].skip_next = False
     return states + [x.to_gradio_chatbot() for x in states] + [""] + [disable_btn] * 6
 
 
 def clear_history(request: gr.Request):
-    logger.info(f"clear_history (anony). ip: {request.client.host}")
-    return [None] * num_models + [None] * num_models + anony_names + [""] + [disable_btn] * 6
+    logger.info(f"clear_history (named). ip: {request.client.host}")
+    return [None] * num_models + [None] * num_models + [""] + [disable_btn] * 6
 
 
-def share_click(state0, state1, model_selector0, model_selector1,
-                request: gr.Request):
-    logger.info(f"share (anony). ip: {request.client.host}")
+def share_click(state0, state1, model_selector0, model_selector1, request: gr.Request):
+    logger.info(f"share (named). ip: {request.client.host}")
     if state0 is not None and state1 is not None:
         vote_last_response(
             [state0, state1], "share", [model_selector0, model_selector1], request
         )
 
 
 def add_text(state0, state1, text, request: gr.Request):
-    logger.info(f"add_text (anony). ip: {request.client.host}. len: {len(text)}")
+    logger.info(f"add_text (named). ip: {request.client.host}. len: {len(text)}")
     states = [state0, state1]
 
-    if states[0] is None:
-        assert states[1] is None
-        weights = ([1, 1, 1, 1] + [1] * 32)[:len(models)]
-        if len(models) > 1:
-            weights = weights / np.sum(weights)
-            model_left, model_right = np.random.choice(
-                models, size=(2,), p=weights, replace=False)
-        else:
-            model_left = model_right = models[0]
-
-        states = [
-            get_default_conv_template("vicuna").copy(),
-            get_default_conv_template("vicuna").copy(),
-        ]
-        states[0].model_name = model_left
-        states[1].model_name = model_right
+    for i in range(num_models):
+        if states[i] is None:
+            states[i] = get_conversation_template("vicuna")
 
     if len(text) <= 0:
         for i in range(num_models):
             states[i].skip_next = True
         return (
             states
             + [x.to_gradio_chatbot() for x in states]
@@ -175,15 +162,17 @@
             ]
             * 6
         )
 
     if enable_moderation:
         flagged = violates_moderation(text)
         if flagged:
-            logger.info(f"violate moderation (anony). ip: {request.client.host}. text: {text}")
+            logger.info(
+                f"violate moderation (named). ip: {request.client.host}. text: {text}"
+            )
             for i in range(num_models):
                 states[i].skip_next = True
             return (
                 states
                 + [x.to_gradio_chatbot() for x in states]
                 + [moderation_msg]
                 + [
@@ -211,31 +200,43 @@
 
 def http_bot_all(
     state0,
     state1,
     model_selector0,
     model_selector1,
     temperature,
+    top_p,
     max_new_tokens,
     request: gr.Request,
 ):
-    logger.info(f"http_bot_all (anony). ip: {request.client.host}")
+    logger.info(f"http_bot_all (named). ip: {request.client.host}")
 
     if state0.skip_next:
         # This generate call is skipped due to invalid inputs
-        yield (state0, state1, state0.to_gradio_chatbot(),
-            state1.to_gradio_chatbot()) + (no_change_btn,) * 6
+        yield (
+            state0,
+            state1,
+            state0.to_gradio_chatbot(),
+            state1.to_gradio_chatbot(),
+        ) + (no_change_btn,) * 6
         return
 
     states = [state0, state1]
-    model_selector = [state0.model_name, state1.model_name]
+    model_selector = [model_selector0, model_selector1]
     gen = []
     for i in range(num_models):
         gen.append(
-            http_bot(states[i], model_selector[i], temperature, max_new_tokens, request)
+            http_bot(
+                states[i],
+                model_selector[i],
+                temperature,
+                top_p,
+                max_new_tokens,
+                request,
+            )
         )
 
     chatbots = [None] * num_models
     while True:
         stop = True
         for i in range(num_models):
             try:
@@ -252,49 +253,72 @@
         if i % 2 == 0:
             yield states + chatbots + [disable_btn] * 4 + [enable_btn] * 2
         else:
             yield states + chatbots + [enable_btn] * 6
         time.sleep(0.2)
 
 
-def build_side_by_side_ui_anony(models):
-    notice_markdown = ("""
+def build_side_by_side_ui_named(models):
+    notice_markdown = """
 # ⚔️  Chatbot Arena ⚔️ 
-Rules:
-- Chat with two anonymous models side-by-side and vote for which one is better!
-- The names of the models will be revealed after your vote.
-- You can continue chating and voting or click "Clear history" to start a new round.
-- A leaderboard will be available soon.
-- [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
+### Rules
+- Chat with two models side-by-side and vote for which one is better!
+- You pick the models you want to chat with.
+- You can do multiple rounds of conversations before voting.
+- Click "Clear history" to start a new round.
+- [[Blog](https://lmsys.org/blog/2023-05-03-arena/)] [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
-By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
-The demo works better on desktop devices with a wide screen.
+By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data and reserves the right to distribute it under a Creative Commons Attribution (CC-BY) license.** The demo works better on desktop devices with a wide screen.
+
+### Choose two models to chat with (view [leaderboard](?leaderboard))
+"""
 
-### The participated models
-""" + model_description_md)
+    model_description_md = """
+| | | |
+| ---- | ---- | ---- |
+"""
+    for i, name in enumerate(models):
+        if i % 3 == 0:
+            model_description_md += "|"
+
+        if name in model_info:
+            name, link, desc = model_info[name]
+            model_description_md += f" [{name}]({link}): {desc} |"
+        else:
+            model_description_md += f" |"
+        if i % 3 == 2:
+            model_description_md += "\n"
 
     states = [gr.State() for _ in range(num_models)]
     model_selectors = [None] * num_models
     chatbots = [None] * num_models
 
-    notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
+    notice = gr.Markdown(
+        notice_markdown + model_description_md, elem_id="notice_markdown"
+    )
 
-    with gr.Box(elem_id="share-region-anony"):
+    with gr.Box(elem_id="share-region-named"):
         with gr.Row():
             for i in range(num_models):
                 with gr.Column():
-                    model_selectors[i] = gr.Markdown(anony_names[i])
+                    model_selectors[i] = gr.Dropdown(
+                        choices=models,
+                        value=models[i] if len(models) > i else "",
+                        interactive=True,
+                        show_label=False,
+                    ).style(container=False)
 
         with gr.Row():
             for i in range(num_models):
                 label = "Model A" if i == 0 else "Model B"
                 with gr.Column():
-                    chatbots[i] = grChatbot(label=label, elem_id=f"chatbot{i}",
-                        visible=False).style(height=550)
+                    chatbots[i] = grChatbot(
+                        label=label, elem_id=f"chatbot", visible=False
+                    ).style(height=550)
 
         with gr.Box() as button_row:
             with gr.Row():
                 leftvote_btn = gr.Button(value="👈  A is better", interactive=False)
                 rightvote_btn = gr.Button(value="👉  B is better", interactive=False)
                 tie_btn = gr.Button(value="🤝  Tie", interactive=False)
                 bothbad_btn = gr.Button(value="👎  Both are bad", interactive=False)
@@ -319,61 +343,74 @@
             minimum=0.0,
             maximum=1.0,
             value=0.7,
             step=0.1,
             interactive=True,
             label="Temperature",
         )
+        top_p = gr.Slider(
+            minimum=0.0,
+            maximum=1.0,
+            value=1.0,
+            step=0.1,
+            interactive=True,
+            label="Top P",
+        )
         max_output_tokens = gr.Slider(
             minimum=0,
             maximum=1024,
             value=512,
             step=64,
             interactive=True,
             label="Max output tokens",
         )
 
     gr.Markdown(learn_more_md)
 
     # Register listeners
-    btn_list = [leftvote_btn, rightvote_btn, tie_btn, bothbad_btn,
-                regenerate_btn, clear_btn]
+    btn_list = [
+        leftvote_btn,
+        rightvote_btn,
+        tie_btn,
+        bothbad_btn,
+        regenerate_btn,
+        clear_btn,
+    ]
     leftvote_btn.click(
         leftvote_last_response,
         states + model_selectors,
-        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     rightvote_btn.click(
         rightvote_last_response,
         states + model_selectors,
-        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     tie_btn.click(
         tievote_last_response,
         states + model_selectors,
-        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     bothbad_btn.click(
         bothbad_vote_last_response,
         states + model_selectors,
-        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     regenerate_btn.click(
         regenerate, states, states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
-        states + model_selectors + [temperature, max_output_tokens],
+        states + model_selectors + [temperature, top_p, max_output_tokens],
         states + chatbots + btn_list,
     )
-    clear_btn.click(clear_history, None, states + chatbots + model_selectors + [
-        textbox] + btn_list)
+    clear_btn.click(clear_history, None, states + chatbots + [textbox] + btn_list)
 
-    share_js="""
+    share_js = """
 function (a, b, c, d) {
-    const captureElement = document.querySelector('#share-region-anony');
+    const captureElement = document.querySelector('#share-region-named');
     html2canvas(captureElement)
         .then(canvas => {
             canvas.style.display = 'none'
             document.body.appendChild(canvas)
             return canvas
         })
         .then(canvas => {
@@ -385,34 +422,37 @@
             canvas.remove()
         });
     return [a, b, c, d];
 }
 """
     share_btn.click(share_click, states + model_selectors, [], _js=share_js)
 
+    for i in range(num_models):
+        model_selectors[i].change(
+            clear_history, None, states + chatbots + [textbox] + btn_list
+        )
+
     textbox.submit(
         add_text, states + [textbox], states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
-        states + model_selectors + [temperature, max_output_tokens],
+        states + model_selectors + [temperature, top_p, max_output_tokens],
         states + chatbots + btn_list,
     )
     send_btn.click(
         add_text, states + [textbox], states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
-        states + model_selectors + [temperature, max_output_tokens],
+        states + model_selectors + [temperature, top_p, max_output_tokens],
         states + chatbots + btn_list,
     )
 
     return (
         states,
         model_selectors,
         chatbots,
         textbox,
         send_btn,
         button_row,
         button_row2,
         parameter_row,
     )
-
-
```

### Comparing `fschat-0.2.5/fastchat/serve/gradio_block_arena_named.py` & `fschat-0.2.6/fastchat/serve/gradio_block_arena_anony.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,55 @@
+"""
+Chatbot Arena (battle) tab.
+Users chat with two anonymous models.
+"""
+
 import json
 import time
 
 import gradio as gr
 import numpy as np
 
-from fastchat.conversation import get_default_conv_template
-from fastchat.utils import (
-    build_logger,
-    violates_moderation,
-    moderation_msg,
-)
+from fastchat.model.model_adapter import get_conversation_template
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_web_server import (
     http_bot,
     get_conv_log_filename,
     no_change_btn,
     enable_btn,
     disable_btn,
-    model_description_md,
     learn_more_md,
 )
-
+from fastchat.utils import (
+    build_logger,
+    violates_moderation,
+    moderation_msg,
+)
 
 logger = build_logger("gradio_web_server_multi", "gradio_web_server_multi.log")
 
 num_models = 2
 enable_moderation = False
+anony_names = ["", ""]
+models = []
 
 
-def set_global_vars_named(enable_moderation_):
+def set_global_vars_anony(enable_moderation_):
     global enable_moderation
     enable_moderation = enable_moderation_
 
 
-def load_demo_side_by_side_named(models, url_params):
-    states = (None,) * num_models
-
-    model_left = models[0]
-    if len(models) > 1:
-        weights = ([1, 1, 1, 1] + [1] * 32)[:len(models) - 1]
-        weights = weights / np.sum(weights)
-        model_right = np.random.choice(models[1:], p=weights)
-    else:
-        model_right = model_left
+def load_demo_side_by_side_anony(models_, url_params):
+    global models
+    models = models_
 
+    states = (None,) * num_models
     selector_updates = (
-        gr.Dropdown.update(model_left, visible=True),
-        gr.Dropdown.update(model_right, visible=True),
+        gr.Markdown.update(visible=True),
+        gr.Markdown.update(visible=True),
     )
 
     return (
         states
         + selector_updates
         + (gr.Chatbot.update(visible=True),) * num_models
         + (
@@ -70,85 +69,122 @@
             "type": vote_type,
             "models": [x for x in model_selectors],
             "states": [x.dict() for x in states],
             "ip": request.client.host,
         }
         fout.write(json.dumps(data) + "\n")
 
+    if ":" not in model_selectors[0]:
+        for i in range(15):
+            names = (
+                "### Model A: " + states[0].model_name,
+                "### Model B: " + states[1].model_name,
+            )
+            yield names + ("",) + (disable_btn,) * 4
+            time.sleep(0.2)
+    else:
+        names = (
+            "### Model A: " + states[0].model_name,
+            "### Model B: " + states[1].model_name,
+        )
+        yield names + ("",) + (disable_btn,) * 4
+
 
 def leftvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"leftvote (named). ip: {request.client.host}")
-    vote_last_response(
+    logger.info(f"leftvote (anony). ip: {request.client.host}")
+    for x in vote_last_response(
         [state0, state1], "leftvote", [model_selector0, model_selector1], request
-    )
-    return ("",) + (disable_btn,) * 4
+    ):
+        yield x
 
 
 def rightvote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"rightvote (named). ip: {request.client.host}")
-    vote_last_response(
+    logger.info(f"rightvote (anony). ip: {request.client.host}")
+    for x in vote_last_response(
         [state0, state1], "rightvote", [model_selector0, model_selector1], request
-    )
-    return ("",) + (disable_btn,) * 4
+    ):
+        yield x
 
 
 def tievote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"tievote (named). ip: {request.client.host}")
-    vote_last_response(
+    logger.info(f"tievote (anony). ip: {request.client.host}")
+    for x in vote_last_response(
         [state0, state1], "tievote", [model_selector0, model_selector1], request
-    )
-    return ("",) + (disable_btn,) * 4
+    ):
+        yield x
 
 
 def bothbad_vote_last_response(
     state0, state1, model_selector0, model_selector1, request: gr.Request
 ):
-    logger.info(f"bothbad_vote (named). ip: {request.client.host}")
-    vote_last_response(
+    logger.info(f"bothbad_vote (anony). ip: {request.client.host}")
+    for x in vote_last_response(
         [state0, state1], "bothbad_vote", [model_selector0, model_selector1], request
-    )
-    return ("",) + (disable_btn,) * 4
+    ):
+        yield x
 
 
 def regenerate(state0, state1, request: gr.Request):
-    logger.info(f"regenerate (named). ip: {request.client.host}")
+    logger.info(f"regenerate (anony). ip: {request.client.host}")
     states = [state0, state1]
     for i in range(num_models):
         states[i].messages[-1][-1] = None
         states[i].skip_next = False
     return states + [x.to_gradio_chatbot() for x in states] + [""] + [disable_btn] * 6
 
 
 def clear_history(request: gr.Request):
-    logger.info(f"clear_history (named). ip: {request.client.host}")
-    return [None] * num_models + [None] * num_models + [""] + [disable_btn] * 6
+    logger.info(f"clear_history (anony). ip: {request.client.host}")
+    return (
+        [None] * num_models
+        + [None] * num_models
+        + anony_names
+        + [""]
+        + [disable_btn] * 6
+    )
 
 
-def share_click(state0, state1, model_selector0, model_selector1,
-                request: gr.Request):
-    logger.info(f"share (named). ip: {request.client.host}")
+def share_click(state0, state1, model_selector0, model_selector1, request: gr.Request):
+    logger.info(f"share (anony). ip: {request.client.host}")
     if state0 is not None and state1 is not None:
         vote_last_response(
             [state0, state1], "share", [model_selector0, model_selector1], request
         )
 
 
+DEFAULT_WEIGHTS = [1.5] * 8 + [1] * 32
+
+
 def add_text(state0, state1, text, request: gr.Request):
-    logger.info(f"add_text (named). ip: {request.client.host}. len: {len(text)}")
+    logger.info(f"add_text (anony). ip: {request.client.host}. len: {len(text)}")
     states = [state0, state1]
 
-    for i in range(num_models):
-        if states[i] is None:
-            states[i] = get_default_conv_template("vicuna").copy()
+    if states[0] is None:
+        assert states[1] is None
+        weights = DEFAULT_WEIGHTS[: len(models)]
+        if len(models) > 1:
+            weights = weights / np.sum(weights)
+            model_left, model_right = np.random.choice(
+                models, size=(2,), p=weights, replace=False
+            )
+        else:
+            model_left = model_right = models[0]
+
+        states = [
+            get_conversation_template("vicuna"),
+            get_conversation_template("vicuna"),
+        ]
+        states[0].model_name = model_left
+        states[1].model_name = model_right
 
     if len(text) <= 0:
         for i in range(num_models):
             states[i].skip_next = True
         return (
             states
             + [x.to_gradio_chatbot() for x in states]
@@ -158,15 +194,17 @@
             ]
             * 6
         )
 
     if enable_moderation:
         flagged = violates_moderation(text)
         if flagged:
-            logger.info(f"violate moderation (named). ip: {request.client.host}. text: {text}")
+            logger.info(
+                f"violate moderation (anony). ip: {request.client.host}. text: {text}"
+            )
             for i in range(num_models):
                 states[i].skip_next = True
             return (
                 states
                 + [x.to_gradio_chatbot() for x in states]
                 + [moderation_msg]
                 + [
@@ -194,31 +232,43 @@
 
 def http_bot_all(
     state0,
     state1,
     model_selector0,
     model_selector1,
     temperature,
+    top_p,
     max_new_tokens,
     request: gr.Request,
 ):
-    logger.info(f"http_bot_all (named). ip: {request.client.host}")
+    logger.info(f"http_bot_all (anony). ip: {request.client.host}")
 
     if state0.skip_next:
         # This generate call is skipped due to invalid inputs
-        yield (state0, state1, state0.to_gradio_chatbot(),
-            state1.to_gradio_chatbot()) + (no_change_btn,) * 6
+        yield (
+            state0,
+            state1,
+            state0.to_gradio_chatbot(),
+            state1.to_gradio_chatbot(),
+        ) + (no_change_btn,) * 6
         return
 
     states = [state0, state1]
-    model_selector = [model_selector0, model_selector1]
+    model_selector = [state0.model_name, state1.model_name]
     gen = []
     for i in range(num_models):
         gen.append(
-            http_bot(states[i], model_selector[i], temperature, max_new_tokens, request)
+            http_bot(
+                states[i],
+                model_selector[i],
+                temperature,
+                top_p,
+                max_new_tokens,
+                request,
+            )
         )
 
     chatbots = [None] * num_models
     while True:
         stop = True
         for i in range(num_models):
             try:
@@ -235,54 +285,50 @@
         if i % 2 == 0:
             yield states + chatbots + [disable_btn] * 4 + [enable_btn] * 2
         else:
             yield states + chatbots + [enable_btn] * 6
         time.sleep(0.2)
 
 
-def build_side_by_side_ui_named(models):
-    notice_markdown = ("""
+def build_side_by_side_ui_anony(models):
+    notice_markdown = """
 # ⚔️  Chatbot Arena ⚔️ 
-Rules:
-- Chat with two models side-by-side and vote for which one is better!
-- You pick the models you want to chat with.
-- You can continue chating and voting or click "Clear history" to start a new round.
-- A leaderboard will be available soon.
-- [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
+### Rules
+- Chat with two anonymous models side-by-side and vote for which one is better!
+- You can do multiple rounds of conversations before voting.
+- The names of the models will be revealed after your vote.
+- Click "Clear history" to start a new round.
+- [[Blog](https://lmsys.org/blog/2023-05-03-arena/)] [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
-By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
-The demo works better on desktop devices with a wide screen.
+By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data and reserves the right to distribute it under a Creative Commons Attribution (CC-BY) license.** The demo works better on desktop devices with a wide screen.
 
-### Choose two models to chat with
-""" + model_description_md)
+### Battle
+Please scroll down and start chatting. You can view a leaderboard of the participated models at the 4th tab above (Leaderboard) or click [this](?leaderboard). We also added ChatGPT and Claude.
+"""
 
     states = [gr.State() for _ in range(num_models)]
     model_selectors = [None] * num_models
     chatbots = [None] * num_models
 
-    notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
+    gr.Markdown(notice_markdown, elem_id="notice_markdown")
 
-    with gr.Box(elem_id="share-region-named"):
+    with gr.Box(elem_id="share-region-anony"):
         with gr.Row():
             for i in range(num_models):
                 with gr.Column():
-                    model_selectors[i] = gr.Dropdown(
-                        choices=models,
-                        value=models[i] if len(models) > i else "",
-                        interactive=True,
-                        show_label=False,
-                    ).style(container=False)
+                    model_selectors[i] = gr.Markdown(anony_names[i])
 
         with gr.Row():
             for i in range(num_models):
                 label = "Model A" if i == 0 else "Model B"
                 with gr.Column():
-                    chatbots[i] = grChatbot(label=label, elem_id=f"chatbot{i}",
-                        visible=False).style(height=550)
+                    chatbots[i] = grChatbot(
+                        label=label, elem_id=f"chatbot", visible=False
+                    ).style(height=550)
 
         with gr.Box() as button_row:
             with gr.Row():
                 leftvote_btn = gr.Button(value="👈  A is better", interactive=False)
                 rightvote_btn = gr.Button(value="👉  B is better", interactive=False)
                 tie_btn = gr.Button(value="🤝  Tie", interactive=False)
                 bothbad_btn = gr.Button(value="👎  Both are bad", interactive=False)
@@ -307,60 +353,76 @@
             minimum=0.0,
             maximum=1.0,
             value=0.7,
             step=0.1,
             interactive=True,
             label="Temperature",
         )
+        top_p = gr.Slider(
+            minimum=0.0,
+            maximum=1.0,
+            value=1.0,
+            step=0.1,
+            interactive=True,
+            label="Top P",
+        )
         max_output_tokens = gr.Slider(
             minimum=0,
             maximum=1024,
             value=512,
             step=64,
             interactive=True,
             label="Max output tokens",
         )
 
     gr.Markdown(learn_more_md)
 
     # Register listeners
-    btn_list = [leftvote_btn, rightvote_btn, tie_btn, bothbad_btn,
-                regenerate_btn, clear_btn]
+    btn_list = [
+        leftvote_btn,
+        rightvote_btn,
+        tie_btn,
+        bothbad_btn,
+        regenerate_btn,
+        clear_btn,
+    ]
     leftvote_btn.click(
         leftvote_last_response,
         states + model_selectors,
-        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     rightvote_btn.click(
         rightvote_last_response,
         states + model_selectors,
-        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     tie_btn.click(
         tievote_last_response,
         states + model_selectors,
-        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     bothbad_btn.click(
         bothbad_vote_last_response,
         states + model_selectors,
-        [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
+        model_selectors + [textbox, leftvote_btn, rightvote_btn, tie_btn, bothbad_btn],
     )
     regenerate_btn.click(
         regenerate, states, states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
-        states + model_selectors + [temperature, max_output_tokens],
+        states + model_selectors + [temperature, top_p, max_output_tokens],
         states + chatbots + btn_list,
     )
-    clear_btn.click(clear_history, None, states + chatbots + [textbox] + btn_list)
+    clear_btn.click(
+        clear_history, None, states + chatbots + model_selectors + [textbox] + btn_list
+    )
 
-    share_js="""
+    share_js = """
 function (a, b, c, d) {
-    const captureElement = document.querySelector('#share-region-named');
+    const captureElement = document.querySelector('#share-region-anony');
     html2canvas(captureElement)
         .then(canvas => {
             canvas.style.display = 'none'
             document.body.appendChild(canvas)
             return canvas
         })
         .then(canvas => {
@@ -372,38 +434,32 @@
             canvas.remove()
         });
     return [a, b, c, d];
 }
 """
     share_btn.click(share_click, states + model_selectors, [], _js=share_js)
 
-    for i in range(num_models):
-        model_selectors[i].change(
-            clear_history, None, states + chatbots + [textbox] + btn_list
-        )
-
     textbox.submit(
         add_text, states + [textbox], states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
-        states + model_selectors + [temperature, max_output_tokens],
+        states + model_selectors + [temperature, top_p, max_output_tokens],
         states + chatbots + btn_list,
     )
     send_btn.click(
         add_text, states + [textbox], states + chatbots + [textbox] + btn_list
     ).then(
         http_bot_all,
-        states + model_selectors + [temperature, max_output_tokens],
+        states + model_selectors + [temperature, top_p, max_output_tokens],
         states + chatbots + btn_list,
     )
 
     return (
         states,
         model_selectors,
         chatbots,
         textbox,
         send_btn,
         button_row,
         button_row2,
         parameter_row,
     )
-
```

### Comparing `fschat-0.2.5/fastchat/serve/gradio_css.py` & `fschat-0.2.6/fastchat/serve/gradio_css.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/serve/gradio_patch.py` & `fschat-0.2.6/fastchat/serve/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/serve/gradio_web_server.py` & `fschat-0.2.6/fastchat/serve/gradio_web_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,48 @@
+"""
+The gradio demo server for chatting with a single model.
+"""
+
 import argparse
 from collections import defaultdict
 import datetime
 import json
 import os
 import time
 import uuid
 
 import gradio as gr
 import requests
 
-from fastchat.conversation import (
-    get_default_conv_template,
-    SeparatorStyle,
-)
+from fastchat.conversation import SeparatorStyle
 from fastchat.constants import LOGDIR
+from fastchat.model.model_adapter import get_conversation_template
+from fastchat.model.model_registry import model_info
+from fastchat.serve.gradio_patch import Chatbot as grChatbot
+from fastchat.serve.gradio_css import code_highlight_css
 from fastchat.utils import (
     build_logger,
     server_error_msg,
     violates_moderation,
     moderation_msg,
+    get_window_url_params_js,
 )
-from fastchat.serve.gradio_patch import Chatbot as grChatbot
-from fastchat.serve.gradio_css import code_highlight_css
 
 
 logger = build_logger("gradio_web_server", "gradio_web_server.log")
 
 headers = {"User-Agent": "fastchat Client"}
 
 no_change_btn = gr.Button.update()
 enable_btn = gr.Button.update(interactive=True)
 disable_btn = gr.Button.update(interactive=False)
 
 controller_url = None
 enable_moderation = False
 
-
-priority = {
-    "vicuna-13b": "aaa",
-    "koala-13b": "aab",
-    "fastchat-t5-3b": "aac",
-    "oasst-pythia-12b": "aad",
-    "chatglm-6b": "aae",
-    "stablelm-tuned-alpha-7b": "aaf",
-    "alpaca-13b": "aag",
-    "llama-13b": "aah",
-    "dolly-v2-12b": "aai",
-}
-
-model_description_md = """
-| | |
-| ---- | ---- |
-| [Vicuna](https://vicuna.lmsys.org): a chat assistant fine-tuned from LLaMA on user-shared conversations by LMSYS. | [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/): a dialogue model for academic research by BAIR |
-| [FastChat-T5](https://huggingface.co/lmsys/fastchat-t5-3b-v1.0): a chat assistant fine-tuned from FLAN-T5 by LMSYS. | [OpenAssistant (oasst)](https://open-assistant.io/): a chat-based assistant for everyone by LAION. |
-| [ChatGLM](https://chatglm.cn/blog): an open bilingual dialogue language model by Tsinghua University | [StableLM](https://github.com/stability-AI/stableLM/): Stability AI language models. |
-| [Alpaca](https://crfm.stanford.edu/2023/03/13/alpaca.html): a model fine-tuned from LLaMA on instruction-following demonstrations by Stanford. | [LLaMA](https://arxiv.org/abs/2302.13971): open and efficient foundation language models by Meta. |
-| [Dolly](https://www.databricks.com/blog/2023/04/12/dolly-first-open-commercially-viable-instruction-tuned-llm): an instruction-tuned open large language model by Databricks. | |
-"""
-
 learn_more_md = """
 ### License
 The service is a research preview intended for non-commercial use only, subject to the model [License](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) of LLaMA, [Terms of Use](https://openai.com/policies/terms-of-use) of the data generated by OpenAI, and [Privacy Practices](https://chrome.google.com/webstore/detail/sharegpt-share-your-chatg/daiacboceoaocpibfodeljbdfacokfjb) of ShareGPT. Please contact us if you find any potential violation.
 """
 
 
 def set_global_vars(controller_url_, enable_moderation_):
@@ -77,29 +58,20 @@
 
 
 def get_model_list(controller_url):
     ret = requests.post(controller_url + "/refresh_all_workers")
     assert ret.status_code == 200
     ret = requests.post(controller_url + "/list_models")
     models = ret.json()["models"]
+    priority = {k: f"___{i:02d}" for i, k in enumerate(model_info)}
     models.sort(key=lambda x: priority.get(x, x))
     logger.info(f"Models: {models}")
     return models
 
 
-get_window_url_params = """
-function() {
-    const params = new URLSearchParams(window.location.search);
-    url_params = Object.fromEntries(params);
-    console.log("url_params", url_params);
-    return url_params;
-    }
-"""
-
-
 def load_demo_single(models, url_params):
     dropdown_update = gr.Dropdown.update(visible=True)
     if "model" in url_params:
         model = url_params["model"]
         if model in models:
             dropdown_update = gr.Dropdown.update(value=model, visible=True)
 
@@ -163,15 +135,15 @@
     return (state, [], "") + (disable_btn,) * 5
 
 
 def add_text(state, text, request: gr.Request):
     logger.info(f"add_text. ip: {request.client.host}. len: {len(text)}")
 
     if state is None:
-        state = get_default_conv_template("vicuna").copy()
+        state = get_conversation_template("vicuna")
 
     if len(text) <= 0:
         state.skip_next = True
         return (state, state.to_gradio_chatbot(), "") + (no_change_btn,) * 5
     if enable_moderation:
         flagged = violates_moderation(text)
         if flagged:
@@ -195,131 +167,224 @@
         if len(blocks) % 2 == 1:
             for i in range(1, len(blocks), 2):
                 blocks[i] = blocks[i].replace("\\_", "_")
         code = sep.join(blocks)
     return code
 
 
-def http_bot(state, model_selector, temperature, max_new_tokens, request: gr.Request):
+def openai_api_stream_iter(model_name, messages, temperature, top_p, max_new_tokens):
+    import openai
+
+    # Make requests
+    gen_params = {
+        "model": model_name,
+        "prompt": messages,
+        "temperature": temperature,
+        "top_p": top_p,
+    }
+    logger.info(f"==== request ====\n{gen_params}")
+
+    res = openai.ChatCompletion.create(
+        model=model_name, messages=messages, temperature=temperature, stream=True
+    )
+    text = ""
+    for chunk in res:
+        text += chunk["choices"][0]["delta"].get("content", "")
+        data = {
+            "text": text,
+            "error_code": 0,
+        }
+        yield data
+
+
+def anthropic_api_stream_iter(model_name, prompt, temperature, top_p, max_new_tokens):
+    import anthropic
+
+    c = anthropic.Client(os.environ["ANTHROPIC_API_KEY"])
+
+    # Make requests
+    gen_params = {
+        "model": model_name,
+        "prompt": prompt,
+        "temperature": temperature,
+        "top_p": top_p,
+    }
+    logger.info(f"==== request ====\n{gen_params}")
+
+    res = c.completion_stream(
+        prompt=prompt,
+        stop_sequences=[anthropic.HUMAN_PROMPT],
+        max_tokens_to_sample=max_new_tokens,
+        temperature=temperature,
+        top_p=top_p,
+        model=model_name,
+        stream=True,
+    )
+    for chunk in res:
+        data = {
+            "text": chunk["completion"],
+            "error_code": 0,
+        }
+        yield data
+
+
+def model_worker_stream_iter(
+    conv, model_name, worker_addr, prompt, temperature, top_p, max_new_tokens
+):
+    # Make requests
+    gen_params = {
+        "model": model_name,
+        "prompt": prompt,
+        "temperature": temperature,
+        "top_p": top_p,
+        "max_new_tokens": max_new_tokens,
+        "stop": conv.stop_str,
+        "stop_token_ids": conv.stop_token_ids,
+        "echo": False,
+    }
+    logger.info(f"==== request ====\n{gen_params}")
+
+    # Stream output
+    response = requests.post(
+        worker_addr + "/worker_generate_stream",
+        headers=headers,
+        json=gen_params,
+        stream=True,
+        timeout=20,
+    )
+    for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
+        if chunk:
+            data = json.loads(chunk.decode())
+            yield data
+
+
+def http_bot(
+    state, model_selector, temperature, top_p, max_new_tokens, request: gr.Request
+):
     logger.info(f"http_bot. ip: {request.client.host}")
     start_tstamp = time.time()
     model_name = model_selector
     temperature = float(temperature)
+    top_p = float(top_p)
     max_new_tokens = int(max_new_tokens)
 
     if state.skip_next:
         # This generate call is skipped due to invalid inputs
         yield (state, state.to_gradio_chatbot()) + (no_change_btn,) * 5
         return
 
     if len(state.messages) == state.offset + 2:
         # First round of conversation
-        new_state = get_default_conv_template(model_name).copy()
+        new_state = get_conversation_template(model_name)
         new_state.conv_id = uuid.uuid4().hex
         new_state.model_name = state.model_name or model_selector
         new_state.append_message(new_state.roles[0], state.messages[-2][1])
         new_state.append_message(new_state.roles[1], None)
         state = new_state
 
-    # Query worker address
-    ret = requests.post(
-        controller_url + "/get_worker_address", json={"model": model_name}
-    )
-    worker_addr = ret.json()["address"]
-    logger.info(f"model_name: {model_name}, worker_addr: {worker_addr}")
-
-    # No available worker
-    if worker_addr == "":
-        state.messages[-1][-1] = server_error_msg
-        yield (
-            state,
-            state.to_gradio_chatbot(),
-            disable_btn,
-            disable_btn,
-            disable_btn,
-            enable_btn,
-            enable_btn,
+    if model_name == "gpt-3.5-turbo" or model_name == "gpt-4":
+        prompt = state.to_openai_api_messages()
+        stream_iter = openai_api_stream_iter(
+            model_name, prompt, temperature, top_p, max_new_tokens
+        )
+    elif model_name == "claude-v1":
+        prompt = state.get_prompt()
+        stream_iter = anthropic_api_stream_iter(
+            model_name, prompt, temperature, top_p, max_new_tokens
         )
-        return
-
-    # Construct prompt
-    conv = state
-    if "chatglm" in model_name:
-        prompt = conv.messages[conv.offset :]
     else:
-        prompt = conv.get_prompt()
+        # Query worker address
+        ret = requests.post(
+            controller_url + "/get_worker_address", json={"model": model_name}
+        )
+        worker_addr = ret.json()["address"]
+        logger.info(f"model_name: {model_name}, worker_addr: {worker_addr}")
 
-    # Make requests
-    gen_params = {
-        "model": model_name,
-        "prompt": prompt,
-        "temperature": temperature,
-        "max_new_tokens": max_new_tokens,
-        "stop": conv.stop_str,
-        "stop_token_ids": conv.stop_token_ids,
-        "echo": False,
-    }
-    logger.info(f"==== request ====\n{gen_params}")
+        # No available worker
+        if worker_addr == "":
+            state.messages[-1][-1] = server_error_msg
+            yield (
+                state,
+                state.to_gradio_chatbot(),
+                disable_btn,
+                disable_btn,
+                disable_btn,
+                enable_btn,
+                enable_btn,
+            )
+            return
+
+        # Construct prompt
+        conv = state
+        if "chatglm" in model_name:
+            prompt = list(list(x) for x in conv.messages[conv.offset :])
+        else:
+            prompt = conv.get_prompt()
+        stream_iter = model_worker_stream_iter(
+            conv, model_name, worker_addr, prompt, temperature, top_p, max_new_tokens
+        )
 
     state.messages[-1][-1] = "▌"
     yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
 
     try:
-        # Stream output
-        response = requests.post(
-            worker_addr + "/worker_generate_stream",
-            headers=headers,
-            json=gen_params,
-            stream=True,
-            timeout=20,
-        )
-        for chunk in response.iter_lines(decode_unicode=False, delimiter=b"\0"):
-            if chunk:
-                data = json.loads(chunk.decode())
-                if data["error_code"] == 0:
-                    output = data["text"].strip()
+        for data in stream_iter:
+            if data["error_code"] == 0:
+                output = data["text"].strip()
+                if "vicuna" in model_name:
                     output = post_process_code(output)
-                    state.messages[-1][-1] = output + "▌"
-                    yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
-                else:
-                    output = data["text"] + f" (error_code: {data['error_code']})"
-                    state.messages[-1][-1] = output
-                    yield (state, state.to_gradio_chatbot()) + (
-                        disable_btn,
-                        disable_btn,
-                        disable_btn,
-                        enable_btn,
-                        enable_btn,
-                    )
-                    return
-                time.sleep(0.02)
+                state.messages[-1][-1] = output + "▌"
+                yield (state, state.to_gradio_chatbot()) + (disable_btn,) * 5
+            else:
+                output = data["text"] + f" (error_code: {data['error_code']})"
+                state.messages[-1][-1] = output
+                yield (state, state.to_gradio_chatbot()) + (
+                    disable_btn,
+                    disable_btn,
+                    disable_btn,
+                    enable_btn,
+                    enable_btn,
+                )
+                return
+            time.sleep(0.02)
     except requests.exceptions.RequestException as e:
         state.messages[-1][-1] = server_error_msg + f" (error_code: 4)"
         yield (state, state.to_gradio_chatbot()) + (
             disable_btn,
             disable_btn,
             disable_btn,
             enable_btn,
             enable_btn,
         )
         return
+    except Exception as e:
+        state.messages[-1][-1] = server_error_msg + f" (error_code: 5, {e})"
+        yield (state, state.to_gradio_chatbot()) + (
+            disable_btn,
+            disable_btn,
+            disable_btn,
+            enable_btn,
+            enable_btn,
+        )
+        return
 
     state.messages[-1][-1] = state.messages[-1][-1][:-1]
     yield (state, state.to_gradio_chatbot()) + (enable_btn,) * 5
 
     finish_tstamp = time.time()
     logger.info(f"{output}")
 
     with open(get_conv_log_filename(), "a") as fout:
         data = {
             "tstamp": round(finish_tstamp, 4),
             "type": "chat",
             "model": model_name,
             "gen_params": {
                 "temperature": temperature,
+                "top_p": top_p,
                 "max_new_tokens": max_new_tokens,
             },
             "start": round(start_tstamp, 4),
             "finish": round(start_tstamp, 4),
             "state": state.dict(),
             "ip": request.client.host,
         }
@@ -340,65 +405,90 @@
     display: none;
 }
 """
 )
 
 
 def build_single_model_ui(models):
-    notice_markdown = ("""
+    notice_markdown = """
 # 🏔️ Chat with Open Large Language Models
-- Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://vicuna.lmsys.org) [[Evaluation]](https://vicuna.lmsys.org/eval/)
+- Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality. [[Blog post]](https://lmsys.org/blog/2023-03-30-vicuna/)
 - Koala: A Dialogue Model for Academic Research. [[Blog post]](https://bair.berkeley.edu/blog/2023/04/03/koala/)
 - [[GitHub]](https://github.com/lm-sys/FastChat) [[Twitter]](https://twitter.com/lmsysorg) [[Discord]](https://discord.gg/h6kCZb72G7)
 
 ### Terms of use
-By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data for future research.**
+By using this service, users are required to agree to the following terms: The service is a research preview intended for non-commercial use only. It only provides limited safety measures and may generate offensive content. It must not be used for any illegal, harmful, violent, racist, or sexual purposes. **The service collects user dialogue data and reserves the right to distribute it under a Creative Commons Attribution (CC-BY) license.**
 
 ### Choose a model to chat with
-""" + model_description_md)
+"""
+
+    model_description_md = """
+| | | |
+| ---- | ---- | ---- |
+"""
+    for i, name in enumerate(models):
+        if i % 3 == 0:
+            model_description_md += "|"
+
+        if name in model_info:
+            minfo = model_info[name]
+            model_description_md += f" [{name}]({minfo.link}): {minfo.description} |"
+        else:
+            model_description_md += f" {name} |"
+        if i % 3 == 2:
+            model_description_md += "\n"
 
     state = gr.State()
-    notice = gr.Markdown(notice_markdown, elem_id="notice_markdown")
+    gr.Markdown(notice_markdown + model_description_md, elem_id="notice_markdown")
 
     with gr.Row(elem_id="model_selector_row"):
         model_selector = gr.Dropdown(
             choices=models,
             value=models[0] if len(models) > 0 else "",
             interactive=True,
             show_label=False,
         ).style(container=False)
 
-    chatbot = grChatbot(elem_id="chatbot", visible=False).style(height=550)
+    chatbot = grChatbot(
+        elem_id="chatbot", label="Scroll down and start chatting", visible=False
+    ).style(height=550)
     with gr.Row():
         with gr.Column(scale=20):
             textbox = gr.Textbox(
                 show_label=False,
                 placeholder="Enter text and press ENTER",
                 visible=False,
             ).style(container=False)
         with gr.Column(scale=1, min_width=50):
             send_btn = gr.Button(value="Send", visible=False)
 
     with gr.Row(visible=False) as button_row:
         upvote_btn = gr.Button(value="👍  Upvote", interactive=False)
         downvote_btn = gr.Button(value="👎  Downvote", interactive=False)
         flag_btn = gr.Button(value="⚠️  Flag", interactive=False)
-        # stop_btn = gr.Button(value="⏹️  Stop Generation", interactive=False)
         regenerate_btn = gr.Button(value="🔄  Regenerate", interactive=False)
         clear_btn = gr.Button(value="🗑️  Clear history", interactive=False)
 
     with gr.Accordion("Parameters", open=False, visible=False) as parameter_row:
         temperature = gr.Slider(
             minimum=0.0,
             maximum=1.0,
             value=0.7,
             step=0.1,
             interactive=True,
             label="Temperature",
         )
+        top_p = gr.Slider(
+            minimum=0.0,
+            maximum=1.0,
+            value=1.0,
+            step=0.1,
+            interactive=True,
+            label="Top P",
+        )
         max_output_tokens = gr.Slider(
             minimum=0,
             maximum=1024,
             value=512,
             step=64,
             interactive=True,
             label="Max output tokens",
@@ -421,33 +511,33 @@
     flag_btn.click(
         flag_last_response,
         [state, model_selector],
         [textbox, upvote_btn, downvote_btn, flag_btn],
     )
     regenerate_btn.click(regenerate, state, [state, chatbot, textbox] + btn_list).then(
         http_bot,
-        [state, model_selector, temperature, max_output_tokens],
+        [state, model_selector, temperature, top_p, max_output_tokens],
         [state, chatbot] + btn_list,
     )
     clear_btn.click(clear_history, None, [state, chatbot, textbox] + btn_list)
 
     model_selector.change(clear_history, None, [state, chatbot, textbox] + btn_list)
 
     textbox.submit(
         add_text, [state, textbox], [state, chatbot, textbox] + btn_list
     ).then(
         http_bot,
-        [state, model_selector, temperature, max_output_tokens],
+        [state, model_selector, temperature, top_p, max_output_tokens],
         [state, chatbot] + btn_list,
     )
     send_btn.click(
         add_text, [state, textbox], [state, chatbot, textbox] + btn_list
     ).then(
         http_bot,
-        [state, model_selector, temperature, max_output_tokens],
+        [state, model_selector, temperature, top_p, max_output_tokens],
         [state, chatbot] + btn_list,
     )
 
     return state, model_selector, chatbot, textbox, send_btn, button_row, parameter_row
 
 
 def build_demo(models):
@@ -477,15 +567,15 @@
                     model_selector,
                     chatbot,
                     textbox,
                     send_btn,
                     button_row,
                     parameter_row,
                 ],
-                _js=get_window_url_params,
+                _js=get_window_url_params_js,
             )
         else:
             raise ValueError(f"Unknown model list mode: {args.model_list_mode}")
 
     return demo
 
 
@@ -498,20 +588,35 @@
     parser.add_argument(
         "--model-list-mode", type=str, default="once", choices=["once", "reload"]
     )
     parser.add_argument("--share", action="store_true")
     parser.add_argument(
         "--moderate", action="store_true", help="Enable content moderation"
     )
+    parser.add_argument(
+        "--add-chatgpt",
+        action="store_true",
+        help="Add OpenAI's ChatGPT models (gpt-3.5-turbo, gpt-4)",
+    )
+    parser.add_argument(
+        "--add-claude",
+        action="store_true",
+        help="Add Anthropic's Claude models (claude-v1)",
+    )
+
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     set_global_vars(args.controller_url, args.moderate)
     models = get_model_list(args.controller_url)
 
-    logger.info(args)
+    if args.add_chatgpt:
+        models = ["gpt-3.5-turbo", "gpt-4"] + models
+    if args.add_claude:
+        models = ["claude-v1"] + models
+
     demo = build_demo(models)
     demo.queue(
         concurrency_count=args.concurrency_count, status_update_rate=10, api_open=False
     ).launch(
         server_name=args.host, server_port=args.port, share=args.share, max_threads=200
     )
```

### Comparing `fschat-0.2.5/fastchat/serve/gradio_web_server_multi.py` & `fschat-0.2.6/fastchat/serve/gradio_web_server_multi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,70 @@
+"""
+The gradio demo server with multiple tabs.
+It supports chatting with a single model or chatting with two models side-by-side.
+"""
+
 import argparse
+import pickle
 
 import gradio as gr
 
-from fastchat.utils import build_logger
+from fastchat.serve.gradio_block_arena_anony import (
+    build_side_by_side_ui_anony,
+    load_demo_side_by_side_anony,
+    set_global_vars_anony,
+)
+from fastchat.serve.gradio_block_arena_named import (
+    build_side_by_side_ui_named,
+    load_demo_side_by_side_named,
+    set_global_vars_named,
+)
 from fastchat.serve.gradio_patch import Chatbot as grChatbot
 from fastchat.serve.gradio_web_server import (
     set_global_vars,
-    get_window_url_params,
     block_css,
     build_single_model_ui,
     get_model_list,
     load_demo_single,
 )
-from fastchat.serve.gradio_block_arena_anony import (build_side_by_side_ui_anony,
-    load_demo_side_by_side_anony, set_global_vars_anony)
-from fastchat.serve.gradio_block_arena_named import (build_side_by_side_ui_named,
-    load_demo_side_by_side_named, set_global_vars_named)
+from fastchat.serve.monitor.monitor import build_leaderboard_tab
+from fastchat.utils import build_logger, get_window_url_params_js
 
 
 logger = build_logger("gradio_web_server_multi", "gradio_web_server_multi.log")
 
 
 def load_demo(url_params, request: gr.Request):
     logger.info(f"load_demo. ip: {request.client.host}. params: {url_params}")
     selected = 0
     if "arena" in url_params:
         selected = 1
     elif "compare" in url_params:
         selected = 2
+    elif "leaderboard" in url_params:
+        selected = 3
     single_updates = load_demo_single(models, url_params)
-    side_by_side_anony_updates = load_demo_side_by_side_anony(models, url_params)
+
+    models_anony = models
+    if args.add_chatgpt:
+        models_anony = ["gpt-4", "gpt-3.5-turbo"] + models_anony
+    if args.add_claude:
+        models_anony = ["claude-v1"] + models_anony
+
+    side_by_side_anony_updates = load_demo_side_by_side_anony(models_anony, url_params)
     side_by_side_named_updates = load_demo_side_by_side_named(models, url_params)
-    return ((gr.Tabs.update(selected=selected),) + single_updates +
-            side_by_side_anony_updates + side_by_side_named_updates)
+    return (
+        (gr.Tabs.update(selected=selected),)
+        + single_updates
+        + side_by_side_anony_updates
+        + side_by_side_named_updates
+    )
 
 
-def build_demo(models):
+def build_demo(models, elo_results_file):
     with gr.Blocks(
         title="Chat with Open Large Language Models",
         theme=gr.themes.Base(),
         css=block_css,
     ) as demo:
         with gr.Tabs() as tabs:
             with gr.Tab("Single Model", id=0):
@@ -106,22 +131,26 @@
                         c_send_btn,
                         c_button_row,
                         c_button_row2,
                         c_parameter_row,
                     ]
                 )
 
+            if elo_results_file:
+                with gr.Tab("Leaderboard", id=3):
+                    build_leaderboard_tab(elo_results_file)
+
         url_params = gr.JSON(visible=False)
 
         if args.model_list_mode == "once":
             demo.load(
                 load_demo,
                 [url_params],
                 [tabs] + a_list + b_list + c_list,
-                _js=get_window_url_params,
+                _js=get_window_url_params_js,
             )
         else:
             raise ValueError(f"Unknown model list mode: {args.model_list_mode}")
 
     return demo
 
 
@@ -134,22 +163,32 @@
     parser.add_argument(
         "--model-list-mode", type=str, default="once", choices=["once", "reload"]
     )
     parser.add_argument("--share", action="store_true")
     parser.add_argument(
         "--moderate", action="store_true", help="Enable content moderation"
     )
+    parser.add_argument(
+        "--add-chatgpt",
+        action="store_true",
+        help="Add OpenAI ChatGPT models (gpt-3.5-turbo, gpt-4)",
+    )
+    parser.add_argument(
+        "--add-claude",
+        action="store_true",
+        help="Add Anthropic's Claude models (claude-v1)",
+    )
+    parser.add_argument("--elo-results-file", type=str)
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     set_global_vars(args.controller_url, args.moderate)
     set_global_vars_named(args.moderate)
     set_global_vars_anony(args.moderate)
     models = get_model_list(args.controller_url)
 
-    logger.info(args)
-    demo = build_demo(models)
+    demo = build_demo(models, args.elo_results_file)
     demo.queue(
         concurrency_count=args.concurrency_count, status_update_rate=10, api_open=False
     ).launch(
         server_name=args.host, server_port=args.port, share=args.share, max_threads=200
     )
```

### Comparing `fschat-0.2.5/fastchat/serve/huggingface_api.py` & `fschat-0.2.6/fastchat/serve/huggingface_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Usage:
+python3 -m fastchat.serve.huggingface_api --model lmsys/fastchat-t5-3b-v1.0
 python3 -m fastchat.serve.huggingface_api --model ~/model_weights/vicuna-7b/
 """
 import argparse
 import json
 
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 
-from fastchat.conversation import get_default_conv_template
-from fastchat.serve.inference import load_model, add_model_args
+from fastchat import load_model, get_conversation_template, add_model_args
 
 
 @torch.inference_mode()
 def main(args):
     model, tokenizer = load_model(
         args.model_path,
         args.device,
@@ -22,43 +22,41 @@
         args.load_8bit,
         args.cpu_offloading,
         debug=args.debug,
     )
 
     msg = args.message
 
-    conv = get_default_conv_template(args.model_path).copy()
+    conv = get_conversation_template(args.model_path)
     conv.append_message(conv.roles[0], msg)
     conv.append_message(conv.roles[1], None)
     prompt = conv.get_prompt()
 
     input_ids = tokenizer([prompt]).input_ids
     output_ids = model.generate(
         torch.as_tensor(input_ids).cuda(),
         do_sample=True,
-        temperature=0.7,
-        max_new_tokens=1024,
+        temperature=args.temperature,
+        max_new_tokens=args.max_new_tokens,
     )
     if model.config.is_encoder_decoder:
         output_ids = output_ids[0]
     else:
-        output_ids = output_ids[0][len(input_ids[0]):]
-    outputs = tokenizer.decode(output_ids, skip_special_tokens=True,
-                               spaces_between_special_tokens=False)
+        output_ids = output_ids[0][len(input_ids[0]) :]
+    outputs = tokenizer.decode(
+        output_ids, skip_special_tokens=True, spaces_between_special_tokens=False
+    )
 
     print(f"{conv.roles[0]}: {msg}")
     print(f"{conv.roles[1]}: {outputs}")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     add_model_args(parser)
-    parser.add_argument(
-        "--conv-template", type=str, default=None, help="Conversation prompt template."
-    )
     parser.add_argument("--temperature", type=float, default=0.7)
     parser.add_argument("--max-new-tokens", type=int, default=512)
     parser.add_argument("--debug", action="store_true")
     parser.add_argument("--message", type=str, default="Hello! Who are you?")
     args = parser.parse_args()
 
     main(args)
```

### Comparing `fschat-0.2.5/fastchat/serve/model_worker.py` & `fschat-0.2.6/fastchat/serve/model_worker.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import time
 from typing import List, Union
 import threading
 import uuid
 
 from fastapi import FastAPI, Request, BackgroundTasks
-from fastapi.responses import StreamingResponse
+from fastapi.responses import StreamingResponse, JSONResponse
 import requests
 
 try:
     from transformers import (
         AutoTokenizer,
         AutoModelForCausalLM,
         LlamaTokenizer,
@@ -30,16 +30,17 @@
         LLaMATokenizer,
         AutoModel,
     )
 import torch
 import uvicorn
 
 from fastchat.constants import WORKER_HEART_BEAT_INTERVAL
-from fastchat.serve.inference import load_model, generate_stream, add_model_args
-from fastchat.serve.serve_chatglm import chatglm_generate_stream
+from fastchat.model.model_adapter import load_model, add_model_args
+from fastchat.model.chatglm_model import chatglm_generate_stream
+from fastchat.serve.inference import generate_stream
 from fastchat.utils import build_logger, server_error_msg, pretty_print_semaphore
 
 GB = 1 << 30
 
 worker_id = str(uuid.uuid4())[:6]
 logger = build_logger("model_worker", f"model_worker_{worker_id}.log")
 global_counter = 0
@@ -180,37 +181,129 @@
         except torch.cuda.OutOfMemoryError:
             ret = {
                 "text": server_error_msg,
                 "error_code": 1,
             }
             yield json.dumps(ret).encode() + b"\0"
 
+    def generate_completion(self, params):
+        try:
+            input_ids = self.tokenizer([params["prompt"]]).input_ids
+            output_ids = self.model.generate(
+                torch.as_tensor(input_ids).cuda(),
+                do_sample=True,
+                temperature=params["temperature"],
+                max_new_tokens=params["max_tokens"]
+                - 1,  # generate max_new_tokens + 1 tokens
+            )
+            if self.model.config.is_encoder_decoder:
+                output_ids = output_ids[0]
+            else:
+                output_ids = output_ids[0][len(input_ids[0]) :]
+            outputs = self.tokenizer.decode(
+                output_ids,
+                skip_special_tokens=True,
+                spaces_between_special_tokens=False,
+            )
+            completion_tokens = len(self.tokenizer(outputs).input_ids)
+            if completion_tokens >= params["max_tokens"]:
+                finish_reason = "length"
+            else:
+                finish_reason = "stop"
+            return json.dumps(
+                {
+                    "text": outputs,
+                    "finish_reason": finish_reason,
+                    "completion_tokens": completion_tokens,
+                    "prompt_tokens": len(input_ids[0]),
+                }
+            )
+
+        except torch.cuda.OutOfMemoryError:
+            ret = {
+                "text": server_error_msg,
+                "error_code": 1,
+            }
+            return json.dumps(ret).encode() + b"\0"
+
+    def get_embeddings(self, params):
+        try:
+            tokenizer = self.tokenizer
+            input_ids = tokenizer.encode(params["input"], return_tensors="pt").to(
+                self.device
+            )
+            model_output = self.model(input_ids, output_hidden_states=True)
+            is_chatglm = "chatglm" in str(type(self.model)).lower()
+            if is_chatglm:
+                data = (model_output.hidden_states[-1].transpose(0, 1))[0]
+            else:
+                data = model_output.hidden_states[-1][0]
+            embedding = torch.mean(data, dim=0)
+            return json.dumps(
+                {
+                    "embedding": embedding.tolist(),
+                    "token_num": len(self.tokenizer(params["input"]).input_ids),
+                }
+            )
+        except torch.cuda.OutOfMemoryError:
+            ret = {
+                "text": server_error_msg,
+                "error_code": 1,
+            }
+            return json.dumps(ret).encode() + b"\0"
+
 
 app = FastAPI()
 
 
 def release_model_semaphore():
     model_semaphore.release()
 
 
-@app.post("/worker_generate_stream")
-async def api_generate_stream(request: Request):
+def acquire_model_semaphore():
     global model_semaphore, global_counter
     global_counter += 1
-    params = await request.json()
-
     if model_semaphore is None:
         model_semaphore = asyncio.Semaphore(args.limit_model_concurrency)
-    await model_semaphore.acquire()
-    generator = worker.generate_stream_gate(params)
+    return model_semaphore.acquire()
+
+
+def create_background_tasks():
     background_tasks = BackgroundTasks()
     background_tasks.add_task(release_model_semaphore)
+    return background_tasks
+
+
+@app.post("/worker_generate_stream")
+async def api_generate_stream(request: Request):
+    params = await request.json()
+    await acquire_model_semaphore()
+    generator = worker.generate_stream_gate(params)
+    background_tasks = create_background_tasks()
     return StreamingResponse(generator, background=background_tasks)
 
 
+@app.post("/worker_generate_completion")
+async def api_generate_completion(request: Request):
+    params = await request.json()
+    await acquire_model_semaphore()
+    completion = worker.generate_completion(params)
+    background_tasks = create_background_tasks()
+    return JSONResponse(content=completion, background=background_tasks)
+
+
+@app.post("/worker_get_embeddings")
+async def api_get_embeddings(request: Request):
+    params = await request.json()
+    await acquire_model_semaphore()
+    embedding = worker.get_embeddings(params)
+    background_tasks = create_background_tasks()
+    return JSONResponse(content=embedding, background=background_tasks)
+
+
 @app.post("/worker_get_status")
 async def api_get_status(request: Request):
     return worker.get_status()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
@@ -226,17 +319,19 @@
     parser.add_argument("--stream-interval", type=int, default=2)
     parser.add_argument("--no-register", action="store_true")
     args = parser.parse_args()
     logger.info(f"args: {args}")
 
     if args.gpus:
         if len(args.gpus.split(",")) < args.num_gpus:
-            raise ValueError(f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!")
+            raise ValueError(
+                f"Larger --num-gpus ({args.num_gpus}) than --gpus {args.gpus}!"
+            )
         os.environ["CUDA_VISIBLE_DEVICES"] = args.gpus
-    
+
     worker = ModelWorker(
         args.controller_address,
         args.worker_address,
         worker_id,
         args.no_register,
         args.model_path,
         args.model_name,
```

### Comparing `fschat-0.2.5/fastchat/serve/monkey_patch_non_inplace.py` & `fschat-0.2.6/fastchat/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/serve/register_worker.py` & `fschat-0.2.6/fastchat/serve/register_worker.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/serve/serve_chatglm.py` & `fschat-0.2.6/fastchat/model/chatglm_model.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/serve/test_message.py` & `fschat-0.2.6/fastchat/serve/test_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import argparse
 import json
 
 import requests
 
-from fastchat.conversation import (
-    get_default_conv_template,
-    SeparatorStyle,
-)
+from fastchat.model.model_adapter import get_conversation_template
 
 
 def main():
     model_name = args.model_name
 
     if args.worker_address:
         worker_addr = args.worker_address
@@ -28,15 +25,15 @@
         worker_addr = ret.json()["address"]
         print(f"worker_addr: {worker_addr}")
 
     if worker_addr == "":
         print(f"No available workers for {model_name}")
         return
 
-    conv = get_default_conv_template(model_name).copy()
+    conv = get_conversation_template(model_name)
     conv.append_message(conv.roles[0], args.message)
     conv.append_message(conv.roles[1], None)
     prompt = conv.get_prompt()
 
     headers = {"User-Agent": "FastChat Client"}
     gen_params = {
         "model": model_name,
```

### Comparing `fschat-0.2.5/fastchat/serve/test_throughput.py` & `fschat-0.2.6/fastchat/serve/test_throughput.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/train/llama_flash_attn_monkey_patch.py` & `fschat-0.2.6/fastchat/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/train/train.py` & `fschat-0.2.6/fastchat/train/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 import numpy as np
 import torch
 from torch.utils.data import Dataset
 import transformers
 from transformers import Trainer
 from transformers.trainer_pt_utils import LabelSmoother
 
-from fastchat.conversation import get_default_conv_template, SeparatorStyle
+from fastchat.conversation import SeparatorStyle
+from fastchat.model.model_adapter import get_conversation_template
 
 IGNORE_TOKEN_ID = LabelSmoother.ignore_index
 
 
 @dataclass
 class ModelArguments:
     model_name_or_path: Optional[str] = field(default="facebook/opt-125m")
@@ -73,15 +74,15 @@
         trainer._save(output_dir, state_dict=cpu_state_dict)  # noqa
 
 
 def preprocess(
     sources,
     tokenizer: transformers.PreTrainedTokenizer,
 ) -> Dict:
-    conv = get_default_conv_template("vicuna").copy()
+    conv = get_conversation_template("vicuna")
     roles = {"human": conv.roles[0], "gpt": conv.roles[1]}
 
     # Apply prompt templates
     conversations = []
     for i, source in enumerate(sources):
         if roles[source[0]["from"]] != conv.roles[0]:
             # Skip the first one if it is not from human
```

### Comparing `fschat-0.2.5/fastchat/train/train_flant5.py` & `fschat-0.2.6/fastchat/train/train_flant5.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 import torch
 
 import transformers
 from torch.utils.data import Dataset
 from transformers import Trainer, AddedToken
 
-from fastchat.conversation import conv_one_shot as default_conversation
+from fastchat.model.model_adapter import get_conversation_template
+
+default_conversation = get_conversation_template("t5")
 
 # TODO: import and use code from ../data/dataset.py
 
 IGNORE_INDEX = -100
 DEFAULT_PAD_TOKEN = "[PAD]"
 DEFAULT_EOS_TOKEN = "</s>"
 DEFAULT_BOS_TOKEN = "</s>"
@@ -43,44 +45,41 @@
 @dataclass
 class ModelArguments:
     model_name_or_path: Optional[str] = field(default="facebook/opt-125m")
 
 
 @dataclass
 class DataArguments:
-    data_path: str = field(default=None,
-                           metadata={"help": "Path to the training data."})
+    data_path: str = field(
+        default=None, metadata={"help": "Path to the training data."}
+    )
     lazy_preprocess: bool = False
     num_data: int = -1
-    preprocessed_path: str = field(default=None,
-                                       metadata={"help": "Path to the preprocessed training data."})
+    preprocessed_path: str = field(
+        default=None, metadata={"help": "Path to the preprocessed training data."}
+    )
 
 
 @dataclass
 class TrainingArguments(transformers.TrainingArguments):
     cache_dir: Optional[str] = field(default=None)
     optim: str = field(default="adamw_torch")
     model_max_length: int = field(
         default=2048,
         metadata={
-            "help":
-            "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
+            "help": "Maximum sequence length. Sequences will be right padded (and possibly truncated)."
         },
     )
 
 
-def safe_save_model_for_hf_trainer(trainer: transformers.Trainer,
-                                   output_dir: str):
+def safe_save_model_for_hf_trainer(trainer: transformers.Trainer, output_dir: str):
     """Collects the state dict and dump to disk."""
     state_dict = trainer.model.state_dict()
     if trainer.args.should_save:
-        cpu_state_dict = {
-            key: value.cpu()
-            for key, value in state_dict.items()
-        }
+        cpu_state_dict = {key: value.cpu() for key, value in state_dict.items()}
         # potential bug for T5 model
         del state_dict
         trainer._save(output_dir, state_dict=cpu_state_dict)  # noqa
 
 
 def smart_tokenizer_and_embedding_resize(
     special_tokens_dict: Dict,
@@ -99,118 +98,127 @@
     model.resize_token_embeddings(len(tokenizer))
 
     if num_new_tokens > 0:
         input_embeddings = model.get_input_embeddings().weight.data
         output_embeddings = model.get_output_embeddings().weight.data
 
         input_embeddings_avg = input_embeddings[:-num_new_tokens].mean(
-            dim=0, keepdim=True)
+            dim=0, keepdim=True
+        )
         output_embeddings_avg = output_embeddings[:-num_new_tokens].mean(
-            dim=0, keepdim=True)
+            dim=0, keepdim=True
+        )
 
         input_embeddings[-num_new_tokens:] = input_embeddings_avg
         output_embeddings[-num_new_tokens:] = output_embeddings_avg
 
 
-def _tokenize_fn(strings: Sequence[str],
-                 tokenizer: transformers.PreTrainedTokenizer) -> Dict:
+def _tokenize_fn(
+    strings: Sequence[str], tokenizer: transformers.PreTrainedTokenizer
+) -> Dict:
     """Tokenize a list of strings."""
     tokenized_list = [
         tokenizer(
             text,
             return_tensors="pt",
             padding="longest",
             max_length=tokenizer.model_max_length,
             truncation=True,
-        ) for text in strings
-    ]
-    input_ids = labels = [
-        tokenized.input_ids[0] for tokenized in tokenized_list
+        )
+        for text in strings
     ]
+    input_ids = labels = [tokenized.input_ids[0] for tokenized in tokenized_list]
     input_ids_lens = labels_lens = [
         tokenized.input_ids.ne(tokenizer.pad_token_id).sum().item()
         for tokenized in tokenized_list
     ]
     return dict(
         input_ids=input_ids,
         labels=labels,
         input_ids_lens=input_ids_lens,
         labels_lens=labels_lens,
     )
 
 
-def _form_qa(q_list, a_list, tokenized_conversation, tokenized_lens, speakers, header_len, max_length, eos_id):
+def _form_qa(
+    q_list,
+    a_list,
+    tokenized_conversation,
+    tokenized_lens,
+    speakers,
+    header_len,
+    max_length,
+    eos_id,
+):
     cur_idx = header_len
     conv_len = len(tokenized_conversation)
 
     for tokenized_len, speaker in zip(tokenized_lens, speakers):
         if cur_idx >= conv_len:
             break
         if speaker == "gpt":
             # truncate answer if it is too long
             content_a = None
             if tokenized_len > max_length:
-                content_a = tokenized_conversation[cur_idx:cur_idx + max_length]
+                content_a = tokenized_conversation[cur_idx : cur_idx + max_length]
             else:
-                content_a = tokenized_conversation[cur_idx:cur_idx + tokenized_len]
+                content_a = tokenized_conversation[cur_idx : cur_idx + tokenized_len]
             content_a.append(eos_id)
             a_list.append(content_a)
             content_q = None
             if cur_idx >= max_length:
-                content_q = tokenized_conversation[cur_idx-max_length: cur_idx]
+                content_q = tokenized_conversation[cur_idx - max_length : cur_idx]
             else:
                 content_q = tokenized_conversation[:cur_idx]
             content_q.append(eos_id)
             q_list.append(content_q)
             # asser the last token is actually a EOS for an answer
             assert a_list[-1][-1] == eos_id, "Last Token is not EOS!"
         cur_idx += tokenized_len
 
+
 def _add_speaker_and_signal(header, source, get_conversation=True):
     """Add speaker and start/end signal on each round."""
     BEGIN_SIGNAL = "### "
     END_SIGNAL = "\n"
     conversation = header
-    
+
     unknown_role = "unknown"  # use default unknown role
     roles = {
         "human": default_conversation.roles[0],  # human role
         "gpt": default_conversation.roles[1],  # gpt role
     }
 
     for i in range(len(source)):
         sentence = source[i]
         sentence_from = sentence["from"].lower()
-  
+
         # TODO(Dacheng): verify this is a good way to split sentences
         if sentence_from == "human":
             # if this is not the last sentence
             if i != len(source) - 1:
-                next_sentence = source[i+1]
+                next_sentence = source[i + 1]
                 sentence["value"] = (
-                BEGIN_SIGNAL
-                + roles.get(sentence_from, unknown_role)
-                + ": "
-                + sentence["value"]
-                + END_SIGNAL
-                + BEGIN_SIGNAL
-                + roles.get(next_sentence["from"].lower(), unknown_role)
-                + ": "
-            )
+                    BEGIN_SIGNAL
+                    + roles.get(sentence_from, unknown_role)
+                    + ": "
+                    + sentence["value"]
+                    + END_SIGNAL
+                    + BEGIN_SIGNAL
+                    + roles.get(next_sentence["from"].lower(), unknown_role)
+                    + ": "
+                )
             else:
-            # if human is the last speaker, it does not contribute to an answer
+                # if human is the last speaker, it does not contribute to an answer
                 pass
         else:
-            sentence["value"] = (
-                sentence["value"]
-                + END_SIGNAL
-            )
+            sentence["value"] = sentence["value"] + END_SIGNAL
         if get_conversation:
             conversation += sentence["value"]
-       
+
     return conversation
 
 
 def preprocess(
     sources: Sequence[str],
     tokenizer: transformers.PreTrainedTokenizer,
 ) -> Dict:
@@ -231,31 +239,44 @@
     # Assume we get long conversations, don't pad, don't return tensor
     tokenized_conversations = tokenizer(conversations, max_length=None)["input_ids"]
     q_list = []
     a_list = []
     # count for EOS length
     header_len = _tokenize_fn([header], tokenizer)["input_ids_lens"][0] - 1
     from tqdm import tqdm
+
     for tokenized_conversation, source in tqdm(zip(tokenized_conversations, sources)):
         tokenized_sentence = _tokenize_fn([s["value"] for s in source], tokenizer)
         tokenized_lens = tokenized_sentence["input_ids_lens"]
-        tokenized_lens = [l-1 for l in tokenized_lens]
+        tokenized_lens = [l - 1 for l in tokenized_lens]
         speakers = [sentence["from"] for sentence in source]
         ids = tokenized_sentence["input_ids"]
-        _form_qa(q_list, a_list, tokenized_conversation, tokenized_lens, speakers, header_len, tokenizer.model_max_length, tokenizer.eos_token_id)
+        _form_qa(
+            q_list,
+            a_list,
+            tokenized_conversation,
+            tokenized_lens,
+            speakers,
+            header_len,
+            tokenizer.model_max_length,
+            tokenizer.eos_token_id,
+        )
     return dict(input_ids=q_list, labels=a_list)
 
 
 class SupervisedDataset(Dataset):
     """Dataset for supervised fine-tuning."""
 
-    def __init__(self, data_path: str,
-                 tokenizer: transformers.PreTrainedTokenizer,
-                 preprocessed_path,
-                 num_data):
+    def __init__(
+        self,
+        data_path: str,
+        tokenizer: transformers.PreTrainedTokenizer,
+        preprocessed_path,
+        num_data,
+    ):
         super(SupervisedDataset, self).__init__()
 
         # save to file
         self.preprocessed_path = preprocessed_path
         if not os.path.exists("./preprocessed_data/"):
             os.mkdir("preprocessed_data/")
         if os.path.exists(self.preprocessed_path):
@@ -263,51 +284,53 @@
             data_dict = json.load(open(self.preprocessed_path, "r"))
         else:
             logging.warning("Loading data...")
             list_data_dict = json.load(open(data_path, "r"))
 
             logging.warning("Formatting inputs...")
             sources = []
-          
+
             sources = [example["conversations"] for example in list_data_dict]
 
             data_dict = preprocess(sources, tokenizer)
             json_data_dict = json.dumps(data_dict)
 
-            # open file for writing, "w" 
-            f = open(self.preprocessed_path,"w")
+            # open file for writing, "w"
+            f = open(self.preprocessed_path, "w")
 
             # write json object to file
             f.write(json_data_dict)
-     
+
         if num_data != -1:
             data_dict["input_ids"] = data_dict["input_ids"][:num_data]
             data_dict["labels"] = data_dict["labels"][:num_data]
-       
+
         # Shuffle data to see more conversations, if only train on partial data
         temp = list(zip(data_dict["input_ids"], data_dict["labels"]))
         random.shuffle(temp)
         res1, res2 = zip(*temp)
         data_dict["input_ids"], data_dict["labels"] = list(res1), list(res2)
 
         # Dacheng: Get rid of short QA pair
         self.input_ids = copy.deepcopy(data_dict["input_ids"])
         self.labels = copy.deepcopy(data_dict["labels"])
         length_arr = defaultdict(int)
-        for idx, (input, label) in enumerate(zip(data_dict["input_ids"], data_dict["labels"])):
+        for idx, (input, label) in enumerate(
+            zip(data_dict["input_ids"], data_dict["labels"])
+        ):
             length_arr[str(len(label) // 100)] += 1
             if len(input) <= 5:
                 del_idx = self.input_ids.index(input)
                 self.input_ids.pop(del_idx)
                 self.labels.pop(del_idx)
             if len(label) <= 5:
                 del_idx = self.labels.index(label)
                 self.input_ids.pop(del_idx)
                 self.labels.pop(del_idx)
-        
+
         for input, label in zip(self.input_ids, self.labels):
             assert len(input) >= 5
             assert len(label) >= 5
 
     def __len__(self):
         return len(self.input_ids)
 
@@ -318,56 +341,64 @@
 @dataclass
 class DataCollatorForSupervisedDataset(object):
     """Collate examples for supervised fine-tuning."""
 
     tokenizer: transformers.PreTrainedTokenizer
 
     def __call__(self, instances: Sequence[Dict]) -> Dict[str, torch.Tensor]:
-        input_ids, labels = tuple([torch.as_tensor(instance[key], dtype=torch.int64) for instance in instances]
-                                  for key in ("input_ids", "labels"))
+        input_ids, labels = tuple(
+            [
+                torch.as_tensor(instance[key], dtype=torch.int64)
+                for instance in instances
+            ]
+            for key in ("input_ids", "labels")
+        )
         input_ids = torch.nn.utils.rnn.pad_sequence(
-            input_ids,
-            batch_first=True,
-            padding_value=self.tokenizer.pad_token_id)
-        labels = torch.nn.utils.rnn.pad_sequence(labels,
-                                                 batch_first=True,
-                                                 padding_value=IGNORE_INDEX)
+            input_ids, batch_first=True, padding_value=self.tokenizer.pad_token_id
+        )
+        labels = torch.nn.utils.rnn.pad_sequence(
+            labels, batch_first=True, padding_value=IGNORE_INDEX
+        )
         ret = dict(
             input_ids=input_ids,
             labels=labels,
             attention_mask=input_ids.ne(self.tokenizer.pad_token_id),
         )
         torch.set_printoptions(profile="full")
         return ret
 
 
-def make_supervised_data_module(tokenizer: transformers.PreTrainedTokenizer,
-                                data_args) -> Dict:
+def make_supervised_data_module(
+    tokenizer: transformers.PreTrainedTokenizer, data_args
+) -> Dict:
     """Make dataset and collator for supervised fine-tuning."""
     dataset_cls = SupervisedDataset
-    train_dataset = dataset_cls(tokenizer=tokenizer,
-                                data_path=data_args.data_path,
-                                preprocessed_path=data_args.preprocessed_path,
-                                num_data=data_args.num_data)
+    train_dataset = dataset_cls(
+        tokenizer=tokenizer,
+        data_path=data_args.data_path,
+        preprocessed_path=data_args.preprocessed_path,
+        num_data=data_args.num_data,
+    )
     data_collator = DataCollatorForSupervisedDataset(tokenizer=tokenizer)
-    return dict(train_dataset=train_dataset,
-                eval_dataset=None,
-                data_collator=data_collator)
+    return dict(
+        train_dataset=train_dataset, eval_dataset=None, data_collator=data_collator
+    )
 
 
 def train():
     parser = transformers.HfArgumentParser(
-        (ModelArguments, DataArguments, TrainingArguments))
+        (ModelArguments, DataArguments, TrainingArguments)
+    )
     model_args, data_args, training_args = parser.parse_args_into_dataclasses()
 
     model = transformers.AutoModelForSeq2SeqLM.from_pretrained(
-             model_args.model_name_or_path,
+        model_args.model_name_or_path,
         cache_dir=training_args.cache_dir,
     )
-    # Dacheng: Note we can only use T5Tokenizer, otherwise it will prepend 
+    # Dacheng: Note we can only use T5Tokenizer, otherwise it will prepend
     # a space before special tokens.
     tokenizer = transformers.T5Tokenizer.from_pretrained(
         model_args.model_name_or_path,
         cache_dir=training_args.cache_dir,
         model_max_length=training_args.model_max_length,
         padding_side="right",
         use_fast=False,
@@ -376,25 +407,22 @@
     smart_tokenizer_and_embedding_resize(
         special_tokens_dict=dict(pad_token=DEFAULT_PAD_TOKEN),
         other_tokens=["<", "{", "\n", "}", "`", " ", "\\", "^", "\t"],
         tokenizer=tokenizer,
         model=model,
     )
 
-    data_module = make_supervised_data_module(tokenizer=tokenizer,
-                                              data_args=data_args)
-    trainer = Trainer(model=model,
-                    tokenizer=tokenizer,
-                    args=training_args,
-                    **data_module)
+    data_module = make_supervised_data_module(tokenizer=tokenizer, data_args=data_args)
+    trainer = Trainer(
+        model=model, tokenizer=tokenizer, args=training_args, **data_module
+    )
 
     if list(pathlib.Path(training_args.output_dir).glob("checkpoint-*")):
         trainer.train(resume_from_checkpoint=True)
     else:
         trainer.train()
     trainer.save_state()
-    safe_save_model_for_hf_trainer(trainer=trainer,
-                                   output_dir=training_args.output_dir)
+    safe_save_model_for_hf_trainer(trainer=trainer, output_dir=training_args.output_dir)
 
 
 if __name__ == "__main__":
     train()
```

### Comparing `fschat-0.2.5/fastchat/train/train_lora.py` & `fschat-0.2.6/fastchat/train/train_lora.py`

 * *Files identical despite different names*

### Comparing `fschat-0.2.5/fastchat/utils.py` & `fschat-0.2.6/fastchat/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,16 +32,18 @@
     # Set the format of root handlers
     if not logging.getLogger().handlers:
         if sys.version_info[1] >= 9:
             # This is for windows
             logging.basicConfig(level=logging.INFO, encoding="utf-8")
         else:
             if platform.system() == "Windows":
-                warnings.warn("If you are running on Windows, "
-                              "we recommend you use Python >= 3.9 for UTF-8 encoding.")
+                warnings.warn(
+                    "If you are running on Windows, "
+                    "we recommend you use Python >= 3.9 for UTF-8 encoding."
+                )
             logging.basicConfig(level=logging.INFO)
     logging.getLogger().handlers[0].setFormatter(formatter)
 
     # Redirect stdout and stderr to loggers
     stdout_logger = logging.getLogger("stdout")
     stdout_logger.setLevel(logging.INFO)
     sl = StreamToLogger(stdout_logger, logging.INFO)
@@ -57,15 +59,15 @@
     logger.setLevel(logging.INFO)
 
     # Add a file handler for all loggers
     if handler is None:
         os.makedirs(LOGDIR, exist_ok=True)
         filename = os.path.join(LOGDIR, logger_filename)
         handler = logging.handlers.TimedRotatingFileHandler(
-            filename, when="D", utc=True
+            filename, when="D", utc=True, encoding="utf-8"
         )
         handler.setFormatter(formatter)
 
         for name, item in logging.root.manager.loggerDict.items():
             if isinstance(item, logging.Logger):
                 item.addHandler(handler)
 
@@ -114,14 +116,34 @@
     """
     import torch
 
     setattr(torch.nn.Linear, "reset_parameters", lambda self: None)
     setattr(torch.nn.LayerNorm, "reset_parameters", lambda self: None)
 
 
+def get_gpu_memory(max_gpus=None):
+    """Get available memory for each GPU."""
+    gpu_memory = []
+    num_gpus = (
+        torch.cuda.device_count()
+        if max_gpus is None
+        else min(max_gpus, torch.cuda.device_count())
+    )
+
+    for gpu_id in range(num_gpus):
+        with torch.cuda.device(gpu_id):
+            device = torch.cuda.current_device()
+            gpu_properties = torch.cuda.get_device_properties(device)
+            total_memory = gpu_properties.total_memory / (1024**3)
+            allocated_memory = torch.cuda.memory_allocated() / (1024**3)
+            available_memory = total_memory - allocated_memory
+            gpu_memory.append(available_memory)
+    return gpu_memory
+
+
 def violates_moderation(text):
     """
     Check whether the text violates OpenAI moderation API.
     """
     url = "https://api.openai.com/v1/moderations"
     headers = {
         "Content-Type": "application/json",
@@ -161,7 +183,17 @@
         torch.save(weight, os.path.join(ckpt_path, weight_file))
 
 
 def pretty_print_semaphore(semaphore):
     if semaphore is None:
         return "None"
     return f"Semaphore(value={semaphore._value}, locked={semaphore.locked()})"
+
+
+get_window_url_params_js = """
+function() {
+    const params = new URLSearchParams(window.location.search);
+    url_params = Object.fromEntries(params);
+    console.log("url_params", url_params);
+    return url_params;
+    }
+"""
```

### Comparing `fschat-0.2.5/fschat.egg-info/PKG-INFO` & `fschat-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: fschat
-Version: 0.2.5
-Summary: An open platform for training, serving, and evaluating large language model based chatbots.
-Project-URL: Homepage, https://github.com/lm-sys/fastchat
-Project-URL: Bug Tracker, https://github.com/lm-sys/fastchat/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # FastChat
-| [Demo](https://chat.lmsys.org/) | [Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) | [Twitter](https://twitter.com/lmsysorg) |
-
-An open platform for training, serving, and evaluating large language model based chatbots.
-
-## Release
-<p align="center">
-<a href="https://vicuna.lmsys.org"><img src="assets/vicuna_logo.jpeg" width="20%"></a>
-</p>
+| [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**](https://twitter.com/lmsysorg) |
 
-- 🔥 We released **FastChat-T5** compatible with commercial usage. Checkout [weights](#fastchat-t5).
-
-- 🔥 We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org/).
+FastChat is an open platform for training, serving, and evaluating large language model based chatbots. The core features include:
+- The weights, training code, and evaluation code for state-of-the-art models (e.g., Vicuna, FastChat-T5).
+- A distributed multi-model serving system with Web UI and OpenAI-Compatible RESTful APIs.
+
+## News
+- [2023/05] 🔥 We introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post](https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
+- [2023/04] We released **FastChat-T5** compatible with commercial usage. Check out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org).
+- [2023/03] We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo](https://chat.lmsys.org).
 
 <a href="https://chat.lmsys.org"><img src="assets/demo_narrow.gif" width="70%"></a>
 
 ## Contents
 - [Install](#install)
 - [Model Weights](#model-weights)
 - [Inference with Command Line Interface](#inference-with-command-line-interface)
@@ -64,38 +49,40 @@
 ```
 
 ## Model Weights
 ### Vicuna Weights
 We release [Vicuna](https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA model license.
 You can add our delta to the original LLaMA weights to obtain the Vicuna weights. Instructions:
 
-1. Get the original LLaMA weights in the huggingface format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
+1. Get the original LLaMA weights in the Hugging Face format by following the instructions [here](https://huggingface.co/docs/transformers/main/model_doc/llama).
 2. Use the following scripts to get Vicuna weights by applying our delta. They will automatically download delta weights from our Hugging Face [account](https://huggingface.co/lmsys).
 
 **NOTE**:
 Weights v1.1 are only compatible with ```transformers>=4.28.0``` and ``fschat >= 0.2.0``.
 Please update your local packages accordingly. If you follow the above commands to do a fresh install, then you should get all the correct versions.
 
 #### Vicuna-7B
 This conversion command needs around 30 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
+Replace `/path/to/*` with the real paths.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-7b \
-    --target-model-path /output/path/to/vicuna-7b \
+    --target-model-path /path/to/output/vicuna-7b \
     --delta-path lmsys/vicuna-7b-delta-v1.1
 ```
 
 #### Vicuna-13B
 This conversion command needs around 60 GB of CPU RAM.
 See the "Low CPU Memory Conversion" section below if you do not have enough memory.
+Replace `/path/to/*` with the real paths.
 ```bash
 python3 -m fastchat.model.apply_delta \
     --base-model-path /path/to/llama-13b \
-    --target-model-path /output/path/to/vicuna-13b \
+    --target-model-path /path/to/output/vicuna-13b \
     --delta-path lmsys/vicuna-13b-delta-v1.1
 ```
 
 #### Old weights
 See [docs/vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of weights and their differences.
 
 #### Low CPU Memory Conversion
@@ -117,24 +104,26 @@
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_cli.png" width="70%"></a>
 
 #### Supported Models
 The following models are tested:
 - Vicuna, Alpaca, LLaMA, Koala
 - [lmsys/fastchat-t5-3b-v1.0](https://huggingface.co/lmsys/fastchat-t5)
+- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [databricks/dolly-v2-12b](https://huggingface.co/databricks/dolly-v2-12b)
 - [OpenAssistant/oasst-sft-1-pythia-12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b)
 - [project-baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B)
-- [BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven)
 - [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/stablelm-tuned-alpha-7b)
 - [THUDM/chatglm-6b](https://huggingface.co/THUDM/chatglm-6b)
+- [FreedomIntelligence/phoenix-inst-chat-7b](https://huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b)
 
 #### Single GPU
 The command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B.
 See the "No Enough Memory" section below if you do not have enough memory.
+Replace `/path/to/model/weights` with the a local folder or a Hugging repo id.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights
 ```
 
 #### Multiple GPUs
 You can use model parallelism to aggregate GPU memory from multiple GPUs on the same machine.
 ```
@@ -163,32 +152,38 @@
 Vicuna-13B with 8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU.
 ```
 python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
 ```
 
 In addition to that, you can add `--cpu-offloading` to commands above to offload weights that don't fit on your GPU onto the CPU memory. This requires 8-bit compression to be enabled and the bitsandbytes package to be installed, which is only available on linux operating systems.
 
+#### More Platforms
+
+- [MLC LLM](https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs and web browsers via Vulkan, Metal, CUDA and WebGPU.
+
 ## Serving with Web GUI
 
 <a href="https://chat.lmsys.org"><img src="assets/screenshot_gui.png" width="70%"></a>
 
-To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. Here are the commands to follow in your terminal:
+To serve using the web UI, you need three main components: web servers that interface with users, model workers that host one or more models, and a controller to coordinate the webserver and model workers. You can learn more about the architecture [here](docs/server_arch.md).
+
+Here are the commands to follow in your terminal:
 
 #### Launch the controller
 ```bash
 python3 -m fastchat.serve.controller
 ```
 
 This controller manages the distributed workers.
 
-#### Launch the model worker
+#### Launch the model worker(s)
 ```bash
 python3 -m fastchat.serve.model_worker --model-path /path/to/model/weights
 ```
-Wait until the process finishes loading the model and you see "Uvicorn running on ...". You can launch multiple model workers to serve multiple models concurrently. The model worker will connect to the controller automatically.
+Wait until the process finishes loading the model and you see "Uvicorn running on ...". The model worker will register itself to the controller .
 
 To ensure that your model worker is connected to your controller properly, send a test message using the following command:
 ```bash
 python3 -m fastchat.serve.test_message --model-name vicuna-7b
 ```
 You will see a short output.
 
@@ -196,88 +191,36 @@
 ```bash
 python3 -m fastchat.serve.gradio_web_server
 ```
 
 This is the user interface that users will interact with.
 
 By following these steps, you will be able to serve your models using the web UI. You can open your browser and chat with a model now.
+If the models do not show up, try to reboot the gradio web server.
 
-
-## API
-
-### Huggingface Generation APIs
-See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py)
-
-### OpenAI-compatible RESTful APIs & SDK
-
-(Experimental. We will keep improving the API and SDK.)
-
-#### Chat Completion
-
-Reference: https://platform.openai.com/docs/api-reference/chat/create
-
-Some features/compatibilities to be implemented:
-
-- [ ] streaming
-- [ ] support of some parameters like `top_p`, `presence_penalty`
-- [ ] proper error handling (e.g. model not found)
-- [ ] the return value in the client SDK could be used like a dict
-
-
-**RESTful API Server**
-
-First, launch the controller
-
-```bash
-python3 -m fastchat.serve.controller
+#### (Optional): Advanced Features
+- You can register multiple model workers to a single controller, which can be used for serving a single model with higher throughput or serving multiple models at the same time. When doing so, please allocate different GPUs and ports for different model workers.
 ```
-
-Then, launch the model worker(s)
-
-```bash
-python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-path /path/to/vicuna/weights
+# worker 0
+CUDA_VISIBLE_DEVICES=0 python3 -m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --controller http://localhost:21001 --port 31000 --worker http://localhost:31000
+# worker 1
+CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --port 31001 --worker http://localhost:31001
 ```
-
-Finally, launch the RESTful API server
-
+- You can also launch a multi-tab gradio server, which includes the Chatbot Arena tabs.
 ```bash
-export FASTCHAT_CONTROLLER_URL=http://localhost:21001
-python3 -m fastchat.serve.api --host localhost --port 8000
+python3 -m fastchat.serve.gradio_web_server_multi
 ```
 
-Test the API server
-
-```bash
-curl http://localhost:8000/v1/chat/completions \
-  -H "Content-Type: application/json" \
-  -d '{
-    "model": "vicuna-7b-v1.1",
-    "messages": [{"role": "user", "content": "Hello!"}]
-  }'
-```
-
-**Client SDK**
-
-Assuming environment variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://localhost:8000`), you can use the following code to send a request to the API server:
-
-```python
-import os
-from fastchat import client
-
-client.set_baseurl(os.getenv("FASTCHAT_BASEURL"))
-
-completion = client.ChatCompletion.create(
-  model="vicuna-7b-v1.1",
-  messages=[
-    {"role": "user", "content": "Hello!"}
-  ]
-)
+## API
+### OpenAI-Compatible RESTful APIs & SDK
+FastChat provides OpenAI-Compatible APIs for its supported models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+See [docs/openai_api.md](docs/openai_api.md).
 
-print(completion.choices[0].message)
-```
+### Hugging Face Generation APIs
+See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py).
 
 ## Evaluation
 
 Our AI-enhanced evaluation pipeline is based on GPT-4. This section provides a high-level summary of the pipeline. For detailed instructions, please refer to the [evaluation](fastchat/eval) documentation.
 
 ### Pipeline Steps
```

#### html2text {}

```diff
@@ -1,50 +1,50 @@
-Metadata-Version: 2.1 Name: fschat Version: 0.2.5 Summary: An open platform for
-training, serving, and evaluating large language model based chatbots. Project-
-URL: Homepage, https://github.com/lm-sys/fastchat Project-URL: Bug Tracker,
-https://github.com/lm-sys/fastchat/issues Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev License-File: LICENSE # FastChat | [Demo](https://chat.lmsys.org/) |
-[Arena](https://arena.lmsys.org) | [Discord](https://discord.gg/h6kCZb72G7) |
-[Twitter](https://twitter.com/lmsysorg) | An open platform for training,
-serving, and evaluating large language model based chatbots. ## Release
-                           [assets/vicuna_logo.jpeg]
-- ð¥ We released **FastChat-T5** compatible with commercial usage. Checkout
-[weights](#fastchat-t5). - ð¥ We released **Vicuna: An Open-Source Chatbot
-Impressing GPT-4 with 90% ChatGPT Quality**. Checkout the blog [post](https://
-vicuna.lmsys.org) and [demo](https://chat.lmsys.org/). [assets/demo_narrow.gif]
-## Contents - [Install](#install) - [Model Weights](#model-weights) -
-[Inference with Command Line Interface](#inference-with-command-line-interface)
-- [Serving with Web GUI](#serving-with-web-gui) - [API](#api) - [Evaluation]
-(#evaluation) - [Fine-tuning](#fine-tuning) ## Install ### Method 1: With pip
-```bash pip3 install fschat ``` ### Method 2: From source 1. Clone this
-repository and navigate to the FastChat folder ```bash git clone https://
-github.com/lm-sys/FastChat.git cd FastChat ``` If you are running on Mac:
-```bash brew install rust cmake ``` 2. Install Package ```bash pip3 install --
-upgrade pip # enable PEP 660 support pip3 install -e . ``` ## Model Weights ###
-Vicuna Weights We release [Vicuna](https://vicuna.lmsys.org/) weights as delta
-weights to comply with the LLaMA model license. You can add our delta to the
-original LLaMA weights to obtain the Vicuna weights. Instructions: 1. Get the
-original LLaMA weights in the huggingface format by following the instructions
-[here](https://huggingface.co/docs/transformers/main/model_doc/llama). 2. Use
-the following scripts to get Vicuna weights by applying our delta. They will
-automatically download delta weights from our Hugging Face [account](https://
-huggingface.co/lmsys). **NOTE**: Weights v1.1 are only compatible with
+# FastChat | [**Demo**](https://chat.lmsys.org/) | [**Arena**](https://
+arena.lmsys.org) | [**Discord**](https://discord.gg/h6kCZb72G7) | [**Twitter**]
+(https://twitter.com/lmsysorg) | FastChat is an open platform for training,
+serving, and evaluating large language model based chatbots. The core features
+include: - The weights, training code, and evaluation code for state-of-the-art
+models (e.g., Vicuna, FastChat-T5). - A distributed multi-model serving system
+with Web UI and OpenAI-Compatible RESTful APIs. ## News - [2023/05] ð¥ We
+introduced **Chatbot Arena** for battles among LLMs. Check out the blog [post]
+(https://lmsys.org/blog/2023-05-03-arena) and [demo](https://arena.lmsys.org).
+- [2023/04] We released **FastChat-T5** compatible with commercial usage. Check
+out the [weights](#fastchat-t5) and [demo](https://chat.lmsys.org). - [2023/03]
+We released **Vicuna: An Open-Source Chatbot Impressing GPT-4 with 90% ChatGPT
+Quality**. Check out the blog [post](https://vicuna.lmsys.org) and [demo]
+(https://chat.lmsys.org). [assets/demo_narrow.gif] ## Contents - [Install]
+(#install) - [Model Weights](#model-weights) - [Inference with Command Line
+Interface](#inference-with-command-line-interface) - [Serving with Web GUI]
+(#serving-with-web-gui) - [API](#api) - [Evaluation](#evaluation) - [Fine-
+tuning](#fine-tuning) ## Install ### Method 1: With pip ```bash pip3 install
+fschat ``` ### Method 2: From source 1. Clone this repository and navigate to
+the FastChat folder ```bash git clone https://github.com/lm-sys/FastChat.git cd
+FastChat ``` If you are running on Mac: ```bash brew install rust cmake ``` 2.
+Install Package ```bash pip3 install --upgrade pip # enable PEP 660 support
+pip3 install -e . ``` ## Model Weights ### Vicuna Weights We release [Vicuna]
+(https://vicuna.lmsys.org/) weights as delta weights to comply with the LLaMA
+model license. You can add our delta to the original LLaMA weights to obtain
+the Vicuna weights. Instructions: 1. Get the original LLaMA weights in the
+Hugging Face format by following the instructions [here](https://
+huggingface.co/docs/transformers/main/model_doc/llama). 2. Use the following
+scripts to get Vicuna weights by applying our delta. They will automatically
+download delta weights from our Hugging Face [account](https://huggingface.co/
+lmsys). **NOTE**: Weights v1.1 are only compatible with
 ```transformers>=4.28.0``` and ``fschat >= 0.2.0``. Please update your local
 packages accordingly. If you follow the above commands to do a fresh install,
 then you should get all the correct versions. #### Vicuna-7B This conversion
 command needs around 30 GB of CPU RAM. See the "Low CPU Memory Conversion"
-section below if you do not have enough memory. ```bash python3 -
-m fastchat.model.apply_delta \ --base-model-path /path/to/llama-7b \ --target-
-model-path /output/path/to/vicuna-7b \ --delta-path lmsys/vicuna-7b-delta-v1.1
-``` #### Vicuna-13B This conversion command needs around 60 GB of CPU RAM. See
-the "Low CPU Memory Conversion" section below if you do not have enough memory.
+section below if you do not have enough memory. Replace `/path/to/*` with the
+real paths. ```bash python3 -m fastchat.model.apply_delta \ --base-model-path /
+path/to/llama-7b \ --target-model-path /path/to/output/vicuna-7b \ --delta-path
+lmsys/vicuna-7b-delta-v1.1 ``` #### Vicuna-13B This conversion command needs
+around 60 GB of CPU RAM. See the "Low CPU Memory Conversion" section below if
+you do not have enough memory. Replace `/path/to/*` with the real paths.
 ```bash python3 -m fastchat.model.apply_delta \ --base-model-path /path/to/
-llama-13b \ --target-model-path /output/path/to/vicuna-13b \ --delta-path
+llama-13b \ --target-model-path /path/to/output/vicuna-13b \ --delta-path
 lmsys/vicuna-13b-delta-v1.1 ``` #### Old weights See [docs/
 vicuna_weights_version.md](docs/vicuna_weights_version.md) for all versions of
 weights and their differences. #### Low CPU Memory Conversion You can try these
 methods to reduce the CPU RAM requirement of weight conversion. 1. Append `--
 low-cpu-mem` to the commands above, which will split large weight files into
 smaller ones and use the disk as temporary storage. This can keep the peak
 memory at less than 16GB. 2. Create a large swap file and rely on the operating
@@ -53,92 +53,92 @@
 weights from a Hugging Face [repo](https://huggingface.co/lmsys/fastchat-t5-3b-
 v1.0). ```bash python3 -m fastchat.serve.cli --model-path lmsys/fastchat-t5-3b-
 v1.0 ``` ## Inference with Command Line Interface (Experimental Feature: You
 can specify `--style rich` to enable rich text output and better text streaming
 quality for some non-ASCII content. This may not work properly on certain
 terminals.) [assets/screenshot_cli.png] #### Supported Models The following
 models are tested: - Vicuna, Alpaca, LLaMA, Koala - [lmsys/fastchat-t5-3b-v1.0]
-(https://huggingface.co/lmsys/fastchat-t5) - [databricks/dolly-v2-12b](https://
+(https://huggingface.co/lmsys/fastchat-t5) - [BlinkDL/RWKV-4-Raven](https://
+huggingface.co/BlinkDL/rwkv-4-raven) - [databricks/dolly-v2-12b](https://
 huggingface.co/databricks/dolly-v2-12b) - [OpenAssistant/oasst-sft-1-pythia-
 12b](https://huggingface.co/OpenAssistant/oasst-sft-1-pythia-12b) - [project-
 baize/baize-lora-7B](https://huggingface.co/project-baize/baize-lora-7B) -
-[BlinkDL/RWKV-4-Raven](https://huggingface.co/BlinkDL/rwkv-4-raven) -
 [StabilityAI/stablelm-tuned-alpha-7b](https://huggingface.co/stabilityai/
 stablelm-tuned-alpha-7b) - [THUDM/chatglm-6b](https://huggingface.co/THUDM/
-chatglm-6b) #### Single GPU The command below requires around 28GB of GPU
-memory for Vicuna-13B and 14GB of GPU memory for Vicuna-7B. See the "No Enough
-Memory" section below if you do not have enough memory. ``` python3 -
-m fastchat.serve.cli --model-path /path/to/model/weights ``` #### Multiple GPUs
-You can use model parallelism to aggregate GPU memory from multiple GPUs on the
-same machine. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
-weights --num-gpus 2 ``` #### CPU Only This runs on the CPU only and does not
-require GPU. It requires around 60GB of CPU memory for Vicuna-13B and around
-30GB of CPU memory for Vicuna-7B. ``` python3 -m fastchat.serve.cli --model-
-path /path/to/model/weights --device cpu ``` #### Metal Backend (Mac Computers
-with Apple Silicon or AMD GPUs) Use `--device mps` to enable GPU acceleration
-on Mac computers (requires torch >= 2.0). Use `--load-8bit` to turn on 8-bit
-compression. ``` python3 -m fastchat.serve.cli --model-path /path/to/model/
-weights --device mps --load-8bit ``` Vicuna-7B can run on a 32GB M1 Macbook
-with 1 - 2 words / second. #### No Enough Memory If you do not have enough
-memory, you can enable 8-bit compression by adding `--load-8bit` to commands
-above. This can reduce memory usage by around half with slightly degraded model
-quality. It is compatible with the CPU, GPU, and Metal backend. Vicuna-13B with
-8-bit compression can run on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ```
-python3 -m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit
-``` In addition to that, you can add `--cpu-offloading` to commands above to
-offload weights that don't fit on your GPU onto the CPU memory. This requires
-8-bit compression to be enabled and the bitsandbytes package to be installed,
-which is only available on linux operating systems. ## Serving with Web GUI
+chatglm-6b) - [FreedomIntelligence/phoenix-inst-chat-7b](https://
+huggingface.co/FreedomIntelligence/phoenix-inst-chat-7b) #### Single GPU The
+command below requires around 28GB of GPU memory for Vicuna-13B and 14GB of GPU
+memory for Vicuna-7B. See the "No Enough Memory" section below if you do not
+have enough memory. Replace `/path/to/model/weights` with the a local folder or
+a Hugging repo id. ``` python3 -m fastchat.serve.cli --model-path /path/to/
+model/weights ``` #### Multiple GPUs You can use model parallelism to aggregate
+GPU memory from multiple GPUs on the same machine. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --num-gpus 2 ``` ####
+CPU Only This runs on the CPU only and does not require GPU. It requires around
+60GB of CPU memory for Vicuna-13B and around 30GB of CPU memory for Vicuna-7B.
+``` python3 -m fastchat.serve.cli --model-path /path/to/model/weights --device
+cpu ``` #### Metal Backend (Mac Computers with Apple Silicon or AMD GPUs) Use
+`--device mps` to enable GPU acceleration on Mac computers (requires torch >=
+2.0). Use `--load-8bit` to turn on 8-bit compression. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --device mps --load-
+8bit ``` Vicuna-7B can run on a 32GB M1 Macbook with 1 - 2 words / second. ####
+No Enough Memory If you do not have enough memory, you can enable 8-bit
+compression by adding `--load-8bit` to commands above. This can reduce memory
+usage by around half with slightly degraded model quality. It is compatible
+with the CPU, GPU, and Metal backend. Vicuna-13B with 8-bit compression can run
+on a single NVIDIA 3090/4080/T4/V100(16GB) GPU. ``` python3 -
+m fastchat.serve.cli --model-path /path/to/model/weights --load-8bit ``` In
+addition to that, you can add `--cpu-offloading` to commands above to offload
+weights that don't fit on your GPU onto the CPU memory. This requires 8-bit
+compression to be enabled and the bitsandbytes package to be installed, which
+is only available on linux operating systems. #### More Platforms - [MLC LLM]
+(https://mlc.ai/mlc-llm/), backed by [TVM Unity](https://github.com/apache/tvm/
+tree/unity) compiler, deploys Vicuna natively on phones, consumer-class GPUs
+and web browsers via Vulkan, Metal, CUDA and WebGPU. ## Serving with Web GUI
 [assets/screenshot_gui.png] To serve using the web UI, you need three main
 components: web servers that interface with users, model workers that host one
 or more models, and a controller to coordinate the webserver and model workers.
-Here are the commands to follow in your terminal: #### Launch the controller
-```bash python3 -m fastchat.serve.controller ``` This controller manages the
-distributed workers. #### Launch the model worker ```bash python3 -
+You can learn more about the architecture [here](docs/server_arch.md). Here are
+the commands to follow in your terminal: #### Launch the controller ```bash
+python3 -m fastchat.serve.controller ``` This controller manages the
+distributed workers. #### Launch the model worker(s) ```bash python3 -
 m fastchat.serve.model_worker --model-path /path/to/model/weights ``` Wait
 until the process finishes loading the model and you see "Uvicorn running on
-...". You can launch multiple model workers to serve multiple models
-concurrently. The model worker will connect to the controller automatically. To
-ensure that your model worker is connected to your controller properly, send a
-test message using the following command: ```bash python3 -
-m fastchat.serve.test_message --model-name vicuna-7b ``` You will see a short
-output. #### Launch the Gradio web server ```bash python3 -
-m fastchat.serve.gradio_web_server ``` This is the user interface that users
-will interact with. By following these steps, you will be able to serve your
-models using the web UI. You can open your browser and chat with a model now.
-## API ### Huggingface Generation APIs See [fastchat/serve/huggingface_api.py]
-(fastchat/serve/huggingface_api.py) ### OpenAI-compatible RESTful APIs & SDK
-(Experimental. We will keep improving the API and SDK.) #### Chat Completion
-Reference: https://platform.openai.com/docs/api-reference/chat/create Some
-features/compatibilities to be implemented: - [ ] streaming - [ ] support of
-some parameters like `top_p`, `presence_penalty` - [ ] proper error handling
-(e.g. model not found) - [ ] the return value in the client SDK could be used
-like a dict **RESTful API Server** First, launch the controller ```bash python3
--m fastchat.serve.controller ``` Then, launch the model worker(s) ```bash
-python3 -m fastchat.serve.model_worker --model-name 'vicuna-7b-v1.1' --model-
-path /path/to/vicuna/weights ``` Finally, launch the RESTful API server ```bash
-export FASTCHAT_CONTROLLER_URL=http://localhost:21001 python3 -
-m fastchat.serve.api --host localhost --port 8000 ``` Test the API server
-```bash curl http://localhost:8000/v1/chat/completions \ -H "Content-Type:
-application/json" \ -d '{ "model": "vicuna-7b-v1.1", "messages": [{"role":
-"user", "content": "Hello!"}] }' ``` **Client SDK** Assuming environment
-variable `FASTCHAT_BASEURL` is set to the API server URL (e.g., `http://
-localhost:8000`), you can use the following code to send a request to the API
-server: ```python import os from fastchat import client client.set_baseurl
-(os.getenv("FASTCHAT_BASEURL")) completion = client.ChatCompletion.create
-( model="vicuna-7b-v1.1", messages=[ {"role": "user", "content": "Hello!"} ] )
-print(completion.choices[0].message) ``` ## Evaluation Our AI-enhanced
-evaluation pipeline is based on GPT-4. This section provides a high-level
-summary of the pipeline. For detailed instructions, please refer to the
-[evaluation](fastchat/eval) documentation. ### Pipeline Steps 1. Generate
-answers from different models: Use `qa_baseline_gpt35.py` for ChatGPT, or
-specify the model checkpoint and run `get_model_answer.py` for Vicuna and other
-models. 2. Generate reviews with GPT-4: Use GPT-4 to generate reviews
-automatically. This step can also be performed manually if the GPT-4 API is not
-available to you. 3. Generate visualization data: Run
+...". The model worker will register itself to the controller . To ensure that
+your model worker is connected to your controller properly, send a test message
+using the following command: ```bash python3 -m fastchat.serve.test_message --
+model-name vicuna-7b ``` You will see a short output. #### Launch the Gradio
+web server ```bash python3 -m fastchat.serve.gradio_web_server ``` This is the
+user interface that users will interact with. By following these steps, you
+will be able to serve your models using the web UI. You can open your browser
+and chat with a model now. If the models do not show up, try to reboot the
+gradio web server. #### (Optional): Advanced Features - You can register
+multiple model workers to a single controller, which can be used for serving a
+single model with higher throughput or serving multiple models at the same
+time. When doing so, please allocate different GPUs and ports for different
+model workers. ``` # worker 0 CUDA_VISIBLE_DEVICES=0 python3 -
+m fastchat.serve.model_worker --model-path lmsys/fastchat-t5-3b-v1.0 --
+controller http://localhost:21001 --port 31000 --worker http://localhost:31000
+# worker 1 CUDA_VISIBLE_DEVICES=1 python3 -m fastchat.serve.model_worker --
+model-path ~/model_weights/vicuna-7b/ --controller http://localhost:21001 --
+port 31001 --worker http://localhost:31001 ``` - You can also launch a multi-
+tab gradio server, which includes the Chatbot Arena tabs. ```bash python3 -
+m fastchat.serve.gradio_web_server_multi ``` ## API ### OpenAI-Compatible
+RESTful APIs & SDK FastChat provides OpenAI-Compatible APIs for its supported
+models, so you can use FastChat as a local drop-in replacement for OpenAI APIs.
+See [docs/openai_api.md](docs/openai_api.md). ### Hugging Face Generation APIs
+See [fastchat/serve/huggingface_api.py](fastchat/serve/huggingface_api.py). ##
+Evaluation Our AI-enhanced evaluation pipeline is based on GPT-4. This section
+provides a high-level summary of the pipeline. For detailed instructions,
+please refer to the [evaluation](fastchat/eval) documentation. ### Pipeline
+Steps 1. Generate answers from different models: Use `qa_baseline_gpt35.py` for
+ChatGPT, or specify the model checkpoint and run `get_model_answer.py` for
+Vicuna and other models. 2. Generate reviews with GPT-4: Use GPT-4 to generate
+reviews automatically. This step can also be performed manually if the GPT-
+4 API is not available to you. 3. Generate visualization data: Run
 `generate_webpage_data_from_table.py` to generate data for a static website,
 which allows you to visualize the evaluation data. 4. Visualize the data: Serve
 a static website under the `webpage` directory. You can use `python3 -
 m http.server` to serve the website locally. ### Data Format and Contribution
 We use a data format encoded with JSON Lines for evaluation. The format
 includes information on models, prompts, reviewers, questions, answers, and
 reviews. You can customize the evaluation process or contribute to our project
```

### Comparing `fschat-0.2.5/pyproject.toml` & `fschat-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fschat"
-version = "0.2.5"
+version = "0.2.6"
 description = "An open platform for training, serving, and evaluating large language model based chatbots."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
-    "accelerate", "fastapi", "gradio==3.23", "markdown2[all]", "numpy",
-    "prompt_toolkit>=3.0.0", "requests", "rich>=10.0.0", "sentencepiece",
-    "shortuuid", "transformers>=4.28.0,<4.29.0", "tokenizers>=0.12.1", "torch",
-    "uvicorn", "wandb", "httpx", "shortuuid", "pydantic", "nh3",
+    "accelerate", "fastapi", "gradio==3.23", "httpx", "markdown2[all]", "nh3", "numpy",
+    "prompt_toolkit>=3.0.0", "pydantic", "requests", "rich>=10.0.0", "sentencepiece",
+    "shortuuid", "shortuuid", "tokenizers>=0.12.1", "torch",
+    "transformers>=4.28.0,<4.29.0", "uvicorn", "wandb"
 ]
 
 [project.optional-dependencies]
 dev = ["black==23.3.0", "pylint==2.8.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/lm-sys/fastchat"
```

