# Comparing `tmp/pyvariant-2.0.0.tar.gz` & `tmp/pyvariant-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvariant-2.0.0.tar", last modified: Mon May 15 23:44:36 2023, max compression
+gzip compressed data, was "pyvariant-2.1.0.tar", last modified: Fri May 26 20:34:34 2023, max compression
```

## Comparing `pyvariant-2.0.0.tar` & `pyvariant-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-15 23:44:36.520002 pyvariant-2.0.0/
--rw-r--r--   0 mdouglas  (2185) users      (100)     1072 2023-01-16 21:09:00.000000 pyvariant-2.0.0/LICENSE
--rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-05-15 23:44:36.522394 pyvariant-2.0.0/PKG-INFO
--rw-r--r--   0 mdouglas  (2185) users      (100)     6903 2023-05-15 18:16:29.000000 pyvariant-2.0.0/README.md
--rw-r--r--   0 mdouglas  (2185) users      (100)      342 2023-05-15 18:16:29.000000 pyvariant-2.0.0/pyproject.toml
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-15 23:44:36.306341 pyvariant-2.0.0/pyvariant/
--rw-r--r--   0 mdouglas  (2185) users      (100)      197 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/__init__.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1995 2023-05-15 22:01:05.000000 pyvariant-2.0.0/pyvariant/cli.py
--rw-r--r--   0 mdouglas  (2185) users      (100)      958 2023-05-15 18:16:29.000000 pyvariant-2.0.0/pyvariant/constants.py
--rw-r--r--   0 mdouglas  (2185) users      (100)   139747 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/core.py
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-15 23:44:36.387863 pyvariant-2.0.0/pyvariant/data/
--rw-r--r--   0 mdouglas  (2185) users      (100)        4 2023-01-16 21:09:00.000000 pyvariant-2.0.0/pyvariant/data/empty.fa
--rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-01-16 21:09:00.000000 pyvariant-2.0.0/pyvariant/data/empty.fa.fai
--rw-r--r--   0 mdouglas  (2185) users      (100)    26111 2023-05-15 22:12:41.000000 pyvariant-2.0.0/pyvariant/ensembl_cache.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     7387 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/ensembl_release.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     4877 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/files.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     4051 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/parser.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    29669 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/positions.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    13398 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/regex.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     8451 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/sequence.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1623 2023-05-15 16:19:41.000000 pyvariant-2.0.0/pyvariant/tables.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    14143 2023-05-15 18:16:29.000000 pyvariant-2.0.0/pyvariant/utils.py
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-15 23:44:36.366416 pyvariant-2.0.0/pyvariant.egg-info/
--rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-05-15 23:44:36.000000 pyvariant-2.0.0/pyvariant.egg-info/PKG-INFO
--rw-r--r--   0 mdouglas  (2185) users      (100)      780 2023-05-15 23:44:36.000000 pyvariant-2.0.0/pyvariant.egg-info/SOURCES.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-05-15 23:44:36.000000 pyvariant-2.0.0/pyvariant.egg-info/dependency_links.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)       49 2023-05-15 23:44:36.000000 pyvariant-2.0.0/pyvariant.egg-info/entry_points.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)      166 2023-05-15 23:44:36.000000 pyvariant-2.0.0/pyvariant.egg-info/requires.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-15 23:44:36.000000 pyvariant-2.0.0/pyvariant.egg-info/top_level.txt
--rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-05-15 23:44:35.000000 pyvariant-2.0.0/pyvariant.egg-info/zip-safe
--rw-r--r--   0 mdouglas  (2185) users      (100)     1624 2023-05-15 23:44:36.528836 pyvariant-2.0.0/setup.cfg
-drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-15 23:44:36.511672 pyvariant-2.0.0/tests/
--rw-r--r--   0 mdouglas  (2185) users      (100)    67453 2023-05-15 18:26:02.000000 pyvariant-2.0.0/tests/test_core.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1376 2023-05-15 18:16:29.000000 pyvariant-2.0.0/tests/test_ensembl_cache.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1343 2023-05-15 18:16:29.000000 pyvariant-2.0.0/tests/test_ensembl_release.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     1920 2023-05-15 18:16:29.000000 pyvariant-2.0.0/tests/test_files.py
--rw-r--r--   0 mdouglas  (2185) users      (100)       88 2023-05-15 18:16:29.000000 pyvariant-2.0.0/tests/test_init.py
--rw-r--r--   0 mdouglas  (2185) users      (100)    37583 2023-05-15 18:16:29.000000 pyvariant-2.0.0/tests/test_parser.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     3400 2023-05-15 18:16:29.000000 pyvariant-2.0.0/tests/test_sequence.py
--rw-r--r--   0 mdouglas  (2185) users      (100)     7262 2023-05-15 18:16:29.000000 pyvariant-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.200603 pyvariant-2.1.0/
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1072 2023-05-16 21:59:33.000000 pyvariant-2.1.0/LICENSE
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-05-26 20:34:34.203496 pyvariant-2.1.0/PKG-INFO
+-rw-r--r--   0 mdouglas  (2185) users      (100)     6903 2023-05-16 21:59:33.000000 pyvariant-2.1.0/README.md
+-rw-r--r--   0 mdouglas  (2185) users      (100)      342 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyproject.toml
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:33.931073 pyvariant-2.1.0/pyvariant/
+-rw-r--r--   0 mdouglas  (2185) users      (100)      197 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/__init__.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1995 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/cli.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)      956 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/constants.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)   141512 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/core.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.102744 pyvariant-2.1.0/pyvariant/data/
+-rw-r--r--   0 mdouglas  (2185) users      (100)        4 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/data/empty.fa
+-rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/data/empty.fa.fai
+-rw-r--r--   0 mdouglas  (2185) users      (100)    25066 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/ensembl_cache.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     7150 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/ensembl_release.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     4877 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/files.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     4051 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/parser.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    32268 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/positions.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    13398 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/regex.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8450 2023-05-26 20:27:04.000000 pyvariant-2.1.0/pyvariant/sequence.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1623 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/tables.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    14143 2023-05-16 21:59:33.000000 pyvariant-2.1.0/pyvariant/utils.py
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.083579 pyvariant-2.1.0/pyvariant.egg-info/
+-rw-r--r--   0 mdouglas  (2185) users      (100)     8087 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/PKG-INFO
+-rw-r--r--   0 mdouglas  (2185) users      (100)      803 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/SOURCES.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/dependency_links.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)       49 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/entry_points.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)      166 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/requires.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)       10 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/top_level.txt
+-rw-r--r--   0 mdouglas  (2185) users      (100)        1 2023-05-26 20:34:33.000000 pyvariant-2.1.0/pyvariant.egg-info/zip-safe
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1624 2023-05-26 20:34:34.210161 pyvariant-2.1.0/setup.cfg
+drwxr-xr-x   0 mdouglas  (2185) users      (100)        0 2023-05-26 20:34:34.191862 pyvariant-2.1.0/tests/
+-rw-r--r--   0 mdouglas  (2185) users      (100)    70716 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_core.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     9802 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_core_map.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     6158 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_ensembl_cache.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     1487 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_ensembl_release.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     2025 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_files.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)       88 2023-05-16 21:59:34.000000 pyvariant-2.1.0/tests/test_init.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)    37583 2023-05-16 21:59:34.000000 pyvariant-2.1.0/tests/test_parser.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     3400 2023-05-26 20:27:05.000000 pyvariant-2.1.0/tests/test_sequence.py
+-rw-r--r--   0 mdouglas  (2185) users      (100)     7262 2023-05-16 21:59:34.000000 pyvariant-2.1.0/tests/test_utils.py
```

### Comparing `pyvariant-2.0.0/LICENSE` & `pyvariant-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/PKG-INFO` & `pyvariant-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvariant
-Version: 2.0.0
+Version: 2.1.0
 Summary: Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 Home-page: https://github.com/mattdoug604/pyvariant.git
 Author: Matthew Douglas
 Author-email: mattdoug604@gmail.com
 Maintainer: Matthew Douglas
 Maintainer-email: mattdoug604@gmail.com
 License: MIT
```

### Comparing `pyvariant-2.0.0/README.md` & `pyvariant-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/pyvariant/cli.py` & `pyvariant-2.1.0/pyvariant/cli.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/pyvariant/constants.py` & `pyvariant-2.1.0/pyvariant/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os.path
 
 # Default Ensembl species and release
 DEFAULT_SPECIES = "homo_sapiens"
 DEFAULT_ENSEMBL_RELEASE = 100
 
 # Environmental variable used to set the cache directory
-CACHE_DIR_ENV = "VARIANT_MAP_CACHE"
+CACHE_DIR_ENV = "PYVARIANT_CACHE"
 CACHE_DIR_NAME = "pyvariant"
 
 # Attribute name literals
 CONTIG_ID = "contig_id"
 EXON_ID = "exon_id"
 GENE_ID = "gene_id"
 GENE_NAME = "gene_name"
```

### Comparing `pyvariant-2.0.0/pyvariant/core.py` & `pyvariant-2.1.0/pyvariant/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,20 +100,20 @@
     def __init__(
         self,
         gtf: str,
         cds: List[str],
         dna: List[str],
         peptide: List[str],
         rna: List[str],
-        canonical_transcript: Union[List[str], str] = [],
-        contig_alias: Union[str, Dict] = {},
-        exon_alias: Union[str, Dict] = {},
-        gene_alias: Union[str, Dict] = {},
-        protein_alias: Union[str, Dict] = {},
-        transcript_alias: Union[str, Dict] = {},
+        canonical_transcript: Union[Callable, List[str], str] = [],
+        contig_alias: Union[Callable, Dict, str] = {},
+        exon_alias: Union[Callable, Dict, str] = {},
+        gene_alias: Union[Callable, Dict, str] = {},
+        protein_alias: Union[Callable, Dict, str] = {},
+        transcript_alias: Union[Callable, Dict, str] = {},
     ):
         """_summary_
 
         Args:
             gtf (str): Path to a GTF files with feature annotations
             cds (List[str]): List of paths to a FASTA files of CDS sequences
             dna (List[str]): List of paths to a FASTA files of DNA sequences
@@ -133,39 +133,45 @@
         self.protein_fasta: List[PyfaidxFasta] = []
         self.rna_fasta: List[PyfaidxFasta] = []
         self.cds_fasta = [PyfaidxFasta.load(i) for i in cds]
         self.dna_fasta = [PyfaidxFasta.load(i) for i in dna]
         self.protein_fasta = [PyfaidxFasta.load(i) for i in peptide]
         self.rna_fasta = [PyfaidxFasta.load(i) for i in rna]
 
+        self._canonical_transcript: Union[Callable, List[str]]
         if isinstance(canonical_transcript, str):
             self._canonical_transcript = txt_to_list(canonical_transcript)
         else:
             self._canonical_transcript = canonical_transcript
 
+        self._contig_alias: Union[Callable, Dict]
         if isinstance(contig_alias, str):
             self._contig_alias = tsv_to_dict(contig_alias)
         else:
             self._contig_alias = contig_alias
 
+        self._exon_alias: Union[Callable, Dict]
         if isinstance(exon_alias, str):
             self._exon_alias = tsv_to_dict(exon_alias)
         else:
             self._exon_alias = exon_alias
 
+        self._gene_alias: Union[Callable, Dict]
         if isinstance(gene_alias, str):
             self._gene_alias = tsv_to_dict(gene_alias)
         else:
             self._gene_alias = gene_alias
 
+        self._protein_alias: Union[Callable, Dict]
         if isinstance(protein_alias, str):
             self._protein_alias = tsv_to_dict(protein_alias)
         else:
             self._protein_alias = protein_alias
 
+        self._transcript_alias: Union[Callable, Dict]
         if isinstance(transcript_alias, str):
             self._transcript_alias = tsv_to_dict(transcript_alias)
         else:
             self._transcript_alias = transcript_alias
 
     # ---------------------------------------------------------------------------------------------
     # Functions for loading variants
@@ -375,15 +381,15 @@
                     end=end2,
                     end_offset=end_offset2,
                     strand=strand2,
                     refseq=refseq2,
                     altseq=altseq2,
                 )
 
-                return list(fusion(b1, b2) for b1, b2 in product(breakpoint1, breakpoint2))
+                return list(fusion(self, b1, b2) for b1, b2 in product(breakpoint1, breakpoint2))
 
         # Respect the given strand, otherwise check both strands
         if strand:
             strand_ = [strand]
         else:
             strand_ = [""]
 
@@ -1095,15 +1101,15 @@
         rnaf: Callable,
         canonical: bool,
     ) -> List:
         if position.is_fusion:
             fusion = cast(_Fusion, position)
             breakpoint1 = fusionf(fusion.breakpoint1, canonical)
             breakpoint2 = fusionf(fusion.breakpoint2, canonical)
-            return [fusiont(b1, b2) for b1, b2 in product(breakpoint1, breakpoint2)]
+            return [fusiont(self, b1, b2) for b1, b2 in product(breakpoint1, breakpoint2)]
         elif position.is_small_variant:
             if position.is_cdna:
                 position = cast(_CdnaSmallVariant, position)
                 return cdnavf(
                     [position.transcript_id],
                     position.start,
                     position.start_offset,
@@ -1245,14 +1251,15 @@
                 n_ = n + offset
                 if cds.cdna_start <= n_ <= cds.cdna_end:
                     n = n_
                     offset = 0
 
                 result.append(
                     CdnaPosition(
+                        _core=self,
                         contig_id=cds.contig_id,
                         start=n,
                         start_offset=offset,
                         end=n,
                         end_offset=offset,
                         strand=cds.strand,
                         gene_id=cds.gene_id,
@@ -1335,14 +1342,15 @@
                     new_start = new_end = cds.start + (n - cds.cdna_start) + offset
 
                 offset = 0
 
                 # TODO: Check that new new_start is actually on the contig
                 result.append(
                     DnaPosition(
+                        _core=self,
                         contig_id=cds.contig_id,
                         start=new_start,
                         start_offset=offset,
                         end=new_end,
                         end_offset=offset,
                         strand=cds.strand,
                     )
@@ -1427,14 +1435,15 @@
                     (self.df[TRANSCRIPT_ID].isin(transcript_id))
                     & (self.df["exon_number"] == cds.exon_number)
                     & (self.df["feature"] == EXON)
                 )
                 for _, exon in self.df[mask_exon].iterrows():
                     result.append(
                         ExonPosition(
+                            _core=self,
                             contig_id=exon.contig_id,
                             start=int(exon.exon_number),
                             start_offset=offset,
                             end=int(exon.exon_number),
                             end_offset=offset,
                             strand=exon.strand,
                             gene_id=exon.gene_id,
@@ -1615,14 +1624,15 @@
                 if cds.cdna_start <= n_ <= cds.cdna_end:
                     n = n_
                     offset = 0
 
                 new_start = new_end = cds.transcript_start + (n - cds.cdna_start)
                 result.append(
                     RnaPosition(
+                        _core=self,
                         contig_id=cds.contig_id,
                         start=new_start,
                         start_offset=offset,
                         end=new_end,
                         end_offset=offset,
                         strand=cds.strand,
                         gene_id=cds.gene_id,
@@ -1706,14 +1716,15 @@
                         new_start = new_end = n_ - cds.start + cds.cdna_start
 
                     if canonical and not self.is_canonical_transcript(cds.transcript_id):
                         continue
 
                     result.append(
                         CdnaPosition(
+                            _core=self,
                             contig_id=cds.contig_id,
                             start=new_start,
                             start_offset=offset,
                             end=new_end,
                             end_offset=offset,
                             strand=cds.strand,
                             gene_id=cds.gene_id,
@@ -1787,14 +1798,15 @@
             end_offset = 0
 
             # Sort the start and end positions after adjusting by offsets
             new_start, new_end = sorted([new_start, new_end])
 
             result.append(
                 DnaPosition(
+                    _core=self,
                     contig_id=contig_id_,
                     start=new_start,
                     start_offset=start_offset,
                     end=new_end,
                     end_offset=end_offset,
                     strand=strand_,
                 )
@@ -1851,14 +1863,15 @@
 
                 for _, exon in self.df[mask].iterrows():
                     if canonical and not self.is_canonical_transcript(exon.transcript_id):
                         continue
 
                     result.append(
                         ExonPosition(
+                            _core=self,
                             contig_id=exon.contig_id,
                             start=int(exon.exon_number),
                             start_offset=offset,
                             end=int(exon.exon_number),
                             end_offset=offset,
                             strand=exon.strand,
                             gene_id=exon.gene_id,
@@ -1986,14 +1999,15 @@
                         new_start = new_end = n_ - exon.start + exon.transcript_start
 
                     if canonical and not self.is_canonical_transcript(exon.transcript_id):
                         continue
 
                     result.append(
                         RnaPosition(
+                            _core=self,
                             contig_id=exon.contig_id,
                             start=new_start,
                             start_offset=offset,
                             end=new_end,
                             end_offset=offset,
                             strand=exon.strand,
                             gene_id=exon.gene_id,
@@ -2061,14 +2075,15 @@
                 (self.df[TRANSCRIPT_ID].isin(transcript_id))
                 & (self.df["exon_number"] == float(n))
                 & (self.df["feature"].isin(feature))
             )
             for _, cds in self.df[mask].iterrows():
                 result.append(
                     CdnaPosition(
+                        _core=self,
                         contig_id=cds.contig_id,
                         start=cds.cdna_start,
                         start_offset=offset,
                         end=cds.cdna_end,
                         end_offset=offset,
                         strand=cds.strand,
                         gene_id=cds.gene_id,
@@ -2113,14 +2128,15 @@
                 (self.df[TRANSCRIPT_ID].isin(transcript_id))
                 & (self.df["exon_number"] == float(n))
                 & (self.df["feature"] == EXON)
             )
             for _, exon in self.df[mask].iterrows():
                 result.append(
                     DnaPosition(
+                        _core=self,
                         contig_id=exon.contig_id,
                         start=exon.start,
                         start_offset=offset,
                         end=exon.end,
                         end_offset=offset,
                         strand=exon.strand,
                     )
@@ -2160,14 +2176,15 @@
                 (self.df[TRANSCRIPT_ID].isin(transcript_id))
                 & (self.df["exon_number"] == float(n))
                 & (self.df["feature"] == EXON)
             )
             for _, exon in self.df[mask].iterrows():
                 result.append(
                     ExonPosition(
+                        _core=self,
                         contig_id=exon.contig_id,
                         start=int(exon.exon_number),
                         start_offset=offset,
                         end=int(exon.exon_number),
                         end_offset=offset,
                         strand=exon.strand,
                         gene_id=exon.gene_id,
@@ -2248,14 +2265,15 @@
                 (self.df[TRANSCRIPT_ID].isin(transcript_id))
                 & (self.df["exon_number"] == float(n))
                 & (self.df["feature"] == EXON)
             )
             for _, exon in self.df[mask].iterrows():
                 result.append(
                     RnaPosition(
+                        _core=self,
                         contig_id=exon.contig_id,
                         start=exon.transcript_start,
                         start_offset=offset,
                         end=exon.transcript_end,
                         end_offset=offset,
                         strand=exon.strand,
                         gene_id=exon.gene_id,
@@ -2646,14 +2664,15 @@
                 if cds.cdna_start <= n_ <= cds.cdna_end:
                     n = n_
                     offset = 0
 
                 new_start = new_end = cds.cdna_start + (n - cds.transcript_start)
                 result.append(
                     CdnaPosition(
+                        _core=self,
                         contig_id=cds.contig_id,
                         start=new_start,
                         start_offset=offset,
                         end=new_end,
                         end_offset=offset,
                         strand=cds.strand,
                         gene_id=cds.gene_id,
@@ -2734,14 +2753,15 @@
                     new_start = new_end = exon.start + (n - exon.transcript_start) + offset
 
                 offset = 0
 
                 # TODO: Check that new new_start is actually on the contig
                 result.append(
                     DnaPosition(
+                        _core=self,
                         contig_id=exon.contig_id,
                         start=new_start,
                         start_offset=offset,
                         end=new_end,
                         end_offset=offset,
                         strand=exon.strand,
                     )
@@ -2809,14 +2829,15 @@
                     n = n_
                     offset = 0
                 else:
                     continue
 
                 result.append(
                     ExonPosition(
+                        _core=self,
                         contig_id=exon.contig_id,
                         start=int(exon.exon_number),
                         start_offset=offset,
                         end=int(exon.exon_number),
                         end_offset=offset,
                         strand=exon.strand,
                         gene_id=exon.gene_id,
@@ -2965,14 +2986,15 @@
                 n_ = n + offset
                 if exon.transcript_start <= n_ <= exon.transcript_end:
                     n = n_
                     offset = 0
 
                 result.append(
                     RnaPosition(
+                        _core=self,
                         contig_id=exon.contig_id,
                         start=n,
                         start_offset=offset,
                         end=n,
                         end_offset=offset,
                         strand=exon.strand,
                         gene_id=exon.gene_id,
@@ -3609,33 +3631,45 @@
             transcript_id (str): transcript ID
 
         Returns:
             List[str]: All aliases of the given transcript ID
         """
         return self._alias(transcript_id, self._transcript_alias)
 
-    def _alias(self, feature: str, alias_dict: Dict[str, List[str]]) -> List[str]:
+    def _alias(self, feature: str, aliases: Union[Callable, Dict]) -> List[str]:
         feature = str(feature)
 
+        # Expect `aliases` to be a function that returns an alias, or dictionary, or an object
+        # has a dictionary-like `get` function.
+        if callable(aliases):
+            alias_func = aliases
+        elif hasattr(aliases, "get") and callable(aliases.get):
+            alias_func = aliases.get
+        else:
+            raise AssertionError(
+                f"Alias object must be a dictionary or callable, not {type(aliases)}"
+            )
+
         # Try different variations on the feature ID until one is found
         alias_list = [
             feature,
             strip_version(feature),
             feature.lower(),
             strip_version(feature).lower(),
             feature.upper(),
             strip_version(feature).upper(),
         ]
         for key in alias_list:
-            if alias := alias_dict.get(key, []):
-                # Coerce the alias to a list
-                if isinstance(alias, str):
-                    alias_list.append(alias)
-                else:
-                    alias_list.extend(alias)
+            if alias := alias_func(key):
+                if alias != key:
+                    # Coerce the alias to a list
+                    if isinstance(alias, str):
+                        alias_list.append(alias)
+                    else:
+                        alias_list.extend(alias)
 
         return sorted(set(alias_list))
 
     # ---------------------------------------------------------------------------------------------
     # Functions for normalizing feature ID/names
     # ---------------------------------------------------------------------------------------------
     def normalize_id(self, feature: str) -> List[Tuple[str, str]]:
@@ -3783,15 +3817,18 @@
 
         Args:
             transcript_id (str): transcript ID
 
         Returns:
             bool: True if the transcript is the canonical transcript else False
         """
-        return transcript_id in self._canonical_transcript
+        if callable(self._canonical_transcript):
+            return self._canonical_transcript(transcript_id)
+        else:
+            return transcript_id in self._canonical_transcript
 
     # ---------------------------------------------------------------------------------------------
     # <feature>
     # ---------------------------------------------------------------------------------------------
     def cdna(self, feature: str, canonical: bool = False) -> List[CdnaPosition]:
         """Return the cDNA position(s) matching the given feature ID or name.
 
@@ -3808,14 +3845,15 @@
         mask = (self.df[TRANSCRIPT_ID].isin(transcript_ids)) & (self.df["feature"] == CDNA)
         for _, cdna in self.df[mask].iterrows():
             if canonical and not self.is_canonical_transcript(cdna.transcript_id):
                 continue
 
             result.append(
                 CdnaPosition(
+                    _core=self,
                     contig_id=cdna.contig_id,
                     start=cdna.cdna_start,
                     start_offset=0,
                     end=cdna.cdna_end,
                     end_offset=0,
                     strand=cdna.strand,
                     gene_id=cdna.gene_id,
@@ -3855,14 +3893,15 @@
                 raise KeyError(f"Sequence '{contig_id}' not found")
 
             start = 1
             end = len(contig_seq)
             for strand in strand_list:
                 result.append(
                     DnaPosition(
+                        _core=self,
                         contig_id=contig_id,
                         start=start,
                         start_offset=0,
                         end=end,
                         end_offset=0,
                         strand=strand,
                     )
@@ -3886,14 +3925,15 @@
         mask = (self.df[EXON_ID].isin(exon_ids)) & (self.df["feature"] == EXON)
         for _, exon in self.df[mask].iterrows():
             if canonical and not self.is_canonical_transcript(exon.transcript_id):
                 continue
 
             result.append(
                 ExonPosition(
+                    _core=self,
                     contig_id=exon.contig_id,
                     start=int(exon.exon_number),
                     start_offset=0,
                     end=int(exon.exon_number),
                     end_offset=0,
                     strand=exon.strand,
                     gene_id=exon.gene_id,
@@ -3919,14 +3959,15 @@
         result = []
 
         gene_ids = self.gene_ids(feature)
         mask = (self.df[GENE_ID].isin(gene_ids)) & (self.df["feature"] == "gene")
         for _, gene in self.df[mask].iterrows():
             result.append(
                 DnaPosition(
+                    _core=self,
                     contig_id=gene.contig_id,
                     start=gene.start,
                     start_offset=0,
                     end=gene.end,
                     end_offset=0,
                     strand=gene.strand,
                 )
@@ -3973,14 +4014,15 @@
         mask = (self.df[TRANSCRIPT_ID].isin(transcript_ids)) & (self.df["feature"] == "transcript")
         for _, transcript in self.df[mask].iterrows():
             if canonical and not self.is_canonical_transcript(transcript.transcript_id):
                 continue
 
             result.append(
                 RnaPosition(
+                    _core=self,
                     contig_id=transcript.contig_id,
                     start=transcript.transcript_start,
                     start_offset=0,
                     end=transcript.transcript_end,
                     end_offset=0,
                     strand=transcript.strand,
                     gene_id=transcript.gene_id,
```

### Comparing `pyvariant-2.0.0/pyvariant/ensembl_cache.py` & `pyvariant-2.1.0/pyvariant/ensembl_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Definitions for the `EnsemblCache` class."""
 import os.path
 import sys
 from pathlib import Path
-from typing import List
 
 import numpy as np
 import pandas as pd
 from gtfparse import read_gtf
 from pyfaidx import Fasta
 
 from .constants import CONTIG_ID
@@ -38,30 +37,33 @@
 GTF_SUBDIR_TEMPLATE = "pub/release-{release}/gtf/{species}"
 
 # GTF annotation file example: Homo_sapiens.GRCh38.100.gtf.gz
 GTF_FILENAME_TEMPLATE = "{species}.{reference}.{release}.gtf.gz"
 
 # GTF column names and features
 GTF_COLUMN_RENAME = {"seqname": CONTIG_ID}
-GTF_KEEP_FEATURES = ["CDS", "exon", "gene", "stop_codon", "transcript"]
-GTF_KEEP_COLUMNS = [
-    "contig_id",
-    "feature",
-    "start",
-    "end",
-    "strand",
-    "gene_id",
-    "gene_name",
-    "transcript_id",
-    "transcript_name",
-    "exon_id",
-    "exon_number",
-    "protein_id",
-]
-GTF_ADD_COLUMNS = ["transcript_start", "transcript_end", "cdna_start", "cdna_end"]
+GTF_KEEP_FEATURES = ["cdna", "CDS", "exon", "gene", "stop_codon", "transcript"]
+DATAFRAME_COLUMNS = {
+    "contig_id": "category",
+    "feature": "category",
+    "start": "Int64",
+    "end": "Int64",
+    "strand": "category",
+    "gene_id": "category",
+    "gene_name": "category",
+    "transcript_id": "category",
+    "transcript_name": "category",
+    "exon_id": "category",
+    "exon_number": "Int16",
+    "protein_id": "category",
+    "transcript_start": "Int64",
+    "transcript_end": "Int64",
+    "cdna_start": "Int64",
+    "cdna_end": "Int64",
+}
 
 
 class EnsemblCache:
     """Class for managing Ensembl files."""
 
     def __init__(self, species: str, release: int, cache_dir: str = ""):
         self.species = normalize_species(species)
@@ -69,28 +71,21 @@
         self.reference = reference_by_release(self.release)
 
         if cache_dir:
             self.cache_dir = os.path.abspath(cache_dir)
         else:
             self.cache_dir = get_cache_dir()
 
-    def install(
-        self,
-        clean: bool = True,
-        recache: bool = False,
-        redownload: bool = False,
-        restrict_genes: List[str] = [],
-    ):
+    def install(self, clean: bool = True, recache: bool = False, redownload: bool = False):
         """Download missing data, process, and cache.
 
         Args:
             clean (bool, optional): Delete temporary files. Defaults to True.
             recache (bool, optional): Overwrite any existing cache. Defaults to False.
             redownload (bool, optional): Redownload files from Ensembl. Defaults to False.
-            restrict_genes (List[str], optional): Restrict cache to the specified genes. Defaults to [].
         """
         # Create the cache directory structure
         self.make_release_cache_dir()
 
         # Download each FASTA file
         for fasta, index, downloadf in [
             (
@@ -133,21 +128,15 @@
         if (gtf_missing and cache_missing) or (gtf_missing and recache) or redownload:
             self.download_gtf()
 
         # Process and cache the GTF file
         if cache_missing or recache:
             # TODO: switch to 'polars'?
             df = read_gtf(self.local_gtf_filepath, result_type="pandas")
-
-            restrict_genes = ["ARF5"]  # DEBUG
-
-            if restrict_genes:
-                df = df[df["gene_name"].isin(restrict_genes)]
-
-            df = normalize_df(df)
+            df = infer_missing_values(df)
             self.cache_df(df)
             if clean:
                 self.delete_gtf()
 
     # ---------------------------------------------------------------------------------------------
     # Release cache directory
     # ---------------------------------------------------------------------------------------------
@@ -398,46 +387,46 @@
         df.to_pickle(self.local_gtf_cache_filepath)
 
     def load_df(self) -> pd.DataFrame:
         """Return the cached Ensembl GTF data."""
         return pd.read_pickle(self.local_gtf_cache_filepath)
 
 
-def normalize_df(df: pd.DataFrame) -> pd.DataFrame:
-    """Normalize a pandas DataFrame and infer missing data."""
-    df = df.replace("", np.nan)
-    df = normlize_columns(df)
-    df = df.sort_values(["start", "end"])
+def infer_missing_values(df: pd.DataFrame) -> pd.DataFrame:
+    """Infer values missing from the DataFrame."""
+    df = normalize_df(df)
     df = infer_transcripts(df)
     df = infer_cdna(df)
-    df = infer_missing_genes(df)
+    df = infer_genes(df)
     df = exon_offset_transcript(df)
     df = cds_offset_transcript(df)
     df = cds_offset_cdna(df)
-    df = set_protein_id(df)
-    df = df.replace("", np.nan)
+    df = infer_protein_id(df)
 
     return df
 
 
-def normlize_columns(df: pd.DataFrame) -> pd.DataFrame:
-    """Rename columns, drop unused data, and set data types for each column."""
+def normalize_df(df: pd.DataFrame) -> pd.DataFrame:
+    """Read the GTF file into a normalized dataframe."""
     # Rename column(s)
     df = df.rename(columns=GTF_COLUMN_RENAME)
-    # Drop unused columns
-    df = df.drop(df.columns.difference(GTF_KEEP_COLUMNS), axis=1)
+    # Drop columns that aren't needed
+    df = df.drop(df.columns.difference(list(DATAFRAME_COLUMNS)), axis=1)
+    # Replace null values
+    df = df.replace("", np.nan)
+    # Add in any missing columns
+    for col in DATAFRAME_COLUMNS:
+        if col not in df:
+            df[col] = np.nan
+    # Coerce column values to the expected types
+    df = df.astype(DATAFRAME_COLUMNS)
     # Drop unused feature types
     df = df[df.feature.isin(GTF_KEEP_FEATURES)]
-    # Add additional columns
-    df = df.reindex(columns=GTF_KEEP_COLUMNS + GTF_ADD_COLUMNS)
-    # Assert that all the expected columns exist
-    missing = [i for i in GTF_KEEP_COLUMNS + GTF_ADD_COLUMNS if i not in df.columns]
-    assert not missing, f"Found columns {list(df.columns)}, missing {missing}"
-    # Coerce the non-null values in the 'exon_number' to float
-    df["exon_number"] = df["exon_number"].astype(float, errors="raise")
+    # Sort by genomic position
+    df = df.sort_values(["contig_id", "start", "end"])
 
     return df
 
 
 def infer_transcripts(df: pd.DataFrame) -> pd.DataFrame:
     """Infer transcripts position(s) from other features, if not already defined."""
     transcript_rows = []
@@ -457,29 +446,28 @@
                 "gene_name": first.gene_name,
                 "transcript_id": transcript_id,
                 "transcript_name": first.transcript_name,
             }
             transcript_rows.append(new_row)
             print(f"Inferred transcript {new_row}", file=sys.stderr)
 
-    new_transcript_df = pd.DataFrame(transcript_rows)
-    df = pd.concat([df, new_transcript_df], ignore_index=True)
-    df = df.sort_values(["start", "end"])
+    df = pd.concat([df, pd.DataFrame(transcript_rows)], ignore_index=True)
+    df = normalize_df(df)
 
     return df
 
 
 def infer_cdna(df: pd.DataFrame) -> pd.DataFrame:
     """Infer cDNA position(s) from other features, if not already defined."""
     cdna_rows = []
 
     print("Inferring cDNA...", file=sys.stderr)
     for transcript_id, group in df.groupby("transcript_id"):
         if group[group.feature == "cdna"].empty:
-            cds_df = group[group.feature == "cds"]
+            cds_df = group[group.feature == "CDS"]
             if not cds_df.empty:
                 first = cds_df.iloc[0]
                 last = cds_df.iloc[-1]
                 new_row = {
                     "contig_id": first.contig_id,
                     "feature": "cdna",
                     "start": first.start,
@@ -489,22 +477,21 @@
                     "gene_name": first.gene_name,
                     "transcript_id": transcript_id,
                     "transcript_name": first.transcript_name,
                 }
                 cdna_rows.append(new_row)
                 print(f"Inferred cDNA {new_row}", file=sys.stderr)
 
-    new_cdna_df = pd.DataFrame(cdna_rows)
-    df = pd.concat([df, new_cdna_df], ignore_index=True)
-    df = df.sort_values(["start", "end"])
+    df = pd.concat([df, pd.DataFrame(cdna_rows)], ignore_index=True)
+    df = normalize_df(df)
 
     return df
 
 
-def infer_missing_genes(df: pd.DataFrame) -> pd.DataFrame:
+def infer_genes(df: pd.DataFrame) -> pd.DataFrame:
     """Infer gene position(s) from other features, if not already defined."""
     gene_rows = []
 
     print("Inferring missing genes...", file=sys.stderr)
     for _, group in df.groupby("gene_id"):
         if group[group.feature == "gene"].empty:
             first = group.iloc[0]
@@ -517,17 +504,16 @@
                 "strand": first.strand,
                 "gene_id": first.gene_id,
                 "gene_name": first.gene_name,
             }
             gene_rows.append(new_row)
             print(f"Inferred gene {new_row}", file=sys.stderr)
 
-    new_gene_df = pd.DataFrame(gene_rows)
-    df = pd.concat([df, new_gene_df], ignore_index=True)
-    df = df.sort_values(["start", "end"])
+    df = pd.concat([df, pd.DataFrame(gene_rows)], ignore_index=True)
+    df = normalize_df(df)
 
     return df
 
 
 def exon_offset_transcript(df: pd.DataFrame) -> pd.DataFrame:
     """Calculate the position of each exon, relative to the start of the transcript."""
     print("Inferring exon offsets from transcripts...", file=sys.stderr)
@@ -561,26 +547,22 @@
             df.at[exon.Index, "transcript_start"] = transcript_start
             df.at[exon.Index, "transcript_end"] = transcript_end
 
         # add the new offsets to the transcript
         df.at[transcript_index, "transcript_start"] = 1
         df.at[transcript_index, "transcript_end"] = offset
 
-    # convert the offset values to integers
-    df["transcript_start"] = df["transcript_start"].astype("Int64")
-    df["transcript_end"] = df["transcript_end"].astype("Int64")
-
     return df
 
 
 def cds_offset_transcript(df: pd.DataFrame) -> pd.DataFrame:
     """Calculate the position of each CDS, relative to the start of the transcript."""
     print("Inferring CDS offsets from transcripts...", file=sys.stderr)
     for _, group in df.groupby("transcript_id"):
-        cds_df = group[group.feature.isin(["cds", "stop_codon"])]
+        cds_df = group[group.feature.isin(["CDS", "stop_codon"])]
         if cds_df.empty:
             continue
 
         ascending = cds_df.iloc[0].strand == "+"
         for cds in cds_df.sort_values(["start", "end"], ascending=ascending).itertuples():
             exon_mask = (
                 (group.start <= cds.start) & (group.end >= cds.end) & (group.feature == "exon")
@@ -601,18 +583,14 @@
             offset += length
 
             # add the new offsets and exon ID to the CDS
             df.at[cds.Index, "exon_id"] = exon.exon_id
             df.at[cds.Index, "transcript_start"] = transcript_start
             df.at[cds.Index, "transcript_end"] = transcript_end
 
-    # convert the offset values to integers
-    df["transcript_start"] = df["transcript_start"].astype("Int64")
-    df["transcript_end"] = df["transcript_end"].astype("Int64")
-
     return df
 
 
 def cds_offset_cdna(df: pd.DataFrame) -> pd.DataFrame:
     """Calculate the position of each CDS, relative to the start of the cDNA."""
     print("Inferring CDS offsets from cDNA...", file=sys.stderr)
     for _, group in df.groupby("transcript_id"):
@@ -620,15 +598,15 @@
         if cdna_df.empty:
             continue
 
         cdna_index = cdna_df.index[0]
         cdna = cdna_df.iloc[0]
         ascending = cdna.strand == "+"
 
-        cds_df = group[group.feature.isin(["cds", "stop_codon"])]
+        cds_df = group[group.feature.isin(["CDS", "stop_codon"])]
         if cds_df.empty:
             continue
 
         offset = 0
         cds_df = cds_df.sort_values(["start", "end"], ascending=ascending)
         for cds in cds_df.itertuples():
             # if this is the first exon/CDS/etc start the offset relative to the RNA
@@ -647,22 +625,18 @@
             df.at[cds.Index, "cdna_start"] = start_offset
             df.at[cds.Index, "cdna_end"] = end_offset
 
         # add the new offsets to the cDNA
         df.at[cdna_index, "cdna_start"] = 1
         df.at[cdna_index, "cdna_end"] = offset
 
-    # convert the offset values to integers
-    df["cdna_start"] = df["cdna_start"].astype("Int64")
-    df["cdna_end"] = df["cdna_end"].astype("Int64")
-
     return df
 
 
-def set_protein_id(df: pd.DataFrame) -> pd.DataFrame:
+def infer_protein_id(df: pd.DataFrame) -> pd.DataFrame:
     """Add the protein ID as info for each cDNA and stop codon, if not already defined."""
     print("Inferring protein IDs...", file=sys.stderr)
     for _, group in df.groupby("transcript_id"):
         # Get the first non-NA protein ID matching the transcript ID
         # A protein coding transcript should only have 1 matching protein ID
         if pidx := group["protein_id"].first_valid_index():
             protein_id = group["protein_id"].loc[pidx]
```

### Comparing `pyvariant-2.0.0/pyvariant/ensembl_release.py` & `pyvariant-2.1.0/pyvariant/ensembl_release.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,32 +87,23 @@
             self._transcript_alias = tsv_to_dict(transcript_alias)
         else:
             self._transcript_alias = transcript_alias
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(species={self.species}, release={self.release})"
 
-    def install(
-        self,
-        clean: bool = True,
-        recache: bool = False,
-        redownload: bool = False,
-        restrict_genes: List[str] = [],
-    ):
+    def install(self, clean: bool = True, recache: bool = False, redownload: bool = False):
         """Download missing data, process, and cache.
 
         Args:
             clean (bool, optional): Delete temporary files. Defaults to True.
             recache (bool, optional): Overwrite any existing cache. Defaults to False.
             redownload (bool, optional): Redownload files from Ensembl. Defaults to False.
-            restrict_genes (List[str], optional): Restrict cache to the specified genes. Defaults to [].
         """
-        self.ensembl_cache.install(
-            clean=clean, recache=recache, redownload=redownload, restrict_genes=restrict_genes
-        )
+        self.ensembl_cache.install(clean=clean, recache=recache, redownload=redownload)
 
     def _sequence(
         self,
         position,
         mutate: bool,
         strand: Optional[str],
         window: Optional[int],
```

### Comparing `pyvariant-2.0.0/pyvariant/files.py` & `pyvariant-2.1.0/pyvariant/files.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/pyvariant/parser.py` & `pyvariant-2.1.0/pyvariant/parser.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/pyvariant/positions.py` & `pyvariant-2.1.0/pyvariant/positions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Class definitions for position/variant objects."""
 from __future__ import annotations
 
 from dataclasses import dataclass, fields
-from typing import Any, Dict, Type
+from typing import TYPE_CHECKING, Any, Dict, List, Type
 
 from .constants import (
     CDNA,
     DELETION,
     DELINS,
     DNA,
     DUPLICATION,
@@ -16,19 +16,24 @@
     INSERTION,
     PROTEIN,
     RNA,
     SUBSTITUTION,
 )
 from .utils import format_hgvs_position
 
+if TYPE_CHECKING:
+    from .core import Core
+
 
 @dataclass(eq=True, frozen=True)
 class _Base:
     """Base class for all position and variant classes."""
 
+    _core: Core
+
     @classmethod
     def copy_from(cls, obj: _Base, **kwargs):
         """Initialize a new `_Base`-derived object by copying values from another `_Base`-derived object.
 
         Args:
             obj (_Base): Position object to copy attributes from
             **kwargs: Arguments with keys that match the attribute names of this `_Base`-derived class will override attributes from `obj`
@@ -48,14 +53,25 @@
 
     def __lt__(self, other: _Base) -> bool:
         return str(self) < str(other)
 
     def __str__(self) -> str:
         raise NotImplementedError()  # Defined by inheriting class
 
+    # The `__getstate__` and `__setstate__` methods control how class instances are pickled. Since
+    # `Core` and `Core`-derived instances can't be pickled, we need to remove them as values in
+    # order to be able to pickle `_Base`-dervied class instances. This does mean that any functions
+    # that rely on `Core` will break upon being un-pickled.
+    # TODO: Is there a way to preserve `Core` values when pickling?
+    def __getstate__(self):
+        state = self.__dict__.copy()
+        state["_core"] = None
+
+        return state
+
     @property
     def is_cdna(self) -> bool:
         """Check if this fusion is between cDNA.
 
         Returns:
             bool: True if the fusion is between cDNA else False
         """
@@ -218,14 +234,69 @@
         """Convert this position's attributes to a dictionary.
 
         Returns:
             Dict[str, Any]: Dictionary of attribute names and corresponding values
         """
         return {f.name: self[f.name] for f in fields(self)}
 
+    def to_cdna(self, canonical: bool = False) -> List:
+        """Map this position to zero or more cDNA positions.
+
+        Args:
+            canonical (bool, optional): Only consider the canonical transcript when mapping. Defaults to False.
+
+        Returns:
+            List[DnaPosition]: Equivalent cDNA positions.
+        """
+        return self._core.to_cdna(self, canonical=canonical)
+
+    def to_dna(self, canonical: bool = False) -> List:
+        """Map this position to zero or more DNA positions.
+
+        Args:
+            canonical (bool, optional): Only consider the canonical transcript when mapping. Defaults to False.
+
+        Returns:
+            List[DnaPosition]: Equivalent DNA positions.
+        """
+        return self._core.to_dna(self, canonical=canonical)
+
+    def to_exon(self, canonical: bool = False) -> List:
+        """Map this position to zero or more exon positions.
+
+        Args:
+            canonical (bool, optional): Only consider the canonical transcript when mapping. Defaults to False.
+
+        Returns:
+            List[DnaPosition]: Equivalent exon positions.
+        """
+        return self._core.to_exon(self, canonical=canonical)
+
+    def to_protein(self, canonical: bool = False) -> List:
+        """Map this position to zero or more protein positions.
+
+        Args:
+            canonical (bool, optional): Only consider the canonical transcript when mapping. Defaults to False.
+
+        Returns:
+            List[DnaPosition]: Equivalent protein positions.
+        """
+        return self._core.to_protein(self, canonical=canonical)
+
+    def to_rna(self, canonical: bool = False) -> List:
+        """Map this position to zero or more RNA positions.
+
+        Args:
+            canonical (bool, optional): Only consider the canonical transcript when mapping. Defaults to False.
+
+        Returns:
+            List[DnaPosition]: Equivalent RNA positions.
+        """
+        return self._core.to_rna(self, canonical=canonical)
+
 
 @dataclass(eq=True, frozen=True)
 class _Position(_Base):
     """Base class for positions."""
 
     contig_id: str
     start: int
```

### Comparing `pyvariant-2.0.0/pyvariant/regex.py` & `pyvariant-2.1.0/pyvariant/regex.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/pyvariant/sequence.py` & `pyvariant-2.1.0/pyvariant/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             path = EMPTY_FASTA
 
         fasta = Fasta(
             path,
             key_function=strip_version,
             as_raw=True,
             sequence_always_upper=True,
-            build_index=False,
+            build_index=True,
             rebuild=False,
             read_ahead=cls.read_ahead,
         )
 
         return cls(fasta)
 
     def __init__(self, fasta: Fasta):
```

### Comparing `pyvariant-2.0.0/pyvariant/tables.py` & `pyvariant-2.1.0/pyvariant/tables.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/pyvariant/utils.py` & `pyvariant-2.1.0/pyvariant/utils.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/pyvariant.egg-info/PKG-INFO` & `pyvariant-2.1.0/pyvariant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvariant
-Version: 2.0.0
+Version: 2.1.0
 Summary: Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 Home-page: https://github.com/mattdoug604/pyvariant.git
 Author: Matthew Douglas
 Author-email: mattdoug604@gmail.com
 Maintainer: Matthew Douglas
 Maintainer-email: mattdoug604@gmail.com
 License: MIT
```

### Comparing `pyvariant-2.0.0/pyvariant.egg-info/SOURCES.txt` & `pyvariant-2.1.0/pyvariant.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 pyvariant.egg-info/entry_points.txt
 pyvariant.egg-info/requires.txt
 pyvariant.egg-info/top_level.txt
 pyvariant.egg-info/zip-safe
 pyvariant/data/empty.fa
 pyvariant/data/empty.fa.fai
 tests/test_core.py
+tests/test_core_map.py
 tests/test_ensembl_cache.py
 tests/test_ensembl_release.py
 tests/test_files.py
 tests/test_init.py
 tests/test_parser.py
 tests/test_sequence.py
 tests/test_utils.py
```

### Comparing `pyvariant-2.0.0/setup.cfg` & `pyvariant-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyvariant
-version = 2.0.0
+version = 2.1.0
 description = Map biological sequence variants (mutations) to their equivalent chromosome, cDNA, gene, exon, protein, and RNA positions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mattdoug604/pyvariant.git
 author = Matthew Douglas
 author_email = mattdoug604@gmail.com
 maintainer = Matthew Douglas
```

### Comparing `pyvariant-2.0.0/tests/test_core.py` & `pyvariant-2.1.0/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pandas as pd
 import pytest
 from constants import (
-    CANONICAL_TRANSCRIPT,
-    CONTIG_ALIAS,
-    EXON_ALIAS,
-    GENE_ALIAS,
-    PROTEIN_ALIAS,
+    TEST_ENS100_CANONICAL_TRANSCRIPT,
     TEST_ENS100_CDNA_FASTA,
+    TEST_ENS100_CONTIG_ALIAS,
     TEST_ENS100_DNA_FASTA,
+    TEST_ENS100_EXON_ALIAS,
+    TEST_ENS100_GENE_ALIAS,
     TEST_ENS100_GTF,
     TEST_ENS100_NCRNA_FASTA,
     TEST_ENS100_PEP_FASTA,
-    TRANSCRIPT_ALIAS,
+    TEST_ENS100_PROTEIN_ALIAS,
+    TEST_ENS100_TRANSCRIPT_ALIAS,
 )
 
 from pyvariant.constants import (
     CONTIG_ID,
     EXON_ID,
     GENE_ID,
     GENE_NAME,
@@ -52,20 +52,20 @@
 def test_init():
     obj = Core(
         gtf=TEST_ENS100_GTF,
         cds=[TEST_ENS100_CDNA_FASTA],
         dna=[TEST_ENS100_DNA_FASTA],
         peptide=[TEST_ENS100_PEP_FASTA],
         rna=[TEST_ENS100_NCRNA_FASTA],
-        canonical_transcript=CANONICAL_TRANSCRIPT,
-        contig_alias=CONTIG_ALIAS,
-        exon_alias=EXON_ALIAS,
-        gene_alias=GENE_ALIAS,
-        protein_alias=PROTEIN_ALIAS,
-        transcript_alias=TRANSCRIPT_ALIAS,
+        canonical_transcript=TEST_ENS100_CANONICAL_TRANSCRIPT,
+        contig_alias=TEST_ENS100_CONTIG_ALIAS,
+        exon_alias=TEST_ENS100_EXON_ALIAS,
+        gene_alias=TEST_ENS100_GENE_ALIAS,
+        protein_alias=TEST_ENS100_PROTEIN_ALIAS,
+        transcript_alias=TEST_ENS100_TRANSCRIPT_ALIAS,
     )
     assert isinstance(obj.df, pd.DataFrame)
     assert isinstance(obj.cds_fasta, list)
     assert isinstance(obj.cds_fasta[0], PyfaidxFasta)
     assert isinstance(obj.dna_fasta, list)
     assert isinstance(obj.dna_fasta[0], PyfaidxFasta)
     assert isinstance(obj.protein_fasta, list)
@@ -82,27 +82,29 @@
 
 # -------------------------------------------------------------------------------------------------
 # to_cdna
 # -------------------------------------------------------------------------------------------------
 def test_to_cdna_canonical(ensembl100):
     assert ensembl100.to_cdna("7:g.127589084", canonical=False) == [
         CdnaPosition(
+            _core=ensembl100,
             contig_id="7",
             start=69,
             start_offset=0,
             end=69,
             end_offset=0,
             strand="+",
             gene_id="ENSG00000004059",
             gene_name="ARF5",
             transcript_id="ENST00000000233",
             transcript_name="ARF5-201",
             protein_id="ENSP00000000233",
         ),
         CdnaPosition(
+            _core=ensembl100,
             contig_id="7",
             start=69,
             start_offset=0,
             end=69,
             end_offset=0,
             strand="+",
             gene_id="ENSG00000004059",
@@ -110,14 +112,15 @@
             transcript_id="ENST00000415666",
             transcript_name="ARF5-202",
             protein_id="ENSP00000412701",
         ),
     ]
     assert ensembl100.to_cdna("7:g.127589084", canonical=True) == [
         CdnaPosition(
+            _core=ensembl100,
             contig_id="7",
             start=69,
             start_offset=0,
             end=69,
             end_offset=0,
             strand="+",
             gene_id="ENSG00000004059",
@@ -133,14 +136,15 @@
 # to_protein
 # -------------------------------------------------------------------------------------------------
 def test_to_protein_from_dna(ensembl100):
     assert ensembl100.to_protein("17:g.7674252G>A") == [
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=237,
             start_offset=0,
             end=237,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -148,14 +152,15 @@
             transcript_id="ENST00000269305",
             transcript_name="TP53-201",
             protein_id="ENSP00000269305",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=237,
             start_offset=0,
             end=237,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -163,14 +168,15 @@
             transcript_id="ENST00000359597",
             transcript_name="TP53-202",
             protein_id="ENSP00000352610",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=237,
             start_offset=0,
             end=237,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -178,14 +184,15 @@
             transcript_id="ENST00000420246",
             transcript_name="TP53-204",
             protein_id="ENSP00000391127",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=237,
             start_offset=0,
             end=237,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -193,14 +200,15 @@
             transcript_id="ENST00000445888",
             transcript_name="TP53-205",
             protein_id="ENSP00000391478",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=237,
             start_offset=0,
             end=237,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -208,14 +216,15 @@
             transcript_id="ENST00000455263",
             transcript_name="TP53-206",
             protein_id="ENSP00000398846",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=237,
             start_offset=0,
             end=237,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -223,14 +232,15 @@
             transcript_id="ENST00000413465",
             transcript_name="TP53-203",
             protein_id="ENSP00000410739",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=144,
             start_offset=0,
             end=144,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -238,14 +248,15 @@
             transcript_id="ENST00000514944",
             transcript_name="TP53-214",
             protein_id="ENSP00000423862",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=105,
             start_offset=0,
             end=105,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -253,14 +264,15 @@
             transcript_id="ENST00000509690",
             transcript_name="TP53-212",
             protein_id="ENSP00000425104",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=78,
             start_offset=0,
             end=78,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -268,14 +280,15 @@
             transcript_id="ENST00000610623",
             transcript_name="TP53-221",
             protein_id="ENSP00000477531",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=198,
             start_offset=0,
             end=198,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -283,14 +296,15 @@
             transcript_id="ENST00000610292",
             transcript_name="TP53-219",
             protein_id="ENSP00000478219",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=105,
             start_offset=0,
             end=105,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -298,14 +312,15 @@
             transcript_id="ENST00000510385",
             transcript_name="TP53-213",
             protein_id="ENSP00000478499",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=198,
             start_offset=0,
             end=198,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -313,14 +328,15 @@
             transcript_id="ENST00000610538",
             transcript_name="TP53-220",
             protein_id="ENSP00000480868",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=105,
             start_offset=0,
             end=105,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -328,14 +344,15 @@
             transcript_id="ENST00000504937",
             transcript_name="TP53-209",
             protein_id="ENSP00000481179",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=78,
             start_offset=0,
             end=78,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -343,14 +360,15 @@
             transcript_id="ENST00000618944",
             transcript_name="TP53-224",
             protein_id="ENSP00000481401",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=198,
             start_offset=0,
             end=198,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -358,14 +376,15 @@
             transcript_id="ENST00000620739",
             transcript_name="TP53-227",
             protein_id="ENSP00000481638",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=198,
             start_offset=0,
             end=198,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -373,14 +392,15 @@
             transcript_id="ENST00000622645",
             transcript_name="TP53-228",
             protein_id="ENSP00000482222",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=237,
             start_offset=0,
             end=237,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -388,14 +408,15 @@
             transcript_id="ENST00000617185",
             transcript_name="TP53-223",
             protein_id="ENSP00000482258",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=198,
             start_offset=0,
             end=198,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -403,14 +424,15 @@
             transcript_id="ENST00000619485",
             transcript_name="TP53-226",
             protein_id="ENSP00000482537",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=226,
             start_offset=0,
             end=226,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -418,14 +440,15 @@
             transcript_id="ENST00000615910",
             transcript_name="TP53-222",
             protein_id="ENSP00000482903",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=78,
             start_offset=0,
             end=78,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -433,14 +456,15 @@
             transcript_id="ENST00000619186",
             transcript_name="TP53-225",
             protein_id="ENSP00000484375",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=105,
             start_offset=0,
             end=105,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -448,14 +472,15 @@
             transcript_id="ENST00000504290",
             transcript_name="TP53-208",
             protein_id="ENSP00000484409",
         ),
         ProteinSubstitution(
             refseq="M",
             altseq="I",
+            _core=ensembl100,
             contig_id="17",
             start=198,
             start_offset=0,
             end=198,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000141510",
@@ -894,16 +919,17 @@
     assert ensembl100.is_transcript("ALDOA-219") is True
 
 
 # -------------------------------------------------------------------------------------------------
 # sequence
 # -------------------------------------------------------------------------------------------------
 @pytest.fixture
-def test_sequence_cdna_pos():
+def test_sequence_cdna_pos(ensembl100):
     return CdnaPosition(
+        ensembl100,
         "4",
         7,
         0,
         9,
         0,
         "+",
         "ENSG00000157404",
@@ -915,31 +941,32 @@
 
 
 def test_sequence_cdna(ensembl100, test_sequence_cdna_pos):
     assert ensembl100.sequence(test_sequence_cdna_pos) == "GGC"
 
 
 @pytest.fixture
-def test_sequence_dna_pos_plus():
-    return DnaPosition("4", 54695512, 0, 54695514, 0, "+")
+def test_sequence_dna_pos_plus(ensembl100):
+    return DnaPosition(ensembl100, "4", 54695512, 0, 54695514, 0, "+")
 
 
 @pytest.fixture
-def test_sequence_dna_pos_minus():
-    return DnaPosition("4", 54695512, 0, 54695514, 0, "-")
+def test_sequence_dna_pos_minus(ensembl100):
+    return DnaPosition(ensembl100, "4", 54695512, 0, 54695514, 0, "-")
 
 
 def test_sequence_dna(ensembl100, test_sequence_dna_pos_plus, test_sequence_dna_pos_minus):
     assert ensembl100.sequence(test_sequence_dna_pos_plus) == "GCT"
     assert ensembl100.sequence(test_sequence_dna_pos_minus) == "AGC"
 
 
 @pytest.fixture
-def test_sequence_protein_pos():
+def test_sequence_protein_pos(ensembl100):
     return ProteinPosition(
+        ensembl100,
         "4",
         3,
         0,
         4,
         0,
         "+",
         "ENSG00000157404",
@@ -951,17 +978,17 @@
 
 
 def test_sequence_protein(ensembl100, test_sequence_protein_pos):
     assert ensembl100.sequence(test_sequence_protein_pos) == "GA"
 
 
 @pytest.fixture
-def test_sequence_rna_pos():
+def test_sequence_rna_pos(ensembl100):
     return RnaPosition(
-        "4", 126, 0, 128, 0, "+", "ENSG00000157404", "KIT", "ENST00000288135", "KIT-201"
+        ensembl100, "4", 126, 0, 128, 0, "+", "ENSG00000157404", "KIT", "ENST00000288135", "KIT-201"
     )
 
 
 def test_sequence_rna(ensembl100, test_sequence_rna_pos):
     assert ensembl100.sequence(test_sequence_rna_pos) == "GCT"
 
 
@@ -1060,16 +1087,17 @@
     assert ensembl100.normalize_id("ALDOA-219") == [("ALDOA-219", TRANSCRIPT_NAME)]
 
 
 # -------------------------------------------------------------------------------------------------
 # cdna
 # -------------------------------------------------------------------------------------------------
 @pytest.fixture
-def test_cdna_pos():
+def test_cdna_pos(ensembl100):
     return CdnaPosition(
+        _core=ensembl100,
         contig_id="5",
         start=1,
         start_offset=0,
         end=3399,
         end_offset=0,
         strand="-",
         gene_id="ENSG00000164362",
@@ -1104,17 +1132,23 @@
     assert results[0].transcript_id == "ENST00000000233"
 
 
 # -------------------------------------------------------------------------------------------------
 # dna
 # -------------------------------------------------------------------------------------------------
 @pytest.fixture
-def expected_dna():
+def expected_dna(ensembl100):
     return DnaPosition(
-        contig_id="5", start=1253147, start_offset=0, end=1295068, end_offset=0, strand="-"
+        _core=ensembl100,
+        contig_id="5",
+        start=1253147,
+        start_offset=0,
+        end=1295068,
+        end_offset=0,
+        strand="-",
     )
 
 
 @pytest.mark.parametrize(
     "feature,num_results",
     [
         ("5", 2987),
@@ -1129,17 +1163,23 @@
 def test_gene(ensembl100, expected_dna, feature, num_results):
     results = ensembl100.gene(feature)
     assert len(results) == num_results
     assert expected_dna in results
 
 
 @pytest.fixture
-def test_dna_pos_whole_contig():
+def test_dna_pos_whole_contig(ensembl100):
     return DnaPosition(
-        contig_id="5", start=1, start_offset=0, end=181538259, end_offset=0, strand="-"
+        _core=ensembl100,
+        contig_id="5",
+        start=1,
+        start_offset=0,
+        end=181538259,
+        end_offset=0,
+        strand="-",
     )
 
 
 @pytest.mark.parametrize(
     "feature,num_results",
     [
         ("5", 2),
@@ -1157,16 +1197,17 @@
     assert test_dna_pos_whole_contig in results
 
 
 # -------------------------------------------------------------------------------------------------
 # exon
 # -------------------------------------------------------------------------------------------------
 @pytest.fixture
-def test_exon_pos():
+def test_exon_pos(ensembl100):
     return ExonPosition(
+        _core=ensembl100,
         contig_id="5",
         start=1,
         start_offset=0,
         end=1,
         end_offset=0,
         strand="-",
         gene_id="ENSG00000164362",
@@ -1202,16 +1243,17 @@
         assert exon.transcript_id == "ENST00000000233"
 
 
 # -------------------------------------------------------------------------------------------------
 # protein
 # -------------------------------------------------------------------------------------------------
 @pytest.fixture
-def test_protein_pos():
+def test_protein_pos(ensembl100):
     return ProteinPosition(
+        _core=ensembl100,
         contig_id="5",
         start=1,
         start_offset=0,
         end=1133,
         end_offset=0,
         strand="-",
         gene_id="ENSG00000164362",
@@ -1246,16 +1288,17 @@
     assert results[0].transcript_id == "ENST00000000233"
 
 
 # -------------------------------------------------------------------------------------------------
 # rna
 # -------------------------------------------------------------------------------------------------
 @pytest.fixture
-def test_rna_pos():
+def test_rna_pos(ensembl100):
     return RnaPosition(
+        _core=ensembl100,
         contig_id="5",
         start=1,
         start_offset=0,
         end=4039,
         end_offset=0,
         strand="-",
         gene_id="ENSG00000164362",
@@ -1289,16 +1332,17 @@
     assert results[0].transcript_id == "ENST00000000233"
 
 
 # -------------------------------------------------------------------------------------------------
 # translate_cdna_variant
 # -------------------------------------------------------------------------------------------------
 @pytest.fixture
-def test_translate_cdna_variant_pos_1():
+def test_translate_cdna_variant_pos_1(ensembl100):
     return CdnaPosition(
+        ensembl100,
         "4",
         38,
         0,
         38,
         0,
         "+",
         "ENSG00000157404",
@@ -1329,16 +1373,17 @@
 def test_translate_cdna_variant_3(ensembl100, test_translate_cdna_variant_pos_1):
     # A frameshifting deletion of T
     # GTT -> GT
     assert ensembl100.translate_cdna_variant(test_translate_cdna_variant_pos_1, "") == [("", True)]
 
 
 @pytest.fixture
-def test_translate_cdna_variant_pos_2():
+def test_translate_cdna_variant_pos_2(ensembl100):
     return CdnaPosition(
+        ensembl100,
         "4",
         38,
         0,
         40,
         0,
         "+",
         "ENSG00000157404",
@@ -1362,16 +1407,17 @@
     # GTTCTG -> GTG
     assert ensembl100.translate_cdna_variant(test_translate_cdna_variant_pos_2, "") == [
         ("V", False)
     ]
 
 
 @pytest.fixture
-def test_translate_cdna_variant_pos_3():
+def test_translate_cdna_variant_pos_3(ensembl100):
     return CdnaPosition(
+        ensembl100,
         "4",
         1674,
         0,
         1675,
         0,
         "+",
         "ENSG00000157404",
@@ -1401,14 +1447,15 @@
 # -------------------------------------------------------------------------------------------------
 # parse
 # -------------------------------------------------------------------------------------------------
 def test_parse_cdna_position(ensembl100):
     result = ensembl100.parse("ENST00000288135:c.68-1")
     assert result == [
         CdnaPosition(
+            _core=ensembl100,
             contig_id="4",
             start=68,
             start_offset=-1,
             end=68,
             end_offset=-1,
             strand="+",
             gene_id="ENSG00000157404",
@@ -1420,14 +1467,15 @@
     ]
 
 
 def test_parse_cdna_intron_deletion(ensembl100):
     result = ensembl100.parse("ENST00000372348:c.136+596_136+650del")
     assert result == [
         CdnaDeletion(
+            _core=ensembl100,
             contig_id="9",
             start=136,
             start_offset=596,
             end=136,
             end_offset=650,
             strand="+",
             gene_id="ENSG00000097007",
@@ -1442,15 +1490,15 @@
 
 
 def test_parse_cdna_stop_deletion(ensembl100):
     # TODO: Support positions offset from stop codon
     # result = ensembl100.parse("ENST00000257430:c.*6_*7del")
     # assert result == [
     #     CdnaDeletion(
-    #         contig_id="9",
+    #         _core=ensembl100,contig_id="9",
     #         start=10704,
     #         start_offset=6,
     #         end=10704,
     #         end_offset=7,
     #         strand="+",
     #         gene_id="ENSG00000134982",
     #         gene_name="ABL1",
@@ -1465,14 +1513,15 @@
         ensembl100.parse("ENST00000257430:c.*6_*7del")
 
 
 def test_parse_cdna_promoter_delins_multiple(ensembl100):
     result = ensembl100.parse("ENST00000257430:c.-30347_-30346delinsA")
     assert result == [
         CdnaDelins(
+            _core=ensembl100,
             contig_id="5",
             start=1,
             start_offset=-30347,
             end=1,
             end_offset=-30346,
             strand="+",
             gene_id="ENSG00000134982",
@@ -1486,14 +1535,15 @@
     ]
 
 
 def test_parse_cdna_promoter_delins_to_deletion(ensembl100):
     result = ensembl100.parse("ENST00000257430:c.-30353_-30352delinsA")
     assert result == [
         CdnaDeletion(
+            _core=ensembl100,
             contig_id="5",
             start=1,
             start_offset=-30353,
             end=1,
             end_offset=-30353,
             strand="+",
             gene_id="ENSG00000134982",
@@ -1507,14 +1557,15 @@
     ]
 
 
 def test_parse_cdna_duplication(ensembl100):
     result = ensembl100.parse("ENST00000307078:c.1394_1399dup")
     assert result == [
         CdnaDuplication(
+            _core=ensembl100,
             contig_id="17",
             start=1394,
             start_offset=0,
             end=1399,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000168646",
@@ -1528,14 +1579,15 @@
     ]
 
 
 def test_parse_cdna_promoter_substitution(ensembl100):
     result = ensembl100.parse("ENST00000257430:c.-290G>A")
     assert result == [
         CdnaSubstitution(
+            _core=ensembl100,
             contig_id="5",
             start=1,
             start_offset=-290,
             end=1,
             end_offset=-290,
             strand="+",
             gene_id="ENSG00000134982",
@@ -1549,14 +1601,15 @@
     ]
 
 
 def test_parse_cdna_substitution(ensembl100):
     result = ensembl100.parse("ENST00000256078:c.38G>A")
     assert result == [
         CdnaSubstitution(
+            _core=ensembl100,
             contig_id="12",
             start=38,
             start_offset=0,
             end=38,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000133703",
@@ -1570,23 +1623,30 @@
     ]
 
 
 def test_parse_dna_position(ensembl100):
     result = ensembl100.parse("5:g.1282623_1282626")
     assert result == [
         DnaPosition(
-            contig_id="5", start=1282623, start_offset=0, end=1282626, end_offset=0, strand=""
+            _core=ensembl100,
+            contig_id="5",
+            start=1282623,
+            start_offset=0,
+            end=1282626,
+            end_offset=0,
+            strand="",
         )
     ]
 
 
 def test_parse_dna_substitution(ensembl100):
     result = ensembl100.parse("5:g.1282623C>G")
     assert result == [
         DnaSubstitution(
+            _core=ensembl100,
             contig_id="5",
             start=1282623,
             start_offset=0,
             end=1282623,
             end_offset=0,
             strand="",
             refseq="C",
@@ -1595,28 +1655,31 @@
     ]
 
 
 def test_parse_exon_fusion(ensembl100):
     result = ensembl100.parse("ENST00000315869:e.3_4::ENST00000271526:e.2")
     assert result == [
         ExonFusion(
+            ensembl100,
             ExonPosition(
+                _core=ensembl100,
                 contig_id="X",
                 start=3,
                 start_offset=0,
                 end=4,
                 end_offset=0,
                 strand="-",
                 gene_id="ENSG00000068323",
                 gene_name="TFE3",
                 transcript_id="ENST00000315869",
                 transcript_name="TFE3-201",
                 exon_id="ENSE00003528623",
             ),
             ExonPosition(
+                _core=ensembl100,
                 contig_id="1",
                 start=2,
                 start_offset=0,
                 end=2,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000143294",
@@ -1632,14 +1695,15 @@
 # -------------------------------------------------------------------------------------------------
 # variant
 # -------------------------------------------------------------------------------------------------
 def test_variant_cdna_minimal(ensembl100):
     result = ensembl100.variant(position_type="cdna", feature="ENST00000375562", start=123)
     assert result == [
         CdnaPosition(
+            _core=ensembl100,
             contig_id="6",
             start=123,
             start_offset=0,
             end=123,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000204385",
@@ -1659,14 +1723,15 @@
         start_offset=-1,
         end=68,
         end_offset=-1,
         strand="+",
     )
     assert result == [
         CdnaPosition(
+            _core=ensembl100,
             contig_id="4",
             start=68,
             start_offset=-1,
             end=68,
             end_offset=-1,
             strand="+",
             gene_id="ENSG00000157404",
@@ -1689,14 +1754,15 @@
         strand="-",
         refseq="G",
         altseq="A",
         variant_type="substitution",
     )
     assert result == [
         CdnaSubstitution(
+            _core=ensembl100,
             contig_id="12",
             start=38,
             start_offset=0,
             end=38,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000133703",
@@ -1710,26 +1776,38 @@
     ]
 
 
 def test_variant_dna_minimal(ensembl100):
     result = ensembl100.variant(position_type="dna", feature="5", start=1282623)
     assert result == [
         DnaPosition(
-            contig_id="5", start=1282623, start_offset=0, end=1282623, end_offset=0, strand=""
+            _core=ensembl100,
+            contig_id="5",
+            start=1282623,
+            start_offset=0,
+            end=1282623,
+            end_offset=0,
+            strand="",
         )
     ]
 
 
 def test_variant_dna_position(ensembl100):
     result = ensembl100.variant(
         position_type="dna", feature="5", start=1282623, end=1282626, strand="-"
     )
     assert result == [
         DnaPosition(
-            contig_id="5", start=1282623, start_offset=0, end=1282626, end_offset=0, strand="-"
+            _core=ensembl100,
+            contig_id="5",
+            start=1282623,
+            start_offset=0,
+            end=1282626,
+            end_offset=0,
+            strand="-",
         )
     ]
 
 
 def test_variant_dna_insertion_normalized(ensembl100):
     result = ensembl100.variant(
         position_type="dna",
@@ -1739,14 +1817,15 @@
         strand="+",
         refseq="A",
         altseq="AT",
         variant_type="insertion",
     )
     assert result == [
         DnaInsertion(
+            _core=ensembl100,
             contig_id="1",
             start=826577,
             start_offset=0,
             end=826578,
             end_offset=0,
             strand="+",
             refseq="AC",
@@ -1764,14 +1843,15 @@
         strand="+",
         refseq="C",
         altseq="G",
         variant_type="substitution",
     )
     assert result == [
         DnaSubstitution(
+            _core=ensembl100,
             contig_id="5",
             start=1282623,
             start_offset=0,
             end=1282623,
             end_offset=0,
             strand="+",
             refseq="C",
@@ -1792,28 +1872,31 @@
         feature2="ENST00000271526",
         start2=2,
         end2=2,
         strand2="+",
     )
     assert result == [
         ExonFusion(
+            ensembl100,
             ExonPosition(
+                _core=ensembl100,
                 contig_id="X",
                 start=3,
                 start_offset=0,
                 end=4,
                 end_offset=0,
                 strand="-",
                 gene_id="ENSG00000068323",
                 gene_name="TFE3",
                 transcript_id="ENST00000315869",
                 transcript_name="TFE3-201",
                 exon_id="ENSE00003528623",
             ),
             ExonPosition(
+                _core=ensembl100,
                 contig_id="1",
                 start=2,
                 start_offset=0,
                 end=2,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000143294",
@@ -1832,14 +1915,15 @@
 def test_to_all_from_cdna_delins(ensembl100):
     result = ensembl100.to_all("ENST00000288135:c.126_128delinsGT")
     assert result == {
         "cdna": [
             CdnaDelins(
                 refseq="AAA",
                 altseq="GT",
+                _core=ensembl100,
                 contig_id="4",
                 start=126,
                 start_offset=0,
                 end=128,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
@@ -1849,27 +1933,29 @@
                 protein_id="ENSP00000288135",
             )
         ],
         "dna": [
             DnaDelins(
                 refseq="AAA",
                 altseq="GT",
+                _core=ensembl100,
                 contig_id="4",
                 start=54695570,
                 start_offset=0,
                 end=54695572,
                 end_offset=0,
                 strand="+",
             )
         ],
         "exon": [],
         "protein": [
             ProteinFrameshift(
                 refseq="K",
                 altseq="",
+                _core=ensembl100,
                 contig_id="4",
                 start=43,
                 start_offset=0,
                 end=43,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
@@ -1879,14 +1965,15 @@
                 protein_id="ENSP00000288135",
             )
         ],
         "rna": [
             RnaDelins(
                 refseq="AAA",
                 altseq="GT",
+                _core=ensembl100,
                 contig_id="4",
                 start=184,
                 start_offset=0,
                 end=186,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
@@ -1899,27 +1986,29 @@
 
 
 def test_to_all_from_dna_position(ensembl100):
     result = ensembl100.to_all("4:g.54695570_54695572")
     assert result == {
         "cdna": [
             CdnaPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=126,
                 start_offset=0,
                 end=128,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
                 gene_name="KIT",
                 transcript_id="ENST00000288135",
                 transcript_name="KIT-201",
                 protein_id="ENSP00000288135",
             ),
             CdnaPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=126,
                 start_offset=0,
                 end=128,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
@@ -1927,45 +2016,54 @@
                 transcript_id="ENST00000412167",
                 transcript_name="KIT-202",
                 protein_id="ENSP00000390987",
             ),
         ],
         "dna": [
             DnaPosition(
-                contig_id="4", start=54695570, start_offset=0, end=54695572, end_offset=0, strand=""
+                _core=ensembl100,
+                contig_id="4",
+                start=54695570,
+                start_offset=0,
+                end=54695572,
+                end_offset=0,
+                strand="",
             )
         ],
         "exon": [
             ExonPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=2,
                 start_offset=0,
                 end=2,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
                 gene_name="KIT",
                 transcript_id="ENST00000288135",
                 transcript_name="KIT-201",
                 exon_id="ENSE00001032350",
             ),
             ExonPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=2,
                 start_offset=0,
                 end=2,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
                 gene_name="KIT",
                 transcript_id="ENST00000412167",
                 transcript_name="KIT-202",
                 exon_id="ENSE00001032350",
             ),
             ExonPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=2,
                 start_offset=0,
                 end=2,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
@@ -1973,27 +2071,29 @@
                 transcript_id="ENST00000514582",
                 transcript_name="KIT-204",
                 exon_id="ENSE00002084370",
             ),
         ],
         "protein": [
             ProteinPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=42,
                 start_offset=0,
                 end=43,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
                 gene_name="KIT",
                 transcript_id="ENST00000288135",
                 transcript_name="KIT-201",
                 protein_id="ENSP00000288135",
             ),
             ProteinPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=42,
                 start_offset=0,
                 end=43,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
@@ -2001,38 +2101,41 @@
                 transcript_id="ENST00000412167",
                 transcript_name="KIT-202",
                 protein_id="ENSP00000390987",
             ),
         ],
         "rna": [
             RnaPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=184,
                 start_offset=0,
                 end=186,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
                 gene_name="KIT",
                 transcript_id="ENST00000288135",
                 transcript_name="KIT-201",
             ),
             RnaPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=223,
                 start_offset=0,
                 end=225,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
                 gene_name="KIT",
                 transcript_id="ENST00000412167",
                 transcript_name="KIT-202",
             ),
             RnaPosition(
+                _core=ensembl100,
                 contig_id="4",
                 start=202,
                 start_offset=0,
                 end=204,
                 end_offset=0,
                 strand="+",
                 gene_id="ENSG00000157404",
@@ -2050,14 +2153,15 @@
 def test_diff(ensembl100):
     assert ensembl100.diff("ENSP00000358548:p.Q61K", "NRAS:c.181C>A") == {
         "cdna": (
             [
                 CdnaDelins(
                     refseq="CAA",
                     altseq="AAG",
+                    _core=ensembl100,
                     contig_id="1",
                     start=181,
                     start_offset=0,
                     end=183,
                     end_offset=0,
                     strand="-",
                     gene_id="ENSG00000213281",
@@ -2070,14 +2174,15 @@
             [],
         ),
         "dna": (
             [
                 DnaDelins(
                     refseq="CAA",
                     altseq="AAG",
+                    _core=ensembl100,
                     contig_id="1",
                     start=114713907,
                     start_offset=0,
                     end=114713909,
                     end_offset=0,
                     strand="-",
                 )
@@ -2087,14 +2192,15 @@
         "exon": ([], []),
         "protein": ([], []),
         "rna": (
             [
                 RnaDelins(
                     refseq="CAA",
                     altseq="AAG",
+                    _core=ensembl100,
                     contig_id="1",
                     start=312,
                     start_offset=0,
                     end=314,
                     end_offset=0,
                     strand="-",
                     gene_id="ENSG00000213281",
@@ -2110,14 +2216,15 @@
 
 def test_same(ensembl100):
     assert ensembl100.same("ENSP00000358548:p.Q61K", "NRAS:c.181C>A") == {
         "cdna": [
             CdnaSubstitution(
                 refseq="C",
                 altseq="A",
+                _core=ensembl100,
                 contig_id="1",
                 start=181,
                 start_offset=0,
                 end=181,
                 end_offset=0,
                 strand="-",
                 gene_id="ENSG00000213281",
@@ -2127,27 +2234,29 @@
                 protein_id="ENSP00000358548",
             )
         ],
         "dna": [
             DnaSubstitution(
                 refseq="C",
                 altseq="A",
+                _core=ensembl100,
                 contig_id="1",
                 start=114713909,
                 start_offset=0,
                 end=114713909,
                 end_offset=0,
                 strand="-",
             )
         ],
         "exon": [],
         "protein": [
             ProteinSubstitution(
                 refseq="Q",
                 altseq="K",
+                _core=ensembl100,
                 contig_id="1",
                 start=61,
                 start_offset=0,
                 end=61,
                 end_offset=0,
                 strand="-",
                 gene_id="ENSG00000213281",
@@ -2157,14 +2266,15 @@
                 protein_id="ENSP00000358548",
             )
         ],
         "rna": [
             RnaSubstitution(
                 refseq="C",
                 altseq="A",
+                _core=ensembl100,
                 contig_id="1",
                 start=312,
                 start_offset=0,
                 end=312,
                 end_offset=0,
                 strand="-",
                 gene_id="ENSG00000213281",
@@ -2177,14 +2287,15 @@
 
 
 def test_same_cdna(ensembl100):
     assert ensembl100.same_cdna("ENSP00000358548:p.Q61K", "NRAS:c.181C>A") == [
         CdnaSubstitution(
             refseq="C",
             altseq="A",
+            _core=ensembl100,
             contig_id="1",
             start=181,
             start_offset=0,
             end=181,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000213281",
@@ -2197,27 +2308,29 @@
 
 
 def test_same_dna(ensembl100):
     assert ensembl100.same_dna("ENSP00000358548:p.Q61K", "NRAS:c.181C>A") == [
         DnaSubstitution(
             refseq="C",
             altseq="A",
+            _core=ensembl100,
             contig_id="1",
             start=114713909,
             start_offset=0,
             end=114713909,
             end_offset=0,
             strand="-",
         )
     ]
 
 
 def test_same_exon(ensembl100):
     assert ensembl100.same_exon("ENSP00000358548:p.61", "NRAS:c.181") == [
         ExonPosition(
+            _core=ensembl100,
             contig_id="1",
             start=3,
             start_offset=0,
             end=3,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000213281",
@@ -2230,14 +2343,15 @@
 
 
 def test_same_protein(ensembl100):
     assert ensembl100.same_protein("ENSP00000358548:p.Q61K", "NRAS:c.181C>A") == [
         ProteinSubstitution(
             refseq="Q",
             altseq="K",
+            _core=ensembl100,
             contig_id="1",
             start=61,
             start_offset=0,
             end=61,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000213281",
@@ -2250,14 +2364,15 @@
 
 
 def test_same_rna(ensembl100):
     assert ensembl100.same_rna("ENSP00000358548:p.Q61K", "NRAS:c.181C>A") == [
         RnaSubstitution(
             refseq="C",
             altseq="A",
+            _core=ensembl100,
             contig_id="1",
             start=312,
             start_offset=0,
             end=312,
             end_offset=0,
             strand="-",
             gene_id="ENSG00000213281",
```

### Comparing `pyvariant-2.0.0/tests/test_ensembl_release.py` & `pyvariant-2.1.0/tests/test_ensembl_release.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import pandas as pd
 from constants import (
     CACHE_DIR,
-    CANONICAL_TRANSCRIPT,
-    CONTIG_ALIAS,
-    EXON_ALIAS,
-    GENE_ALIAS,
-    PROTEIN_ALIAS,
-    TRANSCRIPT_ALIAS,
+    TEST_ENS100_CANONICAL_TRANSCRIPT,
+    TEST_ENS100_CONTIG_ALIAS,
+    TEST_ENS100_EXON_ALIAS,
+    TEST_ENS100_GENE_ALIAS,
+    TEST_ENS100_PROTEIN_ALIAS,
+    TEST_ENS100_TRANSCRIPT_ALIAS,
 )
 
 from pyvariant.ensembl_release import EnsemblRelease
 from pyvariant.sequence import PyfaidxFasta
 
 
 def test_init():
     obj = EnsemblRelease(
         species="homo_sapiens",
         release=100,
         cache_dir=CACHE_DIR,
-        canonical_transcript=CANONICAL_TRANSCRIPT,
-        contig_alias=CONTIG_ALIAS,
-        exon_alias=EXON_ALIAS,
-        gene_alias=GENE_ALIAS,
-        protein_alias=PROTEIN_ALIAS,
-        transcript_alias=TRANSCRIPT_ALIAS,
+        canonical_transcript=TEST_ENS100_CANONICAL_TRANSCRIPT,
+        contig_alias=TEST_ENS100_CONTIG_ALIAS,
+        exon_alias=TEST_ENS100_EXON_ALIAS,
+        gene_alias=TEST_ENS100_GENE_ALIAS,
+        protein_alias=TEST_ENS100_PROTEIN_ALIAS,
+        transcript_alias=TEST_ENS100_TRANSCRIPT_ALIAS,
     )
     assert isinstance(obj.df, pd.DataFrame)
     assert isinstance(obj.cds_fasta, list)
     assert not obj.cds_fasta
     assert isinstance(obj.dna_fasta, list)
     assert isinstance(obj.dna_fasta[0], PyfaidxFasta)
     assert isinstance(obj.protein_fasta, list)
```

### Comparing `pyvariant-2.0.0/tests/test_files.py` & `pyvariant-2.1.0/tests/test_files.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import gzip
 import os
 import os.path
 
 import pytest
 from Bio.bgzf import BgzfWriter
-from constants import CANONICAL_TRANSCRIPT, CONTIG_ALIAS
+from constants import TEST_ENS100_CANONICAL_TRANSCRIPT, TEST_ENS100_CONTIG_ALIAS
 
 from pyvariant.constants import CACHE_DIR_ENV, CACHE_DIR_NAME
 from pyvariant.files import bgzip, get_cache_dir, is_bgzipped, tsv_to_dict, txt_to_list
 
 
 @pytest.fixture
 def bgzip_file(tmpdir) -> str:
@@ -72,14 +72,14 @@
 
 
 def test_get_cache_dir_env_var(cache_env_var):
     assert get_cache_dir() == "TEST"
 
 
 def test_tsv_to_dict():
-    result = tsv_to_dict(CONTIG_ALIAS)
-    assert result == {"chr4": ["4"]}
+    result = tsv_to_dict(TEST_ENS100_CONTIG_ALIAS)
+    assert result == {"chr12": ["12"], "chr13": ["13"]}
 
 
 def test_txt_to_list():
-    result = txt_to_list(CANONICAL_TRANSCRIPT)
-    assert result == ["ENST00000000233"]
+    result = txt_to_list(TEST_ENS100_CANONICAL_TRANSCRIPT)
+    assert result == ["ENST00000000233", "ENST00000256078", "ENST00000380152"]
```

### Comparing `pyvariant-2.0.0/tests/test_parser.py` & `pyvariant-2.1.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyvariant-2.0.0/tests/test_sequence.py` & `pyvariant-2.1.0/tests/test_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyvariant.sequence import PyfaidxFasta, get_sequence, mutate_sequence
 
 
 def test_pyfaidx_fasta_load():
     result = PyfaidxFasta.load(TEST_ENS100_CDNA_FASTA)
     assert isinstance(result, PyfaidxFasta)
     assert isinstance(result.fasta, Fasta)
-    assert result["ENST00000643777"]
+    assert result["ENST00000256078"]
 
 
 def test_pyfaidx_fasta_load_empty():
     result = PyfaidxFasta.load("")
     assert isinstance(result, PyfaidxFasta)
     assert isinstance(result.fasta, Fasta)
```

### Comparing `pyvariant-2.0.0/tests/test_utils.py` & `pyvariant-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

