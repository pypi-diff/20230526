# Comparing `tmp/fastgedcom-0.0.3.tar.gz` & `tmp/fastgedcom-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastgedcom-0.0.3.tar", last modified: Thu May 25 16:56:48 2023, max compression
+gzip compressed data, was "fastgedcom-0.0.4.tar", last modified: Fri May 26 20:37:58 2023, max compression
```

## Comparing `fastgedcom-0.0.3.tar` & `fastgedcom-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 16:56:48.632524 fastgedcom-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5000 2023-05-25 16:56:48.632524 fastgedcom-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4152 2023-05-25 16:53:48.000000 fastgedcom-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 16:56:48.592493 fastgedcom-0.0.3/fastgedcom/
--rw-rw-rw-   0        0        0      234 2023-05-20 15:25:33.000000 fastgedcom-0.0.3/fastgedcom/__init__.py
--rw-rw-rw-   0        0        0     9254 2023-05-24 23:22:27.000000 fastgedcom-0.0.3/fastgedcom/base.py
--rw-rw-rw-   0        0        0     1415 2023-05-24 17:51:16.000000 fastgedcom-0.0.3/fastgedcom/future.py
--rw-rw-rw-   0        0        0     5336 2023-05-24 22:45:41.000000 fastgedcom-0.0.3/fastgedcom/helpers.py
--rw-rw-rw-   0        0        0     3689 2023-05-24 22:13:35.000000 fastgedcom-0.0.3/fastgedcom/parser.py
--rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.3/fastgedcom/py.typed
--rw-rw-rw-   0        0        0     1436 2023-05-25 16:44:01.000000 fastgedcom-0.0.3/fastgedcom/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:56:48.624522 fastgedcom-0.0.3/fastgedcom.egg-info/
--rw-rw-rw-   0        0        0     5000 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 16:52:11.000000 fastgedcom-0.0.3/fastgedcom.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-25 16:56:48.000000 fastgedcom-0.0.3/fastgedcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 16:56:48.632524 fastgedcom-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1316 2023-05-25 16:47:45.000000 fastgedcom-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:37:58.297807 fastgedcom-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-05-22 23:10:18.000000 fastgedcom-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-05-25 13:57:11.000000 fastgedcom-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3874 2023-05-26 20:37:58.296810 fastgedcom-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3030 2023-05-26 20:32:34.000000 fastgedcom-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 20:37:58.274048 fastgedcom-0.0.4/fastgedcom/
+-rw-rw-rw-   0        0        0      236 2023-05-26 17:04:30.000000 fastgedcom-0.0.4/fastgedcom/__init__.py
+-rw-rw-rw-   0        0        0     6908 2023-05-26 17:50:33.000000 fastgedcom-0.0.4/fastgedcom/base.py
+-rw-rw-rw-   0        0        0     5045 2023-05-26 17:07:54.000000 fastgedcom-0.0.4/fastgedcom/family_aid.py
+-rw-rw-rw-   0        0        0     5508 2023-05-26 17:11:25.000000 fastgedcom-0.0.4/fastgedcom/helpers.py
+-rw-rw-rw-   0        0        0     2858 2023-05-26 16:55:14.000000 fastgedcom-0.0.4/fastgedcom/parser.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 13:48:45.000000 fastgedcom-0.0.4/fastgedcom/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-26 20:37:58.294808 fastgedcom-0.0.4/fastgedcom.egg-info/
+-rw-rw-rw-   0        0        0     3874 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 20:37:58.000000 fastgedcom-0.0.4/fastgedcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 20:37:58.297807 fastgedcom-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1312 2023-05-26 20:21:00.000000 fastgedcom-0.0.4/setup.py
```

### Comparing `fastgedcom-0.0.3/LICENSE` & `fastgedcom-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastgedcom-0.0.3/fastgedcom/helpers.py` & `fastgedcom-0.0.4/fastgedcom/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 from typing import Any, Callable, Iterator, Literal
 
-from .base import FakeLine, Gedcom, GedcomLine, line_exists
-from .structure import IndiRef
+from .base import Document, FakeLine, IndiRef, TrueLine, is_true
+from .family_aid import FamilyAid
 
 MINIMAL_DATE = -99999
 """Used to sort empty date fields"""
 
-def get_all_sub_records(line: GedcomLine) -> Iterator[GedcomLine]:
+def get_all_sub_lines(line: TrueLine) -> Iterator[TrueLine]:
 	"""Recursively iterate on all lines under the given line."""
-	sub_records = list(line.sub_rec)
-	while len(sub_records) > 0:
-		record = sub_records.pop(0)
-		yield record
-		sub_records = record.sub_rec + sub_records
-
-def get_gedcom_source(line: GedcomLine | FakeLine) -> str:
-	"""Return all the contents of the gedcom under this level 0 id (person id, family id, source id, ...)."""
-	if not line_exists(line): return ""
+	lines = list(line.sub_lines)
+	while len(lines) > 0:
+		line = lines.pop(0)
+		yield line
+		lines = line.sub_lines + lines
+
+def get_source_infos(line: TrueLine | FakeLine) -> str:
+	"""Return the gedcom text for the line and the sub-lines."""
+	if not is_true(line): return ""
 	text = str(line) + "\n"
-	for sub_rec in get_all_sub_records(line):
-		text += str(sub_rec) + "\n"
+	for sub_line in get_all_sub_lines(line):
+		text += str(sub_line) + "\n"
 	return text
 
 def format_name(name: str) -> str:
-	"""Format the payload of the gedcom tag NAME.
+	"""Format the payload of NAME lines.
 	Remove the backslash around the surname."""
 	return name.replace("/", "")
 
-def gender_to_ascii(gender: Literal['M', 'F'] | Any) -> Literal['♂', '♀', '⚥']:
+def gender_to_ascii(gender: Literal['M', 'F'] | str) -> Literal['♂', '♀', '⚥']:
 	if gender == 'M': return '♂'
 	if gender == 'F': return '♀'
 	return '⚥'
 
 def format_date(date: str) -> str:
-	"""Format the gedcom date into a shorter string.
-	Replace gedcom keywords by symbols.
+	"""Format the payload of DATE lines.
+	Return a short string representation of the date by
+	replacing keywords by symbols.
 
 	Replacements:
 	- 'd BC' standing for before christ is replaced by '-d',
 	- 'd BCE' or before common era with '-d',
 	- 'ABT d' stading for about is replaced by '~ d',
 	- 'EST d' stading for estimated is replaced by '~ d',
 	- 'CAL d' stading for calculated is replaced by '~ d',
@@ -69,25 +70,26 @@
 	elif date[:4]=='BEF ': date = '< '+date[4:]
 	elif date[:4]=='AFT ': date = '> '+date[4:]
 	elif date[:5]=='FROM ': date = date[5:]
 	elif date[:3]=='TO ': date = date[3:]
 	return date
 
 def remove_trailing_zeros(date: str) -> str:
+	"""Removes useless prefixing 0 from numbers."""
 	k = 0
 	while k+1 < len(date):
 		if date[k]=='0' and (k==0 or (k>0 and (date[k-1].isspace() or date[k-1] == '-'))):
 			date = date[:k] + date[k+1:]
 		else:
 			k += 1
 	return date
 
 def extract_year(date: str) -> str:
-	"""Return the only year of the date.
-	The parameter is the gedcom date or the formatted date string.
+	"""Format the payload of DATE lines and remove day and month information.
+	The parameter is the DATE payload or the formatted date string.
 	Keep the context of the date: '-', '~', '<', '>' and '--'."""
 	formated_date = format_date(date)
 	if ' -- ' in formated_date:
 		first_date, second_date = formated_date.split(' -- ', 1)
 		first_year = extract_year(first_date)
 		second_year = extract_year(second_date)
 		if first_year == second_year: return first_year
@@ -101,38 +103,41 @@
 	if '<' in formated_date: year = '< '+year
 	if '>' in formated_date: year = '> '+year
 	return year
 
 def extract_int_year(date: str) -> float | None:
 	"""Return the year of the date as an integer.
 	Keep the context: A date BCE returns a negative number.
-	A date range of type `between` or `from-to` returns the median number of the range."""
+	For date range of type `between` or `from-to`, this function returns
+	the median number of the range, hence the float type.
+	Return None on failure."""
 	year = extract_year(date)
 	if ' -- ' in year:
 		str_year1, str_year2 = year.split(' -- ', 1)
 		year1 = extract_int_year(str_year1)
 		year2 = extract_int_year(str_year2)
 		if year1 is None: return year2
 		elif year2 is None: return year1
 		return (year1 + year2) / 2
 	year_without_context = ''.join(filter(lambda c: c.isdecimal() or c=='-', year))
 	if year_without_context == "": return None
 	return int(year_without_context)
 
 
-def sorting_key_indi_birth(gedcom: Gedcom) -> Callable[[IndiRef | None], float]:
+def sorting_key_indi_birth(document: Document) -> Callable[[IndiRef | None], float]:
 	def get_sorting_key_indi_birth(indi: IndiRef | None) -> float:
 		if indi is None: return MINIMAL_DATE
-		birth_year = extract_int_year((gedcom[indi] > "BIRT") >= "DATE")
+		birth_year = extract_int_year((document[indi] > "BIRT") >= "DATE")
 		return MINIMAL_DATE if birth_year is None else birth_year
 	return get_sorting_key_indi_birth
 
-def sorting_key_indi_union(
-	gedcom: Gedcom, ref_indi: IndiRef
+def sorting_key_indi_union_with(
+	document: Document, ref_indi: IndiRef
 ) -> Callable[[IndiRef | None], float]:
-	def get_sorting_key_indi_union(indi: IndiRef | None) -> float:
+	family_aid = FamilyAid(document)
+	def get_sorting_key_indi_union_with(indi: IndiRef | None) -> float:
 		if indi is None: return MINIMAL_DATE
-		unions = gedcom.get_unions(ref_indi, indi)
+		unions = family_aid.get_unions_with(ref_indi, indi)
 		if len(unions) == 0: return MINIMAL_DATE
-		union_year = extract_int_year(gedcom[unions[0]] >= "DATE")
+		union_year = extract_int_year(document[unions[0]] >= "DATE")
 		return MINIMAL_DATE if union_year is None else union_year
-	return get_sorting_key_indi_union
+	return get_sorting_key_indi_union_with
```

### Comparing `fastgedcom-0.0.3/fastgedcom/parser.py` & `fastgedcom-0.0.4/fastgedcom/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import IO
 from pathlib import Path
 
-from .base import Gedcom, GedcomLine
-from .structure import XRef
-
 import ansel
+
+from .base import Document, TrueLine, XRef
+
 ansel.register()
 
 class ParsingError(Exception): pass
 
 class ParsingWarning():
 	"""Base warning class."""
 
@@ -23,74 +23,50 @@
 class DuplicateParsingWarning(ParsingWarning):
 	"""Warn about a level 0 reference that is present twice."""
 	def __init__(self, xref: XRef) -> None:
 		self.xref = xref
 	def __repr__(self) -> str:
 		return f"<{self.__class__.__qualname__} xref={self.xref}>"
 
-def parse(readable_lines: IO[str]) -> tuple[Gedcom, list[ParsingWarning]]:
-	"""Parse the text input to create the Gedcom class.
+def parse(readable_lines: IO[str]) -> tuple[Document, list[ParsingWarning]]:
+	"""Parse the text input to create the Document object.
 	
-	Return the Gedcom based on the input and the warnings about
-	input lines that can't be put into the Gedcom class.
+	Return the Document based on the input and the warnings about
+	input lines that can't be put into the Document.
 	
 	Raise ParsingError on failure."""
-	gedcom = Gedcom()
+	document = Document()
 	warnings: list[ParsingWarning] = []
 	line_number = 0
 	try:
-		parent_lines: list[GedcomLine] = []
+		parent_lines: list[TrueLine] = []
 		for line in readable_lines:
 			line_number += 1
 			line_info = line.rstrip().split(' ', 2)
 			if len(line_info) == 3:
-				parsed_line = GedcomLine(int(line_info[0]), line_info[1], line_info[2], [])
+				parsed_line = TrueLine(int(line_info[0]), line_info[1], line_info[2], [])
 			elif len(line_info) == 2:
-				parsed_line = GedcomLine(int(line_info[0]), line_info[1], "", [])
+				parsed_line = TrueLine(int(line_info[0]), line_info[1], "", [])
 			else:
 				warnings.append(LineParsingWarning(line_number, line))
 				continue
 			if parsed_line.level == 0:
 				parent_lines = [parsed_line]
-				if parsed_line.tag in gedcom.level0_index:
+				if parsed_line.tag in document.level0_index:
 					warnings.append(DuplicateParsingWarning(parsed_line.tag))
-				gedcom.level0_index[parsed_line.tag] = parsed_line
+				document.level0_index[parsed_line.tag] = parsed_line
 			else:
 				while parent_lines and parsed_line.level <= parent_lines[-1].level:
 					parent_lines.pop(-1)
 				if len(parent_lines) == 0: raise ParsingError("Inconsistent use of line levels")
-				parent_lines[-1].sub_rec.append(parsed_line)
+				parent_lines[-1].sub_lines.append(parsed_line)
 				parent_lines.append(parsed_line)
 	except ValueError as err: # raised on int parsing error
 		raise ParsingError(line_number, "Line parsing failed") from err
-	__build_parents(gedcom)
-	return (gedcom, warnings)
-
-def __build_parents(gedcom: Gedcom) -> None:
-	for fam_record in gedcom.level0_index.values():
-		if fam_record.payload != "FAM": continue
-		father = mother = None
-		children = []
-		for record in fam_record.sub_rec:
-			if record.payload is None: continue
-			if record.tag == "CHIL":
-				children.append(record.payload)
-			elif record.tag == "HUSB":
-				father = record.payload
-				if father in gedcom.unions:
-					gedcom.unions[father].append(fam_record.tag)
-				else: gedcom.unions[father] = [fam_record.tag]
-			elif record.tag == "WIFE":
-				mother = record.payload
-				if mother in gedcom.unions:
-					gedcom.unions[mother].append(fam_record.tag)
-				else: gedcom.unions[mother] = [fam_record.tag]
-		for child in children:
-			gedcom.parents[child] = (father, mother)
-
+	return (document, warnings)
 
 def guess_encoding(file: str | Path) -> str | None:
 	try:
 		with open(file, "r", encoding="utf-8-sig") as f:
 			f.read()
 	except UnicodeDecodeError: pass
 	else: return "utf-8-sig"
```

### Comparing `fastgedcom-0.0.3/setup.py` & `fastgedcom-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     requirements = f.readlines()
 
 setup(
     name="fastgedcom",
-    version="0.0.3",
+    version="0.0.4",
     description="A gedcom tool to parse, browse and modify gedcom files",
     packages=["fastgedcom"],
     package_data={"fastgedcom": ["py.typed"]},
     long_description=long_description,
     long_description_content_type="text/markdown",
     zip_safe=False,
     install_requires=requirements,
@@ -26,15 +26,15 @@
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.11",
         "Topic :: Sociology :: Genealogy",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
     ],
     keywords='fastgedcom gedcom parser genealogy',
 	project_urls={
         'Bug Reports': 'https://github.com/GatienBouyer/fastgedcom/issues',
         'Source': 'https://github.com/GatienBouyer/fastgedcom',
     },
 )
```

