# Comparing `tmp/svbench-0.6.0.tar.gz` & `tmp/svbench-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/svbench-0.6.0.tar", last modified: Thu Apr 14 10:15:44 2022, max compression
+gzip compressed data, was "svbench-0.7.0.tar", last modified: Fri May 26 13:39:58 2023, max compression
```

## Comparing `svbench-0.6.0.tar` & `svbench-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-04-14 10:15:44.000000 svbench-0.6.0/
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.6.0/svbench/.DS_Store
--rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.6.0/svbench/loaders.py
--rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.6.0/svbench/__init__.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench/models/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.6.0/svbench/models/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)    68884 2021-12-08 16:16:24.000000 svbench-0.6.0/svbench/io_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.6.0/svbench/quant_tools.py
--rw-r--r--   0 kezcleal   (501) staff       (20)      162 2022-04-14 10:15:44.000000 svbench-0.6.0/PKG-INFO
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      162 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)      312 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       50 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        8 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench.egg-info/top_level.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2022-04-14 10:15:44.000000 svbench-0.6.0/svbench.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.6.0/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      386 2022-04-14 10:11:35.000000 svbench-0.6.0/setup.py
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2022-04-14 10:15:44.000000 svbench-0.6.0/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)      404 2021-07-27 09:35:05.000000 svbench-0.6.0/README.rst
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.912095 svbench-0.7.0/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2019-06-25 15:21:27.000000 svbench-0.7.0/LICENSE.md
+-rw-r--r--   0 kezcleal   (501) staff       (20)       33 2020-04-17 10:48:39.000000 svbench-0.7.0/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-05-26 13:39:58.911707 svbench-0.7.0/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      662 2023-05-26 13:36:56.000000 svbench-0.7.0/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-05-26 13:39:58.912196 svbench-0.7.0/setup.cfg
+-rw-r--r--   0 kezcleal   (501) staff       (20)      487 2023-05-26 11:53:14.000000 svbench-0.7.0/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.898792 svbench-0.7.0/svbench/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-04-06 14:34:09.000000 svbench-0.7.0/svbench/.DS_Store
+-rw-r--r--   0 kezcleal   (501) staff       (20)       94 2021-04-30 10:31:14.000000 svbench-0.7.0/svbench/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1158 2023-05-26 13:39:20.000000 svbench-0.7.0/svbench/cli.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)    69040 2023-05-26 12:20:45.000000 svbench-0.7.0/svbench/io_tools.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2320 2021-04-30 10:40:25.000000 svbench-0.7.0/svbench/loaders.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.911378 svbench-0.7.0/svbench/models/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2020-04-17 10:48:39.000000 svbench-0.7.0/svbench/models/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8106 2021-12-02 16:05:54.000000 svbench-0.7.0/svbench/quant_tools.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-26 13:39:58.910923 svbench-0.7.0/svbench.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      112 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)      372 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       45 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/entry_points.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       50 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/requires.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        8 2023-05-26 13:39:58.000000 svbench-0.7.0/svbench.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `svbench-0.6.0/svbench/.DS_Store` & `svbench-0.7.0/svbench/.DS_Store`

 * *Files identical despite different names*

### Comparing `svbench-0.6.0/svbench/loaders.py` & `svbench-0.7.0/svbench/loaders.py`

 * *Files identical despite different names*

### Comparing `svbench-0.6.0/svbench/io_tools.py` & `svbench-0.7.0/svbench/io_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -898,33 +898,30 @@
                     if allowed_svtypes is not None and svtype not in allowed_svtypes:
                         continue
 
             if keep is not None and not check_passed(operations, r, keep):
                 continue
 
             svlen = -1
+            if r.ID.endswith("_2"):  # Skip second part of BND, or multirow record
+                continue
             if svtype == "BND":
-                if "_2" in r.ID:  # Skip second part of BND record
-                    continue
                 if r.ALT[0] is None:
                     continue
                 try:
                     chrom2 = r.ALT[0].chr
                     end = r.ALT[0].pos
                 except AttributeError:
                     print("Error parsing", r, file=stderr)
                     continue
                 if end is None:
                     end = start + 1
                 else:
                     end = int(r.ALT[0].pos)
 
-
-
-
             else:
                 chrom2 = chrom
                 if "CHR2" in r.INFO:
                     chrom2 = r.INFO["CHR2"]
                     if chrom2[0] != "c":
                         chrom2 = "chr" + chrom2
 
@@ -1023,31 +1020,33 @@
 
             if other_cols:
                 parsed = parse_cols_list(r, other_cols, {})
                 if not new_cols:
                     new_cols = list(parsed.keys())
                 d.update(parsed)
 
-            if load_genotype:
-                samps = r.__getattribute__("samples")
-                if len(samps) > 1:
-                    raise ValueError("Cannot parse genotype for multi-sample vcf, set load_genotype=False")
+            samps = r.__getattribute__("samples")
+            if load_genotype and len(samps) == 1:
+                # if len(samps) > 1:
+                    # raise ValueError("Cannot parse genotype for multi-sample vcf, set load_genotype=False")
                 done = False
                 try:
                     d["GT"] = str(samps[0]["GT"])
                     done = True
                 except IndexError:
                     pass
 
                 if not done:
-                    try:
-                        d["GT"] = r.INFO["GT"]
-                    except KeyError:
-                        pass
+                    # try:
+                    #     d["GT"] = r.INFO["GT"]
+                    # except KeyError:
+                    #     pass
                     d["GT"] = "NA"
+            else:
+                d["GT"] = "NA"
 
             res.append(d)
 
         if len(res) == 0:
             print(f"Warning: empty vcf {path}", file=stderr)
             return self
 
@@ -1063,15 +1062,15 @@
                     if ecs[0] == k or (ecs[0], ecs[1]) == k:
                         df[ec] = v.norm(df[ec], self.kwargs)
 
         # Order df
         base_cols = ["chrom", "start", "chrom2", "end", "svtype", "w", "strata", "id", "size_filter_pass", "svlen", "filter"]
         if load_genotype:
             base_cols.append("GT")
-            df["GT"] = df["GT"].str.replace("|", "/")
+            df["GT"] = [i.replace("|", "/") if isinstance(i, str) else i for i in df["GT"]] #df["GT"].str.replace("|", "/")
         df = df[[i for i in base_cols if i in df.columns] + new_cols]
 
         self.breaks_df = df
         self.extra_cols = new_cols
 
         if stratify is not None:
             self.stratify_range = stratify.bins
```

### Comparing `svbench-0.6.0/svbench/quant_tools.py` & `svbench-0.7.0/svbench/quant_tools.py`

 * *Files identical despite different names*

