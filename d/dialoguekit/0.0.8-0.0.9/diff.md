# Comparing `tmp/dialoguekit-0.0.8.tar.gz` & `tmp/dialoguekit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialoguekit-0.0.8.tar", last modified: Tue Jan 31 14:12:44 2023, max compression
+gzip compressed data, was "dialoguekit-0.0.9.tar", last modified: Mon May  8 08:14:35 2023, max compression
```

## Comparing `dialoguekit-0.0.8.tar` & `dialoguekit-0.0.9.tar`

### file list

```diff
@@ -1,166 +1,171 @@
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.049963 dialoguekit-0.0.8/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       56 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/.environment.yml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      106 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/.flake8
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.702606 dialoguekit-0.0.8/.github/
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.702346 dialoguekit-0.0.8/.github/actions/
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.892411 dialoguekit-0.0.8/.github/actions/build_docs/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3903 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/.github/actions/build_docs/action.yml
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.901645 dialoguekit-0.0.8/.github/workflows/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     5424 2023-01-25 12:56:56.000000 dialoguekit-0.0.8/.github/workflows/CI.yaml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1038 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/.github/workflows/build_docs.yaml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1596 2023-01-27 14:40:23.000000 dialoguekit-0.0.8/.github/workflows/merge.yaml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2068 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/.gitignore
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1312 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    11357 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/LICENSE
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       57 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/MANIFEST.in
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3696 2023-01-31 14:12:44.049601 dialoguekit-0.0.8/PKG-INFO
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3064 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/README.md
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      119 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/conftest.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.734721 dialoguekit-0.0.8/dialoguekit/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      168 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/dialoguekit/__init__.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.736885 dialoguekit-0.0.8/dialoguekit/connector/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      141 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/dialoguekit/connector/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     6580 2023-01-31 14:10:51.000000 dialoguekit-0.0.8/dialoguekit/connector/dialogue_connector.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.748644 dialoguekit-0.0.8/dialoguekit/core/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      565 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/core/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     5284 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/dialoguekit/core/annotated_utterance.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      277 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/dialoguekit/core/annotation.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3497 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/dialoguekit/core/dialogue.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      834 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/core/domain.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2057 2023-01-02 14:36:22.000000 dialoguekit-0.0.8/dialoguekit/core/intent.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      461 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/dialoguekit/core/slot_value_annotation.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2379 2023-01-02 14:55:53.000000 dialoguekit-0.0.8/dialoguekit/core/utterance.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.759518 dialoguekit-0.0.8/dialoguekit/nlg/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      247 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/__init__.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.941661 dialoguekit-0.0.8/dialoguekit/nlg/models/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   589309 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/models/LinearSVC_2_0.joblib
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   287694 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/models/vectorizer_0_0.joblib
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   288104 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/models/vectorizer_2_0.joblib
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)  1425754 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/models/xgb_0_0.json
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1370 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/nlg_abstract.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     7769 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/nlg_conditional.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     8143 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlg/nlg_template.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     6857 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/dialoguekit/nlg/template_from_training_data.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.763304 dialoguekit-0.0.8/dialoguekit/nlu/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      674 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlu/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2084 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/dialoguekit/nlu/intent_classifier.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.767797 dialoguekit-0.0.8/dialoguekit/nlu/models/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       40 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    10246 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/diet_classifier_rasa.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3120 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/intent_classifier_cosine.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.953084 dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   589309 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/LinearSVC_2_0.joblib
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       29 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   287694 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/vectorizer_0_0.joblib
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   288104 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/vectorizer_2_0.joblib
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)  1425754 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/xgb_0_0.json
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4643 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction_classifier.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1337 2022-12-06 15:17:26.000000 dialoguekit-0.0.8/dialoguekit/nlu/nlu.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      296 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/dialoguekit/nlu/slot_annotator_dict.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.839197 dialoguekit-0.0.8/dialoguekit/participant/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      243 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/dialoguekit/participant/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1715 2023-01-31 14:10:51.000000 dialoguekit-0.0.8/dialoguekit/participant/agent.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1858 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/dialoguekit/participant/participant.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1410 2023-01-20 13:53:02.000000 dialoguekit-0.0.8/dialoguekit/participant/user.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1821 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/dialoguekit/participant/user_preferences.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.845836 dialoguekit-0.0.8/dialoguekit/platforms/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      119 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/platforms/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      658 2022-11-21 09:36:14.000000 dialoguekit-0.0.8/dialoguekit/platforms/platform.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.848881 dialoguekit-0.0.8/dialoguekit/utils/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      349 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/utils/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1133 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/utils/annotation_converter.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     9558 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/dialoguekit/utils/annotation_converter_dialoguekit_to_rasa.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     9444 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/dialoguekit/utils/dialogue_evaluation.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2637 2022-11-25 14:51:04.000000 dialoguekit-0.0.8/dialoguekit/utils/dialogue_reader.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.912617 dialoguekit-0.0.8/dialoguekit.egg-info/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3696 2023-01-31 14:12:43.000000 dialoguekit-0.0.8/dialoguekit.egg-info/PKG-INFO
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     6820 2023-01-31 14:12:43.000000 dialoguekit-0.0.8/dialoguekit.egg-info/SOURCES.txt
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)        1 2023-01-31 14:12:43.000000 dialoguekit-0.0.8/dialoguekit.egg-info/dependency_links.txt
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)        1 2023-01-24 12:23:50.000000 dialoguekit-0.0.8/dialoguekit.egg-info/not-zip-safe
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       10 2023-01-31 14:12:43.000000 dialoguekit-0.0.8/dialoguekit.egg-info/requires.txt
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       32 2023-01-31 14:12:43.000000 dialoguekit-0.0.8/dialoguekit.egg-info/top_level.txt
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.970136 dialoguekit-0.0.8/docs/
--rwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)      646 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/Makefile
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      309 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/docs/README.md
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    10698 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/components.graffle
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      898 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/evaluation.md
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       73 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/index.html
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.002692 dialoguekit-0.0.8/docs/source/
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.010909 dialoguekit-0.0.8/docs/source/_static/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    82269 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/source/_static/DialogueKit-Architecture.png
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     8167 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/source/_static/favicon.png
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.016356 dialoguekit-0.0.8/docs/source/_templates/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      719 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/docs/source/_templates/layout.html
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      816 2023-01-20 13:53:09.000000 dialoguekit-0.0.8/docs/source/_templates/versions.html
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      172 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/docs/source/components.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3505 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/docs/source/concepts.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3589 2023-01-27 14:40:23.000000 dialoguekit-0.0.8/docs/source/conf.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      792 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/source/dialogue_export.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      352 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/source/docs_env.yaml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1519 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/docs/source/external_agents.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      443 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/docs/source/index.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      886 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/source/installation.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2497 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/docs/source/nlg.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3470 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/docs/source/nlu.rst
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      945 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/docs/source/usage.rst
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.710337 dialoguekit-0.0.8/external_agents/
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.024757 dialoguekit-0.0.8/external_agents/rasa-parrot/
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.026219 dialoguekit-0.0.8/external_agents/rasa-parrot/actions/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       47 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/actions/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1628 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/actions/actions.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1517 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/config.yml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      980 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/credentials.yml
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.038958 dialoguekit-0.0.8/external_agents/rasa-parrot/data/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      372 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/data/nlu.yml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       25 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/data/rules.yml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      169 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/data/stories.yml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      223 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/domain.yml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1409 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/external_agents/rasa-parrot/endpoints.yml
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      141 2023-01-25 12:03:24.000000 dialoguekit-0.0.8/pyproject.toml
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.045172 dialoguekit-0.0.8/requirements/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      175 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/requirements/docs_requirements.txt
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      195 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/requirements/pre_commit.txt
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       52 2023-01-26 07:58:32.000000 dialoguekit-0.0.8/requirements/requirements.txt
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.856392 dialoguekit-0.0.8/sample_agents/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      337 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/sample_agents/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4232 2023-01-31 14:10:51.000000 dialoguekit-0.0.8/sample_agents/moviebot_agent.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1819 2023-01-31 14:10:51.000000 dialoguekit-0.0.8/sample_agents/parrot_agent.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2261 2023-01-31 14:10:51.000000 dialoguekit-0.0.8/sample_agents/rasa_parrot_agent.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3910 2023-01-31 14:10:51.000000 dialoguekit-0.0.8/sample_agents/woz_agent.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       38 2023-01-31 14:12:44.050107 dialoguekit-0.0.8/setup.cfg
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1249 2023-01-27 14:40:23.000000 dialoguekit-0.0.8/setup.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.860727 dialoguekit-0.0.8/tests/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       35 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/__init__.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.867457 dialoguekit-0.0.8/tests/core/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       41 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/core/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1489 2023-01-02 14:56:07.000000 dialoguekit-0.0.8/tests/core/test_annotated_utterance.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     5531 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/tests/core/test_dialogue.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1300 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/core/test_intent.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      434 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/core/test_ontology.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1627 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/tests/core/test_slot_value_annotation.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1002 2023-01-02 14:56:11.000000 dialoguekit-0.0.8/tests/core/test_utterance.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.047324 dialoguekit-0.0.8/tests/data/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    35729 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/data/annotated_dialogues.json
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:44.048841 dialoguekit-0.0.8/tests/data/domains/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       39 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/data/domains/movie.yaml
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.871044 dialoguekit-0.0.8/tests/nlg/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       46 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/nlg/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     5469 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/nlg/test_conditional_nlg.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     7640 2023-01-27 13:58:47.000000 dialoguekit-0.0.8/tests/nlg/test_template_from_training_data.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4158 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/nlg/test_template_nlg.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.875677 dialoguekit-0.0.8/tests/nlu/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       39 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/nlu/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2967 2022-12-06 15:17:26.000000 dialoguekit-0.0.8/tests/nlu/test_diet_classifier_rasa.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4135 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/nlu/test_intent_classifier_cosine.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1408 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/nlu/test_satisfaction_classifier.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.878928 dialoguekit-0.0.8/tests/sample_agents/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       49 2022-12-12 10:58:22.000000 dialoguekit-0.0.8/tests/sample_agents/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1449 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/tests/sample_agents/test_parrot_agent.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.880965 dialoguekit-0.0.8/tests/user/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       40 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/user/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1252 2023-01-16 17:29:08.000000 dialoguekit-0.0.8/tests/user/test_user_preferences.py
-drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-01-31 14:12:43.884093 dialoguekit-0.0.8/tests/utils/
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       39 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/utils/__init__.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2670 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/utils/test_annotation_converter_dialoguekit_to_rasa.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      677 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/utils/test_dialogue_reader.py
--rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3138 2022-11-18 08:39:36.000000 dialoguekit-0.0.8/tests/utils/test_evaluator.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.912495 dialoguekit-0.0.9/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       56 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/.environment.yml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      106 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/.flake8
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.164211 dialoguekit-0.0.9/.github/
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.163927 dialoguekit-0.0.9/.github/actions/
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.654680 dialoguekit-0.0.9/.github/actions/build_docs/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3903 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/.github/actions/build_docs/action.yml
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.678736 dialoguekit-0.0.9/.github/workflows/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     5424 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/.github/workflows/CI.yaml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1038 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/.github/workflows/build_docs.yaml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2652 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/.github/workflows/merge.yaml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2068 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/.gitignore
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1312 2023-03-10 08:13:40.000000 dialoguekit-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    11357 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/LICENSE
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       57 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/MANIFEST.in
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3869 2023-05-08 08:14:35.912089 dialoguekit-0.0.9/PKG-INFO
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3237 2023-05-08 08:14:09.000000 dialoguekit-0.0.9/README.md
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      119 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/conftest.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.223971 dialoguekit-0.0.9/dialoguekit/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      168 2022-12-12 10:58:22.000000 dialoguekit-0.0.9/dialoguekit/__init__.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.229810 dialoguekit-0.0.9/dialoguekit/connector/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      141 2022-12-12 10:58:22.000000 dialoguekit-0.0.9/dialoguekit/connector/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     6533 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/connector/dialogue_connector.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.263316 dialoguekit-0.0.9/dialoguekit/core/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      565 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/core/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1875 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/core/annotated_utterance.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      277 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/core/annotation.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4623 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/core/dialogue.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      971 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/core/dialogue_act.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1456 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/core/domain.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      606 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/core/feedback.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2057 2023-01-02 14:36:22.000000 dialoguekit-0.0.9/dialoguekit/core/intent.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      461 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/core/slot_value_annotation.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      929 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/core/utterance.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.289566 dialoguekit-0.0.9/dialoguekit/nlg/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      247 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlg/__init__.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.756015 dialoguekit-0.0.9/dialoguekit/nlg/models/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   589309 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlg/models/LinearSVC_2_0.joblib
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   287694 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlg/models/vectorizer_0_0.joblib
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   288104 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlg/models/vectorizer_2_0.joblib
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)  1425754 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlg/models/xgb_0_0.json
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1370 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlg/nlg_abstract.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     7764 2023-04-18 09:49:07.000000 dialoguekit-0.0.9/dialoguekit/nlg/nlg_conditional.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     8116 2023-04-18 09:49:07.000000 dialoguekit-0.0.9/dialoguekit/nlg/nlg_template.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     7123 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/nlg/template_from_training_data.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.322304 dialoguekit-0.0.9/dialoguekit/nlu/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      674 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlu/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2084 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/nlu/intent_classifier.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.337321 dialoguekit-0.0.9/dialoguekit/nlu/models/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       40 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    10318 2023-05-05 12:08:03.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/diet_classifier_rasa.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3120 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/intent_classifier_cosine.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.775979 dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   589309 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/LinearSVC_2_0.joblib
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       29 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   287694 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/vectorizer_0_0.joblib
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)   288104 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/vectorizer_2_0.joblib
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)  1425754 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/xgb_0_0.json
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4643 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction_classifier.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1430 2023-05-05 12:08:03.000000 dialoguekit-0.0.9/dialoguekit/nlu/nlu.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      685 2023-05-05 12:08:03.000000 dialoguekit-0.0.9/dialoguekit/nlu/slot_annotator.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      296 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/nlu/slot_annotator_dict.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.384809 dialoguekit-0.0.9/dialoguekit/participant/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      377 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/participant/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1715 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/participant/agent.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2101 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/participant/participant.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1875 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/participant/user.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1821 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/dialoguekit/participant/user_preferences.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.401685 dialoguekit-0.0.9/dialoguekit/platforms/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      307 2023-05-05 12:08:03.000000 dialoguekit-0.0.9/dialoguekit/platforms/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4158 2023-05-05 12:08:03.000000 dialoguekit-0.0.9/dialoguekit/platforms/flask_socket_platform.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3309 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/platforms/platform.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1651 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/platforms/terminal_platform.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.444172 dialoguekit-0.0.9/dialoguekit/utils/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      349 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/utils/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1133 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/dialoguekit/utils/annotation_converter.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     9755 2023-04-18 09:49:07.000000 dialoguekit-0.0.9/dialoguekit/utils/annotation_converter_dialoguekit_to_rasa.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     9778 2023-04-18 09:49:07.000000 dialoguekit-0.0.9/dialoguekit/utils/dialogue_evaluation.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3482 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/dialoguekit/utils/dialogue_reader.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.689472 dialoguekit-0.0.9/dialoguekit.egg-info/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3869 2023-05-08 08:14:35.000000 dialoguekit-0.0.9/dialoguekit.egg-info/PKG-INFO
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     6967 2023-05-08 08:14:35.000000 dialoguekit-0.0.9/dialoguekit.egg-info/SOURCES.txt
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)        1 2023-05-08 08:14:35.000000 dialoguekit-0.0.9/dialoguekit.egg-info/dependency_links.txt
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)        1 2023-01-24 12:23:50.000000 dialoguekit-0.0.9/dialoguekit.egg-info/not-zip-safe
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       77 2023-05-08 08:14:35.000000 dialoguekit-0.0.9/dialoguekit.egg-info/requires.txt
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       32 2023-05-08 08:14:35.000000 dialoguekit-0.0.9/dialoguekit.egg-info/top_level.txt
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.795306 dialoguekit-0.0.9/docs/
+-rwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)      646 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/docs/Makefile
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      309 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/docs/README.md
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    10698 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/docs/components.graffle
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      898 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/docs/evaluation.md
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       73 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/docs/index.html
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.836176 dialoguekit-0.0.9/docs/source/
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.837205 dialoguekit-0.0.9/docs/source/_static/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     8167 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/docs/source/_static/favicon.png
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.847347 dialoguekit-0.0.9/docs/source/_templates/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      719 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/docs/source/_templates/layout.html
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      816 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/docs/source/_templates/versions.html
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      294 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/components.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2049 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/concepts.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3589 2023-05-05 12:20:37.000000 dialoguekit-0.0.9/docs/source/conf.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      792 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/dialogue_export.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      352 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/docs/source/docs_env.yaml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2128 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/external_agents.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      738 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/index.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      912 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/installation.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2490 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/nlg.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2983 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/nlu.rst
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      465 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/docs/source/usage.rst
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.166919 dialoguekit-0.0.9/external_agents/
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.867499 dialoguekit-0.0.9/external_agents/rasa-parrot/
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.882316 dialoguekit-0.0.9/external_agents/rasa-parrot/actions/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       47 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/actions/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1628 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/actions/actions.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1517 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/config.yml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      980 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/credentials.yml
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.891747 dialoguekit-0.0.9/external_agents/rasa-parrot/data/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      372 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/data/nlu.yml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       25 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/data/rules.yml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      169 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/data/stories.yml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      223 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/domain.yml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1409 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/external_agents/rasa-parrot/endpoints.yml
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      141 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/pyproject.toml
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.898547 dialoguekit-0.0.9/requirements/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      175 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/requirements/docs_requirements.txt
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      269 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/requirements/pre_commit.txt
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      124 2023-05-08 08:14:09.000000 dialoguekit-0.0.9/requirements/requirements.txt
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.475100 dialoguekit-0.0.9/sample_agents/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      337 2023-03-10 08:17:54.000000 dialoguekit-0.0.9/sample_agents/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4232 2023-03-10 08:18:16.000000 dialoguekit-0.0.9/sample_agents/moviebot_agent.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1819 2023-04-18 09:49:07.000000 dialoguekit-0.0.9/sample_agents/parrot_agent.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2261 2023-03-10 08:18:35.000000 dialoguekit-0.0.9/sample_agents/rasa_parrot_agent.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     3910 2023-03-10 08:18:46.000000 dialoguekit-0.0.9/sample_agents/woz_agent.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       38 2023-05-08 08:14:35.912562 dialoguekit-0.0.9/setup.cfg
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1375 2023-05-08 08:14:09.000000 dialoguekit-0.0.9/setup.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.477556 dialoguekit-0.0.9/tests/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       35 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/__init__.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.504715 dialoguekit-0.0.9/tests/core/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       41 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/core/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1203 2023-04-18 09:49:07.000000 dialoguekit-0.0.9/tests/core/test_annotated_utterance.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     7108 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/core/test_dialogue.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      504 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/core/test_domain.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)      697 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/core/test_feedback.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1300 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/core/test_intent.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1627 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/tests/core/test_slot_value_annotation.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1325 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/core/test_utterance.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.903769 dialoguekit-0.0.9/tests/data/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)    37113 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/data/annotated_dialogues.json
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.911156 dialoguekit-0.0.9/tests/data/domains/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       51 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/data/domains/movie.yaml
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.537060 dialoguekit-0.0.9/tests/nlg/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       46 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/nlg/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     5491 2023-05-02 11:59:51.000000 dialoguekit-0.0.9/tests/nlg/test_conditional_nlg.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     7649 2023-05-02 11:59:51.000000 dialoguekit-0.0.9/tests/nlg/test_template_from_training_data.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4180 2023-05-02 11:59:51.000000 dialoguekit-0.0.9/tests/nlg/test_template_nlg.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.590520 dialoguekit-0.0.9/tests/nlu/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       39 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/nlu/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2968 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/nlu/test_diet_classifier_rasa.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4136 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/nlu/test_intent_classifier_cosine.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1408 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/nlu/test_satisfaction_classifier.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.601847 dialoguekit-0.0.9/tests/sample_agents/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       49 2022-12-12 10:58:22.000000 dialoguekit-0.0.9/tests/sample_agents/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1084 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/sample_agents/test_parrot_agent.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.620028 dialoguekit-0.0.9/tests/user/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       40 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/user/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1252 2023-03-10 08:13:27.000000 dialoguekit-0.0.9/tests/user/test_user_preferences.py
+drwxr-xr-x   0 2925364  (1211013142) UIS\Domain Users (698202959)        0 2023-05-08 08:14:35.645129 dialoguekit-0.0.9/tests/utils/
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)       39 2022-11-18 08:39:36.000000 dialoguekit-0.0.9/tests/utils/__init__.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     2671 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/utils/test_annotation_converter_dialoguekit_to_rasa.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     1728 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/utils/test_dialogue_reader.py
+-rw-r--r--   0 2925364  (1211013142) UIS\Domain Users (698202959)     4245 2023-05-05 07:07:31.000000 dialoguekit-0.0.9/tests/utils/test_evaluator.py
```

### Comparing `dialoguekit-0.0.8/.github/actions/build_docs/action.yml` & `dialoguekit-0.0.9/.github/actions/build_docs/action.yml`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/.github/workflows/CI.yaml` & `dialoguekit-0.0.9/.github/workflows/CI.yaml`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/.github/workflows/build_docs.yaml` & `dialoguekit-0.0.9/.github/workflows/build_docs.yaml`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/.gitignore` & `dialoguekit-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/.pre-commit-config.yaml` & `dialoguekit-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/LICENSE` & `dialoguekit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/PKG-INFO` & `dialoguekit-0.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,105 +1,82 @@
-Metadata-Version: 2.1
-Name: dialoguekit
-Version: 0.0.8
-Summary: Toolkit for building conversational information access systems.
-Home-page: https://github.com/iai-group/dialoguekit
-Author: Jafar Afzali, Krisztian Balog, Nolwenn Bernard,         Aleksander Drzewiecki and Shuo Zhang
-Author-email: author@example.com
-Project-URL: Bug Tracker, https://github.com/iai-group/dialoguekit/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DialogueKit
 
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
-[![PyPi version](https://img.shields.io/pypi/v/dialoguekit)](https://pypi.org/project/dialoguekit/) 
-![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/adrzewiecki/35bb996459f0949b38da651c66cf95cb/raw/coverage.DialogueKit.main.json) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPi version](https://img.shields.io/pypi/v/dialoguekit)](https://pypi.org/project/dialoguekit/)
+![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/adrzewiecki/35bb996459f0949b38da651c66cf95cb/raw/coverage.DialogueKit.main.json)
 ![Tests](https://img.shields.io/github/actions/workflow/status/iai-group/DialogueKit/merge.yaml?label=Tests&branch=main)
+![docs](https://img.shields.io/github/actions/workflow/status/iai-group/DialogueKit/build_docs.yaml?label=docs&branch=main)
 ![Python version](https://img.shields.io/badge/python-3.9-blue)
 
 DialogueKit is a library for conversational information access (CIA). It contains based classes for fundamental [concepts](https://iai-group.github.io/DialogueKit/main/concepts.html), such as dialogue participants, dialogue management, [natural language understanding](https://iai-group.github.io/DialogueKit/main/nlu.html), natural language generation, etc. In addition to the fundamental concepts DialogueKit contains an evaluation module, for evaluating the performance of and CIA systems.
 Consult the [documentation](https://iai-group.github.io/DialogueKit/main/) for details.
 
 ## Install as a package
 
 DialogueKit is published to PyPI, install it by running:
 
 ```shell
 pip install dialoguekit
 ```
 
-If you want to install a DialogueKit from a specific commit or straight from github this is still possible.
+Follow the commands below to install DialogueKit from a specific commit or straight from GitHub.
 
 The command will install the latest version from the main branch.
 
-  * On Windows you may need to run this command before pip installing
+  - On Windows you may need to run this command before pip installing
 
-  ```shell
-  ssh -t git github.com    
-  ```
+```shell
+ssh -t git github.com
+```
 
-  * pip install
+  - pip install
 
-  ```shell
-  pip install git+ssh://git@github.com/iai-group/dialoguekit.git
-  ```
+```shell
+pip install git+ssh://git@github.com/iai-group/dialoguekit.git
+```
 
 If you want to specify a specific commit as the source of the package append the commit hash to the end of the command separated with a "@".
 
-  * Specific commit as the source of the package.
+  - Specific commit as the source of the package.
 
-  ```shell
-  pip install git+ssh://git@github.com/iai-group/dialoguekit.git@faa5c1fca37aaa275105cc1ca7698783719551c2
-  ```
+```shell
+pip install git+ssh://git@github.com/iai-group/dialoguekit.git@faa5c1fca37aaa275105cc1ca7698783719551c2
+```
 
 ## Usage example
 
-1. Define agent and user
+1. Create and connect a platform that manages dialogues. The platform requires information about the agent it serves.
 
-    ```python
-    from dialoguekit.core.utterance import Utterance
-    from dialoguekit.participant.user import User, UserType
-    from sample_agents.parrot_agent import ParrotAgent
+   ```python
+   from dialoguekit.platforms.terminal_platform import TerminalPlatform
+   from sample_agents.parrot_agent import ParrotAgent
 
-    # Participants
-    agent = ParrotAgent("A01")
-    user = User("U01")
-    ```
+   platform = TerminalPlatform(ParrotAgent)
+   ```
 
-2. Create and connect platform and dialogue manager
+2. Start conversation
 
-    ```python
-    from dialoguekit.platforms.platform import Platform
-    from dialoguekit.manager.dialogue_manager import DialogueManager
-
-    platform = Platform()
-    dm = DialogueManager(agent, user, platform)
-
-    user.connect_dialogue_manager(dm)
-    agent.connect_dialogue_manager(dm)
-    ```
-
-3. Start conversation
-
-    ```python
-      dm.start()
-      dm.close()
-    ```
+   ```python
+      platform.start()
+   ```
 
 ## Conventions
 
-We follow the [IAI Python Style Guide](https://github.com/iai-group/styleguide/tree/main/python).
+We follow the [IAI Python Style Guide](https://github.com/iai-group/styleguide/tree/main/python).  
+We use `UTF-8` encodings that is widely used on Unix systems. Windows users need to use the `Python UTF-8 Mode`; see [here](https://docs.python.org/3/using/windows.html#utf-8-mode) for more details. In practice, we specify the encoding when opening files, as in this example:
+
+```python
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+```
 
 ## Contributors
 
-(Alphabetically ordered by last name) 
+(Alphabetically ordered by last name)
 
-  * Jafar Afzali (2022)
-  * Krisztian Balog (2021-present)
-  * Nolwenn Bernard (2022-present)
-  * Aleksander Drzewiecki (2022)
-  * Shuo Zhang (2021)
+  - Jafar Afzali (2022)
+  - Krisztian Balog (2021-present)
+  - Nolwenn Bernard (2022-present)
+  - Aleksander Drzewiecki (2022)
+  - Ivica Kostric (2023)
+  - Weronika Lajewska (2023)
+  - Shuo Zhang (2021)
```

### Comparing `dialoguekit-0.0.8/dialoguekit/connector/dialogue_connector.py` & `dialoguekit-0.0.9/dialoguekit/connector/dialogue_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,55 +9,66 @@
 `receive_utterance()` methods.
 It is left to to specific Agent and User instances when and how they respond.
 It is expected that most will respond immediately upon receiving an utterance,
 but this is not required.  Whenever there is a message from either the Agent or
 the User, the DialogueConnector sends it to the other party by calling their
 `receive_{agent/user}_utterance()` method.
 """
+from __future__ import annotations
+
 import json
 import os
+from typing import TYPE_CHECKING
 
 from dialoguekit.core.annotated_utterance import AnnotatedUtterance
 from dialoguekit.core.dialogue import Dialogue
 from dialoguekit.participant.agent import Agent
 from dialoguekit.participant.user import User
-from dialoguekit.platforms.platform import Platform
+
+if TYPE_CHECKING:
+    from dialoguekit.platforms.platform import Platform
 
 _DIALOGUE_EXPORT_PATH = "dialogue_export"
 
 
 class DialogueConnector:
     def __init__(
         self,
         agent: Agent,
         user: User,
         platform: Platform,
+        conversation_id: str = None,
         save_dialogue_history: bool = True,
     ) -> None:
         """Represents a dialogue connector.
 
         Args:
             agent: An instance of Agent.
             user: An instance of User.
             platform: An instance of Platform.
+            conversation_id: Conversation ID. Defaults to None.
             save_dialogue_history: Flag to save the dialogue or not.
         """
+        self._platform = platform
         self._agent = agent
         self._agent.connect_dialogue_connector(self)
         self._user = user
         self._user.connect_dialogue_connector(self)
-        self._platform = platform
-        self._dialogue_history = Dialogue(agent.id, user.id)
+        self._dialogue_history = Dialogue(agent.id, user.id, conversation_id)
         self._save_dialogue_history = save_dialogue_history
 
     @property
     def dialogue_history(self):
         """Return the dialogue history."""
         return self._dialogue_history
 
+    def get_platform(self) -> Platform:
+        """Returns the platform."""
+        return self._platform
+
     def register_user_utterance(
         self, annotated_utterance: AnnotatedUtterance
     ) -> None:
         """Registers an annotated utterance from the user.
 
         In most cases the Agent should not know about the Users Intent and
         Annotation-s. But for some use cases this additional information may
@@ -66,15 +77,17 @@
         the Agents responsibility to only use the information it is supposed
         to.
 
         Args:
             annotated_utterance: User utterance.
         """
         self._dialogue_history.add_utterance(annotated_utterance)
-        self._platform.display_user_utterance(annotated_utterance)
+        self._platform.display_user_utterance(
+            self._user.id, annotated_utterance
+        )
         self._agent.receive_utterance(annotated_utterance)
 
     def register_agent_utterance(
         self, annotated_utterance: AnnotatedUtterance
     ) -> None:
         """Registers an annotated utterance from the agent.
 
@@ -88,15 +101,17 @@
             If the Intent label is 'EXIT' the DialogueConnector will close. Thus
             it is only the agent that can close the DialogueConnector.
 
         Args:
             annotated_utterance: Agent utterance.
         """
         self._dialogue_history.add_utterance(annotated_utterance)
-        self._platform.display_agent_utterance(annotated_utterance)
+        self._platform.display_agent_utterance(
+            self._user.id, annotated_utterance
+        )
         # TODO: Replace with appropriate intent (make sure all intent schemes
         # have an EXIT intent.)
         if annotated_utterance.intent == self._agent.stop_intent:
             self.close()
         else:
             self._user.receive_utterance(annotated_utterance)
 
@@ -136,43 +151,23 @@
         )
         json_file = []
 
         # Check directory and read if exists.
         if not os.path.exists(_DIALOGUE_EXPORT_PATH):
             os.makedirs(_DIALOGUE_EXPORT_PATH)
         if os.path.exists(file_name):
-            with open(file_name) as json_file_out:
+            with open(file_name, encoding="utf-8") as json_file_out:
                 json_file = json.load(json_file_out)
 
         dialogue_as_dict = history.to_dict()
         dialogue_as_dict["agent"] = self._agent.to_dict()
         dialogue_as_dict["user"] = self._user.to_dict()
 
         json_file.append(dialogue_as_dict)
 
-        with open(file_name, "w") as outfile:
+        with open(file_name, "w", encoding="utf-8") as outfile:
             json.dump(json_file, outfile)
 
         # Empty dialogue history to avoid duplicate save
         for _ in range(len(self._dialogue_history.utterances)):
             self._dialogue_history.utterances.pop()
         # TODO: save dialogue history, subject to config parameters
-
-
-if __name__ == "__main__":
-    from dialoguekit.participant.user import User
-    from sample_agents.moviebot_agent import MovieBotAgent
-
-    # Participants
-    agent = MovieBotAgent(
-        agent_id="MovieBot01", uri="http://152.94.232.43:5001/"
-    )
-    user = User(id="TEST01")
-
-    platform = Platform()
-    dm = DialogueConnector(agent, user, platform)
-
-    user.connect_dialogue_connector(dm)
-    agent.connect_dialogue_connector(dm)
-    dm.start()
-
-    dm.close()
```

### Comparing `dialoguekit-0.0.8/dialoguekit/core/__init__.py` & `dialoguekit-0.0.9/dialoguekit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/core/intent.py` & `dialoguekit-0.0.9/dialoguekit/core/intent.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/core/utterance.py` & `dialoguekit-0.0.9/sample_agents/rasa_parrot_agent.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,67 @@
-"""Interface representing the basic unit of communication."""
+"""Simplest possible agent that parrots back everything the user says.
 
-from datetime import datetime
-from typing import Optional, Text
+This agent depends on Rasa parrot project to parrot back. See
+'docs/rasa-parrot.md' for more information
+"""
 
+import requests
+
+from dialoguekit.core.annotated_utterance import AnnotatedUtterance
+from dialoguekit.core.utterance import Utterance
+from dialoguekit.participant.agent import Agent
 from dialoguekit.participant.participant import DialogueParticipant
 
 
-class Utterance:
-    def __init__(
-        self,
-        text: str,
-        participant: DialogueParticipant,
-        timestamp: Optional[datetime] = None,
-    ) -> None:
-        """Represents an utterance.
+class RasaParrotAgent(Agent):
+    def __init__(self, agent_id: str):
+        """Rasa Parrot agent.
+
+        This agent connects to the sample Rasa parrot agent found here:
+        https://github.com/iai-group/dialoguekit/tree/main/external_agents
+
+        To end the conversation the user has to say `EXIT`, `QUIT` or `STOP`.
 
         Args:
-            text: Utterance text.
-            participant: Who said the utterance.
-            timestamp: When was the utterance uttered.
+            agent_id: Agent id.
         """
-        self._text = text
-        self._participant = participant
-        self._timestamp = timestamp
-
-    def __str__(self) -> Text:
-        """Returns the utterance text."""
-        return self._text
-
-    def __repr__(self) -> Text:
-        """Represents the utterance as a string."""
-        if self._timestamp:
-            time = self._timestamp.strftime("%m/%d/%Y, %H:%M:%S")
-            return f"Utterance({self._text}, {self._participant.value}, {time})"
-        return f"Utterance({self._text}, {self._participant.value})"
-
-    def __hash__(self) -> int:
-        """Represents the utterance as a hash."""
-        return hash(f"{self._text}{self._participant}{self._timestamp_text()}")
-
-    def __eq__(self, __o: object) -> bool:
-        """Comparison function."""
-        if not isinstance(__o, Utterance):
-            return False
-        if self._text != __o._text:
-            return False
-        if self._timestamp != __o._timestamp:
-            return False
-        if self._participant != __o._participant:
-            return False
-        return True
-
-    @property
-    def text(self) -> str:
-        """Returns the utterance text."""
-        return self._text
-
-    @property
-    def participant(self) -> DialogueParticipant:
-        """Returns the utterance participant."""
-        return self._participant
-
-    @property
-    def timestamp(self) -> datetime:
-        """Returns the utterance timestamp."""
-        return self._timestamp
+        super().__init__(agent_id)
+        self._RASA_URI = "http://localhost:5002/webhooks/rest/webhook"
 
-    def _timestamp_text(self) -> str:
-        """Returns the timestamp as a string.
+    def welcome(self) -> None:
+        """Sends the agent's welcome message."""
+        utterance = AnnotatedUtterance(
+            "Hello, I'm Rasa Parrot. What can I help u with?",
+            participant=DialogueParticipant.AGENT,
+        )
+        self._dialogue_connector.register_agent_utterance(utterance)
+
+    def goodbye(self) -> None:
+        """Sends the agent's goodbye message."""
+        utterance = AnnotatedUtterance(
+            "It was nice talking to you. Bye",
+            intent=self.stop_intent,
+            participant=DialogueParticipant.AGENT,
+        )
+        self._dialogue_connector.register_agent_utterance(utterance)
 
-        If no timestamp, this method will return an empty string.
+    def receive_utterance(self, utterance: Utterance) -> None:
+        """Gets called each time there is a new user utterance.
 
-        Returns:
-            Timestamp with the format: `%m/%d/%Y, %H:%M:%S`.
+        Args:
+            utterance: User utterance.
         """
-        if self._timestamp:
-            return self._timestamp.strftime("%m/%d/%Y, %H:%M:%S")
-        return ""
+        if utterance.text.lower() in ["quit", "stop", "exit"]:
+            return
+
+        r = requests.post(
+            self._RASA_URI,
+            json={
+                "sender": "RasaParrotAgent",
+                "message": "(Rasa Parroting) " + utterance.text,
+            },
+        )
+        response = AnnotatedUtterance(
+            r.json()[0]["text"],
+            participant=DialogueParticipant.AGENT,
+        )
+        self._dialogue_connector.register_agent_utterance(response)
```

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/models/LinearSVC_2_0.joblib` & `dialoguekit-0.0.9/dialoguekit/nlg/models/LinearSVC_2_0.joblib`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/models/vectorizer_0_0.joblib` & `dialoguekit-0.0.9/dialoguekit/nlg/models/vectorizer_0_0.joblib`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/models/vectorizer_2_0.joblib` & `dialoguekit-0.0.9/dialoguekit/nlg/models/vectorizer_2_0.joblib`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/models/xgb_0_0.json` & `dialoguekit-0.0.9/dialoguekit/nlg/models/xgb_0_0.json`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/nlg_abstract.py` & `dialoguekit-0.0.9/dialoguekit/nlg/nlg_abstract.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/nlg_conditional.py` & `dialoguekit-0.0.9/dialoguekit/nlg/nlg_conditional.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,22 +155,22 @@
                 conditional_value=conditional_value,
             )
         else:
             response_utterance = random.choice(templates)
             response_utterance = deepcopy(response_utterance)
 
         # Clear out annotations
-        response_utterance._annotations = []
+        response_utterance.annotations = []
 
         if annotations is not None:
             for annotation in annotations:
-                response_utterance._text = response_utterance._text.replace(
+                response_utterance.text = response_utterance.text.replace(
                     f"{{{annotation.slot}}}", annotation.value, 1
                 )
-                response_utterance.add_annotation(annotation)
+            response_utterance.add_annotations(annotations)
         return response_utterance
 
     def _select_closest_to_conditional(
         self,
         templates: List[AnnotatedUtterance],
         conditional: str,
         conditional_value: Number,
```

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/nlg_template.py` & `dialoguekit-0.0.9/dialoguekit/nlg/nlg_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,33 +97,33 @@
         if len(templates) == 0:
             raise ValueError("NLG text generation failed.")
 
         response_utterance = random.choice(templates)
         response_utterance = deepcopy(response_utterance)
 
         # Clear out annotations
-        response_utterance._annotations = []
+        response_utterance.annotations = []
 
         if annotations is not None:
             for annotation in annotations:
-                response_utterance._text = response_utterance._text.replace(
+                response_utterance.text = response_utterance.text.replace(
                     f"{{{annotation.slot}}}", annotation.value, 1
                 )
-                response_utterance.add_annotation(annotation)
+            response_utterance.add_annotations(annotations)
         return response_utterance
 
     def dump_template(self, filepath: str) -> None:
         """Dump template to JSON."""
         dump_dict = {}
         for intent, utterances in self._response_templates.items():
             dump_dict[intent.label] = [
                 annotated_utterance.text for annotated_utterance in utterances
             ]
 
-        with open(filepath, "w") as file:
+        with open(filepath, "w", encoding="utf-8") as file:
             json.dump(dump_dict, file, indent=4)
 
     def _filter_templates(
         self,
         templates: List[AnnotatedUtterance],
         annotations: List[Annotation],
         force_annotation: bool,
@@ -150,24 +150,24 @@
         """
         filtered_annotated_utterances = []
         annotations_slots = set([annotation.slot for annotation in annotations])
         for annotated_utterance in templates:
             utterance_slots = set(
                 [
                     annotation.slot
-                    for annotation in annotated_utterance.get_annotations()
+                    for annotation in annotated_utterance.annotations
                 ]
             )
             if all(x in annotations_slots for x in utterance_slots):
                 filtered_annotated_utterances.append(annotated_utterance)
         if force_annotation and len(annotations) > 0:
             filtered_annotated_utterances = [
                 template
                 for template in filtered_annotated_utterances
-                if len(template.get_annotations()) > 0
+                if len(template.annotations) > 0
             ]
         return filtered_annotated_utterances
 
     def get_intent_annotation_specifications(
         self,
         intent: Intent,
     ) -> Dict[str, Dict[str, Any]]:
@@ -200,17 +200,15 @@
         templates = self._response_templates.get(intent)
         if templates is None:
             raise TypeError(f"Intent: {intent}, is not part of the template")
 
         min_annotations = {"amount": sys.maxsize, "examples": []}
         max_annotations = {"amount": 0, "examples": []}
 
-        template_lengths = [
-            len(template.get_annotations()) for template in templates
-        ]
+        template_lengths = [len(template.annotations) for template in templates]
         max_annotations["amount"] = max(template_lengths)
         min_annotations["amount"] = min(template_lengths)
         max_annotations["examples"] = [
             templates[i]
             for i, _ in enumerate(template_lengths)
             if template_lengths[i] == max_annotations["amount"]
         ]
```

### Comparing `dialoguekit-0.0.8/dialoguekit/nlg/template_from_training_data.py` & `dialoguekit-0.0.9/dialoguekit/nlg/template_from_training_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,33 @@
 from dialoguekit.core.annotated_utterance import AnnotatedUtterance
 from dialoguekit.core.annotation import Annotation
 from dialoguekit.core.intent import Intent
 from dialoguekit.nlu.models.satisfaction_classifier import (
     SatisfactionClassifier,
 )
 from dialoguekit.participant.participant import DialogueParticipant
+from dialoguekit.utils.dialogue_reader import (
+    _FIELD_CONVERSATION,
+    _FIELD_INTENT,
+    _FIELD_PARTICIPANT,
+    _FIELD_SLOT_VALUES,
+    _FIELD_UTTERANCE,
+)
 
 # The default satisfaction level used for classifying the NLG template.
 _DEFAULT_SATISFACTION = 3
 
 
 def _replace_slot_with_placeholder(
     annotated_utterance: AnnotatedUtterance,
 ) -> None:
-    annotations = annotated_utterance.get_annotations()
+    annotations = annotated_utterance.annotations
     for annotation in annotations:
         placeholder_label, value = annotation.slot, annotation.value
-        annotated_utterance._text = annotated_utterance.text.replace(
+        annotated_utterance.text = annotated_utterance.text.replace(
             value, f"{{{placeholder_label}}}", 1
         )
         annotation.value = None
 
 
 def build_template_from_instances(
     utterances: List[AnnotatedUtterance],
@@ -92,59 +99,61 @@
     if not os.path.isfile(annotated_dialogue_file):
         raise FileNotFoundError(
             f"Annotated dialog file not found: {annotated_dialogue_file}"
         )
     response_templates: DefaultDict[
         Intent, Set[AnnotatedUtterance]
     ] = defaultdict(set)
-    with open(annotated_dialogue_file) as input_file:
+    with open(annotated_dialogue_file, encoding="utf-8") as input_file:
         annotated_dialogs = json.load(input_file)
         for dialog in annotated_dialogs:
             counter_participant_utterance = None
             participant_utterance = None
             satisfaction = None
-            for utterance_record in dialog.get("conversation"):
-                participant = utterance_record.get("participant")
+            for utterance_record in dialog.get(_FIELD_CONVERSATION):
+                participant = utterance_record.get(_FIELD_PARTICIPANT)
 
                 if satisfaction_classifier:
                     annotated_utterance = AnnotatedUtterance(
-                        text=utterance_record.get("utterance").strip(),
-                        intent=Intent(utterance_record.get("intent")),
+                        text=utterance_record.get(_FIELD_UTTERANCE).strip(),
+                        intent=Intent(utterance_record.get(_FIELD_INTENT)),
                         metadata={
                             "satisfaction": _DEFAULT_SATISFACTION
                         },  # Satisfaction defaults to 3 (Normal)
                         participant=DialogueParticipant.AGENT,
                     )
                 else:
                     annotated_utterance = AnnotatedUtterance(
-                        text=utterance_record.get("utterance").strip(),
-                        intent=Intent(utterance_record.get("intent")),
+                        text=utterance_record.get(_FIELD_UTTERANCE).strip(),
+                        intent=Intent(utterance_record.get(_FIELD_INTENT)),
                         participant=DialogueParticipant.AGENT,
                     )
                 annotated_utterance_copy = copy.deepcopy(annotated_utterance)
 
                 # Only use the utterances from the wanted participant
                 if participant == participant_to_learn:
                     if (
                         counter_participant_utterance
                         and participant_utterance
                         and satisfaction_classifier
                     ):
-                        annotated_utterance._metadata[
+                        annotated_utterance.metadata[
                             "satisfaction"
                         ] = satisfaction
                         counter_participant_utterance = None
                         participant_utterance = None
 
                     # Keep the original utterance as template when it does not
                     # contain slot values.
                     if "slot_values" in utterance_record:
-                        for slot, value in utterance_record.get("slot_values"):
-                            annotated_utterance.add_annotation(
-                                Annotation(slot=slot, value=value)
+                        for slot, value in utterance_record.get(
+                            _FIELD_SLOT_VALUES
+                        ):
+                            annotated_utterance.add_annotations(
+                                [Annotation(slot=slot, value=value)]
                             )
                         if satisfaction_classifier:
                             annotated_utterance_copy = copy.deepcopy(
                                 annotated_utterance
                             )
 
                         _replace_slot_with_placeholder(annotated_utterance)
```

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/__init__.py` & `dialoguekit-0.0.9/dialoguekit/nlu/__init__.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/intent_classifier.py` & `dialoguekit-0.0.9/dialoguekit/nlu/intent_classifier.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/models/diet_classifier_rasa.py` & `dialoguekit-0.0.9/dialoguekit/nlu/models/diet_classifier_rasa.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,20 +27,21 @@
 from rasa.shared.nlu.training_data.message import Message
 from rasa.shared.nlu.training_data.training_data import TrainingData
 
 from dialoguekit.core.intent import Intent
 from dialoguekit.core.slot_value_annotation import SlotValueAnnotation
 from dialoguekit.core.utterance import Utterance
 from dialoguekit.nlu.intent_classifier import IntentClassifier
+from dialoguekit.nlu.slot_annotator import SlotAnnotator
 from dialoguekit.utils.annotation_converter_dialoguekit_to_rasa import (
     AnnotationConverterRasa,
 )
 
 
-class IntentClassifierRasa(IntentClassifier):
+class IntentClassifierRasa(IntentClassifier, SlotAnnotator):
     def __init__(
         self,
         intents: List[Intent],
         training_data_path: Optional[str] = "",
         model_path: Optional[str] = ".rasa",
     ) -> None:
         """Initializes the intent classifier.
```

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/models/intent_classifier_cosine.py` & `dialoguekit-0.0.9/dialoguekit/nlu/models/intent_classifier_cosine.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/LinearSVC_2_0.joblib` & `dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/LinearSVC_2_0.joblib`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/vectorizer_0_0.joblib` & `dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/vectorizer_0_0.joblib`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/vectorizer_2_0.joblib` & `dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/vectorizer_2_0.joblib`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction/xgb_0_0.json` & `dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction/xgb_0_0.json`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/nlu/models/satisfaction_classifier.py` & `dialoguekit-0.0.9/dialoguekit/nlu/models/satisfaction_classifier.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/participant/agent.py` & `dialoguekit-0.0.9/dialoguekit/participant/agent.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/participant/participant.py` & `dialoguekit-0.0.9/dialoguekit/participant/participant.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import TYPE_CHECKING, Dict
 
 if TYPE_CHECKING:
     from dialoguekit.connector.dialogue_connector import DialogueConnector
-    from dialoguekit.core.utterance import Utterance
+    from dialoguekit.core import Utterance
 
 
 class DialogueParticipant(Enum):
     """Represents possible dialogue participants."""
 
     AGENT = 0
     USER = 1
@@ -32,14 +32,23 @@
         self._dialogue_connector: DialogueConnector = None
 
     @property
     def id(self):
         """Returns the participant id."""
         return self._id
 
+    @property
+    def dialogue_connector(self) -> DialogueConnector:
+        """Returns the DialogueConnector instance for the participant.
+
+        Returns:
+            A DialogueConnector instance.
+        """
+        return self._dialogue_connector
+
     def to_dict(self) -> Dict[str, str]:
         """Returns participant as a dictionary.
 
         Returns:
             A dictionary representation of the participant.
         """
         return {"id": str(self._id), "type": str(self._type.name)}
```

### Comparing `dialoguekit-0.0.8/dialoguekit/participant/user.py` & `dialoguekit-0.0.9/dialoguekit/participant/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Abstract representation of core user-related data and functionality.
 
 For communicating with an agent, the specific user instance needs to be
 connected with a DialogueConnector by invoking
 `register_dialogue_connector()`.
 """
-
 from __future__ import annotations
 
 from enum import Enum
+from typing import TYPE_CHECKING
 
 from dialoguekit.core.annotated_utterance import AnnotatedUtterance
-from dialoguekit.core.utterance import Utterance
 from dialoguekit.participant.participant import DialogueParticipant, Participant
 
+if TYPE_CHECKING:
+    from dialoguekit.core.utterance import Utterance
+
 
 class UserType(Enum):
     """Represents different types of users (humans vs simulated users)."""
 
     HUMAN = 0
     SIMULATOR = 1
 
@@ -27,20 +29,34 @@
 
         Args:
             id: User ID.
             user_type: User type (default: HUMAN).
         """
         super().__init__(id=id, type=DialogueParticipant.USER)
         self._user_type = user_type
+        self._ready_for_input = False
+
+    @property
+    def ready_for_input(self) -> bool:
+        """Returns whether the user is ready to listen for input."""
+        return self._ready_for_input
+
+    def handle_input(self, text: str) -> None:
+        """Gets called every time there is a new user input.
+
+        Args:
+            text: User input.
+        """
+        if self._ready_for_input:
+            self._ready_for_input = False
+            utterance = AnnotatedUtterance(
+                text, participant=DialogueParticipant.USER
+            )
+            self._dialogue_connector.register_user_utterance(utterance)
 
     def receive_utterance(self, utterance: Utterance) -> None:
         """Gets called every time there is a new agent utterance.
 
         Args:
             utterance: Agent utterance.
         """
-        # TODO: Move input part to Platform.
-        text = input("Your response: ")
-        response = AnnotatedUtterance(
-            text, participant=DialogueParticipant.USER
-        )
-        self._dialogue_connector.register_user_utterance(response)
+        self._ready_for_input = True
```

### Comparing `dialoguekit-0.0.8/dialoguekit/participant/user_preferences.py` & `dialoguekit-0.0.9/dialoguekit/participant/user_preferences.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/utils/annotation_converter.py` & `dialoguekit-0.0.9/dialoguekit/utils/annotation_converter.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/dialoguekit/utils/annotation_converter_dialoguekit_to_rasa.py` & `dialoguekit-0.0.9/dialoguekit/utils/annotation_converter_dialoguekit_to_rasa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Convert annotations to be compatible with the rasa models."""
 import json
 import time
 from collections import defaultdict
 from typing import Any, Callable, Dict, List, Optional
 
 import yaml
+from yaml.representer import SafeRepresenter
+
 from dialoguekit.core.intent import Intent
 from dialoguekit.core.utterance import Utterance
 from dialoguekit.utils.annotation_converter import AnnotationConverter
-from yaml.representer import SafeRepresenter
 
 
 # Used for yaml formatting
 class LiteralString(str):
     pass
 
 
@@ -87,15 +88,15 @@
         """
         utterance_text = utterance_text.strip()
         utterance_text = utterance_text.replace("\n", " ")
         return utterance_text
 
     def read_original(self) -> None:
         """Reads the original training data."""
-        f = open(self._filepath)
+        f = open(self._filepath, encoding="utf-8")
         data = json.load(f)
         self._data["original"] = data
 
         for conversation in data:
             for turn in conversation["conversation"]:
                 intent = turn.get("intent", None)
                 slot_values = turn.get("slot_values", [])
@@ -173,22 +174,26 @@
         )
         save_name_base = self._filepath.split("/")[-1].split(".")[-2]
 
         # Save original as yaml
         extension = "_reformat.yaml"
         filename = save_name_base + extension
         return_dictionary[filename] = save_path_name + extension
-        with open(return_dictionary[filename], "w") as outfile:
+        with open(
+            return_dictionary[filename], "w", encoding="utf-8"
+        ) as outfile:
             yaml.dump(self._data["original"], outfile, default_flow_style=False)
 
         # Save the intent types with examples
         extension = "_types_w_examples.yaml"
         filename = save_name_base + extension
         return_dictionary[filename] = save_path_name + extension
-        with open(return_dictionary[filename], "w") as outfile:
+        with open(
+            return_dictionary[filename], "w", encoding="utf-8"
+        ) as outfile:
             yaml.dump(self._slot_value_pairs, outfile, default_flow_style=False)
 
         represent_literal_list = self.change_style(
             "|", SafeRepresenter.represent_str
         )
         yaml.add_representer(LiteralString, represent_literal_list)
 
@@ -203,21 +208,25 @@
             formatted_dict = {"intent": k, "examples": self.rasa_string(v)}
             rasa_dict_agent["nlu"].append(formatted_dict)
 
         # Save rasa compatible format
         extension = "_rasa_user.yaml"
         filename = save_name_base + extension
         return_dictionary[filename] = save_path_name + extension
-        with open(return_dictionary[filename], "w") as outfile:
+        with open(
+            return_dictionary[filename], "w", encoding="utf-8"
+        ) as outfile:
             yaml.dump(rasa_dict_user, outfile, default_flow_style=False)
 
         extension = "_rasa_agent.yaml"
         filename = save_name_base + extension
         return_dictionary[filename] = save_path_name + extension
-        with open(return_dictionary[filename], "w") as outfile:
+        with open(
+            return_dictionary[filename], "w", encoding="utf-8"
+        ) as outfile:
             yaml.dump(rasa_dict_agent, outfile, default_flow_style=False)
 
         return return_dictionary
 
     def dialoguekit_to_rasa(
         self, utterances: List[Utterance], intents: List[Intent]
     ) -> str:
@@ -242,15 +251,15 @@
             "|", SafeRepresenter.represent_str
         )
         yaml.add_representer(LiteralString, represent_literal_list)
         # Save rasa compatible format
         filepath = (
             self._save_to_path + "_" + str(int(time.time())) + "_rasa.yaml"
         )
-        with open(filepath, "w") as outfile:
+        with open(filepath, "w", encoding="utf-8") as outfile:
             yaml.dump(rasa_dict, outfile, default_flow_style=False)
 
         return filepath
 
 
 if __name__ == "__main__":
     converter = AnnotationConverterRasa(
```

### Comparing `dialoguekit-0.0.8/dialoguekit/utils/dialogue_evaluation.py` & `dialoguekit-0.0.9/dialoguekit/utils/dialogue_evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,61 +109,69 @@
 
     def reward(self) -> Dict[str, List[Dict[str, float]]]:
         """Computes reward for the dialogues, according to the reward config.
 
         Reward is used to penalize agents that do not support a set of intents
         defined in the config file, and long dialogues.
 
+        Raises:
+            TypeError: if utterances are not annotated.
+
         Returns:
             A dictionary with following structure (most important is "reward"):
 
             .. code:: python
 
                 {
                     "missing_intents": [],
                     "dialogues": [{
                         "reward": int,
                         "user_turns": int,
                         "repeats": int,
                     }]
                 }
         """
-        warnings.warn("This function does not yet penalize 'Repeat' actions")
+        warnings.warn("This function does not yet penalize 'Repeat' actions.")
+
+        if not all(
+            isinstance(utterance, AnnotatedUtterance)
+            for dialogue in self._dialogues
+            for utterance in dialogue.utterances
+        ):
+            raise TypeError(
+                "Some utterances are not instance of 'AnnotatedUtterance'."
+            )
 
         # Initialize result by checking which intents are included
         results = self._check_included_intents()
 
         # Check for Repeats
         for i, dialogue in enumerate(self._dialogues):
-
             previous_intent = None
             previous_sender = None
             n_repeat_intents = 0
 
             # Start dialogue with Agent first.
             for j, utterance in enumerate(dialogue.utterances):
                 if utterance.participant == DialogueParticipant.AGENT.name:
-                    dialogue_utterances_start_agent = [
-                        AnnotatedUtterance.from_utterance(u)
-                        for u in dialogue.utterances[j:]
-                    ]
+                    dialogue_utterances_start_agent = dialogue.utterances[j:]
                     break
             previous_sender = dialogue_utterances_start_agent[0].participant
-            previous_intent = dialogue_utterances_start_agent[0].intent
+            previous_intent = dialogue_utterances_start_agent[0].intent  # type: ignore[attr-defined] # noqa
             for j, annotated_utterance in enumerate(
                 dialogue_utterances_start_agent, start=1
             ):
                 if (
                     annotated_utterance.participant == previous_sender
-                    and previous_intent == annotated_utterance.intent
+                    and previous_intent == annotated_utterance.intent  # type: ignore[attr-defined] # noqa
                 ):
                     n_repeat_intents += 1
                     previous_intent = None
                     continue
-                previous_intent = annotated_utterance.intent
+                previous_intent = annotated_utterance.intent  # type: ignore[attr-defined]  # noqa
                 previous_sender = annotated_utterance.participant
 
             results["dialogues"][i]["repeats"] = n_repeat_intents
             results["dialogues"][i]["reward"] -= n_repeat_intents
 
         # * Calculate USER/AGENT ratios.
         results = self._user_agent_ratio(results=results)
@@ -193,22 +201,19 @@
             ],
         }
 
         dialogue_intents = []
         reward = self._reward_config["full_set_points"]
         for dialogue in self._dialogues:
             for utterance in dialogue.utterances:
-                if (
-                    isinstance(utterance, AnnotatedUtterance)
-                    and utterance.participant == DialogueParticipant.USER.name
-                ):
+                if utterance.participant == DialogueParticipant.USER.name:
                     dialogue_intents.append(
-                        Intent(utterance.intent.label.split(".")[0])
+                        Intent(utterance.intent.label.split(".")[0])  # type: ignore[attr-defined]  # noqa
                     )
-                    dialogue_intents.append(utterance.intent)
+                    dialogue_intents.append(utterance.intent)  # type: ignore[attr-defined] # noqa
 
         dialogue_intents_set = set(dialogue_intents)
 
         for intent_str, penalty in self._reward_config.get("intents").items():
             if Intent(intent_str) not in dialogue_intents_set:
                 reward -= penalty
                 results["missing_intents"].append(Intent(intent_str))
```

### Comparing `dialoguekit-0.0.8/dialoguekit/utils/dialogue_reader.py` & `dialoguekit-0.0.9/dialoguekit/utils/dialogue_reader.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 
 from dialoguekit.core.annotated_utterance import AnnotatedUtterance
 from dialoguekit.core.annotation import Annotation
 from dialoguekit.core.dialogue import Dialogue
 from dialoguekit.core.intent import Intent
 
 _FIELD_UTTERANCE = "utterance"
+_FIELD_UTTERANCE_ID = "utterance_id"
 _FIELD_INTENT = "intent"
 _FIELD_SLOT_VALUES = "slot_values"
 _FIELD_CONVERSATION = "conversation"
+_FIELD_CONVERSATION_ID = "conversation_id"
 _FIELD_PARTICIPANT = "participant"
+_FIELD_AGENT = "agent"
+_FIELD_USER = "user"
 
 
 def json_to_annotated_utterance(
     json_utterance: Dict[Any, Any]
 ) -> AnnotatedUtterance:
     """Converts an utterance from JSON format to AnnotatedUtterance.
 
@@ -33,14 +37,15 @@
 
     Returns:
         An AnnotatedUtterance object representation of the json utterance.
     """
     participant = json_utterance.get(_FIELD_PARTICIPANT)
 
     utterance_text = json_utterance.get(_FIELD_UTTERANCE)
+    utterance_id = json_utterance.get(_FIELD_UTTERANCE_ID)
 
     intent = json_utterance.get(_FIELD_INTENT)
     if intent:
         intent = Intent(intent)
 
     annotations = json_utterance.get(_FIELD_SLOT_VALUES)
     if annotations:
@@ -57,39 +62,53 @@
                 _FIELD_INTENT,
             ]
         ):
             metadata[k] = v
 
     return AnnotatedUtterance(
         text=utterance_text,
+        utterance_id=utterance_id,
         participant=participant,
         annotations=annotations,
         intent=intent,
         metadata=metadata,
     )
 
 
 def json_to_dialogues(
-    filepath: str, agent_id: str, user_id: str
+    filepath: str,
+    agent_ids: List[str] = None,
+    user_ids: List[str] = None,
 ) -> List[Dialogue]:
     """Parses a JSON file containing dialogues.
 
     Args:
         filepath: Path to JSON file containing the dialogues.
-        agent_id: Agent ID in the dialogues.
-        user_id: User ID in the dialogues.
+        agent_ids: List of agents' id to filter loaded dialogues. Defaults to
+          None.
+        user_ids: List of users' id to filter loaded dialogues. Defaults to
+          None.
 
     Returns:
         A list of Dialogue objects.
     """
-    f = open(filepath)
+    f = open(filepath, encoding="utf-8")
     data = json.load(f)
 
     dialogues = []
     for dialogue_data in data:
-        dialogue = Dialogue(agent_id, user_id)
+        conversation_id = dialogue_data.get(_FIELD_CONVERSATION_ID, None)
+        agent_id = dialogue_data.get(_FIELD_AGENT, {}).get("id", "Agent")
+        user_id = dialogue_data.get(_FIELD_USER, {}).get("id", "User")
+        if (agent_ids and agent_id not in agent_ids) or (
+            user_ids and user_id not in user_ids
+        ):
+            # Filter loaded dialogues based on agent_ids and/or user_ids if
+            # provided
+            continue
+        dialogue = Dialogue(agent_id, user_id, conversation_id)
         for utterance_data in dialogue_data.get(_FIELD_CONVERSATION):
             annotated_utterance = json_to_annotated_utterance(utterance_data)
             dialogue.add_utterance(annotated_utterance)
         dialogues.append(dialogue)
 
     return dialogues
```

### Comparing `dialoguekit-0.0.8/dialoguekit.egg-info/PKG-INFO` & `dialoguekit-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,97 @@
 Metadata-Version: 2.1
 Name: dialoguekit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Toolkit for building conversational information access systems.
 Home-page: https://github.com/iai-group/dialoguekit
 Author: Jafar Afzali, Krisztian Balog, Nolwenn Bernard,         Aleksander Drzewiecki and Shuo Zhang
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/iai-group/dialoguekit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DialogueKit
 
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
-[![PyPi version](https://img.shields.io/pypi/v/dialoguekit)](https://pypi.org/project/dialoguekit/) 
-![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/adrzewiecki/35bb996459f0949b38da651c66cf95cb/raw/coverage.DialogueKit.main.json) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![PyPi version](https://img.shields.io/pypi/v/dialoguekit)](https://pypi.org/project/dialoguekit/)
+![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/adrzewiecki/35bb996459f0949b38da651c66cf95cb/raw/coverage.DialogueKit.main.json)
 ![Tests](https://img.shields.io/github/actions/workflow/status/iai-group/DialogueKit/merge.yaml?label=Tests&branch=main)
+![docs](https://img.shields.io/github/actions/workflow/status/iai-group/DialogueKit/build_docs.yaml?label=docs&branch=main)
 ![Python version](https://img.shields.io/badge/python-3.9-blue)
 
 DialogueKit is a library for conversational information access (CIA). It contains based classes for fundamental [concepts](https://iai-group.github.io/DialogueKit/main/concepts.html), such as dialogue participants, dialogue management, [natural language understanding](https://iai-group.github.io/DialogueKit/main/nlu.html), natural language generation, etc. In addition to the fundamental concepts DialogueKit contains an evaluation module, for evaluating the performance of and CIA systems.
 Consult the [documentation](https://iai-group.github.io/DialogueKit/main/) for details.
 
 ## Install as a package
 
 DialogueKit is published to PyPI, install it by running:
 
 ```shell
 pip install dialoguekit
 ```
 
-If you want to install a DialogueKit from a specific commit or straight from github this is still possible.
+Follow the commands below to install DialogueKit from a specific commit or straight from GitHub.
 
 The command will install the latest version from the main branch.
 
-  * On Windows you may need to run this command before pip installing
+  - On Windows you may need to run this command before pip installing
 
-  ```shell
-  ssh -t git github.com    
-  ```
+```shell
+ssh -t git github.com
+```
 
-  * pip install
+  - pip install
 
-  ```shell
-  pip install git+ssh://git@github.com/iai-group/dialoguekit.git
-  ```
+```shell
+pip install git+ssh://git@github.com/iai-group/dialoguekit.git
+```
 
 If you want to specify a specific commit as the source of the package append the commit hash to the end of the command separated with a "@".
 
-  * Specific commit as the source of the package.
+  - Specific commit as the source of the package.
 
-  ```shell
-  pip install git+ssh://git@github.com/iai-group/dialoguekit.git@faa5c1fca37aaa275105cc1ca7698783719551c2
-  ```
+```shell
+pip install git+ssh://git@github.com/iai-group/dialoguekit.git@faa5c1fca37aaa275105cc1ca7698783719551c2
+```
 
 ## Usage example
 
-1. Define agent and user
+1. Create and connect a platform that manages dialogues. The platform requires information about the agent it serves.
 
-    ```python
-    from dialoguekit.core.utterance import Utterance
-    from dialoguekit.participant.user import User, UserType
-    from sample_agents.parrot_agent import ParrotAgent
+   ```python
+   from dialoguekit.platforms.terminal_platform import TerminalPlatform
+   from sample_agents.parrot_agent import ParrotAgent
 
-    # Participants
-    agent = ParrotAgent("A01")
-    user = User("U01")
-    ```
+   platform = TerminalPlatform(ParrotAgent)
+   ```
 
-2. Create and connect platform and dialogue manager
+2. Start conversation
 
-    ```python
-    from dialoguekit.platforms.platform import Platform
-    from dialoguekit.manager.dialogue_manager import DialogueManager
-
-    platform = Platform()
-    dm = DialogueManager(agent, user, platform)
-
-    user.connect_dialogue_manager(dm)
-    agent.connect_dialogue_manager(dm)
-    ```
-
-3. Start conversation
-
-    ```python
-      dm.start()
-      dm.close()
-    ```
+   ```python
+      platform.start()
+   ```
 
 ## Conventions
 
-We follow the [IAI Python Style Guide](https://github.com/iai-group/styleguide/tree/main/python).
+We follow the [IAI Python Style Guide](https://github.com/iai-group/styleguide/tree/main/python).  
+We use `UTF-8` encodings that is widely used on Unix systems. Windows users need to use the `Python UTF-8 Mode`; see [here](https://docs.python.org/3/using/windows.html#utf-8-mode) for more details. In practice, we specify the encoding when opening files, as in this example:
+
+```python
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+```
 
 ## Contributors
 
-(Alphabetically ordered by last name) 
+(Alphabetically ordered by last name)
 
-  * Jafar Afzali (2022)
-  * Krisztian Balog (2021-present)
-  * Nolwenn Bernard (2022-present)
-  * Aleksander Drzewiecki (2022)
-  * Shuo Zhang (2021)
+  - Jafar Afzali (2022)
+  - Krisztian Balog (2021-present)
+  - Nolwenn Bernard (2022-present)
+  - Aleksander Drzewiecki (2022)
+  - Ivica Kostric (2023)
+  - Weronika Lajewska (2023)
+  - Shuo Zhang (2021)
```

### Comparing `dialoguekit-0.0.8/dialoguekit.egg-info/SOURCES.txt` & `dialoguekit-0.0.9/dialoguekit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 ./dialoguekit/__init__.py
 ./dialoguekit/connector/__init__.py
 ./dialoguekit/connector/dialogue_connector.py
 ./dialoguekit/core/__init__.py
 ./dialoguekit/core/annotated_utterance.py
 ./dialoguekit/core/annotation.py
 ./dialoguekit/core/dialogue.py
+./dialoguekit/core/dialogue_act.py
 ./dialoguekit/core/domain.py
+./dialoguekit/core/feedback.py
 ./dialoguekit/core/intent.py
 ./dialoguekit/core/slot_value_annotation.py
 ./dialoguekit/core/utterance.py
 ./dialoguekit/nlg/__init__.py
 ./dialoguekit/nlg/nlg_abstract.py
 ./dialoguekit/nlg/nlg_conditional.py
 ./dialoguekit/nlg/nlg_template.py
 ./dialoguekit/nlg/template_from_training_data.py
 ./dialoguekit/nlu/__init__.py
 ./dialoguekit/nlu/intent_classifier.py
 ./dialoguekit/nlu/nlu.py
+./dialoguekit/nlu/slot_annotator.py
 ./dialoguekit/nlu/slot_annotator_dict.py
 ./dialoguekit/nlu/models/__init__.py
 ./dialoguekit/nlu/models/diet_classifier_rasa.py
 ./dialoguekit/nlu/models/intent_classifier_cosine.py
 ./dialoguekit/nlu/models/satisfaction_classifier.py
 ./dialoguekit/nlu/models/satisfaction/LinearSVC_2_0.joblib
 ./dialoguekit/nlu/models/satisfaction/__init__.py
@@ -38,31 +41,34 @@
 ./dialoguekit/nlu/models/satisfaction/vectorizer_2_0.joblib
 ./dialoguekit/participant/__init__.py
 ./dialoguekit/participant/agent.py
 ./dialoguekit/participant/participant.py
 ./dialoguekit/participant/user.py
 ./dialoguekit/participant/user_preferences.py
 ./dialoguekit/platforms/__init__.py
+./dialoguekit/platforms/flask_socket_platform.py
 ./dialoguekit/platforms/platform.py
+./dialoguekit/platforms/terminal_platform.py
 ./dialoguekit/utils/__init__.py
 ./dialoguekit/utils/annotation_converter.py
 ./dialoguekit/utils/annotation_converter_dialoguekit_to_rasa.py
 ./dialoguekit/utils/dialogue_evaluation.py
 ./dialoguekit/utils/dialogue_reader.py
 ./sample_agents/__init__.py
 ./sample_agents/moviebot_agent.py
 ./sample_agents/parrot_agent.py
 ./sample_agents/rasa_parrot_agent.py
 ./sample_agents/woz_agent.py
 ./tests/__init__.py
 ./tests/core/__init__.py
 ./tests/core/test_annotated_utterance.py
 ./tests/core/test_dialogue.py
+./tests/core/test_domain.py
+./tests/core/test_feedback.py
 ./tests/core/test_intent.py
-./tests/core/test_ontology.py
 ./tests/core/test_slot_value_annotation.py
 ./tests/core/test_utterance.py
 ./tests/nlg/__init__.py
 ./tests/nlg/test_conditional_nlg.py
 ./tests/nlg/test_template_from_training_data.py
 ./tests/nlg/test_template_nlg.py
 ./tests/nlu/__init__.py
@@ -144,15 +150,14 @@
 docs/source/docs_env.yaml
 docs/source/external_agents.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/nlg.rst
 docs/source/nlu.rst
 docs/source/usage.rst
-docs/source/_static/DialogueKit-Architecture.png
 docs/source/_static/favicon.png
 docs/source/_templates/layout.html
 docs/source/_templates/versions.html
 external_agents/rasa-parrot/config.yml
 external_agents/rasa-parrot/credentials.yml
 external_agents/rasa-parrot/domain.yml
 external_agents/rasa-parrot/endpoints.yml
@@ -170,15 +175,14 @@
 sample_agents/rasa_parrot_agent.py
 sample_agents/woz_agent.py
 tests/__init__.py
 tests/core/__init__.py
 tests/core/test_annotated_utterance.py
 tests/core/test_dialogue.py
 tests/core/test_intent.py
-tests/core/test_ontology.py
 tests/core/test_slot_value_annotation.py
 tests/core/test_utterance.py
 tests/data/annotated_dialogues.json
 tests/data/domains/movie.yaml
 tests/nlg/__init__.py
 tests/nlg/test_conditional_nlg.py
 tests/nlg/test_template_from_training_data.py
```

### Comparing `dialoguekit-0.0.8/docs/Makefile` & `dialoguekit-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/docs/components.graffle` & `dialoguekit-0.0.9/docs/components.graffle`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/docs/evaluation.md` & `dialoguekit-0.0.9/docs/evaluation.md`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/docs/source/_static/favicon.png` & `dialoguekit-0.0.9/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/docs/source/_templates/layout.html` & `dialoguekit-0.0.9/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/docs/source/_templates/versions.html` & `dialoguekit-0.0.9/docs/source/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/docs/source/conf.py` & `dialoguekit-0.0.9/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 project = "DialogueKit"
 copyright = "2022, IAI group, University of Stavanger"
 author = "Jafar Afzali, Krisztian Balog, Aleksander Drzewiecki \
         and Shuo Zhang"
 
 # The short X.Y version.
-version = "0.0.8"
+version = "0.0.9"
 # The full version, including alpha/beta/rc tags.
-release = "0.0.8"
+release = "0.0.9"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `dialoguekit-0.0.8/docs/source/dialogue_export.rst` & `dialoguekit-0.0.9/docs/source/dialogue_export.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 DialogueKit Dialogue Export Format
 =====================================
 
 DialogueKit follows a specific format when exporting dialogues to JSON.
-Dialogues are stored in seperate files for each user-agent pair.
+Dialogues are stored in separate files for each user-agent pair.
 
 Format
 ------
 
 .. code-block:: json
 
   {
```

### Comparing `dialoguekit-0.0.8/docs/source/external_agents.rst` & `dialoguekit-0.0.9/docs/source/external_agents.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,35 @@
----
-orphan: true
----
-
 External Agents
 ===============
 
-Rasa parrot
---------------
+DialogueKit is shipped with 4 agents, which are presented below.
+New agents can be implemented by inheriting from :py:class:`dialoguekit.participant.agent.Agent`.
+
+ParrotAgent
+-----------
+
+:py:mod:`sample_agents.parrot_agent`
+
+This agent will welcome the user, but will always parrot (echo) what the user says.
+
+RasaParrotAgent
+---------------
 
-The :py:mod:`sample_agents.rasa_parrot_agent.py` **Agent** is just an example of how a Rasa agent could be used in DialogueKit.
-This **Agent** talks to the :py:mod:`additional.rasa-parrot` which does all the processing while the **DialogueKit Rasa Agent** only handles the communication.
+:py:mod:`sample_agents.rasa_parrot_agent`
 
+This agent is just an example of how a Rasa agent could be used in DialogueKit.
+It talks to the :py:mod:`external_agents.rasa-parrot` which does all the processing, while the RasaParrotAgent only handles the communication.
 
 How to use the Rasa parrot
-^^^^^^^^^^^^^^^^^^^^^^^^^^
+""""""""""""""""""""""""""
 
 Start the Rasa service
 """"""""""""""""""""""
 
-To use the Rasa parroting **Agent** we firstly need to start the **Rasa service**.
+To use RasaParrotAgent, we firstly need to start the **Rasa service**.
 
 1. Move to the right directory
 
     .. code-block:: shell
 
         cd additional/rasa-parrot
 
@@ -41,27 +48,40 @@
 4. Start service endpoint
 
     .. code-block:: shell
 
         rasa run -m models --endpoints endpoints.yml --port 5002 --credentials credentials.yml
 
 
-Use the Rasa parroting Agent
-""""""""""""""""""""""""""""
+Use RasaParrotAgent
+"""""""""""""""""""
 
-We can now talk to the Rasa parroting service with the **Agent**.
-To do this we need to actually use the **Agent** in our project.
+We can now talk to the Rasa parroting service with the RasaParrotAgent.
+To do this we need to actually use the RasaParrotAgent in our project.
 An example can be seen below.
 
 .. code-block:: python
 
     agent = RasaParrotAgent(agent_id="TestId")
     user = User("U01")
-    platform = Platform()
+    platform = TerminalPlatform()
     dc = DialogueConnector(agent, user, platform)
     dc.start()
     dc.close()
 
 
-In this example we use a **User** to talk to the Rasa parroting service.
+In this example, we use a user to talk to the Rasa parroting service.
 This allows us to interact with the parrot with python inputs.
 
+MovieBotAgent
+-------------
+
+:py:mod:`sample_agents.moviebot_agent`
+
+A connector agent for `IAI MovieBot <https://github.com/iai-group/moviebot>`_ .
+
+WozAgent
+--------
+
+:py:mod:`sample_agents.woz_agent`
+
+Allows a real human to play the role of the agent ("wizard") when interacting with a user. This can be useful, e.g., when testing user simulators.
```

### Comparing `dialoguekit-0.0.8/docs/source/installation.rst` & `dialoguekit-0.0.9/docs/source/installation.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Installation
 ============
 
 Install as a package
 --------------------
 
-**Note:** *Packaging is still a work in progress and may not work perfectly.*
+DialogueKit is published to PyPI. Install it by running:
+
+  .. code-block:: shell
+    pip install dialoguekit
+
+
+Follow the commands below to install DialogueKit from a specific commit or straight from GitHub.
 
-As of now DialogueKit is not published as a package, but it is still possible to install it with pip.
 The command will install the latest version from the main branch.
 
 * On Windows you may need to run this command before pip installing
   
   .. code-block:: shell
 
     ssh -t git github.com    
@@ -26,8 +31,7 @@
 If you want to specify a specific commit as the source of the package append the commit hash to the end of the command separated with a "@".
 
 * Specific commit as the source of the package.
 
   .. code-block:: shell
     
     pip install git+ssh://git@github.com/iai-group/dialoguekit.git@faa5c1fca37aaa275105cc1ca7698783719551c2
-
```

### Comparing `dialoguekit-0.0.8/docs/source/nlg.rst` & `dialoguekit-0.0.9/docs/source/nlg.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Natural Language Generation (NLG)
 =================================
 
-The NLG components in Dialoguekit are currently template-based.
+The NLG components in DialogueKit are currently template-based.
 The basic template-based generation works by extracting templates from a set of training data. The templates are the user and agent utterances with the annotations removed. This version can be found here: :py:class:`dialoguekit.nlg.nlg_template.TemplateNLG`.
 
-An extended version of the basic template-based implementation which can perform conditional language generation is :py:class:`dialoguekit.nlg.nlg_conditional.ConditionalNLG`. Using a conditional may be useful in cases were other attributes then the intent and annotations may be of interest. Such as the users satisfaction. This can then be used to selecting templates that have a different tone based on the conditional, in this case the satisfaction score.
+An extended version of the basic template-based implementation which can perform conditional language generation is :py:class:`dialoguekit.nlg.nlg_conditional.ConditionalNLG`.
+Using a conditional may be useful in cases where other attributes than the intent and annotations may be of interest , for example, the user's satisfaction.
+This can then be used to select templates that have a different tone based on the conditional.
 
 These two are used in similar ways. The only difference is that the `ConditionalNLG` can use a conditional in the :py:attr:`dialoguekit.core.annotated_utterance.AnnotatedUtterance.metadata` as long as the conditional value is a number.
 
 To start using these NLG classes a template needs to be generated. 
 Two methods for doing this are provided:
 
     * :py:meth:`dialoguekit.nlg.template_from_training_data.build_template_from_instances`
@@ -17,23 +19,23 @@
 Usage Example
 """""""""""""
 
 .. code:: python
 
     from dialoguekit.core.annotation import Annotation
     from dialoguekit.core.intent import Intent
-    from dialoguekit.nlg.nlg import NLG
+    from dialoguekit.nlg.nlg_template import TemplateNLG
     from dialoguekit.nlg.template_from_training_data import (
         extract_utterance_template,
     )
 
     template = extract_utterance_template(
         annotated_dialogue_file=ANNOTATED_DIALOGUE_FILE_PATH,
     )
-    nlg = NLG(response_templates=template)
+    nlg = TemplateNLG(response_templates=template)
     
     response = nlg.generate_utterance_text(intent=Intent("COMPLETE"))
 
 ConditionalNLG
 """"""""""""""
 
 The ConditionalNLG class contains two additional parameters to the ``generate_utterance_text()`` method.
```

### Comparing `dialoguekit-0.0.8/docs/source/nlu.rst` & `dialoguekit-0.0.9/docs/source/nlu.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,46 +2,41 @@
 ====================================
 
 The NLU component is responsible for obtaining a structured representation of text utterances. Currently, it entails intent classification, entity recognition, and user satisfaction prediction.
 
 Intent Classification
 ---------------------
 
-Thus far two different NLU pipelines are implemented for intent classification
+Thus far two different NLU pipelines are implemented for intent classification.
 
-* Cosine intent classifier :py:mod:`dialoguekit.nlu.intent_classifier_cosine`
+* Cosine intent classifier :py:mod:`dialoguekit.nlu.models.intent_classifier_cosine`
 
-* Rasa DIET classifier :py:mod:`dialoguekit.nlu.diet_classifier_rasa`
-
-An explanation of the implementation of Rasa DIET classifier can be read
+* Rasa DIET classifier :py:mod:`dialoguekit.nlu.models.diet_classifier_rasa`
 
+See below for details on how the Rasa DIET classifier is used in our implementation.
 
 Rasa as a component library
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 *diet_classifier_rasa* implement Rasa's DIET classifier. This is a Dual Intent and Entity Transformer, their paper can be read 
 `here. <https://arxiv.org/pdf/2004.09936.pdf>`_
 
-Normally one would use Rasa as the underlying platform. But for our use-case we need to use it as a component in Dialoguekit. This proved to be possible with a bit of effort. Rasa is distributed with a Apache 2.0 license, granting us free use.
+Normally, one would use Rasa as the underlying platform. Here, instead, we use it as a component in DialogueKit. Rasa is distributed with a Apache 2.0 license, granting us free use.
 
 General idea
 """"""""""""
 
-In general the idea was to import the necessary packages and re-implement the rasa workflow with their components and structures. Rasa is built in a very object oriented structure. This does not allow us to use Dialoguekit objects, they need to be transformed to Rasa components before use.
-
-How we implemented it
-"""""""""""""""""""""
-
-As stated by a author on medium (link will be updated), the general structure of Rasa is a hard one to understand at first, but after a lot of trial and error we found the best way to get what we needed was to look at the implementation of the tests. They often show a minimal way of using the components separately and in conjunction with each other
+In general, the idea is to import the necessary packages and re-implement the Rasa workflow with their components and structures. 
+However, because of how Rasa is structured, DialogueKit objects need to be transformed to Rasa components before use.
 
-The result
-""""""""""
+Implementation
+""""""""""""""
 
-The first rasa implementation is in *diet_classifier_rasa*, this model can be trained and thus uses multiple rasa components and structures.
-Below you can see all the imports that are used, only from rasa.
+The implementation is in *diet_classifier_rasa*; this model can be trained and thus uses multiple Rasa components and structures.
+Below is a list of all the Rasa imports that are used.
 
 .. code-block:: python
 
     from rasa.engine.graph import ExecutionContext, GraphComponent, GraphSchema
     from rasa.shared.nlu.constants import TEXT
     from rasa.nlu.featurizers.sparse_featurizer.count_vectors_featurizer import (
         CountVectorsFeaturizer,
@@ -56,15 +51,15 @@
 
 Entity Extraction
 -----------------
 
 As of now only one implementation exists, the Rasa DIET classifier.
 
 User Satisfaction Prediction
----------------------------
+----------------------------
 
 User satisfaction prediction entails the task of predicting a user's satisfaction with the system, based on the conversation.
 We model this as a classification task, where, given the previous *n* user-agent turns, the task of the classifier is to predict the user satisfaction on a scale from 1-5:
 
 #. Very dissatisfied
 #. Dissatisfied
 #. Normal
```

### Comparing `dialoguekit-0.0.8/external_agents/rasa-parrot/actions/actions.py` & `dialoguekit-0.0.9/external_agents/rasa-parrot/actions/actions.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/external_agents/rasa-parrot/config.yml` & `dialoguekit-0.0.9/external_agents/rasa-parrot/config.yml`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/external_agents/rasa-parrot/credentials.yml` & `dialoguekit-0.0.9/external_agents/rasa-parrot/credentials.yml`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/external_agents/rasa-parrot/endpoints.yml` & `dialoguekit-0.0.9/external_agents/rasa-parrot/endpoints.yml`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/sample_agents/moviebot_agent.py` & `dialoguekit-0.0.9/sample_agents/moviebot_agent.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/sample_agents/parrot_agent.py` & `dialoguekit-0.0.9/sample_agents/parrot_agent.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/sample_agents/woz_agent.py` & `dialoguekit-0.0.9/sample_agents/woz_agent.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/setup.py` & `dialoguekit-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 
 packages = setuptools.find_packages(where="dialoguekit")
 
 setuptools.setup(
     name="dialoguekit",
-    version="0.0.8",
+    version="0.0.9",
     author="Jafar Afzali, Krisztian Balog, Nolwenn Bernard, \
         Aleksander Drzewiecki and Shuo Zhang",
     author_email="author@example.com",
     description=(
         "Toolkit for building conversational information access systems."
     ),
     long_description=long_description,
@@ -34,9 +34,15 @@
             "*.joblib",
             "dialoguekit/nlu/models/satisfaction/*.joblib",
         ]
     },
     include_package_data=True,
     python_requires=">=3.9",
     zip_safe=False,
-    install_requires=["rasa>=3.0"],
+    install_requires=[
+        "rasa>=3.0",
+        "Flask==2.2.3",
+        "flask-socketio==5.3.3",
+        "Werkzeug==2.2.3",
+        "websockets<11.0",
+    ],
 )
```

### Comparing `dialoguekit-0.0.8/tests/core/test_annotated_utterance.py` & `dialoguekit-0.0.9/tests/core/test_annotated_utterance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 """Tests for the Utterance class."""
-import pytest
+
 from dialoguekit.core import AnnotatedUtterance, Intent
 from dialoguekit.participant import DialogueParticipant
 
 
 def test_utterance_text():
     """Tests setting text."""
     u = AnnotatedUtterance("Hello world", DialogueParticipant.USER)
     assert u.text == "Hello world"
 
 
-def test_hash():
-    """Tests hashing of the object."""
-    u1 = AnnotatedUtterance(
-        "Test1", intent=Intent("1"), participant=DialogueParticipant.AGENT
-    )
-    try:
-        hash(u1)
-    except TypeError:
-        pytest.fail("AnnotatedUtterance hashing failed")
-
-
 def test_comparison():
     """Tests object comparison."""
     u1 = AnnotatedUtterance(
         "Test1", intent=Intent("1"), participant=DialogueParticipant.AGENT
     )
     u2 = u1
     assert u1 == u2
```

### Comparing `dialoguekit-0.0.8/tests/core/test_dialogue.py` & `dialoguekit-0.0.9/tests/core/test_dialogue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """Tests for the Dialogue class."""
 
+import calendar
+import datetime
+
 import pytest
 
-from dialoguekit.core import Dialogue, Utterance
-from dialoguekit.core.annotated_utterance import AnnotatedUtterance
-from dialoguekit.core.annotation import Annotation
-from dialoguekit.core.intent import Intent
+from dialoguekit.core import (
+    AnnotatedUtterance,
+    Annotation,
+    Dialogue,
+    Intent,
+    Utterance,
+)
 from dialoguekit.participant import DialogueParticipant
 
 
 # Dialogue history object to be shared across multiple test cases.
 @pytest.fixture(scope="module")
 def dialogue_history_1() -> Dialogue:
     """Dialogue with unannotated utterances fixture."""
     agent_id = "agent-001"
     user_id = "USR01"
+    conversation_id = "CNV1"
     agent_utterance_1 = Utterance(
         "Hello", participant=DialogueParticipant.AGENT
     )
     user_utterance_1 = Utterance("Hi", participant=DialogueParticipant.USER)
     agent_utterance_2 = Utterance(
         "Can I help you?", participant=DialogueParticipant.AGENT
     )
@@ -30,25 +37,26 @@
         agent_utterance_1,
         user_utterance_1,
         agent_utterance_2,
         user_utterance_2,
         agent_utterance_3,
     ]
 
-    dialogue_history = Dialogue(agent_id, user_id)
+    dialogue_history = Dialogue(agent_id, user_id, conversation_id)
     for utterance in utterances:
         dialogue_history.add_utterance(utterance)
     return dialogue_history
 
 
 @pytest.fixture(scope="module")
 def dialogue_history_2() -> Dialogue:
     """Dialogue with annotated utterances and metadata fixture."""
     agent_id = "agent-002"
     user_id = "USR02"
+    conversation_id = "CNV1"
     agent_utterance_1 = AnnotatedUtterance(
         "Hello",
         participant=DialogueParticipant.AGENT,
         intent=Intent("GREETINGS"),
     )
     user_utterance_1 = AnnotatedUtterance(
         "Hi", participant=DialogueParticipant.USER, intent=Intent("GREETINGS")
@@ -61,28 +69,41 @@
     )
     utterances = [
         agent_utterance_1,
         user_utterance_1,
         agent_utterance_2,
     ]
 
-    dialogue_history = Dialogue(agent_id, user_id)
+    dialogue_history = Dialogue(agent_id, user_id, conversation_id)
     dialogue_history.metadata.update(
         {"description": "Dialogue fixture for testing"}
     )
     for utterance in utterances:
         dialogue_history.add_utterance(utterance)
 
     return dialogue_history
 
 
 @pytest.fixture(scope="module")
 def dialogue_history_3() -> Dialogue:
     """Empty dialogue fixture."""
-    return Dialogue("agent-003", "USR03")
+    return Dialogue("agent-003", "USR03", "CNV1")
+
+
+def test_initialization():
+    """Tests dialogue initialization."""
+    agent_id = "agent-002"
+    user_id = "USR02"
+    conversation_id = "CNV1"
+    dialogue_1 = Dialogue(agent_id, user_id, conversation_id)
+    assert dialogue_1.conversation_id == conversation_id
+    dialogue_2 = Dialogue(agent_id, user_id)
+    date = datetime.datetime.utcnow()
+    utc_time = calendar.timegm(date.utctimetuple())
+    assert dialogue_2.conversation_id == f"{agent_id}-{user_id}-{str(utc_time)}"
 
 
 def test_ids(dialogue_history_1: Dialogue) -> None:
     """Tests dialogue parameters.
 
     Args:
         dialogue_history_1: Test Dialogue object.
@@ -97,43 +118,70 @@
     Args:
         dialogue_history_1: Test Dialogue object.
     """
     assert len(dialogue_history_1.utterances) == len(
         dialogue_history_1.utterances
     )
     assert dialogue_history_1.utterances[0].text == "Hello"
+    assert dialogue_history_1.utterances[0].utterance_id == "CNV1_agent-001_0"
     assert (
         dialogue_history_1.utterances[0].participant
         == DialogueParticipant.AGENT
     )
     assert (
         dialogue_history_1.utterances[1].participant == DialogueParticipant.USER
     )
     assert dialogue_history_1.utterances[1].text == "Hi"
+    assert dialogue_history_1.utterances[1].utterance_id == "CNV1_USR01_1"
     assert (
         dialogue_history_1.utterances[4].participant
         == DialogueParticipant.AGENT
     )
 
 
+def test_add_utterance() -> None:
+    """Tests adding utterance to dialogue history."""
+    agent_id = "agent-002"
+    user_id = "USR02"
+    conversation_id = "CNV1"
+    utterance_no_id = AnnotatedUtterance(
+        "Hi", participant=DialogueParticipant.USER, intent=Intent("GREETINGS")
+    )
+    utterance_with_id = AnnotatedUtterance(
+        "Hi",
+        utterance_id="u_1",
+        participant=DialogueParticipant.AGENT,
+        intent=Intent("GREETINGS"),
+    )
+    dialogue_history = Dialogue(agent_id, user_id, conversation_id)
+
+    dialogue_history.add_utterance(utterance_no_id)
+    dialogue_history.add_utterance(utterance_with_id)
+
+    assert dialogue_history.utterances[0].utterance_id == "CNV1_USR02_0"
+    assert dialogue_history.utterances[1].utterance_id == "u_1"
+
+
 def test_to_dict_d1(dialogue_history_1: Dialogue) -> None:
     """Tests dialogue export to dictionary.
 
     Args:
         dialogue_history_1: Test Dialogue object 1.
         dialogue_history_2: Test Dialogue object 2.
     """
     dialogue_dict_1 = dialogue_history_1.to_dict()
 
     assert dialogue_dict_1.get("agent") == "agent-001"
     assert dialogue_dict_1.get("user") == "USR01"
+    assert dialogue_dict_1.get("conversation ID") == "CNV1"
     assert dialogue_dict_1.get("metadata") is None
     assert len(dialogue_dict_1.get("conversation")) == 5
     utterance_1 = dialogue_dict_1.get("conversation")[0]
     assert utterance_1["utterance"] == "Hello"
+    assert utterance_1["utterance ID"] == "CNV1_agent-001_0"
     assert utterance_1.get("slot_values") is None
 
 
 def test_to_dict_d2(dialogue_history_2: Dialogue) -> None:
     """Tests dialogue export to dictionary.
 
     Dialogue has annotations and metadata.
```

### Comparing `dialoguekit-0.0.8/tests/core/test_intent.py` & `dialoguekit-0.0.9/tests/core/test_intent.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/tests/core/test_slot_value_annotation.py` & `dialoguekit-0.0.9/tests/core/test_slot_value_annotation.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/tests/core/test_utterance.py` & `dialoguekit-0.0.9/tests/core/test_utterance.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """Tests for the Utterance class."""
 import pytest
+
 from dialoguekit.core import Utterance
 from dialoguekit.participant import DialogueParticipant
 
 
 def test_utterance_text():
     """Tests setting of the utterance text."""
-    u = Utterance("Hello world", participant=DialogueParticipant.AGENT)
+    u = Utterance(
+        "Hello world", utterance_id="u1", participant=DialogueParticipant.AGENT
+    )
     assert u.text == "Hello world"
 
 
 def test_hash():
     """Tests hashing of the utterance object."""
-    u1 = Utterance("Test1", participant=DialogueParticipant.AGENT)
+    u1 = Utterance(
+        "Test1", utterance_id="u1", participant=DialogueParticipant.AGENT
+    )
     try:
         hash(u1)
     except TypeError:
         pytest.fail("Utterance hashing failed")
 
 
 def test_comparison():
@@ -28,7 +33,16 @@
     u3 = Utterance("Test1", participant=DialogueParticipant.AGENT)
     assert u1 == u3
 
     # Test Text difference
     u1 = Utterance(text="Test1", participant=DialogueParticipant.AGENT)
     u2 = Utterance(text="Test2", participant=DialogueParticipant.AGENT)
     assert u1 != u2
+
+    # Test ID difference
+    u1 = Utterance(
+        text="Test1", utterance_id="u1", participant=DialogueParticipant.AGENT
+    )
+    u2 = Utterance(
+        text="Test1", utterance_id="u2", participant=DialogueParticipant.AGENT
+    )
+    assert u1 != u2
```

### Comparing `dialoguekit-0.0.8/tests/data/annotated_dialogues.json` & `dialoguekit-0.0.9/tests/data/annotated_dialogues.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.28135265700483086%*

 * *Differences: {'0': "{'conversation': {0: {'utterance_id': 'CNV1_TEST03_0'}, 1: {'utterance_id': "*

 * *      "'CNV1_MovieBotTester_1'}, 2: {'utterance_id': 'CNV1_TEST03_2'}, 3: {'utterance_id': "*

 * *      "'CNV1_MovieBotTester_3'}, 4: {'utterance_id': 'CNV1_MovieBotTester_4'}, 5: {'utterance_id': "*

 * *      "'CNV1_TEST03_5'}, 6: {'utterance_id': 'CNV1_MovieBotTester_6'}, 7: {'utterance_id': "*

 * *      "'CNV1_TEST03_7'}, 8: {'utterance_id': 'CNV1_MovieBotTester_8'}, 9: {'utterance_id': "*

 * *      "'CNV1_TEST03_9'}, 10: {'utterance_id': ' […]*

```diff
@@ -1,103 +1,119 @@
 [
     {
+        "agent": {
+            "id": "MovieBotTester",
+            "type": "AGENT"
+        },
         "conversation": [
             {
                 "intent": "DISCLOSE.NON-DISCLOSE",
                 "participant": "USER",
-                "utterance": "hello\n"
+                "utterance": "hello\n",
+                "utterance_id": "CNV1_TEST03_0"
             },
             {
                 "intent": "INQUIRE.ELICIT",
                 "participant": "AGENT",
-                "utterance": "Which genres do you prefer?\n"
+                "utterance": "Which genres do you prefer?\n",
+                "utterance_id": "CNV1_MovieBotTester_1"
             },
             {
                 "intent": "DISCLOSE",
                 "participant": "USER",
                 "slot_values": [
                     [
                         "GENRE",
                         "action"
                     ],
                     [
                         "GENRE",
                         "fantasy"
                     ]
                 ],
-                "utterance": "action, fantasy\n"
+                "utterance": "action, fantasy\n",
+                "utterance_id": "CNV1_TEST03_2"
             },
             {
                 "intent": "REVEAL.EXPAND",
                 "participant": "AGENT",
-                "utterance": "I have found almost 500 fantasy and action films. Can you guide me more to narrow down the search space?\n"
+                "utterance": "I have found almost 500 fantasy and action films. Can you guide me more to narrow down the search space?\n",
+                "utterance_id": "CNV1_MovieBotTester_3"
             },
             {
                 "intent": "REVEAL.EXPAND",
                 "participant": "AGENT",
-                "utterance": "Can you give me a few keywords? For example, 'space opera' or 'galactic war'.\n"
+                "utterance": "Can you give me a few keywords? For example, 'space opera' or 'galactic war'.\n",
+                "utterance_id": "CNV1_MovieBotTester_4"
             },
             {
                 "intent": "REVEAL.EXPAND",
                 "participant": "USER",
                 "slot_values": [
                     [
                         "TITLE",
                         "lord of the rings"
                     ]
                 ],
-                "utterance": "something like the lord of the rings\n"
+                "utterance": "something like the lord of the rings\n",
+                "utterance_id": "CNV1_TEST03_5"
             },
             {
                 "intent": "REVEAL.LIST",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "TITLE",
                         "Kung Fu Hustle"
                     ]
                 ],
-                "utterance": "There is a fantasy and action, lord film named \"\"Kung Fu Hustle\"\". Have you seen this one?\n"
+                "utterance": "There is a fantasy and action, lord film named \"\"Kung Fu Hustle\"\". Have you seen this one?\n",
+                "utterance_id": "CNV1_MovieBotTester_6"
             },
             {
                 "intent": "REVEAL.SIMILAR",
                 "participant": "USER",
-                "utterance": "anything else?\n"
+                "utterance": "anything else?\n",
+                "utterance_id": "CNV1_TEST03_7"
             },
             {
                 "intent": "REVEAL.SIMILAR",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "TITLE",
                         "Conan the Barbarian"
                     ]
                 ],
-                "utterance": "There is a fantasy and action, lord film named \"\"Conan the Barbarian\"\". Have you seen this one?\n"
+                "utterance": "There is a fantasy and action, lord film named \"\"Conan the Barbarian\"\". Have you seen this one?\n",
+                "utterance_id": "CNV1_MovieBotTester_8"
             },
             {
                 "intent": "NOTE.NOTE-YES",
                 "participant": "USER",
-                "utterance": "already seen it\n"
+                "utterance": "already seen it\n",
+                "utterance_id": "CNV1_TEST03_9"
             },
             {
                 "intent": "REVEAL.SIMILAR",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "TITLE",
                         "Dracula Untold"
                     ]
                 ],
-                "utterance": "I would like to recommend you a fantasy and action, lord film named \"\"Dracula Untold\"\". Have you watched it?\n"
+                "utterance": "I would like to recommend you a fantasy and action, lord film named \"\"Dracula Untold\"\". Have you watched it?\n",
+                "utterance_id": "CNV1_MovieBotTester_10"
             },
             {
                 "intent": "NOTE.NOTE-YES",
                 "participant": "USER",
-                "utterance": "i know this one\n"
+                "utterance": "i know this one\n",
+                "utterance_id": "CNV1_TEST03_11"
             },
             {
                 "intent": "SUGGEST",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "GENRE",
@@ -112,20 +128,22 @@
                         "lord"
                     ],
                     [
                         "TITLE",
                         "similar to one"
                     ]
                 ],
-                "utterance": "Sorry, I don't have any fantasy and action, lord films named similar to one. Please select from the list of options to continue.\n"
+                "utterance": "Sorry, I don't have any fantasy and action, lord films named similar to one. Please select from the list of options to continue.\n",
+                "utterance_id": "CNV1_MovieBotTester_12"
             },
             {
                 "intent": "DISCLOSE",
                 "participant": "USER",
-                "utterance": "a new movie\n"
+                "utterance": "a new movie\n",
+                "utterance_id": "CNV1_TEST03_13"
             },
             {
                 "intent": "SUGGEST",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "GENRE",
@@ -140,20 +158,22 @@
                         "lord"
                     ],
                     [
                         "TITLE",
                         "similar to one"
                     ]
                 ],
-                "utterance": "Sorry, I couldn't find any fantasy and action, lord films named similar to one from the year  > 2010. Please select from the list of options to continue.\n"
+                "utterance": "Sorry, I couldn't find any fantasy and action, lord films named similar to one from the year  > 2010. Please select from the list of options to continue.\n",
+                "utterance_id": "CNV1_MovieBotTester_14"
             },
             {
                 "intent": "INQUIRE",
                 "participant": "USER",
-                "utterance": "Release year shouldn't be the \"\"year  > 2010\"\".\n"
+                "utterance": "Release year shouldn't be the \"\"year  > 2010\"\".\n",
+                "utterance_id": "CNV1_TEST03_15"
             },
             {
                 "intent": "SUGGEST",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "GENRE",
@@ -168,26 +188,28 @@
                         "lord"
                     ],
                     [
                         "TITLE",
                         "similar to one"
                     ]
                 ],
-                "utterance": "Sorry, I couldn't find any fantasy and action, lord films named similar to one. Please select from the list of options to continue.\n"
+                "utterance": "Sorry, I couldn't find any fantasy and action, lord films named similar to one. Please select from the list of options to continue.\n",
+                "utterance_id": "CNV1_MovieBotTester_16"
             },
             {
                 "intent": "REVEAL.REFINE",
                 "participant": "USER",
                 "slot_values": [
                     [
                         "TITLE",
                         "one"
                     ]
                 ],
-                "utterance": "No movies named like \"\"one\"\".\n"
+                "utterance": "No movies named like \"\"one\"\".\n",
+                "utterance_id": "CNV1_TEST03_17"
             },
             {
                 "intent": "REVEAL.LIST",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "GENRE",
@@ -202,20 +224,22 @@
                         "lord"
                     ],
                     [
                         "TITLE",
                         "Bright"
                     ]
                 ],
-                "utterance": "I would like to recommend you a fantasy and action, lord film named \"\"Bright\"\". Have you watched it?\n"
+                "utterance": "I would like to recommend you a fantasy and action, lord film named \"\"Bright\"\". Have you watched it?\n",
+                "utterance_id": "CNV1_MovieBotTester_18"
             },
             {
                 "intent": "COMPLETE",
                 "participant": "USER",
-                "utterance": "thank you\n"
+                "utterance": "thank you\n",
+                "utterance_id": "CNV1_TEST03_19"
             },
             {
                 "intent": "FAILED",
                 "participant": "AGENT",
                 "slot_values": [
                     [
                         "GENRE",
@@ -226,28 +250,35 @@
                         "lord"
                     ],
                     [
                         "TITLE",
                         "similar to thank you"
                     ]
                 ],
-                "utterance": "Sorry, I don't have any action, lord films named similar to thank you. Please select from the list of options to continue.\n"
+                "utterance": "Sorry, I don't have any action, lord films named similar to thank you. Please select from the list of options to continue.\n",
+                "utterance_id": "CNV1_MovieBotTester_20"
             },
             {
                 "intent": "COMPLETE",
                 "participant": "USER",
-                "utterance": "/exit\n"
+                "utterance": "/exit\n",
+                "utterance_id": "CNV1_TEST03_21"
             },
             {
                 "intent": "END",
                 "participant": "AGENT",
-                "utterance": "You are exiting. I hope you found a movie. Bye.\",\n"
+                "utterance": "You are exiting. I hope you found a movie. Bye.\",\n",
+                "utterance_id": "CNV1_MovieBotTester_22"
             }
         ],
-        "conversation ID": "\"39GHHAVOMGCMCWD43ZNZ2ARD9RF4JH\""
+        "conversation_id": "CNV1",
+        "user": {
+            "id": "TEST03",
+            "type": "USER"
+        }
     },
     {
         "conversation": [
             {
                 "intent": "DISCLOSE.NON-DISCLOSE",
                 "participant": "USER",
                 "utterance": "/start\n"
@@ -793,15 +824,15 @@
             },
             {
                 "intent": "END",
                 "participant": "AGENT",
                 "utterance": "Hope to see you soon. Bye.\n"
             }
         ],
-        "conversation ID": "\"3WOKGM4L721JEJM00BS2Y3IMR910O8\""
+        "conversation_id": "\"3WOKGM4L721JEJM00BS2Y3IMR910O8\""
     },
     {
         "conversation": [
             {
                 "intent": "DISCLOSE.NON-DISCLOSE",
                 "participant": "USER",
                 "utterance": "/start\n"
@@ -1043,10 +1074,10 @@
             },
             {
                 "intent": "END",
                 "participant": "AGENT",
                 "utterance": "Hope to see you soon. Bye.\n"
             }
         ],
-        "conversation ID": "\"3IXEICO7934U5MDNYHUI1EY03KLT65\""
+        "conversation_id": "\"3IXEICO7934U5MDNYHUI1EY03KLT65\""
     }
 ]
```

### Comparing `dialoguekit-0.0.8/tests/nlg/test_conditional_nlg.py` & `dialoguekit-0.0.9/tests/nlg/test_conditional_nlg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Test cases for NLG."""
 import json
 
 import pytest
+
 from dialoguekit.core import AnnotatedUtterance, Annotation, Intent
 from dialoguekit.nlg import ConditionalNLG
 from dialoguekit.nlg.template_from_training_data import (
     extract_utterance_template,
 )
 from dialoguekit.nlu import SatisfactionClassifierSVM
 from dialoguekit.participant import DialogueParticipant
@@ -40,16 +41,16 @@
     """
     expected_response1 = AnnotatedUtterance(
         text="something like the A Test Movie Title",
         intent=Intent("REVEAL.EXPAND"),
         participant=DialogueParticipant.AGENT,
         metadata={"satisfaction": 2},
     )
-    expected_response1.add_annotation(
-        Annotation(slot="TITLE", value="A Test Movie Title")
+    expected_response1.add_annotations(
+        [Annotation(slot="TITLE", value="A Test Movie Title")]
     )
     sample_response_text = [
         (
             Intent("REVEAL.EXPAND"),
             [Annotation(slot="TITLE", value="A Test Movie Title")],
             expected_response1,
         )
@@ -167,15 +168,15 @@
     """
     save_to_dir = tmp_path
     full_path = save_to_dir.absolute()
     my_path = full_path.as_posix()
 
     nlg_class.dump_template(filepath=f"{my_path}/nlg_dump.json")
 
-    with open(f"{my_path}/nlg_dump.json", "r") as file:
+    with open(f"{my_path}/nlg_dump.json", "r", encoding="utf-8") as file:
         json_template = json.load(file)
         assert len(json_template.keys()) == len(
             nlg_class._response_templates.keys()
         )
 
         for intent in json_template.keys():
             assert Intent(intent) in nlg_class._response_templates.keys()
```

### Comparing `dialoguekit-0.0.8/tests/nlg/test_template_from_training_data.py` & `dialoguekit-0.0.9/tests/nlg/test_template_from_training_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,21 +159,21 @@
 def test_replace_slot_with_placeholder():
     """Tests placeholder replacement."""
     # Given
     a1 = AnnotatedUtterance(
         text="I like action or fantasy movies.",
         participant=DialogueParticipant.AGENT,
     )
-    a1.add_annotation(Annotation(slot="GENRE", value="action"))
-    a1.add_annotation(Annotation(slot="GENRE", value="fantasy"))
+    a1.add_annotations([Annotation(slot="GENRE", value="action")])
+    a1.add_annotations([Annotation(slot="GENRE", value="fantasy")])
 
     a2 = AnnotatedUtterance(
         text="How about old street?", participant=DialogueParticipant.AGENT
     )
-    a2.add_annotation(Annotation(slot="TITLE", value="old street"))
+    a2.add_annotations([Annotation(slot="TITLE", value="old street")])
     annotated_utterances = [
         (a1, "I like {GENRE} or {GENRE} movies."),
         (a2, "How about {TITLE}?"),
     ]
 
     for utterance, expected_text in annotated_utterances:
         _replace_slot_with_placeholder(utterance)
```

### Comparing `dialoguekit-0.0.8/tests/nlg/test_template_nlg.py` & `dialoguekit-0.0.9/tests/nlg/test_template_nlg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Test cases for NLG."""
 import json
 
 import pytest
+
 from dialoguekit.core.annotated_utterance import AnnotatedUtterance
 from dialoguekit.core.annotation import Annotation
 from dialoguekit.core.intent import Intent
 from dialoguekit.nlg.nlg_template import TemplateNLG
 from dialoguekit.nlg.template_from_training_data import (
     extract_utterance_template,
 )
@@ -28,16 +29,16 @@
 def test_generate_utterance_text(nlg_class: TemplateNLG):
     """Tests utterance generation."""
     expected_response1 = AnnotatedUtterance(
         text="something like the A Test Movie Title",
         intent=Intent("REVEAL.EXPAND"),
         participant=DialogueParticipant.AGENT,
     )
-    expected_response1.add_annotation(
-        Annotation(slot="TITLE", value="A Test Movie Title")
+    expected_response1.add_annotations(
+        [Annotation(slot="TITLE", value="A Test Movie Title")]
     )
     sample_response_text = [
         (
             Intent("REVEAL.EXPAND"),
             [Annotation(slot="TITLE", value="A Test Movie Title")],
             expected_response1,
         )
@@ -110,15 +111,15 @@
     """Tests template export."""
     save_to_dir = tmp_path
     full_path = save_to_dir.absolute()
     my_path = full_path.as_posix()
 
     nlg_class.dump_template(filepath=f"{my_path}/nlg_dump.json")
 
-    with open(f"{my_path}/nlg_dump.json", "r") as file:
+    with open(f"{my_path}/nlg_dump.json", "r", encoding="utf-8") as file:
         json_template = json.load(file)
         assert len(json_template.keys()) == len(
             nlg_class._response_templates.keys()
         )
 
         for intent in json_template.keys():
             assert Intent(intent) in nlg_class._response_templates.keys()
```

### Comparing `dialoguekit-0.0.8/tests/nlu/test_diet_classifier_rasa.py` & `dialoguekit-0.0.9/tests/nlu/test_diet_classifier_rasa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for IntentClassifierRasa."""
 
 import pytest
+
 from dialoguekit.core import Intent, Utterance
 from dialoguekit.nlu import IntentClassifierRasa
 from dialoguekit.participant import DialogueParticipant
 
 PLACEHOLDER = "(.*)"
```

### Comparing `dialoguekit-0.0.8/tests/nlu/test_intent_classifier_cosine.py` & `dialoguekit-0.0.9/tests/nlu/test_intent_classifier_cosine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for IntentClassifierCosine."""
 
 import os
 
 import pytest
+
 from dialoguekit.core import Intent, Utterance
 from dialoguekit.nlu import IntentClassifierCosine
 from dialoguekit.participant import DialogueParticipant
 
 PLACEHOLDER = "(.*)"
```

### Comparing `dialoguekit-0.0.8/tests/nlu/test_satisfaction_classifier.py` & `dialoguekit-0.0.9/tests/nlu/test_satisfaction_classifier.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/tests/sample_agents/test_parrot_agent.py` & `dialoguekit-0.0.9/tests/sample_agents/test_parrot_agent.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,35 @@
 """Tests for ParrotAgent."""
 import io
 import sys
+from unittest.mock import patch
 
 import pytest
 
-from dialoguekit.connector.dialogue_connector import DialogueConnector
-from dialoguekit.participant.agent import AgentType
-from dialoguekit.participant.user import User, UserType
-from dialoguekit.platforms.platform import Platform
+from dialoguekit.platforms import TerminalPlatform
 from sample_agents.parrot_agent import ParrotAgent
 
 
 @pytest.fixture
-def user() -> User:
-    """User fixture."""
-    return User("TestUser", user_type=UserType.SIMULATOR)
-
-
-@pytest.fixture
-def agent() -> ParrotAgent:
-    """Parrot agent fixture."""
-    agent = ParrotAgent("TestParrotAgent")
-    assert agent.id == "TestParrotAgent"
-    assert agent._agent_type == AgentType.BOT
-    return agent
-
-
-@pytest.fixture
-def connector(user: User, agent: ParrotAgent) -> DialogueConnector:
+def platform() -> TerminalPlatform:
     """Dialogue connector fixture."""
-    connector = DialogueConnector(
-        agent, user, Platform(), save_dialogue_history=False
-    )
-    return connector
+    platform = TerminalPlatform(ParrotAgent)
+    yield platform
 
 
-def test_greetings(connector: DialogueConnector, monkeypatch) -> None:
+@patch("dialoguekit.connector.dialogue_connector.DialogueConnector.close")
+@patch("dialoguekit.platforms.Platform.disconnect")
+def test_greetings(
+    close, disconect, platform: TerminalPlatform, monkeypatch
+) -> None:
     """Test for welcome and goodbye methods."""
     monkeypatch.setattr(sys, "stdin", io.StringIO("EXIT"))
-    connector.start()
+    platform.start()
+    connector = platform.get_user("terminal_user").dialogue_connector
+
     assert len(connector.dialogue_history.utterances) == 3
     assert (
         connector.dialogue_history.utterances[0].text
         == "Hello, I'm Parrot. What can I help u with?"
     )
     assert (
         connector.dialogue_history.utterances[-1].text
```

### Comparing `dialoguekit-0.0.8/tests/user/test_user_preferences.py` & `dialoguekit-0.0.9/tests/user/test_user_preferences.py`

 * *Files identical despite different names*

### Comparing `dialoguekit-0.0.8/tests/utils/test_annotation_converter_dialoguekit_to_rasa.py` & `dialoguekit-0.0.9/tests/utils/test_annotation_converter_dialoguekit_to_rasa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for AnnotationConverterRasa."""
 
 import pytest
+
 from dialoguekit.core import Intent, Utterance
 from dialoguekit.participant import DialogueParticipant
 from dialoguekit.utils import AnnotationConverterRasa
 
 PLACEHOLDER = "(.*)"
```

### Comparing `dialoguekit-0.0.8/tests/utils/test_evaluator.py` & `dialoguekit-0.0.9/tests/utils/test_evaluator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """Tests the dialogue evaluation."""
 
+from typing import Any, Dict, List
+
 import pytest
+
+from dialoguekit.core.dialogue import Dialogue
+from dialoguekit.core.utterance import Utterance
 from dialoguekit.nlu import SatisfactionClassifierSVM
 from dialoguekit.participant import DialogueParticipant
 from dialoguekit.utils import Evaluator
 from dialoguekit.utils.dialogue_reader import json_to_dialogues
 
 
 @pytest.fixture
-def dialogues():
+def annotated_dialogues() -> List[Dialogue]:
     """Test dialogue fixture."""
     export_dialogues = json_to_dialogues(
         filepath="tests/data/annotated_dialogues.json",
-        agent_id=DialogueParticipant.AGENT,
-        user_id=DialogueParticipant.USER,
     )
     return export_dialogues
 
 
 @pytest.fixture
-def reward_config():
+def reward_config() -> Dict[str, Any]:
     """Test reward config."""
     _REWARD_CONFIG = {
         "full_set_points": 20,
         "intents": {
             "DISCLOSE": 4,
             "REVEAL.REFINE": 4,
             "INQUIRE": 4,
@@ -32,85 +35,114 @@
         "repeat_penalty": 1,
         "cost": 1,
     }
     return _REWARD_CONFIG
 
 
 @pytest.fixture
-def satisfaction_classifier():
+def satisfaction_classifier() -> SatisfactionClassifierSVM:
     """Tests satisfaction classifier init.
 
     Also used as a fixture for the tests.
     """
     return SatisfactionClassifierSVM()
 
 
-def test_init(dialogues, reward_config):
+def test_init(
+    annotated_dialogues: List[Dialogue], reward_config: Dict[str, Any]
+) -> None:
     """Tests evaluator initialization.
 
     Args:
-        dialogues: Testing dialogues.
-        reward_config: _description_
+        annotated_dialogues: Test dialogue object.
+        reward_config: Test reward config.
     """
-    Evaluator(dialogues=dialogues, reward_config=reward_config)
+    Evaluator(dialogues=annotated_dialogues, reward_config=reward_config)
 
 
-def test_avg_turns(dialogues, reward_config):
-    """Tests avg turns method.
+def test_avg_turns(
+    annotated_dialogues: List[Dialogue], reward_config: Dict[str, Any]
+) -> None:
+    """Tests avg_turns method.
 
     Args:
-        dialogues: Test dialogue object.
+        annotated_dialogues: Test dialogue object.
         reward_config: Test reward config.
     """
-    ev = Evaluator(dialogues=dialogues, reward_config=reward_config)
+    ev = Evaluator(dialogues=annotated_dialogues, reward_config=reward_config)
     avg_turns = ev.avg_turns()
     assert avg_turns == pytest.approx(16.33, 0.1)
     avg_turns2 = ev.avg_turns()
     assert avg_turns2 == pytest.approx(16.33, 0.1)
 
 
-def test_user_act_ratio(dialogues, reward_config):
+def test_user_act_ratio(
+    annotated_dialogues: List[Dialogue], reward_config: Dict[str, Any]
+) -> None:
     """Tests user action ratio method.
 
     Args:
-        dialogues: Test dialogue object.
+        annotated_dialogues: Test dialogue object.
         reward_config: Test reward config.
     """
-    ev = Evaluator(dialogues=dialogues, reward_config=reward_config)
+    ev = Evaluator(dialogues=annotated_dialogues, reward_config=reward_config)
     stats = ev.user_act_ratio()
 
     assert stats
     assert "AGENT/USER" in list(stats.keys())
     assert stats.get("USER") == 50
     assert stats.get("USER/AGENT") == pytest.approx(0.84, 0.1)
 
 
-def test_reward(dialogues, reward_config):
-    """Test reward calculation.
+def test_reward(
+    annotated_dialogues: List[Dialogue], reward_config: Dict[str, Any]
+) -> None:
+    """Tests reward calculation.
 
     Args:
-        dialogues: Test dialogue object.
+        annotated_dialogues: Test dialogue object.
         reward_config: Test reward config.
     """
-    ev = Evaluator(dialogues=dialogues, reward_config=reward_config)
+    ev = Evaluator(dialogues=annotated_dialogues, reward_config=reward_config)
     rewards = ev.reward()
-    assert len(rewards["dialogues"]) == len(dialogues)
+    assert len(rewards["dialogues"]) == len(annotated_dialogues)
     for reward in rewards["dialogues"]:
         assert reward["reward"] >= 0
 
 
+def test_reward_type_error(reward_config: Dict[str, Any]) -> None:
+    """Tests reward calculation.
+
+    Args:
+        reward_config: Test reward config.
+    """
+    dialogue = Dialogue("AGENT01", "USER01", "CNV1")
+    dialogue.add_utterance(
+        Utterance(
+            "Hello, which genres do you prefer?", DialogueParticipant.AGENT
+        )
+    )
+    dialogue.add_utterance(Utterance("Hello", DialogueParticipant.USER))
+    ev = Evaluator(dialogues=[dialogue], reward_config=reward_config)
+
+    with pytest.raises(TypeError):
+        ev.reward()
+
+
 def test_satisfaction_classification(
-    dialogues, reward_config, satisfaction_classifier
-):
+    annotated_dialogues: List[Dialogue],
+    reward_config: Dict[str, Any],
+    satisfaction_classifier: SatisfactionClassifierSVM,
+) -> None:
     """Tests satisfaction classification.
 
     Args:
-        dialogues: Test dialogue object.
+        annotated_dialogues: Test dialogue object.
         reward_config: Test reward config.
         satisfaction_classifier: Satisfaction classifier.
     """
-    ev = Evaluator(dialogues=dialogues, reward_config=reward_config)
+    ev = Evaluator(dialogues=annotated_dialogues, reward_config=reward_config)
     satisfactions = ev.satisfaction(satisfaction_classifier)
     print(satisfactions)
     assert satisfactions
     for sc in satisfactions:
         assert 1 <= sc <= 5
```

