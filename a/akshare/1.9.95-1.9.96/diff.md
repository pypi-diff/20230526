# Comparing `tmp/akshare-1.9.95.tar.gz` & `tmp/akshare-1.9.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akshare-1.9.95.tar", last modified: Thu May 25 15:46:40 2023, max compression
+gzip compressed data, was "akshare-1.9.96.tar", last modified: Fri May 26 12:48:20 2023, max compression
```

## Comparing `akshare-1.9.95.tar` & `akshare-1.9.96.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.348586 akshare-1.9.95/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-25 15:46:27.000000 akshare-1.9.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-25 15:46:40.348586 akshare-1.9.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-25 15:46:27.000000 akshare-1.9.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.308586 akshare-1.9.95/akshare/
--rw-r--r--   0 runner    (1001) docker     (123)   154203 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.308586 akshare-1.9.95/akshare/air/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/air/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/air/air_hebei.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/air/air_zhenqi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/air/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/air/crypto.js
--rw-r--r--   0 runner    (1001) docker     (123)   142353 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/air/outcrypto.js
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/air/sunrise_tad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.308586 akshare-1.9.95/akshare/article/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/article/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/article/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/article/epu_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/article/ff_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/article/fred_md.py
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/article/risk_rv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.308586 akshare-1.9.95/akshare/bank/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bank/bank_cbirc_2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bank/cons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.308586 akshare-1.9.95/akshare/bond/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_cb_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_cbond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_china_money.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_info_cm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_issue_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    23003 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_zh_cov_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/bond_zh_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/china_bond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/china_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/bond/cons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.308586 akshare-1.9.95/akshare/cost/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/cost/cost_living.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.312586 akshare-1.9.95/akshare/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/crypto/crypto_bitcoin_cme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/crypto/crypto_crix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/crypto/crypto_hist_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/crypto/crypto_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.312586 akshare-1.9.95/akshare/currency/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/currency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/currency/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/currency/currency_china_bank_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/currency/currency_safe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.312586 akshare-1.9.95/akshare/data/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   209327 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/data/covid.js
--rw-r--r--   0 runner    (1001) docker     (123)   122225 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/data/crypto_info.zip
--rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/data/ths.js
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.316586 akshare-1.9.95/akshare/economic/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_australia.py
--rw-r--r--   0 runner    (1001) docker     (123)    31987 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_canada.py
--rw-r--r--   0 runner    (1001) docker     (123)   181370 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_china.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_china_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_constitute.py
--rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_euro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_germany.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_japan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_swiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_uk.py
--rw-r--r--   0 runner    (1001) docker     (123)   121733 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/macro_usa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/economic/marco_cnbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.316586 akshare-1.9.95/akshare/energy/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/energy/energy_carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/energy/energy_oil_em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.316586 akshare-1.9.95/akshare/event/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/event/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    38159 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/event/covid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.316586 akshare-1.9.95/akshare/file_fold/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/file_fold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   112983 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/file_fold/calendar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.316586 akshare-1.9.95/akshare/fortune/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fortune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fortune/fortune_500.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fortune/fortune_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fortune/fortune_forbes_500.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fortune/fortune_hurun.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fortune/fortune_it_juzi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fortune/fortune_xincaifu_500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.320586 akshare-1.9.95/akshare/fund/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31203 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_amac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_aum_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    40604 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_etf_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_etf_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_fhsp_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_init_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_portfolio_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_position_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_rank_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_rating.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_report_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_scale_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fund/fund_scale_sina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.320586 akshare-1.9.95/akshare/futures/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    48979 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_comex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_comm_qihuo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_contract_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_daily_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_foreign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_hq_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_index_ccidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_international.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_inventory_99.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_inventory_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_news_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_news_shmet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_roll_yield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_sgx_daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_spot_stock_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_to_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_warehouse_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/futures_zh_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/inventory_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/requests_fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures/symbol_var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.324586 akshare-1.9.95/akshare/futures_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/futures_egg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/futures_hog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/futures_index_price_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/futures_index_return_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/futures_index_volatility_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/futures_other_index_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/futures_sina_cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/sina_futures_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/futures_derivative/sys_spot_futures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.324586 akshare-1.9.95/akshare/fx/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fx/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fx/currency_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fx/fx_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/fx/fx_quote_baidu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.324586 akshare-1.9.95/akshare/hf/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/hf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/hf/hf_sp500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.328586 akshare-1.9.95/akshare/index/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/dailydata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/drewry_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    53902 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_cflp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_cni.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_eri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_hog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_kq_fz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_kq_ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_stock_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_stock_zh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)    28826 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_sw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_sw_research.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_weibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_yw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/index_zh_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/index/stock_zh_index_csindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.328586 akshare-1.9.95/akshare/interest_rate/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/interest_rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/interest_rate/interbank_rate_em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.328586 akshare-1.9.95/akshare/movie/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/movie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/movie/artist_yien.py
--rw-r--r--   0 runner    (1001) docker     (123)   117172 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/movie/jm.js
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/movie/movie_yien.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/movie/video_yien.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.328586 akshare-1.9.95/akshare/news/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/news/news_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/news/news_cctv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/news/news_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.328586 akshare-1.9.95/akshare/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/nlp/nlp_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/option/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_commodity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_commodity_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_czce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_finance.py
--rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_finance_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_lhb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_premium_analysis_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_qvix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_risk_analysis_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_risk_indicator_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/option/option_value_analysis_em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/other/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/other/other_car.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/other/other_game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/pro/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/pro/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/pro/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/pro/data_pro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/qhkc/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/qhkc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/qhkc/qhkc_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/qhkc_web/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/qhkc_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/qhkc_web/qhkc_fund.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/qhkc_web/qhkc_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/qhkc_web/qhkc_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/rate/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/rate/repo_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/reits/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/reits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/reits/reits_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/sport/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/sport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/sport/sport_olympic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/sport/sport_olympic_winter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.332586 akshare-1.9.95/akshare/spot/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/spot/spot_sge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.340587 akshare-1.9.95/akshare/stock/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_allotment_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_ask_bid_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_board_concept_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_board_industry_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_cg_equity_mortgage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_cg_guarantee.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_cg_lawsuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_dividents_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_dzjy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_fund_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_fund_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_hk_fhpx_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_hk_hot_rank_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_hk_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_hold_control_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_hold_num_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_hot_rank_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_hot_search_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_industry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_industry_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_industry_pe_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_info_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_new_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_profile_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_rank_forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_repurchase_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_share_changes_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)    22524 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_us_famous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_us_js.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_us_pink.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_us_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_us_zh_hx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_weibo_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_zh_a_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_zh_a_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_zh_a_tick_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_zh_ah_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_zh_b_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_zh_kcb_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock/stock_zh_kcb_sina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.344586 akshare-1.9.95/akshare/stock_feature/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_a_below_net_asset_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_a_high_low.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_a_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_a_pe_and_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_account_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_all_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_analyst_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_average_position_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_board_concept_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_board_industry_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_buffett_index_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_classify_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_cls_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_cninfo_yjyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_comment_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_congestion_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_dxsyl_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_ebs_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_fhps_em.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_fhps_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_fund_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_gdfx_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_gdhs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_gdzjc_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_gpzy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_gxl_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    66460 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_hist_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_hk_valuation_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_hot_tgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_hot_xq.py
--rw-r--r--   0 runner    (1001) docker     (123)    66045 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_hsgt_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_hsgt_exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_inner_trade_xq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_jgdy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_lh_yybpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_lhb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_lhb_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_market_legu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_pankou_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_qsjy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_report_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_sse_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_sy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_szse_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_technology_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_tfp_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_three_report_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_ttm_lyr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_us_hist_futunn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_wencai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_yjbb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_yjyg_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_yzxdr_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_zf_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_zh_valuation_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_zh_vote_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/stock_ztb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_feature/ths.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.344586 akshare-1.9.95/akshare/stock_fundamental/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26766 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_finance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_finance_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_finance_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_ipo_declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_kcb_detail_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_kcb_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_mda_ym.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_notice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_profit_forecast_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_profit_forecast_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_recommend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_register.py
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_restricted_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_zygc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/stock_fundamental/stock_zyjs_ths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.348586 akshare-1.9.95/akshare/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/tool/trade_date_hist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.348586 akshare-1.9.95/akshare/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   241609 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/utils/demjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 15:46:27.000000 akshare-1.9.95/akshare/utils/token_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.308586 akshare-1.9.95/akshare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-25 15:46:40.000000 akshare-1.9.95/akshare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-05-25 15:46:40.000000 akshare-1.9.95/akshare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:46:40.000000 akshare-1.9.95/akshare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-25 15:46:40.000000 akshare-1.9.95/akshare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 15:46:40.000000 akshare-1.9.95/akshare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-25 15:46:27.000000 akshare-1.9.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:46:40.348586 akshare-1.9.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-25 15:46:27.000000 akshare-1.9.95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:46:40.348586 akshare-1.9.95/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-25 15:46:27.000000 akshare-1.9.95/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-25 15:46:27.000000 akshare-1.9.95/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.088326 akshare-1.9.96/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-26 12:48:11.000000 akshare-1.9.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-26 12:48:20.088326 akshare-1.9.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-26 12:48:11.000000 akshare-1.9.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.048325 akshare-1.9.96/akshare/
+-rw-r--r--   0 runner    (1001) docker     (123)   154255 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.052325 akshare-1.9.96/akshare/air/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/air/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/air/air_hebei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/air/air_zhenqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/air/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/air/crypto.js
+-rw-r--r--   0 runner    (1001) docker     (123)   142353 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/air/outcrypto.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/air/sunrise_tad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.052325 akshare-1.9.96/akshare/article/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/article/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/article/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/article/epu_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/article/ff_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/article/fred_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/article/risk_rv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.052325 akshare-1.9.96/akshare/bank/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bank/bank_cbirc_2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bank/cons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.052325 akshare-1.9.96/akshare/bond/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_cb_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_cbond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_china_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_info_cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_issue_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23003 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_zh_cov_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/bond_zh_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/china_bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/china_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/bond/cons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.052325 akshare-1.9.96/akshare/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/cost/cost_living.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.056325 akshare-1.9.96/akshare/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/crypto/crypto_bitcoin_cme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/crypto/crypto_crix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/crypto/crypto_hist_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/crypto/crypto_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.056325 akshare-1.9.96/akshare/currency/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/currency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/currency/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/currency/currency_china_bank_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/currency/currency_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.056325 akshare-1.9.96/akshare/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209327 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/data/covid.js
+-rw-r--r--   0 runner    (1001) docker     (123)   122225 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/data/crypto_info.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/data/ths.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.056325 akshare-1.9.96/akshare/economic/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_australia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31987 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_canada.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181370 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_china.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_china_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_constitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_euro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_germany.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_japan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_swiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_uk.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121733 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/macro_usa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/economic/marco_cnbs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.056325 akshare-1.9.96/akshare/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/energy/energy_carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/energy/energy_oil_em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.060325 akshare-1.9.96/akshare/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/event/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38159 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/event/covid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.060325 akshare-1.9.96/akshare/file_fold/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/file_fold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112983 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/file_fold/calendar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.060325 akshare-1.9.96/akshare/fortune/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fortune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fortune/fortune_500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fortune/fortune_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fortune/fortune_forbes_500.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fortune/fortune_hurun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fortune/fortune_it_juzi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fortune/fortune_xincaifu_500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.060325 akshare-1.9.96/akshare/fund/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31203 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_amac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_aum_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40604 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_etf_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_etf_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_fhsp_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_init_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_portfolio_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_position_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_rank_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_report_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_scale_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fund/fund_scale_sina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.064325 akshare-1.9.96/akshare/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48979 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_comex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_comm_qihuo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_contract_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_daily_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_hq_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_index_ccidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_international.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_inventory_99.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_inventory_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_news_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_news_shmet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_roll_yield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_sgx_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_spot_stock_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_to_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_warehouse_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/futures_zh_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/inventory_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/requests_fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures/symbol_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.064325 akshare-1.9.96/akshare/futures_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/futures_egg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/futures_hog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/futures_index_price_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/futures_index_return_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/futures_index_volatility_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/futures_other_index_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/futures_sina_cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/sina_futures_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/futures_derivative/sys_spot_futures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.064325 akshare-1.9.96/akshare/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fx/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fx/currency_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fx/fx_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/fx/fx_quote_baidu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.064325 akshare-1.9.96/akshare/hf/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/hf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/hf/hf_sp500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.068325 akshare-1.9.96/akshare/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/dailydata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/drewry_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53902 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_cflp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_cni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_eri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_hog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_kq_fz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_kq_ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_stock_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_stock_zh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28826 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_sw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_sw_research.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_weibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_yw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/index_zh_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/index/stock_zh_index_csindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.068325 akshare-1.9.96/akshare/interest_rate/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/interest_rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/interest_rate/interbank_rate_em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.068325 akshare-1.9.96/akshare/movie/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/movie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/movie/artist_yien.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117172 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/movie/jm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/movie/movie_yien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/movie/video_yien.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.068325 akshare-1.9.96/akshare/news/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/news/news_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/news/news_cctv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/news/news_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/nlp/nlp_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/option/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20225 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_commodity_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_czce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_finance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_finance_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_lhb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_premium_analysis_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_qvix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_risk_analysis_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_risk_indicator_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/option/option_value_analysis_em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/other/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/other/other_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/other/other_game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/pro/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/pro/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/pro/data_pro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/qhkc/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/qhkc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/qhkc/qhkc_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/qhkc_web/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/qhkc_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/qhkc_web/qhkc_fund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/qhkc_web/qhkc_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/qhkc_web/qhkc_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/rate/repo_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/reits/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/reits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/reits/reits_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/sport/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/sport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/sport/sport_olympic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/sport/sport_olympic_winter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.072325 akshare-1.9.96/akshare/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/spot/spot_sge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.080326 akshare-1.9.96/akshare/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_allotment_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_ask_bid_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_board_concept_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_board_industry_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_cg_equity_mortgage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_cg_guarantee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_cg_lawsuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_dividents_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_dzjy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42905 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_fund_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_fund_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_hk_fhpx_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_hk_hot_rank_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_hk_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)   214887 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_hold_control_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_hold_num_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_hot_rank_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_hot_search_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_industry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_industry_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_industry_pe_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_info_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_new_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   211181 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_profile_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_rank_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_repurchase_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_share_changes_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22524 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_us_famous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_us_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_us_pink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_us_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_us_zh_hx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_weibo_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_zh_a_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_zh_a_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_zh_a_tick_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_zh_ah_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_zh_b_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_zh_kcb_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock/stock_zh_kcb_sina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.084326 akshare-1.9.96/akshare/stock_feature/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_a_below_net_asset_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_a_high_low.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_a_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_a_pe_and_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_account_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_all_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_analyst_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_average_position_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_board_concept_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_board_industry_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_buffett_index_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_classify_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_cls_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_cninfo_yjyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_comment_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_congestion_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_dxsyl_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_ebs_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_fhps_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_fhps_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_fund_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_gdfx_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_gdhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_gdzjc_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_gpzy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_gxl_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66460 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_hist_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_hk_valuation_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_hot_tgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_hot_xq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66045 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_hsgt_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_hsgt_exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_inner_trade_xq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_jgdy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_lh_yybpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_lhb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_lhb_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_market_legu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_pankou_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_qsjy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_report_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_sse_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_sy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_szse_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_technology_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_tfp_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_three_report_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_ttm_lyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_us_hist_futunn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_wencai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_yjbb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_yjyg_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_yzxdr_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_zf_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_zh_valuation_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_zh_vote_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/stock_ztb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_feature/ths.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.088326 akshare-1.9.96/akshare/stock_fundamental/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26766 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_finance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_finance_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_finance_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_ipo_declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_kcb_detail_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_kcb_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_mda_ym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_profit_forecast_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_profit_forecast_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_recommend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_restricted_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_zygc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/stock_fundamental/stock_zyjs_ths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.088326 akshare-1.9.96/akshare/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/tool/trade_date_hist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.088326 akshare-1.9.96/akshare/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241609 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/utils/demjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 12:48:11.000000 akshare-1.9.96/akshare/utils/token_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.052325 akshare-1.9.96/akshare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-26 12:48:19.000000 akshare-1.9.96/akshare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-05-26 12:48:20.000000 akshare-1.9.96/akshare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:48:19.000000 akshare-1.9.96/akshare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-26 12:48:19.000000 akshare-1.9.96/akshare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 12:48:19.000000 akshare-1.9.96/akshare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 12:48:11.000000 akshare-1.9.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 12:48:20.088326 akshare-1.9.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-26 12:48:11.000000 akshare-1.9.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:48:20.088326 akshare-1.9.96/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 12:48:11.000000 akshare-1.9.96/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-26 12:48:11.000000 akshare-1.9.96/tests/test_func.py
```

### Comparing `akshare-1.9.95/LICENSE` & `akshare-1.9.96/LICENSE`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/PKG-INFO` & `akshare-1.9.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akshare
-Version: 1.9.95
+Version: 1.9.96
 Summary: AKShare is an elegant and simple financial data interface library for Python, built for human beings!
 Home-page: https://github.com/akfamily/akshare
 Author: AKFamily
 Author-email: akfamily.akshare@gmail.com
 License: MIT
 Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `akshare-1.9.95/README.md` & `akshare-1.9.96/README.md`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/__init__.py` & `akshare-1.9.96/akshare/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2407,17 +2407,18 @@
 1.9.89 fix: fix index_kq_fz interface
 1.9.90 fix: fix stock_sse_deal_daily interface
 1.9.91 add: add stock_financial_abstract_ths interface
 1.9.92 fix: fix article_ff_crr interface
 1.9.93 fix: fix index_level_one_hist_sw interface
 1.9.94 fix: fix stock_a_indicator_lg interface
 1.9.95 fix: fix stock_zh_index_hist_csindex interface
+1.9.96 fix: fix stock_hold_control_cninfo interface
 """
 
-__version__ = "1.9.95"
+__version__ = "1.9.96"
 __author__ = "AKFamily"
 
 import sys
 import warnings
 
 if sys.version_info < (3, 8):
     warnings.warn("为了支持更多 AKShare 特性，请尽快升级 Python 到 3.8 以上版本")
```

### Comparing `akshare-1.9.95/akshare/air/air_hebei.py` & `akshare-1.9.96/akshare/air/air_hebei.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/air/air_zhenqi.py` & `akshare-1.9.96/akshare/air/air_zhenqi.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/air/cons.py` & `akshare-1.9.96/akshare/air/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/air/crypto.js` & `akshare-1.9.96/akshare/air/crypto.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/air/outcrypto.js` & `akshare-1.9.96/akshare/air/outcrypto.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/air/sunrise_tad.py` & `akshare-1.9.96/akshare/air/sunrise_tad.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/article/epu_index.py` & `akshare-1.9.96/akshare/article/epu_index.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/article/ff_factor.py` & `akshare-1.9.96/akshare/article/ff_factor.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/article/fred_md.py` & `akshare-1.9.96/akshare/article/fred_md.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/article/risk_rv.py` & `akshare-1.9.96/akshare/article/risk_rv.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bank/bank_cbirc_2020.py` & `akshare-1.9.96/akshare/bank/bank_cbirc_2020.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bank/cons.py` & `akshare-1.9.96/akshare/bank/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_bank.py` & `akshare-1.9.96/akshare/bond/bond_bank.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_cb_ths.py` & `akshare-1.9.96/akshare/bond/bond_cb_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_cbond.py` & `akshare-1.9.96/akshare/bond/bond_cbond.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_china_money.py` & `akshare-1.9.96/akshare/bond/bond_china_money.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_convert.py` & `akshare-1.9.96/akshare/bond/bond_convert.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_em.py` & `akshare-1.9.96/akshare/bond/bond_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_futures.py` & `akshare-1.9.96/akshare/bond/bond_futures.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_info_cm.py` & `akshare-1.9.96/akshare/bond/bond_info_cm.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_investing.py` & `akshare-1.9.96/akshare/bond/bond_investing.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_issue_cninfo.py` & `akshare-1.9.96/akshare/bond/bond_issue_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_summary.py` & `akshare-1.9.96/akshare/bond/bond_summary.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_zh_cov_sina.py` & `akshare-1.9.96/akshare/bond/bond_zh_cov_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/bond_zh_sina.py` & `akshare-1.9.96/akshare/bond/bond_zh_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/china_bond.py` & `akshare-1.9.96/akshare/bond/china_bond.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/china_repo.py` & `akshare-1.9.96/akshare/bond/china_repo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/bond/cons.py` & `akshare-1.9.96/akshare/bond/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/cost/cost_living.py` & `akshare-1.9.96/akshare/cost/cost_living.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/crypto/crypto_bitcoin_cme.py` & `akshare-1.9.96/akshare/crypto/crypto_bitcoin_cme.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/crypto/crypto_crix.py` & `akshare-1.9.96/akshare/crypto/crypto_crix.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/crypto/crypto_hist_investing.py` & `akshare-1.9.96/akshare/crypto/crypto_hist_investing.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/crypto/crypto_hold.py` & `akshare-1.9.96/akshare/crypto/crypto_hold.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/currency/currency.py` & `akshare-1.9.96/akshare/currency/currency.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/currency/currency_china_bank_sina.py` & `akshare-1.9.96/akshare/currency/currency_china_bank_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/currency/currency_safe.py` & `akshare-1.9.96/akshare/currency/currency_safe.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/data/covid.js` & `akshare-1.9.96/akshare/data/covid.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/data/crypto_info.zip` & `akshare-1.9.96/akshare/data/crypto_info.zip`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/data/ths.js` & `akshare-1.9.96/akshare/data/ths.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/datasets.py` & `akshare-1.9.96/akshare/datasets.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/cons.py` & `akshare-1.9.96/akshare/economic/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_australia.py` & `akshare-1.9.96/akshare/economic/macro_australia.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_bank.py` & `akshare-1.9.96/akshare/economic/macro_bank.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_canada.py` & `akshare-1.9.96/akshare/economic/macro_canada.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_china.py` & `akshare-1.9.96/akshare/economic/macro_china.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_china_hk.py` & `akshare-1.9.96/akshare/economic/macro_china_hk.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_constitute.py` & `akshare-1.9.96/akshare/economic/macro_constitute.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_euro.py` & `akshare-1.9.96/akshare/economic/macro_euro.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_germany.py` & `akshare-1.9.96/akshare/economic/macro_germany.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_japan.py` & `akshare-1.9.96/akshare/economic/macro_japan.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_other.py` & `akshare-1.9.96/akshare/economic/macro_other.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_swiss.py` & `akshare-1.9.96/akshare/economic/macro_swiss.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_uk.py` & `akshare-1.9.96/akshare/economic/macro_uk.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/macro_usa.py` & `akshare-1.9.96/akshare/economic/macro_usa.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/economic/marco_cnbs.py` & `akshare-1.9.96/akshare/economic/marco_cnbs.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/energy/energy_carbon.py` & `akshare-1.9.96/akshare/energy/energy_carbon.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/energy/energy_oil_em.py` & `akshare-1.9.96/akshare/energy/energy_oil_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/event/cons.py` & `akshare-1.9.96/akshare/event/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/event/covid.py` & `akshare-1.9.96/akshare/event/covid.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/file_fold/calendar.json` & `akshare-1.9.96/akshare/file_fold/calendar.json`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fortune/fortune_500.py` & `akshare-1.9.96/akshare/fortune/fortune_500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fortune/fortune_bloomberg.py` & `akshare-1.9.96/akshare/fortune/fortune_bloomberg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fortune/fortune_forbes_500.py` & `akshare-1.9.96/akshare/fortune/fortune_forbes_500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fortune/fortune_hurun.py` & `akshare-1.9.96/akshare/fortune/fortune_hurun.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fortune/fortune_it_juzi.py` & `akshare-1.9.96/akshare/fortune/fortune_it_juzi.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fortune/fortune_xincaifu_500.py` & `akshare-1.9.96/akshare/fortune/fortune_xincaifu_500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_amac.py` & `akshare-1.9.96/akshare/fund/fund_amac.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_aum_em.py` & `akshare-1.9.96/akshare/fund/fund_aum_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_em.py` & `akshare-1.9.96/akshare/fund/fund_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_etf_em.py` & `akshare-1.9.96/akshare/fund/fund_etf_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_etf_sina.py` & `akshare-1.9.96/akshare/fund/fund_etf_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_fhsp_em.py` & `akshare-1.9.96/akshare/fund/fund_fhsp_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_init_em.py` & `akshare-1.9.96/akshare/fund/fund_init_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_manager.py` & `akshare-1.9.96/akshare/fund/fund_manager.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_portfolio_em.py` & `akshare-1.9.96/akshare/fund/fund_portfolio_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_position_lg.py` & `akshare-1.9.96/akshare/fund/fund_position_lg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_rank_em.py` & `akshare-1.9.96/akshare/fund/fund_rank_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_rating.py` & `akshare-1.9.96/akshare/fund/fund_rating.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_report_cninfo.py` & `akshare-1.9.96/akshare/fund/fund_report_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_scale_em.py` & `akshare-1.9.96/akshare/fund/fund_scale_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fund/fund_scale_sina.py` & `akshare-1.9.96/akshare/fund/fund_scale_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/cons.py` & `akshare-1.9.96/akshare/futures/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/cot.py` & `akshare-1.9.96/akshare/futures/cot.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_basis.py` & `akshare-1.9.96/akshare/futures/futures_basis.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_comex.py` & `akshare-1.9.96/akshare/futures/futures_comex.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_comm_qihuo.py` & `akshare-1.9.96/akshare/futures/futures_comm_qihuo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_contract_detail.py` & `akshare-1.9.96/akshare/futures/futures_contract_detail.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_daily_bar.py` & `akshare-1.9.96/akshare/futures/futures_daily_bar.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_foreign.py` & `akshare-1.9.96/akshare/futures/futures_foreign.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_hq_sina.py` & `akshare-1.9.96/akshare/futures/futures_hq_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_index_ccidx.py` & `akshare-1.9.96/akshare/futures/futures_index_ccidx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_international.py` & `akshare-1.9.96/akshare/futures/futures_international.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_inventory_99.py` & `akshare-1.9.96/akshare/futures/futures_inventory_99.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_inventory_em.py` & `akshare-1.9.96/akshare/futures/futures_inventory_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_news_baidu.py` & `akshare-1.9.96/akshare/futures/futures_news_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_news_shmet.py` & `akshare-1.9.96/akshare/futures/futures_news_shmet.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_roll_yield.py` & `akshare-1.9.96/akshare/futures/futures_roll_yield.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_rule.py` & `akshare-1.9.96/akshare/futures/futures_rule.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_sgx_daily.py` & `akshare-1.9.96/akshare/futures/futures_sgx_daily.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_spot_stock_em.py` & `akshare-1.9.96/akshare/futures/futures_spot_stock_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_to_spot.py` & `akshare-1.9.96/akshare/futures/futures_to_spot.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_warehouse_receipt.py` & `akshare-1.9.96/akshare/futures/futures_warehouse_receipt.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/futures_zh_sina.py` & `akshare-1.9.96/akshare/futures/futures_zh_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/inventory_data.py` & `akshare-1.9.96/akshare/futures/inventory_data.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/receipt.py` & `akshare-1.9.96/akshare/futures/receipt.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/requests_fun.py` & `akshare-1.9.96/akshare/futures/requests_fun.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures/symbol_var.py` & `akshare-1.9.96/akshare/futures/symbol_var.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/cons.py` & `akshare-1.9.96/akshare/futures_derivative/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/futures_egg.py` & `akshare-1.9.96/akshare/futures_derivative/futures_egg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/futures_hog.py` & `akshare-1.9.96/akshare/futures_derivative/futures_hog.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/futures_index_price_nh.py` & `akshare-1.9.96/akshare/futures_derivative/futures_index_price_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/futures_index_return_nh.py` & `akshare-1.9.96/akshare/futures_derivative/futures_index_return_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/futures_index_volatility_nh.py` & `akshare-1.9.96/akshare/futures_derivative/futures_index_volatility_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/futures_other_index_nh.py` & `akshare-1.9.96/akshare/futures_derivative/futures_other_index_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/futures_sina_cot.py` & `akshare-1.9.96/akshare/futures_derivative/futures_sina_cot.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/sina_futures_index.py` & `akshare-1.9.96/akshare/futures_derivative/sina_futures_index.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/futures_derivative/sys_spot_futures.py` & `akshare-1.9.96/akshare/futures_derivative/sys_spot_futures.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fx/cons.py` & `akshare-1.9.96/akshare/fx/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fx/currency_investing.py` & `akshare-1.9.96/akshare/fx/currency_investing.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fx/fx_quote.py` & `akshare-1.9.96/akshare/fx/fx_quote.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/fx/fx_quote_baidu.py` & `akshare-1.9.96/akshare/fx/fx_quote_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/hf/hf_sp500.py` & `akshare-1.9.96/akshare/hf/hf_sp500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/cons.py` & `akshare-1.9.96/akshare/index/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/dailydata.py` & `akshare-1.9.96/akshare/index/dailydata.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/drewry_index.py` & `akshare-1.9.96/akshare/index/drewry_index.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_baidu.py` & `akshare-1.9.96/akshare/index/index_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_cflp.py` & `akshare-1.9.96/akshare/index/index_cflp.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_cni.py` & `akshare-1.9.96/akshare/index/index_cni.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_cons.py` & `akshare-1.9.96/akshare/index/index_cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_cx.py` & `akshare-1.9.96/akshare/index/index_cx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_eri.py` & `akshare-1.9.96/akshare/index/index_eri.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_google.py` & `akshare-1.9.96/akshare/index/index_google.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_hog.py` & `akshare-1.9.96/akshare/index/index_hog.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_investing.py` & `akshare-1.9.96/akshare/index/index_investing.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_kq_fz.py` & `akshare-1.9.96/akshare/index/index_kq_fz.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_kq_ss.py` & `akshare-1.9.96/akshare/index/index_kq_ss.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_spot.py` & `akshare-1.9.96/akshare/index/index_spot.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_stock_hk.py` & `akshare-1.9.96/akshare/index/index_stock_hk.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_stock_zh.py` & `akshare-1.9.96/akshare/index/index_stock_zh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_sugar.py` & `akshare-1.9.96/akshare/index/index_sugar.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_sw.py` & `akshare-1.9.96/akshare/index/index_sw.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_sw_research.py` & `akshare-1.9.96/akshare/index/index_sw_research.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_weibo.py` & `akshare-1.9.96/akshare/index/index_weibo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_yw.py` & `akshare-1.9.96/akshare/index/index_yw.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/index_zh_em.py` & `akshare-1.9.96/akshare/index/index_zh_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/request.py` & `akshare-1.9.96/akshare/index/request.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/index/stock_zh_index_csindex.py` & `akshare-1.9.96/akshare/index/stock_zh_index_csindex.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/interest_rate/interbank_rate_em.py` & `akshare-1.9.96/akshare/interest_rate/interbank_rate_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/movie/artist_yien.py` & `akshare-1.9.96/akshare/movie/artist_yien.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/movie/jm.js` & `akshare-1.9.96/akshare/movie/jm.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/movie/movie_yien.py` & `akshare-1.9.96/akshare/movie/movie_yien.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/movie/video_yien.py` & `akshare-1.9.96/akshare/movie/video_yien.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/news/news_baidu.py` & `akshare-1.9.96/akshare/news/news_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/news/news_cctv.py` & `akshare-1.9.96/akshare/news/news_cctv.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/news/news_stock.py` & `akshare-1.9.96/akshare/news/news_stock.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/nlp/nlp_interface.py` & `akshare-1.9.96/akshare/nlp/nlp_interface.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/cons.py` & `akshare-1.9.96/akshare/option/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_commodity.py` & `akshare-1.9.96/akshare/option/option_commodity.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_commodity_sina.py` & `akshare-1.9.96/akshare/option/option_commodity_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_czce.py` & `akshare-1.9.96/akshare/option/option_czce.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_em.py` & `akshare-1.9.96/akshare/option/option_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_finance.py` & `akshare-1.9.96/akshare/option/option_finance.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_finance_sina.py` & `akshare-1.9.96/akshare/option/option_finance_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_lhb_em.py` & `akshare-1.9.96/akshare/option/option_lhb_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_premium_analysis_em.py` & `akshare-1.9.96/akshare/option/option_premium_analysis_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_qvix.py` & `akshare-1.9.96/akshare/option/option_qvix.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_risk_analysis_em.py` & `akshare-1.9.96/akshare/option/option_risk_analysis_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_risk_indicator_sse.py` & `akshare-1.9.96/akshare/option/option_risk_indicator_sse.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/option/option_value_analysis_em.py` & `akshare-1.9.96/akshare/option/option_value_analysis_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/other/other_car.py` & `akshare-1.9.96/akshare/other/other_car.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/other/other_game.py` & `akshare-1.9.96/akshare/other/other_game.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/pro/client.py` & `akshare-1.9.96/akshare/pro/client.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/pro/data_pro.py` & `akshare-1.9.96/akshare/pro/data_pro.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/qhkc/qhkc_api.py` & `akshare-1.9.96/akshare/qhkc/qhkc_api.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/qhkc_web/qhkc_fund.py` & `akshare-1.9.96/akshare/qhkc_web/qhkc_fund.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/qhkc_web/qhkc_index.py` & `akshare-1.9.96/akshare/qhkc_web/qhkc_index.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/qhkc_web/qhkc_tool.py` & `akshare-1.9.96/akshare/qhkc_web/qhkc_tool.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/rate/repo_rate.py` & `akshare-1.9.96/akshare/rate/repo_rate.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/reits/reits_basic.py` & `akshare-1.9.96/akshare/reits/reits_basic.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/sport/sport_olympic.py` & `akshare-1.9.96/akshare/sport/sport_olympic.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/sport/sport_olympic_winter.py` & `akshare-1.9.96/akshare/sport/sport_olympic_winter.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/spot/spot_sge.py` & `akshare-1.9.96/akshare/spot/spot_sge.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/cons.py` & `akshare-1.9.96/akshare/stock/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_allotment_cninfo.py` & `akshare-1.9.96/akshare/stock/stock_allotment_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_ask_bid_em.py` & `akshare-1.9.96/akshare/stock/stock_ask_bid_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_board_concept_em.py` & `akshare-1.9.96/akshare/stock/stock_board_concept_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_board_industry_em.py` & `akshare-1.9.96/akshare/stock/stock_board_industry_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_cg_equity_mortgage.py` & `akshare-1.9.96/akshare/stock/stock_cg_equity_mortgage.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_cg_guarantee.py` & `akshare-1.9.96/akshare/stock/stock_cg_guarantee.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_cg_lawsuit.py` & `akshare-1.9.96/akshare/stock/stock_cg_lawsuit.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_dividents_cninfo.py` & `akshare-1.9.96/akshare/stock/stock_dividents_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_dzjy_em.py` & `akshare-1.9.96/akshare/stock/stock_dzjy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_fund_em.py` & `akshare-1.9.96/akshare/stock/stock_fund_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_fund_hold.py` & `akshare-1.9.96/akshare/stock/stock_fund_hold.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_hk_fhpx_ths.py` & `akshare-1.9.96/akshare/stock/stock_hk_fhpx_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_hk_hot_rank_em.py` & `akshare-1.9.96/akshare/stock/stock_hk_hot_rank_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_hk_sina.py` & `akshare-1.9.96/akshare/stock/stock_hk_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_hold_control_cninfo.py` & `akshare-1.9.96/akshare/stock/stock_industry_cninfo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-#!/usr/bin/env python
 # -*- coding:utf-8 -*-
+# !/usr/bin/env python
 """
-Date: 2021/9/22 15:59
-Desc: 巨潮资讯-数据中心-专题统计-股东股本-实际控制人持股变动
-http://webapi.cninfo.com.cn/#/thematicStatistics
-
-巨潮资讯-数据中心-专题统计-股东股本-高管持股变动明细
-http://webapi.cninfo.com.cn/#/thematicStatistics
+Date: 2022/7/13 15:34
+Desc: 巨潮资讯-行业分类数据
+http://webapi.cninfo.com.cn/#/apiDoc
+http://webapi.cninfo.com.cn/api/stock/p_stock2110
 """
 import time
-import datetime
 
+import numpy as np
 import pandas as pd
 import requests
 from py_mini_racer import py_mini_racer
 
 js_str = """
-    function mcode(input) {  
-                var keyStr = "ABCDEFGHIJKLMNOP" + "QRSTUVWXYZabcdef" + "ghijklmnopqrstuv"   + "wxyz0123456789+/" + "=";  
-                var output = "";  
-                var chr1, chr2, chr3 = "";  
-                var enc1, enc2, enc3, enc4 = "";  
-                var i = 0;  
-                do {  
-                    chr1 = input.charCodeAt(i++);  
-                    chr2 = input.charCodeAt(i++);  
-                    chr3 = input.charCodeAt(i++);  
-                    enc1 = chr1 >> 2;  
-                    enc2 = ((chr1 & 3) << 4) | (chr2 >> 4);  
-                    enc3 = ((chr2 & 15) << 2) | (chr3 >> 6);  
-                    enc4 = chr3 & 63;  
-                    if (isNaN(chr2)) {  
-                        enc3 = enc4 = 64;  
-                    } else if (isNaN(chr3)) {  
-                        enc4 = 64;  
-                    }  
-                    output = output + keyStr.charAt(enc1) + keyStr.charAt(enc2)  
-                            + keyStr.charAt(enc3) + keyStr.charAt(enc4);  
-                    chr1 = chr2 = chr3 = "";  
-                    enc1 = enc2 = enc3 = enc4 = "";  
-                } while (i < input.length);  
-          
-                return output;  
-            }  
+    function mcode(input) {
+                var keyStr = "ABCDEFGHIJKLMNOP" + "QRSTUVWXYZabcdef" + "ghijklmnopqrstuv"   + "wxyz0123456789+/" + "=";
+                var output = "";
+                var chr1, chr2, chr3 = "";
+                var enc1, enc2, enc3, enc4 = "";
+                var i = 0;
+                do {
+                    chr1 = input.charCodeAt(i++);
+                    chr2 = input.charCodeAt(i++);
+                    chr3 = input.charCodeAt(i++);
+                    enc1 = chr1 >> 2;
+                    enc2 = ((chr1 & 3) << 4) | (chr2 >> 4);
+                    enc3 = ((chr2 & 15) << 2) | (chr3 >> 6);
+                    enc4 = chr3 & 63;
+                    if (isNaN(chr2)) {
+                        enc3 = enc4 = 64;
+                    } else if (isNaN(chr3)) {
+                        enc4 = 64;
+                    }
+                    output = output + keyStr.charAt(enc1) + keyStr.charAt(enc2)
+                            + keyStr.charAt(enc3) + keyStr.charAt(enc4);
+                    chr1 = chr2 = chr3 = "";
+                    enc1 = enc2 = enc3 = enc4 = "";
+                } while (i < input.length);
+
+                return output;
+            }
 """
 
 
-def stock_hold_control_cninfo(symbol: str = "全部") -> pd.DataFrame:
+def stock_industry_category_cninfo(symbol: str = "巨潮行业分类标准") -> pd.DataFrame:
     """
-    巨潮资讯-数据中心-专题统计-股东股本-实际控制人持股变动
-    http://webapi.cninfo.com.cn/#/thematicStatistics
-    :param symbol: choice of {"单独控制", "实际控制人", "一致行动人", "家族控制", "全部"}; 从 2010 开始
+    巨潮资讯-行业分类数据
+    http://webapi.cninfo.com.cn/#/apiDoc
+    查询 p_public0002 接口
+    :param symbol: 行业类型; choice of {"证监会行业分类标准", "巨潮行业分类标准", "申银万国行业分类标准", "新财富行业分类标准", "国资委行业分类标准", "巨潮产业细分标准", "天相行业分类标准", "全球行业分类标准"}
     :type symbol: str
-    :return: 实际控制人持股变动
+    :return: 行业分类数据
     :rtype: pandas.DataFrame
     """
     symbol_map = {
-        "单独控制": "069001",
-        "实际控制人": "069002",
-        "一致行动人": "069003",
-        "家族控制": "069004",
-        "全部": "",
+        "证监会行业分类标准": "008001",
+        "巨潮行业分类标准": "008002",
+        "申银万国行业分类标准": "008003",
+        "新财富行业分类标准": "008004",
+        "国资委行业分类标准": "008005",
+        "巨潮产业细分标准": "008006",
+        "天相行业分类标准": "008007",
+        "全球行业分类标准": "008008",
     }
-    url = "http://webapi.cninfo.com.cn/api/sysapi/p_sysapi1033"
+    url = "http://webapi.cninfo.com.cn/api/stock/p_public0002"
+    params = {"indcode": "", "indtype": symbol_map[symbol], "format": "json"}
     random_time_str = str(int(time.time()))
     js_code = py_mini_racer.MiniRacer()
     js_code.eval(js_str)
     mcode = js_code.call("mcode", random_time_str)
     headers = {
         "Accept": "*/*",
         "Accept-Encoding": "gzip, deflate",
@@ -78,63 +81,68 @@
         "Origin": "http://webapi.cninfo.com.cn",
         "Pragma": "no-cache",
         "Proxy-Connection": "keep-alive",
         "Referer": "http://webapi.cninfo.com.cn/",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/93.0.4577.63 Safari/537.36",
         "X-Requested-With": "XMLHttpRequest",
     }
-    params = {
-        "ctype": symbol_map[symbol],
-    }
-    r = requests.post(url, headers=headers, params=params)
+    r = requests.get(url, params=params, headers=headers)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["records"])
-    temp_df.columns = [
-        "控股比例",
-        "控股数量",
-        "证券简称",
-        "实际控制人名称",
-        "直接控制人名称",
-        "控制类型",
-        "证券代码",
-        "变动日期",
-    ]
-    temp_df = temp_df[
-        [
-            "证券代码",
-            "证券简称",
-            "变动日期",
-            "实际控制人名称",
-            "控股数量",
-            "控股比例",
-            "直接控制人名称",
-            "控制类型",
-        ]
-    ]
-    temp_df["变动日期"] = pd.to_datetime(temp_df["变动日期"]).dt.date
-    temp_df["控股数量"] = pd.to_numeric(temp_df["控股数量"])
-    temp_df["控股比例"] = pd.to_numeric(temp_df["控股比例"])
+    cols_map = {
+        "PARENTCODE": "父类编码",
+        "SORTCODE": "类目编码",
+        "SORTNAME": "类目名称",
+        "F001V": "类目名称英文",
+        "F002D": "终止日期",
+        "F003V": "行业类型编码",
+        "F004V": "行业类型",
+    }
+    temp_df.rename(columns=cols_map, inplace=True)
+    # 行业按分级排序
+    tmp = temp_df[["类目编码"]].copy()
+    tmp["len"] = temp_df["类目编码"].str.len()
+    tmp["Level"] = 0
+    g = tmp.groupby("len")
+    level = 0
+    for k in g.groups.keys():
+        temp_df.loc[
+            temp_df["类目编码"].isin(g.get_group(k)["类目编码"]), "Level"
+        ] = level
+        level += 1
+    temp_df["Level"] = temp_df["Level"].astype(int)
+    temp_df.rename(columns={"Level": "分级"}, inplace=True)
+    temp_df["终止日期"] = pd.to_datetime(temp_df["终止日期"]).dt.date
     return temp_df
 
 
-def stock_hold_management_detail_cninfo(symbol: str = "增持") -> pd.DataFrame:
+def stock_industry_change_cninfo(
+    symbol: str = "002594",
+    start_date: str = "20091227",
+    end_date: str = "20220713",
+) -> pd.DataFrame:
     """
-    巨潮资讯-数据中心-专题统计-股东股本-高管持股变动明细
-    http://webapi.cninfo.com.cn/#/thematicStatistics
-    :param symbol: choice of {"增持", "减持"}
+    巨潮资讯-上市公司行业归属的变动情况
+    http://webapi.cninfo.com.cn/#/apiDoc
+    查询 p_stock2110 接口
+    :param symbol: 股票代码
     :type symbol: str
-    :return: 高管持股变动明细
+    :param start_date: 开始变动日期
+    :type start_date: str
+    :param end_date: 结束变动日期
+    :type end_date: str
+    :return: 行业归属的变动情况
     :rtype: pandas.DataFrame
     """
-    symbol_map = {
-        "增持": "B",
-        "减持": "S",
+    url = "http://webapi.cninfo.com.cn/api/stock/p_stock2110"
+    params = {
+        "scode": symbol,
+        "sdate": "-".join([start_date[:4], start_date[4:6], start_date[6:]]),
+        "edate": "-".join([end_date[:4], end_date[4:6], end_date[6:]]),
     }
-    current_date = datetime.datetime.now().date().isoformat()
-    url = "http://webapi.cninfo.com.cn/api/sysapi/p_sysapi1030"
     random_time_str = str(int(time.time()))
     js_code = py_mini_racer.MiniRacer()
     js_code.eval(js_str)
     mcode = js_code.call("mcode", random_time_str)
     headers = {
         "Accept": "*/*",
         "Accept-Encoding": "gzip, deflate",
@@ -146,70 +154,42 @@
         "Origin": "http://webapi.cninfo.com.cn",
         "Pragma": "no-cache",
         "Proxy-Connection": "keep-alive",
         "Referer": "http://webapi.cninfo.com.cn/",
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/93.0.4577.63 Safari/537.36",
         "X-Requested-With": "XMLHttpRequest",
     }
-    params = {
-        "sdate": str(int(current_date[:4]) - 1) + current_date[4:],
-        "edate": current_date,
-        "varytype": symbol_map[symbol],
-    }
-    r = requests.post(url, headers=headers, params=params)
+    r = requests.post(url, params=params, headers=headers)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["records"])
-    temp_df.columns = [
-        "证券简称",
-        "公告日期",
-        "高管姓名",
-        "期末市值",
-        "成交均价",
-        "证券代码",
-        "变动比例",
-        "变动数量",
-        "截止日期",
-        "期末持股数量",
-        "期初持股数量",
-        "变动人与董监高关系",
-        "董监高职务",
-        "董监高姓名",
-        "数据来源",
-        "持股变动原因",
-    ]
-    temp_df = temp_df[
-        [
-            "证券代码",
-            "证券简称",
-            "截止日期",
-            "公告日期",
-            "高管姓名",
-            "董监高姓名",
-            "董监高职务",
-            "变动人与董监高关系",
-            "期初持股数量",
-            "期末持股数量",
-            "变动数量",
-            "变动比例",
-            "成交均价",
-            "期末市值",
-            "持股变动原因",
-            "数据来源",
-        ]
-    ]
-    temp_df["截止日期"] = pd.to_datetime(temp_df["截止日期"]).dt.date
-    temp_df["公告日期"] = pd.to_datetime(temp_df["公告日期"]).dt.date
-    temp_df["期初持股数量"] = pd.to_numeric(temp_df["期初持股数量"], errors="coerce")
-    temp_df["期末持股数量"] = pd.to_numeric(temp_df["期末持股数量"], errors="coerce")
-    temp_df["变动数量"] = pd.to_numeric(temp_df["变动数量"], errors="coerce")
-    temp_df["变动比例"] = pd.to_numeric(temp_df["变动比例"], errors="coerce")
-    temp_df["成交均价"] = pd.to_numeric(temp_df["成交均价"], errors="coerce")
-    temp_df["期末市值"] = pd.to_numeric(temp_df["期末市值"], errors="coerce")
-    return temp_df
+    cols_map = {
+        "ORGNAME": "机构名称",
+        "SECCODE": "证券代码",
+        "SECNAME": "新证券简称",
+        "VARYDATE": "变更日期",
+        "F001V": "分类标准编码",
+        "F002V": "分类标准",
+        "F003V": "行业编码",
+        "F004V": "行业门类",
+        "F005V": "行业次类",
+        "F006V": "行业大类",
+        "F007V": "行业中类",
+        "F008C": "最新记录标识",
+    }
+    ignore_cols = ["最新记录标识"]
+    temp_df.rename(columns=cols_map, inplace=True)
+    temp_df.fillna(np.nan, inplace=True)
+    temp_df["变更日期"] = pd.to_datetime(temp_df["变更日期"]).dt.date
+    data_df = temp_df[[c for c in temp_df.columns if c not in ignore_cols]]
+    return data_df
 
 
 if __name__ == "__main__":
-    stock_hold_control_cninfo_df = stock_hold_control_cninfo(symbol="全部")
-    print(stock_hold_control_cninfo_df)
-
-    stock_hold_management_detail_cninfo_df = stock_hold_management_detail_cninfo(symbol="增持")
-    print(stock_hold_management_detail_cninfo_df)
+    stock_industry_category_cninfo_df = stock_industry_category_cninfo(
+        symbol="巨潮行业分类标准"
+    )
+    print(stock_industry_category_cninfo_df)
+
+    stock_industry_change_cninfo_df = stock_industry_change_cninfo(
+        symbol="002594", start_date="20091227", end_date="20220708"
+    )
+    print(stock_industry_change_cninfo_df)
```

### Comparing `akshare-1.9.95/akshare/stock/stock_hold_num_cninfo.py` & `akshare-1.9.96/akshare/stock/stock_hold_num_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_hot_rank_em.py` & `akshare-1.9.96/akshare/stock/stock_hot_rank_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_hot_search_baidu.py` & `akshare-1.9.96/akshare/stock/stock_hot_search_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_industry.py` & `akshare-1.9.96/akshare/stock/stock_industry.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_industry_pe_cninfo.py` & `akshare-1.9.96/akshare/stock/stock_industry_pe_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_info.py` & `akshare-1.9.96/akshare/stock/stock_info.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_info_em.py` & `akshare-1.9.96/akshare/stock/stock_info_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_new_cninfo.py` & `akshare-1.9.96/akshare/stock/stock_new_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_rank_forecast.py` & `akshare-1.9.96/akshare/stock/stock_rank_forecast.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_repurchase_em.py` & `akshare-1.9.96/akshare/stock/stock_repurchase_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_share_changes_cninfo.py` & `akshare-1.9.96/akshare/stock/stock_share_changes_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_stop.py` & `akshare-1.9.96/akshare/stock/stock_stop.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_summary.py` & `akshare-1.9.96/akshare/stock/stock_summary.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_us_famous.py` & `akshare-1.9.96/akshare/stock/stock_us_famous.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_us_js.py` & `akshare-1.9.96/akshare/stock/stock_us_js.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_us_pink.py` & `akshare-1.9.96/akshare/stock/stock_us_pink.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_us_sina.py` & `akshare-1.9.96/akshare/stock/stock_us_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_us_zh_hx.py` & `akshare-1.9.96/akshare/stock/stock_us_zh_hx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_weibo_nlp.py` & `akshare-1.9.96/akshare/stock/stock_weibo_nlp.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_zh_a_sina.py` & `akshare-1.9.96/akshare/stock/stock_zh_a_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_zh_a_special.py` & `akshare-1.9.96/akshare/stock/stock_zh_a_special.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_zh_a_tick_tx.py` & `akshare-1.9.96/akshare/stock/stock_zh_a_tick_tx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_zh_ah_tx.py` & `akshare-1.9.96/akshare/stock/stock_zh_ah_tx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_zh_b_sina.py` & `akshare-1.9.96/akshare/stock/stock_zh_b_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_zh_kcb_report.py` & `akshare-1.9.96/akshare/stock/stock_zh_kcb_report.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock/stock_zh_kcb_sina.py` & `akshare-1.9.96/akshare/stock/stock_zh_kcb_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_a_below_net_asset_statistics.py` & `akshare-1.9.96/akshare/stock_feature/stock_a_below_net_asset_statistics.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_a_high_low.py` & `akshare-1.9.96/akshare/stock_feature/stock_a_high_low.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_a_indicator.py` & `akshare-1.9.96/akshare/stock_feature/stock_a_indicator.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_a_pe_and_pb.py` & `akshare-1.9.96/akshare/stock_feature/stock_a_pe_and_pb.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_account_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_account_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_all_pb.py` & `akshare-1.9.96/akshare/stock_feature/stock_all_pb.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_analyst_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_analyst_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_average_position_lg.py` & `akshare-1.9.96/akshare/stock_feature/stock_average_position_lg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_board_concept_ths.py` & `akshare-1.9.96/akshare/stock_feature/stock_board_concept_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_board_industry_ths.py` & `akshare-1.9.96/akshare/stock_feature/stock_board_industry_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_buffett_index_lg.py` & `akshare-1.9.96/akshare/stock_feature/stock_buffett_index_lg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_classify_sina.py` & `akshare-1.9.96/akshare/stock_feature/stock_classify_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_cls_alerts.py` & `akshare-1.9.96/akshare/stock_feature/stock_cls_alerts.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_cninfo_yjyg.py` & `akshare-1.9.96/akshare/stock_feature/stock_cninfo_yjyg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_comment_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_comment_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_congestion_lg.py` & `akshare-1.9.96/akshare/stock_feature/stock_congestion_lg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_dxsyl_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_dxsyl_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_ebs_lg.py` & `akshare-1.9.96/akshare/stock_feature/stock_ebs_lg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_fhps_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_fhps_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_fhps_ths.py` & `akshare-1.9.96/akshare/stock_feature/stock_fhps_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_fund_flow.py` & `akshare-1.9.96/akshare/stock_feature/stock_fund_flow.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_gdfx_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_gdfx_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_gdhs.py` & `akshare-1.9.96/akshare/stock_feature/stock_gdhs.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_gdzjc_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_gdzjc_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_gpzy_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_gpzy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_gxl_lg.py` & `akshare-1.9.96/akshare/stock_feature/stock_gxl_lg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_hist_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_hist_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_hk_valuation_baidu.py` & `akshare-1.9.96/akshare/stock_feature/stock_hk_valuation_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_hot_tgb.py` & `akshare-1.9.96/akshare/stock_feature/stock_hot_tgb.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_hot_xq.py` & `akshare-1.9.96/akshare/stock_feature/stock_hot_xq.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_hsgt_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_hsgt_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_hsgt_exchange_rate.py` & `akshare-1.9.96/akshare/stock_feature/stock_hsgt_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_inner_trade_xq.py` & `akshare-1.9.96/akshare/stock_feature/stock_inner_trade_xq.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_jgdy_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_jgdy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_lh_yybpm.py` & `akshare-1.9.96/akshare/stock_feature/stock_lh_yybpm.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_lhb_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_lhb_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_lhb_sina.py` & `akshare-1.9.96/akshare/stock_feature/stock_lhb_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_market_legu.py` & `akshare-1.9.96/akshare/stock_feature/stock_market_legu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_pankou_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_pankou_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_qsjy_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_qsjy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_report_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_report_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_sse_margin.py` & `akshare-1.9.96/akshare/stock_feature/stock_sse_margin.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_sy_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_sy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_szse_margin.py` & `akshare-1.9.96/akshare/stock_feature/stock_szse_margin.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_technology_ths.py` & `akshare-1.9.96/akshare/stock_feature/stock_technology_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_tfp_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_tfp_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_three_report_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_three_report_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_ttm_lyr.py` & `akshare-1.9.96/akshare/stock_feature/stock_ttm_lyr.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_us_hist_futunn.py` & `akshare-1.9.96/akshare/stock_feature/stock_us_hist_futunn.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_wencai.py` & `akshare-1.9.96/akshare/stock_feature/stock_wencai.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_yjbb_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_yjbb_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_yjyg_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_yjyg_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_yzxdr_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_yzxdr_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_zf_pg.py` & `akshare-1.9.96/akshare/stock_feature/stock_zf_pg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_zh_valuation_baidu.py` & `akshare-1.9.96/akshare/stock_feature/stock_zh_valuation_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_zh_vote_baidu.py` & `akshare-1.9.96/akshare/stock_feature/stock_zh_vote_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/stock_ztb_em.py` & `akshare-1.9.96/akshare/stock_feature/stock_ztb_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_feature/ths.js` & `akshare-1.9.96/akshare/stock_feature/ths.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_finance.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_finance.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_finance_hk.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_finance_hk.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_finance_ths.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_finance_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_hold.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_hold.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_ipo_declare.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_ipo_declare.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_kcb_detail_sse.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_kcb_detail_sse.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_kcb_sse.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_kcb_sse.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_mda_ym.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_mda_ym.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_notice.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_notice.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_profit_forecast_em.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_profit_forecast_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_profit_forecast_ths.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_profit_forecast_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_recommend.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_recommend.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_register.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_register.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_restricted_em.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_restricted_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_zygc.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_zygc.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/stock_fundamental/stock_zyjs_ths.py` & `akshare-1.9.96/akshare/stock_fundamental/stock_zyjs_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/tool/trade_date_hist.py` & `akshare-1.9.96/akshare/tool/trade_date_hist.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/utils/demjson.py` & `akshare-1.9.96/akshare/utils/demjson.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare/utils/token_process.py` & `akshare-1.9.96/akshare/utils/token_process.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/akshare.egg-info/PKG-INFO` & `akshare-1.9.96/akshare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akshare
-Version: 1.9.95
+Version: 1.9.96
 Summary: AKShare is an elegant and simple financial data interface library for Python, built for human beings!
 Home-page: https://github.com/akfamily/akshare
 Author: AKFamily
 Author-email: akfamily.akshare@gmail.com
 License: MIT
 Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `akshare-1.9.95/akshare.egg-info/SOURCES.txt` & `akshare-1.9.96/akshare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/setup.py` & `akshare-1.9.96/setup.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.95/tests/test_func.py` & `akshare-1.9.96/tests/test_func.py`

 * *Files identical despite different names*

