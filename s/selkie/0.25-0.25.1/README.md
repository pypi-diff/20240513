# Comparing `tmp/selkie-0.25.tar.gz` & `tmp/selkie-0.25.1.tar.gz`

## Comparing `selkie-0.25.tar` & `selkie-0.25.1.tar`

### file list

```diff
@@ -1,614 +1,641 @@
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 selkie-0.25/.readthedocs.yaml
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 selkie-0.25/setup.cfg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 selkie-0.25/utf8.txt
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 selkie-0.25/dev/language_codes.ipynb
--rw-r--r--   0        0        0    13413 2020-02-02 00:00:00.000000 selkie-0.25/dev/lazylist.ipynb
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 selkie-0.25/dev/rom.ipynb
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 selkie-0.25/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 selkie-0.25/docs/make.bat
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/conf.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/index.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/requirements.txt
--rw-r--r--   0        0        0    90260 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/app.fig1.jpeg
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/index.rst
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/mvmov.xml
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/corpus.rst
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/corpus_resources.rst
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/export.rst
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/index.rst
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/langdb.rst
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/language.rst
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/learn.rst
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/lexicon.rst
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/media.rst
--rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/text.rst
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/token.rst
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/corpus/words.rst
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/index.rst
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/overview.rst
--rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/elt.rst
--rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/framework.rst
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/index.rst
--rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/requests.rst
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/content/responses.rst
--rw-r--r--   0        0        0    36559 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/database.rst
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/db_files.rst
--rw-r--r--   0        0        0    16872 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/db_toplevel.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/index.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/db/substrate.rst
--rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/app_toplevel.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/index.rst
--rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/python_servers.rst
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/resources.rst
--rw-r--r--   0        0        0    18025 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/sealapp.rst
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/server.rst
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/imp/server/wsgi.rst
--rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/js/PlainTextPanel.html
--rw-r--r--   0        0        0    14838 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/js/XScript.html
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/config.rst
--rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/fs.rst
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/index.rst
--rw-r--r--   0        0        0    43447 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/io.rst
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/kvi.rst.ignore
--rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/misc.rst
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/pyext/scripts.rst
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/cgi.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/index.rst
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/intro.rst
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/cld/userguide/text.rst
--rw-r--r--   0        0        0    31927 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/corpora.rst
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/data.rst
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/index.rst
--rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/lexica.rst
--rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/wiktionary.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/index.rst
--rw-r--r--   0        0        0    28709 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex2.rst
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex_comline.rst
--rw-r--r--   0        0        0    22026 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex_intro.rst
--rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/data/panlex/panlex_module.rst
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/index.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/conc.rst
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/corpus.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/index.rst
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic-student.html
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic-student.rhtm
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic.html
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/gothic.rhtm
--rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/corpus/rom/index.rst
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/disk.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/index.rst
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/intro.rst
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/store.rst
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/editor/server/webserver.rst
--rw-r--r--   0        0        0    17089 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/figs/fig9.jpg
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/intro/index.rst
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/intro/langdig.rst
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/intro/overview.rst
--rw-r--r--   0        0        0    15174 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/bot.rst
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/chartparser.rst
--rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dep.rst
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/expr.rst
--rw-r--r--   0        0        0    31295 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/fsa.rst
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/fst.rst
--rw-r--r--   0        0        0    43843 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/glab.rst
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/head.rst
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/index.rst
--rw-r--r--   0        0        0    19125 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/interp.rst
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/interpreter.rst
--rw-r--r--   0        0        0    24103 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/logic.rst
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/morph.rst
--rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/parser.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/preproc.rst
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/pretts.rst
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/stemmer.rst
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/textgrid.rst
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/tok.rst
--rw-r--r--   0        0        0    31625 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/tree.rst
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/eval.rst
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/features.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/index.rst
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/mst.rst
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/nivre.rst
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/nnproj.rst
--rw-r--r--   0        0        0    22915 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/parser.rst
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/cluster.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/index.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/mat.tex
--rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/dp/ml/prob.tex
--rw-r--r--   0        0        0    12746 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/avs.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/eng.rst
--rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/features.rst
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/gdev.rst
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/grammar.rst
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/nlp/grammar/index.rst
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/com.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/data.rst
--rw-r--r--   0        0        0    20329 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/formats.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/index.rst
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/io.rst
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/persist.rst
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/reflect.rst
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/seq.rst
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/string.rst
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/table.rst
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/xml.rst
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 selkie-0.25/docs/source/pyx/xterm.rst
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/utf8.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/abspath.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/auth.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/char.py
--rw-r--r--   0        0        0    12649 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/dependencies.py
--rw-r--r--   0        0        0    14840 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/doc.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/doctest.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/glab.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/manifest.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/_script/panlex.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/__init__.py
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/__main__.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/config.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/core.py
--rw-r--r--   0        0        0    20739 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/toplevel.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/__init__.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/app-scraps.py.disabled
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/app_scraps.py.disabled
--rw-r--r--   0        0        0    21962 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/auth.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/cgi.py
--rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/client.py
--rw-r--r--   0        0        0    16886 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/config.py
--rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/core.py
--rw-r--r--   0        0        0    11311 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/dualserver.py
--rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/dualserver_full.py
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/env.py
--rw-r--r--   0        0        0    14359 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/handler.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/handler_orig.py.ignore
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/html.py
--rw-r--r--   0        0        0    14451 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/item.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/log.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/parse.py
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/request.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/resources.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/response.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/server.py
--rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/server2_old.py
--rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/server_old.py
--rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/session.py.disabled
--rw-r--r--   0        0        0    27457 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/toplevel.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/ui-scraps.py
--rw-r--r--   0        0        0    47958 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/ui.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/ui_scraps.py.disabled
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/weblib.py
--rw-r--r--   0        0        0    10716 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/app/wsgi.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/__init__.py
--rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/audio.py.todelete
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/core.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/course.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/drill.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/env.py
--rw-r--r--   0        0        0    31570 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/export.py
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/export_file.py
--rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/langdb.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/language.py
--rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/lexicon.py
--rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/media.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/rom.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/sim.py
--rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/text.py
--rw-r--r--   0        0        0    35404 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/token-new.py.disabled
--rw-r--r--   0        0        0    34350 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/token.py
--rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/transcript.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/corpus/user.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/core.py
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/dir.py
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/disk.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/env.py
--rw-r--r--   0        0        0    24305 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/file.py
--rw-r--r--   0        0        0    15014 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/meta.py
--rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/db/permissions.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/__init__.py
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/eval.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/file.py
--rw-r--r--   0        0        0    58024 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/functions.py
--rw-r--r--   0        0        0    17038 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/lang.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/glab/ui.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/config.py
--rw-r--r--   0        0        0    70509 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/io.py
--rw-r--r--   0        0        0    57270 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/misc.py
--rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/rom.py
--rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/sh.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/version.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/seal/xterm.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/__init__.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/audio.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/conc.py
--rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/corpus.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/course.py
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/file.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/igt.py
--rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/language.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/lexicon.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/media.py
--rw-r--r--   0        0        0    13156 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/page.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/rom.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/text.py
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/toc.py
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/users.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/cld/ui/video.py
--rw-r--r--   0        0        0    28573 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/__init__.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/drill.py
--rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/langs.py
--rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/lgc21.py
--rw-r--r--   0        0        0    28476 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/lgc22.py
--rw-r--r--   0        0        0    20075 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/rom.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/romfile.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/corpus/user.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/Makefile
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/__init__.py
--rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/bionlp.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/brown.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census.py
--rw-r--r--   0        0        0    26282 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/dep.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/idp.py
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/make_seal_info
--rw-r--r--   0        0        0    13736 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/panlex.py
--rw-r--r--   0        0        0    26108 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/panlex_old.py
--rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/panlex_scraps.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/perseus.py
--rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/propbank.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/ptb-rest.py.disabled
--rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/ptb.py
--rw-r--r--   0        0        0    27553 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/udt.py
--rw-r--r--   0        0        0    21353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/wiktionary.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/wn.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/README
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/both
--rw-r--r--   0        0        0  3107965 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/dist.all.last
--rw-r--r--   0        0        0   149625 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/dist.female.first
--rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/dist.male.first
--rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/census/methodology.txt
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/README
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/README.seal
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ar-padt.map
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/bg-btb.map
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ca-cat3lb.map
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/cs-pdt.map
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/da-ddt.map
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/de-negra.map
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/de-tiger.map
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/el-gdt.map
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-brown.map
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-ptb.map
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.README
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.map
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/es-cast3lb.map
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/eu-eus3lb.map
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/fi-tdt.map
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/fr-paris.map
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/hu-szeged.map
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/it-isst.map
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/iw-mila.map
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ja-kyoto.map
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ja-verbmobil.map
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ko-sejong.map
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/nl-alpino.map
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/pl-ipipan.map
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/pt-bosque.map
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ru-rnc.map
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/sl-sdt.map
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/sv-talbanken.map
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/tu-metusbanci.map
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/universal_tags.py.ignore
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/zh-ctb6.map
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/zh-sinica.map
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/eng.g
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/eng.sents
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/main.decl
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/main.g
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/main.lex
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/num.decl
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/num.g
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/eng/num.lex
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/EXAMPLES
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/Makefile
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/apptest.cfg
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/bad.html
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ca.info
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ca.pass
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/cfgfile
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class1.arff
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class2.test
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class2.train
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class3.test
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/class3.train
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/cnf.expr
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/coder1
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp1.ef
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp2.ef
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp2.ef.1
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp2.ef.2
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/crime.kb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/curiosity.kb
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent1
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent2
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent3_gold
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/depsent3_pred
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/deu.g
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/docs.mat
--rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/dream
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/drill.txt
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fg0
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/form.html
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa1
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa2
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa3
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fsa4
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/fst1
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g1
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g1.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g1a.g
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g2
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g3
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g4.g
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g4.lex
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g4.test
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g5.g
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g5.lex
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g5.test
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g6.g
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g6.lex
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g6.test
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g7.g
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g7.lex
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g7.test
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g8.g
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g8.labels
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g8.sents
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g9.g
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/g9.sents
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/intro.html
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/intro.tex
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lex1
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lex2
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lex3
--rw-r--r--   0        0        0   249612 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-1.test
--rw-r--r--   0        0        0   192782 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-1.train
--rw-r--r--   0        0        0   165698 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-2.train
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-3.test
--rw-r--r--   0        0        0   305582 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/libsvm-3.train
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/lisp1.lisp
--rwxr-xr-x   0        0        0      749 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/make_repo_example
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/make_utf8.py.ignore
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/nivre-2007.ftrs
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/nivre.exp
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/normpointers.txt
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/northwind.TextGrid
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook.gl
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook2.gl
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook3.gl
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook_test.gl
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/notebook_test.output
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/par1.txt
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.abb
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.g
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.lex
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/ptb.test
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/romtest.rom
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/s1.snt
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_3
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_4
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_5
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_6
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sec_7
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sem.g
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sem.lex
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/server.info
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/server.pass
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0.defs
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0.g
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0.lex
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg0a.g
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg1a.g
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2.defs
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2.g
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2.lex
--rw-r--r--   0        0        0    11651 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg2a.g
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg3.defs
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg3.g
--rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/sg3.lex
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/t1
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/t2
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tab1.tab
--rwxr-xr-x   0        0        0      330 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/test.cgi
--rw-r--r--   0        0        0    31700 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/test123.mp3
--rwxr-xr-x   0        0        0   404992 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/test123.wav
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/testfiles
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/testinclude.gl
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/text1
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/text1.utf8
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tinygen.g
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tok1
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tree1
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tree2
--rw-r--r--   0        0        0   796908 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tuebingen.m4a
--rw-r--r--   0        0        0   409461 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tuebingen.mp3
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/tuebingen.txt
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/upload.html
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/utf8.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/xml1
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/toc
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/deu.lg/2.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/deu.lg/3.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp22.lgc/deu.lg/toc
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/corpus
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/deu/2.txt
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/deu/3.txt
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp23.lgc/deu/lang
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/langs
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/deu/toc
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/deu/txt/2
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corp25.lgc/deu/txt/3
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/eng/texts/1/orig
--rw-r--r--   0        0        0    38333 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/lexicon
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/clips
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/transcript
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/Database.hdr
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/index.tab
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/abney/arapesh/104.txt
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/100.txt
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/101.txt
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/102.txt
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/103.txt
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/104.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/18.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/19.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/20.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/21.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/kutenai/22.txt
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/cards/index.hdr
--rw-r--r--   0        0        0    20056 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/cards/index.tab
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/igt/117
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/index.hdr
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/index.tab
--rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/ape/13.txt
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/1.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/11.lex
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/2.snt
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/2.spn
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/deu/3.snt
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/10.snt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/12.lex
--rw-r--r--   0        0        0   204790 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/15.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/16.spn
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/4.txt
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/5.snt
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/6.tok
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/7.snt
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/8.txt
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/eng/9.snt
--rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/kernel/sat/14.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/langs/index.hdr
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/langs/index.tab
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/index.hdr
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/index.tab
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/100
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/101
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/102
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/103
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/104
--rw-r--r--   0        0        0    25355 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/111/info
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/18
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/19
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/20
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/21
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/pages/99/22
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/users/index.hdr
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/examples/uc/users/index.tab
--rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-2.txt
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-5.txt
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3-macrolanguages_20170131.tab
--rw-r--r--   0        0        0   184065 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_20170202.tab
--rw-r--r--   0        0        0   206914 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_Name_Index_20170217.tab
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_Retirements_20170131.tab
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/gothic-student.rom
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/gothic.rom
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/korean.rom
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/otw-jones.rom
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/otw-webkamigad.rom
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/roms/salish.rom
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/abbreviations
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/archive.gif
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/cog.png
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/entities.txt
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/external.gif
--rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/fourletter.txt
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/headrules_main.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/headrules_np.txt
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/original_headrules_main.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/original_headrules_np.txt
--rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/ptb_filenames
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/seal.info
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/standard.rmg
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/stemmer_stems
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/data/seal/stemmer_words
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/eval.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/features.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/mst.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/nivre.py
--rw-r--r--   0        0        0    11113 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/nnproj.py
--rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/parser.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/tree.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/__init__.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/cluster.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/experiment.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/instance.py
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/libsvm.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/mat.py
--rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/num.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/prob.py
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/split.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/dp/ml/sym.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/editor/webserver.py
--rw-r--r--   0        0        0    25338 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/avs.py
--rw-r--r--   0        0        0    10713 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/bot.py
--rw-r--r--   0        0        0    38502 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/com.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/conc.py
--rw-r--r--   0        0        0    22515 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/dep.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/eng.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/expr.py
--rw-r--r--   0        0        0    15836 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/features.py
--rw-r--r--   0        0        0    21557 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/fsa.py
--rw-r--r--   0        0        0    15430 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/fst.py
--rw-r--r--   0        0        0    17385 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/gdev.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/gen.py
--rw-r--r--   0        0        0    20833 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/grammar.py
--rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/head.py
--rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/interp.py
--rw-r--r--   0        0        0    80152 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/io.py
--rw-r--r--   0        0        0    23405 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/logic.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/map.py
--rw-r--r--   0        0        0    15359 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/parser.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/pretts.py
--rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/seq.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/stemmer.py
--rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/string.py
--rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/textgrid.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/tok.py
--rw-r--r--   0        0        0    30483 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlp/tree.py
--rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/avs.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/expr.py
--rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/features.py
--rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/gdev.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/glab.py
--rw-r--r--   0        0        0    21099 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/grammar.py
--rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/parser.py
--rw-r--r--   0        0        0    30353 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/nlpx/tree.py
--rw-r--r--   0        0        0    16989 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/com.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/disk.py
--rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/formats.py
--rw-r--r--   0        0        0    46908 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/io.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/ipynb.py
--rw-r--r--   0        0        0    15507 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/manifest.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/object.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/persist.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/reflect.py
--rw-r--r--   0        0        0    15569 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/seq.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/store.py
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/string.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/table.py
--rw-r--r--   0        0        0    21059 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/xml.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 selkie-0.25/src/selkie/pyx/xterm.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25/tests/Makefile
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 selkie-0.25/tests/checkdist.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 selkie-0.25/tests/run_tests.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 selkie-0.25/tests/test_bot.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 selkie-0.25/tests/test_rom.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 selkie-0.25/tests/test_rom_graph
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 selkie-0.25/.gitignore
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25/README.rst
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 selkie-0.25/pyproject.toml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 selkie-0.25/PKG-INFO
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 selkie-0.25.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 selkie-0.25.1/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 selkie-0.25.1/utf8.txt
+-rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 selkie-0.25.1/dev/language_codes.ipynb
+-rw-r--r--   0        0        0    13413 2020-02-02 00:00:00.000000 selkie-0.25.1/dev/lazylist.ipynb
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 selkie-0.25.1/dev/rom.ipynb
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/make.bat
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/conf.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/index.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/requirements.txt
+-rw-r--r--   0        0        0    90260 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/app.fig1.jpeg
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/index.rst
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/mvmov.xml
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/corpus.rst
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/corpus_resources.rst
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/export.rst
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/index.rst
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/langdb.rst
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/language.rst
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/learn.rst
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/lexicon.rst
+-rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/media.rst
+-rw-r--r--   0        0        0    11312 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/text.rst
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/token.rst
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/corpus/words.rst
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/index.rst
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/overview.rst
+-rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/content/elt.rst
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/content/framework.rst
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/content/index.rst
+-rw-r--r--   0        0        0     8293 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/content/requests.rst
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/content/responses.rst
+-rw-r--r--   0        0        0    36559 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/db/database.rst
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/db/db_files.rst
+-rw-r--r--   0        0        0    16872 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/db/db_toplevel.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/db/index.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/db/substrate.rst
+-rw-r--r--   0        0        0    27996 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/server/app_toplevel.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/server/index.rst
+-rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/server/python_servers.rst
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/server/resources.rst
+-rw-r--r--   0        0        0    18025 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/server/sealapp.rst
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/server/server.rst
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/imp/server/wsgi.rst
+-rw-r--r--   0        0        0    10962 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/js/PlainTextPanel.html
+-rw-r--r--   0        0        0    14838 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/js/XScript.html
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/pyext/config.rst
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/pyext/fs.rst
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/pyext/index.rst
+-rw-r--r--   0        0        0    43447 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/pyext/io.rst
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/pyext/kvi.rst.ignore
+-rw-r--r--   0        0        0     5339 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/pyext/misc.rst
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/pyext/scripts.rst
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/userguide/cgi.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/userguide/index.rst
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/userguide/intro.rst
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/cld/userguide/text.rst
+-rw-r--r--   0        0        0    31927 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/corpora.rst
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/data.rst
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/index.rst
+-rw-r--r--   0        0        0     3682 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/lexica.rst
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/wiktionary.rst
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/panlex/index.rst
+-rw-r--r--   0        0        0    28709 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/panlex/panlex2.rst
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/panlex/panlex_comline.rst
+-rw-r--r--   0        0        0    22026 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/panlex/panlex_intro.rst
+-rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/data/panlex/panlex_module.rst
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/index.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/conc.rst
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/corpus.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/index.rst
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/rom/gothic-student.html
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/rom/gothic-student.rhtm
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/rom/gothic.html
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/rom/gothic.rhtm
+-rw-r--r--   0        0        0     8946 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/corpus/rom/index.rst
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/server/disk.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/server/index.rst
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/server/intro.rst
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/server/store.rst
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/editor/server/webserver.rst
+-rw-r--r--   0        0        0    17089 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/figs/fig9.jpg
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/intro/index.rst
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/intro/langdig.rst
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/intro/overview.rst
+-rw-r--r--   0        0        0    15174 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/bot.rst
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/chartparser.rst
+-rw-r--r--   0        0        0    20110 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dep.rst
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/expr.rst
+-rw-r--r--   0        0        0    31295 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/fsa.rst
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/fst.rst
+-rw-r--r--   0        0        0    43843 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/glab.rst
+-rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/head.rst
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/index.rst
+-rw-r--r--   0        0        0    19125 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/interp.rst
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/interpreter.rst
+-rw-r--r--   0        0        0    24103 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/logic.rst
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/morph.rst
+-rw-r--r--   0        0        0    11912 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/parser.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/preproc.rst
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/pretts.rst
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/stemmer.rst
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/textgrid.rst
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/tok.rst
+-rw-r--r--   0        0        0    31625 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/tree.rst
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/eval.rst
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/features.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/index.rst
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/mst.rst
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/nivre.rst
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/nnproj.rst
+-rw-r--r--   0        0        0    22915 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/parser.rst
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/ml/cluster.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/ml/index.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/ml/mat.tex
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/dp/ml/prob.tex
+-rw-r--r--   0        0        0    12746 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/grammar/avs.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/grammar/eng.rst
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/grammar/features.rst
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/grammar/gdev.rst
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/grammar/grammar.rst
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/nlp/grammar/index.rst
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/com.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/data.rst
+-rw-r--r--   0        0        0    20329 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/formats.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/index.rst
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/io.rst
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/persist.rst
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/reflect.rst
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/seq.rst
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/string.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/table.rst
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/xml.rst
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 selkie-0.25.1/docs/source/pyx/xterm.rst
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/utf8.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/abspath.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/auth.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/char.py
+-rw-r--r--   0        0        0    12649 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/dependencies.py
+-rw-r--r--   0        0        0    14840 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/doc.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/doctest.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/glab.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/manifest.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/_script/panlex.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/__init__.py
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/__main__.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/config.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/core.py
+-rw-r--r--   0        0        0    20739 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/toplevel.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/__init__.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/app-scraps.py.disabled
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/app_scraps.py.disabled
+-rw-r--r--   0        0        0    21962 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/auth.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/cgi.py
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/client.py
+-rw-r--r--   0        0        0    16886 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/config.py
+-rw-r--r--   0        0        0    10405 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/core.py
+-rw-r--r--   0        0        0    11311 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/dualserver.py
+-rw-r--r--   0        0        0    17368 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/dualserver_full.py
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/env.py
+-rw-r--r--   0        0        0    14359 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/handler.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/handler_orig.py.ignore
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/html.py
+-rw-r--r--   0        0        0    14451 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/item.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/log.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/parse.py
+-rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/request.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/resources.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/response.py
+-rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/server.py
+-rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/server2_old.py
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/server_old.py
+-rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/session.py.disabled
+-rw-r--r--   0        0        0    27457 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/toplevel.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/ui-scraps.py
+-rw-r--r--   0        0        0    47958 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/ui.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/ui_scraps.py.disabled
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/weblib.py
+-rw-r--r--   0        0        0    10716 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/app/wsgi.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/__init__.py
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/audio.py.todelete
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/core.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/course.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/drill.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/env.py
+-rw-r--r--   0        0        0    31570 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/export.py
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/export_file.py
+-rw-r--r--   0        0        0    15330 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/langdb.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/language.py
+-rw-r--r--   0        0        0    22626 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/lexicon.py
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/media.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/rom.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/sim.py
+-rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/text.py
+-rw-r--r--   0        0        0    35404 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/token-new.py.disabled
+-rw-r--r--   0        0        0    34350 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/token.py
+-rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/transcript.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/corpus/user.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/core.py
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/dir.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/disk.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/env.py
+-rw-r--r--   0        0        0    24305 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/file.py
+-rw-r--r--   0        0        0    15014 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/meta.py
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/db/permissions.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/glab/__init__.py
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/glab/eval.py
+-rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/glab/file.py
+-rw-r--r--   0        0        0    58024 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/glab/functions.py
+-rw-r--r--   0        0        0    17038 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/glab/lang.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/glab/ui.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/IGTEditor.css
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/IGTEditor.js
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/LexentViewer.css
+-rw-r--r--   0        0        0    17532 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/LexentViewer.js
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/PlainTextPanel.css
+-rw-r--r--   0        0        0    13796 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/PlainTextPanel.js
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/RomEditor.js
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/XScript.css
+-rw-r--r--   0        0        0    20429 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/XScript.js
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/ajax.js
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/conc.css
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/conc.js
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/default.css
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/default.js
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/editor.css
+-rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/editor.js
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/element.js
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/grid.css
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/login.html
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/master.js
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/plaintext.css
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/plaintext.js
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/transcriber.css
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/transcriber.js
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/trigger.js
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/util.css
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/lib/util.js
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/seal/config.py
+-rw-r--r--   0        0        0    70509 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/seal/io.py
+-rw-r--r--   0        0        0    57270 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/seal/misc.py
+-rw-r--r--   0        0        0    18126 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/seal/rom.py
+-rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/seal/sh.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/seal/version.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/seal/xterm.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/__init__.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/audio.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/conc.py
+-rw-r--r--   0        0        0    16981 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/corpus.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/course.py
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/file.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/igt.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/language.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/lexicon.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/media.py
+-rw-r--r--   0        0        0    13156 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/page.py
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/rom.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/text.py
+-rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/toc.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/users.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/cld/ui/video.py
+-rw-r--r--   0        0        0    28573 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/__init__.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/drill.py
+-rw-r--r--   0        0        0    15440 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/langs.py
+-rw-r--r--   0        0        0    21939 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/lgc21.py
+-rw-r--r--   0        0        0    28476 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/lgc22.py
+-rw-r--r--   0        0        0    20075 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/rom.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/romfile.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/corpus/user.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/Makefile
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/__init__.py
+-rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/bionlp.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/brown.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/census.py
+-rw-r--r--   0        0        0    26282 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/dep.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/idp.py
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/make_seal_info
+-rw-r--r--   0        0        0    13736 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/panlex.py
+-rw-r--r--   0        0        0    26108 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/panlex_old.py
+-rw-r--r--   0        0        0    19693 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/panlex_scraps.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/perseus.py
+-rw-r--r--   0        0        0    11392 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/propbank.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/ptb-rest.py.disabled
+-rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/ptb.py
+-rw-r--r--   0        0        0    27553 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/udt.py
+-rw-r--r--   0        0        0    21353 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/wiktionary.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/wn.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/census/README
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/census/both
+-rw-r--r--   0        0        0  3107965 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/census/dist.all.last
+-rw-r--r--   0        0        0   149625 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/census/dist.female.first
+-rw-r--r--   0        0        0    42665 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/census/dist.male.first
+-rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/census/methodology.txt
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/README
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/README.seal
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ar-padt.map
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/bg-btb.map
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ca-cat3lb.map
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/cs-pdt.map
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/da-ddt.map
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/de-negra.map
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/de-tiger.map
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/el-gdt.map
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/en-brown.map
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/en-ptb.map
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.README
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.map
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/es-cast3lb.map
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/eu-eus3lb.map
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/fi-tdt.map
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/fr-paris.map
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/hu-szeged.map
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/it-isst.map
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/iw-mila.map
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ja-kyoto.map
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ja-verbmobil.map
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ko-sejong.map
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/nl-alpino.map
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/pl-ipipan.map
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/pt-bosque.map
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ru-rnc.map
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/sl-sdt.map
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/sv-talbanken.map
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/tu-metusbanci.map
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/universal_tags.py.ignore
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/zh-ctb6.map
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/zh-sinica.map
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/eng.g
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/eng.sents
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/main.decl
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/main.g
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/main.lex
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/num.decl
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/num.g
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/eng/num.lex
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/EXAMPLES
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/Makefile
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/apptest.cfg
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/bad.html
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/ca.info
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/ca.pass
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/cfgfile
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/class1.arff
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/class2.test
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/class2.train
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/class3.test
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/class3.train
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/cnf.expr
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/coder1
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp1.ef
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp2.ef
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp2.ef.1
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp2.ef.2
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/crime.kb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/curiosity.kb
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/depsent1
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/depsent2
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/depsent3_gold
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/depsent3_pred
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/deu.g
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/docs.mat
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/dream
+-rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/drill.txt
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/fg0
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/form.html
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/fsa1
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/fsa2
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/fsa3
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/fsa4
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/fst1
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g1
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g1.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g1a.g
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g2
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g3
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g4.g
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g4.lex
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g4.test
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g5.g
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g5.lex
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g5.test
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g6.g
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g6.lex
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g6.test
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g7.g
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g7.lex
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g7.test
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g8.g
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g8.labels
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g8.sents
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g9.g
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/g9.sents
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/intro.html
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/intro.tex
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/lex1
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/lex2
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/lex3
+-rw-r--r--   0        0        0   249612 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/libsvm-1.test
+-rw-r--r--   0        0        0   192782 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/libsvm-1.train
+-rw-r--r--   0        0        0   165698 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/libsvm-2.train
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/libsvm-3.test
+-rw-r--r--   0        0        0   305582 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/libsvm-3.train
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/lisp1.lisp
+-rwxr-xr-x   0        0        0      749 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/make_repo_example
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/make_utf8.py.ignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/nivre-2007.ftrs
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/nivre.exp
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/normpointers.txt
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/northwind.TextGrid
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/notebook.gl
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/notebook2.gl
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/notebook3.gl
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/notebook_test.gl
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/notebook_test.output
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/par1.txt
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/ptb.abb
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/ptb.g
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/ptb.lex
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/ptb.test
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/romtest.rom
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/s1.snt
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sec_3
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sec_4
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sec_5
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sec_6
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sec_7
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sem.g
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sem.lex
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/server.info
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/server.pass
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg0
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg0.defs
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg0.g
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg0.lex
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg0a.g
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg1a.g
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg2.defs
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg2.g
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg2.lex
+-rw-r--r--   0        0        0    11651 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg2a.g
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg3.defs
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg3.g
+-rw-r--r--   0        0        0     7838 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/sg3.lex
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/t1
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/t2
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tab1.tab
+-rwxr-xr-x   0        0        0      330 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/test.cgi
+-rw-r--r--   0        0        0    31700 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/test123.mp3
+-rwxr-xr-x   0        0        0   404992 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/test123.wav
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/testfiles
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/testinclude.gl
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/text1
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/text1.utf8
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tinygen.g
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tok1
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tree1
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tree2
+-rw-r--r--   0        0        0   796908 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tuebingen.m4a
+-rw-r--r--   0        0        0   409461 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tuebingen.mp3
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/tuebingen.txt
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/upload.html
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/utf8.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/xml1
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp22.lgc/toc
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp22.lgc/deu.lg/2.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp22.lgc/deu.lg/3.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp22.lgc/deu.lg/toc
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp23.lgc/corpus
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp23.lgc/deu/2.txt
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp23.lgc/deu/3.txt
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp23.lgc/deu/lang
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp25.lgc/langs
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp25.lgc/deu/toc
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp25.lgc/deu/txt/2
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corp25.lgc/deu/txt/3
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corpus.cld/langs/eng/texts/1/orig
+-rw-r--r--   0        0        0    38333 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corpus.cld/langs/otw/lexicon
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/clips
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/transcript
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/Database.hdr
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/index.tab
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/abney/arapesh/104.txt
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/100.txt
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/101.txt
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/102.txt
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/103.txt
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/104.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/kutenai/18.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/kutenai/19.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/kutenai/20.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/kutenai/21.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/kutenai/22.txt
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/cards/index.hdr
+-rw-r--r--   0        0        0    20056 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/cards/index.tab
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/igt/117
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/index.hdr
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/index.tab
+-rw-r--r--   0        0        0    10116 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/ape/13.txt
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/deu/1.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/deu/11.lex
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/deu/2.snt
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/deu/2.spn
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/deu/3.snt
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/10.snt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/12.lex
+-rw-r--r--   0        0        0   204790 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/15.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/16.spn
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/4.txt
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/5.snt
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/6.tok
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/7.snt
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/8.txt
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/9.snt
+-rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/kernel/sat/14.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/langs/index.hdr
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/langs/index.tab
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/index.hdr
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/index.tab
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/111/100
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/111/101
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/111/102
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/111/103
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/111/104
+-rw-r--r--   0        0        0    25355 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/111/info
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/99/18
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/99/19
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/99/20
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/99/21
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/pages/99/22
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/users/index.hdr
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/examples/uc/users/index.tab
+-rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/iso/639-2.txt
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/iso/639-5.txt
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3-macrolanguages_20170131.tab
+-rw-r--r--   0        0        0   184065 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3_20170202.tab
+-rw-r--r--   0        0        0   206914 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3_Name_Index_20170217.tab
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3_Retirements_20170131.tab
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/roms/gothic-student.rom
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/roms/gothic.rom
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/roms/korean.rom
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/roms/otw-jones.rom
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/roms/otw-webkamigad.rom
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/roms/salish.rom
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/abbreviations
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/archive.gif
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/cog.png
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/entities.txt
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/external.gif
+-rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/fourletter.txt
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/headrules_main.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/headrules_np.txt
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/original_headrules_main.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/original_headrules_np.txt
+-rw-r--r--   0        0        0    89058 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/ptb_filenames
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/seal.info
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/standard.rmg
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/stemmer_stems
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/data/seal/stemmer_words
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/eval.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/features.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/mst.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/nivre.py
+-rw-r--r--   0        0        0    11113 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/nnproj.py
+-rw-r--r--   0        0        0    15832 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/parser.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/tree.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/__init__.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/cluster.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/experiment.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/instance.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/libsvm.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/mat.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/num.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/prob.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/split.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/dp/ml/sym.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/editor/webserver.py
+-rw-r--r--   0        0        0    25338 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/avs.py
+-rw-r--r--   0        0        0    10713 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/bot.py
+-rw-r--r--   0        0        0    38502 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/com.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/conc.py
+-rw-r--r--   0        0        0    22515 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/dep.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/eng.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/expr.py
+-rw-r--r--   0        0        0    15836 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/features.py
+-rw-r--r--   0        0        0    21557 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/fsa.py
+-rw-r--r--   0        0        0    15430 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/fst.py
+-rw-r--r--   0        0        0    17385 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/gdev.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/gen.py
+-rw-r--r--   0        0        0    20833 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/grammar.py
+-rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/head.py
+-rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/interp.py
+-rw-r--r--   0        0        0    80152 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/io.py
+-rw-r--r--   0        0        0    23405 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/logic.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/map.py
+-rw-r--r--   0        0        0    15359 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/parser.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/pretts.py
+-rw-r--r--   0        0        0    11121 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/seq.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/stemmer.py
+-rw-r--r--   0        0        0    11934 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/string.py
+-rw-r--r--   0        0        0    11535 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/textgrid.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/tok.py
+-rw-r--r--   0        0        0    30483 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlp/tree.py
+-rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/avs.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/expr.py
+-rw-r--r--   0        0        0    15901 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/features.py
+-rw-r--r--   0        0        0    15805 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/gdev.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/glab.py
+-rw-r--r--   0        0        0    21099 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/grammar.py
+-rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/parser.py
+-rw-r--r--   0        0        0    30353 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/nlpx/tree.py
+-rw-r--r--   0        0        0    16989 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/com.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/disk.py
+-rw-r--r--   0        0        0    17346 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/formats.py
+-rw-r--r--   0        0        0    46908 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/io.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/ipynb.py
+-rw-r--r--   0        0        0    15507 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/manifest.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/object.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/persist.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/reflect.py
+-rw-r--r--   0        0        0    15569 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/seq.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/store.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/string.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/table.py
+-rw-r--r--   0        0        0    21059 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/xml.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 selkie-0.25.1/src/selkie/pyx/xterm.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 selkie-0.25.1/tests/Makefile
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 selkie-0.25.1/tests/checkdist.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 selkie-0.25.1/tests/run_tests.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 selkie-0.25.1/tests/test_bot.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 selkie-0.25.1/tests/test_rom.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 selkie-0.25.1/tests/test_rom_graph
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 selkie-0.25.1/.gitignore
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 selkie-0.25.1/README.rst
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 selkie-0.25.1/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 selkie-0.25.1/PKG-INFO
```

### Comparing `selkie-0.25/.readthedocs.yaml` & `selkie-0.25.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `selkie-0.25/setup.cfg` & `selkie-0.25.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = selkie
-version = 0.25.0
+version = 0.25.1
 author = Steven Abney
 author_email = abney@umich.edu
 description = Natural language processing and digital language description
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://www.vinartus.net/spa/
 classifiers =
```

### Comparing `selkie-0.25/dev/language_codes.ipynb` & `selkie-0.25.1/dev/language_codes.ipynb`

 * *Files identical despite different names*

### Comparing `selkie-0.25/dev/lazylist.ipynb` & `selkie-0.25.1/dev/lazylist.ipynb`

 * *Files identical despite different names*

### Comparing `selkie-0.25/dev/rom.ipynb` & `selkie-0.25.1/dev/rom.ipynb`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/Makefile` & `selkie-0.25.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/make.bat` & `selkie-0.25.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/conf.py` & `selkie-0.25.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 project = 'Selkie'
 copyright = '2022, University of Michigan'
 author = 'Steven Abney'
 
 # release: x.y, version: x.y.z
 release = '0.25'
-version = '0.25.0'
+version = '0.25.1'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
```

### Comparing `selkie-0.25/docs/source/cld/app.fig1.jpeg` & `selkie-0.25.1/docs/source/cld/app.fig1.jpeg`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/mvmov.xml` & `selkie-0.25.1/docs/source/cld/mvmov.xml`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/corpus.rst` & `selkie-0.25.1/docs/source/cld/corpus/corpus.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/corpus_resources.rst` & `selkie-0.25.1/docs/source/cld/corpus/corpus_resources.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/export.rst` & `selkie-0.25.1/docs/source/cld/corpus/export.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/langdb.rst` & `selkie-0.25.1/docs/source/cld/corpus/langdb.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/language.rst` & `selkie-0.25.1/docs/source/cld/corpus/language.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/learn.rst` & `selkie-0.25.1/docs/source/cld/corpus/learn.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/lexicon.rst` & `selkie-0.25.1/docs/source/cld/corpus/lexicon.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/media.rst` & `selkie-0.25.1/docs/source/cld/corpus/media.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/text.rst` & `selkie-0.25.1/docs/source/cld/corpus/text.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/token.rst` & `selkie-0.25.1/docs/source/cld/corpus/token.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/corpus/words.rst` & `selkie-0.25.1/docs/source/cld/corpus/words.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/overview.rst` & `selkie-0.25.1/docs/source/cld/imp/overview.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/content/elt.rst` & `selkie-0.25.1/docs/source/cld/imp/content/elt.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/content/framework.rst` & `selkie-0.25.1/docs/source/cld/imp/content/framework.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/content/requests.rst` & `selkie-0.25.1/docs/source/cld/imp/content/requests.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/content/responses.rst` & `selkie-0.25.1/docs/source/cld/imp/content/responses.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/db/database.rst` & `selkie-0.25.1/docs/source/cld/imp/db/database.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/db/db_files.rst` & `selkie-0.25.1/docs/source/cld/imp/db/db_files.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/db/db_toplevel.rst` & `selkie-0.25.1/docs/source/cld/imp/db/db_toplevel.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/server/app_toplevel.rst` & `selkie-0.25.1/docs/source/cld/imp/server/app_toplevel.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/server/python_servers.rst` & `selkie-0.25.1/docs/source/cld/imp/server/python_servers.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/server/resources.rst` & `selkie-0.25.1/docs/source/cld/imp/server/resources.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/server/sealapp.rst` & `selkie-0.25.1/docs/source/cld/imp/server/sealapp.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/server/server.rst` & `selkie-0.25.1/docs/source/cld/imp/server/server.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/imp/server/wsgi.rst` & `selkie-0.25.1/docs/source/cld/imp/server/wsgi.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/js/PlainTextPanel.html` & `selkie-0.25.1/docs/source/cld/js/PlainTextPanel.html`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/js/XScript.html` & `selkie-0.25.1/docs/source/cld/js/XScript.html`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/pyext/config.rst` & `selkie-0.25.1/docs/source/cld/pyext/config.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/pyext/fs.rst` & `selkie-0.25.1/docs/source/cld/pyext/fs.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/pyext/io.rst` & `selkie-0.25.1/docs/source/cld/pyext/io.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/pyext/kvi.rst.ignore` & `selkie-0.25.1/docs/source/cld/pyext/kvi.rst.ignore`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/pyext/misc.rst` & `selkie-0.25.1/docs/source/cld/pyext/misc.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/pyext/scripts.rst` & `selkie-0.25.1/docs/source/cld/pyext/scripts.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/userguide/cgi.rst` & `selkie-0.25.1/docs/source/cld/userguide/cgi.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/userguide/intro.rst` & `selkie-0.25.1/docs/source/cld/userguide/intro.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/cld/userguide/text.rst` & `selkie-0.25.1/docs/source/cld/userguide/text.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/data/corpora.rst` & `selkie-0.25.1/docs/source/data/corpora.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/data/lexica.rst` & `selkie-0.25.1/docs/source/data/lexica.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/data/wiktionary.rst` & `selkie-0.25.1/docs/source/data/wiktionary.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/data/panlex/panlex2.rst` & `selkie-0.25.1/docs/source/data/panlex/panlex2.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/data/panlex/panlex_intro.rst` & `selkie-0.25.1/docs/source/data/panlex/panlex_intro.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/data/panlex/panlex_module.rst` & `selkie-0.25.1/docs/source/data/panlex/panlex_module.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/index.rst` & `selkie-0.25.1/docs/source/editor/index.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/corpus/corpus.rst` & `selkie-0.25.1/docs/source/editor/corpus/corpus.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/corpus/rom/gothic-student.html` & `selkie-0.25.1/docs/source/editor/corpus/rom/gothic-student.html`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/corpus/rom/gothic-student.rhtm` & `selkie-0.25.1/docs/source/editor/corpus/rom/gothic-student.rhtm`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/corpus/rom/gothic.html` & `selkie-0.25.1/docs/source/editor/corpus/rom/gothic.html`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/corpus/rom/gothic.rhtm` & `selkie-0.25.1/docs/source/editor/corpus/rom/gothic.rhtm`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/corpus/rom/index.rst` & `selkie-0.25.1/docs/source/editor/corpus/rom/index.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/server/disk.rst` & `selkie-0.25.1/docs/source/editor/server/disk.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/server/intro.rst` & `selkie-0.25.1/docs/source/editor/server/intro.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/server/store.rst` & `selkie-0.25.1/docs/source/editor/server/store.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/editor/server/webserver.rst` & `selkie-0.25.1/docs/source/editor/server/webserver.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/figs/fig9.jpg` & `selkie-0.25.1/docs/source/figs/fig9.jpg`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/intro/langdig.rst` & `selkie-0.25.1/docs/source/intro/langdig.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/intro/overview.rst` & `selkie-0.25.1/docs/source/intro/overview.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/bot.rst` & `selkie-0.25.1/docs/source/nlp/bot.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dep.rst` & `selkie-0.25.1/docs/source/nlp/dep.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/expr.rst` & `selkie-0.25.1/docs/source/nlp/expr.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/fsa.rst` & `selkie-0.25.1/docs/source/nlp/fsa.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/fst.rst` & `selkie-0.25.1/docs/source/nlp/fst.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/glab.rst` & `selkie-0.25.1/docs/source/nlp/glab.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/head.rst` & `selkie-0.25.1/docs/source/nlp/head.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/index.rst` & `selkie-0.25.1/docs/source/nlp/index.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/interp.rst` & `selkie-0.25.1/docs/source/nlp/interp.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/logic.rst` & `selkie-0.25.1/docs/source/nlp/logic.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/parser.rst` & `selkie-0.25.1/docs/source/nlp/parser.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/pretts.rst` & `selkie-0.25.1/docs/source/nlp/pretts.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/stemmer.rst` & `selkie-0.25.1/docs/source/nlp/stemmer.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/textgrid.rst` & `selkie-0.25.1/docs/source/nlp/textgrid.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/tok.rst` & `selkie-0.25.1/docs/source/nlp/tok.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/tree.rst` & `selkie-0.25.1/docs/source/nlp/tree.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/eval.rst` & `selkie-0.25.1/docs/source/nlp/dp/eval.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/features.rst` & `selkie-0.25.1/docs/source/nlp/dp/features.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/mst.rst` & `selkie-0.25.1/docs/source/nlp/dp/mst.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/nivre.rst` & `selkie-0.25.1/docs/source/nlp/dp/nivre.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/nnproj.rst` & `selkie-0.25.1/docs/source/nlp/dp/nnproj.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/parser.rst` & `selkie-0.25.1/docs/source/nlp/dp/parser.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/ml/cluster.rst` & `selkie-0.25.1/docs/source/nlp/dp/ml/cluster.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/dp/ml/prob.tex` & `selkie-0.25.1/docs/source/nlp/dp/ml/prob.tex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/grammar/avs.rst` & `selkie-0.25.1/docs/source/nlp/grammar/avs.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/grammar/features.rst` & `selkie-0.25.1/docs/source/nlp/grammar/features.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/grammar/gdev.rst` & `selkie-0.25.1/docs/source/nlp/grammar/gdev.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/nlp/grammar/grammar.rst` & `selkie-0.25.1/docs/source/nlp/grammar/grammar.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/com.rst` & `selkie-0.25.1/docs/source/pyx/com.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/formats.rst` & `selkie-0.25.1/docs/source/pyx/formats.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/io.rst` & `selkie-0.25.1/docs/source/pyx/io.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/seq.rst` & `selkie-0.25.1/docs/source/pyx/seq.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/string.rst` & `selkie-0.25.1/docs/source/pyx/string.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/table.rst` & `selkie-0.25.1/docs/source/pyx/table.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/xml.rst` & `selkie-0.25.1/docs/source/pyx/xml.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/docs/source/pyx/xterm.rst` & `selkie-0.25.1/docs/source/pyx/xterm.rst`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/auth.py` & `selkie-0.25.1/src/selkie/_script/auth.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/char.py` & `selkie-0.25.1/src/selkie/_script/char.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/dependencies.py` & `selkie-0.25.1/src/selkie/_script/dependencies.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/doc.py` & `selkie-0.25.1/src/selkie/_script/doc.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/doctest.py` & `selkie-0.25.1/src/selkie/_script/doctest.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/glab.py` & `selkie-0.25.1/src/selkie/_script/glab.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/manifest.py` & `selkie-0.25.1/src/selkie/_script/manifest.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/_script/panlex.py` & `selkie-0.25.1/src/selkie/_script/panlex.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/__main__.py` & `selkie-0.25.1/src/selkie/cld/__main__.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/config.py` & `selkie-0.25.1/src/selkie/cld/config.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/core.py` & `selkie-0.25.1/src/selkie/cld/core.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/toplevel.py` & `selkie-0.25.1/src/selkie/cld/toplevel.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/app-scraps.py.disabled` & `selkie-0.25.1/src/selkie/cld/app/app-scraps.py.disabled`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/app_scraps.py.disabled` & `selkie-0.25.1/src/selkie/cld/app/app_scraps.py.disabled`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/auth.py` & `selkie-0.25.1/src/selkie/cld/app/auth.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/cgi.py` & `selkie-0.25.1/src/selkie/cld/app/cgi.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/client.py` & `selkie-0.25.1/src/selkie/cld/app/client.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/config.py` & `selkie-0.25.1/src/selkie/cld/app/config.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/core.py` & `selkie-0.25.1/src/selkie/cld/app/core.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/dualserver.py` & `selkie-0.25.1/src/selkie/cld/app/dualserver.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/dualserver_full.py` & `selkie-0.25.1/src/selkie/cld/app/dualserver_full.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/env.py` & `selkie-0.25.1/src/selkie/cld/app/env.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/handler.py` & `selkie-0.25.1/src/selkie/cld/app/handler.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/handler_orig.py.ignore` & `selkie-0.25.1/src/selkie/cld/app/handler_orig.py.ignore`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/html.py` & `selkie-0.25.1/src/selkie/cld/app/html.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/item.py` & `selkie-0.25.1/src/selkie/cld/app/item.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/log.py` & `selkie-0.25.1/src/selkie/cld/app/log.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/parse.py` & `selkie-0.25.1/src/selkie/cld/app/parse.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/request.py` & `selkie-0.25.1/src/selkie/cld/app/request.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/resources.py` & `selkie-0.25.1/src/selkie/cld/app/resources.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/response.py` & `selkie-0.25.1/src/selkie/cld/app/response.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/server.py` & `selkie-0.25.1/src/selkie/cld/app/server.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/server2_old.py` & `selkie-0.25.1/src/selkie/cld/app/server2_old.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/server_old.py` & `selkie-0.25.1/src/selkie/cld/app/server_old.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/session.py.disabled` & `selkie-0.25.1/src/selkie/cld/app/session.py.disabled`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/toplevel.py` & `selkie-0.25.1/src/selkie/cld/app/toplevel.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/ui-scraps.py` & `selkie-0.25.1/src/selkie/cld/app/ui-scraps.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/ui.py` & `selkie-0.25.1/src/selkie/cld/app/ui.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/ui_scraps.py.disabled` & `selkie-0.25.1/src/selkie/cld/app/ui_scraps.py.disabled`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/weblib.py` & `selkie-0.25.1/src/selkie/cld/app/weblib.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/app/wsgi.py` & `selkie-0.25.1/src/selkie/cld/app/wsgi.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/audio.py.todelete` & `selkie-0.25.1/src/selkie/cld/corpus/audio.py.todelete`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/core.py` & `selkie-0.25.1/src/selkie/cld/corpus/core.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/course.py` & `selkie-0.25.1/src/selkie/cld/corpus/course.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/drill.py` & `selkie-0.25.1/src/selkie/cld/corpus/drill.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/env.py` & `selkie-0.25.1/src/selkie/cld/corpus/env.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/export.py` & `selkie-0.25.1/src/selkie/cld/corpus/export.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/export_file.py` & `selkie-0.25.1/src/selkie/cld/corpus/export_file.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/langdb.py` & `selkie-0.25.1/src/selkie/cld/corpus/langdb.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/language.py` & `selkie-0.25.1/src/selkie/cld/corpus/language.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/lexicon.py` & `selkie-0.25.1/src/selkie/cld/corpus/lexicon.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/media.py` & `selkie-0.25.1/src/selkie/cld/corpus/media.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/rom.py` & `selkie-0.25.1/src/selkie/cld/corpus/rom.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/sim.py` & `selkie-0.25.1/src/selkie/cld/corpus/sim.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/text.py` & `selkie-0.25.1/src/selkie/cld/corpus/text.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/token-new.py.disabled` & `selkie-0.25.1/src/selkie/cld/corpus/token-new.py.disabled`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/token.py` & `selkie-0.25.1/src/selkie/cld/corpus/token.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/transcript.py` & `selkie-0.25.1/src/selkie/cld/corpus/transcript.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/corpus/user.py` & `selkie-0.25.1/src/selkie/cld/corpus/user.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/__init__.py` & `selkie-0.25.1/src/selkie/cld/db/__init__.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/core.py` & `selkie-0.25.1/src/selkie/cld/db/core.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/dir.py` & `selkie-0.25.1/src/selkie/cld/db/dir.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/disk.py` & `selkie-0.25.1/src/selkie/cld/db/disk.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/env.py` & `selkie-0.25.1/src/selkie/cld/db/env.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/file.py` & `selkie-0.25.1/src/selkie/cld/db/file.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/meta.py` & `selkie-0.25.1/src/selkie/cld/db/meta.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/db/permissions.py` & `selkie-0.25.1/src/selkie/cld/db/permissions.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/glab/eval.py` & `selkie-0.25.1/src/selkie/cld/glab/eval.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/glab/file.py` & `selkie-0.25.1/src/selkie/cld/glab/file.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/glab/functions.py` & `selkie-0.25.1/src/selkie/cld/glab/functions.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/glab/lang.py` & `selkie-0.25.1/src/selkie/cld/glab/lang.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/glab/ui.py` & `selkie-0.25.1/src/selkie/cld/glab/ui.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/seal/config.py` & `selkie-0.25.1/src/selkie/cld/seal/config.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/seal/io.py` & `selkie-0.25.1/src/selkie/cld/seal/io.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/seal/misc.py` & `selkie-0.25.1/src/selkie/cld/seal/misc.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/seal/rom.py` & `selkie-0.25.1/src/selkie/cld/seal/rom.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/seal/sh.py` & `selkie-0.25.1/src/selkie/cld/seal/sh.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/seal/xterm.py` & `selkie-0.25.1/src/selkie/cld/seal/xterm.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/audio.py` & `selkie-0.25.1/src/selkie/cld/ui/audio.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/conc.py` & `selkie-0.25.1/src/selkie/cld/ui/conc.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/corpus.py` & `selkie-0.25.1/src/selkie/cld/ui/corpus.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/course.py` & `selkie-0.25.1/src/selkie/cld/ui/course.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/file.py` & `selkie-0.25.1/src/selkie/cld/ui/file.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/igt.py` & `selkie-0.25.1/src/selkie/cld/ui/igt.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/language.py` & `selkie-0.25.1/src/selkie/cld/ui/language.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/lexicon.py` & `selkie-0.25.1/src/selkie/cld/ui/lexicon.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/media.py` & `selkie-0.25.1/src/selkie/cld/ui/media.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/page.py` & `selkie-0.25.1/src/selkie/cld/ui/page.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/rom.py` & `selkie-0.25.1/src/selkie/cld/ui/rom.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/text.py` & `selkie-0.25.1/src/selkie/cld/ui/text.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/toc.py` & `selkie-0.25.1/src/selkie/cld/ui/toc.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/cld/ui/users.py` & `selkie-0.25.1/src/selkie/cld/ui/users.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/__init__.py` & `selkie-0.25.1/src/selkie/corpus/__init__.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/drill.py` & `selkie-0.25.1/src/selkie/corpus/drill.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/langs.py` & `selkie-0.25.1/src/selkie/corpus/langs.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/lgc21.py` & `selkie-0.25.1/src/selkie/corpus/lgc21.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/lgc22.py` & `selkie-0.25.1/src/selkie/corpus/lgc22.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/rom.py` & `selkie-0.25.1/src/selkie/corpus/rom.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/romfile.py` & `selkie-0.25.1/src/selkie/corpus/romfile.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/corpus/user.py` & `selkie-0.25.1/src/selkie/corpus/user.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/__init__.py` & `selkie-0.25.1/src/selkie/data/__init__.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/bionlp.py` & `selkie-0.25.1/src/selkie/data/bionlp.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/brown.py` & `selkie-0.25.1/src/selkie/data/brown.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/census.py` & `selkie-0.25.1/src/selkie/data/census.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/dep.py` & `selkie-0.25.1/src/selkie/data/dep.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/idp.py` & `selkie-0.25.1/src/selkie/data/idp.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/panlex.py` & `selkie-0.25.1/src/selkie/data/panlex.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/panlex_old.py` & `selkie-0.25.1/src/selkie/data/panlex_old.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/panlex_scraps.py` & `selkie-0.25.1/src/selkie/data/panlex_scraps.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/perseus.py` & `selkie-0.25.1/src/selkie/data/perseus.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/propbank.py` & `selkie-0.25.1/src/selkie/data/propbank.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/ptb-rest.py.disabled` & `selkie-0.25.1/src/selkie/data/ptb-rest.py.disabled`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/ptb.py` & `selkie-0.25.1/src/selkie/data/ptb.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/udt.py` & `selkie-0.25.1/src/selkie/data/udt.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/wiktionary.py` & `selkie-0.25.1/src/selkie/data/wiktionary.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/wn.py` & `selkie-0.25.1/src/selkie/data/wn.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/census/README` & `selkie-0.25.1/src/selkie/data/census/README`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/census/both` & `selkie-0.25.1/src/selkie/data/census/both`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/census/dist.all.last` & `selkie-0.25.1/src/selkie/data/census/dist.all.last`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/census/dist.female.first` & `selkie-0.25.1/src/selkie/data/census/dist.female.first`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/census/dist.male.first` & `selkie-0.25.1/src/selkie/data/census/dist.male.first`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/census/methodology.txt` & `selkie-0.25.1/src/selkie/data/census/methodology.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/README` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/README`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/de-negra.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/de-negra.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-brown.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/en-brown.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-ptb.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/en-ptb.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.README` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/en-tweet.README`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/eu-eus3lb.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/eu-eus3lb.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ja-verbmobil.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ja-verbmobil.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/ko-sejong.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/ko-sejong.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/sl-sdt.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/sl-sdt.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/universal_tags.py.ignore` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/universal_tags.py.ignore`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/conll/2006/universal-pos-tags/zh-sinica.map` & `selkie-0.25.1/src/selkie/data/conll/2006/universal-pos-tags/zh-sinica.map`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/eng/eng.sents` & `selkie-0.25.1/src/selkie/data/eng/eng.sents`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/eng/main.decl` & `selkie-0.25.1/src/selkie/data/eng/main.decl`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/eng/main.g` & `selkie-0.25.1/src/selkie/data/eng/main.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/eng/main.lex` & `selkie-0.25.1/src/selkie/data/eng/main.lex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/eng/num.decl` & `selkie-0.25.1/src/selkie/data/eng/num.decl`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/eng/num.g` & `selkie-0.25.1/src/selkie/data/eng/num.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/EXAMPLES` & `selkie-0.25.1/src/selkie/data/examples/EXAMPLES`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/Makefile` & `selkie-0.25.1/src/selkie/data/examples/Makefile`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/class3.train` & `selkie-0.25.1/src/selkie/data/examples/class3.train`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/corp1.ef` & `selkie-0.25.1/src/selkie/data/examples/corp1.ef`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/corp2.ef` & `selkie-0.25.1/src/selkie/data/examples/corp2.ef`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/corp2.ef.1` & `selkie-0.25.1/src/selkie/data/examples/corp2.ef.1`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/corp2.ef.2` & `selkie-0.25.1/src/selkie/data/examples/corp2.ef.2`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/crime.kb` & `selkie-0.25.1/src/selkie/data/examples/crime.kb`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/deu.g` & `selkie-0.25.1/src/selkie/data/examples/deu.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/dream` & `selkie-0.25.1/src/selkie/data/examples/dream`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/drill.txt` & `selkie-0.25.1/src/selkie/data/examples/drill.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/form.html` & `selkie-0.25.1/src/selkie/data/examples/form.html`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/g6.lex` & `selkie-0.25.1/src/selkie/data/examples/g6.lex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/g7.g` & `selkie-0.25.1/src/selkie/data/examples/g7.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/g7.lex` & `selkie-0.25.1/src/selkie/data/examples/g7.lex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/g8.g` & `selkie-0.25.1/src/selkie/data/examples/g8.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/g8.sents` & `selkie-0.25.1/src/selkie/data/examples/g8.sents`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/intro.html` & `selkie-0.25.1/src/selkie/data/examples/intro.html`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/intro.tex` & `selkie-0.25.1/src/selkie/data/examples/intro.tex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/libsvm-1.test` & `selkie-0.25.1/src/selkie/data/examples/libsvm-1.test`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/libsvm-1.train` & `selkie-0.25.1/src/selkie/data/examples/libsvm-1.train`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/libsvm-2.train` & `selkie-0.25.1/src/selkie/data/examples/libsvm-2.train`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/libsvm-3.test` & `selkie-0.25.1/src/selkie/data/examples/libsvm-3.test`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/libsvm-3.train` & `selkie-0.25.1/src/selkie/data/examples/libsvm-3.train`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/make_repo_example` & `selkie-0.25.1/src/selkie/data/examples/make_repo_example`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/northwind.TextGrid` & `selkie-0.25.1/src/selkie/data/examples/northwind.TextGrid`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/notebook3.gl` & `selkie-0.25.1/src/selkie/data/examples/notebook3.gl`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/notebook_test.gl` & `selkie-0.25.1/src/selkie/data/examples/notebook_test.gl`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/notebook_test.output` & `selkie-0.25.1/src/selkie/data/examples/notebook_test.output`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/ptb.g` & `selkie-0.25.1/src/selkie/data/examples/ptb.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/ptb.lex` & `selkie-0.25.1/src/selkie/data/examples/ptb.lex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/ptb.test` & `selkie-0.25.1/src/selkie/data/examples/ptb.test`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sec_3` & `selkie-0.25.1/src/selkie/data/examples/sec_3`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sec_4` & `selkie-0.25.1/src/selkie/data/examples/sec_4`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sec_6` & `selkie-0.25.1/src/selkie/data/examples/sec_6`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sec_7` & `selkie-0.25.1/src/selkie/data/examples/sec_7`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sg2.g` & `selkie-0.25.1/src/selkie/data/examples/sg2.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sg2.lex` & `selkie-0.25.1/src/selkie/data/examples/sg2.lex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sg2a.g` & `selkie-0.25.1/src/selkie/data/examples/sg2a.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sg3.g` & `selkie-0.25.1/src/selkie/data/examples/sg3.g`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/sg3.lex` & `selkie-0.25.1/src/selkie/data/examples/sg3.lex`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/test123.mp3` & `selkie-0.25.1/src/selkie/data/examples/test123.mp3`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/test123.wav` & `selkie-0.25.1/src/selkie/data/examples/test123.wav`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/tuebingen.m4a` & `selkie-0.25.1/src/selkie/data/examples/tuebingen.m4a`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/tuebingen.mp3` & `selkie-0.25.1/src/selkie/data/examples/tuebingen.mp3`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/lexicon` & `selkie-0.25.1/src/selkie/data/examples/corpus.cld/langs/otw/lexicon`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/clips` & `selkie-0.25.1/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/clips`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/transcript` & `selkie-0.25.1/src/selkie/data/examples/corpus.cld/langs/otw/texts/16/audio/transcript`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/100.txt` & `selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/100.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/101.txt` & `selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/101.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/102.txt` & `selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/102.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/annotations/ghuse/arapesh/103.txt` & `selkie-0.25.1/src/selkie/data/examples/uc/annotations/ghuse/arapesh/103.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/cards/index.tab` & `selkie-0.25.1/src/selkie/data/examples/uc/cards/index.tab`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/kernel/ape/13.txt` & `selkie-0.25.1/src/selkie/data/examples/uc/kernel/ape/13.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/kernel/eng/15.txt` & `selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/15.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/kernel/eng/6.tok` & `selkie-0.25.1/src/selkie/data/examples/uc/kernel/eng/6.tok`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/kernel/sat/14.txt` & `selkie-0.25.1/src/selkie/data/examples/uc/kernel/sat/14.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/index.tab` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/index.tab`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/111/100` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/111/100`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/111/101` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/111/101`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/111/102` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/111/102`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/111/103` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/111/103`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/111/104` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/111/104`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/111/info` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/111/info`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/99/18` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/99/18`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/99/19` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/99/19`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/99/20` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/99/20`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/99/21` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/99/21`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/examples/uc/pages/99/22` & `selkie-0.25.1/src/selkie/data/examples/uc/pages/99/22`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/iso/639-2.txt` & `selkie-0.25.1/src/selkie/data/iso/639-2.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/iso/639-5.txt` & `selkie-0.25.1/src/selkie/data/iso/639-5.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/iso/639-3/iso-639-3-macrolanguages_20170131.tab` & `selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3-macrolanguages_20170131.tab`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_20170202.tab` & `selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3_20170202.tab`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_Name_Index_20170217.tab` & `selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3_Name_Index_20170217.tab`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/iso/639-3/iso-639-3_Retirements_20170131.tab` & `selkie-0.25.1/src/selkie/data/iso/639-3/iso-639-3_Retirements_20170131.tab`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/roms/korean.rom` & `selkie-0.25.1/src/selkie/data/roms/korean.rom`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/roms/salish.rom` & `selkie-0.25.1/src/selkie/data/roms/salish.rom`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/cog.png` & `selkie-0.25.1/src/selkie/data/seal/cog.png`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/entities.txt` & `selkie-0.25.1/src/selkie/data/seal/entities.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/external.gif` & `selkie-0.25.1/src/selkie/data/seal/external.gif`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/fourletter.txt` & `selkie-0.25.1/src/selkie/data/seal/fourletter.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/headrules_main.txt` & `selkie-0.25.1/src/selkie/data/seal/headrules_main.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/original_headrules_main.txt` & `selkie-0.25.1/src/selkie/data/seal/original_headrules_main.txt`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/ptb_filenames` & `selkie-0.25.1/src/selkie/data/seal/ptb_filenames`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/stemmer_stems` & `selkie-0.25.1/src/selkie/data/seal/stemmer_stems`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/data/seal/stemmer_words` & `selkie-0.25.1/src/selkie/data/seal/stemmer_words`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/eval.py` & `selkie-0.25.1/src/selkie/dp/eval.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/features.py` & `selkie-0.25.1/src/selkie/dp/features.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/mst.py` & `selkie-0.25.1/src/selkie/dp/mst.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/nivre.py` & `selkie-0.25.1/src/selkie/dp/nivre.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/nnproj.py` & `selkie-0.25.1/src/selkie/dp/nnproj.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/parser.py` & `selkie-0.25.1/src/selkie/dp/parser.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/tree.py` & `selkie-0.25.1/src/selkie/dp/tree.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/__init__.py` & `selkie-0.25.1/src/selkie/dp/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/cluster.py` & `selkie-0.25.1/src/selkie/dp/ml/cluster.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/experiment.py` & `selkie-0.25.1/src/selkie/dp/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/instance.py` & `selkie-0.25.1/src/selkie/dp/ml/instance.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/libsvm.py` & `selkie-0.25.1/src/selkie/dp/ml/libsvm.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/mat.py` & `selkie-0.25.1/src/selkie/dp/ml/mat.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/num.py` & `selkie-0.25.1/src/selkie/dp/ml/num.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/prob.py` & `selkie-0.25.1/src/selkie/dp/ml/prob.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/split.py` & `selkie-0.25.1/src/selkie/dp/ml/split.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/dp/ml/sym.py` & `selkie-0.25.1/src/selkie/dp/ml/sym.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/editor/webserver.py` & `selkie-0.25.1/src/selkie/editor/webserver.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/avs.py` & `selkie-0.25.1/src/selkie/nlp/avs.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/bot.py` & `selkie-0.25.1/src/selkie/nlp/bot.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/com.py` & `selkie-0.25.1/src/selkie/nlp/com.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/conc.py` & `selkie-0.25.1/src/selkie/nlp/conc.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/dep.py` & `selkie-0.25.1/src/selkie/nlp/dep.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/eng.py` & `selkie-0.25.1/src/selkie/nlp/eng.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/expr.py` & `selkie-0.25.1/src/selkie/nlp/expr.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/features.py` & `selkie-0.25.1/src/selkie/nlp/features.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/fsa.py` & `selkie-0.25.1/src/selkie/nlp/fsa.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/fst.py` & `selkie-0.25.1/src/selkie/nlp/fst.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/gdev.py` & `selkie-0.25.1/src/selkie/nlp/gdev.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/gen.py` & `selkie-0.25.1/src/selkie/nlp/gen.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/grammar.py` & `selkie-0.25.1/src/selkie/nlp/grammar.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/head.py` & `selkie-0.25.1/src/selkie/nlp/head.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/interp.py` & `selkie-0.25.1/src/selkie/nlp/interp.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/io.py` & `selkie-0.25.1/src/selkie/nlp/io.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/logic.py` & `selkie-0.25.1/src/selkie/nlp/logic.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/map.py` & `selkie-0.25.1/src/selkie/nlp/map.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/parser.py` & `selkie-0.25.1/src/selkie/nlp/parser.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/pretts.py` & `selkie-0.25.1/src/selkie/nlp/pretts.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/seq.py` & `selkie-0.25.1/src/selkie/nlp/seq.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/stemmer.py` & `selkie-0.25.1/src/selkie/nlp/stemmer.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/string.py` & `selkie-0.25.1/src/selkie/nlp/string.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/textgrid.py` & `selkie-0.25.1/src/selkie/nlp/textgrid.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/tok.py` & `selkie-0.25.1/src/selkie/nlp/tok.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlp/tree.py` & `selkie-0.25.1/src/selkie/nlp/tree.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlpx/avs.py` & `selkie-0.25.1/src/selkie/nlpx/avs.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlpx/expr.py` & `selkie-0.25.1/src/selkie/nlpx/expr.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlpx/features.py` & `selkie-0.25.1/src/selkie/nlpx/features.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlpx/gdev.py` & `selkie-0.25.1/src/selkie/nlpx/gdev.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlpx/grammar.py` & `selkie-0.25.1/src/selkie/nlpx/grammar.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlpx/parser.py` & `selkie-0.25.1/src/selkie/nlpx/parser.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/nlpx/tree.py` & `selkie-0.25.1/src/selkie/nlpx/tree.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/com.py` & `selkie-0.25.1/src/selkie/pyx/com.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/disk.py` & `selkie-0.25.1/src/selkie/pyx/disk.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/formats.py` & `selkie-0.25.1/src/selkie/pyx/formats.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/io.py` & `selkie-0.25.1/src/selkie/pyx/io.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/ipynb.py` & `selkie-0.25.1/src/selkie/pyx/ipynb.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/manifest.py` & `selkie-0.25.1/src/selkie/pyx/manifest.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/object.py` & `selkie-0.25.1/src/selkie/pyx/object.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/persist.py` & `selkie-0.25.1/src/selkie/pyx/persist.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/reflect.py` & `selkie-0.25.1/src/selkie/pyx/reflect.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/seq.py` & `selkie-0.25.1/src/selkie/pyx/seq.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/store.py` & `selkie-0.25.1/src/selkie/pyx/store.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/string.py` & `selkie-0.25.1/src/selkie/pyx/string.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/table.py` & `selkie-0.25.1/src/selkie/pyx/table.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/xml.py` & `selkie-0.25.1/src/selkie/pyx/xml.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/src/selkie/pyx/xterm.py` & `selkie-0.25.1/src/selkie/pyx/xterm.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/tests/checkdist.py` & `selkie-0.25.1/tests/checkdist.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/tests/run_tests.py` & `selkie-0.25.1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/tests/test_bot.py` & `selkie-0.25.1/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/tests/test_rom.py` & `selkie-0.25.1/tests/test_rom.py`

 * *Files identical despite different names*

### Comparing `selkie-0.25/tests/test_rom_graph` & `selkie-0.25.1/tests/test_rom_graph`

 * *Files identical despite different names*

### Comparing `selkie-0.25/.gitignore` & `selkie-0.25.1/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
-lib/
 lib64/
 parts/
 sdist/
 var/
 wheels/
 share/python-wheels/
 *.egg-info/
```

### Comparing `selkie-0.25/pyproject.toml` & `selkie-0.25.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "selkie"
 
 # When changing the version, remember to update:
 #     setup.py
 #     src/selkie/__init__.py
 #     docs/source/conf.py
 
-version = "0.25"
+version = "0.25.1"
 
 authors = [
   { name="Steven Abney", email="abney@umich.edu" },
 ]
 description = "Natural language processing and digital language description"
 readme = "README.rst"
 requires-python = ">=3.7"
@@ -22,8 +22,9 @@
     "Programming Language :: Python :: 3",
     "License :: Other/Proprietary License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/abney/selkie"
+"Documentation" = "https://selkie.readthedocs.io/"
 "Bug Tracker" = "https://github.com/abney/selkie/issues"
```

### Comparing `selkie-0.25/PKG-INFO` & `selkie-0.25.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: selkie
-Version: 0.25
+Version: 0.25.1
 Summary: Natural language processing and digital language description
 Project-URL: Homepage, https://github.com/abney/selkie
+Project-URL: Documentation, https://selkie.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/abney/selkie/issues
 Author-email: Steven Abney <abney@umich.edu>
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

