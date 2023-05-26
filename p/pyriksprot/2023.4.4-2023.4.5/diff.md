# Comparing `tmp/pyriksprot-2023.4.4.tar.gz` & `tmp/pyriksprot-2023.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot-2023.4.4.tar", max compression
+gzip compressed data, was "pyriksprot-2023.4.5.tar", max compression
```

## Comparing `pyriksprot-2023.4.4.tar` & `pyriksprot-2023.4.5.tar`

### file list

```diff
@@ -1,97 +1,98 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.4/LICENSE
--rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.4/README.md
--rw-r--r--   0        0        0     3597 2023-05-15 14:39:35.617625 pyriksprot-2023.4.4/pyproject.toml
--rw-r--r--   0        0        0     1248 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/__init__.py
--rw-r--r--   0        0        0      122 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/configuration/__init__.py
--rw-r--r--   0        0        0     5905 2023-05-15 14:37:02.779664 pyriksprot-2023.4.4/pyriksprot/configuration/config.py
--rw-r--r--   0        0        0     4915 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/configuration/inject.py
--rw-r--r--   0        0        0     2599 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/configuration/registry.py
--rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/corpus/__init__.py
--rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/corpus_index.py
--rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/iterate.py
--rw-r--r--   0        0        0      220 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/__init__.py
--rw-r--r--   0        0        0     2770 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/convert.py
--rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/iterate.py
--rw-r--r--   0        0        0     5368 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/parse.py
--rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/__init__.py
--rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
--rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
--rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
--rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
--rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
--rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
--rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
--rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
--rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
--rw-r--r--   0        0        0     2302 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/tf.py
--rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/corpus/tagged/__init__.py
--rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/tagged/iterate.py
--rw-r--r--   0        0        0     5790 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/tagged/persist.py
--rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/corpus/utility.py
--rw-r--r--   0        0        0        0 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/cwb/__init__.py
--rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/dehyphenation/__init__.py
--rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/dehyphenation/flair_dehyphen.py
--rw-r--r--   0        0        0     8902 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/dehyphenation/swe_dehyphen.py
--rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/dehyphenation/utility.py
--rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.4/pyriksprot/dispatch/__init__.py
--rw-r--r--   0        0        0    21600 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/dispatch/dispatch.py
--rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/dispatch/item.py
--rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/dispatch/merge.py
--rw-r--r--   0        0        0     4908 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/dispatch/utility.py
--rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/foss/README.md
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/foss/__init__.py
--rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/foss/pos_tags.py
--rw-r--r--   0        0        0     2335 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv
--rw-r--r--   0        0        0      945 2023-05-15 14:15:47.775429 pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv.saldo-tokens
--rw-r--r--   0        0        0  3493683 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/foss/resources/punkt-nltk-svenska.pickle
--rw-r--r--   0        0        0    13495 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/foss/sparv_tokenize.py
--rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/foss/stopwords.py
--rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/foss/untangle.py
--rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/gitchen.py
--rw-r--r--   0        0        0    13080 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/interface.py
--rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/metadata/__init__.py
--rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/codecs.py
--rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/config.py
--rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/generate.py
--rw-r--r--   0        0        0    14671 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/person.py
--rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/repository.py
--rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/subset.py
--rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/utility.py
--rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/utterance.py
--rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/metadata/verify.py
--rw-r--r--   0        0        0     1657 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/preprocess.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.4/pyriksprot/scripts/__init__.py
--rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/csv2pgsql.py
--rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/fix_speaker_notes.py
--rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/metadata2db.py
--rw-r--r--   0        0        0     2789 2023-04-19 09:21:24.587202 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech.py
--rw-r--r--   0        0        0     3475 2023-04-19 09:07:54.192237 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech_text.py
--rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2tagged.py
--rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2text.py
--rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2tfs.py
--rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/speaker_note2csv
--rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/speech_index.py
--rw-r--r--   0        0        0     1162 2023-04-19 09:21:24.591202 pyriksprot-2023.4.4/pyriksprot/scripts/subset_corpus.py
--rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/utils.py
--rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.4/pyriksprot/scripts/xml2csv
--rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/00_rename.sql
--rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/01_data_updates.sql
--rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/02_code_tables.sql
--rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/03_persons_of_interest.sql
--rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/04_terms_of_office.sql
--rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/05_person_party.sql
--rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/06_unknown.sql
--rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/09_cleanup.sql
--rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/sql/__init__.py
--rw-r--r--   0        0        0     7144 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/to_speech.py
--rw-r--r--   0        0        0    14138 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/utility.py
--rw-r--r--   0        0        0      266 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/__init__.py
--rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/workflows/_extract_speech_ids.py
--rw-r--r--   0        0        0     4429 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/extract_speech_text.py
--rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.4/pyriksprot/workflows/extract_tags.py
--rw-r--r--   0        0        0     4556 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/extract_text.py
--rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.4/pyriksprot/workflows/speech_index.py
--rw-r--r--   0        0        0     2230 2023-04-13 13:53:26.190262 pyriksprot-2023.4.4/pyriksprot/workflows/subset_corpus.py
--rw-r--r--   0        0        0     7476 2023-05-15 14:15:47.791429 pyriksprot-2023.4.4/pyriksprot/workflows/tag.py
--rw-r--r--   0        0        0     4159 2023-04-19 09:21:24.591202 pyriksprot-2023.4.4/pyriksprot/workflows/tf.py
--rw-r--r--   0        0        0     8856 1970-01-01 00:00:00.000000 pyriksprot-2023.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:38.857587 pyriksprot-2023.4.5/LICENSE
+-rw-r--r--   0        0        0     7547 2023-04-13 10:55:09.499216 pyriksprot-2023.4.5/README.md
+-rw-r--r--   0        0        0     3672 2023-05-26 08:44:19.302847 pyriksprot-2023.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1284 2023-05-26 07:51:45.656946 pyriksprot-2023.4.5/pyriksprot/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/configuration/__init__.py
+-rw-r--r--   0        0        0     5905 2023-05-16 07:22:44.405874 pyriksprot-2023.4.5/pyriksprot/configuration/config.py
+-rw-r--r--   0        0        0     4915 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/configuration/inject.py
+-rw-r--r--   0        0        0     2599 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/configuration/registry.py
+-rw-r--r--   0        0        0      152 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/corpus/__init__.py
+-rw-r--r--   0        0        0     4111 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/corpus/corpus_index.py
+-rw-r--r--   0        0        0    11973 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/corpus/iterate.py
+-rw-r--r--   0        0        0      220 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/__init__.py
+-rw-r--r--   0        0        0     2770 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/convert.py
+-rw-r--r--   0        0        0     2467 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/iterate.py
+-rw-r--r--   0        0        0     5368 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/parse.py
+-rw-r--r--   0        0        0        0 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/__init__.py
+-rw-r--r--   0        0        0      244 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/templates/__init__.py
+-rw-r--r--   0        0        0      330 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.txt.jinja
+-rw-r--r--   0        0        0      447 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/templates/paragraphs.xml.jinja
+-rw-r--r--   0        0        0      352 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/templates/speeches.cdata.xml.jinja
+-rw-r--r--   0        0        0      278 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/templates/speeches.txt.jinja
+-rw-r--r--   0        0        0      342 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/templates/speeches.xml.jinja
+-rw-r--r--   0        0        0     1779 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt
+-rw-r--r--   0        0        0     1578 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt
+-rw-r--r--   0        0        0     1201 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt
+-rw-r--r--   0        0        0     2302 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/tf.py
+-rw-r--r--   0        0        0      170 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/corpus/tagged/__init__.py
+-rw-r--r--   0        0        0     1630 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/corpus/tagged/iterate.py
+-rw-r--r--   0        0        0     6307 2023-05-26 08:21:06.316335 pyriksprot-2023.4.5/pyriksprot/corpus/tagged/persist.py
+-rw-r--r--   0        0        0     1515 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/corpus/utility.py
+-rw-r--r--   0        0        0      113 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/dehyphenation/__init__.py
+-rw-r--r--   0        0        0     1693 2022-03-14 19:05:38.861587 pyriksprot-2023.4.5/pyriksprot/dehyphenation/flair_dehyphen.py
+-rw-r--r--   0        0        0     8902 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/dehyphenation/swe_dehyphen.py
+-rw-r--r--   0        0        0      843 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/dehyphenation/utility.py
+-rw-r--r--   0        0        0      438 2023-01-24 09:13:07.490512 pyriksprot-2023.4.5/pyriksprot/dispatch/__init__.py
+-rw-r--r--   0        0        0    21600 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/dispatch/dispatch.py
+-rw-r--r--   0        0        0     2100 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/dispatch/item.py
+-rw-r--r--   0        0        0     4594 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/dispatch/merge.py
+-rw-r--r--   0        0        0     4939 2023-05-26 08:38:53.738304 pyriksprot-2023.4.5/pyriksprot/dispatch/utility.py
+-rw-r--r--   0        0        0       40 2022-03-14 19:05:38.861587 pyriksprot-2023.4.5/pyriksprot/foss/README.md
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.5/pyriksprot/foss/__init__.py
+-rw-r--r--   0        0        0    12236 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/foss/pos_tags.py
+-rw-r--r--   0        0        0     2335 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/foss/resources/bettertokenizer.sv
+-rw-r--r--   0        0        0      945 2023-05-15 14:15:47.775429 pyriksprot-2023.4.5/pyriksprot/foss/resources/bettertokenizer.sv.saldo-tokens
+-rw-r--r--   0        0        0  3493683 2023-05-15 14:15:47.791429 pyriksprot-2023.4.5/pyriksprot/foss/resources/punkt-nltk-svenska.pickle
+-rw-r--r--   0        0        0    13495 2023-05-15 14:15:47.791429 pyriksprot-2023.4.5/pyriksprot/foss/sparv_tokenize.py
+-rw-r--r--   0        0        0     1420 2022-03-14 19:05:38.861587 pyriksprot-2023.4.5/pyriksprot/foss/stopwords.py
+-rw-r--r--   0        0        0     6119 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/foss/untangle.py
+-rw-r--r--   0        0        0     3582 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/gitchen.py
+-rw-r--r--   0        0        0    17812 2023-05-26 07:51:45.656946 pyriksprot-2023.4.5/pyriksprot/interface.py
+-rw-r--r--   0        0        0      769 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/metadata/__init__.py
+-rw-r--r--   0        0        0     5145 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/codecs.py
+-rw-r--r--   0        0        0    12475 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/config.py
+-rw-r--r--   0        0        0     7737 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/generate.py
+-rw-r--r--   0        0        0    14685 2023-05-26 07:51:45.656946 pyriksprot-2023.4.5/pyriksprot/metadata/person.py
+-rw-r--r--   0        0        0     3125 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/repository.py
+-rw-r--r--   0        0        0     2373 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/subset.py
+-rw-r--r--   0        0        0     6384 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/utility.py
+-rw-r--r--   0        0        0     1461 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/utterance.py
+-rw-r--r--   0        0        0     4296 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/metadata/verify.py
+-rw-r--r--   0        0        0     1657 2023-05-15 14:15:47.791429 pyriksprot-2023.4.5/pyriksprot/preprocess.py
+-rw-r--r--   0        0        0        0 2022-03-14 19:05:38.861587 pyriksprot-2023.4.5/pyriksprot/scripts/__init__.py
+-rw-r--r--   0        0        0     1596 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/scripts/csv2pgsql.py
+-rw-r--r--   0        0        0     1648 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/scripts/fix_speaker_notes.py
+-rw-r--r--   0        0        0     3543 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/scripts/metadata2db.py
+-rw-r--r--   0        0        0     2789 2023-04-19 09:21:24.587202 pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2speech.py
+-rw-r--r--   0        0        0     3475 2023-04-19 09:07:54.192237 pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2speech_text.py
+-rw-r--r--   0        0        0     2902 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2tagged.py
+-rw-r--r--   0        0        0     4650 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2text.py
+-rw-r--r--   0        0        0      487 2022-03-31 10:06:39.806371 pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2tfs.py
+-rw-r--r--   0        0        0     3157 2023-05-26 07:51:45.656946 pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2vrt.py
+-rwxr-xr-x   0        0        0      680 2023-01-24 09:13:07.494512 pyriksprot-2023.4.5/pyriksprot/scripts/speaker_note2csv
+-rw-r--r--   0        0        0     2568 2023-01-24 09:13:07.494512 pyriksprot-2023.4.5/pyriksprot/scripts/speech_index.py
+-rw-r--r--   0        0        0     1162 2023-04-19 09:21:24.591202 pyriksprot-2023.4.5/pyriksprot/scripts/subset_corpus.py
+-rw-r--r--   0        0        0     5266 2023-01-24 09:13:07.494512 pyriksprot-2023.4.5/pyriksprot/scripts/utils.py
+-rwxr-xr-x   0        0        0      541 2023-01-24 09:13:07.494512 pyriksprot-2023.4.5/pyriksprot/scripts/xml2csv
+-rw-r--r--   0        0        0      599 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/00_rename.sql
+-rw-r--r--   0        0        0     4522 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/01_data_updates.sql
+-rw-r--r--   0        0        0     2592 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/02_code_tables.sql
+-rw-r--r--   0        0        0     2199 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/03_persons_of_interest.sql
+-rw-r--r--   0        0        0     5973 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/04_terms_of_office.sql
+-rw-r--r--   0        0        0     2818 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/05_person_party.sql
+-rw-r--r--   0        0        0     1707 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/06_unknown.sql
+-rw-r--r--   0        0        0     1344 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/09_cleanup.sql
+-rw-r--r--   0        0        0      204 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/sql/__init__.py
+-rw-r--r--   0        0        0     7204 2023-05-26 07:51:45.656946 pyriksprot-2023.4.5/pyriksprot/to_speech.py
+-rw-r--r--   0        0        0    14580 2023-05-26 07:51:45.660946 pyriksprot-2023.4.5/pyriksprot/utility.py
+-rw-r--r--   0        0        0      266 2023-05-15 14:15:47.791429 pyriksprot-2023.4.5/pyriksprot/workflows/__init__.py
+-rw-r--r--   0        0        0     1415 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/workflows/_extract_speech_ids.py
+-rw-r--r--   0        0        0     1576 2023-05-26 07:51:45.660946 pyriksprot-2023.4.5/pyriksprot/workflows/export_vrt.py
+-rw-r--r--   0        0        0     4429 2023-05-15 14:15:47.791429 pyriksprot-2023.4.5/pyriksprot/workflows/extract_speech_text.py
+-rw-r--r--   0        0        0     6449 2023-04-13 10:55:09.503216 pyriksprot-2023.4.5/pyriksprot/workflows/extract_tags.py
+-rw-r--r--   0        0        0     4556 2023-05-15 14:15:47.791429 pyriksprot-2023.4.5/pyriksprot/workflows/extract_text.py
+-rw-r--r--   0        0        0     3254 2023-03-27 13:27:29.397414 pyriksprot-2023.4.5/pyriksprot/workflows/speech_index.py
+-rw-r--r--   0        0        0     2230 2023-04-13 13:53:26.190262 pyriksprot-2023.4.5/pyriksprot/workflows/subset_corpus.py
+-rw-r--r--   0        0        0     7563 2023-05-26 07:51:45.660946 pyriksprot-2023.4.5/pyriksprot/workflows/tag.py
+-rw-r--r--   0        0        0     4159 2023-04-19 09:21:24.591202 pyriksprot-2023.4.5/pyriksprot/workflows/tf.py
+-rw-r--r--   0        0        0     8791 1970-01-01 00:00:00.000000 pyriksprot-2023.4.5/PKG-INFO
```

### Comparing `pyriksprot-2023.4.4/LICENSE` & `pyriksprot-2023.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/README.md` & `pyriksprot-2023.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyproject.toml` & `pyriksprot-2023.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksprot"
-version = "2023.4.4"
+version = "2023.4.5"
 description = "Python API for Riksdagens Protokoll"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "pyriksprot" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -35,14 +35,15 @@
 unidecode = "^1.3.6"
 pygit2 = "^1.11.1"
 sqlalchemy = "^2.0.6"
 psycopg2-binary = "^2.9.5"
 nltk = "^3.8.1"
 dynaconf = "^3.1.12"
 pathvalidate = "^2.5.2"
+cwb-ccc = "^0.11.8"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 coverage = "*"
 flake8 = "*"
 flake8-black = "*"
 isort = "*"
@@ -54,14 +55,15 @@
 pytest-cov = "*"
 pyinstrument = "*"
 pytest-codeblocks = "*"
 
 [tool.poetry.scripts]
 riksprot2any = "pyriksprot.scripts.riksprot2any:main"
 riksprot2tfs = "pyriksprot.scripts.riksprot2tfs:main"
+riksprot2vrt = "pyriksprot.scripts.riksprot2vrt:main"
 riksprot2text = "pyriksprot.scripts.riksprot2text:main"
 riksprot2speech = "pyriksprot.scripts.riksprot2speech:main"
 riksprot2speech_text = "pyriksprot.scripts.riksprot2speech_text:main"
 subset-corpus = "pyriksprot.scripts.subset_corpus:main"
 speech-index = "pyriksprot.scripts.speech_index:main"
 metadata2db = "pyriksprot.scripts.metadata2db:main"
 
@@ -126,18 +128,14 @@
 disallow_untyped_defs = true
 ignore_missing_imports = true
 show_error_codes = true
 strict_optional = false
 warn_no_return = false
 python_version = 3.8
 
-[build-system]
-requires = ["setuptools", "poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.pyright]
 include = ["pyriksprot", "tests"]
 exclude = [
     ".git",
     ".vscode",
     "**/__init__.py",
     "**/__pycache__",
@@ -151,7 +149,12 @@
 reportMissingTypeStubs = false
 reportUntypedFunctionDecorator = false
 reportUntypedClassDecorator = true
 reportOptionalSubscript = false
 reportOptionalMemberAccess = false
 reportOptionalCall = false
 pythonVersion = "3.11"
+
+[build-system]
+requires = ["setuptools", "poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/__init__.py` & `pyriksprot-2023.4.5/pyriksprot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,18 +32,20 @@
     strip_path_and_extension,
     strip_paths,
     sync_delta_names,
     temporary_file,
     touch,
     ts_data_path,
     unlink,
+    xml_escape,
 )
 from .workflows import compute_term_frequencies, extract_corpus_tags, extract_corpus_text
 from .workflows.tag import (
     ITagger,
     ITaggerFactory,
     TaggedDocument,
+    TaggerProvider,
     TaggerRegistry,
     tag_protocol,
     tag_protocol_xml,
     tag_protocols,
 )
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/configuration/config.py` & `pyriksprot-2023.4.5/pyriksprot/configuration/config.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/configuration/inject.py` & `pyriksprot-2023.4.5/pyriksprot/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/configuration/registry.py` & `pyriksprot-2023.4.5/pyriksprot/configuration/registry.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/corpus_index.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/corpus_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/iterate.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/convert.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/convert.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/iterate.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/parse.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/parse.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt` & `pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_csv.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt` & `pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/xslt/parla_clarin_to_xml.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt` & `pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/resources/xslt/test.xslt`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/parlaclarin/tf.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/parlaclarin/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/tagged/iterate.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/tagged/iterate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/tagged/persist.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/tagged/persist.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,32 +105,46 @@
             utterances: List[interface.Utterance] = PROTOCOL_LOADERS.get(ext)(data_str)
 
             protocol: interface.Protocol = interface.Protocol(utterances=utterances, **metadata, speaker_notes={})
 
             return protocol
 
 
-def load_protocols(source: str | List, file_pattern: str = 'prot-*.zip') -> Iterable[interface.Protocol]:
-    return (p for p in (load_protocol(filename) for filename in glob_protocols(source, file_pattern)) if p is not None)
+def load_protocols(source: str | list[str], pattern: str = '**/prot-*.zip') -> Iterable[interface.Protocol]:
+    """Loads all protocols in `source` folder, matching `file_pattern`"""
+    filenames: list[str] = glob_protocols(source, pattern)
+    for p in (load_protocol(filename) for filename in filenames):
+        if p is None:
+            continue
+        yield p
+
+
+def glob_protocols(source: str, pattern: str = None, strip_path: bool = False):
+    """Glob for protocols in `source` folder, matching `file_pattern`"""
+    filenames: list[str] = []
+    if isinstance(source, str):
+        path: str = jj(source, pattern) if pattern else source
+        filenames = glob.glob(path, recursive=True)
+    elif isinstance(source, list):
+        filenames = source
 
-
-def glob_protocols(source: str, file_pattern: str, strip_path: bool = False):
-    filenames: List[str] = (
-        glob.glob(os.path.join(source, file_pattern), recursive=True)
+    filenames: list[str] = (
+        glob.glob(jj(source, pattern), recursive=True)
         if isinstance(source, str)
         else source
         if isinstance(source, list)
         else []
     )
     if strip_path:
         filenames = strip_paths(filenames)
     return filenames
 
 
 def validate_checksum(filename: str, checksum: str) -> bool:
+    """Validate that computed checksum of a protocol matches `checksum`."""
     if not os.path.isfile(filename):
         return False
     metadata: dict = load_metadata(filename)
     if metadata is None:
         return False
     return checksum == metadata.get('checksum', 'oo')
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/corpus/utility.py` & `pyriksprot-2023.4.5/pyriksprot/corpus/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/dehyphenation/flair_dehyphen.py` & `pyriksprot-2023.4.5/pyriksprot/dehyphenation/flair_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/dehyphenation/swe_dehyphen.py` & `pyriksprot-2023.4.5/pyriksprot/dehyphenation/swe_dehyphen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/dehyphenation/utility.py` & `pyriksprot-2023.4.5/pyriksprot/dehyphenation/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/dispatch/dispatch.py` & `pyriksprot-2023.4.5/pyriksprot/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/dispatch/item.py` & `pyriksprot-2023.4.5/pyriksprot/dispatch/item.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/dispatch/merge.py` & `pyriksprot-2023.4.5/pyriksprot/dispatch/merge.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/dispatch/utility.py` & `pyriksprot-2023.4.5/pyriksprot/dispatch/utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def hashcoder(item: iterate.ProtocolSegment, source_item: corpus_index.ICorpusSourceItem) -> tuple[dict, str, str]:
         """Compute hash for item, speaker and source item. Return values, hash string and hash code"""
         assert issubclass(type(source_item), corpus_index.ICorpusSourceItem)
         parts: dict[str, str | int] = {
             # **take(item.speaker_info.asdict(), grouping_keys),
             # **take(source_item.to_dict(), grouping_keys),
             # **take(item.to_dict(), grouping_keys),
-            **probe(item.speaker_info.term_of_office, grouping_keys),
+            **(probe(item.speaker_info.term_of_office, grouping_keys) if item.speaker_info else {}),
             **probe(item.speaker_info, grouping_keys),
             **probe(source_item, grouping_keys),
             **probe(item, grouping_keys),
         }
         missing: set[str] = grouping_keys - set(parts.keys())
         if len(missing) > 0:
             raise ValueError(f"unknown keys: {', '.join(list(missing))}")
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/foss/pos_tags.py` & `pyriksprot-2023.4.5/pyriksprot/foss/pos_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv` & `pyriksprot-2023.4.5/pyriksprot/foss/resources/bettertokenizer.sv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/foss/resources/bettertokenizer.sv.saldo-tokens` & `pyriksprot-2023.4.5/pyriksprot/foss/resources/bettertokenizer.sv.saldo-tokens`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/foss/resources/punkt-nltk-svenska.pickle` & `pyriksprot-2023.4.5/pyriksprot/foss/resources/punkt-nltk-svenska.pickle`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/foss/sparv_tokenize.py` & `pyriksprot-2023.4.5/pyriksprot/foss/sparv_tokenize.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/foss/stopwords.py` & `pyriksprot-2023.4.5/pyriksprot/foss/stopwords.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/foss/untangle.py` & `pyriksprot-2023.4.5/pyriksprot/foss/untangle.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/gitchen.py` & `pyriksprot-2023.4.5/pyriksprot/gitchen.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/__init__.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/codecs.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/codecs.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/config.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/config.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/generate.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/generate.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/person.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/person.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         return self.start_date.year if self._is_date(self.start_date) else 0
 
     @property
     def end_year(self) -> int:
         return self.end_date.year if self._is_date(self.end_date) else 9999
 
     def covers(self, pit: int | datetime.date) -> bool:
-        if isinstance(pit, int):
+        if isinstance(pit, (int, np.integer)):
             return self.start_year <= pit <= self.end_year
         return self.start_date <= pit <= self.end_date
 
     @property
     def is_closed(self) -> bool:
         return self._is_date(self.start_year) and self._is_date(self.end_year)
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/repository.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/repository.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/subset.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/subset.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/utility.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/utility.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/utterance.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/utterance.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/metadata/verify.py` & `pyriksprot-2023.4.5/pyriksprot/metadata/verify.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/preprocess.py` & `pyriksprot-2023.4.5/pyriksprot/preprocess.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/csv2pgsql.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/csv2pgsql.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/fix_speaker_notes.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/fix_speaker_notes.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/metadata2db.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/metadata2db.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2speech.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2speech_text.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2speech_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2tagged.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2tagged.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/riksprot2text.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/riksprot2text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/speaker_note2csv` & `pyriksprot-2023.4.5/pyriksprot/scripts/speaker_note2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/speech_index.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/subset_corpus.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/subset_corpus.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/utils.py` & `pyriksprot-2023.4.5/pyriksprot/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/scripts/xml2csv` & `pyriksprot-2023.4.5/pyriksprot/scripts/xml2csv`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/00_rename.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/00_rename.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/01_data_updates.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/01_data_updates.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/02_code_tables.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/02_code_tables.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/03_persons_of_interest.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/03_persons_of_interest.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/04_terms_of_office.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/04_terms_of_office.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/05_person_party.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/05_person_party.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/06_unknown.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/06_unknown.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/sql/09_cleanup.sql` & `pyriksprot-2023.4.5/pyriksprot/sql/09_cleanup.sql`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/to_speech.py` & `pyriksprot-2023.4.5/pyriksprot/to_speech.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
 import abc
 import inspect
 from collections import defaultdict
 from enum import Enum
 from itertools import groupby
-from typing import Type
+from typing import TYPE_CHECKING, Type
 
 from loguru import logger
 
-from .interface import Protocol, Speech, Utterance
+from .interface import Speech
+
+if TYPE_CHECKING:
+    from .interface import Protocol, Utterance
 
 # pylint: disable=too-many-arguments, no-member
 
 
 class MergeStrategyType(str, Enum):
     who = 'who'
     who_sequence = 'who_sequence'
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/utility.py` & `pyriksprot-2023.4.5/pyriksprot/utility.py`

 * *Files 3% similar despite different names*

```diff
@@ -452,14 +452,39 @@
     return {v: k for k, v in d.items()}
 
 
 def props(cls: Type) -> list[str]:
     return [i for i in cls.__dict__.keys() if i[:1] != '_']
 
 
+XML_ESCAPES = str.maketrans(
+    {
+        "<": "&lt;",
+        ">": "&gt;",
+        "&": "&amp;",
+        "'": "&apos;",
+        '"': "&quot;",
+    }
+)
+
+
+def xml_escape(txt: str) -> str:
+    return txt.translate(XML_ESCAPES)
+
+
+def xml_unescape(txt: str) -> str:
+    return (
+        txt.replace("&lt;", "<")
+        .replace("&gt;", ">")
+        .replace("&amp;", "&")
+        .replace("&apos;", "'")
+        .replace("&quot;", '"')
+    )
+
+
 # def register(registry: dict | Type[Any], key: str = None):
 #     if not isinstance(registry, dict):
 #         if not hasattr(registry, "registry"):
 #             registry.registry = {}
 #             registry = registry.registry
 
 #     def registrar(func):
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/_extract_speech_ids.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/_extract_speech_ids.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/extract_speech_text.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/extract_speech_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/extract_tags.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/extract_tags.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/extract_text.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/extract_text.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/speech_index.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/speech_index.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/subset_corpus.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/subset_corpus.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/tag.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from .. import interface
 from .. import preprocess as pp
 from ..configuration import ConfigValue, inject_config
 from ..utility import ensure_path, strip_path_and_extension, touch, unlink
 
 METADATA_FILENAME: str = 'metadata.json'
+TAGGED_COLUMNS: list[str] = ['token', 'lemma', 'pos', 'xpos', 'sentence_id']
 
 TaggedDocument = Mapping[str, List[str]]
 
 
 class ITaggerFactory(abc.ABC):
     identifier: str = "undefined"
 
@@ -60,30 +61,32 @@
     @abc.abstractmethod
     def _to_dict(self, tagged_document: Any) -> TaggedDocument:
         return {}
 
     @staticmethod
     def to_csv(tagged_document: TaggedDocument, sep='\t') -> str:
         """Converts a TaggedDocument to a TSV string"""
-        columns: list[str] = [c for c in ['token', 'lemma', 'pos', 'xpos', 'sentence_id'] if c in tagged_document]
+        columns: list[str] = [c for c in TAGGED_COLUMNS if c in tagged_document]
         csv_str: str = (
             sep.join(columns)
             + '\n'
             + '\n'.join(
                 sep.join(str(tagged_document[c][i]) for c in columns) for i in range(0, len(tagged_document['token']))
             )
         )
         return csv_str
 
     def preprocess(self, text: str) -> str:
         """Transform `text` with preprocessors."""
         text: str = reduce(lambda res, f: f(res), self.preprocessors, text)
         return text
 
-    def resolve_preprocessors(self, preprocessors: str | list[Callable[[str], str] | str]):
+    def resolve_preprocessors(
+        self, preprocessors: str | list[Callable[[str], str] | str]
+    ) -> list[Callable[[str], str]]:
         if isinstance(preprocessors, str):
             preprocessors = preprocessors.split(",")
 
         if not any(isinstance(p, str) for p in preprocessors):
             return preprocessors
 
         self.is_satisfied(preprocessors)
```

### Comparing `pyriksprot-2023.4.4/pyriksprot/workflows/tf.py` & `pyriksprot-2023.4.5/pyriksprot/workflows/tf.py`

 * *Files identical despite different names*

### Comparing `pyriksprot-2023.4.4/PKG-INFO` & `pyriksprot-2023.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: pyriksprot
-Version: 2023.4.4
+Version: 2023.4.5
 Summary: Python API for Riksdagens Protokoll
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
-Requires-Python: >=3.11.0,<3.12.0
+Requires-Python: ==3.11.*
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: Jinja2
 Requires-Dist: click
+Requires-Dist: cwb-ccc (>=0.11.8,<0.12.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: loguru
 Requires-Dist: lz4
 Requires-Dist: more-itertools
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pandas
 Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
```

