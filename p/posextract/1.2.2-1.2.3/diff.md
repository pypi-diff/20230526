# Comparing `tmp/posextract-1.2.2.tar.gz` & `tmp/posextract-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posextract-1.2.2.tar", last modified: Wed Mar 15 18:36:58 2023, max compression
+gzip compressed data, was "posextract-1.2.3.tar", last modified: Fri May 26 20:08:15 2023, max compression
```

## Comparing `posextract-1.2.2.tar` & `posextract-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-03-15 18:36:58.120089 posextract-1.2.2/
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     1093 2023-01-26 20:31:45.000000 posextract-1.2.2/LICENSE
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     5046 2023-03-15 18:36:58.120089 posextract-1.2.2/PKG-INFO
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     3027 2023-01-26 20:31:45.000000 posextract-1.2.2/README.md
-drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-03-15 18:36:58.112089 posextract-1.2.2/posextract.egg-info/
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     5046 2023-03-15 18:36:58.000000 posextract-1.2.2/posextract.egg-info/PKG-INFO
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      539 2023-03-15 18:36:58.000000 posextract-1.2.2/posextract.egg-info/SOURCES.txt
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)        1 2023-03-15 18:36:58.000000 posextract-1.2.2/posextract.egg-info/dependency_links.txt
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)       71 2023-03-15 18:36:58.000000 posextract-1.2.2/posextract.egg-info/requires.txt
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)       11 2023-03-15 18:36:58.000000 posextract-1.2.2/posextract.egg-info/top_level.txt
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     1036 2023-03-15 18:36:44.000000 posextract-1.2.2/pyproject.toml
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)       38 2023-03-15 18:36:58.120089 posextract-1.2.2/setup.cfg
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      172 2023-01-26 20:31:45.000000 posextract-1.2.2/setup.py
-drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-03-15 18:36:58.112089 posextract-1.2.2/src/
-drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-03-15 18:36:58.120089 posextract-1.2.2/src/posextract/
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      132 2023-01-26 20:31:45.000000 posextract-1.2.2/src/posextract/__init__.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     6271 2023-03-04 19:33:12.000000 posextract-1.2.2/src/posextract/adj_noun_pairs.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      124 2023-01-26 20:31:45.000000 posextract-1.2.2/src/posextract/download_language_model.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)    10908 2023-03-15 18:35:47.000000 posextract-1.2.2/src/posextract/grammatical_triples.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     7942 2023-01-26 20:31:45.000000 posextract-1.2.2/src/posextract/rules.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     5909 2023-03-04 19:33:12.000000 posextract-1.2.2/src/posextract/subj_verb_pairs.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     6674 2023-03-07 15:46:25.000000 posextract-1.2.2/src/posextract/traversal.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     3466 2023-03-06 21:27:28.000000 posextract-1.2.2/src/posextract/triple_extraction.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     4755 2023-03-15 18:35:47.000000 posextract-1.2.2/src/posextract/util.py
--rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     6773 2023-03-07 23:52:55.000000 posextract-1.2.2/src/posextract/verb_phrase.py
-drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-03-15 18:36:58.120089 posextract-1.2.2/tests/
--rwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)      862 2023-01-26 20:31:45.000000 posextract-1.2.2/tests/test.py
+drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-05-26 20:08:15.552857 posextract-1.2.3/
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     1093 2023-01-26 20:31:45.000000 posextract-1.2.3/LICENSE
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     5380 2023-05-26 20:08:15.552857 posextract-1.2.3/PKG-INFO
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     3361 2023-05-26 20:05:00.000000 posextract-1.2.3/README.md
+drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-05-26 20:08:15.544857 posextract-1.2.3/posextract.egg-info/
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     5380 2023-05-26 20:08:15.000000 posextract-1.2.3/posextract.egg-info/PKG-INFO
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      539 2023-05-26 20:08:15.000000 posextract-1.2.3/posextract.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)        1 2023-05-26 20:08:15.000000 posextract-1.2.3/posextract.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)       71 2023-05-26 20:08:15.000000 posextract-1.2.3/posextract.egg-info/requires.txt
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)       11 2023-05-26 20:08:15.000000 posextract-1.2.3/posextract.egg-info/top_level.txt
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     1036 2023-05-26 20:07:51.000000 posextract-1.2.3/pyproject.toml
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)       38 2023-05-26 20:08:15.552857 posextract-1.2.3/setup.cfg
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      172 2023-01-26 20:31:45.000000 posextract-1.2.3/setup.py
+drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-05-26 20:08:15.544857 posextract-1.2.3/src/
+drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-05-26 20:08:15.552857 posextract-1.2.3/src/posextract/
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      132 2023-01-26 20:31:45.000000 posextract-1.2.3/src/posextract/__init__.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     6271 2023-03-04 19:33:12.000000 posextract-1.2.3/src/posextract/adj_noun_pairs.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)      124 2023-01-26 20:31:45.000000 posextract-1.2.3/src/posextract/download_language_model.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)    12859 2023-05-26 20:07:08.000000 posextract-1.2.3/src/posextract/grammatical_triples.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     7942 2023-01-26 20:31:45.000000 posextract-1.2.3/src/posextract/rules.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     5909 2023-03-04 19:33:12.000000 posextract-1.2.3/src/posextract/subj_verb_pairs.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     6674 2023-03-07 15:46:25.000000 posextract-1.2.3/src/posextract/traversal.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     3466 2023-03-06 21:27:28.000000 posextract-1.2.3/src/posextract/triple_extraction.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     4921 2023-05-26 19:57:50.000000 posextract-1.2.3/src/posextract/util.py
+-rw-rw-r--   0 stephbuon  (1000) stephbuon  (1000)     6773 2023-03-07 23:52:55.000000 posextract-1.2.3/src/posextract/verb_phrase.py
+drwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)        0 2023-05-26 20:08:15.552857 posextract-1.2.3/tests/
+-rwxrwxr-x   0 stephbuon  (1000) stephbuon  (1000)      862 2023-01-26 20:31:45.000000 posextract-1.2.3/tests/test.py
```

### Comparing `posextract-1.2.2/LICENSE` & `posextract-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/PKG-INFO` & `posextract-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posextract
-Version: 1.2.2
+Version: 1.2.3
 Summary: Grammatical information extraction methods designed for the analysis of historical and contemporary textual corpora.
 Author-email: Steph Buongiorno <steph.buon@gmail.com>, Alexander Cerpa <acerpa@smu.edu>
 License: MIT License
         
         Copyright (c) 2021 Steph Buongiorno and Alexander Cerpa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,14 +75,22 @@
 
 for triple in triples:
     print(triple)
 
 # Output: Landlords exercise oppression, soldiers were ill
 ```
 
+Extract grammatical triples using different options from default: 
+
+```
+from posextract.util import TripleExtractorOptions
+
+triples = grammatical_triples.extract(sent, TripleExtractorOptions(prep_phrase = True))
+```
+
 Or extract adjectives and the nouns they modify. 
 
 ```
 from posextract import adj_noun_pairs
 
 adj_noun = adj_noun_pairs.extract()
 ```
@@ -125,7 +133,8 @@
 python -m posextract.extract_triples --data_column sentence --id_column sentence_id input.csv output.csv
 ```
 
 ## For More Information...
 ... see our Wiki: 
 - [About Our Evaluation Data](https://github.com/stephbuon/posextract/wiki/Evaluation-Data-Sets)
 - [About the Syntactic Dependency Parser](https://github.com/stephbuon/posextract/wiki/Our-Application-of-spaCy-NLP)
+- [How to Use posextract on Databricks](https://github.com/stephbuon/posextract/wiki/Using-posextract-on-Databricks)
```

### Comparing `posextract-1.2.2/README.md` & `posextract-1.2.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -36,14 +36,22 @@
 
 for triple in triples:
     print(triple)
 
 # Output: Landlords exercise oppression, soldiers were ill
 ```
 
+Extract grammatical triples using different options from default: 
+
+```
+from posextract.util import TripleExtractorOptions
+
+triples = grammatical_triples.extract(sent, TripleExtractorOptions(prep_phrase = True))
+```
+
 Or extract adjectives and the nouns they modify. 
 
 ```
 from posextract import adj_noun_pairs
 
 adj_noun = adj_noun_pairs.extract()
 ```
@@ -86,7 +94,8 @@
 python -m posextract.extract_triples --data_column sentence --id_column sentence_id input.csv output.csv
 ```
 
 ## For More Information...
 ... see our Wiki: 
 - [About Our Evaluation Data](https://github.com/stephbuon/posextract/wiki/Evaluation-Data-Sets)
 - [About the Syntactic Dependency Parser](https://github.com/stephbuon/posextract/wiki/Our-Application-of-spaCy-NLP)
+- [How to Use posextract on Databricks](https://github.com/stephbuon/posextract/wiki/Using-posextract-on-Databricks)
```

### Comparing `posextract-1.2.2/posextract.egg-info/PKG-INFO` & `posextract-1.2.3/posextract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: posextract
-Version: 1.2.2
+Version: 1.2.3
 Summary: Grammatical information extraction methods designed for the analysis of historical and contemporary textual corpora.
 Author-email: Steph Buongiorno <steph.buon@gmail.com>, Alexander Cerpa <acerpa@smu.edu>
 License: MIT License
         
         Copyright (c) 2021 Steph Buongiorno and Alexander Cerpa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -75,14 +75,22 @@
 
 for triple in triples:
     print(triple)
 
 # Output: Landlords exercise oppression, soldiers were ill
 ```
 
+Extract grammatical triples using different options from default: 
+
+```
+from posextract.util import TripleExtractorOptions
+
+triples = grammatical_triples.extract(sent, TripleExtractorOptions(prep_phrase = True))
+```
+
 Or extract adjectives and the nouns they modify. 
 
 ```
 from posextract import adj_noun_pairs
 
 adj_noun = adj_noun_pairs.extract()
 ```
@@ -125,7 +133,8 @@
 python -m posextract.extract_triples --data_column sentence --id_column sentence_id input.csv output.csv
 ```
 
 ## For More Information...
 ... see our Wiki: 
 - [About Our Evaluation Data](https://github.com/stephbuon/posextract/wiki/Evaluation-Data-Sets)
 - [About the Syntactic Dependency Parser](https://github.com/stephbuon/posextract/wiki/Our-Application-of-spaCy-NLP)
+- [How to Use posextract on Databricks](https://github.com/stephbuon/posextract/wiki/Using-posextract-on-Databricks)
```

### Comparing `posextract-1.2.2/posextract.egg-info/SOURCES.txt` & `posextract-1.2.3/posextract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/pyproject.toml` & `posextract-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "posextract"
-version = "1.2.2"
+version = "1.2.3"
 description = "Grammatical information extraction methods designed for the analysis of historical and contemporary textual corpora."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     {name="Steph Buongiorno", email="steph.buon@gmail.com" },
     {name="Alexander Cerpa", email="acerpa@smu.edu"},
 ]
```

### Comparing `posextract-1.2.2/src/posextract/adj_noun_pairs.py` & `posextract-1.2.3/src/posextract/adj_noun_pairs.py`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/src/posextract/grammatical_triples.py` & `posextract-1.2.3/src/posextract/grammatical_triples.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import collections
 import copy
-from typing import List, Union, Iterable
+from typing import List, Union, Iterable, Optional
 
 import pandas
 
 import argparse
 import os
 
+from posextract.posrule.parser import parse_posrule
 from posextract.traversal import graph_tokens
 from posextract.triple_extraction import TripleExtraction, TripleExtractionFlattened
 from posextract.util import *
 import pandas as pd
 
+
+try:
+    collectionsAbc = collections.abc
+except AttributeError:
+    collectionsAbc = collections
+
+
 nlp = get_nlp()
 
 
 def post_process_combine_adj(extractions: List[TripleExtraction]):
     possible_dupes = {}
 
     for extraction in extractions:
@@ -68,27 +76,28 @@
             if len(nouns) != 1:
                 continue
 
             extraction.object_prep = child
             extraction.object_prep_noun = nouns[0]
 
             return extraction
-
-    # for child in extraction.verb.children:
-    #     if child == extraction.poa:
-    #         continue
-    #     if child.text == 'with':
-    #         pobjs = [childchild for childchild in child.children if childchild.dep == pobj]
-    #
-    #         if len(pobjs) != 1:
-    #             continue
-    #
-    #         extraction.object_prep = child
-    #         extraction.object_prep_noun = pobjs[0]
-    #         return extraction
+        
+    # Experimenting with adding this back (may result in double counted "with" statements
+     for child in extraction.verb.children:
+         if child == extraction.poa:
+             continue
+         if child.text == 'with':
+             pobjs = [childchild for childchild in child.children if childchild.dep == pobj]
+    
+             if len(pobjs) != 1:
+                 continue
+    
+             extraction.object_prep = child
+             extraction.object_prep_noun = pobjs[0]
+             return extraction
 
     return extraction
 
 
 def post_process_conj_triples(triple: TripleExtraction):
     new_extractions = []
 
@@ -180,15 +189,16 @@
         h = triple.get_triple_hash()
         if h not in hashes:
             yield triple
             hashes.add(h)
 
 
 def extract_one(doc: Doc, extractor_options: TripleExtractorOptions = None,
-                verbose: bool = False, flatten: bool = False):
+                verbose: bool = False, flatten: bool = False,
+                filters: Optional[List] = None):
     if extractor_options is None:
         extractor_options = TripleExtractorOptions()
 
     extractions = graph_tokens(doc, verbose=verbose)
     extractions = list(yield_non_duplicate_triples(extractions))
 
     for triple in extractions:
@@ -205,116 +215,157 @@
 
         if extractor_options.add_auxiliary:
             add_auxiliary_verb(triple)
 
         if extractor_options.prep_phrase:
             post_process_prep_phrase(triple)
 
+    def filter_func(ext):
+        for ext_filter in filters:
+            if ext_filter.eval(ext):
+                return True
+        return False
+
+    if filters:
+        extractions = list(filter(filter_func, extractions))
+
     if flatten:
         extractions = [
             triple.flatten(lemmatize=extractor_options.lemmatize,
                            compound_subject=extractor_options.compound_subject,
                            compound_object=extractor_options.compound_object)
             for triple in extractions]
 
     return extractions
 
 
 def extract(input_object: Union[str, Iterable[str]], extractor_options: TripleExtractorOptions = None,
             verbose: bool = False,
-            want_dataframe: bool = False) -> Union[List[TripleExtractionFlattened], pandas.DataFrame]:
+            want_dataframe: bool = False,
+            filters: Optional[List] = None) -> Union[List[TripleExtractionFlattened], pandas.DataFrame]:
     if extractor_options is None:
         extractor_options = TripleExtractorOptions()
 
+    if extractor_options.use_noun_chunks:
+        get_nlp().add_pipe('merge_noun_chunks')
+
     output_extractions = []
 
     if type(input_object) == str:
         input_object = [input_object, ]
-    elif not isinstance(input_object, collections.Iterable):
+    elif not isinstance(input_object, collectionsAbc.Iterable):
         raise ValueError('extract_triples: input should be a string or a collection of strings')
 
     for i, doc in enumerate(input_object):
         for sent in split_quotes(doc):
             sent = nlp(sent)
             output_extractions.extend(
-                extract_one(sent,extractor_options, flatten=True, verbose=verbose))
+                extract_one(sent,extractor_options, flatten=True, verbose=verbose,
+                            filters=filters))
 
     if want_dataframe:
         extractions_df = pd.DataFrame([t.__dict__ for t in output_extractions])
         return extractions_df
 
+    if extractor_options.use_noun_chunks:
+        get_nlp().remove_pipe('merge_noun_chunks')
+
     return output_extractions
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='posextractor')
-    parser.add_argument('input', metavar='input', type=str,
-                        help='a filepath to a csv file or an input string')
-    parser.add_argument('output', metavar='output', type=str,
-                        help='an output path')
+    parser.add_argument('--input',  type=str,
+                        help='an input string')
+    parser.add_argument('--input-file', type=str,
+                        help='The filepath of a input csv file')
+    parser.add_argument('--input-filters', type=str,
+                        help='An input file or directory containing posextract filter rules.')
+    parser.add_argument('--output', metavar='output', type=str,
+                        help='an output path', required=True)
     parser.add_argument('--data-column', type=str, default=None, metavar='data_col',
                         help='what column to use if a csv is given', dest='data_column')
     parser.add_argument('--id-column', type=str, default=None, metavar='id_col',
                         help='what column to use if a csv is given', dest='id_column')
     parser.add_argument('--file-delimiter', default='comma', const='comma', nargs='?',
                         choices=['comma', 'pipe', 'tab'],
                         help='delimiter character for data file (default: %(default)s)')
     parser.add_argument('--post-combine-adj', action='store_true')
     parser.add_argument('--lemma', action='store_true')
     parser.add_argument('--add-auxiliary', action='store_true')
     parser.add_argument('--verbose', action='store_true')
     parser.add_argument('--prep-phrase', action='store_true')
     parser.add_argument('--no-compound-subject', action='store_true')
     parser.add_argument('--no-compound-object', action='store_true')
+    parser.add_argument('--use-noun-chunks', action='store_true')
 
     args = parser.parse_args()
-    is_file = os.path.isfile(args.input)
+    is_file = args.input_file is not None
 
     extractor_options = TripleExtractorOptions(
         compound_subject=not args.no_compound_subject,
         compound_object=not args.no_compound_object,
         combine_adj=args.post_combine_adj,
         add_auxiliary=args.add_auxiliary,
         prep_phrase=args.prep_phrase,
-        lemmatize=args.lemma
+        lemmatize=args.lemma,
+        use_noun_chunks=args.use_noun_chunks,
     )
 
     inputs = []
     outputs = []
+    filters = []
 
     delimiter = {'comma': ',', 'pipe': '|', 'tab': '\t'}[args.file_delimiter]
 
     input_values = None
     df = None
 
+    if not args.input and not args.input_file:
+        exit('Please provide either an input string or an input file')
+
     if is_file:
         if args.verbose:
-            print('Loading input (%s) as a CSV file...' % args.input)
+            print('Loading input (%s) as a CSV file...' % args.input_file)
             print('delimiter:', args.file_delimiter)
         if args.data_column is None:
             exit('Invalid arguments: Must specify column name for data using --data-column')
 
         usecols = [args.data_column, ]
 
         if args.id_column is not None:
             usecols.append(args.id_column)
 
-        df = pd.read_csv(args.input, index_col=args.id_column, usecols=usecols, delimiter=delimiter)
+        df = pd.read_csv(args.input_file, index_col=args.id_column, usecols=usecols, delimiter=delimiter)
         input_values = df[args.data_column]
     else:
         input_values = [args.input, ]
 
+    if args.input_filters:
+        input_filters = args.input_filters
+        if os.path.isfile(input_filters):
+            filters.append(parse_posrule(input_filters))
+        elif os.path.isdir(input_filters):
+            for dirpath, dirnames, filenames in os.walk(input_filters):
+                filenames = [fn for fn in filenames if fn.endswith('.posrule')]
+                for fn in filenames:
+                    fn = f'{dirpath}{"/" if not fn.startswith("/") else ""}{fn}'
+                    filters.append(parse_posrule(fn))
+        else:
+            raise FileNotFoundError(args.input_filters)
+
     with open(args.output, 'w+') as f:
         pass
 
     extraction_count = 0
     header = True
 
     for i, data_str in enumerate(input_values):
-        triples_df = extract(data_str, extractor_options=extractor_options, verbose=args.verbose, want_dataframe=True)
+        triples_df = extract(data_str, extractor_options=extractor_options, verbose=args.verbose, want_dataframe=True,
+                             filters=filters)
         extraction_count += len(triples_df)
         if df is not None:
             triples_df['sentence_id'] = df.index[i]
         triples_df.to_csv(args.output, mode='a', sep=delimiter, header=header, index=False)
 
         if header:
             header = False
```

### Comparing `posextract-1.2.2/src/posextract/rules.py` & `posextract-1.2.3/src/posextract/rules.py`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/src/posextract/subj_verb_pairs.py` & `posextract-1.2.3/src/posextract/subj_verb_pairs.py`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/src/posextract/traversal.py` & `posextract-1.2.3/src/posextract/traversal.py`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/src/posextract/triple_extraction.py` & `posextract-1.2.3/src/posextract/triple_extraction.py`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/src/posextract/util.py` & `posextract-1.2.3/src/posextract/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 def get_nlp():
     global __NLP
     if __NLP is None:
         __NLP = spacy.load("en_core_web_sm")
     return __NLP
 
 
+def enable_pipe(pipe_name):
+    get_nlp().add_pipe(pipe_name)
+
+
+def disable_pipe(pipe_name):
+    get_nlp().remove_pipe(pipe_name)
+
+
 def get_dep_matcher(nlp):
     global __DEP_MATCHER
 
     if __DEP_MATCHER is None:
         matcher = DependencyMatcher(get_nlp().vocab)
         add_verb_phrase_patterns(matcher)
         __DEP_MATCHER = matcher
@@ -47,14 +55,15 @@
 class TripleExtractorOptions(NamedTuple):
     compound_subject: bool = True
     compound_object: bool = True
     combine_adj: bool = False
     add_auxiliary: bool = False
     prep_phrase: bool = False
     lemmatize: bool = False
+    use_noun_chunks: bool = False
 
 
 VERB_DEP_TAGS = {ccomp, relcl, xcomp, acl, advcl, pcomp, csubj, csubjpass, conj}
 OBJ_DEP_TAGS = {dobj, pobj, acomp}  # dative?
 
 
 def is_root(token: Token):
```

### Comparing `posextract-1.2.2/src/posextract/verb_phrase.py` & `posextract-1.2.3/src/posextract/verb_phrase.py`

 * *Files identical despite different names*

### Comparing `posextract-1.2.2/tests/test.py` & `posextract-1.2.3/tests/test.py`

 * *Files identical despite different names*

