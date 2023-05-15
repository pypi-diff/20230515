# Comparing `tmp/evals-nightly-1.0.3.dev20230513.tar.gz` & `tmp/evals-nightly-1.0.3.dev20230515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evals-nightly-1.0.3.dev20230513.tar", last modified: Sat May 13 00:13:42 2023, max compression
+gzip compressed data, was "evals-nightly-1.0.3.dev20230515.tar", last modified: Mon May 15 21:38:53 2023, max compression
```

## Comparing `evals-nightly-1.0.3.dev20230513.tar` & `evals-nightly-1.0.3.dev20230515.tar`

### file list

```diff
@@ -1,175 +1,177 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.535945 evals-nightly-1.0.3.dev20230513/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/LICENSE
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-13 00:13:42.535945 evals-nightly-1.0.3.dev20230513/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5460 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.519944 evals-nightly-1.0.3.dev20230513/evals/
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/api.py
--rw-r--r--   0 root         (0) root         (0)     1900 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.519944 evals-nightly-1.0.3.dev20230513/evals/cli/
--rw-r--r--   0 root         (0) root         (0)     5645 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/cli/oaieval.py
--rw-r--r--   0 root         (0) root         (0)     3294 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/cli/oaievalset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.519944 evals-nightly-1.0.3.dev20230513/evals/completion_fns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/completion_fns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2678 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/completion_fns/cot.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/completion_fns/langchain_llm.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/completion_fns/langchain_math.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/completion_fns/openai.py
--rw-r--r--   0 root         (0) root         (0)     4422 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/completion_fns/retrieval.py
--rw-r--r--   0 root         (0) root         (0)     5699 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.519944 evals-nightly-1.0.3.dev20230513/evals/elsuite/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.519944 evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/
--rw-r--r--   0 root         (0) root         (0)     1755 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/fuzzy_match.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/fuzzy_match_test.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/includes.py
--rw-r--r--   0 root         (0) root         (0)     1185 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/json_validator.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/match.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.519944 evals-nightly-1.0.3.dev20230513/evals/elsuite/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/modelgraded/base.py
--rw-r--r--   0 root         (0) root         (0)     4573 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/modelgraded/classify.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/modelgraded/classify_utils.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/multiple_choice.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/translate.py
--rw-r--r--   0 root         (0) root         (0)     6436 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/elsuite/utils.py
--rw-r--r--   0 root         (0) root         (0)     5534 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/eval.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/formatting.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.519944 evals-nightly-1.0.3.dev20230513/evals/prompt/
--rw-r--r--   0 root         (0) root         (0)     4093 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/prompt/base.py
--rw-r--r--   0 root         (0) root         (0)    18168 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.515944 evals-nightly-1.0.3.dev20230513/evals/registry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.523944 evals-nightly-1.0.3.dev20230513/evals/registry/completion_fns/
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/completion_fns/cot.yaml
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/completion_fns/langchain_chains.yaml
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/completion_fns/langchain_llms.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.523944 evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      560 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/test-all.yaml
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/test-modelgraded.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.535945 evals-nightly-1.0.3.dev20230513/evals/registry/evals/
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/aba-mrpc-true-false.yaml
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/actors-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/algebra-word-problems.yaml
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/anagrams.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/balance-chemical-equation.yaml
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/banking77.yaml
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/belarusian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/bigrams.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/bitwise.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/born-first.yaml
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/brazilian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/bulgarian-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/categorize_with_distractors.yaml
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/chess-piece-count.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/chess.yaml
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/compare-countries-area.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/complex-replace-characters.yaml
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/connect-4.yaml
--rw-r--r--   0 root         (0) root         (0)      335 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/convert-hex-hsl-lightness.yaml
--rw-r--r--   0 root         (0) root         (0)     1719 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/coqa-ex.yaml
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/crepe.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/cube-pack.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/decrypt-caesar-cipher.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/determinant.yaml
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/diagrammatic_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      377 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/dice-rotation-sequence.yaml
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/dutch-lexicon.yaml
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/emoji-riddle.yaml
--rw-r--r--   0 root         (0) root         (0)      387 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/emotional-intelligence.yaml
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/escher-sentences.yaml
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/fcc_amateur_extra.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/finance.yaml
--rw-r--r--   0 root         (0) root         (0)      183 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/first-letters.yaml
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/formal_logic.yaml
--rw-r--r--   0 root         (0) root         (0)      928 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/forth-stack-sim.yaml
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/greek-vocabulary.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/heart-disease.yaml
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/hebrew-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/hindi_upsc.yaml
--rw-r--r--   0 root         (0) root         (0)      265 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/illinois-law.yaml
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/imperial_date_to_string.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/infiniteloop-match.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/invoices.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/japanese-national-medical-exam01.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/japanese_driving_license.yaml
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/knot-theory.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/language.yaml
--rw-r--r--   0 root         (0) root         (0)      327 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/last-word-nth.yaml
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/lat_long_identify.yaml
--rw-r--r--   0 root         (0) root         (0)      456 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/logic-liar-paradox.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/logic-statements.yaml
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/logic.yaml
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/logiqa.yaml
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/loss-logic.yaml
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/manga-translation.yaml
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/map-electronic-component-part-to-fact.yaml
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/medmcqa.yaml
--rw-r--r--   0 root         (0) root         (0)      215 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/mendelian_inheritance.yaml
--rw-r--r--   0 root         (0) root         (0)    14586 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/mmlu.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/moral_exceptQA.yaml
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/multi-step-equations.yaml
--rw-r--r--   0 root         (0) root         (0)     1193 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/naughty_strings.yaml
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/number-pattern.yaml
--rw-r--r--   0 root         (0) root         (0)      292 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/number-reading.yaml
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/partially_solved_crossword_clues.yaml
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/pattern_identification.yaml
--rw-r--r--   0 root         (0) root         (0)      287 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/ph_calculation.yaml
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/poker_hand_ranks.yaml
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/positive-binary-operations.yaml
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/qa.yaml
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/regex-match.yaml
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/reverse-string.yaml
--rw-r--r--   0 root         (0) root         (0)      255 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/rot13.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/rucola.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/russe.yaml
--rw-r--r--   0 root         (0) root         (0)      199 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/russian-nlp-tasks.yaml
--rw-r--r--   0 root         (0) root         (0)      254 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/russian-rhyme.yaml
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/russian_medical.yaml
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/sarcasm.yaml
--rw-r--r--   0 root         (0) root         (0)      364 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/simple-knowledge-mongolian.yaml
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/sort-numeric.yaml
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/sql.yaml
--rw-r--r--   0 root         (0) root         (0)     4472 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/stock-options.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/svg_understanding.yaml
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/swedish-spelling.yaml
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/taxes.yaml
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/tempo_to_measure_count.yaml
--rw-r--r--   0 root         (0) root         (0)     1218 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-basic.yaml
--rw-r--r--   0 root         (0) root         (0)      400 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-comp-sci.yaml
--rw-r--r--   0 root         (0) root         (0)     1271 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-modelgraded-battle.yaml
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-modelgraded-generated.yaml
--rw-r--r--   0 root         (0) root         (0)     3040 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-modelgraded.yaml
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/three-pt-mapping.yaml
--rw-r--r--   0 root         (0) root         (0)      174 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/ukraine-eit.yaml
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/unified-patch.yaml
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/us-tort-law.yaml
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/utility_price_parsing.yaml
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/evals/which-is-heavier.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.535945 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/
--rw-r--r--   0 root         (0) root         (0)      492 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/battle.yaml
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/best.yaml
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/closedqa.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/diversity.yaml
--rw-r--r--   0 root         (0) root         (0)     1157 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/fact.yaml
--rw-r--r--   0 root         (0) root         (0)     2564 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/humor.yaml
--rw-r--r--   0 root         (0) root         (0)      230 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/security.yaml
--rw-r--r--   0 root         (0) root         (0)     1152 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/sql.yaml
--rw-r--r--   0 root         (0) root         (0)     9600 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.535945 evals-nightly-1.0.3.dev20230513/evals/utils/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/utils/api_utils.py
--rw-r--r--   0 root         (0) root         (0)      713 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/evals/utils/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 00:13:42.535945 evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-13 00:13:42.000000 evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6002 2023-05-13 00:13:42.000000 evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 00:13:42.000000 evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-13 00:13:42.000000 evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-05-13 00:13:42.000000 evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-13 00:13:42.000000 evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-13 00:13:40.000000 evals-nightly-1.0.3.dev20230513/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 00:13:42.535945 evals-nightly-1.0.3.dev20230513/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.767266 evals-nightly-1.0.3.dev20230515/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-15 21:38:53.763266 evals-nightly-1.0.3.dev20230515/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5460 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.747265 evals-nightly-1.0.3.dev20230515/evals/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/api.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.747265 evals-nightly-1.0.3.dev20230515/evals/cli/
+-rw-r--r--   0 root         (0) root         (0)     5645 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/cli/oaieval.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/cli/oaievalset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.747265 evals-nightly-1.0.3.dev20230515/evals/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/completion_fns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/completion_fns/cot.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/completion_fns/langchain_llm.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/completion_fns/langchain_math.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/completion_fns/openai.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/completion_fns/retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.747265 evals-nightly-1.0.3.dev20230515/evals/elsuite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.747265 evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/
+-rw-r--r--   0 root         (0) root         (0)     1755 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/fuzzy_match.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/fuzzy_match_test.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/includes.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/json_validator.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.747265 evals-nightly-1.0.3.dev20230515/evals/elsuite/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/modelgraded/base.py
+-rw-r--r--   0 root         (0) root         (0)     4573 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/modelgraded/classify.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/modelgraded/classify_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/multiple_choice.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/translate.py
+-rw-r--r--   0 root         (0) root         (0)     6436 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/elsuite/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5534 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/eval.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/formatting.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.747265 evals-nightly-1.0.3.dev20230515/evals/prompt/
+-rw-r--r--   0 root         (0) root         (0)     4093 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/prompt/base.py
+-rw-r--r--   0 root         (0) root         (0)    18168 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.743265 evals-nightly-1.0.3.dev20230515/evals/registry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.751265 evals-nightly-1.0.3.dev20230515/evals/registry/completion_fns/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/completion_fns/cot.yaml
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/completion_fns/langchain_chains.yaml
+-rw-r--r--   0 root         (0) root         (0)      524 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/completion_fns/langchain_llms.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.751265 evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      119 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      560 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      454 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/test-all.yaml
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/test-modelgraded.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.763266 evals-nightly-1.0.3.dev20230515/evals/registry/evals/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/aba-mrpc-true-false.yaml
+-rw-r--r--   0 root         (0) root         (0)      297 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/actors-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/algebra-word-problems.yaml
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/anagrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      280 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/ascii-wordart.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/balance-chemical-equation.yaml
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/banking77.yaml
+-rw-r--r--   0 root         (0) root         (0)      310 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/belarusian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/bigrams.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/bitwise.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/born-first.yaml
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/brazilian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      305 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/bulgarian-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/categorize_with_distractors.yaml
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/chess-piece-count.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/chess.yaml
+-rw-r--r--   0 root         (0) root         (0)      308 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/compare-countries-area.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/complex-replace-characters.yaml
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/connect-4.yaml
+-rw-r--r--   0 root         (0) root         (0)      335 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/convert-hex-hsl-lightness.yaml
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/coqa-ex.yaml
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/crepe.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/cube-pack.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/decrypt-caesar-cipher.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/determinant.yaml
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/diagrammatic_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      377 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/dice-rotation-sequence.yaml
+-rw-r--r--   0 root         (0) root         (0)      306 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/dutch-lexicon.yaml
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/emoji-riddle.yaml
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/emotional-intelligence.yaml
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/escher-sentences.yaml
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/event-categories.yaml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/fcc_amateur_extra.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/finance.yaml
+-rw-r--r--   0 root         (0) root         (0)      183 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/first-letters.yaml
+-rw-r--r--   0 root         (0) root         (0)      276 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/formal_logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      928 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/forth-stack-sim.yaml
+-rw-r--r--   0 root         (0) root         (0)      194 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/greek-vocabulary.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/heart-disease.yaml
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/hebrew-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      170 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/hindi_upsc.yaml
+-rw-r--r--   0 root         (0) root         (0)      265 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/illinois-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/imperial_date_to_string.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/infiniteloop-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/invoices.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/japanese-national-medical-exam01.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/japanese_driving_license.yaml
+-rw-r--r--   0 root         (0) root         (0)      382 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/job_listing_title_for_a_caregiver_in_japan.yaml
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/knot-theory.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/language.yaml
+-rw-r--r--   0 root         (0) root         (0)      327 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/last-word-nth.yaml
+-rw-r--r--   0 root         (0) root         (0)      198 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/lat_long_identify.yaml
+-rw-r--r--   0 root         (0) root         (0)      456 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/logic-liar-paradox.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/logic-statements.yaml
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/logiqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      262 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/loss-logic.yaml
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/manga-translation.yaml
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/map-electronic-component-part-to-fact.yaml
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/medmcqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      215 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/mendelian_inheritance.yaml
+-rw-r--r--   0 root         (0) root         (0)    14586 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/mmlu.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/moral_exceptQA.yaml
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/multi-step-equations.yaml
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/naughty_strings.yaml
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/number-pattern.yaml
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/number-reading.yaml
+-rw-r--r--   0 root         (0) root         (0)      258 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/partially_solved_crossword_clues.yaml
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/pattern_identification.yaml
+-rw-r--r--   0 root         (0) root         (0)      287 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/ph_calculation.yaml
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/poker_hand_ranks.yaml
+-rw-r--r--   0 root         (0) root         (0)      320 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/positive-binary-operations.yaml
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/qa.yaml
+-rw-r--r--   0 root         (0) root         (0)      175 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/regex-match.yaml
+-rw-r--r--   0 root         (0) root         (0)      378 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/reverse-string.yaml
+-rw-r--r--   0 root         (0) root         (0)      255 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/rot13.yaml
+-rw-r--r--   0 root         (0) root         (0)      236 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/rucola.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/russe.yaml
+-rw-r--r--   0 root         (0) root         (0)      199 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/russian-nlp-tasks.yaml
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/russian-rhyme.yaml
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/russian_medical.yaml
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/sarcasm.yaml
+-rw-r--r--   0 root         (0) root         (0)      364 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/simple-knowledge-mongolian.yaml
+-rw-r--r--   0 root         (0) root         (0)      374 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/sort-numeric.yaml
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/stock-options.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/svg_understanding.yaml
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/swedish-spelling.yaml
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/taxes.yaml
+-rw-r--r--   0 root         (0) root         (0)      399 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/tempo_to_measure_count.yaml
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-basic.yaml
+-rw-r--r--   0 root         (0) root         (0)      400 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-comp-sci.yaml
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-modelgraded-battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      347 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-modelgraded-generated.yaml
+-rw-r--r--   0 root         (0) root         (0)     3040 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-modelgraded.yaml
+-rw-r--r--   0 root         (0) root         (0)      323 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/three-pt-mapping.yaml
+-rw-r--r--   0 root         (0) root         (0)      174 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/ukraine-eit.yaml
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/unified-patch.yaml
+-rw-r--r--   0 root         (0) root         (0)      329 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/us-tort-law.yaml
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/utility_price_parsing.yaml
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/evals/which-is-heavier.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.763266 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/
+-rw-r--r--   0 root         (0) root         (0)      492 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/battle.yaml
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/best.yaml
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/closedqa.yaml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/diversity.yaml
+-rw-r--r--   0 root         (0) root         (0)     1157 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/fact.yaml
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/humor.yaml
+-rw-r--r--   0 root         (0) root         (0)      230 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/security.yaml
+-rw-r--r--   0 root         (0) root         (0)     1152 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/sql.yaml
+-rw-r--r--   0 root         (0) root         (0)     9600 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.763266 evals-nightly-1.0.3.dev20230515/evals/utils/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/utils/api_utils.py
+-rw-r--r--   0 root         (0) root         (0)      713 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/evals/utils/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 21:38:53.763266 evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-15 21:38:53.000000 evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6085 2023-05-15 21:38:53.000000 evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 21:38:53.000000 evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-15 21:38:53.000000 evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2023-05-15 21:38:53.000000 evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-15 21:38:53.000000 evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-15 21:38:51.000000 evals-nightly-1.0.3.dev20230515/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 21:38:53.767266 evals-nightly-1.0.3.dev20230515/setup.cfg
```

### Comparing `evals-nightly-1.0.3.dev20230513/LICENSE` & `evals-nightly-1.0.3.dev20230515/LICENSE`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/README.md` & `evals-nightly-1.0.3.dev20230515/README.md`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/api.py` & `evals-nightly-1.0.3.dev20230515/evals/api.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/base.py` & `evals-nightly-1.0.3.dev20230515/evals/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/cli/oaieval.py` & `evals-nightly-1.0.3.dev20230515/evals/cli/oaieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/cli/oaievalset.py` & `evals-nightly-1.0.3.dev20230515/evals/cli/oaievalset.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/completion_fns/cot.py` & `evals-nightly-1.0.3.dev20230515/evals/completion_fns/cot.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/completion_fns/langchain_llm.py` & `evals-nightly-1.0.3.dev20230515/evals/completion_fns/langchain_llm.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/completion_fns/langchain_math.py` & `evals-nightly-1.0.3.dev20230515/evals/completion_fns/langchain_math.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/completion_fns/openai.py` & `evals-nightly-1.0.3.dev20230515/evals/completion_fns/openai.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/completion_fns/retrieval.py` & `evals-nightly-1.0.3.dev20230515/evals/completion_fns/retrieval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/data.py` & `evals-nightly-1.0.3.dev20230515/evals/data.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/fuzzy_match.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/fuzzy_match_test.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/fuzzy_match_test.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/includes.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/includes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import Any
 
-import numpy as np
-
 import evals
 import evals.metrics
 from evals.api import CompletionFn
 from evals.elsuite import utils
 
 
 class Includes(evals.Eval):
@@ -28,17 +26,19 @@
             prompt=prompt,
         )
         sampled = result.get_completions()[0]
 
         includes_answer = any(
             [utils.get_answer(sampled, ref, self.ignore_case) for ref in sample["ideal"]]
         )
-        evals.record.record_metrics(accuracy=float(includes_answer))
+        evals.record.record_match(
+            includes_answer, expected=sample["ideal"], picked=sampled, sampled=sampled
+        )
         return includes_answer
 
     def run(self, recorder):
         samples = self.get_samples()
         self.eval_all_samples(recorder, samples)
-        events = recorder.get_scores("accuracy")
+        events = recorder.get_events("match")
         return {
-            "accuracy": np.mean(events),
+            "accuracy": evals.metrics.get_accuracy(events),
         }
```

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/json_validator.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/json_validator.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/basic/match.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/basic/match.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/modelgraded/base.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/modelgraded/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/modelgraded/classify.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/modelgraded/classify.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/modelgraded/classify_utils.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/modelgraded/classify_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/multiple_choice.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/translate.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/translate.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/elsuite/utils.py` & `evals-nightly-1.0.3.dev20230515/evals/elsuite/utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/eval.py` & `evals-nightly-1.0.3.dev20230515/evals/eval.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/formatting.py` & `evals-nightly-1.0.3.dev20230515/evals/formatting.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/metrics.py` & `evals-nightly-1.0.3.dev20230515/evals/metrics.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/prompt/base.py` & `evals-nightly-1.0.3.dev20230515/evals/prompt/base.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/record.py` & `evals-nightly-1.0.3.dev20230515/evals/record.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/completion_fns/langchain_llms.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/completion_fns/langchain_llms.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/eval_sets/stock-options.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/eval_sets/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/categorize_with_distractors.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/categorize_with_distractors.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/coqa-ex.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/coqa-ex.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/forth-stack-sim.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/forth-stack-sim.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/knot-theory.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/knot-theory.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/manga-translation.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/manga-translation.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/mmlu.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/mmlu.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/naughty_strings.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/naughty_strings.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/sql.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/stock-options.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/stock-options.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-basic.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-basic.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-modelgraded-battle.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-modelgraded-battle.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/evals/test-modelgraded.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/evals/test-modelgraded.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/closedqa.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/closedqa.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/fact.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/fact.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/humor.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/humor.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry/modelgraded/sql.yaml` & `evals-nightly-1.0.3.dev20230515/evals/registry/modelgraded/sql.yaml`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/registry.py` & `evals-nightly-1.0.3.dev20230515/evals/registry.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/utils/api_utils.py` & `evals-nightly-1.0.3.dev20230515/evals/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/utils/misc.py` & `evals-nightly-1.0.3.dev20230515/evals/utils/misc.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals/utils/snowflake.py` & `evals-nightly-1.0.3.dev20230515/evals/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `evals-nightly-1.0.3.dev20230513/evals_nightly.egg-info/SOURCES.txt` & `evals-nightly-1.0.3.dev20230515/evals_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 evals/registry/eval_sets/test-all.yaml
 evals/registry/eval_sets/test-basic.yaml
 evals/registry/eval_sets/test-modelgraded.yaml
 evals/registry/evals/aba-mrpc-true-false.yaml
 evals/registry/evals/actors-sequence.yaml
 evals/registry/evals/algebra-word-problems.yaml
 evals/registry/evals/anagrams.yaml
+evals/registry/evals/ascii-wordart.yaml
 evals/registry/evals/balance-chemical-equation.yaml
 evals/registry/evals/banking77.yaml
 evals/registry/evals/belarusian-lexicon.yaml
 evals/registry/evals/bigrams.yaml
 evals/registry/evals/bitwise.yaml
 evals/registry/evals/born-first.yaml
 evals/registry/evals/brazilian-lexicon.yaml
@@ -66,14 +67,15 @@
 evals/registry/evals/determinant.yaml
 evals/registry/evals/diagrammatic_logic.yaml
 evals/registry/evals/dice-rotation-sequence.yaml
 evals/registry/evals/dutch-lexicon.yaml
 evals/registry/evals/emoji-riddle.yaml
 evals/registry/evals/emotional-intelligence.yaml
 evals/registry/evals/escher-sentences.yaml
+evals/registry/evals/event-categories.yaml
 evals/registry/evals/fcc_amateur_extra.yaml
 evals/registry/evals/finance.yaml
 evals/registry/evals/first-letters.yaml
 evals/registry/evals/formal_logic.yaml
 evals/registry/evals/forth-stack-sim.yaml
 evals/registry/evals/greek-vocabulary.yaml
 evals/registry/evals/heart-disease.yaml
```

### Comparing `evals-nightly-1.0.3.dev20230513/pyproject.toml` & `evals-nightly-1.0.3.dev20230515/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "evals-nightly"
-version = "1.0.3.dev20230513"
+version = "1.0.3.dev20230515"
 requires-python = ">=3.9"
 dependencies = [
     "mypy",
     "openai >= 0.27.2",
     "tiktoken",
     "blobfile",
     "backoff",
```

