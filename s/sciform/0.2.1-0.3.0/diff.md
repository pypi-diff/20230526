# Comparing `tmp/sciform-0.2.1.tar.gz` & `tmp/sciform-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciform-0.2.1.tar", last modified: Fri May 26 14:44:32 2023, max compression
+gzip compressed data, was "sciform-0.3.0.tar", last modified: Fri May 26 19:04:49 2023, max compression
```

## Comparing `sciform-0.2.1.tar` & `sciform-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.505710 sciform-0.2.1/
--rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      376 2023-05-26 14:44:32.504451 sciform-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-26 03:37:34.000000 sciform-0.2.1/README.md
--rw-rw-rw-   0        0        0      557 2023-05-26 14:41:29.000000 sciform-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 14:44:32.505710 sciform-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.471731 sciform-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.484733 sciform-0.2.1/src/sciform/
--rw-rw-rw-   0        0        0       84 2023-05-26 14:43:39.000000 sciform-0.2.1/src/sciform/__init__.py
--rw-rw-rw-   0        0        0     6268 2023-05-26 02:13:00.000000 sciform-0.2.1/src/sciform/format.py
--rw-rw-rw-   0        0        0     6178 2023-05-26 01:43:12.000000 sciform-0.2.1/src/sciform/format_utils.py
--rw-rw-rw-   0        0        0     2185 2023-05-26 01:33:01.000000 sciform-0.2.1/src/sciform/grouping.py
--rw-rw-rw-   0        0        0     2388 2023-05-25 23:32:37.000000 sciform-0.2.1/src/sciform/modes.py
--rw-rw-rw-   0        0        0     1772 2023-05-25 23:32:37.000000 sciform-0.2.1/src/sciform/prefix.py
--rw-rw-rw-   0        0        0     2509 2023-05-26 13:43:50.000000 sciform-0.2.1/src/sciform/sfloat.py
--rw-rw-rw-   0        0        0     3535 2023-05-26 03:59:52.000000 sciform-0.2.1/src/sciform/unc_format.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.503449 sciform-0.2.1/src/sciform.egg-info/
--rw-rw-rw-   0        0        0      376 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 14:44:32.000000 sciform-0.2.1/src/sciform.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 14:44:32.504451 sciform-0.2.1/tests/
--rw-rw-rw-   0        0        0     4440 2023-05-26 13:54:12.000000 sciform-0.2.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:04:49.510221 sciform-0.3.0/
+-rw-rw-rw-   0        0        0     1074 2023-05-26 03:30:56.000000 sciform-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      720 2023-05-26 19:04:49.510221 sciform-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-05-26 18:03:16.000000 sciform-0.3.0/README.md
+-rw-rw-rw-   0        0        0      557 2023-05-26 14:41:29.000000 sciform-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 19:04:49.510221 sciform-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 19:04:49.470383 sciform-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 19:04:49.498584 sciform-0.3.0/src/sciform/
+-rw-rw-rw-   0        0        0       84 2023-05-26 19:03:13.000000 sciform-0.3.0/src/sciform/__init__.py
+-rw-rw-rw-   0        0        0      101 2023-05-26 18:11:20.000000 sciform-0.3.0/src/sciform/defaults.py
+-rw-rw-rw-   0        0        0     6698 2023-05-26 18:49:19.000000 sciform-0.3.0/src/sciform/format.py
+-rw-rw-rw-   0        0        0     6178 2023-05-26 01:43:12.000000 sciform-0.3.0/src/sciform/format_utils.py
+-rw-rw-rw-   0        0        0     2373 2023-05-26 18:40:38.000000 sciform-0.3.0/src/sciform/grouping.py
+-rw-rw-rw-   0        0        0     3460 2023-05-26 18:45:16.000000 sciform-0.3.0/src/sciform/modes.py
+-rw-rw-rw-   0        0        0     1772 2023-05-25 23:32:37.000000 sciform-0.3.0/src/sciform/prefix.py
+-rw-rw-rw-   0        0        0     2509 2023-05-26 13:43:50.000000 sciform-0.3.0/src/sciform/sfloat.py
+-rw-rw-rw-   0        0        0     3535 2023-05-26 03:59:52.000000 sciform-0.3.0/src/sciform/unc_format.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:04:49.509217 sciform-0.3.0/src/sciform.egg-info/
+-rw-rw-rw-   0        0        0      720 2023-05-26 19:04:49.000000 sciform-0.3.0/src/sciform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-26 19:04:49.000000 sciform-0.3.0/src/sciform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 19:04:49.000000 sciform-0.3.0/src/sciform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-26 19:04:49.000000 sciform-0.3.0/src/sciform.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 19:04:49.509217 sciform-0.3.0/tests/
+-rw-rw-rw-   0        0        0    15227 2023-05-26 19:01:46.000000 sciform-0.3.0/tests/test.py
```

### Comparing `sciform-0.2.1/LICENSE` & `sciform-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sciform-0.2.1/pyproject.toml` & `sciform-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sciform-0.2.1/src/sciform/format.py` & `sciform-0.3.0/src/sciform/format.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 from typing import Optional
 from dataclasses import dataclass
 import re
 from math import isfinite
 import logging
 
-from sciform.modes import FormatMode, PrecMode, SignMode, GroupingMode
+from sciform.modes import (FormatMode, PrecMode, SignMode, GroupingSeparator,
+                           DecimalSeparator)
 from sciform.format_utils import (get_mantissa_exp, get_exp_str,
                                   get_top_and_bottom_digit,
                                   get_round_digit,
                                   format_float_by_top_bottom_dig)
-from sciform.grouping import add_group_chars_float
+from sciform.grouping import add_separators
 from sciform.prefix import replace_prefix
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class FormatSpec:
     fill_char: str = ''
     sign_mode: SignMode = SignMode.NEGATIVE
-    force_zero_positive: bool = True
     alternate_mode: bool = False
     width: int = 0
-    grouping_option_1: GroupingMode = GroupingMode.NO_GROUPING
-    grouping_option_2: GroupingMode = GroupingMode.NO_GROUPING
+    thousands_separator: GroupingSeparator = GroupingSeparator.NO_GROUPING
+    decimal_separator: DecimalSeparator = DecimalSeparator.POINT
+    thousandths_separator: GroupingSeparator = GroupingSeparator.NO_GROUPING
     prec_mode: PrecMode = PrecMode.SIG_FIG
     precision: Optional[int] = None
     format_mode: FormatMode = FormatMode.FIXEDPOINT
     capital_exp_char: bool = False
     percent_mode: bool = False
     exp: Optional[int] = None
     prefix_mode: bool = False
 
 
 pattern = re.compile(r'''^
                          (?:(?P<fill>[ 0])=)?
                          (?P<sign>[+\- ])?
-                         (?P<pos_zero>z)?  
                          (?P<alternate>\#)?                         
                          (?P<width>\d+)?
-                         (?P<grouping_option_1>[_,v])?                     
-                         (?P<grouping_option_2>[_,v])?                     
+                         (?P<thousands_separator>[n,.s_])?                     
+                         (?P<decimal_separator>[.,])?            
+                         (?P<thousandths_separator>[ns_])?                  
                          (?:(?P<prec_mode>[.!])(?P<prec>-?\d+))?
                          (?P<format_mode>[fF%eErRbB])?
                          (?P<exp>[+-]\d+)?
                          (?P<prefix_mode>p)?
                          $''', re.VERBOSE)
 
 
@@ -56,26 +57,28 @@
         raise ValueError(f'Invalid format specifier: \'{fmt}\'')
 
     fill = match.group('fill') or ' '
 
     sign_flag = match.group('sign') or '-'
     sign_mode = SignMode.from_flag(sign_flag)
 
-    force_pos_zero = match.group('pos_zero') is not None
-
     alternate_mode = match.group('alternate') is not None
 
     width = match.group('width') or 0
     width = int(width)
 
-    grouping_option_flag_1 = match.group('grouping_option_1') or ''
-    grouping_option_1 = GroupingMode.from_flag(grouping_option_flag_1)
+    thousands_separator_flag = match.group('thousands_separator') or 'n'
+    thousands_seperator = GroupingSeparator.from_flag(thousands_separator_flag)
+
+    decimal_separator_flag = match.group('decimal_separator') or '.'
+    decimal_separator = DecimalSeparator.from_flag(decimal_separator_flag)
 
-    grouping_option_flag_2 = match.group('grouping_option_2') or ''
-    grouping_option_2 = GroupingMode.from_flag(grouping_option_flag_2)
+    thousandths_separator_flag = match.group('thousandths_separator') or 'n'
+    thousandths_seperator = GroupingSeparator.from_flag(
+        thousandths_separator_flag)
 
     prec_mode_flag = match.group('prec_mode') or '.'
     prec_mode = PrecMode.from_flag(prec_mode_flag)
 
     prec = match.group('prec')
     if prec:
         prec = int(prec)
@@ -93,19 +96,19 @@
     if exp is not None:
         exp = int(exp)
 
     prefix_mode = match.group('prefix_mode') is not None
 
     format_spec = FormatSpec(fill_char=fill,
                              sign_mode=sign_mode,
-                             force_zero_positive=force_pos_zero,
                              alternate_mode=alternate_mode,
                              width=width,
-                             grouping_option_1=grouping_option_1,
-                             grouping_option_2=grouping_option_2,
+                             thousands_separator=thousands_seperator,
+                             decimal_separator=decimal_separator,
+                             thousandths_separator=thousandths_seperator,
                              prec_mode=prec_mode,
                              precision=prec,
                              format_mode=format_mode,
                              capital_exp_char=capital_exp_char,
                              percent_mode=percent_mode,
                              exp=exp,
                              prefix_mode=prefix_mode)
@@ -134,29 +137,33 @@
             raise ValueError('Invalid format specifier')  # TODO better message
         num *= 100
 
     exp = format_spec.exp
     mantissa, exp = get_mantissa_exp(num, format_mode, exp, alternate_mode)
     exp_str = get_exp_str(exp, format_mode, capital_exp_char)
 
-    if format_spec.force_zero_positive:
-        if mantissa == -0.0:
-            mantissa = abs(mantissa)
+    if mantissa == -0.0:
+        mantissa = abs(mantissa)
 
     top_digit, bottom_digit = get_top_and_bottom_digit(mantissa)
     round_digit = get_round_digit(top_digit, bottom_digit,
                                   prec, prec_mode)
     mantissa_str = format_float_by_top_bottom_dig(mantissa, top_padded_digit,
                                                   round_digit, sign_mode,
                                                   fill_char)
-    grouping_char_1 = GroupingMode.to_char(format_spec.grouping_option_1)
-    grouping_char_2 = GroupingMode.to_char(format_spec.grouping_option_2)
-    mantissa_str = add_group_chars_float(mantissa_str, grouping_char_1,
-                                         grouping_char_2,
-                                         group_size=3)
+    thousands_separator = GroupingSeparator.to_char(
+        format_spec.thousands_separator)
+    decimal_separator = DecimalSeparator.to_char(format_spec.decimal_separator)
+    thousandths_separator = GroupingSeparator.to_char(
+        format_spec.thousandths_separator)
+    mantissa_str = add_separators(mantissa_str,
+                                  thousands_separator,
+                                  decimal_separator,
+                                  thousandths_separator,
+                                  group_size=3)
 
     full_str = f'{mantissa_str}{exp_str}'
 
     if format_spec.prefix_mode:
         full_str = replace_prefix(full_str)
 
     if format_spec.percent_mode:
```

### Comparing `sciform-0.2.1/src/sciform/format_utils.py` & `sciform-0.3.0/src/sciform/format_utils.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.1/src/sciform/grouping.py` & `sciform-0.3.0/src/sciform/grouping.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 
 class GroupingDirection(Enum):
     FORWARD = 'forward'
     BACKWARD = 'backward'
 
 
-def add_group_chars(string, group_char='_',
-                    direction=GroupingDirection.FORWARD, group_size=3):
+def add_group_chars_between_numbers(string, group_char='_',
+                                    direction=GroupingDirection.FORWARD,
+                                    group_size=3):
     num_chars = len(string)
     result_str = ''
 
     group_counter = 0
     char_counter = 0
 
     if direction is GroupingDirection.FORWARD:
@@ -36,29 +37,34 @@
                 group_counter = 0
     else:
         raise ValueError(f'Invalid grouping direction: {direction}')
 
     return result_str
 
 
-def add_group_chars_float(float_string, pre_group_char='_',
-                          post_group_char='_', group_size=3):
+def add_separators(float_string,
+                   thousands_separator='',
+                   decimal_separator='.',
+                   thousandths_separator='',
+                   group_size=3):
     dec_split = float_string.split('.')
-    pre_string = dec_split[0]
+    thousands_string = dec_split[0]
     if len(dec_split) == 1:
-        post_string = ''
+        thousandths_string = ''
     elif len(dec_split) == 2:
-        pre_string, post_string = dec_split
+        thousandths_string = dec_split[1]
     else:
         raise ValueError
 
-    pre_grouped_string = add_group_chars(pre_string, pre_group_char,
-                                         GroupingDirection.BACKWARD,
-                                         group_size)
-    post_grouped_string = add_group_chars(post_string, post_group_char,
-                                          GroupingDirection.FORWARD,
-                                          group_size)
-    if len(post_grouped_string) > 0:
-        grouped_str = pre_grouped_string + '.' + post_grouped_string
+    thousands_grouped_string = add_group_chars_between_numbers(
+        thousands_string, thousands_separator, GroupingDirection.BACKWARD,
+        group_size)
+    thousandths_grouped_string = add_group_chars_between_numbers(
+        thousandths_string, thousandths_separator, GroupingDirection.FORWARD,
+        group_size)
+    if len(thousandths_string) > 0:
+        grouped_str = (f'{thousands_grouped_string}'
+                       f'{decimal_separator}'
+                       f'{thousandths_grouped_string}')
     else:
-        grouped_str = pre_grouped_string
+        grouped_str = thousands_grouped_string
     return grouped_str
```

### Comparing `sciform-0.2.1/src/sciform/prefix.py` & `sciform-0.3.0/src/sciform/prefix.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.1/src/sciform/sfloat.py` & `sciform-0.3.0/src/sciform/sfloat.py`

 * *Files identical despite different names*

### Comparing `sciform-0.2.1/src/sciform/unc_format.py` & `sciform-0.3.0/src/sciform/unc_format.py`

 * *Files identical despite different names*

