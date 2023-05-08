# Comparing `tmp/evals-nightly-1.0.3.dev20230505.tar.gz` & `tmp/evals-nightly-1.0.3.dev20230508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-nightly-1.0.3.dev20230505.tar", last modified: Fri May  5 22:19:37 2023, max compression
+gzip compressed data, was "evals-nightly-1.0.3.dev20230508.tar", last modified: Mon May  8 19:55:27 2023, max compression
```

## Comparing `evals-nightly-1.0.3.dev20230505.tar` & `evals-nightly-1.0.3.dev20230508.tar`

### file list

```diff
@@ -1,171 +1,174 @@
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.498798 evals-nightly-1.0.3.dev20230505/
--rw-r--r--   0 alvin      (502) staff       (20)     1063 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/LICENSE
--rw-r--r--   0 alvin      (502) staff       (20)      136 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/MANIFEST.in
--rw-r--r--   0 alvin      (502) staff       (20)      114 2023-05-05 22:19:37.498087 evals-nightly-1.0.3.dev20230505/PKG-INFO
--rw-r--r--   0 alvin      (502) staff       (20)     5239 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/README.md
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.226775 evals-nightly-1.0.3.dev20230505/evals/
--rw-r--r--   0 alvin      (502) staff       (20)      316 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/__init__.py
--rw-r--r--   0 alvin      (502) staff       (20)     2964 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/api.py
--rw-r--r--   0 alvin      (502) staff       (20)     1900 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/base.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.232867 evals-nightly-1.0.3.dev20230505/evals/cli/
--rw-r--r--   0 alvin      (502) staff       (20)     5645 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/cli/oaieval.py
--rw-r--r--   0 alvin      (502) staff       (20)     3294 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/cli/oaievalset.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.248131 evals-nightly-1.0.3.dev20230505/evals/completion_fns/
--rw-r--r--   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/completion_fns/__init__.py
--rw-r--r--   0 alvin      (502) staff       (20)     2678 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/completion_fns/cot.py
--rw-r--r--   0 alvin      (502) staff       (20)     1245 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/completion_fns/langchain_llm.py
--rw-r--r--   0 alvin      (502) staff       (20)     1068 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/completion_fns/langchain_math.py
--rw-r--r--   0 alvin      (502) staff       (20)     4941 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/completion_fns/openai.py
--rw-r--r--   0 alvin      (502) staff       (20)     4422 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/completion_fns/retrieval.py
--rw-r--r--   0 alvin      (502) staff       (20)     5699 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/data.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.253396 evals-nightly-1.0.3.dev20230505/evals/elsuite/
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.264902 evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/
--rw-r--r--   0 alvin      (502) staff       (20)     1755 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 alvin      (502) staff       (20)     1085 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/fuzzy_match_test.py
--rw-r--r--   0 alvin      (502) staff       (20)     1241 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/includes.py
--rw-r--r--   0 alvin      (502) staff       (20)     1185 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/json_validator.py
--rw-r--r--   0 alvin      (502) staff       (20)     1831 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/match.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.272954 evals-nightly-1.0.3.dev20230505/evals/elsuite/modelgraded/
--rw-r--r--   0 alvin      (502) staff       (20)      624 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/modelgraded/base.py
--rw-r--r--   0 alvin      (502) staff       (20)     4573 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 alvin      (502) staff       (20)     7590 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/modelgraded/classify_utils.py
--rw-r--r--   0 alvin      (502) staff       (20)     2682 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/translate.py
--rw-r--r--   0 alvin      (502) staff       (20)     6436 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/elsuite/utils.py
--rw-r--r--   0 alvin      (502) staff       (20)     5534 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/eval.py
--rw-r--r--   0 alvin      (502) staff       (20)     1137 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/formatting.py
--rw-r--r--   0 alvin      (502) staff       (20)     2455 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/metrics.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.275800 evals-nightly-1.0.3.dev20230505/evals/prompt/
--rw-r--r--   0 alvin      (502) staff       (20)     4093 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/prompt/base.py
--rw-r--r--   0 alvin      (502) staff       (20)    18168 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/record.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.193678 evals-nightly-1.0.3.dev20230505/evals/registry/
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.283006 evals-nightly-1.0.3.dev20230505/evals/registry/completion_fns/
--rw-r--r--   0 alvin      (502) staff       (20)      391 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/completion_fns/cot.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      103 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/completion_fns/langchain_chains.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      524 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/completion_fns/langchain_llms.yaml
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.293615 evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/
--rw-r--r--   0 alvin      (502) staff       (20)      141 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      119 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/manga-translation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      560 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/stock-options.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      454 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      113 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      312 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/test-modelgraded.yaml
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.463635 evals-nightly-1.0.3.dev20230505/evals/registry/evals/
--rw-r--r--   0 alvin      (502) staff       (20)      215 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/aba-mrpc-true-false.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      297 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/actors-sequence.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      457 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/algebra-word-problems.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      229 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/anagrams.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      230 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/balance-chemical-equation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      196 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/banking77.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      310 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/belarusian-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      159 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/bigrams.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      245 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/bitwise.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      246 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/born-first.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      288 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/brazilian-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      305 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/bulgarian-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      573 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/categorize_with_distractors.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      309 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/chess-piece-count.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      230 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/chess.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      308 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/compare-countries-area.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      250 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/complex-replace-characters.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      160 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/connect-4.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      335 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/convert-hex-hsl-lightness.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1719 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      151 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/crepe.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      167 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/cube-pack.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      214 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/decrypt-caesar-cipher.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      175 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/determinant.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      202 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/diagrammatic_logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      377 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/dice-rotation-sequence.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      306 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/dutch-lexicon.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      269 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/emoji-riddle.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      387 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/emotional-intelligence.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      195 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/escher-sentences.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      314 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/fcc_amateur_extra.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      254 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/finance.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      183 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/first-letters.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      276 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/formal_logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      928 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/forth-stack-sim.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      194 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/greek-vocabulary.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      258 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/heart-disease.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      250 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/hebrew-rhyme.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      170 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/hindi_upsc.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      265 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/illinois-law.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      222 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/imperial_date_to_string.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      347 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/infiniteloop-match.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      262 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/invoices.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      292 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/japanese-national-medical-exam01.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      329 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/japanese_driving_license.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      382 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      754 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/knot-theory.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      327 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/last-word-nth.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      198 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/lat_long_identify.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      214 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/logic-statements.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      242 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      153 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/logiqa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      262 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/loss-logic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      674 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/manga-translation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      278 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/map-electronic-component-part-to-fact.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      159 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/medmcqa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      215 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/mendelian_inheritance.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      329 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/moral_exceptQA.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      211 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/multi-step-equations.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1193 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/naughty_strings.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      186 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/number-pattern.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      292 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/number-reading.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      258 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/partially_solved_crossword_clues.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      221 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/pattern_identification.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      287 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/ph_calculation.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      188 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/poker_hand_ranks.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      320 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/positive-binary-operations.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      282 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/qa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      175 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/regex-match.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      378 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/reverse-string.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      255 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/rot13.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      236 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/rucola.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      364 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/russe.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      199 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/russian-nlp-tasks.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      254 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/russian-rhyme.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      190 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/russian_medical.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      274 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/sarcasm.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      364 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/simple-knowledge-mongolian.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      374 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/sort-numeric.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1053 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/sql.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     4472 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/stock-options.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      245 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/svg_understanding.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      272 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/swedish-spelling.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      150 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/taxes.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      399 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/tempo_to_measure_count.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1218 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      400 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-comp-sci.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1271 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      347 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-modelgraded-generated.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     3040 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-modelgraded.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      323 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/three-pt-mapping.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      174 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/ukraine-eit.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      189 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/unified-patch.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      329 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/us-tort-law.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      214 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/utility_price_parsing.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      365 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/evals/which-is-heavier.yaml
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.482099 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/
--rw-r--r--   0 alvin      (502) staff       (20)      492 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      263 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/best.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      831 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      246 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1157 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     2564 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 alvin      (502) staff       (20)      230 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/security.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     1152 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/sql.yaml
--rw-r--r--   0 alvin      (502) staff       (20)     9600 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/registry.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.490995 evals-nightly-1.0.3.dev20230505/evals/utils/
--rw-r--r--   0 alvin      (502) staff       (20)     1504 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/utils/api_utils.py
--rw-r--r--   0 alvin      (502) staff       (20)      713 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/utils/misc.py
--rw-r--r--   0 alvin      (502) staff       (20)     4076 2023-05-05 22:19:08.000000 evals-nightly-1.0.3.dev20230505/evals/utils/snowflake.py
-drwxr-xr-x   0 alvin      (502) staff       (20)        0 2023-05-05 22:19:37.497136 evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/
--rw-r--r--   0 alvin      (502) staff       (20)      114 2023-05-05 22:19:37.000000 evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/PKG-INFO
--rw-r--r--   0 alvin      (502) staff       (20)     5858 2023-05-05 22:19:37.000000 evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 alvin      (502) staff       (20)        1 2023-05-05 22:19:37.000000 evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 alvin      (502) staff       (20)       90 2023-05-05 22:19:37.000000 evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/entry_points.txt
--rw-r--r--   0 alvin      (502) staff       (20)      207 2023-05-05 22:19:37.000000 evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/requires.txt
--rw-r--r--   0 alvin      (502) staff       (20)        6 2023-05-05 22:19:37.000000 evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/top_level.txt
--rw-r--r--   0 alvin      (502) staff       (20)      566 2023-05-05 22:19:27.000000 evals-nightly-1.0.3.dev20230505/pyproject.toml
--rw-r--r--   0 alvin      (502) staff       (20)       38 2023-05-05 22:19:37.498974 evals-nightly-1.0.3.dev20230505/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.739354 evals-nightly-1.0.3.dev20230508/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-08 19:55:27.739354 evals-nightly-1.0.3.dev20230508/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5239 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.719352 evals-nightly-1.0.3.dev20230508/evals/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/api.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.719352 evals-nightly-1.0.3.dev20230508/evals/cli/
+-rw-r--r--   0 root         (0) root         (0)     5645 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/cli/oaieval.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/cli/oaievalset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.723353 evals-nightly-1.0.3.dev20230508/evals/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/completion_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/completion_fns/cot.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/completion_fns/openai.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/completion_fns/retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.723353 evals-nightly-1.0.3.dev20230508/evals/elsuite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.723353 evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/fuzzy_match_test.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/includes.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/json_validator.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.723353 evals-nightly-1.0.3.dev20230508/evals/elsuite/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/multiple_choice.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/translate.py
+-rw-r--r--   0 root         (0) root         (0)     6436 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/elsuite/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5534 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/eval.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/formatting.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.723353 evals-nightly-1.0.3.dev20230508/evals/prompt/
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/prompt/base.py
+-rw-r--r--   0 root         (0) root         (0)    18168 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.719352 evals-nightly-1.0.3.dev20230508/evals/registry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.723353 evals-nightly-1.0.3.dev20230508/evals/registry/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.723353 evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      454 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/test-modelgraded.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.735353 evals-nightly-1.0.3.dev20230508/evals/registry/evals/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/algebra-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/banking77.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/bitwise.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/categorize_with_distractors.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/chess.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/compare-countries-area.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/dice-rotation-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/dutch-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/emoji-riddle.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/escher-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/fcc_amateur_extra.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/finance.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      928 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/greek-vocabulary.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/hindi_upsc.yaml
+-rw-r--r--   0 root         (0) root         (0)      265 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/invoices.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/japanese-national-medical-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/japanese_driving_license.yaml
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/knot-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/language.yaml
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/loss-logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/medmcqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 root         (0) root         (0)    14586 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/mmlu.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/multi-step-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/ph_calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/positive-binary-operations.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/qa.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 root         (0) root         (0)      255 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 root         (0) root         (0)      236 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/russe.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/russian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/russian_medical.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/simple-knowledge-mongolian.yaml
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/sort-numeric.yaml
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/svg_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/tempo_to_measure_count.yaml
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/three-pt-mapping.yaml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/unified-patch.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/utility_price_parsing.yaml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/evals/which-is-heavier.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.739354 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)     9600 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.739354 evals-nightly-1.0.3.dev20230508/evals/utils/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/utils/api_utils.py
+-rw-r--r--   0 root         (0) root         (0)      713 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/evals/utils/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 19:55:27.739354 evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-08 19:55:27.000000 evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5957 2023-05-08 19:55:27.000000 evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 19:55:27.000000 evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-08 19:55:27.000000 evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-08 19:55:27.000000 evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-08 19:55:27.000000 evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-08 19:55:25.000000 evals-nightly-1.0.3.dev20230508/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-08 19:55:27.739354 evals-nightly-1.0.3.dev20230508/setup.cfg
```

### Comparing `evals-nightly-1.0.3.dev20230505/LICENSE` & `evals-nightly-1.0.3.dev20230508/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/README.md` & `evals-nightly-1.0.3.dev20230508/README.md`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/api.py` & `evals-nightly-1.0.3.dev20230508/evals/api.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/base.py` & `evals-nightly-1.0.3.dev20230508/evals/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/cli/oaieval.py` & `evals-nightly-1.0.3.dev20230508/evals/cli/oaieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/cli/oaievalset.py` & `evals-nightly-1.0.3.dev20230508/evals/cli/oaievalset.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/completion_fns/cot.py` & `evals-nightly-1.0.3.dev20230508/evals/completion_fns/cot.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/completion_fns/langchain_llm.py` & `evals-nightly-1.0.3.dev20230508/evals/completion_fns/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/completion_fns/langchain_math.py` & `evals-nightly-1.0.3.dev20230508/evals/completion_fns/langchain_math.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/completion_fns/openai.py` & `evals-nightly-1.0.3.dev20230508/evals/completion_fns/openai.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/completion_fns/retrieval.py` & `evals-nightly-1.0.3.dev20230508/evals/completion_fns/retrieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/data.py` & `evals-nightly-1.0.3.dev20230508/evals/data.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/fuzzy_match.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/fuzzy_match_test.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/fuzzy_match_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/includes.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/includes.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/json_validator.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/json_validator.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/basic/match.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/basic/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/modelgraded/base.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/modelgraded/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/modelgraded/classify.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/modelgraded/classify.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/modelgraded/classify_utils.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/modelgraded/classify_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/translate.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/translate.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/elsuite/utils.py` & `evals-nightly-1.0.3.dev20230508/evals/elsuite/utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/eval.py` & `evals-nightly-1.0.3.dev20230508/evals/eval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/formatting.py` & `evals-nightly-1.0.3.dev20230508/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/metrics.py` & `evals-nightly-1.0.3.dev20230508/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/prompt/base.py` & `evals-nightly-1.0.3.dev20230508/evals/prompt/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/record.py` & `evals-nightly-1.0.3.dev20230508/evals/record.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/completion_fns/langchain_llms.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/completion_fns/langchain_llms.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/eval_sets/stock-options.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/eval_sets/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/categorize_with_distractors.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/categorize_with_distractors.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/coqa-ex.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/coqa-ex.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/forth-stack-sim.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/forth-stack-sim.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/knot-theory.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/knot-theory.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/manga-translation.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/manga-translation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/naughty_strings.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/naughty_strings.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/sql.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/stock-options.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-basic.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-basic.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/evals/test-modelgraded.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/evals/test-modelgraded.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/closedqa.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/closedqa.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/fact.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/fact.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/humor.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/humor.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry/modelgraded/sql.yaml` & `evals-nightly-1.0.3.dev20230508/evals/registry/modelgraded/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/registry.py` & `evals-nightly-1.0.3.dev20230508/evals/registry.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/utils/api_utils.py` & `evals-nightly-1.0.3.dev20230508/evals/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/utils/misc.py` & `evals-nightly-1.0.3.dev20230508/evals/utils/misc.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals/utils/snowflake.py` & `evals-nightly-1.0.3.dev20230508/evals/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230505/evals_nightly.egg-info/SOURCES.txt` & `evals-nightly-1.0.3.dev20230508/evals_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 evals/cli/oaievalset.py
 evals/completion_fns/__init__.py
 evals/completion_fns/cot.py
 evals/completion_fns/langchain_llm.py
 evals/completion_fns/langchain_math.py
 evals/completion_fns/openai.py
 evals/completion_fns/retrieval.py
+evals/elsuite/multiple_choice.py
 evals/elsuite/translate.py
 evals/elsuite/utils.py
 evals/elsuite/basic/fuzzy_match.py
 evals/elsuite/basic/fuzzy_match_test.py
 evals/elsuite/basic/includes.py
 evals/elsuite/basic/json_validator.py
 evals/elsuite/basic/match.py
@@ -82,24 +83,26 @@
 evals/registry/evals/imperial_date_to_string.yaml
 evals/registry/evals/infiniteloop-match.yaml
 evals/registry/evals/invoices.yaml
 evals/registry/evals/japanese-national-medical-exam01.yaml
 evals/registry/evals/japanese_driving_license.yaml
 evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
 evals/registry/evals/knot-theory.yaml
+evals/registry/evals/language.yaml
 evals/registry/evals/last-word-nth.yaml
 evals/registry/evals/lat_long_identify.yaml
 evals/registry/evals/logic-statements.yaml
 evals/registry/evals/logic.yaml
 evals/registry/evals/logiqa.yaml
 evals/registry/evals/loss-logic.yaml
 evals/registry/evals/manga-translation.yaml
 evals/registry/evals/map-electronic-component-part-to-fact.yaml
 evals/registry/evals/medmcqa.yaml
 evals/registry/evals/mendelian_inheritance.yaml
+evals/registry/evals/mmlu.yaml
 evals/registry/evals/moral_exceptQA.yaml
 evals/registry/evals/multi-step-equations.yaml
 evals/registry/evals/naughty_strings.yaml
 evals/registry/evals/number-pattern.yaml
 evals/registry/evals/number-reading.yaml
 evals/registry/evals/partially_solved_crossword_clues.yaml
 evals/registry/evals/pattern_identification.yaml
```

### Comparing `evals-nightly-1.0.3.dev20230505/pyproject.toml` & `evals-nightly-1.0.3.dev20230508/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "evals-nightly"
-version = "1.0.3.dev20230505"
+version = "1.0.3.dev20230508"
 requires-python = ">=3.9"
 dependencies = [
     "mypy",
     "openai >= 0.27.2",
     "tiktoken",
     "blobfile",
     "backoff",
     "numpy",
     "snowflake-connector-python[pandas]",
     "pandas",
+    "datasets",
     "fire",
     "pydantic",
     "tqdm",
     "nltk",
     "filelock",
     "mock",
     "langdetect",
```

