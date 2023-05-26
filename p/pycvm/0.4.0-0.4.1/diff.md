# Comparing `tmp/pycvm-0.4.0.tar.gz` & `tmp/pycvm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycvm-0.4.0.tar", last modified: Fri Oct 14 14:18:23 2022, max compression
+gzip compressed data, was "pycvm-0.4.1.tar", last modified: Fri May 26 16:59:12 2023, max compression
```

## Comparing `pycvm-0.4.0.tar` & `pycvm-0.4.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.339596 pycvm-0.4.0/
--rw-rw-rw-   0        0        0     1088 2022-10-01 17:47:55.000000 pycvm-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     2338 2022-10-14 14:18:23.340596 pycvm-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1883 2022-10-14 14:15:06.000000 pycvm-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.352596 pycvm-0.4.0/cvm/
--rw-rw-rw-   0        0        0      228 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/__init__.py
--rw-rw-rw-   0        0        0      518 2022-10-14 14:18:23.353596 pycvm-0.4.0/cvm/_version.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.121595 pycvm-0.4.0/cvm/balances/
--rw-rw-rw-   0        0        0      133 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/__init__.py
--rw-rw-rw-   0        0        0     5206 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/account_layout.py
--rw-rw-rw-   0        0        0     4572 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/balance_sheet.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.124596 pycvm-0.4.0/cvm/balances/common/
--rw-rw-rw-   0        0        0        0 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/common/__init__.py
--rw-rw-rw-   0        0        0     2807 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/common/dre.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.135596 pycvm-0.4.0/cvm/balances/financial/
--rw-rw-rw-   0        0        0        0 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/financial/__init__.py
--rw-rw-rw-   0        0        0     2704 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/financial/bpa.py
--rw-rw-rw-   0        0        0     2886 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/financial/bpp.py
--rw-rw-rw-   0        0        0     2852 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/balances/financial/cvm_codes.py
--rw-rw-rw-   0        0        0     3597 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/financial/dre.py
--rw-rw-rw-   0        0        0     4613 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/income_statement.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.147595 pycvm-0.4.0/cvm/balances/industrial/
--rw-rw-rw-   0        0        0        0 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/industrial/__init__.py
--rw-rw-rw-   0        0        0     1519 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/industrial/bpa.py
--rw-rw-rw-   0        0        0     2225 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/industrial/bpp.py
--rw-rw-rw-   0        0        0    45506 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/balances/industrial/cvm_codes.py
--rw-rw-rw-   0        0        0     2062 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/industrial/dre.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.180596 pycvm-0.4.0/cvm/balances/insurance/
--rw-rw-rw-   0        0        0        0 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/insurance/__init__.py
--rw-rw-rw-   0        0        0     1689 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/insurance/bpa.py
--rw-rw-rw-   0        0        0     1123 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/insurance/bpp.py
--rw-rw-rw-   0        0        0      486 2022-10-03 22:42:55.000000 pycvm-0.4.0/cvm/balances/insurance/cvm_codes.py
--rw-rw-rw-   0        0        0     2576 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/balances/insurance/dre.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.183595 pycvm-0.4.0/cvm/cad/
--rw-rw-rw-   0        0        0       30 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/cad/__init__.py
--rw-rw-rw-   0        0        0     6127 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/cad/company.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.226601 pycvm-0.4.0/cvm/csvio/
--rw-rw-rw-   0        0        0       94 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/csvio/__init__.py
--rw-rw-rw-   0        0        0     1442 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/csvio/batch.py
--rw-rw-rw-   0        0        0    22807 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/csvio/dfpitr.py
--rw-rw-rw-   0        0        0     2169 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/csvio/document.py
--rw-rw-rw-   0        0        0    48168 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/csvio/fca.py
--rw-rw-rw-   0        0        0     6798 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/csvio/fre.py
--rw-rw-rw-   0        0        0     1311 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/csvio/member.py
--rw-rw-rw-   0        0        0     1410 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/csvio/row.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.282596 pycvm-0.4.0/cvm/datatypes/
--rw-rw-rw-   0        0        0     1038 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/__init__.py
--rw-rw-rw-   0        0        0    10431 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/datatypes/account.py
--rw-rw-rw-   0        0        0      460 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/address.py
--rw-rw-rw-   0        0        0     1456 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/auditor.py
--rw-rw-rw-   0        0        0      995 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/bookkeeping_agent.py
--rw-rw-rw-   0        0        0     2055 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/capital_distribution.py
--rw-rw-rw-   0        0        0      188 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/communication_channel.py
--rw-rw-rw-   0        0        0      250 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/contact.py
--rw-rw-rw-   0        0        0      324 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/controlling_interest.py
--rw-rw-rw-   0        0        0      133 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/currency.py
--rw-rw-rw-   0        0        0     4587 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/document.py
--rw-rw-rw-   0        0        0     5763 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/industry.py
--rw-rw-rw-   0        0        0     1646 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/investor_relations.py
--rw-rw-rw-   0        0        0     4226 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/issuer.py
--rw-rw-rw-   0        0        0      763 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/phone.py
--rw-rw-rw-   0        0        0      392 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/registration.py
--rw-rw-rw-   0        0        0     3013 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/security.py
--rw-rw-rw-   0        0        0      778 2022-10-01 17:48:22.000000 pycvm-0.4.0/cvm/datatypes/shareholder_department.py
--rw-rw-rw-   0        0        0    18981 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/statement.py
--rw-rw-rw-   0        0        0     4759 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/datatypes/tax_id.py
--rw-rw-rw-   0        0        0      440 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/datatypes/trading_admission.py
--rw-rw-rw-   0        0        0     1133 2022-10-01 17:47:55.000000 pycvm-0.4.0/cvm/exceptions.py
--rw-rw-rw-   0        0        0      627 2022-10-14 14:15:06.000000 pycvm-0.4.0/cvm/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-14 14:18:23.338596 pycvm-0.4.0/pycvm.egg-info/
--rw-rw-rw-   0        0        0     2338 2022-10-14 14:18:22.000000 pycvm-0.4.0/pycvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1771 2022-10-14 14:18:22.000000 pycvm-0.4.0/pycvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-14 14:18:22.000000 pycvm-0.4.0/pycvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2022-10-14 14:18:22.000000 pycvm-0.4.0/pycvm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      202 2022-10-14 14:18:23.350596 pycvm-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      998 2022-10-01 17:47:55.000000 pycvm-0.4.0/setup.py
--rw-rw-rw-   0        0        0    84600 2022-10-01 17:47:55.000000 pycvm-0.4.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:12.007861 pycvm-0.4.1/
+-rw-rw-rw-   0        0        0     1111 2023-05-26 16:57:59.000000 pycvm-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2347 2023-05-26 16:59:12.008859 pycvm-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1883 2022-10-14 15:00:15.000000 pycvm-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:12.014857 pycvm-0.4.1/cvm/
+-rw-rw-rw-   0        0        0      228 2022-10-14 15:00:15.000000 pycvm-0.4.1/cvm/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-05-26 16:59:12.015856 pycvm-0.4.1/cvm/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.277989 pycvm-0.4.1/cvm/balances/
+-rw-rw-rw-   0        0        0      133 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/__init__.py
+-rw-rw-rw-   0        0        0     5206 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/account_layout.py
+-rw-rw-rw-   0        0        0     4572 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/balance_sheet.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.290991 pycvm-0.4.1/cvm/balances/common/
+-rw-rw-rw-   0        0        0        0 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/common/__init__.py
+-rw-rw-rw-   0        0        0     2807 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/common/dre.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.358778 pycvm-0.4.1/cvm/balances/financial/
+-rw-rw-rw-   0        0        0        0 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/financial/__init__.py
+-rw-rw-rw-   0        0        0     2704 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/financial/bpa.py
+-rw-rw-rw-   0        0        0     2886 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/financial/bpp.py
+-rw-rw-rw-   0        0        0     2852 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/financial/cvm_codes.py
+-rw-rw-rw-   0        0        0     3597 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/financial/dre.py
+-rw-rw-rw-   0        0        0     4613 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/income_statement.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.429794 pycvm-0.4.1/cvm/balances/industrial/
+-rw-rw-rw-   0        0        0        0 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/industrial/__init__.py
+-rw-rw-rw-   0        0        0     1519 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/industrial/bpa.py
+-rw-rw-rw-   0        0        0     2225 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/industrial/bpp.py
+-rw-rw-rw-   0        0        0    45506 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/industrial/cvm_codes.py
+-rw-rw-rw-   0        0        0     2062 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/industrial/dre.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.508331 pycvm-0.4.1/cvm/balances/insurance/
+-rw-rw-rw-   0        0        0        0 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/insurance/__init__.py
+-rw-rw-rw-   0        0        0     1689 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/insurance/bpa.py
+-rw-rw-rw-   0        0        0     1123 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/insurance/bpp.py
+-rw-rw-rw-   0        0        0      486 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/insurance/cvm_codes.py
+-rw-rw-rw-   0        0        0     2576 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/balances/insurance/dre.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.529332 pycvm-0.4.1/cvm/cad/
+-rw-rw-rw-   0        0        0       30 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/cad/__init__.py
+-rw-rw-rw-   0        0        0     6127 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/cad/company.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.645335 pycvm-0.4.1/cvm/csvio/
+-rw-rw-rw-   0        0        0       94 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/__init__.py
+-rw-rw-rw-   0        0        0     1442 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/batch.py
+-rw-rw-rw-   0        0        0    22807 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/dfpitr.py
+-rw-rw-rw-   0        0        0     2169 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/document.py
+-rw-rw-rw-   0        0        0    48168 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/fca.py
+-rw-rw-rw-   0        0        0     6798 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/fre.py
+-rw-rw-rw-   0        0        0     1311 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/member.py
+-rw-rw-rw-   0        0        0     1410 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/csvio/row.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:11.970856 pycvm-0.4.1/cvm/datatypes/
+-rw-rw-rw-   0        0        0     1038 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/__init__.py
+-rw-rw-rw-   0        0        0    10431 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/account.py
+-rw-rw-rw-   0        0        0      460 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/address.py
+-rw-rw-rw-   0        0        0     1456 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/auditor.py
+-rw-rw-rw-   0        0        0      995 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/bookkeeping_agent.py
+-rw-rw-rw-   0        0        0     2055 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/capital_distribution.py
+-rw-rw-rw-   0        0        0      188 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/communication_channel.py
+-rw-rw-rw-   0        0        0      250 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/contact.py
+-rw-rw-rw-   0        0        0      324 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/controlling_interest.py
+-rw-rw-rw-   0        0        0      133 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/currency.py
+-rw-rw-rw-   0        0        0     4587 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/document.py
+-rw-rw-rw-   0        0        0     5763 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/industry.py
+-rw-rw-rw-   0        0        0     1646 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/investor_relations.py
+-rw-rw-rw-   0        0        0     4226 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/issuer.py
+-rw-rw-rw-   0        0        0      763 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/phone.py
+-rw-rw-rw-   0        0        0      392 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/registration.py
+-rw-rw-rw-   0        0        0     3013 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/security.py
+-rw-rw-rw-   0        0        0      778 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/shareholder_department.py
+-rw-rw-rw-   0        0        0    18981 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/statement.py
+-rw-rw-rw-   0        0        0     4759 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/tax_id.py
+-rw-rw-rw-   0        0        0      440 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/datatypes/trading_admission.py
+-rw-rw-rw-   0        0        0     1133 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/exceptions.py
+-rw-rw-rw-   0        0        0      627 2022-10-14 15:00:16.000000 pycvm-0.4.1/cvm/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:59:12.004871 pycvm-0.4.1/pycvm.egg-info/
+-rw-rw-rw-   0        0        0     2347 2023-05-26 16:59:10.000000 pycvm-0.4.1/pycvm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1771 2023-05-26 16:59:11.000000 pycvm-0.4.1/pycvm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 16:59:10.000000 pycvm-0.4.1/pycvm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-26 16:59:10.000000 pycvm-0.4.1/pycvm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      202 2023-05-26 16:59:12.012858 pycvm-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1007 2023-05-26 16:57:59.000000 pycvm-0.4.1/setup.py
+-rw-rw-rw-   0        0        0    84600 2022-10-14 15:00:16.000000 pycvm-0.4.1/versioneer.py
```

### Comparing `pycvm-0.4.0/LICENSE` & `pycvm-0.4.1/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Giovanni L
+Copyright (c) 2022-2023 Giovanni Lourenço Fernandes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycvm-0.4.0/PKG-INFO` & `pycvm-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pycvm
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python library for processing data from CVM
-Home-page: https://github.com/callmegiorgio/pycvm/
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pycvm/
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: investment,finances
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
```

### Comparing `pycvm-0.4.0/README.md` & `pycvm-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/_version.py` & `pycvm-0.4.1/cvm/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-10-14T11:15:06-0300",
+ "date": "2023-05-26T13:57:33-0300",
  "dirty": false,
  "error": null,
- "full-revisionid": "e358b86480dc91934e4d0eb4839c25931b13f39f",
- "version": "0.4.0"
+ "full-revisionid": "ea628d3141e7221e73b73554d58a45aaa8769881",
+ "version": "0.4.1"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

### Comparing `pycvm-0.4.0/cvm/balances/account_layout.py` & `pycvm-0.4.1/cvm/balances/account_layout.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/balance_sheet.py` & `pycvm-0.4.1/cvm/balances/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/common/dre.py` & `pycvm-0.4.1/cvm/balances/common/dre.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/financial/bpa.py` & `pycvm-0.4.1/cvm/balances/financial/bpa.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/financial/bpp.py` & `pycvm-0.4.1/cvm/balances/financial/bpp.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/financial/cvm_codes.py` & `pycvm-0.4.1/cvm/balances/financial/cvm_codes.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/financial/dre.py` & `pycvm-0.4.1/cvm/balances/financial/dre.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/income_statement.py` & `pycvm-0.4.1/cvm/balances/income_statement.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/industrial/bpa.py` & `pycvm-0.4.1/cvm/balances/industrial/bpa.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/industrial/bpp.py` & `pycvm-0.4.1/cvm/balances/industrial/bpp.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/industrial/cvm_codes.py` & `pycvm-0.4.1/cvm/balances/industrial/cvm_codes.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/industrial/dre.py` & `pycvm-0.4.1/cvm/balances/industrial/dre.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/insurance/bpa.py` & `pycvm-0.4.1/cvm/balances/insurance/bpa.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/insurance/bpp.py` & `pycvm-0.4.1/cvm/balances/insurance/bpp.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/balances/insurance/dre.py` & `pycvm-0.4.1/cvm/balances/insurance/dre.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/cad/company.py` & `pycvm-0.4.1/cvm/cad/company.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/csvio/batch.py` & `pycvm-0.4.1/cvm/csvio/batch.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/csvio/dfpitr.py` & `pycvm-0.4.1/cvm/csvio/dfpitr.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/csvio/document.py` & `pycvm-0.4.1/cvm/csvio/document.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/csvio/fca.py` & `pycvm-0.4.1/cvm/csvio/fca.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/csvio/fre.py` & `pycvm-0.4.1/cvm/csvio/fre.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/csvio/member.py` & `pycvm-0.4.1/cvm/csvio/member.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/csvio/row.py` & `pycvm-0.4.1/cvm/csvio/row.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/__init__.py` & `pycvm-0.4.1/cvm/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/account.py` & `pycvm-0.4.1/cvm/datatypes/account.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/auditor.py` & `pycvm-0.4.1/cvm/datatypes/auditor.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/bookkeeping_agent.py` & `pycvm-0.4.1/cvm/datatypes/bookkeeping_agent.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/capital_distribution.py` & `pycvm-0.4.1/cvm/datatypes/capital_distribution.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/document.py` & `pycvm-0.4.1/cvm/datatypes/document.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/industry.py` & `pycvm-0.4.1/cvm/datatypes/industry.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/investor_relations.py` & `pycvm-0.4.1/cvm/datatypes/investor_relations.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/issuer.py` & `pycvm-0.4.1/cvm/datatypes/issuer.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/phone.py` & `pycvm-0.4.1/cvm/datatypes/phone.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/security.py` & `pycvm-0.4.1/cvm/datatypes/security.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/shareholder_department.py` & `pycvm-0.4.1/cvm/datatypes/shareholder_department.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/statement.py` & `pycvm-0.4.1/cvm/datatypes/statement.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/datatypes/tax_id.py` & `pycvm-0.4.1/cvm/datatypes/tax_id.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/exceptions.py` & `pycvm-0.4.1/cvm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/cvm/utils.py` & `pycvm-0.4.1/cvm/utils.py`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/pycvm.egg-info/PKG-INFO` & `pycvm-0.4.1/pycvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pycvm
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python library for processing data from CVM
-Home-page: https://github.com/callmegiorgio/pycvm/
-Author: Giovanni L
-Author-email: callmegiorgio@hotmail.com
+Home-page: https://github.com/glourencoffee/pycvm/
+Author: Giovanni Lourenço
+Author-email: gvnl.developer@outlook.com
 License: MIT
 Keywords: investment,finances
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About
```

### Comparing `pycvm-0.4.0/pycvm.egg-info/SOURCES.txt` & `pycvm-0.4.1/pycvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycvm-0.4.0/setup.py` & `pycvm-0.4.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 setup(name                          = 'pycvm',
       version                       = versioneer.get_version(),
       cmdclass                      = versioneer.get_cmdclass(),
       description                   = 'Python library for processing data from CVM',
       long_description              = readme_en_us,
       long_description_content_type = 'text/markdown',
-      author                        = 'Giovanni L',
-      author_email                  = 'callmegiorgio@hotmail.com',
-      url                           = 'https://github.com/callmegiorgio/pycvm/',
+      author                        = 'Giovanni Lourenço',
+      author_email                  = 'gvnl.developer@outlook.com',
+      url                           = 'https://github.com/glourencoffee/pycvm/',
       license                       = 'MIT',
       packages                      = find_packages(),
       keywords                      = ['investment', 'finances'],
       install_requires              = [],
       python_requires               = '>=3.7'
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycvm-0.4.0/versioneer.py` & `pycvm-0.4.1/versioneer.py`

 * *Files identical despite different names*

