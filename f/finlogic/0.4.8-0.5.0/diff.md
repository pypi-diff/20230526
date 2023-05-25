# Comparing `tmp/finlogic-0.4.8.tar.gz` & `tmp/finlogic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.8.tar", last modified: Mon May 22 22:51:30 2023, max compression
+gzip compressed data, was "finlogic-0.5.0.tar", last modified: Thu May 25 23:14:58 2023, max compression
```

## Comparing `finlogic-0.4.8.tar` & `finlogic-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.8/LICENSE
--rw-r--r--   0        0        0     9216 2023-05-22 22:49:10.801399 finlogic-0.4.8/README.md
--rw-r--r--   0        0        0      423 2023-05-22 22:42:54.448718 finlogic-0.4.8/finlogic/__init__.py
--rw-r--r--   0        0        0    23696 2023-05-22 22:42:54.448718 finlogic-0.4.8/finlogic/company.py
--rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.8/finlogic/config.py
--rw-r--r--   0        0        0    11931 2023-05-22 22:43:42.677190 finlogic-0.4.8/finlogic/cvm.py
--rw-r--r--   0        0        0     4637 2023-05-22 11:25:57.286389 finlogic-0.4.8/finlogic/database.py
--rw-r--r--   0        0        0     3044 2023-05-22 22:42:54.448718 finlogic-0.4.8/finlogic/fduckdb.py
--rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.8/finlogic/fprint.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.8/finlogic/language.py
--rw-r--r--   0        0        0     1039 2023-05-22 22:51:30.874768 finlogic-0.4.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.8/tests/__init__.py
--rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.8/tests/test_company.py
--rw-r--r--   0        0        0      900 2023-05-22 22:42:54.448718 finlogic-0.4.8/tests/test_database.py
--rw-r--r--   0        0        0    11325 1970-01-01 00:00:00.000000 finlogic-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.5.0/LICENSE
+-rw-r--r--   0        0        0     9178 2023-05-25 21:55:04.282408 finlogic-0.5.0/README.md
+-rw-r--r--   0        0        0      391 2023-05-24 09:12:22.015110 finlogic-0.5.0/finlogic/__init__.py
+-rw-r--r--   0        0        0    23644 2023-05-25 22:49:23.698153 finlogic-0.5.0/finlogic/company.py
+-rw-r--r--   0        0        0      159 2023-05-25 10:59:30.819065 finlogic-0.5.0/finlogic/config.py
+-rw-r--r--   0        0        0    13151 2023-05-25 21:45:27.482813 finlogic-0.5.0/finlogic/cvm.py
+-rw-r--r--   0        0        0     5406 2023-05-25 23:03:39.330450 finlogic-0.5.0/finlogic/data_manager.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.5.0/finlogic/language.py
+-rw-r--r--   0        0        0     1017 2023-05-25 23:14:58.671033 finlogic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3354 2023-05-23 23:02:21.956066 finlogic-0.5.0/tests/test_company.py
+-rw-r--r--   0        0        0      907 2023-05-25 23:05:44.826667 finlogic-0.5.0/tests/test_data.py
+-rw-r--r--   0        0        0    11257 1970-01-01 00:00:00.000000 finlogic-0.5.0/PKG-INFO
```

### Comparing `finlogic-0.4.8/LICENSE` & `finlogic-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.8/README.md` & `finlogic-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 <!-- [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)" -->
 
 ## FinLogic: finance toolkit for listed Brazilian companies.
 
 ---
 
-**FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). FinLogic uses DuckDB as an OLAP database management system and Pandas to process the data to and from the locally builted accounting database (aprox. 8 million rows).
+**FinLogic** offers a Pythonic way to analyze the financial data of companies listed in Brazil, using information made publicly available by the local securities market authority, CVM. FinLogic processes approximately 20 million accounting entries using Pandas, and constructs a local DataFrame for ultra-fast access to this information.
 
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
@@ -24,40 +24,39 @@
 # PyPI:
 pip install finlogic
 ```
 
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
-- [DuckDB](https://github.com/pydata/pandas) \>= 0.8.0
 - [Pandas](https://github.com/pydata/pandas) \>= 1.5.0
 - [Requests](http://docs.python-requests.org/en/master/) \>= 2.30.0
-- [Rich](https://github.com/Textualize/rich) \>= 13.0.0
+- [tqdm](https://github.com/tqdm/tqdm) \>= 4.1.0
 - [Zstandard](https://python-zstandard.readthedocs.io/en/latest/) \>= 0.21.0
 
 ---
 
 ## Quick Start
 
 ### Create FinLogic Database
 
-The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 8 millions rows of accounting values and loading it into FinLogic Database for local data analysis. In the firt run, the process can take more than 1 minute depending on CVM Server connection and local CPU power. For subsequent updates, only updated CVM files will be processed, which will be faster.
+The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take longer than 1 minute, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
 
 ```python
 >>> import finlogic as fl
 
 # Compile FinLogic database for the first time:
->>> fl.update_database()
+>>> fl.update()
 
 Updating CVM raw files...
 ...
 FinLogic database updated ✅
 
 # Show database info:
->>> fl.database_info()
+>>> fl.info()
 ```
 
 | FinLogic Database Info |                         Value |
 | :--------------------- | ----------------------------: |
 | db_path                | .../finlogic/data/finlogic.db |
 | db_size                |                       76.0 MB |
 | db_last_modified       |           2023-04-20 07:29:08 |
@@ -86,18 +85,18 @@
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
->>> petro = fl.Company(9512, acc_method='sep', acc_unit='m')
+>>> petro = fl.Company(9512, is_consolidated='sep', acc_unit='m')
 
 # Change company accounting method back to consolidated (default):
->>> petro.acc_method = 'con'
+>>> petro.is_consolidated = 'con'
 
 # Change company accounting unit to billion (default is 1):
 >>> petro.acc_unit = 'b'
 
 # Show company info:
 >>> petro.info()
 ```
```

### Comparing `finlogic-0.4.8/finlogic/company.py` & `finlogic-0.5.0/finlogic/company.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 financial reports and calculating financial indicators for a company. Users can
 set the accounting method, unit, tax rate, and language for the company object.
 
 Classes:
     Company: Represents a company with its financial information and allows
     users to generate financial reports and indicators.
 
-Abreviations used in code:
-    dfc = company dataframe
-    dfi = input dataframe
-    dfo = output dataframe
+Main variables:
+    cfg.DF  memory dataframe with all accounting data
+    _df     company dataframe (protected)
+    dfi     function input dataframe
+    dfo     function output dataframe
 
 RuntimeWarning:
     Pandas query + numexpr module -> Engine has switched to 'python' because
     numexpr does not support extension array dtypes (category not supported
     yet). Please set your engine to python manually. That means that the query
     method has to use engine='python' to work with category dtype. N.B. Only
     FinLogic Dataframe uses category dtype for efficiency.
 
 """
 from typing import Literal
 import numpy as np
 import pandas as pd
 from .language import language_df
-from .fprint import print_dict
-from .fduckdb import execute
+from . import data_manager as dm
 
 
 class Company:
     """A class to represent a company financial data.
 
      This class provides methods to create financial reports and to calculate
      financial indicators based on a company's accounting data. The class also
      has an AI generated dictionary to translate from Portuguese to English.
 
     Attributes:
          identifier: A unique identifier for the company. Both CVM ID (int) and
             Fiscal ID (str) can be used.
-         acc_method: The accounting methods can be either 'con' for consolidated or
+         is_consolidated: The accounting methods can be either 'con' for consolidated or
             'sep' for separate. Defaults to 'con' (str).
          acc_unit: The accounting unit for the financial statements where "t"
             represents thousands, "m" represents millions and "b" represents
             billions (int, float or str). Defaults to 1.
          tax_rate: The tax rate for the company. Defaults to 0.34, which is
             the standard corporate tax rate in Brazil (float).
          language: The language for the financial reports. Options are "english"
@@ -55,28 +55,28 @@
      Raises:
          ValueError: If the input arguments are invalid.
     """
 
     def __init__(
         self,
         identifier: int | str,
-        acc_method: Literal["con", "sep"] = "con",
+        is_consolidated: bool = True,
         acc_unit: int | float | Literal["t", "m", "b"] = 1,
         tax_rate: float = 0.34,
         language: Literal["english", "portuguese"] = "english",
     ):
         """Initializes a new instance of the Company class."""
         self._initialized = False
         self.identifier = identifier
-        self.acc_method = acc_method
+        self.is_consolidated = is_consolidated
         self.acc_unit = acc_unit
         self.tax_rate = tax_rate
         self.language = language
         self._initialized = True
-        # Only set company dataframe after identifier, acc_method and acc_unit are set
+        # Only set _df after identifier, is_consolidated and acc_unit are setted
         self._set_df()
 
     @property
     def identifier(self) -> int | str:
         """Set a unique identifier to select the company in FinLogic Database.
 
         This method sets the company's CVM and fiscal ID based on a given
@@ -97,56 +97,51 @@
             KeyError: If the given identifier isn't found in Finlogic Database.
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier: int | str):
         # Create custom data frame for ID selection
-        query = f"""
-            SELECT DISTINCT cvm_id, tax_id, name_id
-              FROM reports
-             WHERE CAST(cvm_id AS VARCHAR) = '{identifier}'
-                OR tax_id = '{identifier}'
-        """
-        df = execute(query, "df")
+        df = (
+            dm.get_main_df()[["cvm_id", "tax_id", "name_id"]]
+            .query("cvm_id == @identifier or tax_id == @identifier")
+            .drop_duplicates(ignore_index=True)
+        )
         if not df.empty:
             self._cvm_id = df.loc[0, "cvm_id"]
             self.tax_id = df.loc[0, "tax_id"]
             self.name_id = df.loc[0, "name_id"]
             self._identifier = identifier
         else:
             raise KeyError(f"Company 'identifier' {identifier} not found.")
         # If object was already initialized, reset company dataframe
         if self._initialized:
             self._set_df()
 
     @property
-    def acc_method(self) -> Literal["con", "sep"]:
+    def is_consolidated(self) -> bool:
         """Gets or sets the accounting method for registering investments in
         subsidiaries.
 
-        The "acc_method" must be "con" for consolidated or "sep" for separate.
+        The "is_consolidated" must be True for consolidated or False for separate.
         Consolidated accounting combines the financial statements of a parent
         company and its subsidiaries, while separate accounting keeps them
         separate. Defaults to 'consolidated'.
 
         Raises:
             ValueError: If the accounting method is invalid.
         """
         return self._acc_unit
 
-    @acc_method.setter
-    def acc_method(self, value: Literal["con", "sep"]):
-        # Set accounting method to upper case as in FinLogic Database
-        if value == "con":
-            self._acc_method = "CONSOLIDATED"
-        elif value == "sep":
-            self._acc_method = "SEPARATE"
+    @is_consolidated.setter
+    def is_consolidated(self, value: bool):
+        if type(value) is bool:
+            self._is_consolidated = value
         else:
-            raise ValueError("acc_method expects 'consolidated' or 'separate'")
+            raise ValueError("Company 'is_consolidated' value is invalid")
         # If object was already initialized, reset company dataframe
         if self._initialized:
             self._set_df()
 
     @property
     def acc_unit(self) -> float:
         """Gets or sets the accounting unit for the financial statements.
@@ -253,95 +248,100 @@
 
     def _set_df(self) -> pd.DataFrame:
         """Sets the company data frame.
 
         This method creates a dataframe with the company's financial
         statements.
         """
-        query = f"""
-            SELECT *
-              FROM reports
-             WHERE cvm_id = {self._cvm_id}
-               AND acc_method = '{self._acc_method}'
-             ORDER BY 
-                acc_code,
-                period_reference,
-                report_type,
-                period_begin,
-                period_end
-        """
-        df = execute(query, "df")
+        df = (
+            dm.get_main_df()
+            .query(
+                "cvm_id == @self._cvm_id and \
+                 is_consolidated == @self._is_consolidated"
+            )
+            .reset_index(drop=True)
+        )
 
         # Convert category columns back to string
         columns = df.columns
         cat_cols = [c for c in columns if df[c].dtype == "category"]
         df[cat_cols] = df[cat_cols].astype("string")
 
-        # Change acc_unit only for accounts different from 3.99
+        # Change acc_value only when it is not earnings_per_share (acc_code 8)
         df["acc_value"] = np.where(
-            df["acc_code"].str.startswith("3.99"),
+            df["acc_code"].str.startswith("8"),
             df["acc_value"],
             df["acc_value"] / self._acc_unit,
         )
-        annual_df = df.query('report_type == "ANNUAL"')
-        self._first_annual = annual_df["period_end"].min()
-        self._last_annual = annual_df["period_end"].max()
-        quarterly_df = df.query('report_type == "QUARTERLY"')
-        self._last_quarterly = quarterly_df["period_end"].max()
+
+        self._first_period = df["period_end"].min()
         self._last_period = df["period_end"].max()
 
+        # Not necessarily there will be a quarterly report for the last period
+        self._last_annual = df.query("is_annual")["period_end"].max()
+
+        if self._last_period == self._last_annual:
+            self._last_period_type = "annual"
+            self._last_quarterly = None
+        else:
+            self._last_period_type = "quarterly"
+            self._last_quarterly = df.query("not is_annual")["period_end"].max()
+
         # Drop columns that are already company attributes or will not be used
-        df.drop(columns=["name_id", "cvm_id", "tax_id", "acc_method"], inplace=True)
+        df.drop(
+            columns=["name_id", "cvm_id", "tax_id", "is_consolidated"],
+            inplace=True,
+        )
 
         # Set company data frame
         self._df = df
 
-    def info(self) -> dict:
+    def info(self) -> pd.DataFrame:
         """Print a concise summary of a company."""
-        # Some companies have no quarterly reports (see cvm_id 9784)
-        if self._last_quarterly is pd.NaT:
-            last_quarterly = "No quarterly reports"
-        else:
-            last_quarterly = self._last_quarterly.strftime("%Y-%m-%d")
-
         company_info = {
             "Name": self.name_id,
             "CVM ID": self._cvm_id,
             "Fiscal ID (CNPJ)": self.tax_id,
             "Total Accounting Rows": len(self._df.index),
-            "Selected Accounting Method": self._acc_method,
+            "Selected Accounting Method": "consolidated"
+            if self._is_consolidated
+            else "separate",
             "Selected Accounting Unit": self._acc_unit,
             "Selected Tax Rate": self._tax_rate,
-            "First Annual Report": self._first_annual.strftime("%Y-%m-%d"),
-            "Last Annual Report": self._last_annual.strftime("%Y-%m-%d"),
-            "Last Quarterly Report": last_quarterly,
+            "First Report": self._first_period.strftime("%Y-%m-%d"),
+            "Last Report": self._last_period.strftime("%Y-%m-%d"),
+            "Last Report Type": self._last_period_type,
         }
-        print_dict(info_dict=company_info, table_name="Company Info")
+        s = pd.Series(company_info)
+        s.name = "Company Info"
+        return s.to_frame()
 
     def _build_report_index(self, dfi: pd.DataFrame) -> pd.DataFrame:
-        """Build the index for the report."""
-        # "acc_code" works as a primary key. Other columns set the preference order
+        """Build the index for the report. This function is used by the
+        _build_report function. The index is built from the annual reports
+        "acc_code" works as a primary key. Other columns set the preference order
+        """
         df = (
-            dfi[["acc_code", "acc_name", "period_reference"]]
-            .sort_values(by=["acc_code", "period_reference"])
+            dfi[["acc_code", "acc_name", "period_end"]]
+            .sort_values(by=["acc_code", "period_end"])
             .drop_duplicates(subset=["acc_code"], keep="last", ignore_index=True)[
                 ["acc_code", "acc_name"]
             ]
         )
         return df
 
     def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
         # Start "dfo" with the index
         dfo = self._build_report_index(dfi)
         year_cols = ["acc_code", "acc_value"]
         periods = sorted(dfi["period_end"].drop_duplicates())
         for period in periods:
             df_year = dfi.query("period_end == @period")[year_cols].copy()
             period_str = period.strftime("%Y-%m-%d")
-            if period == self._last_quarterly:
+            if period == self._last_period and self._last_period_type == "quarterly":
                 period_str += " (ttm)"
             df_year.rename(columns={"acc_value": period_str}, inplace=True)
             dfo = pd.merge(dfo, df_year, how="left", on=["acc_code"])
         dfo.fillna(0, inplace=True)
         return dfo.sort_values("acc_code", ignore_index=True)
 
     def report(
@@ -387,21 +387,16 @@
             pd.DataFrame: Generated financial report as a pandas DataFrame.
 
         Raises:
             ValueError: If some argument is invalid.
         """
         # Copy company dataframe to avoid changing it
         df = self._df.copy()
-        periods = sorted(df["period_end"].drop_duplicates())
-        if num_years > len(periods):
-            num_years = len(periods)
-        periods = periods[-num_years:]
-        df.query("period_end in @periods", inplace=True)
         # Check input arguments.
-        if acc_level not in {0, 1, 2, 3, 4}:
+        if acc_level not in [0, 1, 2, 3, 4]:
             raise ValueError("acc_level expects 0, 1, 2, 3 or 4")
 
         # Filter dataframe for selected acc_level
         # Example of an acc_code: "7.08.04.04" -> 4 levels and 3 dots
         if acc_level:
             df.query(rf"acc_code.str.count('\.') <= {acc_level - 1}", inplace=True)
 
@@ -425,69 +420,82 @@
             1 -> Balance Sheet - Assets
             2 -> Balance Sheet - Liabilities and Shareholders’ Equity
             3 -> Income
             4 -> Comprehensive Income
             5 -> Changes in Equity
             6 -> Cash Flow (Indirect Method)
             7 -> Added Value
+            8 -> Earnings per Share
         """
         report_types = {
             "balance_sheet": ("1", "2"),
             "income_statement": ("3"),
             "cash_flow": ("6"),
-            "earnings_per_share": ("3.99"),
-            "comprehensive_income": ("4"),
-            "added_value": ("7"),
             "assets": ("1"),
             "cash": ("1.01.01", "1.01.02"),
             "current_assets": ("1.01"),
             "non_current_assets": ("1.02"),
             "liabilities": ("2.01", "2.02"),
             "debt": ("2.01.04", "2.02.01"),
             "current_liabilities": ("2.01"),
             "non_current_liabilities": ("2.02"),
             "liabilities_and_equity": ("2"),
             "equity": ("2.03"),
+            "comprehensive_income": ("4"),
+            "added_value": ("7"),
+            "earnings_per_share": ("8"),
         }
         acc_codes = report_types[report_type]  # noqa
         df.query("acc_code.str.startswith(@acc_codes)", inplace=True)
         df.reset_index(drop=True, inplace=True)
 
-        if report_type in {"income_statement", "cash_flow"}:
-            # remove earnings per share from income statment
-            df = df[~df["acc_code"].str.startswith("3.99")]
+        if (
+            report_type in ["income_statement", "cash_flow"]
+            and self._last_period_type == "quarterly"
+        ):
             df = self._calculate_ttm(df)
 
+        # Show only selected years
+        all_periods = sorted(df["period_end"].drop_duplicates())
+        selected_periods = all_periods[-num_years:]  # noqa
+        df.query("period_end in @selected_periods", inplace=True)
+
         return self._build_report(df)
 
     def _calculate_ttm(self, dfi: pd.DataFrame) -> pd.DataFrame:
-        if self._last_annual > self._last_quarterly:
-            return dfi.query('report_type == "ANNUAL"')
+        """Calculate trailing twelve months (TTM) for income statement and cash
+        when quarterly data is the most recent available. If the function was
+        called, the last period is quarterly"""
+
+        # Quarterly dataframe
+        dfq = dfi.query("not is_annual").copy()
+        ttm_period_begin = dfq["period_end"].min()
 
-        df1 = dfi.query("period_end == @self._last_quarterly").copy()
-        df1.query("period_begin == period_begin.min()", inplace=True)
+        # Last quarter in quarterly dataframe
+        df1 = dfq.query("period_end == period_end.max()").copy()
 
-        df2 = dfi.query("period_reference == @self._last_quarterly").copy()
-        df2.query("period_begin == period_begin.min()", inplace=True)
+        # Previous quarter in quarterly dataframe
+        df2 = dfq.query("period_end == period_end.min()").copy()
         df2["acc_value"] = -df2["acc_value"]
 
-        df3 = dfi.query("period_end == @self._last_annual").copy()
+        # Last annual report
+        dfa = dfi.query("is_annual and period_end == @self._last_annual").copy()
 
+        # Construct TTM dataframe
         df_ttm = (
-            pd.concat([df1, df2, df3], ignore_index=True)[["acc_code", "acc_value"]]
+            pd.concat([df1, df2, dfa], ignore_index=True)[["acc_code", "acc_value"]]
             .groupby(by="acc_code")
             .sum()
             .reset_index()
         )
         df1.drop(columns="acc_value", inplace=True)
         df_ttm = pd.merge(df1, df_ttm)
-        df_ttm["report_type"] = "QUARTERLY"
-        df_ttm["period_begin"] = self._last_quarterly - pd.DateOffset(years=1)
+        df_ttm["period_begin"] = ttm_period_begin
 
-        df_annual = dfi.query('report_type == "ANNUAL"').copy()
+        df_annual = dfi.query("is_annual").copy()
 
         return pd.concat([df_annual, df_ttm], ignore_index=True)
 
     def custom_report(
         self,
         acc_list: list[str],
         num_years: int = 0,
@@ -502,24 +510,23 @@
 
         Returns:
             pd.DataFrame: Generated financial report as a pandas DataFrame.
 
         Raises:
             ValueError: If some argument is invalid.
         """
-        df_bs = self.report("balance_sheet")
-        df_is = self.report("income_statement")
-        df_cf = self.report("cash_flow")
-        dfo = pd.concat([df_bs, df_is, df_cf]).query(f"acc_code == {acc_list}")
-        # Show only selected years
-        if num_years > 0:
-            cols = dfo.columns.to_list()
-            cols = cols[0:2] + cols[-num_years:]
-            dfo = dfo[cols]
-        return dfo
+        df_bs = self.report("balance_sheet", num_years=num_years)
+        df_is = self.report("income_statement", num_years=num_years)
+        df_cf = self.report("cash_flow", num_years=num_years)
+        df = (
+            pd.concat([df_bs, df_is, df_cf])
+            .query(f"acc_code == {acc_list}")
+            .reset_index(drop=True)
+        )
+        return df
 
     @staticmethod
     def _prior_values(s: pd.Series, is_prior: bool) -> pd.Series:
         """Shift row to the right in order to obtain series previous values"""
         if is_prior:
             arr = s.iloc[:-1].values
             return np.append(np.nan, arr)
@@ -598,12 +605,11 @@
         dfo.loc["return_on_equity"] = net_income / equity_p
         dfo.loc["gross_margin"] = gross_profit / revenues
         dfo.loc["ebitda_margin"] = ebitda / revenues
         dfo.loc["pre_tax_operating_margin"] = ebit / revenues
         dfo.loc["after_tax_operating_margin"] = ebit * (1 - self._tax_rate) / revenues
         dfo.loc["net_margin"] = net_income / revenues
 
-        dfo.index.name = "Company Financial Indicators"
         # Show only the selected number of years
         if num_years > 0:
             dfo = dfo[dfo.columns[-num_years:]]
         return dfo
```

### Comparing `finlogic-0.4.8/finlogic/cvm.py` & `finlogic-0.5.0/finlogic/cvm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Module to download and process CVM data."""
 import re
 from typing import List
 import zipfile as zf
 from pathlib import Path
+from tqdm import tqdm
 import pandas as pd
+import numpy as np
 import requests
 from . import config as cfg
 
 URL_DFP = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/"
 URL_ITR = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/"
 
-CHECKMARK = "\033[32m\u2714\033[0m"
+CVM_RAW_DIR = cfg.DATA_PATH / "cvm" / "raw"
+CVM_PROCESSED_DIR = cfg.DATA_PATH / "cvm" / "processed"
+# Create CVM folders if they do not exist
+Path.mkdir(CVM_RAW_DIR, parents=True, exist_ok=True)
+Path.mkdir(CVM_PROCESSED_DIR, parents=True, exist_ok=True)
 
 
 def get_file_urls(cvm_url) -> List[str]:
     """Return a list of available CVM files.
 
     Urls with CVM raw files:
     https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/
@@ -46,37 +52,40 @@
     urls = urls_dfp + urls_itr
     return urls
 
 
 def update_raw_file(url: str, s: requests.Session) -> Path:
     """Update raw file from CVM portal. Return a Path if file is updated."""
     filename = url[-23:]  # filename = end of url
-    filepath = cfg.CVM_RAW_DIR / filename
+    filepath = CVM_RAW_DIR / filename
     headers = s.head(url).headers
     filesize = filepath.stat().st_size if filepath.exists() else 0
     if filesize == int(headers["Content-Length"]):
-        print(f"    - {filename} is the same -> skip.")
+        # file is already updated
         return None
     r = s.get(url)
     if r.status_code != 200:
         return None
 
     # Save file with Pathlib
     filepath.write_bytes(r.content)
-    print(f"    {CHECKMARK} {filename} updated.")
-
     return filepath
 
 
 def update_raw_files(urls: str) -> List[Path]:
     """Update CVM raw files."""
     s = requests.Session()
-    updated_filepaths = [update_raw_file(url, s) for url in urls]
+    updated_filepaths = []
+    for url in tqdm(urls, desc="Updating..."):
+        filepath = update_raw_file(url, s)
+        # print(f"    {CHECKMARK} {filename} updated.")
+        if filepath:
+            updated_filepaths.append(filepath)
     s.close()
-    return [filepath for filepath in updated_filepaths if filepath is not None]
+    return updated_filepaths
 
 
 def read_raw_file(filepath: Path) -> pd.DataFrame:
     """Read annual file, process it, save the result and return the file path."""
     cvm_zipfile = zf.ZipFile(filepath)
     child_filenames = cvm_zipfile.namelist()
 
@@ -111,15 +120,15 @@
         "DT_REFER": "period_reference",
         "DT_INI_EXERC": "period_begin",
         "DT_FIM_EXERC": "period_end",
         "ORDEM_EXERC": "period_order",
         "CD_CONTA": "acc_code",
         "DS_CONTA": "acc_name",
         "COLUNA_DF": "es_name",  # equity_statement_name
-        "ST_CONTA_FIXA": "acc_fixed",
+        "ST_CONTA_FIXA": "is_acc_fixed",
         "VL_CONTA": "acc_value",
         "GRUPO_DFP": "report_group",
         "MOEDA": "Currency",
         "ESCALA_MOEDA": "currency_unit",
     }
     df = df.rename(columns=columns_translation)[columns_translation.values()]
 
@@ -127,35 +136,35 @@
     df = df.drop(columns=["Currency"])
 
     # The CVM file stores only the last report_version -> drop it.
     df = df.drop(columns=["report_version"])
     # report_version max. value is aprox. 9, so it can be uint8 (0 to 255)
     # df["report_version"] = df["report_version"].astype("uint8")
 
-    # acc_fixed values are ['S', 'N']
+    # is_acc_fixed values are ['S', 'N']
     map_dic = {"S": True, "N": False}
-    df["acc_fixed"] = df["acc_fixed"].map(map_dic).astype(bool)
+    df["is_acc_fixed"] = df["is_acc_fixed"].map(map_dic).astype(bool)
 
-    # Remove rows with acc_value == 0 and acc_fixed == False
-    # df.query("acc_value != 0 or acc_fixed == True", inplace=True)
+    # Remove rows with acc_value == 0 and is_acc_fixed == False
+    # df.query("acc_value != 0 or is_acc_fixed == True", inplace=True)
     df.query("acc_value != 0", inplace=True)
 
-    # acc_fixed is being used used only non fixed accounts with acc_value == 0
+    # is_acc_fixed is being used used only non fixed accounts with acc_value == 0
     # So it can be dropped after the query above.
-    df = df.drop(columns=["acc_fixed"])
+    df = df.drop(columns=["is_acc_fixed"])
 
     # cvm_id max. value is 600_000, so it can be uint32 (0 to 4_294_967_295)
     df["cvm_id"] = df["cvm_id"].astype("uint32")
 
     # There are two types of CVM files: DFP (ANNUAL) and ITR (QUARTERLY).
-    # In database, "report_type" is positioned after "tax_id" -> position = 3
+    # In database, "is_annual" is positioned after "tax_id" -> position = 3
     if filepath.name.startswith("dfp"):
-        df.insert(loc=3, column="report_type", value="ANNUAL")
+        df.insert(loc=3, column="is_annual", value=True)
     else:
-        df.insert(loc=3, column="report_type", value="QUARTERLY")
+        df.insert(loc=3, column="is_annual", value=False)
 
     # For the moment, es_name will not be used since it adds to much complexity to
     # the database. It will be dropped.
     df = df.drop(columns=["es_name"])
 
     # Remove any extra spaces (line breaks, tabs, etc.) from columns below.
     columns = ["name_id", "acc_name"]
@@ -172,19 +181,28 @@
     columns = ["period_reference", "period_begin", "period_end"]
     df[columns] = df[columns].apply(pd.to_datetime)
 
     # currency_unit values are ['MIL', 'UNIDADE']
     map_dic = {"UNIDADE": 1, "MIL": 1000}
     df["currency_unit"] = df["currency_unit"].map(map_dic).astype(int)
 
-    # Do not ajust acc_value for 3.99 codes.
-    df["acc_value"] = df["acc_value"].where(
+    # Earnings per share (EPS) values don't need to be adjusted by currency_unit.
+    df["acc_value"] = np.where(
         df["acc_code"].str.startswith("3.99"),
+        df["acc_value"],
         df["acc_value"] * df["currency_unit"],
     )
+
+    # Change earnings per share codes from 3.99. to 8. to avoid confusion with
+    # 3. (income_statement)
+    df["acc_code"] = np.where(
+        df["acc_code"].str.startswith("3.99"),
+        df["acc_code"].str.replace("3.99", "8"),
+        df["acc_code"],
+    )
     # After the adjustment, currency_unit column is not necessary.
     df.drop(columns=["currency_unit"], inplace=True)
 
     """The "period_order" column is a redundant information, since it is possible to
     infer it from the "period_reference", "period_begin" and "period_end" columns.
     For example:
         if "period_reference" is 2020-12-31
@@ -219,16 +237,16 @@
         'DF Individual - Demonstração de Valor Adicionado',
         'DF Individual - Demonstração do Fluxo de Caixa (Método Indireto)',
         'DF Individual - Demonstração do Resultado',
     Hence, with string position 3:6 we can make:
     if == 'Con' -> consolidated statement
     if == 'Ind' -> separate statement
     """
-    map_dic = {"Con": "CONSOLIDATED", "Ind": "SEPARATE"}
-    df.insert(4, "acc_method", df["report_group"].str[3:6].map(map_dic))
+    map_dic = {"Con": True, "Ind": False}
+    df.insert(4, "is_consolidated", df["report_group"].str[3:6].map(map_dic))
     # 'report_group' data can be inferred from 'acc_code'
     df.drop(columns=["report_group"], inplace=True)
 
     # In "itr_cia_aberta_2022.zip", as an example, 2742 rows are duplicated.
     # Few of them have different values in "acc_value". Only one them will be kept.
     # REMOVE ALL VALUES OR MARK THESE ROWS AS ERRORS?
     cols = df.columns.tolist()
@@ -238,32 +256,38 @@
     return df
 
 
 def process_file(raw_filepath: Path) -> Path:
     """Read, process and save a CVM file."""
     df = read_raw_file(raw_filepath)
     df = process_df(df, raw_filepath)
-    processed_filepath = cfg.CVM_PROCESSED_DIR / (raw_filepath.stem + ".pickle")
+    processed_filepath = CVM_PROCESSED_DIR / (raw_filepath.stem + ".pickle")
     # save_processed_df(df, processed_filepath)
     df.to_pickle(processed_filepath, compression="zstd")
-    print(f"    {CHECKMARK} {raw_filepath.name} processed.")
     return processed_filepath
 
 
+def process_files_with_progress(filepaths_to_process):
+    """Process CVM files with a progress bar."""
+    for filepath in tqdm(filepaths_to_process, desc="Processing..."):
+        # print(f"    {CHECKMARK} {raw_filepath.name} processed.")
+        process_file(filepath)
+
+
 def get_raw_file_mtimes() -> pd.DataFrame:
     """Return a Pandas DataFrame with file_source and file_mtime columns."""
-    filepaths = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
+    filepaths = sorted(CVM_RAW_DIR.glob("*.zip"))
     d_mtimes = {filepath.name: filepath.stat().st_mtime for filepath in filepaths}
     return pd.DataFrame(d_mtimes.items(), columns=["file_source", "file_mtime"])
 
 
 def read_all_processed_files() -> pd.DataFrame:
     """Read all processed CVM files."""
     # list filepaths in processed folder
-    filepaths = sorted(cfg.CVM_PROCESSED_DIR.glob("*.pickle"))
+    filepaths = sorted(CVM_PROCESSED_DIR.glob("*.pickle"))
     df = pd.concat([pd.read_pickle(f, compression="zstd") for f in filepaths])
     columns = df.columns
     cat_cols = [c for c in columns if df[c].dtype in ["object"]]
     df[cat_cols] = df[cat_cols].astype("category")
     return df
 
 
@@ -272,39 +296,45 @@
 
     Because the report holds accounting entries for the year before, we can keep only
     the most recent one in the database. By doing this, we guarantee
     that there is only one valid accounting value in the database -> the last one
     """
     sort_cols = [
         "cvm_id",
-        "acc_method",
+        "is_consolidated",
         "acc_code",
         "period_reference",
-        "report_type",
+        "is_annual",
         "period_begin",
         "period_end",
     ]
     df.sort_values(by=sort_cols, ascending=True, inplace=True, ignore_index=True)
 
     subset_cols = [
         "cvm_id",
-        "acc_method",
+        "is_consolidated",
         "acc_code",
         "period_begin",
         "period_end",
     ]
-    df.drop_duplicates(subset=subset_cols, keep="last", inplace=True, ignore_index=True)
-
-    return df
+    return df.drop_duplicates(subset=subset_cols, keep="last", ignore_index=True)
 
 
 def drop_unecessary_quarterly_entries(df: pd.DataFrame) -> pd.DataFrame:
     """Keep the last QUARTERLY report for each company only when necessary."""
+    # Create a temporary column with the max. period_reference for each company
     df["max_period"] = df.groupby("cvm_id")["period_reference"].transform("max")
 
-    condition1 = df["report_type"] == "QUARTERLY"
-    condition2 = df["period_reference"] < df["max_period"]
-    df = df[~(condition1 & condition2)].reset_index(drop=True)
+    mask1 = ~df["is_annual"]
+    mask2 = df["period_reference"] < df["max_period"]
+    mask = ~(mask1 & mask2)
+    return df[mask].reset_index(drop=True).drop(columns=["max_period"])
 
-    df.drop(columns=["max_period"], inplace=True)
 
-    return df
+def build_main_df():
+    """Build FinLogic Database from processed CVM files."""
+    df = read_all_processed_files()
+    df = drop_not_last_entries(df)
+    df = drop_unecessary_quarterly_entries(df)
+    # After the drop_unecessary entries, period_reference is not necessary anymore
+    df.drop(columns=["period_reference"], inplace=True)
+    df.to_pickle(cfg.DF_PATH, compression="zstd")
```

### Comparing `finlogic-0.4.8/finlogic/database.py` & `finlogic-0.5.0/finlogic/data_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,93 +3,119 @@
 This module provides functions to handle financial data from the CVM Portal. It
 allows updating, processing and consolidating financial statements, as well as
 searching for company names in the FinLogic Database and retrieving information
 about the database itself.
 """
 from pathlib import Path
 from typing import Literal
+from datetime import datetime
 import pandas as pd
-from . import cvm
 from . import config as cfg
+from . import cvm
 from . import language as lng
-from . import fprint as fpr
-from . import fduckdb as fdb
 
 CHECKMARK = "\033[32m\u2714\033[0m"
 
 
+def get_main_df() -> pd.DataFrame:
+    """Return a DataFrame with all accounting data"""
+    if cfg.DF_PATH.is_file():
+        df = pd.read_pickle(cfg.DF_PATH, compression="zstd")
+    else:
+        df = pd.DataFrame()
+
+    return df
+
+
 def get_filepaths_to_process(df1: pd.DataFrame, df2: pd.DataFrame) -> list[Path]:
     """Return a list of CVM files that has to be processed by comparing
     the files mtimes from the raw folder.
     """
     df = pd.concat([df1, df2]).drop_duplicates(keep=False)
     file_sources = sorted(df["file_source"].drop_duplicates())
-    return [cfg.CVM_RAW_DIR / file_source for file_source in file_sources]
+    return [cvm.CVM_RAW_DIR / file_source for file_source in file_sources]
 
 
-def update_database(rebuild: bool = False):
+def update(rebuild: bool = False):
     """Verify changes in CVM files and update Finlogic Database if necessary.
 
     Args:
         rebuild (bool, optional): If True, processes all CVM files and rebuilds
             the database. Defaults to False.
     Returns:
         None
     """
     # Language files
     print('\nUpdating "language" database...')
     lng.process_language_df()
 
     # CVM raw files
-    print("Updating CVM files...")
     # Get files mtimes from the raw folder before updating
     df_raw1 = cvm.get_raw_file_mtimes()
     urls = cvm.get_all_file_urls()
     updated_raw_filepaths = cvm.update_raw_files(urls)
     print(f"Number of CVM files updated = {len(updated_raw_filepaths)}")
     # Get files mtimes from the raw folder after updating
     df_raw2 = cvm.get_raw_file_mtimes()
 
     # CVM processed files
-    print("\nProcessing CVM files...")
     if rebuild:
         # Process all files
-        filepaths_to_process = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
+        filepaths_to_process = sorted(cvm.CVM_RAW_DIR.glob("*.zip"))
     else:
         # Process only updated files
         filepaths_to_process = get_filepaths_to_process(df1=df_raw1, df2=df_raw2)
     print(f"Number of new files to process = {len(filepaths_to_process)}")
-    if filepaths_to_process:
-        [cvm.process_file(filepath) for filepath in filepaths_to_process]
+
+    cvm.process_files_with_progress(filepaths_to_process)
 
     # FinLogic Database
-    fdb.build()
-    print(f"\n{CHECKMARK} FinLogic Database updated!")
+    print("\nBuilding FinLogic main DataFrame...")
+    cvm.build_main_df()
+    print(f"{CHECKMARK} FinLogic updated!")
 
 
-def database_info():
-    """Print a concise summary of FinLogic Database.
+def info() -> pd.DataFrame:
+    """Print a concise summary of FinLogic available data.
 
-    This function prints a dictionary containing main information about
+    This function returns a dataframe containing main information about
     FinLogic Database, such as the database path, file size, last update call,
     last modified dates, size in memory, number of accounting rows, unique
     accounting codes, companies, unique financial statements, first financial
     statement date and last financial statement date.
 
     Args:
         return_dict (bool, optional): If True, returns a dictionary with the
             database information and do not print it.
 
     Returns: None
     """
-    info_dict = fdb.get_info()
-    if info_dict:
-        fpr.print_dict(info_dict=info_dict, table_name="FinLogic Database Info")
-    else:
-        print("FinLogic Database is empty.")
+    info = {}
+    df = get_main_df()
+    if df.empty:
+        return pd.DataFrame()
+
+    info["data_path"] = f"{cfg.DATA_PATH}"
+    info["data_size"] = f"{cfg.DF_PATH.stat().st_size / 1024**2:.1f} MB"
+    db_last_modified = datetime.fromtimestamp(cfg.DF_PATH.stat().st_mtime)
+    info["last_modified_on"] = db_last_modified.strftime("%Y-%m-%d %H:%M:%S")
+
+    info["accounting_entries"] = df.shape[0]
+
+    report_cols = ["cvm_id", "is_annual", "period_end"]
+    info["number_of_reports"] = df[report_cols].drop_duplicates().shape[0]
+    info["first_report"] = df["period_end"].min().strftime("%Y-%m-%d")
+    info["last_report"] = df["period_end"].max().strftime("%Y-%m-%d")
+
+    info["number_of_companies"] = df["cvm_id"].nunique()
+
+    s = pd.Series(info)
+    s.name = "FinLogic Info"
+
+    return s.to_frame()
 
 
 def search_company(
     search_value: str, search_by: Literal["name_id", "cvm_id", "tax_id"] = "name_id"
 ) -> pd.DataFrame:
     """Search for a company name in FinLogic Database.
 
@@ -104,25 +130,21 @@
             values are 'name_id', 'cvm_id', and 'tax_id'. Defaults to 'name_id'.
 
     Returns:
         pd.DataFrame: A DataFrame containing the search results, with columns
             'name_id', 'cvm_id', and 'tax_id' for each unique company that
             matches the search criteria.
     """
+    search_cols = ["name_id", "cvm_id", "tax_id"]
+    df = get_main_df()[search_cols].drop_duplicates(ignore_index=True)
     match search_by:
         case "name_id":
             # Company name is stored in uppercase in the database
-            sql_condition = f"LIKE '%{search_value.upper()}%'"
+            df.query(f"name_id.str.contains('{search_value.upper()}')", inplace=True)
         case "cvm_id":
-            sql_condition = f"= {search_value}"
+            df.query(f"cvm_id == {search_value}", inplace=True)
         case "tax_id":
-            sql_condition = f"LIKE '%{search_value}%'"
+            df.query(f"tax_id == '{search_value}'", inplace=True)
         case _:
             raise ValueError("Invalid value for 'search_by' argument.")
 
-    query = f"""--sql
-        SELECT DISTINCT name_id, cvm_id, tax_id
-          FROM reports
-         WHERE {search_by} {sql_condition}
-         ORDER BY cvm_id;
-    """
-    return fdb.execute(query, "df")
+    return df.reset_index(drop=True)
```

### Comparing `finlogic-0.4.8/finlogic/language.py` & `finlogic-0.5.0/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.8/pyproject.toml` & `finlogic-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -22,19 +22,18 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pandas>=1.5.0",
     "requests>=2.30.0",
-    "duckdb>=0.8.0",
-    "rich>=13.0.0",
+    "tqdm>=4.1.0",
     "zstandard>=0.21.0",
 ]
-version = "0.4.8"
+version = "0.5.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.4.8/tests/test_company.py` & `finlogic-0.5.0/tests/test_company.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 import finlogic as fl
 
 
 class TestCompany(unittest.TestCase):
     def setUp(self):
-        self.petro_sep = fl.Company(9512, acc_method="sep", acc_unit="b")
-        self.petro_con = fl.Company(9512, acc_method="con", acc_unit="b")
+        self.petro_sep = fl.Company(9512, is_consolidated=False, acc_unit="b")
+        self.petro_con = fl.Company(9512, is_consolidated=True, acc_unit="b")
 
     def test_identifier(self):
         """Test the identifier method of the Company class."""
         test_cvm_id = 4170
         test_tax_id = "33.592.510/0001-54"
         self.petro_sep.identifier = test_cvm_id
         self.assertEqual(self.petro_sep._cvm_id, test_cvm_id)
```

### Comparing `finlogic-0.4.8/PKG-INFO` & `finlogic-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.8
+Version: 0.5.0
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -30,16 +30,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/crdcj/FinLogic
 Requires-Python: >=3.10
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: requests>=2.30.0
-Requires-Dist: duckdb>=0.8.0
-Requires-Dist: rich>=13.0.0
+Requires-Dist: tqdm>=4.1.0
 Requires-Dist: zstandard>=0.21.0
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
@@ -49,15 +48,15 @@
 
 <!-- [![Anaconda-Server Badge](https://anaconda.org/conda-forge/finlogic/badges/version.svg)](https://anaconda.org/conda-forge/finlogic)" -->
 
 ## FinLogic: finance toolkit for listed Brazilian companies.
 
 ---
 
-**FinLogic** offers a Pythonic way to analyze financial data of listed companies in Brazil from information made publicly avaible by local securities market authority (CVM). FinLogic uses DuckDB as an OLAP database management system and Pandas to process the data to and from the locally builted accounting database (aprox. 8 million rows).
+**FinLogic** offers a Pythonic way to analyze the financial data of companies listed in Brazil, using information made publicly available by the local securities market authority, CVM. FinLogic processes approximately 20 million accounting entries using Pandas, and constructs a local DataFrame for ultra-fast access to this information.
 
 ---
 
 ## Installation
 
 The source code is currently hosted on GitHub at:
 https://github.com/crdcj/FinLogic
@@ -68,40 +67,39 @@
 # PyPI:
 pip install finlogic
 ```
 
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
-- [DuckDB](https://github.com/pydata/pandas) \>= 0.8.0
 - [Pandas](https://github.com/pydata/pandas) \>= 1.5.0
 - [Requests](http://docs.python-requests.org/en/master/) \>= 2.30.0
-- [Rich](https://github.com/Textualize/rich) \>= 13.0.0
+- [tqdm](https://github.com/tqdm/tqdm) \>= 4.1.0
 - [Zstandard](https://python-zstandard.readthedocs.io/en/latest/) \>= 0.21.0
 
 ---
 
 ## Quick Start
 
 ### Create FinLogic Database
 
-The 'update_database' function is responsible for downloading raw financial files from CVM, processesing aprox. 8 millions rows of accounting values and loading it into FinLogic Database for local data analysis. In the firt run, the process can take more than 1 minute depending on CVM Server connection and local CPU power. For subsequent updates, only updated CVM files will be processed, which will be faster.
+The 'update' function is responsible for downloading and updating raw financial data from the CVM, processing approximately 20 million accounting entries, and storing them for local data analysis. During the initial run, the process might take longer than 1 minute, depending on the CVM server connection and local CPU power. For subsequent updates, only the updated CVM files will be downloaded and processed, which should expedite the operation.
 
 ```python
 >>> import finlogic as fl
 
 # Compile FinLogic database for the first time:
->>> fl.update_database()
+>>> fl.update()
 
 Updating CVM raw files...
 ...
 FinLogic database updated ✅
 
 # Show database info:
->>> fl.database_info()
+>>> fl.info()
 ```
 
 | FinLogic Database Info |                         Value |
 | :--------------------- | ----------------------------: |
 | db_path                | .../finlogic/data/finlogic.db |
 | db_size                |                       76.0 MB |
 | db_last_modified       |           2023-04-20 07:29:08 |
@@ -130,18 +128,18 @@
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
->>> petro = fl.Company(9512, acc_method='sep', acc_unit='m')
+>>> petro = fl.Company(9512, is_consolidated='sep', acc_unit='m')
 
 # Change company accounting method back to consolidated (default):
->>> petro.acc_method = 'con'
+>>> petro.is_consolidated = 'con'
 
 # Change company accounting unit to billion (default is 1):
 >>> petro.acc_unit = 'b'
 
 # Show company info:
 >>> petro.info()
 ```
```

