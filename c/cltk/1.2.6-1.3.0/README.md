# Comparing `tmp/cltk-1.2.6.tar.gz` & `tmp/cltk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltk-1.2.6.tar", max compression
+gzip compressed data, was "cltk-1.3.0.tar", max compression
```

## Comparing `cltk-1.2.6.tar` & `cltk-1.3.0.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0     1083 2024-04-09 16:52:57.656163 cltk-1.2.6/LICENSE
--rw-r--r--   0        0        0     4206 2024-04-09 16:52:57.656273 cltk-1.2.6/README.rst
--rw-r--r--   0        0        0     2758 2024-05-07 15:05:00.985388 cltk-1.2.6/pyproject.toml
--rw-r--r--   0        0        0      180 2024-04-09 16:52:57.660848 cltk-1.2.6/src/cltk/__init__.py
--rw-r--r--   0        0        0       89 2024-04-09 16:52:57.660915 cltk-1.2.6/src/cltk/alphabet/__init__.py
--rw-r--r--   0        0        0      907 2024-04-09 16:52:57.660962 cltk-1.2.6/src/cltk/alphabet/ang.py
--rw-r--r--   0        0        0    10908 2024-04-09 16:52:57.661027 cltk-1.2.6/src/cltk/alphabet/arb.py
--rw-r--r--   0        0        0     5836 2024-04-09 16:52:57.661084 cltk-1.2.6/src/cltk/alphabet/arc.py
--rw-r--r--   0        0        0     3064 2024-04-09 16:52:57.661141 cltk-1.2.6/src/cltk/alphabet/ave.py
--rw-r--r--   0        0        0     1318 2024-04-09 16:52:57.661190 cltk-1.2.6/src/cltk/alphabet/ben.py
--rw-r--r--   0        0        0     2376 2024-04-09 16:52:57.661252 cltk-1.2.6/src/cltk/alphabet/egy.py
--rw-r--r--   0        0        0     3181 2024-04-09 16:52:57.661312 cltk-1.2.6/src/cltk/alphabet/enm.py
--rw-r--r--   0        0        0     2457 2024-04-09 16:52:57.661360 cltk-1.2.6/src/cltk/alphabet/fro.py
--rw-r--r--   0        0        0     3634 2024-04-09 16:52:57.661412 cltk-1.2.6/src/cltk/alphabet/gmh.py
--rw-r--r--   0        0        0      217 2024-04-09 16:52:57.661492 cltk-1.2.6/src/cltk/alphabet/grc/__init__.py
--rw-r--r--   0        0        0     4672 2024-04-09 16:52:57.661562 cltk-1.2.6/src/cltk/alphabet/grc/beta_to_unicode.py
--rw-r--r--   0        0        0     2698 2024-04-09 16:52:57.661622 cltk-1.2.6/src/cltk/alphabet/grc/cypriot.py
--rw-r--r--   0        0        0    26269 2024-04-09 16:52:57.661701 cltk-1.2.6/src/cltk/alphabet/grc/grc.py
--rw-r--r--   0        0        0     1357 2024-04-09 16:52:57.661768 cltk-1.2.6/src/cltk/alphabet/guj.py
--rw-r--r--   0        0        0     1885 2024-04-09 16:52:57.661814 cltk-1.2.6/src/cltk/alphabet/hin.py
--rw-r--r--   0        0        0     1428 2024-04-09 16:52:57.661863 cltk-1.2.6/src/cltk/alphabet/kan.py
--rw-r--r--   0        0        0    16548 2024-04-20 18:11:40.071152 cltk-1.2.6/src/cltk/alphabet/lat.py
--rw-r--r--   0        0        0     8482 2024-04-09 16:52:57.661994 cltk-1.2.6/src/cltk/alphabet/non.py
--rw-r--r--   0        0        0     1858 2024-04-09 16:52:57.662039 cltk-1.2.6/src/cltk/alphabet/omr.py
--rw-r--r--   0        0        0     2579 2024-04-09 16:52:57.662086 cltk-1.2.6/src/cltk/alphabet/ory.py
--rw-r--r--   0        0        0     1005 2024-04-09 16:52:57.662134 cltk-1.2.6/src/cltk/alphabet/osc.py
--rw-r--r--   0        0        0     5601 2024-04-09 16:52:57.662195 cltk-1.2.6/src/cltk/alphabet/ota.py
--rw-r--r--   0        0        0      694 2024-04-09 16:52:57.662243 cltk-1.2.6/src/cltk/alphabet/oty.py
--rw-r--r--   0        0        0     2620 2024-04-09 16:52:57.662287 cltk-1.2.6/src/cltk/alphabet/peo.py
--rw-r--r--   0        0        0     4561 2024-04-09 16:52:57.662343 cltk-1.2.6/src/cltk/alphabet/pes.py
--rw-r--r--   0        0        0      629 2024-04-09 16:52:57.662386 cltk-1.2.6/src/cltk/alphabet/pli.py
--rw-r--r--   0        0        0     2101 2024-04-09 16:52:57.662441 cltk-1.2.6/src/cltk/alphabet/processes.py
--rw-r--r--   0        0        0     2953 2024-04-09 16:52:57.662489 cltk-1.2.6/src/cltk/alphabet/san.py
--rw-r--r--   0        0        0      834 2024-04-09 16:52:57.662531 cltk-1.2.6/src/cltk/alphabet/tel.py
--rw-r--r--   0        0        0     4899 2024-04-20 18:11:40.071375 cltk-1.2.6/src/cltk/alphabet/text_normalization.py
--rw-r--r--   0        0        0      693 2024-04-09 16:52:57.662634 cltk-1.2.6/src/cltk/alphabet/urd.py
--rw-r--r--   0        0        0     4332 2024-04-09 16:52:57.662726 cltk-1.2.6/src/cltk/alphabet/xcl/xcl.py
--rw-r--r--   0        0        0     1404 2024-04-09 16:52:57.662767 cltk-1.2.6/src/cltk/alphabet/xlc.py
--rw-r--r--   0        0        0     1297 2024-04-09 16:52:57.662806 cltk-1.2.6/src/cltk/alphabet/xld.py
--rw-r--r--   0        0        0       54 2024-04-09 16:52:57.662867 cltk-1.2.6/src/cltk/core/__init__.py
--rw-r--r--   0        0        0      756 2024-04-09 16:52:57.662914 cltk-1.2.6/src/cltk/core/cltk_logger.py
--rw-r--r--   0        0        0    12509 2024-04-09 16:52:57.663010 cltk-1.2.6/src/cltk/core/data_types.py
--rw-r--r--   0        0        0     1766 2024-04-09 16:52:57.663075 cltk-1.2.6/src/cltk/core/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.663141 cltk-1.2.6/src/cltk/corpora/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.663204 cltk-1.2.6/src/cltk/corpora/grc/__init__.py
--rw-r--r--   0        0        0     3175 2024-04-09 16:52:57.663274 cltk-1.2.6/src/cltk/corpora/grc/tei.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.663329 cltk-1.2.6/src/cltk/corpora/grc/tlg/__init__.py
--rw-r--r--   0        0        0    30078 2024-04-09 16:52:57.663432 cltk-1.2.6/src/cltk/corpora/grc/tlg/author_date.py
--rw-r--r--   0        0        0    26927 2024-04-09 16:52:57.663523 cltk-1.2.6/src/cltk/corpora/grc/tlg/author_epithet.py
--rw-r--r--   0        0        0      336 2024-04-09 16:52:57.663583 cltk-1.2.6/src/cltk/corpora/grc/tlg/author_female.py
--rw-r--r--   0        0        0    19279 2024-04-09 16:52:57.663660 cltk-1.2.6/src/cltk/corpora/grc/tlg/author_geo.py
--rw-r--r--   0        0        0     2220 2024-04-09 16:52:57.663730 cltk-1.2.6/src/cltk/corpora/grc/tlg/file_utils.py
--rw-r--r--   0        0        0    63351 2024-04-09 16:52:57.664585 cltk-1.2.6/src/cltk/corpora/grc/tlg/id_author.py
--rw-r--r--   0        0        0     2561 2024-04-09 16:52:57.664671 cltk-1.2.6/src/cltk/corpora/grc/tlg/index_lists.py
--rw-r--r--   0        0        0     6589 2024-04-09 16:52:57.664758 cltk-1.2.6/src/cltk/corpora/grc/tlg/parse_tlg_indices.py
--rw-r--r--   0        0        0  1123425 2024-04-09 16:52:57.665244 cltk-1.2.6/src/cltk/corpora/grc/tlg/tlg_index.py
--rw-r--r--   0        0        0    13094 2024-04-09 16:52:57.665650 cltk-1.2.6/src/cltk/corpora/grc/tlg/tlgu.py
--rw-r--r--   0        0        0   332862 2024-04-09 16:52:57.666049 cltk-1.2.6/src/cltk/corpora/grc/tlg/work_numbers.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.666106 cltk-1.2.6/src/cltk/corpora/lat/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.666161 cltk-1.2.6/src/cltk/corpora/lat/phi/__init__.py
--rw-r--r--   0        0        0     3170 2024-04-09 16:52:57.666211 cltk-1.2.6/src/cltk/corpora/lat/phi/file_utils.py
--rw-r--r--   0        0        0    45693 2024-04-09 16:52:57.666293 cltk-1.2.6/src/cltk/corpora/lat/phi/phi5_index.py
--rw-r--r--   0        0        0       29 2024-04-09 16:52:57.666367 cltk-1.2.6/src/cltk/data/__init__.py
--rw-r--r--   0        0        0    30679 2024-04-09 16:52:57.666434 cltk-1.2.6/src/cltk/data/fetch.py
--rw-r--r--   0        0        0       82 2024-04-09 16:52:57.666512 cltk-1.2.6/src/cltk/dependency/__init__.py
--rw-r--r--   0        0        0    13292 2024-05-07 15:04:39.006827 cltk-1.2.6/src/cltk/dependency/processes.py
--rw-r--r--   0        0        0     6369 2024-04-09 16:52:57.666659 cltk-1.2.6/src/cltk/dependency/spacy_wrapper.py
--rw-r--r--   0        0        0    15062 2024-04-09 16:52:57.666746 cltk-1.2.6/src/cltk/dependency/stanza_wrapper.py
--rw-r--r--   0        0        0    10727 2024-04-09 16:52:57.666818 cltk-1.2.6/src/cltk/dependency/tree.py
--rw-r--r--   0        0        0     1372 2024-04-09 16:52:57.666871 cltk-1.2.6/src/cltk/dependency/utils.py
--rw-r--r--   0        0        0       88 2024-04-09 16:52:57.666942 cltk-1.2.6/src/cltk/embeddings/__init__.py
--rw-r--r--   0        0        0    22765 2024-04-09 16:52:57.667008 cltk-1.2.6/src/cltk/embeddings/embeddings.py
--rw-r--r--   0        0        0     7629 2024-04-09 16:52:57.667075 cltk-1.2.6/src/cltk/embeddings/processes.py
--rw-r--r--   0        0        0     3432 2024-04-09 16:52:57.667122 cltk-1.2.6/src/cltk/embeddings/sentence.py
--rw-r--r--   0        0        0       69 2024-04-09 16:52:57.667184 cltk-1.2.6/src/cltk/languages/__init__.py
--rw-r--r--   0        0        0    25709 2024-04-09 16:52:57.667265 cltk-1.2.6/src/cltk/languages/example_texts.py
--rw-r--r--   0        0        0    90226 2024-04-09 16:52:57.667377 cltk-1.2.6/src/cltk/languages/glottolog.py
--rw-r--r--   0        0        0    20578 2024-04-09 16:52:57.667434 cltk-1.2.6/src/cltk/languages/pipelines.py
--rw-r--r--   0        0        0     1835 2024-04-09 16:52:57.667494 cltk-1.2.6/src/cltk/languages/utils.py
--rw-r--r--   0        0        0       62 2024-04-09 16:52:57.667562 cltk-1.2.6/src/cltk/lemmatize/__init__.py
--rw-r--r--   0        0        0     3448 2024-04-09 16:52:57.667610 cltk-1.2.6/src/cltk/lemmatize/ang.py
--rw-r--r--   0        0        0    10571 2024-04-09 16:52:57.667661 cltk-1.2.6/src/cltk/lemmatize/backoff.py
--rw-r--r--   0        0        0     4478 2024-04-09 16:52:57.667718 cltk-1.2.6/src/cltk/lemmatize/fro.py
--rw-r--r--   0        0        0     4623 2024-04-09 16:52:57.667805 cltk-1.2.6/src/cltk/lemmatize/grc.py
--rwxr-xr-x   0        0        0    23414 2024-04-09 16:52:57.667853 cltk-1.2.6/src/cltk/lemmatize/lat.py
--rw-r--r--   0        0        0     4753 2024-04-09 16:52:57.667927 cltk-1.2.6/src/cltk/lemmatize/naive_lemmatizer.py
--rw-r--r--   0        0        0     5032 2024-04-09 16:52:57.667987 cltk-1.2.6/src/cltk/lemmatize/processes.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.668032 cltk-1.2.6/src/cltk/lexicon/__init__.py
--rw-r--r--   0        0        0     3439 2024-04-09 16:52:57.668085 cltk-1.2.6/src/cltk/lexicon/lat.py
--rw-r--r--   0        0        0     2949 2024-04-09 16:52:57.668137 cltk-1.2.6/src/cltk/lexicon/non.py
--rw-r--r--   0        0        0     3975 2024-04-09 16:52:57.668187 cltk-1.2.6/src/cltk/lexicon/processes.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.668228 cltk-1.2.6/src/cltk/morphology/__init__.py
--rw-r--r--   0        0        0     4919 2024-04-09 16:52:57.668290 cltk-1.2.6/src/cltk/morphology/akk.py
--rw-r--r--   0        0        0     8740 2024-04-09 16:52:57.668348 cltk-1.2.6/src/cltk/morphology/lat.py
--rw-r--r--   0        0        0    17291 2024-04-09 16:52:57.668416 cltk-1.2.6/src/cltk/morphology/morphosyntax.py
--rw-r--r--   0        0        0    13787 2024-04-09 16:52:57.668515 cltk-1.2.6/src/cltk/morphology/universal_dependencies_features.py
--rw-r--r--   0        0        0     1610 2024-04-09 16:52:57.668561 cltk-1.2.6/src/cltk/morphology/utils.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.668605 cltk-1.2.6/src/cltk/ner/__init__.py
--rw-r--r--   0        0        0     4777 2024-04-09 16:52:57.668670 cltk-1.2.6/src/cltk/ner/ner.py
--rw-r--r--   0        0        0     4555 2024-04-09 16:52:57.668722 cltk-1.2.6/src/cltk/ner/processes.py
--rw-r--r--   0        0        0     3531 2024-04-09 16:52:57.668768 cltk-1.2.6/src/cltk/ner/spacy_ner.py
--rw-r--r--   0        0        0     7143 2024-04-09 16:52:57.668824 cltk-1.2.6/src/cltk/nlp.py
--rw-r--r--   0        0        0      692 2024-04-09 16:52:57.668902 cltk-1.2.6/src/cltk/phonology/__init__.py
--rw-r--r--   0        0        0    10197 2024-04-09 16:52:57.668960 cltk-1.2.6/src/cltk/phonology/akk.py
--rw-r--r--   0        0        0       29 2024-04-09 16:52:57.669026 cltk-1.2.6/src/cltk/phonology/ang/__init__.py
--rw-r--r--   0        0        0     6119 2024-04-09 16:52:57.669103 cltk-1.2.6/src/cltk/phonology/ang/orthophonology.py
--rw-r--r--   0        0        0     1590 2024-04-09 16:52:57.669171 cltk-1.2.6/src/cltk/phonology/ang/phonology.py
--rw-r--r--   0        0        0      253 2024-04-09 16:52:57.669227 cltk-1.2.6/src/cltk/phonology/ang/syllabifier.py
--rw-r--r--   0        0        0     5877 2024-04-09 16:52:57.669303 cltk-1.2.6/src/cltk/phonology/ang/transcription.py
--rw-r--r--   0        0        0     2208 2024-04-09 16:52:57.669365 cltk-1.2.6/src/cltk/phonology/ang/transliteration.py
--rw-r--r--   0        0        0       34 2024-04-09 16:52:57.669452 cltk-1.2.6/src/cltk/phonology/arb/__init__.py
--rw-r--r--   0        0        0      380 2024-04-09 16:52:57.669505 cltk-1.2.6/src/cltk/phonology/arb/phonology.py
--rw-r--r--   0        0        0    12272 2024-04-09 16:52:57.669570 cltk-1.2.6/src/cltk/phonology/arb/romanization.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.669634 cltk-1.2.6/src/cltk/phonology/arb/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.669699 cltk-1.2.6/src/cltk/phonology/arb/utils/pyarabic/__init__.py
--rw-r--r--   0        0        0    29829 2024-04-09 16:52:57.669799 cltk-1.2.6/src/cltk/phonology/arb/utils/pyarabic/araby.py
--rw-r--r--   0        0        0      957 2024-04-09 16:52:57.669865 cltk-1.2.6/src/cltk/phonology/arb/utils/pyarabic/stack.py
--rw-r--r--   0        0        0       32 2024-04-09 16:52:57.669959 cltk-1.2.6/src/cltk/phonology/enm/__init__.py
--rw-r--r--   0        0        0      563 2024-04-09 16:52:57.670011 cltk-1.2.6/src/cltk/phonology/enm/phonology.py
--rw-r--r--   0        0        0     6825 2024-04-09 16:52:57.670136 cltk-1.2.6/src/cltk/phonology/enm/stress.py
--rw-r--r--   0        0        0     1002 2024-04-09 16:52:57.670194 cltk-1.2.6/src/cltk/phonology/enm/syllabifier.py
--rw-r--r--   0        0        0       36 2024-04-09 16:52:57.670277 cltk-1.2.6/src/cltk/phonology/gmh/__init__.py
--rw-r--r--   0        0        0     1561 2024-04-09 16:52:57.670342 cltk-1.2.6/src/cltk/phonology/gmh/phonology.py
--rw-r--r--   0        0        0     2782 2024-04-09 16:52:57.670399 cltk-1.2.6/src/cltk/phonology/gmh/syllabifier.py
--rw-r--r--   0        0        0     3661 2024-04-09 16:52:57.670469 cltk-1.2.6/src/cltk/phonology/gmh/transcription.py
--rw-r--r--   0        0        0       24 2024-04-09 16:52:57.670544 cltk-1.2.6/src/cltk/phonology/got/__init__.py
--rw-r--r--   0        0        0      944 2024-04-09 16:52:57.670597 cltk-1.2.6/src/cltk/phonology/got/phonology.py
--rw-r--r--   0        0        0     8422 2024-04-09 16:52:57.670677 cltk-1.2.6/src/cltk/phonology/got/transcription.py
--rw-r--r--   0        0        0       31 2024-04-09 16:52:57.670761 cltk-1.2.6/src/cltk/phonology/grc/__init__.py
--rw-r--r--   0        0        0     1319 2024-04-09 16:52:57.670824 cltk-1.2.6/src/cltk/phonology/grc/phonology.py
--rw-r--r--   0        0        0    19789 2024-04-09 16:52:57.670928 cltk-1.2.6/src/cltk/phonology/grc/transcription.py
--rw-r--r--   0        0        0       23 2024-04-09 16:52:57.671023 cltk-1.2.6/src/cltk/phonology/lat/__init__.py
--rw-r--r--   0        0        0     1427 2024-04-09 16:52:57.671079 cltk-1.2.6/src/cltk/phonology/lat/phonology.py
--rw-r--r--   0        0        0     8720 2024-04-09 16:52:57.671142 cltk-1.2.6/src/cltk/phonology/lat/syllabifier.py
--rw-r--r--   0        0        0    25857 2024-04-09 16:52:57.671233 cltk-1.2.6/src/cltk/phonology/lat/transcription.py
--rw-r--r--   0        0        0       27 2024-04-09 16:52:57.671333 cltk-1.2.6/src/cltk/phonology/non/__init__.py
--rw-r--r--   0        0        0       29 2024-04-09 16:52:57.671417 cltk-1.2.6/src/cltk/phonology/non/old_swedish/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-09 16:52:57.671473 cltk-1.2.6/src/cltk/phonology/non/old_swedish/phonology.py
--rw-r--r--   0        0        0     5157 2024-04-09 16:52:57.671566 cltk-1.2.6/src/cltk/phonology/non/old_swedish/transcription.py
--rw-r--r--   0        0        0     4972 2024-04-09 16:52:57.671642 cltk-1.2.6/src/cltk/phonology/non/orthophonology.py
--rw-r--r--   0        0        0     1774 2024-04-09 16:52:57.671689 cltk-1.2.6/src/cltk/phonology/non/phonology.py
--rw-r--r--   0        0        0     1359 2024-04-09 16:52:57.671745 cltk-1.2.6/src/cltk/phonology/non/syllabifier.py
--rw-r--r--   0        0        0    10883 2024-04-09 16:52:57.671809 cltk-1.2.6/src/cltk/phonology/non/transcription.py
--rw-r--r--   0        0        0    23537 2024-04-09 16:52:57.671896 cltk-1.2.6/src/cltk/phonology/non/utils.py
--rw-r--r--   0        0        0    29365 2024-04-09 16:52:57.671987 cltk-1.2.6/src/cltk/phonology/orthophonology.py
--rw-r--r--   0        0        0      137 2024-04-09 16:52:57.672050 cltk-1.2.6/src/cltk/phonology/processes.py
--rw-r--r--   0        0        0     7838 2024-04-09 16:52:57.672137 cltk-1.2.6/src/cltk/phonology/syllabifier_processes.py
--rw-r--r--   0        0        0    22653 2024-04-09 16:52:57.672222 cltk-1.2.6/src/cltk/phonology/syllabify.py
--rw-r--r--   0        0        0    11290 2024-04-09 16:52:57.672286 cltk-1.2.6/src/cltk/phonology/transcription_processes.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.672348 cltk-1.2.6/src/cltk/prosody/__init__.py
--rw-r--r--   0        0        0     1904 2024-04-09 16:52:57.672418 cltk-1.2.6/src/cltk/prosody/gmh.py
--rw-r--r--   0        0        0    15839 2024-04-20 18:11:40.071699 cltk-1.2.6/src/cltk/prosody/grc.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.672571 cltk-1.2.6/src/cltk/prosody/lat/__init__.py
--rw-r--r--   0        0        0     3275 2024-04-09 16:52:57.672640 cltk-1.2.6/src/cltk/prosody/lat/clausulae_analysis.py
--rw-r--r--   0        0        0     9435 2024-04-09 16:52:57.672738 cltk-1.2.6/src/cltk/prosody/lat/hendecasyllable_scanner.py
--rw-r--r--   0        0        0    23238 2024-04-09 16:52:57.672796 cltk-1.2.6/src/cltk/prosody/lat/hexameter_scanner.py
--rw-r--r--   0        0        0     7165 2024-04-09 16:52:57.672877 cltk-1.2.6/src/cltk/prosody/lat/macronizer.py
--rw-r--r--   0        0        0    13038 2024-04-09 16:52:57.672965 cltk-1.2.6/src/cltk/prosody/lat/metrical_validator.py
--rw-r--r--   0        0        0    11364 2024-04-09 16:52:57.673029 cltk-1.2.6/src/cltk/prosody/lat/pentameter_scanner.py
--rw-r--r--   0        0        0    22247 2024-04-09 16:52:57.673100 cltk-1.2.6/src/cltk/prosody/lat/scanner.py
--rw-r--r--   0        0        0     6892 2024-04-09 16:52:57.673191 cltk-1.2.6/src/cltk/prosody/lat/scansion_constants.py
--rw-r--r--   0        0        0     4537 2024-04-09 16:52:57.673261 cltk-1.2.6/src/cltk/prosody/lat/scansion_formatter.py
--rw-r--r--   0        0        0    11343 2024-04-09 16:52:57.673333 cltk-1.2.6/src/cltk/prosody/lat/string_utils.py
--rw-r--r--   0        0        0    16231 2024-04-09 16:52:57.673425 cltk-1.2.6/src/cltk/prosody/lat/syllabifier.py
--rw-r--r--   0        0        0     3834 2024-04-09 16:52:57.673482 cltk-1.2.6/src/cltk/prosody/lat/verse.py
--rw-r--r--   0        0        0    18010 2024-04-09 16:52:57.673555 cltk-1.2.6/src/cltk/prosody/lat/verse_scanner.py
--rw-r--r--   0        0        0    29120 2024-04-09 16:52:57.673641 cltk-1.2.6/src/cltk/prosody/non.py
--rw-r--r--   0        0        0      114 2024-04-09 16:52:57.673726 cltk-1.2.6/src/cltk/sentence/__init__.py
--rw-r--r--   0        0        0     1204 2024-04-09 16:52:57.673780 cltk-1.2.6/src/cltk/sentence/grc.py
--rw-r--r--   0        0        0     2165 2024-04-09 16:52:57.673831 cltk-1.2.6/src/cltk/sentence/lat.py
--rw-r--r--   0        0        0     1013 2024-04-09 16:52:57.673879 cltk-1.2.6/src/cltk/sentence/non.py
--rw-r--r--   0        0        0     2992 2024-04-09 16:52:57.673928 cltk-1.2.6/src/cltk/sentence/processes.py
--rw-r--r--   0        0        0     1024 2024-04-09 16:52:57.673977 cltk-1.2.6/src/cltk/sentence/san.py
--rw-r--r--   0        0        0     4051 2024-04-09 16:52:57.674033 cltk-1.2.6/src/cltk/sentence/sentence.py
--rw-r--r--   0        0        0       61 2024-04-09 16:52:57.674105 cltk-1.2.6/src/cltk/stem/__init__.py
--rw-r--r--   0        0        0     2326 2024-04-09 16:52:57.674156 cltk-1.2.6/src/cltk/stem/akk.py
--rw-r--r--   0        0        0     4288 2024-04-09 16:52:57.674226 cltk-1.2.6/src/cltk/stem/enm.py
--rw-r--r--   0        0        0     4241 2024-04-09 16:52:57.674285 cltk-1.2.6/src/cltk/stem/fro.py
--rw-r--r--   0        0        0     3523 2024-04-09 16:52:57.674349 cltk-1.2.6/src/cltk/stem/gmh.py
--rw-r--r--   0        0        0     4559 2024-04-09 16:52:57.674408 cltk-1.2.6/src/cltk/stem/lat.py
--rw-r--r--   0        0        0     4550 2024-04-09 16:52:57.674474 cltk-1.2.6/src/cltk/stem/processes.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.674533 cltk-1.2.6/src/cltk/stops/__init__.py
--rw-r--r--   0        0        0      437 2024-04-09 16:52:57.674596 cltk-1.2.6/src/cltk/stops/akk.py
--rw-r--r--   0        0        0     3148 2024-04-09 16:52:57.674649 cltk-1.2.6/src/cltk/stops/ang.py
--rw-r--r--   0        0        0     3994 2024-04-09 16:52:57.674706 cltk-1.2.6/src/cltk/stops/arb.py
--rw-r--r--   0        0        0    16649 2024-04-09 16:52:57.674767 cltk-1.2.6/src/cltk/stops/cop.py
--rw-r--r--   0        0        0     3711 2024-04-09 16:52:57.674829 cltk-1.2.6/src/cltk/stops/enm.py
--rw-r--r--   0        0        0     3302 2024-04-09 16:52:57.674886 cltk-1.2.6/src/cltk/stops/fro.py
--rw-r--r--   0        0        0     2866 2024-04-09 16:52:57.674937 cltk-1.2.6/src/cltk/stops/gmh.py
--rw-r--r--   0        0        0     2384 2024-04-09 16:52:57.674988 cltk-1.2.6/src/cltk/stops/grc.py
--rw-r--r--   0        0        0     2772 2024-04-09 16:52:57.675037 cltk-1.2.6/src/cltk/stops/hin.py
--rw-r--r--   0        0        0     1377 2024-04-09 16:52:57.675083 cltk-1.2.6/src/cltk/stops/lat.py
--rw-r--r--   0        0        0     1583 2024-04-09 16:52:57.675133 cltk-1.2.6/src/cltk/stops/non.py
--rw-r--r--   0        0        0     1928 2024-04-09 16:52:57.675185 cltk-1.2.6/src/cltk/stops/omr.py
--rw-r--r--   0        0        0     6575 2024-04-09 16:52:57.675247 cltk-1.2.6/src/cltk/stops/pan.py
--rw-r--r--   0        0        0     1524 2024-04-09 16:52:57.675302 cltk-1.2.6/src/cltk/stops/processes.py
--rw-r--r--   0        0        0    23641 2024-04-09 16:52:57.675361 cltk-1.2.6/src/cltk/stops/san.py
--rw-r--r--   0        0        0     2005 2024-04-09 16:52:57.675423 cltk-1.2.6/src/cltk/stops/words.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.675477 cltk-1.2.6/src/cltk/tag/__init__.py
--rw-r--r--   0        0        0     4422 2024-04-09 16:52:57.675548 cltk-1.2.6/src/cltk/tag/ner.py
--rw-r--r--   0        0        0     6188 2024-04-09 16:52:57.675608 cltk-1.2.6/src/cltk/tag/pos.py
--rw-r--r--   0        0        0     1796 2024-04-09 16:52:57.675669 cltk-1.2.6/src/cltk/tag/treebanks.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.675730 cltk-1.2.6/src/cltk/text/__init__.py
--rw-r--r--   0        0        0     4243 2024-04-09 16:52:57.675803 cltk-1.2.6/src/cltk/text/akk.py
--rw-r--r--   0        0        0      624 2024-04-09 16:52:57.675854 cltk-1.2.6/src/cltk/text/lat.py
--rw-r--r--   0        0        0      627 2024-04-09 16:52:57.675911 cltk-1.2.6/src/cltk/text/non.py
--rw-r--r--   0        0        0     1499 2024-04-09 16:52:57.675956 cltk-1.2.6/src/cltk/text/processes.py
--rw-r--r--   0        0        0       58 2024-04-09 16:52:57.676022 cltk-1.2.6/src/cltk/tokenizers/__init__.py
--rw-r--r--   0        0        0     5872 2024-04-09 16:52:57.676080 cltk-1.2.6/src/cltk/tokenizers/akk.py
--rw-r--r--   0        0        0      593 2024-04-09 16:52:57.676130 cltk-1.2.6/src/cltk/tokenizers/arb.py
--rw-r--r--   0        0        0      600 2024-04-09 16:52:57.676174 cltk-1.2.6/src/cltk/tokenizers/enm.py
--rw-r--r--   0        0        0      560 2024-04-09 16:52:57.676220 cltk-1.2.6/src/cltk/tokenizers/fro.py
--rw-r--r--   0        0        0      727 2024-04-09 16:52:57.676269 cltk-1.2.6/src/cltk/tokenizers/gmh.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.676310 cltk-1.2.6/src/cltk/tokenizers/lat/__init__.py
--rw-r--r--   0        0        0     7014 2024-04-09 16:52:57.676380 cltk-1.2.6/src/cltk/tokenizers/lat/lat.py
--rw-r--r--   0        0        0    12346 2024-04-09 16:52:57.676471 cltk-1.2.6/src/cltk/tokenizers/lat/params.py
--rw-r--r--   0        0        0      916 2024-04-09 16:52:57.676519 cltk-1.2.6/src/cltk/tokenizers/lat/utils.py
--rw-r--r--   0        0        0     1455 2024-04-09 16:52:57.676575 cltk-1.2.6/src/cltk/tokenizers/line.py
--rw-r--r--   0        0        0      627 2024-04-09 16:52:57.676628 cltk-1.2.6/src/cltk/tokenizers/non.py
--rw-r--r--   0        0        0     8655 2024-04-09 16:52:57.676685 cltk-1.2.6/src/cltk/tokenizers/processes.py
--rw-r--r--   0        0        0     2608 2024-04-09 16:52:57.676741 cltk-1.2.6/src/cltk/tokenizers/utils.py
--rw-r--r--   0        0        0     3541 2024-04-09 16:52:57.676799 cltk-1.2.6/src/cltk/tokenizers/word.py
--rw-r--r--   0        0        0       51 2024-04-09 16:52:57.676877 cltk-1.2.6/src/cltk/utils/__init__.py
--rw-r--r--   0        0        0     4518 2024-04-09 16:52:57.676941 cltk-1.2.6/src/cltk/utils/feature_extraction.py
--rw-r--r--   0        0        0     2322 2024-04-09 16:52:57.676994 cltk-1.2.6/src/cltk/utils/file_operations.py
--rw-r--r--   0        0        0     8816 2024-04-09 16:52:57.677053 cltk-1.2.6/src/cltk/utils/utils.py
--rw-r--r--   0        0        0        0 2024-04-09 16:52:57.677093 cltk-1.2.6/src/cltk/wordnet/__init__.py
--rw-r--r--   0        0        0     1388 2024-04-09 16:52:57.677146 cltk-1.2.6/src/cltk/wordnet/processes.py
--rw-r--r--   0        0        0    94460 2024-04-09 16:52:57.677284 cltk-1.2.6/src/cltk/wordnet/wordnet.py
--rw-r--r--   0        0        0     6134 1970-01-01 00:00:00.000000 cltk-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-09-03 15:20:38.550927 cltk-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4206 2023-12-27 18:07:36.188471 cltk-1.3.0/README.rst
+-rw-r--r--   0        0        0     2758 2024-05-12 22:59:56.695453 cltk-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-04-22 21:15:17.487258 cltk-1.3.0/src/cltk/__init__.py
+-rw-r--r--   0        0        0       89 2023-09-03 15:20:38.554927 cltk-1.3.0/src/cltk/alphabet/__init__.py
+-rw-r--r--   0        0        0      907 2023-09-03 15:20:38.554927 cltk-1.3.0/src/cltk/alphabet/ang.py
+-rw-r--r--   0        0        0    10908 2023-09-03 15:20:38.554927 cltk-1.3.0/src/cltk/alphabet/arb.py
+-rw-r--r--   0        0        0     5836 2024-04-22 21:15:17.487258 cltk-1.3.0/src/cltk/alphabet/arc.py
+-rw-r--r--   0        0        0     3064 2023-09-03 15:20:38.554927 cltk-1.3.0/src/cltk/alphabet/ave.py
+-rw-r--r--   0        0        0     1318 2023-09-03 15:20:38.554927 cltk-1.3.0/src/cltk/alphabet/ben.py
+-rw-r--r--   0        0        0     2376 2023-09-03 15:20:38.554927 cltk-1.3.0/src/cltk/alphabet/egy.py
+-rw-r--r--   0        0        0     3181 2023-09-03 15:20:38.554927 cltk-1.3.0/src/cltk/alphabet/enm.py
+-rw-r--r--   0        0        0     2457 2024-04-22 21:15:17.487258 cltk-1.3.0/src/cltk/alphabet/fro.py
+-rw-r--r--   0        0        0     3634 2024-04-22 21:15:17.487258 cltk-1.3.0/src/cltk/alphabet/gmh.py
+-rw-r--r--   0        0        0      217 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/grc/__init__.py
+-rw-r--r--   0        0        0     4672 2024-04-22 21:15:17.487258 cltk-1.3.0/src/cltk/alphabet/grc/beta_to_unicode.py
+-rw-r--r--   0        0        0     2698 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/grc/cypriot.py
+-rw-r--r--   0        0        0    26269 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/alphabet/grc/grc.py
+-rw-r--r--   0        0        0     1357 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/guj.py
+-rw-r--r--   0        0        0     1885 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/hin.py
+-rw-r--r--   0        0        0     1428 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/kan.py
+-rw-r--r--   0        0        0    16548 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/alphabet/lat.py
+-rw-r--r--   0        0        0     8482 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/non.py
+-rw-r--r--   0        0        0     1858 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/omr.py
+-rw-r--r--   0        0        0     2579 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/ory.py
+-rw-r--r--   0        0        0     1005 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/osc.py
+-rw-r--r--   0        0        0     5601 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/ota.py
+-rw-r--r--   0        0        0      694 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/oty.py
+-rw-r--r--   0        0        0     2620 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/peo.py
+-rw-r--r--   0        0        0     4561 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/alphabet/pes.py
+-rw-r--r--   0        0        0      629 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/pli.py
+-rw-r--r--   0        0        0     2101 2023-12-27 18:07:36.236471 cltk-1.3.0/src/cltk/alphabet/processes.py
+-rw-r--r--   0        0        0     2953 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/san.py
+-rw-r--r--   0        0        0      834 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/tel.py
+-rw-r--r--   0        0        0     4899 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/alphabet/text_normalization.py
+-rw-r--r--   0        0        0      693 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/urd.py
+-rw-r--r--   0        0        0     4332 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/xcl/xcl.py
+-rw-r--r--   0        0        0     1404 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/xlc.py
+-rw-r--r--   0        0        0     1297 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/alphabet/xld.py
+-rw-r--r--   0        0        0       54 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/core/__init__.py
+-rw-r--r--   0        0        0      756 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/core/cltk_logger.py
+-rw-r--r--   0        0        0    12509 2024-05-12 21:55:06.122767 cltk-1.3.0/src/cltk/core/data_types.py
+-rw-r--r--   0        0        0     1766 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/core/exceptions.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/corpora/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/corpora/grc/__init__.py
+-rw-r--r--   0        0        0     3175 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/corpora/grc/tei.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.558927 cltk-1.3.0/src/cltk/corpora/grc/tlg/__init__.py
+-rw-r--r--   0        0        0    30078 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/corpora/grc/tlg/author_date.py
+-rw-r--r--   0        0        0    26927 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/corpora/grc/tlg/author_epithet.py
+-rw-r--r--   0        0        0      336 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/corpora/grc/tlg/author_female.py
+-rw-r--r--   0        0        0    19279 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/corpora/grc/tlg/author_geo.py
+-rw-r--r--   0        0        0     2220 2024-04-22 21:15:17.499258 cltk-1.3.0/src/cltk/corpora/grc/tlg/file_utils.py
+-rw-r--r--   0        0        0    63351 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/grc/tlg/id_author.py
+-rw-r--r--   0        0        0     2561 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/grc/tlg/index_lists.py
+-rw-r--r--   0        0        0     6589 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/grc/tlg/parse_tlg_indices.py
+-rw-r--r--   0        0        0  1123425 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/grc/tlg/tlg_index.py
+-rw-r--r--   0        0        0    13094 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/grc/tlg/tlgu.py
+-rw-r--r--   0        0        0   332862 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/grc/tlg/work_numbers.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/corpora/lat/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/corpora/lat/phi/__init__.py
+-rw-r--r--   0        0        0     3170 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/lat/phi/file_utils.py
+-rw-r--r--   0        0        0    45693 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/corpora/lat/phi/phi5_index.py
+-rw-r--r--   0        0        0       29 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/data/__init__.py
+-rw-r--r--   0        0        0    30679 2024-04-22 21:15:17.503259 cltk-1.3.0/src/cltk/data/fetch.py
+-rw-r--r--   0        0        0       82 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/dependency/__init__.py
+-rw-r--r--   0        0        0    13724 2024-05-12 22:59:56.695453 cltk-1.3.0/src/cltk/dependency/processes.py
+-rw-r--r--   0        0        0     6901 2024-05-12 22:59:56.699453 cltk-1.3.0/src/cltk/dependency/spacy_wrapper.py
+-rw-r--r--   0        0        0    15062 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/dependency/stanza_wrapper.py
+-rw-r--r--   0        0        0    10727 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/dependency/tree.py
+-rw-r--r--   0        0        0     1372 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/dependency/utils.py
+-rw-r--r--   0        0        0       88 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/embeddings/__init__.py
+-rw-r--r--   0        0        0    22765 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/embeddings/embeddings.py
+-rw-r--r--   0        0        0     7629 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/embeddings/processes.py
+-rw-r--r--   0        0        0     3432 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/embeddings/sentence.py
+-rw-r--r--   0        0        0       69 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/languages/__init__.py
+-rw-r--r--   0        0        0    25709 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/languages/example_texts.py
+-rw-r--r--   0        0        0    90226 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/languages/glottolog.py
+-rw-r--r--   0        0        0    20633 2024-05-12 22:59:56.699453 cltk-1.3.0/src/cltk/languages/pipelines.py
+-rw-r--r--   0        0        0     1835 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/languages/utils.py
+-rw-r--r--   0        0        0       62 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/lemmatize/__init__.py
+-rw-r--r--   0        0        0     3448 2023-09-03 15:20:38.574926 cltk-1.3.0/src/cltk/lemmatize/ang.py
+-rw-r--r--   0        0        0    10571 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lemmatize/backoff.py
+-rw-r--r--   0        0        0     4478 2023-12-27 18:06:43.024284 cltk-1.3.0/src/cltk/lemmatize/fro.py
+-rw-r--r--   0        0        0     4623 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lemmatize/grc.py
+-rwxr-xr-x   0        0        0    23414 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lemmatize/lat.py
+-rw-r--r--   0        0        0     4753 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lemmatize/naive_lemmatizer.py
+-rw-r--r--   0        0        0     5032 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lemmatize/processes.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/lexicon/__init__.py
+-rw-r--r--   0        0        0     3439 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lexicon/lat.py
+-rw-r--r--   0        0        0     2949 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lexicon/non.py
+-rw-r--r--   0        0        0     3975 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/lexicon/processes.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/morphology/__init__.py
+-rw-r--r--   0        0        0     4919 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/morphology/akk.py
+-rw-r--r--   0        0        0     8740 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/morphology/lat.py
+-rw-r--r--   0        0        0    17291 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/morphology/morphosyntax.py
+-rw-r--r--   0        0        0    13787 2023-12-27 18:06:43.076284 cltk-1.3.0/src/cltk/morphology/universal_dependencies_features.py
+-rw-r--r--   0        0        0     1610 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/morphology/utils.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/ner/__init__.py
+-rw-r--r--   0        0        0     4777 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/ner/ner.py
+-rw-r--r--   0        0        0     4555 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/ner/processes.py
+-rw-r--r--   0        0        0     3531 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/ner/spacy_ner.py
+-rw-r--r--   0        0        0     7143 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/nlp.py
+-rw-r--r--   0        0        0      692 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/__init__.py
+-rw-r--r--   0        0        0    10197 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/akk.py
+-rw-r--r--   0        0        0       29 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/ang/__init__.py
+-rw-r--r--   0        0        0     6119 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/ang/orthophonology.py
+-rw-r--r--   0        0        0     1590 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/ang/phonology.py
+-rw-r--r--   0        0        0      253 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/ang/syllabifier.py
+-rw-r--r--   0        0        0     5877 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/ang/transcription.py
+-rw-r--r--   0        0        0     2208 2023-12-27 18:07:36.264471 cltk-1.3.0/src/cltk/phonology/ang/transliteration.py
+-rw-r--r--   0        0        0       34 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/arb/__init__.py
+-rw-r--r--   0        0        0      380 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/arb/phonology.py
+-rw-r--r--   0        0        0    12272 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/arb/romanization.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/arb/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/arb/utils/pyarabic/__init__.py
+-rw-r--r--   0        0        0    29829 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/arb/utils/pyarabic/araby.py
+-rw-r--r--   0        0        0      957 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/arb/utils/pyarabic/stack.py
+-rw-r--r--   0        0        0       32 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/enm/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/enm/phonology.py
+-rw-r--r--   0        0        0     6825 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/enm/stress.py
+-rw-r--r--   0        0        0     1002 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/enm/syllabifier.py
+-rw-r--r--   0        0        0       36 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/gmh/__init__.py
+-rw-r--r--   0        0        0     1561 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/gmh/phonology.py
+-rw-r--r--   0        0        0     2782 2023-11-10 21:51:02.940430 cltk-1.3.0/src/cltk/phonology/gmh/syllabifier.py
+-rw-r--r--   0        0        0     3661 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/gmh/transcription.py
+-rw-r--r--   0        0        0       24 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/got/__init__.py
+-rw-r--r--   0        0        0      944 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/got/phonology.py
+-rw-r--r--   0        0        0     8422 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/got/transcription.py
+-rw-r--r--   0        0        0       31 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/grc/__init__.py
+-rw-r--r--   0        0        0     1319 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/grc/phonology.py
+-rw-r--r--   0        0        0    19789 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/grc/transcription.py
+-rw-r--r--   0        0        0       23 2023-09-03 15:20:38.578926 cltk-1.3.0/src/cltk/phonology/lat/__init__.py
+-rw-r--r--   0        0        0     1427 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/lat/phonology.py
+-rw-r--r--   0        0        0     8720 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/lat/syllabifier.py
+-rw-r--r--   0        0        0    25857 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/lat/transcription.py
+-rw-r--r--   0        0        0       27 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/non/__init__.py
+-rw-r--r--   0        0        0       29 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/non/old_swedish/__init__.py
+-rw-r--r--   0        0        0     1256 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/non/old_swedish/phonology.py
+-rw-r--r--   0        0        0     5157 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/non/old_swedish/transcription.py
+-rw-r--r--   0        0        0     4972 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/non/orthophonology.py
+-rw-r--r--   0        0        0     1774 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/non/phonology.py
+-rw-r--r--   0        0        0     1359 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/non/syllabifier.py
+-rw-r--r--   0        0        0    10883 2023-11-10 21:51:03.160432 cltk-1.3.0/src/cltk/phonology/non/transcription.py
+-rw-r--r--   0        0        0    23537 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/non/utils.py
+-rw-r--r--   0        0        0    29365 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/orthophonology.py
+-rw-r--r--   0        0        0      137 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/phonology/processes.py
+-rw-r--r--   0        0        0     7838 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/syllabifier_processes.py
+-rw-r--r--   0        0        0    22653 2024-04-22 21:15:17.507259 cltk-1.3.0/src/cltk/phonology/syllabify.py
+-rw-r--r--   0        0        0    11290 2024-04-22 21:15:17.519259 cltk-1.3.0/src/cltk/phonology/transcription_processes.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/prosody/__init__.py
+-rw-r--r--   0        0        0     1904 2023-12-27 18:07:36.272471 cltk-1.3.0/src/cltk/prosody/gmh.py
+-rw-r--r--   0        0        0    15839 2024-04-22 21:15:17.519259 cltk-1.3.0/src/cltk/prosody/grc.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/prosody/lat/__init__.py
+-rw-r--r--   0        0        0     3275 2024-04-22 21:15:17.519259 cltk-1.3.0/src/cltk/prosody/lat/clausulae_analysis.py
+-rw-r--r--   0        0        0     9435 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/prosody/lat/hendecasyllable_scanner.py
+-rw-r--r--   0        0        0    23238 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/prosody/lat/hexameter_scanner.py
+-rw-r--r--   0        0        0     7165 2024-04-22 21:15:17.519259 cltk-1.3.0/src/cltk/prosody/lat/macronizer.py
+-rw-r--r--   0        0        0    13038 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/prosody/lat/metrical_validator.py
+-rw-r--r--   0        0        0    11364 2023-12-27 18:07:36.276471 cltk-1.3.0/src/cltk/prosody/lat/pentameter_scanner.py
+-rw-r--r--   0        0        0    22247 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/prosody/lat/scanner.py
+-rw-r--r--   0        0        0     6892 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/prosody/lat/scansion_constants.py
+-rw-r--r--   0        0        0     4537 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/prosody/lat/scansion_formatter.py
+-rw-r--r--   0        0        0    11343 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/prosody/lat/string_utils.py
+-rw-r--r--   0        0        0    16231 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/prosody/lat/syllabifier.py
+-rw-r--r--   0        0        0     3834 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/prosody/lat/verse.py
+-rw-r--r--   0        0        0    18010 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/prosody/lat/verse_scanner.py
+-rw-r--r--   0        0        0    29120 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/prosody/non.py
+-rw-r--r--   0        0        0      114 2023-11-10 21:51:02.940430 cltk-1.3.0/src/cltk/sentence/__init__.py
+-rw-r--r--   0        0        0     1204 2023-12-27 18:06:43.104284 cltk-1.3.0/src/cltk/sentence/grc.py
+-rw-r--r--   0        0        0     2165 2023-12-27 18:06:43.104284 cltk-1.3.0/src/cltk/sentence/lat.py
+-rw-r--r--   0        0        0     1013 2023-12-27 18:06:43.104284 cltk-1.3.0/src/cltk/sentence/non.py
+-rw-r--r--   0        0        0     2992 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/sentence/processes.py
+-rw-r--r--   0        0        0     1024 2023-12-27 18:06:43.104284 cltk-1.3.0/src/cltk/sentence/san.py
+-rw-r--r--   0        0        0     4051 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/sentence/sentence.py
+-rw-r--r--   0        0        0       61 2023-09-03 15:20:38.582926 cltk-1.3.0/src/cltk/stem/__init__.py
+-rw-r--r--   0        0        0     2326 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stem/akk.py
+-rw-r--r--   0        0        0     4288 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stem/enm.py
+-rw-r--r--   0        0        0     4241 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stem/fro.py
+-rw-r--r--   0        0        0     3523 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stem/gmh.py
+-rw-r--r--   0        0        0     4559 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stem/lat.py
+-rw-r--r--   0        0        0     4550 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stem/processes.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/stops/__init__.py
+-rw-r--r--   0        0        0      437 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/akk.py
+-rw-r--r--   0        0        0     3148 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/ang.py
+-rw-r--r--   0        0        0     3994 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/arb.py
+-rw-r--r--   0        0        0    16649 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/cop.py
+-rw-r--r--   0        0        0     3711 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/enm.py
+-rw-r--r--   0        0        0     3302 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/fro.py
+-rw-r--r--   0        0        0     2866 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/gmh.py
+-rw-r--r--   0        0        0     2384 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/grc.py
+-rw-r--r--   0        0        0     2772 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/hin.py
+-rw-r--r--   0        0        0     1377 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/lat.py
+-rw-r--r--   0        0        0     1583 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/non.py
+-rw-r--r--   0        0        0     1928 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/omr.py
+-rw-r--r--   0        0        0     6575 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/pan.py
+-rw-r--r--   0        0        0     1524 2024-04-22 21:15:17.527259 cltk-1.3.0/src/cltk/stops/processes.py
+-rw-r--r--   0        0        0    23641 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/stops/san.py
+-rw-r--r--   0        0        0     2005 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/stops/words.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tag/__init__.py
+-rw-r--r--   0        0        0     4422 2023-12-27 18:07:36.276471 cltk-1.3.0/src/cltk/tag/ner.py
+-rw-r--r--   0        0        0     6188 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tag/pos.py
+-rw-r--r--   0        0        0     1796 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tag/treebanks.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/text/__init__.py
+-rw-r--r--   0        0        0     4243 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/text/akk.py
+-rw-r--r--   0        0        0      624 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/text/lat.py
+-rw-r--r--   0        0        0      627 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/text/non.py
+-rw-r--r--   0        0        0     1499 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/text/processes.py
+-rw-r--r--   0        0        0       58 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/__init__.py
+-rw-r--r--   0        0        0     5872 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/akk.py
+-rw-r--r--   0        0        0      593 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/arb.py
+-rw-r--r--   0        0        0      600 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/enm.py
+-rw-r--r--   0        0        0      560 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/fro.py
+-rw-r--r--   0        0        0      727 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/gmh.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/lat/__init__.py
+-rw-r--r--   0        0        0     7014 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/tokenizers/lat/lat.py
+-rw-r--r--   0        0        0    12346 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/tokenizers/lat/params.py
+-rw-r--r--   0        0        0      916 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/tokenizers/lat/utils.py
+-rw-r--r--   0        0        0     1455 2023-12-27 18:06:43.104284 cltk-1.3.0/src/cltk/tokenizers/line.py
+-rw-r--r--   0        0        0      627 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/tokenizers/non.py
+-rw-r--r--   0        0        0     8655 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/tokenizers/processes.py
+-rw-r--r--   0        0        0     2608 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/tokenizers/utils.py
+-rw-r--r--   0        0        0     3541 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/tokenizers/word.py
+-rw-r--r--   0        0        0       51 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/utils/__init__.py
+-rw-r--r--   0        0        0     4518 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/utils/feature_extraction.py
+-rw-r--r--   0        0        0     2322 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/utils/file_operations.py
+-rw-r--r--   0        0        0     8816 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-09-03 15:20:38.586926 cltk-1.3.0/src/cltk/wordnet/__init__.py
+-rw-r--r--   0        0        0     1388 2024-04-22 21:15:17.531259 cltk-1.3.0/src/cltk/wordnet/processes.py
+-rw-r--r--   0        0        0    94460 2023-12-27 18:07:36.276471 cltk-1.3.0/src/cltk/wordnet/wordnet.py
+-rw-r--r--   0        0        0     6134 1970-01-01 00:00:00.000000 cltk-1.3.0/PKG-INFO
```

### Comparing `cltk-1.2.6/LICENSE` & `cltk-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/README.rst` & `cltk-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/pyproject.toml` & `cltk-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cltk"
-version = "1.2.6"
+version = "1.3.0"
 description = "The Classical Language Toolkit"
 license = "MIT"
 authors = ["Kyle P. Johnson <kyle@kyle-p-johnson.com>", "Patrick J. Burns <patrick@diyclassics.org>", "John Stewart <johnstewart@aya.yale.edu>", "Todd Cook <todd.g.cook@gmail.com>", "Clément Besnier <clem@clementbesnier.fr>", "William J. B. Mattingly <https://github.com/wjbmattingly>"]
 readme = "README.rst"
 homepage = "http://cltk.org"
 repository = "https://github.com/cltk/cltk"
 documentation = "https://cltk.readthedocs.io/en/latest/"
@@ -44,15 +44,15 @@
 gensim = "^4.3.2"
 boltons = "^21.0.0"
 greek-accentuation = "^1.2.0"
 rapidfuzz = "^3.4.0"
 stanza = "^1.6.0"
 nltk = "^3.7"
 stringcase = "^1.2"
-spacy = "3.7.2"
+spacy = "3.7.4"
 PyYAML = "^6.0.0"
 scikit-learn = "^1.0.2"
 # Note: Adding torch like this should not be necessary,
 # as it is a dependency upstream to other projects
 # however the following is necessary to make torch
 # build on Docker
 torch = ">=2.0.0, !=2.0.1, !=2.1.0"
```

### Comparing `cltk-1.2.6/src/cltk/alphabet/ang.py` & `cltk-1.3.0/src/cltk/alphabet/ang.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/arb.py` & `cltk-1.3.0/src/cltk/alphabet/arb.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/arc.py` & `cltk-1.3.0/src/cltk/alphabet/arc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/ave.py` & `cltk-1.3.0/src/cltk/alphabet/ave.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/ben.py` & `cltk-1.3.0/src/cltk/alphabet/ben.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/egy.py` & `cltk-1.3.0/src/cltk/alphabet/egy.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/enm.py` & `cltk-1.3.0/src/cltk/alphabet/enm.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/fro.py` & `cltk-1.3.0/src/cltk/alphabet/fro.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/gmh.py` & `cltk-1.3.0/src/cltk/alphabet/gmh.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/grc/beta_to_unicode.py` & `cltk-1.3.0/src/cltk/alphabet/grc/beta_to_unicode.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/grc/cypriot.py` & `cltk-1.3.0/src/cltk/alphabet/grc/cypriot.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/grc/grc.py` & `cltk-1.3.0/src/cltk/alphabet/grc/grc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/guj.py` & `cltk-1.3.0/src/cltk/alphabet/guj.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/hin.py` & `cltk-1.3.0/src/cltk/alphabet/hin.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/kan.py` & `cltk-1.3.0/src/cltk/alphabet/kan.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/lat.py` & `cltk-1.3.0/src/cltk/alphabet/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/non.py` & `cltk-1.3.0/src/cltk/alphabet/non.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/omr.py` & `cltk-1.3.0/src/cltk/alphabet/omr.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/ory.py` & `cltk-1.3.0/src/cltk/alphabet/ory.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/osc.py` & `cltk-1.3.0/src/cltk/alphabet/osc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/ota.py` & `cltk-1.3.0/src/cltk/alphabet/ota.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/oty.py` & `cltk-1.3.0/src/cltk/alphabet/oty.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/peo.py` & `cltk-1.3.0/src/cltk/alphabet/peo.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/pes.py` & `cltk-1.3.0/src/cltk/alphabet/pes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/pli.py` & `cltk-1.3.0/src/cltk/alphabet/pli.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/processes.py` & `cltk-1.3.0/src/cltk/alphabet/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/san.py` & `cltk-1.3.0/src/cltk/alphabet/san.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/tel.py` & `cltk-1.3.0/src/cltk/alphabet/tel.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/text_normalization.py` & `cltk-1.3.0/src/cltk/alphabet/text_normalization.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/urd.py` & `cltk-1.3.0/src/cltk/alphabet/urd.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/xcl/xcl.py` & `cltk-1.3.0/src/cltk/alphabet/xcl/xcl.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/xlc.py` & `cltk-1.3.0/src/cltk/alphabet/xlc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/alphabet/xld.py` & `cltk-1.3.0/src/cltk/alphabet/xld.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/core/cltk_logger.py` & `cltk-1.3.0/src/cltk/core/cltk_logger.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/core/data_types.py` & `cltk-1.3.0/src/cltk/core/data_types.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/core/exceptions.py` & `cltk-1.3.0/src/cltk/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tei.py` & `cltk-1.3.0/src/cltk/corpora/grc/tei.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/author_date.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/author_date.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/author_epithet.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/author_epithet.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/author_geo.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/author_geo.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/file_utils.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/file_utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/id_author.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/id_author.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/index_lists.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/index_lists.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/parse_tlg_indices.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/parse_tlg_indices.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/tlg_index.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/tlg_index.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/tlgu.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/tlgu.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/grc/tlg/work_numbers.py` & `cltk-1.3.0/src/cltk/corpora/grc/tlg/work_numbers.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/lat/phi/file_utils.py` & `cltk-1.3.0/src/cltk/corpora/lat/phi/file_utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/corpora/lat/phi/phi5_index.py` & `cltk-1.3.0/src/cltk/corpora/lat/phi/phi5_index.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/data/fetch.py` & `cltk-1.3.0/src/cltk/data/fetch.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/dependency/processes.py` & `cltk-1.3.0/src/cltk/dependency/processes.py`

 * *Files 9% similar despite different names*

```diff
@@ -330,8 +330,19 @@
     """Run a Spacy model.
 
     <https://huggingface.co/latincy>_
     """
 
     language: Literal["lat"] = "lat"
     description: str = "Process for Spacy for Patrick Burn's Latin model."
-    authorship_info: str = "``LatinSpacyProcess`` using LatinCy model by Patrick Burns from https://arxiv.org/abs/2305.04365 . Please cite: https://arxiv.org/abs/2305.04365"
+    authorship_info: str = "``LatinSpacyProcess`` using LatinCy model by Patrick Burns from https://huggingface.co/latincy . Please cite: https://arxiv.org/abs/2305.04365"
+
+@dataclass
+class GreekSpacyProcess(SpacyProcess):
+    """Run a Spacy model.
+
+    <https://huggingface.co/chcaa>_
+    """
+
+    language: Literal["grc"] = "grc"
+    description: str = "Process for Spacy for OdyCy's Greek model."
+    authorship_info: str = "``GreekSpacyProcess`` using OdyCy model by Center for Humanities Computing Aarhus from https://huggingface.co/chcaa . Please cite: https://aclanthology.org/2023.latechclfl-1.14"
```

### Comparing `cltk-1.2.6/src/cltk/dependency/spacy_wrapper.py` & `cltk-1.3.0/src/cltk/dependency/spacy_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 from cltk.core.exceptions import CLTKException, UnknownLanguageError
 from cltk.utils.utils import query_yes_no
 
 LOG = logging.getLogger(__name__)
 LOG.addHandler(logging.NullHandler())
 
 MAP_LANGS_CLTK_SPACY = {
+    "grc": "grc",
     "lat": "la",
 }
 
 MAP_LANG_TO_SPACY_MODEL_NAME: dict[str, str] = {
+    "grc": "grc_odycy_joint_sm",
     "lat": "la_core_web_lg",
 }
 
 MAP_LANG_TO_SPACY_MODEL_URL: dict[str, str] = {
+    "grc": "https://huggingface.co/chcaa/grc_odycy_joint_sm/resolve/main/grc_odycy_joint_sm-any-py3-none-any.whl",
     "lat": "https://huggingface.co/latincy/la_core_web_lg/resolve/main/la_core_web_lg-any-py3-none-any.whl",
 }
 
 
 class SpacyWrapper:
     """`SpacyWrapper` has been made to be an interface
     between spaCy and CLTK.
@@ -116,14 +119,23 @@
             subprocess.check_call(
                 [
                     "pip",
                     "install",
                     "https://huggingface.co/latincy/la_core_web_lg/resolve/main/la_core_web_lg-any-py3-none-any.whl",
                 ]
             )
+        elif self.language == "grc":
+            # Use OdyCy's Spacy models, hosted on HuggingFace
+            subprocess.check_call(
+                [
+                    "pip",
+                    "install",
+                    "https://huggingface.co/chcaa/grc_odycy_joint_sm/resolve/main/grc_odycy_joint_sm-any-py3-none-any.whl",
+                ]
+            )
         else:
             raise CLTKException(
                 f"No spaCy model found for language '{self.language}'. If you know of a publicly available spaCy model for '{self.language}', please open a pull request (with this message) at `https://github.com/cltk/cltk/issues`."
             )
 
     def _is_model_present(self) -> bool:
         return spacy.util.is_package(self.spacy_model_name)
```

### Comparing `cltk-1.2.6/src/cltk/dependency/stanza_wrapper.py` & `cltk-1.3.0/src/cltk/dependency/stanza_wrapper.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/dependency/tree.py` & `cltk-1.3.0/src/cltk/dependency/tree.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/dependency/utils.py` & `cltk-1.3.0/src/cltk/dependency/utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/embeddings/embeddings.py` & `cltk-1.3.0/src/cltk/embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/embeddings/processes.py` & `cltk-1.3.0/src/cltk/embeddings/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/embeddings/sentence.py` & `cltk-1.3.0/src/cltk/embeddings/sentence.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/languages/example_texts.py` & `cltk-1.3.0/src/cltk/languages/example_texts.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/languages/glottolog.py` & `cltk-1.3.0/src/cltk/languages/glottolog.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/languages/pipelines.py` & `cltk-1.3.0/src/cltk/languages/pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from cltk.alphabet.processes import GreekNormalizeProcess, LatinNormalizeProcess
 from cltk.core.data_types import Language, Pipeline, Process
 from cltk.dependency.processes import (
     ChineseStanzaProcess,
     CopticStanzaProcess,
     GothicStanzaProcess,
     GreekStanzaProcess,
+    GreekSpacyProcess,
     LatinSpacyProcess,
     LatinStanzaProcess,
     OCSStanzaProcess,
     OldFrenchStanzaProcess,
 )
 from cltk.embeddings.processes import (
     ArabicEmbeddingsProcess,
@@ -226,15 +227,16 @@
 
     description: str = "Pipeline for the Greek language"
     language: Language = get_lang("grc")
     processes: list[Type[Process]] = field(
         default_factory=lambda: [
             # GreekTokenizationProcess,
             GreekNormalizeProcess,
-            GreekStanzaProcess,
+            #GreekStanzaProcess,
+            GreekSpacyProcess,
             GreekEmbeddingsProcess,
             StopsProcess,
             # GreekNERProcess,
         ]
     )
```

### Comparing `cltk-1.2.6/src/cltk/languages/utils.py` & `cltk-1.3.0/src/cltk/languages/utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lemmatize/ang.py` & `cltk-1.3.0/src/cltk/lemmatize/ang.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lemmatize/backoff.py` & `cltk-1.3.0/src/cltk/lemmatize/backoff.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lemmatize/fro.py` & `cltk-1.3.0/src/cltk/lemmatize/fro.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lemmatize/grc.py` & `cltk-1.3.0/src/cltk/lemmatize/grc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lemmatize/lat.py` & `cltk-1.3.0/src/cltk/lemmatize/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lemmatize/naive_lemmatizer.py` & `cltk-1.3.0/src/cltk/lemmatize/naive_lemmatizer.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lemmatize/processes.py` & `cltk-1.3.0/src/cltk/lemmatize/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lexicon/lat.py` & `cltk-1.3.0/src/cltk/lexicon/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lexicon/non.py` & `cltk-1.3.0/src/cltk/lexicon/non.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/lexicon/processes.py` & `cltk-1.3.0/src/cltk/lexicon/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/morphology/akk.py` & `cltk-1.3.0/src/cltk/morphology/akk.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/morphology/lat.py` & `cltk-1.3.0/src/cltk/morphology/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/morphology/morphosyntax.py` & `cltk-1.3.0/src/cltk/morphology/morphosyntax.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/morphology/universal_dependencies_features.py` & `cltk-1.3.0/src/cltk/morphology/universal_dependencies_features.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/morphology/utils.py` & `cltk-1.3.0/src/cltk/morphology/utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/ner/ner.py` & `cltk-1.3.0/src/cltk/ner/ner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/ner/processes.py` & `cltk-1.3.0/src/cltk/ner/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/ner/spacy_ner.py` & `cltk-1.3.0/src/cltk/ner/spacy_ner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/nlp.py` & `cltk-1.3.0/src/cltk/nlp.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/__init__.py` & `cltk-1.3.0/src/cltk/phonology/__init__.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/akk.py` & `cltk-1.3.0/src/cltk/phonology/akk.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/ang/orthophonology.py` & `cltk-1.3.0/src/cltk/phonology/ang/orthophonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/ang/phonology.py` & `cltk-1.3.0/src/cltk/phonology/ang/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/ang/transcription.py` & `cltk-1.3.0/src/cltk/phonology/ang/transcription.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/ang/transliteration.py` & `cltk-1.3.0/src/cltk/phonology/ang/transliteration.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/arb/romanization.py` & `cltk-1.3.0/src/cltk/phonology/arb/romanization.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/arb/utils/pyarabic/araby.py` & `cltk-1.3.0/src/cltk/phonology/arb/utils/pyarabic/araby.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/arb/utils/pyarabic/stack.py` & `cltk-1.3.0/src/cltk/phonology/arb/utils/pyarabic/stack.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/enm/phonology.py` & `cltk-1.3.0/src/cltk/phonology/enm/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/enm/stress.py` & `cltk-1.3.0/src/cltk/phonology/enm/stress.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/enm/syllabifier.py` & `cltk-1.3.0/src/cltk/phonology/enm/syllabifier.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/gmh/phonology.py` & `cltk-1.3.0/src/cltk/phonology/gmh/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/gmh/syllabifier.py` & `cltk-1.3.0/src/cltk/phonology/gmh/syllabifier.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/gmh/transcription.py` & `cltk-1.3.0/src/cltk/phonology/gmh/transcription.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/got/phonology.py` & `cltk-1.3.0/src/cltk/phonology/got/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/got/transcription.py` & `cltk-1.3.0/src/cltk/phonology/got/transcription.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/grc/phonology.py` & `cltk-1.3.0/src/cltk/phonology/grc/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/grc/transcription.py` & `cltk-1.3.0/src/cltk/phonology/grc/transcription.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/lat/phonology.py` & `cltk-1.3.0/src/cltk/phonology/lat/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/lat/syllabifier.py` & `cltk-1.3.0/src/cltk/phonology/lat/syllabifier.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/lat/transcription.py` & `cltk-1.3.0/src/cltk/phonology/lat/transcription.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/non/old_swedish/phonology.py` & `cltk-1.3.0/src/cltk/phonology/non/old_swedish/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/non/old_swedish/transcription.py` & `cltk-1.3.0/src/cltk/phonology/non/old_swedish/transcription.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/non/orthophonology.py` & `cltk-1.3.0/src/cltk/phonology/non/orthophonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/non/phonology.py` & `cltk-1.3.0/src/cltk/phonology/non/phonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/non/syllabifier.py` & `cltk-1.3.0/src/cltk/phonology/non/syllabifier.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/non/transcription.py` & `cltk-1.3.0/src/cltk/phonology/non/transcription.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/non/utils.py` & `cltk-1.3.0/src/cltk/phonology/non/utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/orthophonology.py` & `cltk-1.3.0/src/cltk/phonology/orthophonology.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/syllabifier_processes.py` & `cltk-1.3.0/src/cltk/phonology/syllabifier_processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/syllabify.py` & `cltk-1.3.0/src/cltk/phonology/syllabify.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/phonology/transcription_processes.py` & `cltk-1.3.0/src/cltk/phonology/transcription_processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/gmh.py` & `cltk-1.3.0/src/cltk/prosody/gmh.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/grc.py` & `cltk-1.3.0/src/cltk/prosody/grc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/clausulae_analysis.py` & `cltk-1.3.0/src/cltk/prosody/lat/clausulae_analysis.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/hendecasyllable_scanner.py` & `cltk-1.3.0/src/cltk/prosody/lat/hendecasyllable_scanner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/hexameter_scanner.py` & `cltk-1.3.0/src/cltk/prosody/lat/hexameter_scanner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/macronizer.py` & `cltk-1.3.0/src/cltk/prosody/lat/macronizer.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/metrical_validator.py` & `cltk-1.3.0/src/cltk/prosody/lat/metrical_validator.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/pentameter_scanner.py` & `cltk-1.3.0/src/cltk/prosody/lat/pentameter_scanner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/scanner.py` & `cltk-1.3.0/src/cltk/prosody/lat/scanner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/scansion_constants.py` & `cltk-1.3.0/src/cltk/prosody/lat/scansion_constants.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/scansion_formatter.py` & `cltk-1.3.0/src/cltk/prosody/lat/scansion_formatter.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/string_utils.py` & `cltk-1.3.0/src/cltk/prosody/lat/string_utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/syllabifier.py` & `cltk-1.3.0/src/cltk/prosody/lat/syllabifier.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/verse.py` & `cltk-1.3.0/src/cltk/prosody/lat/verse.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/lat/verse_scanner.py` & `cltk-1.3.0/src/cltk/prosody/lat/verse_scanner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/prosody/non.py` & `cltk-1.3.0/src/cltk/prosody/non.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/sentence/grc.py` & `cltk-1.3.0/src/cltk/sentence/grc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/sentence/lat.py` & `cltk-1.3.0/src/cltk/sentence/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/sentence/non.py` & `cltk-1.3.0/src/cltk/sentence/non.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/sentence/processes.py` & `cltk-1.3.0/src/cltk/sentence/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/sentence/san.py` & `cltk-1.3.0/src/cltk/sentence/san.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/sentence/sentence.py` & `cltk-1.3.0/src/cltk/sentence/sentence.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stem/akk.py` & `cltk-1.3.0/src/cltk/stem/akk.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stem/enm.py` & `cltk-1.3.0/src/cltk/stem/enm.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stem/fro.py` & `cltk-1.3.0/src/cltk/stem/fro.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stem/gmh.py` & `cltk-1.3.0/src/cltk/stem/gmh.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stem/lat.py` & `cltk-1.3.0/src/cltk/stem/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stem/processes.py` & `cltk-1.3.0/src/cltk/stem/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/ang.py` & `cltk-1.3.0/src/cltk/stops/ang.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/arb.py` & `cltk-1.3.0/src/cltk/stops/arb.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/cop.py` & `cltk-1.3.0/src/cltk/stops/cop.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/enm.py` & `cltk-1.3.0/src/cltk/stops/enm.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/fro.py` & `cltk-1.3.0/src/cltk/stops/fro.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/gmh.py` & `cltk-1.3.0/src/cltk/stops/gmh.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/grc.py` & `cltk-1.3.0/src/cltk/stops/grc.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/hin.py` & `cltk-1.3.0/src/cltk/stops/hin.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/lat.py` & `cltk-1.3.0/src/cltk/stops/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/non.py` & `cltk-1.3.0/src/cltk/stops/non.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/omr.py` & `cltk-1.3.0/src/cltk/stops/omr.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/pan.py` & `cltk-1.3.0/src/cltk/stops/pan.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/processes.py` & `cltk-1.3.0/src/cltk/stops/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/san.py` & `cltk-1.3.0/src/cltk/stops/san.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/stops/words.py` & `cltk-1.3.0/src/cltk/stops/words.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tag/ner.py` & `cltk-1.3.0/src/cltk/tag/ner.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tag/pos.py` & `cltk-1.3.0/src/cltk/tag/pos.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tag/treebanks.py` & `cltk-1.3.0/src/cltk/tag/treebanks.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/text/akk.py` & `cltk-1.3.0/src/cltk/text/akk.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/text/lat.py` & `cltk-1.3.0/src/cltk/text/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/text/non.py` & `cltk-1.3.0/src/cltk/text/non.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/text/processes.py` & `cltk-1.3.0/src/cltk/text/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/akk.py` & `cltk-1.3.0/src/cltk/tokenizers/akk.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/arb.py` & `cltk-1.3.0/src/cltk/tokenizers/arb.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/enm.py` & `cltk-1.3.0/src/cltk/tokenizers/enm.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/fro.py` & `cltk-1.3.0/src/cltk/tokenizers/fro.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/gmh.py` & `cltk-1.3.0/src/cltk/tokenizers/gmh.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/lat/lat.py` & `cltk-1.3.0/src/cltk/tokenizers/lat/lat.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/lat/params.py` & `cltk-1.3.0/src/cltk/tokenizers/lat/params.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/lat/utils.py` & `cltk-1.3.0/src/cltk/tokenizers/lat/utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/line.py` & `cltk-1.3.0/src/cltk/tokenizers/line.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/non.py` & `cltk-1.3.0/src/cltk/tokenizers/non.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/processes.py` & `cltk-1.3.0/src/cltk/tokenizers/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/utils.py` & `cltk-1.3.0/src/cltk/tokenizers/utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/tokenizers/word.py` & `cltk-1.3.0/src/cltk/tokenizers/word.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/utils/feature_extraction.py` & `cltk-1.3.0/src/cltk/utils/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/utils/file_operations.py` & `cltk-1.3.0/src/cltk/utils/file_operations.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/utils/utils.py` & `cltk-1.3.0/src/cltk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/wordnet/processes.py` & `cltk-1.3.0/src/cltk/wordnet/processes.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/src/cltk/wordnet/wordnet.py` & `cltk-1.3.0/src/cltk/wordnet/wordnet.py`

 * *Files identical despite different names*

### Comparing `cltk-1.2.6/PKG-INFO` & `cltk-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltk
-Version: 1.2.6
+Version: 1.3.0
 Summary: The Classical Language Toolkit
 Home-page: http://cltk.org
 License: MIT
 Keywords: nlp,ai,nltk,latin,greek
 Author: Kyle P. Johnson
 Author-email: kyle@kyle-p-johnson.com
 Requires-Python: >=3.9,<3.12
@@ -34,15 +34,15 @@
 Requires-Dist: gitpython (>=3.0,<4.0)
 Requires-Dist: greek-accentuation (>=1.2.0,<2.0.0)
 Requires-Dist: nltk (>=3.7,<4.0)
 Requires-Dist: rapidfuzz (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.22.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
 Requires-Dist: scipy (<1.13.0)
-Requires-Dist: spacy (==3.7.2)
+Requires-Dist: spacy (==3.7.4)
 Requires-Dist: stanza (>=1.6.0,<2.0.0)
 Requires-Dist: stringcase (>=1.2,<2.0)
 Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0)
 Requires-Dist: tqdm (>=4.41.1,<5.0.0)
 Project-URL: Documentation, https://cltk.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/cltk/cltk
 Description-Content-Type: text/x-rst
```

