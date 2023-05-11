# Comparing `tmp/akshare-1.9.80.tar.gz` & `tmp/akshare-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akshare-1.9.80.tar", last modified: Thu May 11 10:08:23 2023, max compression
+gzip compressed data, was "akshare-1.9.9.tar", last modified: Thu Mar  9 15:07:22 2023, max compression
```

## Comparing `akshare-1.9.80.tar` & `akshare-1.9.9.tar`

### file list

```diff
@@ -1,399 +1,396 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.529760 akshare-1.9.80/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-11 10:08:12.000000 akshare-1.9.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-11 10:08:23.529760 akshare-1.9.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-05-11 10:08:12.000000 akshare-1.9.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.497760 akshare-1.9.80/akshare/
--rw-r--r--   0 runner    (1001) docker     (123)   153112 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.497760 akshare-1.9.80/akshare/air/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/air/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/air/air_hebei.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/air/air_zhenqi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/air/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/air/crypto.js
--rw-r--r--   0 runner    (1001) docker     (123)   142353 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/air/outcrypto.js
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/air/sunrise_tad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.497760 akshare-1.9.80/akshare/article/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/article/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/article/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/article/epu_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/article/ff_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/article/fred_md.py
--rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/article/risk_rv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.497760 akshare-1.9.80/akshare/bank/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bank/bank_cbirc_2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bank/cons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.501760 akshare-1.9.80/akshare/bond/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_cb_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_cbond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_china_money.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_info_cm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_issue_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    23003 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_zh_cov_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/bond_zh_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/china_bond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/china_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/bond/cons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.501760 akshare-1.9.80/akshare/cost/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/cost/cost_living.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.501760 akshare-1.9.80/akshare/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/crypto/crypto_bitcoin_cme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/crypto/crypto_crix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/crypto/crypto_hist_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/crypto/crypto_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.501760 akshare-1.9.80/akshare/currency/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/currency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/currency/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/currency/currency_china_bank_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/currency/currency_safe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.501760 akshare-1.9.80/akshare/data/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   209327 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/data/covid.js
--rw-r--r--   0 runner    (1001) docker     (123)   122225 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/data/crypto_info.zip
--rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/data/ths.js
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.501760 akshare-1.9.80/akshare/economic/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_australia.py
--rw-r--r--   0 runner    (1001) docker     (123)    31987 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_bank.py
--rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_canada.py
--rw-r--r--   0 runner    (1001) docker     (123)   181370 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_china.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_china_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_constitute.py
--rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_euro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_germany.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_japan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_other.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_swiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_uk.py
--rw-r--r--   0 runner    (1001) docker     (123)   121733 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/macro_usa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/economic/marco_cnbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.505760 akshare-1.9.80/akshare/energy/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/energy/energy_carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/energy/energy_oil_em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.505760 akshare-1.9.80/akshare/event/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/event/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    38159 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/event/covid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.505760 akshare-1.9.80/akshare/file_fold/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/file_fold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   112983 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/file_fold/calendar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.505760 akshare-1.9.80/akshare/fortune/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fortune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fortune/fortune_500.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fortune/fortune_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fortune/fortune_forbes_500.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fortune/fortune_hurun.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fortune/fortune_it_juzi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fortune/fortune_xincaifu_500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.505760 akshare-1.9.80/akshare/fund/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31203 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_amac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_aum_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    40604 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_etf_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_etf_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_fhsp_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_init_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_portfolio_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_position_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    15544 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_rank_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_rating.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_report_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_scale_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fund/fund_scale_sina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.509760 akshare-1.9.80/akshare/futures/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    48979 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/cot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_comex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_comm_qihuo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_contract_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_daily_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_foreign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_hq_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_index_ccidx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_international.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_inventory_99.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_inventory_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_news_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_news_shmet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_roll_yield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_sgx_daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_spot_stock_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_to_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_warehouse_receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/futures_zh_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/inventory_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19131 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/receipt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/requests_fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures/symbol_var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.509760 akshare-1.9.80/akshare/futures_derivative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/futures_egg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/futures_hog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/futures_index_price_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/futures_index_return_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/futures_index_volatility_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/futures_other_index_nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/futures_sina_cot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/sina_futures_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/futures_derivative/sys_spot_futures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.509760 akshare-1.9.80/akshare/fx/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fx/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    12511 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fx/currency_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fx/fx_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/fx/fx_quote_baidu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.509760 akshare-1.9.80/akshare/hf/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/hf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/hf/hf_sp500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/index/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/dailydata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/drewry_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    53902 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_cflp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_cni.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_eri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_hog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_investing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_kq_fz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_kq_ss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_stock_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_stock_zh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_sugar.py
--rw-r--r--   0 runner    (1001) docker     (123)    29465 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_sw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_sw_research.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_weibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_yw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/index_zh_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/index/stock_zh_index_csindex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/interest_rate/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/interest_rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/interest_rate/interbank_rate_em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/movie/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/movie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/movie/artist_yien.py
--rw-r--r--   0 runner    (1001) docker     (123)   117172 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/movie/jm.js
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/movie/movie_yien.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/movie/video_yien.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/news/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/news/news_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/news/news_cctv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/news/news_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/nlp/nlp_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/option/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)    19039 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_commodity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_commodity_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_czce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_finance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34775 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_finance_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_lhb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_premium_analysis_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_qvix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_risk_analysis_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_risk_indicator_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/option/option_value_analysis_em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/other/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/other/other_car.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/other/other_game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.513760 akshare-1.9.80/akshare/pro/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/pro/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/pro/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/pro/data_pro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.517760 akshare-1.9.80/akshare/qhkc/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/qhkc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/qhkc/qhkc_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.517760 akshare-1.9.80/akshare/qhkc_web/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/qhkc_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/qhkc_web/qhkc_fund.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/qhkc_web/qhkc_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/qhkc_web/qhkc_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.517760 akshare-1.9.80/akshare/rate/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/rate/repo_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.517760 akshare-1.9.80/akshare/reits/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/reits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/reits/reits_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.517760 akshare-1.9.80/akshare/sport/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/sport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/sport/sport_olympic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/sport/sport_olympic_winter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.517760 akshare-1.9.80/akshare/spot/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/spot/spot_sge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.521760 akshare-1.9.80/akshare/stock/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_allotment_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_ask_bid_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_board_concept_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_board_industry_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_cg_equity_mortgage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_cg_guarantee.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_cg_lawsuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_dividents_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_dzjy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    38613 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_fund.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_fund_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_hk_fhpx_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_hk_hot_rank_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_hk_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_hold_control_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_hold_num_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_hot_rank_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_hot_search_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_industry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_industry_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_industry_pe_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_info_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_new_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_profile_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_rank_forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_repurchase_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_share_changes_cninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)    19452 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_us_famous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_us_js.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_us_pink.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_us_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_us_zh_hx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_weibo_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17827 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_zh_a_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_zh_a_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_zh_a_tick_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_zh_ah_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_zh_b_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_zh_kcb_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock/stock_zh_kcb_sina.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.525760 akshare-1.9.80/akshare/stock_feature/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/cons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_a_below_net_asset_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_a_high_low.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_a_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_a_pe_and_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_account_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_all_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_analyst_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_average_position_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_board_concept_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)    23722 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_board_industry_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_buffett_index_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_classify_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_cls_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_cninfo_yjyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_comment_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_congestion_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_dxsyl_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_ebs_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_fhps_em.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_fhps_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_fund_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_gdfx_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_gdhs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_gdzjc_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_gpzy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_gxl_lg.py
--rw-r--r--   0 runner    (1001) docker     (123)    66460 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_hist_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_hk_valuation_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_hot_tgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_hot_xq.py
--rw-r--r--   0 runner    (1001) docker     (123)    66045 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_hsgt_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_hsgt_exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_inner_trade_xq.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_jgdy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_lh_yybpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_lhb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_lhb_sina.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_market_legu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_pankou_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_qsjy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_report_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_sse_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_sy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_szse_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_technology_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_tfp_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_three_report_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_ttm_lyr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_us_hist_futunn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_wencai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_yjbb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_yjyg_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_yzxdr_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_zf_pg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_zh_valuation_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_zh_vote_baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/stock_ztb_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_feature/ths.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.525760 akshare-1.9.80/akshare/stock_fundamental/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26766 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_finance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_finance_hk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_ipo_declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_kcb_detail_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_kcb_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_mda_ym.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_notice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_profit_forecast_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_profit_forecast_ths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_recommend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_register.py
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_restricted_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_zygc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/stock_fundamental/stock_zyjs_ths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.529760 akshare-1.9.80/akshare/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/tool/trade_date_hist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.529760 akshare-1.9.80/akshare/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/utils/ak_session.py
--rw-r--r--   0 runner    (1001) docker     (123)   241609 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/utils/demjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-11 10:08:12.000000 akshare-1.9.80/akshare/utils/token_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.497760 akshare-1.9.80/akshare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14700 2023-05-11 10:08:23.000000 akshare-1.9.80/akshare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-11 10:08:23.000000 akshare-1.9.80/akshare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 10:08:23.000000 akshare-1.9.80/akshare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-11 10:08:23.000000 akshare-1.9.80/akshare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 10:08:23.000000 akshare-1.9.80/akshare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-11 10:08:12.000000 akshare-1.9.80/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 10:08:23.529760 akshare-1.9.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-11 10:08:12.000000 akshare-1.9.80/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 10:08:23.529760 akshare-1.9.80/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-11 10:08:12.000000 akshare-1.9.80/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-11 10:08:12.000000 akshare-1.9.80/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.187285 akshare-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-09 15:07:07.000000 akshare-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-03-09 15:07:22.187285 akshare-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13964 2023-03-09 15:07:07.000000 akshare-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.147284 akshare-1.9.9/akshare/
+-rw-r--r--   0 runner    (1001) docker     (123)   149135 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.151284 akshare-1.9.9/akshare/air/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/air/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/air/air_hebei.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/air/air_zhenqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9771 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/air/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/air/crypto.js
+-rw-r--r--   0 runner    (1001) docker     (123)   142353 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/air/outcrypto.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/air/sunrise_tad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.151284 akshare-1.9.9/akshare/article/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/article/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/article/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/article/epu_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/article/ff_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/article/fred_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13162 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/article/risk_rv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.151284 akshare-1.9.9/akshare/bank/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bank/bank_cbirc_2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bank/cons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.151284 akshare-1.9.9/akshare/bond/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_cbond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_china_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_info_cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_issue_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23003 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_zh_cov_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/bond_zh_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/china_bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/china_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/bond/cons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.151284 akshare-1.9.9/akshare/cost/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/cost/cost_living.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.151284 akshare-1.9.9/akshare/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/crypto/crypto_bitcoin_cme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/crypto/crypto_crix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/crypto/crypto_hist_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/crypto/crypto_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.151284 akshare-1.9.9/akshare/currency/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/currency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/currency/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/currency/currency_china_bank_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/currency/currency_safe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.155284 akshare-1.9.9/akshare/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209327 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/data/covid.js
+-rw-r--r--   0 runner    (1001) docker     (123)   122225 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/data/crypto_info.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/data/ths.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.155284 akshare-1.9.9/akshare/economic/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_australia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31987 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15195 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_canada.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181223 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_china.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_china_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_constitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40919 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_euro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_germany.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_japan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_swiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_uk.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121523 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/macro_usa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/economic/marco_cnbs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.155284 akshare-1.9.9/akshare/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/energy/energy_carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/energy/energy_oil_em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.155284 akshare-1.9.9/akshare/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12807 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/event/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38159 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/event/covid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.155284 akshare-1.9.9/akshare/file_fold/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/file_fold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112983 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/file_fold/calendar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.155284 akshare-1.9.9/akshare/fortune/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fortune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fortune/fortune_500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fortune/fortune_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fortune/fortune_forbes_500.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fortune/fortune_hurun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fortune/fortune_it_juzi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fortune/fortune_xincaifu_500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.159284 akshare-1.9.9/akshare/fund/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31404 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_amac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_aum_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_etf_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_etf_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_fhsp_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_init_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_portfolio_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_position_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_rank_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_rating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_report_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_scale_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fund/fund_scale_sina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.163284 akshare-1.9.9/akshare/futures/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13386 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_comex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_comm_qihuo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_contract_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26034 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_daily_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_foreign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_hq_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_index_ccidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_international.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_inventory_99.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_inventory_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_news_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_news_shmet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_roll_yield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_sgx_daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_spot_stock_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_to_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_warehouse_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23910 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/futures_zh_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/inventory_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/requests_fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures/symbol_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.163284 akshare-1.9.9/akshare/futures_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/futures_egg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14308 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/futures_hog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/futures_index_price_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/futures_index_return_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/futures_index_volatility_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/futures_other_index_nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/futures_sina_cot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/sina_futures_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/futures_derivative/sys_spot_futures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.163284 akshare-1.9.9/akshare/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fx/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fx/currency_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fx/fx_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/fx/fx_quote_baidu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.163284 akshare-1.9.9/akshare/hf/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/hf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/hf/hf_sp500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.167284 akshare-1.9.9/akshare/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/dailydata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/drewry_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53902 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_cflp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_cni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_eri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_hog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_investing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_kq_fz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_kq_ss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_stock_zh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_sugar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29465 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_sw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_sw_research.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_weibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_yw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/index_zh_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/index/stock_zh_index_csindex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.167284 akshare-1.9.9/akshare/interest_rate/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/interest_rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/interest_rate/interbank_rate_em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.167284 akshare-1.9.9/akshare/movie/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/movie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/movie/artist_yien.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117172 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/movie/jm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/movie/movie_yien.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/movie/video_yien.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.167284 akshare-1.9.9/akshare/news/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/news/news_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/news/news_cctv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/news/news_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.167284 akshare-1.9.9/akshare/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/nlp/nlp_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/option/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_commodity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_commodity_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_czce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_finance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34775 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_finance_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_lhb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_premium_analysis_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_qvix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_risk_analysis_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_risk_indicator_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/option/option_value_analysis_em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/other/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/other/other_car.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/other/other_game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/pro/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/pro/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/pro/data_pro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/qhkc/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/qhkc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/qhkc/qhkc_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/qhkc_web/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/qhkc_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17400 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/qhkc_web/qhkc_fund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/qhkc_web/qhkc_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/qhkc_web/qhkc_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/rate/repo_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/reits/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/reits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/reits/reits_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/sport/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/sport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/sport/sport_olympic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/sport/sport_olympic_winter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.171284 akshare-1.9.9/akshare/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/spot/spot_sge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.175284 akshare-1.9.9/akshare/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_allotment_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_board_concept_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_board_industry_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_cg_equity_mortgage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_cg_guarantee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_cg_lawsuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_dividents_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_dzjy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22924 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_fund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_fund_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_hist_163.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_hk_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_hold_control_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_hold_num_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_hot_rank_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_hot_search_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_industry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_industry_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_industry_pe_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15590 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_info_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_new_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_profile_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_rank_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_repurchase_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_share_changes_cninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_us_famous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_us_js.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_us_pink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_us_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_us_zh_hx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_weibo_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17824 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_zh_a_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_zh_a_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_zh_a_tick_tx_163.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_zh_ah_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_zh_b_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_zh_kcb_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock/stock_zh_kcb_sina.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.183284 akshare-1.9.9/akshare/stock_feature/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/cons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_a_below_net_asset_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_a_high_low.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_a_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12741 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_a_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13917 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_a_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_a_pe_and_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_account_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_all_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_analyst_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_average_position_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_board_concept_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_board_industry_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_buffett_index_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_classify_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_cls_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_cninfo_yjyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_comment_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_congestion_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16608 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_dxsyl_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_ebs_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_fhps_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18221 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_fund_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36227 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_gdfx_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_gdhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_gdzjc_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_gpzy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_gxl_lg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63731 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_hist_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_hk_valuation_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_hot_tgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_hot_xq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66043 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_hsgt_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_hsgt_exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_inner_trade_xq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_jgdy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_lh_yybpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_lhb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_lhb_sina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_market_legu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_pankou_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_qsjy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_report_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_sse_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_sy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_szse_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_technology_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_tfp_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15959 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_three_report_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_ttm_lyr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_us_hist_futunn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_wencai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_yjbb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_yjyg_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_yzxdr_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_zf_pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_zh_valuation_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_zh_vote_baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/stock_ztb_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39664 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_feature/ths.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.187285 akshare-1.9.9/akshare/stock_fundamental/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_finance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_finance_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_ipo_declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_kcb_detail_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_kcb_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_mda_ym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_profit_forecast_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_profit_forecast_ths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_recommend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_restricted_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_zygc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/stock_fundamental/stock_zyjs_ths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.187285 akshare-1.9.9/akshare/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/tool/trade_date_hist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.187285 akshare-1.9.9/akshare/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/utils/ak_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241609 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/utils/demjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-09 15:07:07.000000 akshare-1.9.9/akshare/utils/token_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.147284 akshare-1.9.9/akshare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14801 2023-03-09 15:07:22.000000 akshare-1.9.9/akshare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-03-09 15:07:22.000000 akshare-1.9.9/akshare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 15:07:22.000000 akshare-1.9.9/akshare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-09 15:07:22.000000 akshare-1.9.9/akshare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-09 15:07:22.000000 akshare-1.9.9/akshare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-09 15:07:07.000000 akshare-1.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 15:07:22.187285 akshare-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-09 15:07:07.000000 akshare-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 15:07:22.187285 akshare-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-09 15:07:07.000000 akshare-1.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-03-09 15:07:07.000000 akshare-1.9.9/tests/test_func.py
```

### Comparing `akshare-1.9.80/LICENSE` & `akshare-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/PKG-INFO` & `akshare-1.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akshare
-Version: 1.9.80
+Version: 1.9.9
 Summary: AKShare is an elegant and simple financial data interface library for Python, built for human beings!
 Home-page: https://github.com/akfamily/akshare
 Author: AKFamily
 Author-email: akfamily.akshare@gmail.com
 License: MIT
 Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
 Classifier: Programming Language :: Python :: 3.7
@@ -41,15 +41,15 @@
 
 ## Overview
 
 [AKShare](https://github.com/akfamily/akshare) requires Python(64 bit) 3.8 or greater, aims to make fetch financial data as convenient as possible.
 
 **Write less, get more!**
 
-- Documentation: [中文文档](https://akshare.akfamily.xyz/)
+- Documentation: [中文文档](https://www.akshare.xyz/)
 
 ![](https://github.com/akfamily/akshare/blob/master/example/images/AKShare.svg)
 
 ## Installation
 
 ### General
 
@@ -61,31 +61,31 @@
 
 ```shell
 pip install akshare -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host=mirrors.aliyun.com  --upgrade
 ```
 
 ### PR
 
-Please check out [documentation](https://akshare.akfamily.xyz/contributor.html) if you want to contribute to AKShare
+Please check out [documentation](https://www.akshare.xyz/zh_CN/latest/contributor.html) if you want to contribute to AKShare
 
 ### Docker
 
 #### Pull images
 
 ```shell
-docker pull registry.cn-shanghai.aliyuncs.com/akfamily/aktools:jupyter
+docker pull registry.cn-hangzhou.aliyuncs.com/akshare/akdocker
 ```
 
-#### Run Container
+#### Run AKDocker
 
 ```shell
-docker run -it registry.cn-shanghai.aliyuncs.com/akfamily/aktools:jupyter python
+docker run -it registry.cn-hangzhou.aliyuncs.com/akshare/akdocker python
 ```
 
-#### Test
+#### Test AKDocker
 
 ```python
 import akshare as ak
 
 print(ak.__version__)
 ```
 
@@ -161,19 +161,19 @@
 
 - **Easy of use**: Just one line code to fetch the data;
 - **Extensible**: Easy to customize your own code with other application;
 - **Powerful**: Python ecosystem.
 
 ## Tutorials
 
-1. [Overview](https://akshare.akfamily.xyz/introduction.html)
-2. [Installation](https://akshare.akfamily.xyz/installation.html)
-3. [Tutorial](https://akshare.akfamily.xyz/tutorial.html)
-4. [Data Dict](https://akshare.akfamily.xyz/data/index.html)
-5. [Subjects](https://akshare.akfamily.xyz/topic/index.html)
+1. [Overview](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-introduction.html)
+2. [Installation](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-installation.html)
+3. [Tutorial](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-tutorial.html)
+4. [Data Dict](https://akshare.readthedocs.io/zh_CN/latest/README.html)
+5. [Subjects](https://akshare.readthedocs.io/zh_CN/latest/subjects/index.html)
 
 ## Contribution
 
 [AKShare](https://github.com/akfamily/akshare) is still under developing, feel free to open issues and pull requests:
 
 - Report or fix bugs
 - Require or publish interface
```

### Comparing `akshare-1.9.80/README.md` & `akshare-1.9.9/akshare.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: akshare
+Version: 1.9.9
+Summary: AKShare is an elegant and simple financial data interface library for Python, built for human beings!
+Home-page: https://github.com/akfamily/akshare
+Author: AKFamily
+Author-email: akfamily.akshare@gmail.com
+License: MIT
+Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 **AKShare VIP 交流群欢迎大家的加入，加群方式请点击[【加群】](https://zmj.xet.tech/s/28gOeh)**
 
 **相关视频教程已经发布：《AKShare-初阶-使用教学》、《AKShare-初阶-实战应用》、《AKShare-源码解析》、《开源项目巡礼》**，详情请访问[课程](https://app3rqjh1z21630.h5.xiaoeknow.com)查看更多课程信息！
 
 **本次发布 [AKTools](https://github.com/akfamily/aktools) 作为 AKShare 的 HTTP API 版本，突破 Python 语言的限制，欢迎各位小伙伴试用并提出更好的意见或建议！ 点击 [AKTools](https://github.com/akfamily/aktools) 查看使用指南。另外提供 [awesome-data](https://github.com/akfamily/awesome-data) 方便各位小伙伴查询各种数据源。**
 
 ![](https://github.com/akfamily/akshare/blob/master/example/images/AKShare_logo.jpg)
@@ -21,15 +41,15 @@
 
 ## Overview
 
 [AKShare](https://github.com/akfamily/akshare) requires Python(64 bit) 3.8 or greater, aims to make fetch financial data as convenient as possible.
 
 **Write less, get more!**
 
-- Documentation: [中文文档](https://akshare.akfamily.xyz/)
+- Documentation: [中文文档](https://www.akshare.xyz/)
 
 ![](https://github.com/akfamily/akshare/blob/master/example/images/AKShare.svg)
 
 ## Installation
 
 ### General
 
@@ -41,31 +61,31 @@
 
 ```shell
 pip install akshare -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host=mirrors.aliyun.com  --upgrade
 ```
 
 ### PR
 
-Please check out [documentation](https://akshare.akfamily.xyz/contributor.html) if you want to contribute to AKShare
+Please check out [documentation](https://www.akshare.xyz/zh_CN/latest/contributor.html) if you want to contribute to AKShare
 
 ### Docker
 
 #### Pull images
 
 ```shell
-docker pull registry.cn-shanghai.aliyuncs.com/akfamily/aktools:jupyter
+docker pull registry.cn-hangzhou.aliyuncs.com/akshare/akdocker
 ```
 
-#### Run Container
+#### Run AKDocker
 
 ```shell
-docker run -it registry.cn-shanghai.aliyuncs.com/akfamily/aktools:jupyter python
+docker run -it registry.cn-hangzhou.aliyuncs.com/akshare/akdocker python
 ```
 
-#### Test
+#### Test AKDocker
 
 ```python
 import akshare as ak
 
 print(ak.__version__)
 ```
 
@@ -141,19 +161,19 @@
 
 - **Easy of use**: Just one line code to fetch the data;
 - **Extensible**: Easy to customize your own code with other application;
 - **Powerful**: Python ecosystem.
 
 ## Tutorials
 
-1. [Overview](https://akshare.akfamily.xyz/introduction.html)
-2. [Installation](https://akshare.akfamily.xyz/installation.html)
-3. [Tutorial](https://akshare.akfamily.xyz/tutorial.html)
-4. [Data Dict](https://akshare.akfamily.xyz/data/index.html)
-5. [Subjects](https://akshare.akfamily.xyz/topic/index.html)
+1. [Overview](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-introduction.html)
+2. [Installation](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-installation.html)
+3. [Tutorial](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-tutorial.html)
+4. [Data Dict](https://akshare.readthedocs.io/zh_CN/latest/README.html)
+5. [Subjects](https://akshare.readthedocs.io/zh_CN/latest/subjects/index.html)
 
 ## Contribution
 
 [AKShare](https://github.com/akfamily/akshare) is still under developing, feel free to open issues and pull requests:
 
 - Report or fix bugs
 - Require or publish interface
```

### Comparing `akshare-1.9.80/akshare/__init__.py` & `akshare-1.9.9/akshare/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2321,120 +2321,29 @@
 1.9.3 fix: fix fx_quote_baidu interface
 1.9.4 fix: fix drewry_wci_index interface
 1.9.5 fix: fix stock_info_a_code_name interface
 1.9.6 fix: fix futures_hog_info interface
 1.9.7 add: add stock_profit_forecast_ths interface
 1.9.8 fix: fix stock_hk_valuation_baidu interface
 1.9.9 add: add macro_shipping_bci interface
-1.9.10 add: add macro_shipping_bcti interface
-1.9.11 add: add stock_sector_fund_flow_hist interface
-1.9.12 fix: fix stock_hot_rank_wc interface
-1.9.13 fix: fix stock_zh_valuation_baidu interface
-1.9.14 fix: fix option_risk_analysis_em interface
-1.9.15 fix: fix stock_hk_daily interface
-1.9.16 fix: fix stock_financial_abstract interface
-1.9.17 add: add stock_board_industry_spot_em interface
-1.9.18 fix: fix macro_china_market_margin_sh interface
-1.9.19 fix: fix macro_cnbs interface
-1.9.20 fix: fix fund_financial_fund_info_em interface
-1.9.21 fix: fix fund_financial_fund_info_em interface
-1.9.22 fix: fix fund_hk_fund_hist_em interface
-1.9.23 fix: fix bond_cb_redeem_jsl interface
-1.9.24 fix: fix bond_cb_adj_logs_jsl interface
-1.9.25 add: add stock_hk_hot_rank_em interface
-1.9.26 fix: fix bond_cb_jsl interface
-1.9.27 fix: fix fund_exchange_rank_em interface
-1.9.28 fix: fix stock_financial_report_sina interface
-1.9.29 fix: fix stock_a_lg_indicator interface
-1.9.30 fix: fix stock_a_lg_indicator interface
-1.9.31 fix: fix amac_fund_info interface
-1.9.32 fix: fix bank_fjcf_table_detail interface
-1.9.33 add: add stock_hk_main_board_spot_em interface
-1.9.34 fix: fix stock_zh_a_tick_tx_js interface
-1.9.35 fix: fix stock_a_lg_indicator interface
-1.9.36 fix: fix stock_market_pe_lg interface
-1.9.37 fix: fix stock_hk_indicator_eniu interface
-1.9.38 fix: fix stock_a_lg_indicator interface
-1.9.39 fix: fix fund_stock_position_lg interface
-1.9.40 fix: fix stock_profit_forecast_em interface
-1.9.41 fix: fix stock_a_indicator_lg interface
-1.9.42 add: add stock_bid_ask_em interface
-1.9.43 fix: fix stock_a_congestion_lg interface
-1.9.44 fix: fix stock_a_high_low_statistics interface
-1.9.45 add: add stock_fhps_detail_ths interface
-1.9.46 fix: fix stock_a_gxl_lg interface
-1.9.47 fix: fix option_dce_daily interface
-1.9.48 fix: fix index_stock_cons interface
-1.9.49 add: add stock_lhb_yybph_em interface
-1.9.50 fix: fix stock_a_all_pb interface
-1.9.51 fix: fix get_shfe_daily interface
-1.9.52 fix: fix get_shfe_rank_table interface
-1.9.53 fix: fix get_ine_daily interface
-1.9.54 fix: fix stock_board_concept_cons_ths interface
-1.9.55 fix: fix stock_zh_valuation_baidu interface
-1.9.56 fix: fix get_receipt interface
-1.9.57 fix: fix stock_lhb_detail_em interface
-1.9.58 add: add option_gfex_daily interface
-1.9.59 fix: fix stock_hot_search_baidu interface
-1.9.60 add: add stock_hk_fhpx_detail_ths interface
-1.9.61 fix: fix stock_lhb_detail_daily_sina interface
-1.9.62 fix: fix bond_zh_us_rate interface
-1.9.63 fix: fix get_czce_rank_table interface
-1.9.64 fix: fix stock_a_indicator_lg interface
-1.9.65 fix: fix stock_hot_search_baidu interface
-1.9.66 fix: fix match_main_contract interface
-1.9.67 fix: fix futures_zh_daily_sina interface
-1.9.68 fix: fix stock_lh_yyb_capital interface
-1.9.69 fix: fix stock_lh_yyb_capital interface
-1.9.70 fix: fix stock_szse_sector_summary interface
-1.9.71 fix: fix stock_lh_yyb_most interface
-1.9.72 fix: fix fund_manager interface
-1.9.73 add: add bond_zh_cov_info_ths interface
-1.9.74 fix: fix get_shfe_rank_table interface
-1.9.75 fix: fix stock_board_industry_index_ths interface
-1.9.76 fix: fix stock_sector_detail interface
-1.9.77 fix: fix stock_hot_rank_wc interface
-1.9.78 fix: fix macro_usa_gdp_monthly interface
-1.9.79 fix: fix stock_sse_deal_daily interface
-1.9.80 fix: fix futures_spot_price interface
 """
 
-__version__ = "1.9.80"
+__version__ = "1.9.9"
 __author__ = "AKFamily"
 
 import sys
 import warnings
 
 if sys.version_info < (3, 8):
     warnings.warn("为了支持更多 AKShare 特性，请尽快升级 Python 到 3.8 以上版本")
     # sys.exit(1)
 
 del sys
 
 """
-同花顺-数据中心-可转债
-"""
-from akshare.bond.bond_cb_ths import bond_zh_cov_info_ths
-
-"""
-同花顺-港股-分红派息
-"""
-from akshare.stock.stock_hk_fhpx_ths import stock_hk_fhpx_detail_ths
-
-"""
-同花顺-分红融资
-"""
-from akshare.stock_feature.stock_fhps_ths import stock_fhps_detail_ths
-
-"""
-东方财富-行情报价
-"""
-from akshare.stock.stock_ask_bid_em import stock_bid_ask_em
-
-"""
 同花顺-盈利预测
 """
 from akshare.stock_fundamental.stock_profit_forecast_ths import stock_profit_forecast_ths
 
 """
 期货资讯
 """
@@ -2681,51 +2590,43 @@
 from akshare.stock_feature.stock_lhb_em import (
     stock_lhb_hyyyb_em,
     stock_lhb_detail_em,
     stock_lhb_stock_detail_em,
     stock_lhb_jgmmtj_em,
     stock_lhb_stock_statistic_em,
     stock_lhb_stock_detail_date_em,
-    stock_lhb_yybph_em,
-    stock_lhb_jgstatistic_em,
-    stock_lhb_traderstatistic_em,
 )
 
 """
+网易财经-行情首页-沪深 A 股-每日行情
+"""
+from akshare.stock.stock_hist_163 import stock_zh_a_hist_163
+
+"""
 指数行情数据
 """
 from akshare.index.index_zh_em import (
     index_zh_a_hist,
     index_zh_a_hist_min_em,
     index_code_id_map_em,
 )
 
 """
-东方财富个股人气榜-A股
+东方财富个股人气榜
 """
 from akshare.stock.stock_hot_rank_em import (
     stock_hot_rank_detail_em,
     stock_hot_rank_em,
     stock_hot_rank_detail_realtime_em,
     stock_hot_rank_relate_em,
     stock_hot_keyword_em,
     stock_hot_rank_latest_em,
 )
 
 """
-东方财富个股人气榜-港股
-"""
-from akshare.stock.stock_hk_hot_rank_em import (
-    stock_hk_hot_rank_detail_em,
-    stock_hk_hot_rank_latest_em,
-    stock_hk_hot_rank_detail_realtime_em,
-    stock_hk_hot_rank_em,
-)
-
-"""
 冬奥会历届奖牌榜
 """
 from akshare.sport.sport_olympic_winter import sport_olympic_winter_hist
 
 """
 财新指数
 """
@@ -2828,15 +2729,14 @@
 东方财富-行业板块
 """
 from akshare.stock.stock_board_industry_em import (
     stock_board_industry_cons_em,
     stock_board_industry_hist_em,
     stock_board_industry_hist_min_em,
     stock_board_industry_name_em,
-    stock_board_industry_spot_em,
 )
 
 """
 天天基金网-基金数据-规模变动
 """
 from akshare.fund.fund_scale_em import (
     fund_scale_change_em,
@@ -3020,15 +2920,15 @@
 美股-粉单市场
 """
 from akshare.stock.stock_us_pink import stock_us_pink_spot_em
 
 """
 REITs
 """
-from akshare.reits.reits_basic import reits_realtime_em
+from akshare.reits.reits_basic import reits_info_jsl, reits_realtime_em
 
 """
 鸡蛋价格数据
 """
 from akshare.futures_derivative.futures_egg import (
     futures_egg_price_yearly,
     futures_egg_price_area,
@@ -3198,15 +3098,14 @@
     stock_kc_a_spot_em,
     stock_cy_a_spot_em,
     stock_sh_a_spot_em,
     stock_sz_a_spot_em,
     stock_zh_b_spot_em,
     stock_zh_a_hist,
     stock_hk_spot_em,
-    stock_hk_main_board_spot_em,
     stock_hk_hist,
     stock_us_spot_em,
     stock_us_hist,
     stock_zh_a_hist_min_em,
     stock_zh_a_hist_pre_min_em,
     stock_hk_hist_min_em,
     stock_us_hist_min_em,
@@ -3398,15 +3297,15 @@
     stock_board_concept_hist_ths,
     stock_board_cons_ths,
 )
 
 """
 分红配送
 """
-from akshare.stock_feature.stock_fhps_em import stock_fhps_em, stock_fhps_detail_em
+from akshare.stock_feature.stock_fhps_em import stock_fhps_em
 
 """
 中美国债收益率
 """
 from akshare.bond.bond_em import bond_zh_us_rate
 
 """
@@ -3539,19 +3438,19 @@
 """
 from akshare.rate.repo_rate import repo_rate_hist
 
 """
 公募基金排行
 """
 from akshare.fund.fund_rank_em import (
-    fund_exchange_rank_em,
-    fund_money_rank_em,
+    fund_em_exchange_rank,
+    fund_em_money_rank,
     fund_open_fund_rank_em,
-    fund_hk_rank_em,
-    fund_lcx_rank_em,
+    fund_em_hk_rank,
+    fund_em_lcx_rank,
 )
 
 """
 英为财情-加密货币
 """
 from akshare.crypto.crypto_hist_investing import (
     crypto_hist,
@@ -3679,23 +3578,25 @@
     option_commodity_contract_sina,
     option_commodity_hist_sina,
 )
 
 """
 A 股PE和PB
 """
+from akshare.stock_feature.stock_a_pb import stock_a_pb
+from akshare.stock_feature.stock_a_pe import stock_a_pe
 from akshare.stock_feature.stock_a_pe_and_pb import (
     stock_market_pb_lg,
     stock_index_pb_lg,
     stock_market_pe_lg,
     stock_index_pe_lg,
 )
 from akshare.stock_feature.stock_a_indicator import (
-    stock_a_indicator_lg,
-    stock_hk_indicator_eniu,
+    stock_a_lg_indicator,
+    stock_hk_eniu_indicator,
 )
 from akshare.stock_feature.stock_a_high_low import stock_a_high_low_statistics
 from akshare.stock_feature.stock_a_below_net_asset_statistics import (
     stock_a_below_net_asset_statistics,
 )
 
 """
@@ -3800,16 +3701,14 @@
 stock_fund
 """
 from akshare.stock.stock_fund import (
     stock_individual_fund_flow,
     stock_market_fund_flow,
     stock_sector_fund_flow_rank,
     stock_individual_fund_flow_rank,
-    stock_sector_fund_flow_summary,
-    stock_sector_fund_flow_hist,
 )
 
 """
 air-quality
 """
 from akshare.air.air_zhenqi import (
     air_quality_hist,
@@ -4328,17 +4227,19 @@
 timeanddate-日出和日落
 """
 from akshare.air.sunrise_tad import sunrise_daily, sunrise_monthly
 
 """
 新浪-指数实时行情和历史行情
 """
-from akshare.stock.stock_zh_a_tick_tx import (
+from akshare.stock.stock_zh_a_tick_tx_163 import (
     stock_zh_a_tick_tx,
     stock_zh_a_tick_tx_js,
+    stock_zh_a_tick_163,
+    stock_zh_a_tick_163_now,
 )
 
 """
 新浪-指数实时行情和历史行情
 """
 from akshare.index.index_stock_zh import (
     stock_zh_index_daily,
@@ -4619,16 +4520,14 @@
 """
 商品期权
 """
 from akshare.option.option_commodity import (
     option_dce_daily,
     option_czce_daily,
     option_shfe_daily,
-    option_gfex_vol_daily,
-    option_gfex_daily,
 )
 
 """
 英为财情-债券
 """
 from akshare.bond.bond_investing import (
     bond_investing_global,
```

### Comparing `akshare-1.9.80/akshare/air/air_hebei.py` & `akshare-1.9.9/akshare/air/air_hebei.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/air/air_zhenqi.py` & `akshare-1.9.9/akshare/air/air_zhenqi.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/air/cons.py` & `akshare-1.9.9/akshare/air/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/air/crypto.js` & `akshare-1.9.9/akshare/air/crypto.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/air/outcrypto.js` & `akshare-1.9.9/akshare/air/outcrypto.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/air/sunrise_tad.py` & `akshare-1.9.9/akshare/air/sunrise_tad.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/article/epu_index.py` & `akshare-1.9.9/akshare/article/epu_index.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/article/ff_factor.py` & `akshare-1.9.9/akshare/article/ff_factor.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/article/fred_md.py` & `akshare-1.9.9/akshare/article/fred_md.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/article/risk_rv.py` & `akshare-1.9.9/akshare/article/risk_rv.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bank/bank_cbirc_2020.py` & `akshare-1.9.9/akshare/bank/bank_cbirc_2020.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,166 +1,133 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/3 21:06
+Date: 2022/5/16 14:06
 Desc: 中国银行保险监督管理委员会-首页-政务信息-行政处罚-银保监分局本级-XXXX行政处罚信息公开表
-https://www.cbirc.gov.cn/cn/view/pages/ItemList.html?itemPId=923&itemId=4115&itemUrl=ItemListRightList.html&itemName=%E9%93%B6%E4%BF%9D%E7%9B%91%E5%88%86%E5%B1%80%E6%9C%AC%E7%BA%A7&itemsubPId=931&itemsubPName=%E8%A1%8C%E6%94%BF%E5%A4%84%E7%BD%9A#2
+http://www.cbirc.gov.cn/cn/view/pages/ItemList.html?itemPId=923&itemId=4115&itemUrl=ItemListRightList.html&itemName=%E9%93%B6%E4%BF%9D%E7%9B%91%E5%88%86%E5%B1%80%E6%9C%AC%E7%BA%A7&itemsubPId=931&itemsubPName=%E8%A1%8C%E6%94%BF%E5%A4%84%E7%BD%9A#2
 提取 具体页面 html 页面的 json 接口
-https://www.cbirc.gov.cn/cn/static/data/DocInfo/SelectByDocId/data_docId=881446.json
+http://www.cbirc.gov.cn/cn/static/data/DocInfo/SelectByDocId/data_docId=881446.json
 2020新接口
 """
-import warnings
-
-import pandas as pd
 import requests
-from tqdm import tqdm
+import pandas as pd
 
 from akshare.bank.cons import cbirc_headers_without_cookie_2020
 
+item_id_list = {
+    '机关': '4113',
+    '本级': '4114',
+    '分局本级': '4115',
+}
+
 
 def bank_fjcf_total_num(item: str = "分局本级") -> int:
     """
     首页-政务信息-行政处罚-银保监分局本级 总页数
-    https://www.cbirc.gov.cn/cn/view/pages/ItemList.html?itemPId=923&itemId=4115&itemUrl=ItemListRightList.html&itemName=%E9%93%B6%E4%BF%9D%E7%9B%91%E5%88%86%E5%B1%80%E6%9C%AC%E7%BA%A7&itemsubPId=931
-    :param item: choice of {"机关", "本级", "分局本级"}
-    :type item: str
+    http://www.cbirc.gov.cn/cn/view/pages/ItemList.html?itemPId=923&itemId=4115&itemUrl=ItemListRightList.html&itemName=%E9%93%B6%E4%BF%9D%E7%9B%91%E5%88%86%E5%B1%80%E6%9C%AC%E7%BA%A7&itemsubPId=931
     :return: 总页数
     :rtype: int
     """
-    item_id_list = {
-        "机关": "4113",
-        "本级": "4114",
-        "分局本级": "4115",
-    }
     cbirc_headers = cbirc_headers_without_cookie_2020.copy()
     main_url = "http://www.cbirc.gov.cn/cbircweb/DocInfo/SelectDocByItemIdAndChild"
     params = {
         "itemId": item_id_list[item],
         "pageSize": "18",
         "pageIndex": "1",
     }
     res = requests.get(main_url, params=params, headers=cbirc_headers)
     return int(res.json()["data"]["total"])
 
 
 def bank_fjcf_total_page(item: str = "分局本级", begin: int = 1) -> int:
     """
-    获取首页-政务信息-行政处罚-银保监分局本级的总页数
-    https://www.cbirc.gov.cn/cn/view/pages/ItemList.html?itemPId=923&itemId=4115&itemUrl=ItemListRightList.html&itemName=%E9%93%B6%E4%BF%9D%E7%9B%91%E5%88%86%E5%B1%80%E6%9C%AC%E7%BA%A7&itemsubPId=931
-    :param item: choice of {"机关", "本级", "分局本级"}
-    :type item: str
-    :param begin: 开始页数
-    :type begin: str
+    获取  首页-政务信息-行政处罚-银保监分局本级 总页数
+    http://www.cbirc.gov.cn/cn/view/pages/ItemList.html?itemPId=923&itemId=4115&itemUrl=ItemListRightList.html&itemName=%E9%93%B6%E4%BF%9D%E7%9B%91%E5%88%86%E5%B1%80%E6%9C%AC%E7%BA%A7&itemsubPId=931
     :return: 总页数
     :rtype: int
     """
-    item_id_list = {
-        "机关": "4113",
-        "本级": "4114",
-        "分局本级": "4115",
-    }
     cbirc_headers = cbirc_headers_without_cookie_2020.copy()
     main_url = "http://www.cbirc.gov.cn/cbircweb/DocInfo/SelectDocByItemIdAndChild"
     params = {
         "itemId": item_id_list[item],
         "pageSize": "18",
         "pageIndex": str(begin),
     }
     res = requests.get(main_url, params=params, headers=cbirc_headers)
     if res.json()["data"]["total"] / 18 > int(res.json()["data"]["total"] / 18):
         total_page = int(res.json()["data"]["total"] / 18) + 1
     return total_page
 
 
-def bank_fjcf_page_url(
-    page: int = 5, item: str = "分局本级", begin: int = 1
-) -> pd.DataFrame:
+def bank_fjcf_page_url(page: int = 5, item: str = "分局本级", begin: int = 1) -> pd.DataFrame:
     """
     获取 首页-政务信息-行政处罚-银保监分局本级-每一页的 json 数据
-    :param page: 需要获取前 page 页的内容, 总页数请通过 ak.bank_fjcf_total_page() 获取
+    :param page: 需要获取前 page 页的内容, 总页数请通过 bank_fjcf_total_page() 获取
     :type page: int
-    :param item: choice of {"机关", "本级", "分局本级"}
-    :type item: str
-    :param begin: 开始页数
-    :type begin: str
     :return: 需要的字段
     :rtype: pandas.DataFrame
     """
-    item_id_list = {
-        "机关": "4113",
-        "本级": "4114",
-        "分局本级": "4115",
-    }
     cbirc_headers = cbirc_headers_without_cookie_2020.copy()
     main_url = "http://www.cbirc.gov.cn/cbircweb/DocInfo/SelectDocByItemIdAndChild"
     temp_df = pd.DataFrame()
-    for i_page in tqdm(range(begin, page + begin), leave=False):
+    for i_page in range(begin, page+begin):
+        print(i_page)
         params = {
             "itemId": item_id_list[item],
             "pageSize": "18",
             "pageIndex": str(i_page),
         }
         res = requests.get(main_url, params=params, headers=cbirc_headers)
         temp_df = pd.concat([temp_df, pd.DataFrame(res.json()["data"]["rows"])])
-    return temp_df[
-        ["docId", "docSubtitle", "publishDate", "docFileUrl", "docTitle", "generaltype"]
-    ]
+    return temp_df[["docId", "docSubtitle", "publishDate", "docFileUrl", "docTitle", "generaltype"]]
 
 
-def bank_fjcf_table_detail(
-    page: int = 5, item: str = "分局本级", begin: int = 1
-) -> pd.DataFrame:
+def bank_fjcf_table_detail(page: int = 5, item: str = "分局本级", begin: int = 1) -> pd.DataFrame:
     """
     获取 首页-政务信息-行政处罚-银保监分局本级-XXXX行政处罚信息公开表 数据
-    :param page: 需要获取前 page 页的内容, 总页数请通过 ak.bank_fjcf_total_page() 获取
+    :param page: 需要获取前 page 页的内容, 总页数请通过 bank_fjcf_total_page() 获取
     :type page: int
-    :param item: choice of {"机关", "本级", "分局本级"}
-    :type item: str
-    :param begin: 开始页面
-    :type begin: int
     :return: 返回所有行政处罚信息公开表的集合, 按第一页到最后一页的顺序排列
     :rtype: pandas.DataFrame
     """
     id_list = bank_fjcf_page_url(page=page, item=item, begin=begin)["docId"]
     big_df = pd.DataFrame()
     for item in id_list:
+        print(item)
         url = f"http://www.cbirc.gov.cn/cn/static/data/DocInfo/SelectByDocId/data_docId={item}.json"
         res = requests.get(url)
+        # print(res.json()["data"]["docClob"])
         try:
             table_list = pd.read_html(res.json()["data"]["docClob"])[0]
-            if table_list.shape[1] == 2:
-                table_list = table_list.iloc[:, 1].values.tolist()
-            else:
-                table_list = table_list.iloc[:, 3:].values.tolist()
+            table_list = table_list.iloc[:, 3:].values.tolist()
             # 部分旧表缺少字段，所以填充
             if len(table_list) == 7:
                 table_list.insert(2, pd.NA)
                 table_list.insert(3, pd.NA)
                 table_list.insert(4, pd.NA)
             elif len(table_list) == 8:
                 table_list.insert(1, pd.NA)
                 table_list.insert(2, pd.NA)
             elif len(table_list) == 9:
                 table_list.insert(2, pd.NA)
             elif len(table_list) == 11:
                 table_list = table_list[2:]
                 table_list.insert(2, pd.NA)
-
+                
             # 部分会变成嵌套列表, 这里还原
-            table_list = [
-                item[0] if isinstance(item, list) else item for item in table_list
-            ]
+            table_list = [item[0] if isinstance(
+                item, list) else item for item in table_list]
             table_list.append(str(item))
             table_list.append(res.json()["data"]["publishDate"])
             table_df = pd.DataFrame(table_list)
             table_df.columns = ["内容"]
             big_df = pd.concat([big_df, table_df.T], ignore_index=True)
             # 解决有些页面缺少字段的问题, 都放到 try 里面
         except:
-            warnings.warn(f"{item} is not table, it will be skip")
+            print(f"{item} is not table, it will be skip")
             continue
     big_df.columns = [
         "行政处罚决定书文号",
         "姓名",
         "单位",  # 20200108新增
         "单位名称",
         "主要负责人姓名",
@@ -171,10 +138,10 @@
         "作出处罚决定的日期",
         "处罚ID",
         "处罚公布日期",
     ]
     return big_df
 
 
-if __name__ == "__main__":
-    bank_fjcf_table_detail_df = bank_fjcf_table_detail(page=5, item="分局本级")
+if __name__ == '__main__':
+    bank_fjcf_table_detail_df = bank_fjcf_table_detail(page=2)
     print(bank_fjcf_table_detail_df)
```

### Comparing `akshare-1.9.80/akshare/bank/cons.py` & `akshare-1.9.9/akshare/bank/cons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/3 21:06
+Date: 2019/11/7 15:23
 Desc: 银保监会配置文件
 """
 cbirc_headers_without_cookie_2020 = {
     "Accept": "*/*",
     "Accept-Encoding": "gzip, deflate",
     "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
     "Cache-Control": "no-cache",
```

### Comparing `akshare-1.9.80/akshare/bond/bond_bank.py` & `akshare-1.9.9/akshare/bond/bond_bank.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_cbond.py` & `akshare-1.9.9/akshare/bond/bond_cbond.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_china_money.py` & `akshare-1.9.9/akshare/bond/bond_china_money.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_convert.py` & `akshare-1.9.9/akshare/bond/bond_convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/3/25 17:05
+Date: 2022/9/24 15:05
 Desc: 债券-集思录-可转债
 集思录：https://app.jisilu.cn/data/cbnew/#cb
 """
 import pandas as pd
 import requests
 
 from akshare.utils import demjson
@@ -93,19 +93,20 @@
             "sprice": "正股价",
             "sincrease_rt": "正股涨跌",
             "pb": "正股PB",
             "convert_price": "转股价",
             "convert_value": "转股价值",
             "premium_rt": "转股溢价率",
             "dblow": "双低",
-            "rating_cd": "债券评级",
+            "sw_cd": "下修条件",
+            "rating_cd": "评级",
             "put_convert_price": "回售触发价",
             "force_redeem_price": "强赎触发价",
-            "convert_amt_ratio": "转债占比",
-            "maturity_dt": "到期时间",
+            "convert_amt_ratio": "转债流通市值占比",
+            "short_maturity_dt": "到期时间",
             "year_left": "剩余年限",
             "curr_iss_amt": "剩余规模",
             "volume": "成交额",
             "turnover_rt": "换手率",
             "ytm_rt": "到期税前收益",
         },
         inplace=True,
@@ -121,44 +122,45 @@
             "正股名称",
             "正股价",
             "正股涨跌",
             "正股PB",
             "转股价",
             "转股价值",
             "转股溢价率",
-            "债券评级",
+            "双低",
+            "下修条件",
+            "评级",
             "回售触发价",
             "强赎触发价",
-            "转债占比",
+            "转债流通市值占比",
             "到期时间",
             "剩余年限",
             "剩余规模",
             "成交额",
             "换手率",
             "到期税前收益",
-            "双低",
         ]
     ]
-    temp_df['到期时间'] = pd.to_datetime(temp_df['到期时间']).dt.date
-    temp_df["现价"] = pd.to_numeric(temp_df["现价"], errors="coerce")
-    temp_df["涨跌幅"] = pd.to_numeric(temp_df["涨跌幅"], errors="coerce")
-    temp_df["正股价"] = pd.to_numeric(temp_df["正股价"], errors="coerce")
-    temp_df["正股涨跌"] = pd.to_numeric(temp_df["正股涨跌"], errors="coerce")
-    temp_df["正股PB"] = pd.to_numeric(temp_df["正股PB"], errors="coerce")
-    temp_df["转股价"] = pd.to_numeric(temp_df["转股价"], errors="coerce")
-    temp_df["转股价值"] = pd.to_numeric(temp_df["转股价值"], errors="coerce")
-    temp_df["转股溢价率"] = pd.to_numeric(temp_df["转股溢价率"], errors="coerce")
-    temp_df["回售触发价"] = pd.to_numeric(temp_df["回售触发价"], errors="coerce")
-    temp_df["强赎触发价"] = pd.to_numeric(temp_df["强赎触发价"], errors="coerce")
-    temp_df["转债占比"] = pd.to_numeric(temp_df["转债占比"], errors="coerce")
-    temp_df["剩余年限"] = pd.to_numeric(temp_df["剩余年限"], errors="coerce")
-    temp_df["剩余规模"] = pd.to_numeric(temp_df["剩余规模"], errors="coerce")
-    temp_df["成交额"] = pd.to_numeric(temp_df["成交额"], errors="coerce")
-    temp_df["换手率"] = pd.to_numeric(temp_df["换手率"], errors="coerce")
-    temp_df["到期税前收益"] = pd.to_numeric(temp_df["到期税前收益"], errors="coerce")
+    temp_df["现价"] = pd.to_numeric(temp_df["现价"])
+    temp_df["涨跌幅"] = pd.to_numeric(temp_df["涨跌幅"])
+    temp_df["正股价"] = pd.to_numeric(temp_df["正股价"])
+    temp_df["正股涨跌"] = pd.to_numeric(temp_df["正股涨跌"])
+    temp_df["正股PB"] = pd.to_numeric(temp_df["正股PB"])
+    temp_df["转股价"] = pd.to_numeric(temp_df["转股价"])
+    temp_df["转股价值"] = pd.to_numeric(temp_df["转股价值"])
+    temp_df["转股溢价率"] = pd.to_numeric(temp_df["转股溢价率"])
+    temp_df["双低"] = pd.to_numeric(temp_df["双低"])
+    temp_df["回售触发价"] = pd.to_numeric(temp_df["回售触发价"])
+    temp_df["强赎触发价"] = pd.to_numeric(temp_df["强赎触发价"])
+    temp_df["转债流通市值占比"] = pd.to_numeric(temp_df["转债流通市值占比"])
+    temp_df["剩余年限"] = pd.to_numeric(temp_df["剩余年限"])
+    temp_df["剩余规模"] = pd.to_numeric(temp_df["剩余规模"])
+    temp_df["成交额"] = pd.to_numeric(temp_df["成交额"])
+    temp_df["换手率"] = pd.to_numeric(temp_df["换手率"])
+    temp_df["到期税前收益"] = pd.to_numeric(temp_df["到期税前收益"])
     return temp_df
 
 
 def bond_cb_redeem_jsl() -> pd.DataFrame:
     """
     集思录可转债-强赎
     https://www.jisilu.cn/data/cbnew/#redeem
@@ -192,50 +194,45 @@
     }
     payload = {
         "rp": "50",
     }
     r = requests.post(url, params=params, json=payload, headers=headers)
     data_json = r.json()
     temp_df = pd.DataFrame([item["cell"] for item in data_json["rows"]])
-    temp_df.rename(columns={
-        "bond_id": "代码",
-        "bond_nm": "名称",
-        "price": "现价",
-        "stock_id": "正股代码",
-        "stock_nm": "正股名称",
-        "margin_flg": "-",
-        "btype": "-",
-        "orig_iss_amt": "规模",
-        "curr_iss_amt": "剩余规模",
-        "convert_dt": "转股起始日",
-        "convert_price": "转股价",
-        "next_put_dt": "-",
-        "redeem_dt": "-",
-        "force_redeem": "-",
-        "redeem_flag": "-",
-        "redeem_price": "-",
-        "redeem_price_ratio": "强赎触发比",
-        "real_force_redeem_price": "强赎价",
-        "redeem_remain_days": "-",
-        "redeem_real_days": "-",
-        "redeem_total_days": "-",
-        "recount_dt": "-",
-        "redeem_count_days": "-",
-        "redeem_tc": "强赎条款",
-        "sprice": "正股价",
-        "delist_dt": "-",
-        "maturity_dt": "-",
-        "redeem_icon": "强赎状态",
-        "redeem_orders": "-",
-        "at_maturity": "-",
-        "redeem_count": "强赎天计数",
-        "after_next_put_dt": "-",
-        "force_redeem_price": "强赎触发价",
-    }, inplace=True)
-
+    temp_df.columns = [
+        "代码",
+        "名称",
+        "现价",
+        "正股代码",
+        "正股名称",
+        "-",
+        "-",
+        "规模",
+        "剩余规模",
+        "转股起始日",
+        "转股价",
+        "-",
+        "-",
+        "-",
+        "-",
+        "-",
+        "强赎触发比",
+        "强赎价",
+        "-",
+        "-",
+        "-",
+        "-",
+        "强赎条款",
+        "正股价",
+        "强赎状态",
+        "-",
+        "强赎天计数",
+        "-",
+        "强赎触发价",
+    ]
     temp_df = temp_df[
         [
             "代码",
             "名称",
             "现价",
             "正股代码",
             "正股名称",
@@ -248,22 +245,22 @@
             "正股价",
             "强赎价",
             "强赎天计数",
             "强赎条款",
             "强赎状态",
         ]
     ]
-    temp_df["现价"] = pd.to_numeric(temp_df["现价"], errors="coerce")
-    temp_df["规模"] = pd.to_numeric(temp_df["规模"], errors="coerce")
-    temp_df["剩余规模"] = pd.to_numeric(temp_df["剩余规模"], errors="coerce")
+    temp_df["现价"] = pd.to_numeric(temp_df["现价"])
+    temp_df["规模"] = pd.to_numeric(temp_df["规模"])
+    temp_df["剩余规模"] = pd.to_numeric(temp_df["剩余规模"])
     temp_df["转股起始日"] = pd.to_datetime(temp_df["转股起始日"]).dt.date
-    temp_df["转股价"] = pd.to_numeric(temp_df["转股价"], errors="coerce")
-    temp_df["强赎触发比"] = pd.to_numeric(temp_df["强赎触发比"].str.strip("%"), errors="coerce")
-    temp_df["强赎触发价"] = pd.to_numeric(temp_df["强赎触发价"], errors="coerce")
-    temp_df["正股价"] = pd.to_numeric(temp_df["正股价"], errors="coerce")
+    temp_df["转股价"] = pd.to_numeric(temp_df["转股价"])
+    temp_df["强赎触发比"] = pd.to_numeric(temp_df["强赎触发比"].str.strip("%"))
+    temp_df["强赎触发价"] = pd.to_numeric(temp_df["强赎触发价"])
+    temp_df["正股价"] = pd.to_numeric(temp_df["正股价"])
     temp_df["强赎价"] = pd.to_numeric(temp_df["强赎价"], errors="coerce")
     temp_df["强赎天计数"] = temp_df["强赎天计数"].replace(
         r"^.*?(\d{1,2}\/\d{1,2} \| \d{1,2}).*?$", r"\1", regex=True
     )
     temp_df["强赎状态"] = temp_df["强赎状态"].map(
         {"R": "已公告强赎", "O": "公告要强赎", "G": "公告不强赎", "B": "已满足强赎条件", "": ""}
     )
@@ -285,20 +282,19 @@
     if "</table>" not in data_text:
         # 1. 该可转债没有转股价调整记录，服务端返回文本 '暂无数据'
         # 2. 无效可转债代码，服务端返回 {"timestamp":1639565628,"isError":1,"msg":"无效代码格式"}
         # 以上两种情况，返回空的 DataFrame
         return
     else:
         temp_df = pd.read_html(data_text, parse_dates=True)[0]
-        temp_df.columns = [item.replace(" ", "") for item in temp_df.columns]
-        temp_df["下修前转股价"] = pd.to_numeric(temp_df["下修前转股价"], errors="coerce")
-        temp_df["下修后转股价"] = pd.to_numeric(temp_df["下修后转股价"], errors="coerce")
-        temp_df["下修底价"] = pd.to_numeric(temp_df["下修底价"], errors="coerce")
         temp_df["股东大会日"] = pd.to_datetime(temp_df["股东大会日"]).dt.date
+        temp_df["下修前转股价"] = pd.to_numeric(temp_df["下修前转股价"])
+        temp_df["下修后转股价"] = pd.to_numeric(temp_df["下修后转股价"])
         temp_df["新转股价生效日期"] = pd.to_datetime(temp_df["新转股价生效日期"]).dt.date
+        temp_df["下修底价"] = pd.to_numeric(temp_df["下修底价"])
         return temp_df
 
 
 if __name__ == "__main__":
     bond_cb_index_jsl_df = bond_cb_index_jsl()
     print(bond_cb_index_jsl_df)
```

### Comparing `akshare-1.9.80/akshare/bond/bond_em.py` & `akshare-1.9.9/akshare/bond/bond_em.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2022/4/23 17:18
+Date: 2022/3/5 14:18
 Desc: 东方财富网-数据中心-经济数据-中美国债收益率
-https://data.eastmoney.com/cjsj/zmgzsyl.html
+http://data.eastmoney.com/cjsj/zmgzsyl.html
 """
 import pandas as pd
 import requests
 from tqdm import tqdm
 
 
-def bond_zh_us_rate(start_date: str = "19901219") -> pd.DataFrame:
+def bond_zh_us_rate() -> pd.DataFrame:
     """
     东方财富网-数据中心-经济数据-中美国债收益率
-    https://data.eastmoney.com/cjsj/zmgzsyl.html
+    http://data.eastmoney.com/cjsj/zmgzsyl.html
     :return: 中美国债收益率
     :rtype: pandas.DataFrame
     """
     url = "http://datacenter.eastmoney.com/api/data/get"
     params = {
         "type": "RPTA_WEB_TREASURYYIELD",
         "sty": "ALL",
@@ -47,20 +47,14 @@
             "pageNum": page,
             "_": "1615791534490",
         }
         r = requests.get(url, params=params)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["result"]["data"])
         big_df = pd.concat([big_df, temp_df], ignore_index=True)
-        temp_date_list = pd.to_datetime(big_df["SOLAR_DATE"]).dt.date.to_list()
-        if pd.to_datetime(start_date) in pd.date_range(
-            temp_date_list[-1], temp_date_list[0]
-        ):
-            break
-
     big_df.rename(
         columns={
             "SOLAR_DATE": "日期",
             "EMM00166462": "中国国债收益率5年",
             "EMM00166466": "中国国债收益率10年",
             "EMM00166469": "中国国债收益率30年",
             "EMM00588704": "中国国债收益率2年",
@@ -88,31 +82,28 @@
             "美国国债收益率5年",
             "美国国债收益率10年",
             "美国国债收益率30年",
             "美国国债收益率10年-2年",
             "美国GDP年增率",
         ]
     ]
-    big_df["日期"] = pd.to_datetime(big_df["日期"])
-    big_df["中国国债收益率2年"] = pd.to_numeric(big_df["中国国债收益率2年"], errors="coerce")
-    big_df["中国国债收益率5年"] = pd.to_numeric(big_df["中国国债收益率5年"], errors="coerce")
-    big_df["中国国债收益率10年"] = pd.to_numeric(big_df["中国国债收益率10年"], errors="coerce")
-    big_df["中国国债收益率30年"] = pd.to_numeric(big_df["中国国债收益率30年"], errors="coerce")
-    big_df["中国国债收益率10年-2年"] = pd.to_numeric(big_df["中国国债收益率10年-2年"], errors="coerce")
-    big_df["中国GDP年增率"] = pd.to_numeric(big_df["中国GDP年增率"], errors="coerce")
-    big_df["美国国债收益率2年"] = pd.to_numeric(big_df["美国国债收益率2年"], errors="coerce")
-    big_df["美国国债收益率5年"] = pd.to_numeric(big_df["美国国债收益率5年"], errors="coerce")
-    big_df["美国国债收益率10年"] = pd.to_numeric(big_df["美国国债收益率10年"], errors="coerce")
-    big_df["美国国债收益率30年"] = pd.to_numeric(big_df["美国国债收益率30年"], errors="coerce")
-    big_df["美国国债收益率10年-2年"] = pd.to_numeric(big_df["美国国债收益率10年-2年"], errors="coerce")
-    big_df["美国GDP年增率"] = pd.to_numeric(big_df["美国GDP年增率"], errors="coerce")
-    big_df.sort_values("日期", inplace=True)
-    big_df.set_index(["日期"], inplace=True)
-    big_df = big_df[pd.to_datetime(start_date) :]
-    big_df.reset_index(inplace=True)
     big_df["日期"] = pd.to_datetime(big_df["日期"]).dt.date
+    big_df["中国国债收益率2年"] = pd.to_numeric(big_df["中国国债收益率2年"])
+    big_df["中国国债收益率5年"] = pd.to_numeric(big_df["中国国债收益率5年"])
+    big_df["中国国债收益率10年"] = pd.to_numeric(big_df["中国国债收益率10年"])
+    big_df["中国国债收益率30年"] = pd.to_numeric(big_df["中国国债收益率30年"])
+    big_df["中国国债收益率10年-2年"] = pd.to_numeric(big_df["中国国债收益率10年-2年"])
+    big_df["中国GDP年增率"] = pd.to_numeric(big_df["中国GDP年增率"])
+    big_df["美国国债收益率2年"] = pd.to_numeric(big_df["美国国债收益率2年"])
+    big_df["美国国债收益率5年"] = pd.to_numeric(big_df["美国国债收益率5年"])
+    big_df["美国国债收益率10年"] = pd.to_numeric(big_df["美国国债收益率10年"])
+    big_df["美国国债收益率30年"] = pd.to_numeric(big_df["美国国债收益率30年"])
+    big_df["美国国债收益率10年-2年"] = pd.to_numeric(big_df["美国国债收益率10年-2年"])
+    big_df["美国GDP年增率"] = pd.to_numeric(big_df["美国GDP年增率"])
+    big_df.sort_values("日期", inplace=True)
+    big_df.reset_index(inplace=True, drop=True)
     return big_df
 
 
 if __name__ == "__main__":
-    bond_zh_us_rate_df = bond_zh_us_rate(start_date="19901219")
+    bond_zh_us_rate_df = bond_zh_us_rate()
     print(bond_zh_us_rate_df)
```

### Comparing `akshare-1.9.80/akshare/bond/bond_futures.py` & `akshare-1.9.9/akshare/bond/bond_futures.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_info_cm.py` & `akshare-1.9.9/akshare/bond/bond_info_cm.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_investing.py` & `akshare-1.9.9/akshare/bond/bond_investing.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_issue_cninfo.py` & `akshare-1.9.9/akshare/bond/bond_issue_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_summary.py` & `akshare-1.9.9/akshare/bond/bond_summary.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_zh_cov_sina.py` & `akshare-1.9.9/akshare/bond/bond_zh_cov_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/bond_zh_sina.py` & `akshare-1.9.9/akshare/bond/bond_zh_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/china_bond.py` & `akshare-1.9.9/akshare/bond/china_bond.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/23 17:24
+Date: 2022/4/1 17:24
 Desc: 中国外汇交易中心暨全国银行间同业拆借中心
 中国外汇交易中心暨全国银行间同业拆借中心-市场数据-债券市场行情-现券市场做市报价
 中国外汇交易中心暨全国银行间同业拆借中心-市场数据-债券市场行情-现券市场成交行情
 http://www.chinamoney.com.cn/chinese/mkdatabond/
 """
 import pandas as pd
 import requests
@@ -154,23 +154,24 @@
     }
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.130 Safari/537.36",
     }
     res = requests.get(url, params=params, headers=headers)
     data_text = res.text.replace("&nbsp", "")
     data_df = pd.read_html(data_text, header=0)[1]
+
     data_df['日期'] = pd.to_datetime(data_df['日期']).dt.date
-    data_df['3月'] = pd.to_numeric(data_df['3月'], errors="coerce")
-    data_df['6月'] = pd.to_numeric(data_df['6月'], errors="coerce")
-    data_df['1年'] = pd.to_numeric(data_df['1年'], errors="coerce")
-    data_df['3年'] = pd.to_numeric(data_df['3年'], errors="coerce")
-    data_df['5年'] = pd.to_numeric(data_df['5年'], errors="coerce")
-    data_df['7年'] = pd.to_numeric(data_df['7年'], errors="coerce")
-    data_df['10年'] = pd.to_numeric(data_df['10年'], errors="coerce")
-    data_df['30年'] = pd.to_numeric(data_df['30年'], errors="coerce")
+    data_df['3月'] = pd.to_numeric(data_df['3月'])
+    data_df['6月'] = pd.to_numeric(data_df['6月'])
+    data_df['1年'] = pd.to_numeric(data_df['1年'])
+    data_df['3年'] = pd.to_numeric(data_df['3年'])
+    data_df['5年'] = pd.to_numeric(data_df['5年'])
+    data_df['7年'] = pd.to_numeric(data_df['7年'])
+    data_df['10年'] = pd.to_numeric(data_df['10年'])
+    data_df['30年'] = pd.to_numeric(data_df['30年'])
     data_df.sort_values('日期', inplace=True)
     data_df.reset_index(inplace=True, drop=True)
     return data_df
 
 
 if __name__ == "__main__":
     bond_spot_quote_df = bond_spot_quote()
```

### Comparing `akshare-1.9.80/akshare/bond/china_repo.py` & `akshare-1.9.9/akshare/bond/china_repo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/bond/cons.py` & `akshare-1.9.9/akshare/bond/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/cost/cost_living.py` & `akshare-1.9.9/akshare/cost/cost_living.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/crypto/crypto_bitcoin_cme.py` & `akshare-1.9.9/akshare/crypto/crypto_bitcoin_cme.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/crypto/crypto_crix.py` & `akshare-1.9.9/akshare/crypto/crypto_crix.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/crypto/crypto_hist_investing.py` & `akshare-1.9.9/akshare/crypto/crypto_hist_investing.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/crypto/crypto_hold.py` & `akshare-1.9.9/akshare/crypto/crypto_hold.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/currency/currency.py` & `akshare-1.9.9/akshare/currency/currency.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/currency/currency_china_bank_sina.py` & `akshare-1.9.9/akshare/currency/currency_china_bank_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/currency/currency_safe.py` & `akshare-1.9.9/akshare/currency/currency_safe.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/data/covid.js` & `akshare-1.9.9/akshare/data/covid.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/data/crypto_info.zip` & `akshare-1.9.9/akshare/data/crypto_info.zip`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/data/ths.js` & `akshare-1.9.9/akshare/data/ths.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/datasets.py` & `akshare-1.9.9/akshare/datasets.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/cons.py` & `akshare-1.9.9/akshare/economic/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_australia.py` & `akshare-1.9.9/akshare/economic/macro_australia.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_bank.py` & `akshare-1.9.9/akshare/economic/macro_bank.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_canada.py` & `akshare-1.9.9/akshare/economic/macro_canada.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_china.py` & `akshare-1.9.9/akshare/economic/macro_china.py`

 * *Files 1% similar despite different names*

```diff
@@ -1381,16 +1381,28 @@
     params = {
         "max_date": "",
         "category": "fs",
         "attr_id": "1",
         "_": str(int(round(t * 1000))),
     }
     headers = {
-        'x-app-id': 'rU6QIu7JHe2gOUeR',
-        'x-version': '1.0.0'
+        "accept": "*/*",
+        "accept-encoding": "gzip, deflate, br",
+        "accept-language": "zh-CN,zh;q=0.9,en;q=0.8",
+        "cache-control": "no-cache",
+        "origin": "https://datacenter.jin10.com",
+        "pragma": "no-cache",
+        "referer": "https://datacenter.jin10.com/reportType/dc_market_margin_sse",
+        "sec-fetch-dest": "empty",
+        "sec-fetch-mode": "cors",
+        "sec-fetch-site": "same-site",
+        "x-app-id": "rU6QIu7JHe2gOUeR",
+        "x-csrf-token": "",
+        "x-version": "1.0.0",
+        "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.135 Safari/537.36",
     }
     r = requests.get(url, params=params, headers=headers)
     temp_df = pd.DataFrame(r.json()["data"]["values"])
     temp_df.index = pd.to_datetime(temp_df.iloc[:, 0])
     temp_df = temp_df.iloc[:, 1:]
     temp_df.columns = [item["name"] for item in r.json()["data"]["keys"]][1:]
 
@@ -1406,22 +1418,19 @@
             "_": str(int(round(t * 1000))),
         }
         r = requests.get(url, params=params, headers=headers)
         temp_df = pd.DataFrame(r.json()["data"]["values"])
         temp_df.index = pd.to_datetime(temp_df.iloc[:, 0])
         temp_df = temp_df.iloc[:, 1:]
         temp_df.columns = [item["name"] for item in r.json()["data"]["keys"]][1:]
-        big_df = pd.concat([big_df, temp_df])
+        big_df = big_df.append(temp_df)
 
-    value_df = pd.concat([value_df, big_df])
+    value_df = value_df.append(big_df)
     value_df.drop_duplicates(inplace=True)
     value_df.sort_index(inplace=True)
-    value_df.reset_index(inplace=True)
-    value_df.rename(columns={"index": "日期"}, inplace=True)
-    value_df['日期'] = pd.to_datetime(value_df['日期']).dt.date
     return value_df
 
 
 # 金十数据中心-经济指标-中国-其他-上海黄金交易所报告
 def macro_china_au_report() -> pd.DataFrame:
     """
     上海黄金交易所报告, 数据区间从20100331-至今
@@ -1450,37 +1459,18 @@
             "成交量",
             "成交金额",
             "持仓量",
             "交收方向",
             "交收量",
             "日期",
         ]
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
-    big_df = big_df[
-        [
-            "日期",
-            "商品",
-            "开盘价",
-            "最高价",
-            "最低价",
-            "收盘价",
-            "涨跌",
-            "涨跌幅",
-            "加权平均价",
-            "成交量",
-            "成交金额",
-            "持仓量",
-            "交收方向",
-            "交收量",
-        ]
-    ]
-    big_df["日期"] = pd.to_datetime(big_df["日期"]).dt.date
-    big_df.sort_values(["日期"], inplace=True, ignore_index=True)
-    big_df["持仓量"] = pd.to_numeric(big_df["持仓量"], errors="coerce")
-    big_df["交收量"] = pd.to_numeric(big_df["交收量"], errors="coerce")
+        big_df = big_df.append(temp_df, ignore_index=True)
+    big_df.index = pd.to_datetime(big_df["日期"])
+    del big_df["日期"]
+    big_df.sort_index(inplace=True)
     return big_df
 
 
 # 发改委-中国电煤价格指数-全国综合电煤价格指数
 def macro_china_ctci() -> pd.DataFrame:
     """
     中国电煤价格指数-全国综合电煤价格指数
@@ -2498,15 +2488,15 @@
     big_df.sort_values(["日期"], inplace=True)
     big_df.reset_index(inplace=True, drop=True)
     return big_df
 
 
 def _em_macro_1(em_id) -> pd.DataFrame:
     """
-    东财宏观数据的一种通用函数
+    获取东财宏观数据的一种通用函数1
     """
     url = "https://datacenter-web.eastmoney.com/api/data/v1/get"
     ind_id = '"' + em_id + '"'
     params = {
         "sortColumns": "REPORT_DATE",
         "sortTypes": "-1",
         "pageSize": "500",
@@ -2549,15 +2539,15 @@
     big_df.sort_values(["日期"], inplace=True)
     big_df.reset_index(inplace=True, drop=True)
     return big_df
 
 
 def macro_shipping_bci() -> pd.DataFrame:
     """
-    海岬型运费指数(BCI)
+    海岬型运费指数（BCI）
     https://data.eastmoney.com/cjsj/hyzs_list_EMI00107666.html
     :return: 海岬型运费指数
     :rtype: pandas.DataFrame
     """
     ts = _em_macro_1("EMI00107666")
     return ts
```

### Comparing `akshare-1.9.80/akshare/economic/macro_china_hk.py` & `akshare-1.9.9/akshare/economic/macro_china_hk.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_constitute.py` & `akshare-1.9.9/akshare/economic/macro_constitute.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_euro.py` & `akshare-1.9.9/akshare/economic/macro_euro.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_germany.py` & `akshare-1.9.9/akshare/economic/macro_germany.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_japan.py` & `akshare-1.9.9/akshare/economic/macro_japan.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_other.py` & `akshare-1.9.9/akshare/economic/macro_other.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_swiss.py` & `akshare-1.9.9/akshare/economic/macro_swiss.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_uk.py` & `akshare-1.9.9/akshare/economic/macro_uk.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/economic/macro_usa.py` & `akshare-1.9.9/akshare/economic/macro_usa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/10 17:00
+Date: 2022/11/27 19:08
 Desc: 金十数据中心-经济指标-美国
 https://datacenter.jin10.com/economic
 """
 import json
 import time
 
 import pandas as pd
@@ -79,26 +79,26 @@
 def macro_usa_gdp_monthly() -> pd.DataFrame:
     """
     金十数据-美国国内生产总值(GDP)报告, 数据区间从 20080228-至今
     https://datacenter.jin10.com/reportType/dc_usa_gdp
     :return: pandas.Series
     """
     t = time.time()
-    r = requests.get(
+    res = requests.get(
         JS_USA_GDP_MONTHLY_URL.format(
             str(int(round(t * 1000))), str(int(round(t * 1000)) + 90)
         )
     )
-    json_data = json.loads(r.text[r.text.find("{") : r.text.rfind("}") + 1])
+    json_data = json.loads(res.text[res.text.find("{") : res.text.rfind("}") + 1])
     date_list = [item["date"] for item in json_data["list"]]
     value_list = [item["datas"]["美国国内生产总值(GDP)"] for item in json_data["list"]]
     value_df = pd.DataFrame(value_list)
     value_df.columns = json_data["kinds"]
     value_df.index = pd.to_datetime(date_list)
-
+    temp_df = value_df["今值(%)"]
     url = "https://datacenter-api.jin10.com/reports/list_v2"
     params = {
         "max_date": "",
         "category": "ec",
         "attr_id": "53",
         "_": str(int(round(t * 1000))),
     }
@@ -115,29 +115,27 @@
         "sec-fetch-site": "same-site",
         "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36",
         "x-app-id": "rU6QIu7JHe2gOUeR",
         "x-csrf-token": "",
         "x-version": "1.0.0",
     }
     r = requests.get(url, params=params, headers=headers)
-    temp_df = pd.DataFrame(r.json()["data"]["values"])
-    temp_df.index = pd.to_datetime(temp_df.iloc[:, 0])
-    temp_df.columns = ['date'] + json_data["kinds"]
-    del temp_df['date']
-    temp_df = pd.concat([value_df, temp_df])
-
-    temp_df.dropna(subset=["预测值(%)"], inplace=True)
+    temp_se = pd.DataFrame(r.json()["data"]["values"]).iloc[:, :2]
+    temp_se.index = pd.to_datetime(temp_se.iloc[:, 0])
+    temp_se = temp_se.iloc[:, 1]
+    temp_df = temp_df.append(temp_se)
+    temp_df.dropna(inplace=True)
     temp_df.sort_index(inplace=True)
     temp_df = temp_df.reset_index()
     temp_df.drop_duplicates(subset="index", inplace=True)
-    temp_df.columns = ['日期', '今值', '预测值', '前值']
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
-    temp_df['今值'] = pd.to_numeric(temp_df['今值'], errors="coerce")
-    temp_df['预测值'] = pd.to_numeric(temp_df['预测值'], errors="coerce")
-    temp_df['前值'] = pd.to_numeric(temp_df['前值'], errors="coerce")
+    temp_df.set_index("index", inplace=True)
+    temp_df = temp_df.squeeze()
+    temp_df.index.name = None
+    temp_df.name = "gdp"
+    temp_df = temp_df.astype("float")
     return temp_df
 
 
 # 金十数据中心-经济指标-美国-物价水平-美国CPI月率报告
 def macro_usa_cpi_monthly() -> pd.DataFrame:
     """
     美国CPI月率报告, 数据区间从19700101-至今
```

### Comparing `akshare-1.9.80/akshare/economic/marco_cnbs.py` & `akshare-1.9.9/akshare/economic/marco_cnbs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/3/22 20:22
+Date: 2022/2/9 12:22
 Desc: 国家金融与发展实验室-中国宏观杠杆率数据
 http://114.115.232.154:8080/
 """
 import pandas as pd
 
 
 def macro_cnbs() -> pd.DataFrame:
@@ -28,21 +28,21 @@
         "政府部门",
         "中央政府",
         "地方政府",
         "实体经济部门",
         "金融部门资产方",
         "金融部门负债方",
     ]
-    temp_df["居民部门"] = pd.to_numeric(temp_df["居民部门"], errors="coerce")
-    temp_df["非金融企业部门"] = pd.to_numeric(temp_df["非金融企业部门"], errors="coerce")
-    temp_df["政府部门"] = pd.to_numeric(temp_df["政府部门"], errors="coerce")
-    temp_df["中央政府"] = pd.to_numeric(temp_df["中央政府"], errors="coerce")
-    temp_df["地方政府"] = pd.to_numeric(temp_df["地方政府"], errors="coerce")
-    temp_df["实体经济部门"] = pd.to_numeric(temp_df["实体经济部门"], errors="coerce")
-    temp_df["金融部门资产方"] = pd.to_numeric(temp_df["金融部门资产方"], errors="coerce")
-    temp_df["金融部门负债方"] = pd.to_numeric(temp_df["金融部门负债方"], errors="coerce")
+    temp_df["居民部门"] = pd.to_numeric(temp_df["居民部门"])
+    temp_df["非金融企业部门"] = pd.to_numeric(temp_df["非金融企业部门"])
+    temp_df["政府部门"] = pd.to_numeric(temp_df["政府部门"])
+    temp_df["中央政府"] = pd.to_numeric(temp_df["中央政府"])
+    temp_df["地方政府"] = pd.to_numeric(temp_df["地方政府"])
+    temp_df["实体经济部门"] = pd.to_numeric(temp_df["实体经济部门"])
+    temp_df["金融部门资产方"] = pd.to_numeric(temp_df["金融部门资产方"])
+    temp_df["金融部门负债方"] = pd.to_numeric(temp_df["金融部门负债方"])
     return temp_df
 
 
 if __name__ == "__main__":
     macro_cnbs_df = macro_cnbs()
     print(macro_cnbs_df)
```

### Comparing `akshare-1.9.80/akshare/energy/energy_carbon.py` & `akshare-1.9.9/akshare/energy/energy_carbon.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/energy/energy_oil_em.py` & `akshare-1.9.9/akshare/energy/energy_oil_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/event/cons.py` & `akshare-1.9.9/akshare/event/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/event/covid.py` & `akshare-1.9.9/akshare/event/covid.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/file_fold/calendar.json` & `akshare-1.9.9/akshare/file_fold/calendar.json`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fortune/fortune_500.py` & `akshare-1.9.9/akshare/fortune/fortune_500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fortune/fortune_bloomberg.py` & `akshare-1.9.9/akshare/fortune/fortune_bloomberg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fortune/fortune_forbes_500.py` & `akshare-1.9.9/akshare/fortune/fortune_forbes_500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fortune/fortune_hurun.py` & `akshare-1.9.9/akshare/fortune/fortune_hurun.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fortune/fortune_it_juzi.py` & `akshare-1.9.9/akshare/fortune/fortune_it_juzi.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fortune/fortune_xincaifu_500.py` & `akshare-1.9.9/akshare/fortune/fortune_xincaifu_500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fund/fund_amac.py` & `akshare-1.9.9/akshare/fund/fund_amac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-#!/usr/bin/env python
-# -*- coding:utf-8 -*-
 """
-Date: 2023/4/3 20:48
+Date: 2021/11/16 15:48
 Desc: 中国证券投资基金业协会-信息公示数据
-中国证券投资基金业协会-新版: https://gs.amac.org.cn
+中国证券投资基金业协会-新版: http://gs.amac.org.cn
+中国证券投资基金业协会-旧版: http://www1.amac.org.cn/
+目前的网络数据采集基于旧版接口, Guo Yangyang 正在更新新版接口数据
+接口目录设计按照 http://gs.amac.org.cn/ 来设计, 已经整理完该页面所有接口
 """
 import pandas as pd
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
 from tqdm import tqdm
 
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
@@ -359,15 +360,15 @@
 
 
 # 中国证券投资基金业协会-信息公示-基金产品
 # 中国证券投资基金业协会-信息公示-基金产品-私募基金管理人基金产品
 def amac_fund_info(start_page: str = '1', end_page: str = "2000") -> pd.DataFrame:
     """
     中国证券投资基金业协会-信息公示-基金产品-私募基金管理人基金产品
-    https://gs.amac.org.cn/amac-infodisc/res/pof/fund/index.html
+    http://gs.amac.org.cn/amac-infodisc/res/pof/fund/index.html
     :param start_page: 开始页码, 获取指定页码直接的数据
     :type start_page: str
     :param end_page: 结束页码, 获取指定页码直接的数据
     :type end_page: str
     :return: 私募基金管理人基金产品
     :rtype: pandas.DataFrame
     """
@@ -386,15 +387,15 @@
         real_end_page = total_page
     big_df = pd.DataFrame()
     for page in tqdm(range(int(start_page) - 1, real_end_page), leave=False):
         params.update({"page": page})
         r = requests.post(url, params=params, json={}, verify=False)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["content"])
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
+        big_df = big_df.append(temp_df, ignore_index=True)
     keys_list = [
         "fundName",
         "managerName",
         "managerType",
         "workingState",
         "putOnRecordDate",
         "establishDate",
@@ -790,15 +791,15 @@
 
     # 中国证券投资基金业协会-信息公示-私募基金管理人公示-证券公司私募基金子公司管理人信息公示
     amac_member_sub_info_df = amac_member_sub_info()
     print(amac_member_sub_info_df)
 
     # 中国证券投资基金业协会-信息公示-基金产品
     # 中国证券投资基金业协会-信息公示-基金产品-私募基金管理人基金产品
-    amac_fund_info_df = amac_fund_info(start_page="1", end_page='100')
+    amac_fund_info_df = amac_fund_info(start_page="1", end_page='5')
     print(amac_fund_info_df)
     example_df = amac_fund_info_df[amac_fund_info_df["私募基金管理人名称"].str.contains("聚宽")]
     print(example_df)
 
     # 中国证券投资基金业协会-信息公示-基金产品-证券公司集合资管产品公示
     amac_securities_info_df = amac_securities_info()
     print(amac_securities_info_df)
```

### Comparing `akshare-1.9.80/akshare/fund/fund_aum_em.py` & `akshare-1.9.9/akshare/fund/fund_aum_em.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/3 20:32
+Date: 2021/10/7 13:32
 Desc: 东方财富-基金
 """
 import pandas as pd
 import requests
 
 
 def fund_aum_em() -> pd.DataFrame:
     """
     东方财富-基金-基金公司排名列表
-    https://fund.eastmoney.com/Company/lsgm.html
+    http://fund.eastmoney.com/Company/lsgm.html
     :return: 基金公司排名列表
     :rtype: pandas.DataFrame
     """
     url = 'http://fund.eastmoney.com/Company/home/gspmlist'
     params = {
         'fundType': '0'
     }
@@ -32,15 +32,15 @@
     temp_df['全部经理数'] = pd.to_numeric(temp_df['全部经理数'])
     return temp_df
 
 
 def fund_aum_trend_em() -> pd.DataFrame:
     """
     东方财富-基金-基金市场管理规模走势图
-    https://fund.eastmoney.com/Company/default.html
+    http://fund.eastmoney.com/Company/default.html
     :return: 基金市场管理规模走势图
     :rtype: pandas.DataFrame
     """
     url = 'http://fund.eastmoney.com/Company/home/GetFundTotalScaleForChart'
     payload = {
         'fundType': '0'
     }
@@ -51,15 +51,15 @@
     temp_df['value'] = data_json['y']
     return temp_df
 
 
 def fund_aum_hist_em(year: str = "2019") -> pd.DataFrame:
     """
     东方财富-基金-基金公司历年管理规模排行列表
-    https://fund.eastmoney.com/Company/lsgm.html
+    http://fund.eastmoney.com/Company/lsgm.html
     :return: 基金公司历年管理规模排行列表
     :rtype: pandas.DataFrame
     """
     url = 'http://fund.eastmoney.com/Company/home/HistoryScaleTable'
     params = {
         'year': year
     }
```

### Comparing `akshare-1.9.80/akshare/fund/fund_em.py` & `akshare-1.9.9/akshare/fund/fund_em.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/3/24 14:20
+Date: 2022/11/14 19:50
 Desc: 东方财富网站-天天基金网-基金数据-开放式基金净值
 https://fund.eastmoney.com/manager/default.html#dt14;mcreturnjson;ftall;pn20;pi1;scabbname;stasc
 1.基金经理基本数据, 建议包含:基金经理代码,基金经理姓名,从业起始日期,现任基金公司,管理资产总规模,上述数据可在"基金经理列表: http://fund.eastmoney.com/manager/default.html#dt14;mcreturnjson;ftall;pn20;pi1;scabbname;stasc 和"基金经理理档案如:http://fund.eastmoney.com/manager/30040164.html 获取.
 2.基金经理任职数据:可调取全部或特定经理,管理的基金数据,建议包含:基金经理代码,基金经理姓名,基金代码,基金简称,经理位次(在当前基金的经理中排第几位),起始任职时间,截止任职时间,任职回报.在特定基金的经理信息中可以获取如:http://fundf10.eastmoney.com/jjjl_001810.html
 3.在接口：fund_basic"公募基金列表"增加数据"基金经理代码"(或第一基金经理代码),"基金经理姓名"(或第一基金经理姓名),"当前基金经理人数","当前经理任职起始时间".
 用户ID:269993
 """
-import json
 import time
+import json
 
+from akshare.utils import demjson
 import pandas as pd
 import requests
 
-from akshare.utils import demjson
-
 
 def fund_purchase_em() -> pd.DataFrame:
     """
     东方财富网站-天天基金网-基金数据-基金申购状态
     https://fund.eastmoney.com/Fund_sgzt_bzdm.html#fcode,asc_1
     :return: 基金申购状态
     :rtype: pandas.DataFrame
@@ -127,15 +126,15 @@
     }
     indicator_map = {
         "全部": "",
         "被动指数型": "051",
         "增强指数型": "052",
     }
     url = "http://api.fund.eastmoney.com/FundTradeRank/GetRankList"
-    if symbol in {"股票指数", "债券指数"}:
+    if symbol in {"股票指数", "股票指数"}:
         params = {
             "ft": "zs",
             "sc": "1n",
             "st": "desc",
             "pi": "1",
             "pn": "10000",
             "cp": "",
@@ -681,62 +680,57 @@
             "封闭期",
             "申购状态",
         ]
     ]
     return data_df
 
 
-def fund_financial_fund_info_em(symbol: str = "000134") -> pd.DataFrame:
+def fund_financial_fund_info_em(fund: str = "000134") -> pd.DataFrame:
     """
-    东方财富网站-天天基金网-基金数据-理财型基金收益-历史净值明细
-    https://fundf10.eastmoney.com/jjjz_000791.html
-    :param symbol: 理财型基金代码, 可以通过 ak.fund_financial_fund_daily_em() 来获取
-    :type symbol: str
-    :return: 东方财富网站-天天基金网-基金数据-理财型基金收益-历史净值明细
+    东方财富网站-天天基金网-基金数据-理财型基金收益-历史净值数据
+    http://fundf10.eastmoney.com/jjjz_000791.html
+    :param fund: 理财型基金代码, 可以通过 fund_financial_fund_daily_em 来获取
+    :type fund: str
+    :return: 东方财富网站-天天基金网-基金数据-理财型基金收益-历史净值数据
     :rtype: pandas.DataFrame
     """
     url = "http://api.fund.eastmoney.com/f10/lsjz"
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.149 Safari/537.36",
-        "Referer": f"http://fundf10.eastmoney.com/jjjz_{symbol}.html",
+        "Referer": f"http://fundf10.eastmoney.com/jjjz_{fund}.html",
     }
     params = {
         "callback": "jQuery18307915911837995662_1588249228826",
-        "fundCode": symbol,
+        "fundCode": fund,
         "pageIndex": "1",
         "pageSize": "10000",
         "startDate": "",
         "endDate": "",
         "_": round(time.time() * 1000),
     }
     r = requests.get(url, params=params, headers=headers)
     text_data = r.text
     data_json = demjson.decode(text_data[text_data.find("{") : -1])
     temp_df = pd.DataFrame(data_json["Data"]["LSJZList"])
     temp_df.columns = [
         "净值日期",
-        "单位净值",
-        "累计净值",
+        "每万份收益",
+        "7日年化收益率",
+        "_",
         "_",
         "_",
         "_",
-        "日增长率",
         "申购状态",
         "赎回状态",
         "_",
         "_",
         "_",
-        "分红送配",
+        "_",
     ]
-    temp_df = temp_df[["净值日期", "单位净值", "累计净值", "日增长率", "申购状态", "赎回状态", "分红送配"]]
-    temp_df.sort_values(['净值日期'], inplace=True, ignore_index=True)
-    temp_df['净值日期'] = pd.to_datetime(temp_df['净值日期']).dt.date
-    temp_df['单位净值'] = pd.to_numeric(temp_df['单位净值'], errors="coerce")
-    temp_df['累计净值'] = pd.to_numeric(temp_df['累计净值'], errors="coerce")
-    temp_df['日增长率'] = pd.to_numeric(temp_df['日增长率'], errors="coerce")
+    temp_df = temp_df[["净值日期", "每万份收益", "7日年化收益率", "申购状态", "赎回状态"]]
     return temp_df
 
 
 def fund_graded_fund_daily_em() -> pd.DataFrame:
     """
     东方财富网站-天天基金网-基金数据-分级基金净值
     http://fund.eastmoney.com/fjjj.html#1_1__0__zdf,desc_1
@@ -1035,16 +1029,16 @@
 
 
 def fund_hk_fund_hist_em(
     code: str = "1002200683", symbol: str = "历史净值明细"
 ) -> pd.DataFrame:
     """
     东方财富网-天天基金网-基金数据-香港基金-历史净值明细(分红送配详情)
-    https://overseas.1234567.com.cn/f10/FundJz/968092#FHPS
-    :param code: 通过 ak.fund_em_hk_rank() 获取
+    http://overseas.1234567.com.cn/f10/FundJz/968092#FHPS
+    :param code: 通过 fund_em_hk_rank 获取
     :type code: str
     :param symbol: choice of {"历史净值明细", "分红送配详情"}
     :type symbol: str
     :return: 香港基金-历史净值明细(分红送配详情)
     :rtype: pandas.DataFrame
     """
     url = "http://overseas.1234567.com.cn/overseasapi/OpenApiHander.ashx"
@@ -1073,15 +1067,14 @@
             "净值日期",
             "单位净值",
             "_",
             "日增长值",
             "日增长率",
             "_",
             "单位",
-            "_",
         ]
         temp_one_df = temp_one_df[
             [
                 "净值日期",
                 "单位净值",
                 "日增长值",
                 "日增长率",
@@ -1113,15 +1106,14 @@
             "分红金额",
             "除息日",
             "权益登记日",
             "分红发放日",
             "_",
             "单位",
             "_",
-            "_",
         ]
         temp_one_df = temp_one_df[
             [
                 "年份",
                 "权益登记日",
                 "除息日",
                 "分红发放日",
@@ -1136,15 +1128,15 @@
     fund_purchase_em_df = fund_purchase_em()
     print(fund_purchase_em_df)
 
     fund_name_em_df = fund_name_em()
     print(fund_name_em_df)
 
     fund_info_index_em_df = fund_info_index_em(
-        symbol="债券指数", indicator="全部"
+        symbol="沪深指数", indicator="增强指数型"
     )
     print(fund_info_index_em_df)
 
     fund_open_fund_daily_em_df = fund_open_fund_daily_em()
     print(fund_open_fund_daily_em_df)
     time.sleep(3)
 
@@ -1188,21 +1180,21 @@
         fund="161725", indicator="拆分详情"
     )
     print(fund_open_fund_info_em_df)
 
     fund_money_fund_daily_em_df = fund_money_fund_daily_em()
     print(fund_money_fund_daily_em_df)
 
-    fund_money_fund_info_em_df = fund_money_fund_info_em(fund="162411")
+    fund_money_fund_info_em_df = fund_money_fund_info_em(fund="000009")
     print(fund_money_fund_info_em_df)
 
     fund_financial_fund_daily_em_df = fund_financial_fund_daily_em()
     print(fund_financial_fund_daily_em_df)
 
-    fund_financial_fund_info_em_df = fund_financial_fund_info_em(symbol="000134")
+    fund_financial_fund_info_em_df = fund_financial_fund_info_em(fund="000134")
     print(fund_financial_fund_info_em_df)
 
     fund_graded_fund_daily_em_df = fund_graded_fund_daily_em()
     print(fund_graded_fund_daily_em_df)
 
     fund_graded_fund_info_em_df = fund_graded_fund_info_em(fund="150232")
     print(fund_graded_fund_info_em_df)
```

### Comparing `akshare-1.9.80/akshare/fund/fund_etf_em.py` & `akshare-1.9.9/akshare/fund/fund_etf_em.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,11 +351,11 @@
     )
     print(fund_etf_hist_em_df)
 
     fund_etf_hist_min_em_df = fund_etf_hist_min_em(
         symbol="513500",
         period="5",
         adjust="hfq",
-        start_date="2023-05-01 09:32:00",
-        end_date="2023-05-04 14:40:00",
+        start_date="2023-01-01 09:32:00",
+        end_date="2023-01-04 14:40:00",
     )
     print(fund_etf_hist_min_em_df)
```

### Comparing `akshare-1.9.80/akshare/fund/fund_etf_sina.py` & `akshare-1.9.9/akshare/fund/fund_etf_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fund/fund_fhsp_em.py` & `akshare-1.9.9/akshare/fund/fund_fhsp_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fund/fund_init_em.py` & `akshare-1.9.9/akshare/fund/fund_init_em.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
 Date: 2022/3/22 14:30
 Desc: 基金数据-新发基金-新成立基金
-https://fund.eastmoney.com/data/xinfound.html
+http://fund.eastmoney.com/data/xinfound.html
 """
 import pandas as pd
 import requests
 
 from akshare.utils import demjson
```

### Comparing `akshare-1.9.80/akshare/fund/fund_manager.py` & `akshare-1.9.9/akshare/fund/fund_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/4 18:10
+Date: 2021/7/1 16:30
 Desc: 基金经理大全
 http://fund.eastmoney.com/manager/default.html
 """
 import pandas as pd
 import requests
 from tqdm import tqdm
 
 from akshare.utils import demjson
 
 
-def fund_manager(adjust: str = "0") -> pd.DataFrame:
+def fund_manager(adjust: str = '0') -> pd.DataFrame:
     """
     天天基金网-基金数据-基金经理大全
     http://fund.eastmoney.com/manager/default.html
     :param adjust: 默认 adjust='0', 返回目标地址相同格式; adjust='1', 返回根据 `现任基金` 打散后的数据
     :type adjust: str
     :return: 基金经理大全
     :rtype: pandas.DataFrame
@@ -47,16 +47,16 @@
             "sc": "abbname",
             "st": "asc",
         }
         r = requests.get(url, params=params)
         data_text = r.text
         data_json = demjson.decode(data_text.strip("var returnjson= "))
         temp_df = pd.DataFrame(data_json["data"])
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
 
+        big_df = big_df.append(temp_df, ignore_index=True)
     big_df.reset_index(inplace=True)
     big_df["index"] = range(1, len(big_df) + 1)
     big_df.columns = [
         "序号",
         "_",
         "姓名",
         "_",
@@ -79,24 +79,24 @@
             "累计从业时间",
             "现任基金资产总规模",
             "现任基金最佳回报",
         ]
     ]
     big_df["现任基金最佳回报"] = big_df["现任基金最佳回报"].str.split("%", expand=True).iloc[:, 0]
     big_df["现任基金资产总规模"] = big_df["现任基金资产总规模"].str.split("亿元", expand=True).iloc[:, 0]
-    big_df["累计从业时间"] = pd.to_numeric(big_df["累计从业时间"], errors="coerce")
-    big_df["现任基金最佳回报"] = pd.to_numeric(big_df["现任基金最佳回报"], errors="coerce")
-    big_df["现任基金资产总规模"] = pd.to_numeric(big_df["现任基金资产总规模"], errors="coerce")
-    if adjust == "1":
-        big_df["现任基金"] = big_df["现任基金"].apply(lambda x: x.split(","))
-        big_df = big_df.explode(column="现任基金")
+    big_df['累计从业时间'] = pd.to_numeric(big_df['累计从业时间'], errors="coerce")
+    big_df['现任基金最佳回报'] = pd.to_numeric(big_df['现任基金最佳回报'], errors="coerce")
+    big_df['现任基金资产总规模'] = pd.to_numeric(big_df['现任基金资产总规模'], errors="coerce")
+    if adjust == '1':
+        big_df['现任基金'] = big_df['现任基金'].apply(lambda x: x.split(','))
+        big_df = big_df.explode(column='现任基金')
         big_df.reset_index(drop=True, inplace=True)
         return big_df
     return big_df
 
 
 if __name__ == "__main__":
-    fund_manager_df = fund_manager(adjust="0")
+    fund_manager_df = fund_manager(adjust='0')
     print(fund_manager_df)
 
-    fund_manager_df = fund_manager(adjust="1")
+    fund_manager_df = fund_manager(adjust='1')
     print(fund_manager_df)
```

### Comparing `akshare-1.9.80/akshare/fund/fund_portfolio_em.py` & `akshare-1.9.9/akshare/fund/fund_portfolio_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fund/fund_position_lg.py` & `akshare-1.9.9/akshare/fund/fund_position_lg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,67 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/5 22:05
+Date: 2022/12/28 16:05
 Desc: 乐咕乐股-基金仓位
 https://legulegu.com/stockdata/fund-position/pos-stock
 """
 import pandas as pd
 import requests
 
-from akshare.stock_feature.stock_a_indicator import get_token_lg, get_cookie_csrf
+from akshare.stock_feature.stock_a_indicator import get_token_lg
 
 
 def fund_stock_position_lg() -> pd.DataFrame:
     """
     乐咕乐股-基金仓位-股票型基金仓位
     https://legulegu.com/stockdata/fund-position/pos-stock
     :return: 股票型基金仓位
     :rtype: pandas.DataFrame
     """
     url = "https://legulegu.com/api/stockdata/fund-position"
     token = get_token_lg()
     params = {"token": token, "type": "pos_stock", "category": "总仓位", "marketId": "5"}
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(url="https://legulegu.com/stockdata/fund-position/pos-stock")
-    )
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json)
     temp_df["date"] = pd.to_datetime(temp_df["date"]).dt.date
     temp_df = temp_df[
         [
             "date",
             "close",
             "position",
         ]
     ]
-    temp_df['date'] = pd.to_datetime(temp_df['date']).dt.date
     temp_df["close"] = pd.to_numeric(temp_df["close"], errors="coerce")
     temp_df["position"] = pd.to_numeric(temp_df["position"], errors="coerce")
     return temp_df
 
 
 def fund_balance_position_lg() -> pd.DataFrame:
     """
     乐咕乐股-基金仓位-平衡混合型基金仓位
     https://legulegu.com/stockdata/fund-position/pos-pingheng
     :return: 平衡混合型基金仓位
     :rtype: pandas.DataFrame
     """
     url = "https://legulegu.com/api/stockdata/fund-position"
     token = get_token_lg()
-    params = {
-        "token": token,
-        "type": "pos_pingheng",
-        "category": "总仓位",
-        "marketId": "5",
-    }
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(
-            url="https://legulegu.com/stockdata/fund-position/pos-pingheng"
-        )
-    )
+    params = {"token": token, "type": "pos_pingheng", "category": "总仓位", "marketId": "5"}
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json)
     temp_df["date"] = pd.to_datetime(temp_df["date"]).dt.date
     temp_df = temp_df[
         [
             "date",
             "close",
             "position",
         ]
     ]
-    temp_df['date'] = pd.to_datetime(temp_df['date']).dt.date
     temp_df["close"] = pd.to_numeric(temp_df["close"], errors="coerce")
     temp_df["position"] = pd.to_numeric(temp_df["position"], errors="coerce")
     return temp_df
 
 
 def fund_linghuo_position_lg() -> pd.DataFrame:
     """
@@ -86,32 +69,25 @@
     https://legulegu.com/stockdata/fund-position/pos-linghuo
     :return: 灵活配置型基金仓位
     :rtype: pandas.DataFrame
     """
     url = "https://legulegu.com/api/stockdata/fund-position"
     token = get_token_lg()
     params = {"token": token, "type": "pos_linghuo", "category": "总仓位", "marketId": "5"}
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(
-            url="https://legulegu.com/stockdata/fund-position/pos-linghuo"
-        )
-    )
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json)
     temp_df["date"] = pd.to_datetime(temp_df["date"]).dt.date
     temp_df = temp_df[
         [
             "date",
             "close",
             "position",
         ]
     ]
-    temp_df['date'] = pd.to_datetime(temp_df['date']).dt.date
     temp_df["close"] = pd.to_numeric(temp_df["close"], errors="coerce")
     temp_df["position"] = pd.to_numeric(temp_df["position"], errors="coerce")
     return temp_df
 
 
 if __name__ == "__main__":
     fund_stock_position_lg_df = fund_stock_position_lg()
```

### Comparing `akshare-1.9.80/akshare/fund/fund_rank_em.py` & `akshare-1.9.9/akshare/fund/fund_rank_em.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/3/30 15:04
+Date: 2022/4/14 17:04
 Desc: 东方财富网-数据中心-开放基金排行
-https://fund.eastmoney.com/data/fundranking.html
+http://fund.eastmoney.com/data/fundranking.html
 名词解释
-https://help.1234567.com.cn/list_236.html
+http://help.1234567.com.cn/list_236.html
 """
 import datetime
 
 import pandas as pd
 import requests
 
 from akshare.utils import demjson
 
 
 def fund_open_fund_rank_em(symbol: str = "全部") -> pd.DataFrame:
     """
     东方财富网-数据中心-开放基金排行
-    https://fund.eastmoney.com/data/fundranking.html
+    http://fund.eastmoney.com/data/fundranking.html
     :param symbol: choice of {"全部", "股票型", "混合型", "债券型", "指数型", "QDII", "LOF", "FOF"}
     :type symbol: str
     :return: 开放基金排行
     :rtype: pandas.DataFrame
     """
     current_date = datetime.datetime.now().date().isoformat()
     last_date = str(int(current_date[:4]) - 1) + current_date[4:]
@@ -114,29 +114,29 @@
             "自定义",
             "手续费",
         ]
     ]
     return temp_df
 
 
-def fund_exchange_rank_em() -> pd.DataFrame:
+def fund_em_exchange_rank() -> pd.DataFrame:
     """
     东方财富网-数据中心-场内交易基金排行
-    https://fund.eastmoney.com/data/fbsfundranking.html
+    http://fund.eastmoney.com/data/fbsfundranking.html
     :return: 场内交易基金数据
     :rtype: pandas.DataFrame
     """
     url = "http://fund.eastmoney.com/data/rankhandler.aspx"
     params = {
         "op": "ph",
         "dt": "fb",
         "ft": "ct",
         "rs": "",
         "gs": "0",
-        "sc": "1nzf",
+        "sc": "zzf",
         "st": "desc",
         "pi": "1",
         "pn": "10000",
         "v": "0.1591891419018292",
     }
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36",
@@ -162,84 +162,71 @@
         "近3月",
         "近6月",
         "近1年",
         "近2年",
         "近3年",
         "今年来",
         "成立来",
-        "成立日期",
         "_",
         "_",
         "_",
         "_",
         "_",
-        "类型",
+        "_",
+        "_",
         "_",
     ]
     temp_df = temp_df[
         [
             "序号",
             "基金代码",
             "基金简称",
-            "类型",
             "日期",
             "单位净值",
             "累计净值",
             "近1周",
             "近1月",
             "近3月",
             "近6月",
             "近1年",
             "近2年",
             "近3年",
             "今年来",
             "成立来",
-            "成立日期",
         ]
     ]
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
-    temp_df['成立日期'] = pd.to_datetime(temp_df['成立日期']).dt.date
-    temp_df['单位净值'] = pd.to_numeric(temp_df['单位净值'], errors="coerce")
-    temp_df['累计净值'] = pd.to_numeric(temp_df['累计净值'], errors="coerce")
-    temp_df['近1周'] = pd.to_numeric(temp_df['近1周'], errors="coerce")
-    temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
-    temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
-    temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
-    temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
-    temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
-    temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
-    temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
     return temp_df
 
 
-def fund_money_rank_em() -> pd.DataFrame:
+def fund_em_money_rank() -> pd.DataFrame:
     """
     东方财富网-数据中心-货币型基金排行
-    https://fund.eastmoney.com/data/hbxfundranking.html
+    http://fund.eastmoney.com/data/hbxfundranking.html
     :return: 货币型基金排行
     :rtype: pandas.DataFrame
     """
     url = "http://api.fund.eastmoney.com/FundRank/GetHbRankList"
     params = {
         "intCompany": "0",
         "MinsgType": "",
         "IsSale": "1",
-        "strSortCol": "SYL_1N",
+        "strSortCol": "SYL_Y",
         "orderType": "desc",
         "pageIndex": "1",
         "pageSize": "10000",
+        "callback": "jQuery18303264654966943197_1603867158043",
         "_": "1603867224251",
     }
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36",
         "Referer": "http://fund.eastmoney.com/fundguzhi.html",
     }
     r = requests.get(url, params=params, headers=headers)
-    json_data = r.json()
+    text_data = r.text
+    json_data = demjson.decode(text_data[text_data.find("{") : -1])
     temp_df = pd.DataFrame(json_data["Data"])
     temp_df.reset_index(inplace=True)
     temp_df["index"] = list(range(1, len(temp_df) + 1))
     temp_df.columns = [
         "序号",
         "近1年",
         "近2年",
@@ -285,36 +272,22 @@
             "近3年",
             "近5年",
             "今年来",
             "成立来",
             "手续费",
         ]
     ]
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
-    temp_df['万份收益'] = pd.to_numeric(temp_df['万份收益'], errors="coerce")
-    temp_df['年化收益率7日'] = pd.to_numeric(temp_df['年化收益率7日'], errors="coerce")
-    temp_df['年化收益率14日'] = pd.to_numeric(temp_df['年化收益率14日'], errors="coerce")
-    temp_df['年化收益率28日'] = pd.to_numeric(temp_df['年化收益率28日'], errors="coerce")
-    temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
-    temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
-    temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
-    temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
-    temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
-    temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
-    temp_df['近5年'] = pd.to_numeric(temp_df['近5年'], errors="coerce")
-    temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
     return temp_df
 
 
-def fund_lcx_rank_em() -> pd.DataFrame:
+def fund_em_lcx_rank() -> pd.DataFrame:
     """
     东方财富网-数据中心-理财基金排行
     # 该接口暂时没有数据
-    https://fund.eastmoney.com/data/lcxfundranking.html#t;c0;r;sSYL_Z;ddesc;pn50;f;os1;
+    http://fund.eastmoney.com/data/lcxfundranking.html#t;c0;r;sSYL_Z;ddesc;pn50;f;os1;
     :return: 理财基金排行
     :rtype: pandas.DataFrame
     """
     url = "http://api.fund.eastmoney.com/FundRank/GetLcRankList"
     params = {
         "intCompany": "0",
         "MinsgType": "undefined",
@@ -383,33 +356,33 @@
             "可购买",
             "手续费",
         ]
     ]
     return temp_df
 
 
-def fund_hk_rank_em() -> pd.DataFrame:
+def fund_em_hk_rank() -> pd.DataFrame:
     """
     东方财富网-数据中心-香港基金排行
-    https://overseas.1234567.com.cn/FundList
+    http://overseas.1234567.com.cn/FundList
     :return: 香港基金排行
     :rtype: pandas.DataFrame
     """
     format_date = datetime.datetime.now().date().isoformat()
-    url = "https://overseas.1234567.com.cn/overseasapi/OpenApiHander.ashx"
+    url = "http://overseas.1234567.com.cn/overseasapi/OpenApiHander.ashx"
     params = {
         'api': 'HKFDApi',
         'm': 'MethodFundList',
         'action': '1',
         'pageindex': '0',
         'pagesize': '5000',
         'dy': '1',
         'date1': format_date,
         'date2': format_date,
-        'sortfield': 'Y',
+        'sortfield': 'W',
         'sorttype': '-1',
         'isbuy': '0',
         '_': '1610790553848',
     }
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.138 Safari/537.36",
         "Referer": "http://fund.eastmoney.com/fundguzhi.html",
@@ -460,43 +433,29 @@
             "近3年",
             "今年来",
             "成立来",
             "可购买",
             "香港基金代码",
         ]
     ]
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
-    temp_df['单位净值'] = pd.to_numeric(temp_df['单位净值'], errors="coerce")
-    temp_df['日增长率'] = pd.to_numeric(temp_df['日增长率'], errors="coerce")
-    temp_df['近1周'] = pd.to_numeric(temp_df['近1周'], errors="coerce")
-    temp_df['近1月'] = pd.to_numeric(temp_df['近1月'], errors="coerce")
-    temp_df['近3月'] = pd.to_numeric(temp_df['近3月'], errors="coerce")
-    temp_df['近6月'] = pd.to_numeric(temp_df['近6月'], errors="coerce")
-    temp_df['近1年'] = pd.to_numeric(temp_df['近1年'], errors="coerce")
-    temp_df['近2年'] = pd.to_numeric(temp_df['近2年'], errors="coerce")
-    temp_df['近3年'] = pd.to_numeric(temp_df['近3年'], errors="coerce")
-    temp_df['今年来'] = pd.to_numeric(temp_df['今年来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
-    temp_df['成立来'] = pd.to_numeric(temp_df['成立来'], errors="coerce")
-    temp_df['可购买'] = temp_df['可购买'].map(lambda x: "可购买" if x == "1" else "不可购买")
     return temp_df
 
 
 if __name__ == "__main__":
     for item in {"全部", "股票型", "混合型", "债券型", "指数型", "QDII", "LOF", "FOF"}:
         fund_open_fund_rank_em_df = fund_open_fund_rank_em(symbol=item)
         print(fund_open_fund_rank_em_df)
 
     fund_open_fund_rank_em_df = fund_open_fund_rank_em(symbol="全部")
     print(fund_open_fund_rank_em_df)
 
-    fund_exchange_rank_em_df = fund_exchange_rank_em()
-    print(fund_exchange_rank_em_df)
+    fund_em_exchange_rank_df = fund_em_exchange_rank()
+    print(fund_em_exchange_rank_df)
 
-    fund_money_rank_em_df = fund_money_rank_em()
-    print(fund_money_rank_em_df)
+    fund_em_money_rank_df = fund_em_money_rank()
+    print(fund_em_money_rank_df)
 
-    fund_lcx_rank_em_df = fund_lcx_rank_em()
-    print(fund_lcx_rank_em_df)
+    fund_em_lcx_rank_df = fund_em_lcx_rank()
+    print(fund_em_lcx_rank_df)
 
-    fund_hk_rank_em_df = fund_hk_rank_em()
-    print(fund_hk_rank_em_df)
+    fund_em_hk_rank_df = fund_em_hk_rank()
+    print(fund_em_hk_rank_df)
```

### Comparing `akshare-1.9.80/akshare/fund/fund_rating.py` & `akshare-1.9.9/akshare/fund/fund_rating.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fund/fund_report_cninfo.py` & `akshare-1.9.9/akshare/fund/fund_report_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fund/fund_scale_em.py` & `akshare-1.9.9/akshare/fund/fund_scale_em.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding:utf-8 -*-
 # !/usr/bin/env python
 """
 Date: 2021/11/24 15:39
 Desc: 天天基金网-基金数据-规模份额
-https://fund.eastmoney.com/data/cyrjglist.html
+http://fund.eastmoney.com/data/cyrjglist.html
 """
 import requests
 import pandas as pd
 
 from akshare.utils import demjson
```

### Comparing `akshare-1.9.80/akshare/fund/fund_scale_sina.py` & `akshare-1.9.9/akshare/fund/fund_scale_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/cons.py` & `akshare-1.9.9/akshare/futures/cons.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,14 @@
         "BU",
         "RU",
         "SC",
         "NR",
         "SP",
         "SS",
         "LU",
-        "BC",
     ],
     "gfex": ["SI"],
 }
 
 contract_symbols = []
 [contract_symbols.extend(i) for i in market_exchange_symbols.values()]
```

### Comparing `akshare-1.9.80/akshare/futures/cot.py` & `akshare-1.9.9/akshare/futures/cot.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         if start_day.strftime("%Y%m%d") in calendar:
             data = get_rank_sum(start_day, vars_list)
             if data is False:
                 print(
                     f"{start_day.strftime('%Y-%m-%d')}日交易所数据连接失败，已超过20次，您的地址被网站墙了，请保存好返回数据，稍后从该日期起重试"
                 )
                 return records.reset_index(drop=True)
-            records = pd.concat([records, data], ignore_index=True)
+            records = records.append(data)
         else:
             warnings.warn(f"{start_day.strftime('%Y%m%d')}非交易日")
         start_day += datetime.timedelta(days=1)
 
     return records.reset_index(drop=True)
 
 
@@ -258,38 +258,37 @@
                         "short_open_interest"
                     ].sum(),
                     "short_open_interest_chg_top20": table_cut_top20[
                         "short_open_interest_chg"
                     ].sum(),
                     "date": date.strftime("%Y%m%d"),
                 }
-                records = pd.concat([records, pd.DataFrame(big_dict, index=[0])], ignore_index=True)
+                records = records.append(pd.DataFrame(big_dict, index=[0]))
 
     if len(big_dict.items()) > 0:
         add_vars = [
             i
             for i in cons.market_exchange_symbols["dce"]
             + cons.market_exchange_symbols["shfe"]
             + cons.market_exchange_symbols["cffex"]
             if i in records["variety"].tolist()
         ]
         for var in add_vars:
             records_cut = records[records["variety"] == var]
             var_record = pd.DataFrame(records_cut.sum()).T
             var_record["date"] = date.strftime("%Y%m%d")
             var_record.loc[:, ["variety", "symbol"]] = var
-            records = pd.concat([records, var_record], ignore_index=True)
+            records = records.append(var_record)
 
     return records.reset_index(drop=True)
 
 
 def get_shfe_rank_table(date=None, vars_list=cons.contract_symbols):
     """
     上海期货交易所前 20 会员持仓排名数据明细
-    https://www.shfe.com.cn/
     注：该交易所只公布每个品种内部的标的排名，没有公布品种的总排名
     数据从20020107开始，每交易日16:30左右更新数据
     :param date: 日期 format：YYYY-MM-DD 或 YYYYMMDD 或 datetime.date对象 为空时为当天
     :param vars_list: 合约品种如RB、AL等列表 为空时为所有商品
     :return: pd.DataFrame
     rank                        排名                        int
     vol_party_name              成交量排序的当前名次会员        string(中文)
@@ -311,15 +310,15 @@
     if date < datetime.date(2002, 1, 7):
         print("shfe数据源开始日期为20020107，跳过")
         return {}
     if date.strftime("%Y%m%d") not in calendar:
         warnings.warn("%s非交易日" % date.strftime("%Y%m%d"))
         return {}
     url = cons.SHFE_VOL_RANK_URL % (date.strftime("%Y%m%d"))
-    r = requests_link(url, "utf-8", headers=cons.shfe_headers)
+    r = requests_link(url, "utf-8")
     try:
         context = json.loads(r.text)
     except:
         return {}
     df = pd.DataFrame(context["o_cursor"])
 
     df = df.rename(
@@ -491,16 +490,16 @@
             "short_open_interest",
             "short_open_interest_chg",
         ]
         inner_temp_df.reset_index(inplace=True, drop=True)
         big_dict[symbol_list[-1]] = inner_temp_df
     new_big_dict = {}
     for key, value in big_dict.items():
-        value = value.assign(symbol=key)
-        value = value.assign(variety=re.compile(r"[a-zA-Z_]+").findall(key)[0])
+        value["symbol"] = key
+        value["variety"] = re.compile(r"[a-zA-Z_]+").findall(key)[0]
         new_big_dict[key] = value
 
     return new_big_dict
 
 
 def _get_dce_contract_list(date, var):
     """
@@ -788,15 +787,15 @@
     table_cut[intColumns + ["rank"]] = table_cut[intColumns + ["rank"]].astype(
         int
     )
     table_cut_sum = table_cut.sum()
     table_cut_sum["rank"] = 999
     for col in ["vol_party_name", "long_party_name", "short_party_name"]:
         table_cut_sum[col] = None
-    table_cut = pd.concat([table_cut, pd.DataFrame(table_cut_sum).T], sort=True)
+    table_cut = table_cut.append(pd.DataFrame(table_cut_sum).T, sort=True)
     table_cut["symbol"] = symbol
     table_cut["variety"] = var
     table_cut[intColumns + ["rank"]] = table_cut[intColumns + ["rank"]].astype(
         int
     )
     return table_cut
 
@@ -1129,15 +1128,15 @@
     print(get_czce_rank_table_first_df)
 
     # 中国金融期货交易所
     get_cffex_rank_table_df = get_cffex_rank_table(date="20200325")
     print(get_cffex_rank_table_df)
 
     # 上海期货交易所
-    get_shfe_rank_table_df = get_shfe_rank_table(date="20230103")
+    get_shfe_rank_table_df = get_shfe_rank_table(date="20190711")
     print(get_shfe_rank_table_df)
 
     # 大连商品交易所
     get_dce_rank_table_first_df = get_dce_rank_table(date="20131227")
     print(get_dce_rank_table_first_df)
 
     get_dce_rank_table_second_df = get_dce_rank_table(date="20171227")
@@ -1149,15 +1148,15 @@
     get_dce_rank_table_fourth_df = get_dce_rank_table(
         date="20210517", vars_list=["V"]
     )
     print(get_dce_rank_table_fourth_df)
 
     # 总接口
     get_rank_sum_daily_df = get_rank_sum_daily(
-        start_day="20210515", end_day="20210518", vars_list=["MA"]
+        start_day="20210515", end_day="20210518", vars_list=["PF"]
     )
     print(get_rank_sum_daily_df)
 
     futures_dce_detail_dict = futures_dce_position_rank(date="20210407")
     print(futures_dce_detail_dict)
 
     futures_dce_position_rank_other_df = futures_dce_position_rank_other(
```

### Comparing `akshare-1.9.80/akshare/futures/futures_basis.py` & `akshare-1.9.9/akshare/futures/futures_basis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/11 17:30
+Date: 2021/11/9 22:30
 Desc: 生意社网站采集大宗商品现货价格及相应基差数据, 数据时间段从 20110104-至今
 备注：现期差 = 现货价格 - 期货价格(这里的期货价格为结算价)
 黄金为 元/克, 白银为 元/千克, 玻璃现货为 元/平方米, 鸡蛋现货为 元/公斤, 鸡蛋期货为 元/500千克, 其余为 元/吨.
 焦炭现货规格是: 一级冶金焦; 焦炭期货规格: 介于一级和二级之间, 焦炭现期差仅供参考.
 铁矿石现货价格是: 湿吨, 铁矿石期货价格是: 干吨
-网页地址: https://www.100ppi.com/sf/
-历史数据可以通过修改 url 地址来获取, 比如: https://www.100ppi.com/sf/day-2017-09-12.html
+网页地址: http://www.100ppi.com/sf/
+历史数据可以通过修改 url 地址来获取, 比如: http://www.100ppi.com/sf/day-2017-09-12.html
 发现生意社的 bugs:
-1. 2018-09-12 周三 数据缺失是因为生意社源数据在该交易日缺失: https://www.100ppi.com/sf/day-2018-09-12.html
+1. 2018-09-12 周三 数据缺失是因为生意社源数据在该交易日缺失: http://www.100ppi.com/sf/day-2018-09-12.html
 """
 import datetime
 import re
 import time
 import warnings
 from typing import List
 
@@ -30,15 +30,15 @@
 def futures_spot_price_daily(
     start_day: str = "20210201",
     end_day: str = "20210208",
     vars_list=cons.contract_symbols,
 ):
     """
     指定时间段内大宗商品现货价格及相应基差
-    https://www.100ppi.com/sf/
+    http://www.100ppi.com/sf/
     :param start_day: str 开始日期 format：YYYY-MM-DD 或 YYYYMMDD 或 datetime.date对象; 默认为当天
     :param end_day: str 结束数据 format：YYYY-MM-DD 或 YYYYMMDD 或 datetime.date对象; 默认为当天
     :param vars_list: list 合约品种如 [RB, AL]; 默认参数为所有商品
     :return: pandas.DataFrame
     展期收益率数据:
     var               商品品种                      string
     sp                现货价格                      float
@@ -70,18 +70,18 @@
         start_day += datetime.timedelta(days=1)
     if len(df_list) > 0:
         temp_df = pd.concat(df_list)
         temp_df.reset_index(drop=True, inplace=True)
         return temp_df
 
 
-def futures_spot_price(date: str = "20230509", vars_list: list = cons.contract_symbols) -> pd.DataFrame:
+def futures_spot_price(date: str = "20210201", vars_list: list = cons.contract_symbols) -> pd.DataFrame:
     """
     指定交易日大宗商品现货价格及相应基差
-    https://www.100ppi.com/sf/day-2017-09-12.html
+    http://www.100ppi.com/sf/day-2017-09-12.html
     :param date: 开始日期 format: YYYY-MM-DD 或 YYYYMMDD 或 datetime.date 对象; 为空时为当天
     :param vars_list: 合约品种如 RB、AL 等列表 为空时为所有商品
     :return: pandas.DataFrame
     展期收益率数据:
     var              商品品种                     string
     sp               现货价格                     float
     near_symbol      临近交割合约                  string
@@ -96,16 +96,16 @@
     """
     date = cons.convert_date(date) if date is not None else datetime.date.today()
     if date < datetime.date(2011, 1, 4):
         raise Exception("数据源开始日期为 20110104, 请将获取数据时间点设置在 20110104 后")
     if date.strftime("%Y%m%d") not in calendar:
         warnings.warn(f"{date.strftime('%Y%m%d')}非交易日")
         return
-    u1 = "http://www.100ppi.com/sf/"
-    u2 = f'http://www.100ppi.com/sf/day-{date.strftime("%Y-%m-%d")}.html'
+    u1 = cons.SYS_SPOT_PRICE_LATEST_URL
+    u2 = cons.SYS_SPOT_PRICE_URL.format(date.strftime("%Y-%m-%d"))
     i = 1
     while True:
         for url in [u2, u1]:
             try:
                 # url = u2
                 r = pandas_read_html_link(url)
                 string = r[0].loc[1, 1]
@@ -160,28 +160,28 @@
     ]
     records = pd.DataFrame()
     for string in df_data["symbol"].tolist():
         if string == "PTA":
             news = "PTA"
         else:
             news = "".join(re.findall(r"[\u4e00-\u9fa5]", string))
-        if news != "" and news not in ["商品", "价格", "上海期货交易所", "郑州商品交易所", "大连商品交易所", "广州期货交易所"]:
+        if news != "" and news not in ["商品", "价格", "上海期货交易所", "郑州商品交易所", "大连商品交易所"]:
             symbol = chinese_to_english(news)
             record = pd.DataFrame(df_data[df_data["symbol"] == string])
             record.loc[:, "symbol"] = symbol
             record.loc[:, "spot_price"] = record.loc[:, "spot_price"].astype(float)
             if (
                 symbol == "JD"
             ):  # 鸡蛋现货为元/公斤, 鸡蛋期货为元/500千克, 其余元/吨(http://www.100ppi.com/sf/)
-                record.loc[:, "spot_price"] = float(record["spot_price"].iloc[0]) * 500
+                record.loc[:, "spot_price"] = float(record["spot_price"]) * 500
             elif (
                 symbol == "FG"
             ):  # 上表中现货单位为元/平方米, 期货单位为元/吨. 换算公式：元/平方米*80=元/吨(http://www.100ppi.com/sf/959.html)
-                record.loc[:, "spot_price"] = float(record["spot_price"].iloc[0]) * 80
-            records = pd.concat([records, record])
+                record.loc[:, "spot_price"] = float(record["spot_price"]) * 80
+            records = records.append(record)
 
     records.loc[
         :, ["near_contract_price", "dominant_contract_price", "spot_price"]
     ] = records.loc[
         :, ["near_contract_price", "dominant_contract_price", "spot_price"]
     ].astype(
         "float"
@@ -293,12 +293,12 @@
 
 if __name__ == "__main__":
     futures_spot_price_daily_df = futures_spot_price_daily(
         start_day="20180913", end_day="20180916", vars_list=['SR']
     )
     print(futures_spot_price_daily_df)
 
-    futures_spot_price_df = futures_spot_price("20200510")
+    futures_spot_price_df = futures_spot_price("20211109")
     print(futures_spot_price_df)
 
     futures_spot_price_previous_df = futures_spot_price_previous('20220209')
     print(futures_spot_price_previous_df)
```

### Comparing `akshare-1.9.80/akshare/futures/futures_comex.py` & `akshare-1.9.9/akshare/futures/futures_comex.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_comm_qihuo.py` & `akshare-1.9.9/akshare/futures/futures_comm_qihuo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_contract_detail.py` & `akshare-1.9.9/akshare/futures/futures_contract_detail.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_daily_bar.py` & `akshare-1.9.9/akshare/futures/futures_daily_bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
     day = (
         cons.convert_date(date) if date is not None else datetime.date.today()
     )
     if day.strftime("%Y%m%d") not in calendar:
         # warnings.warn(f"{day.strftime('%Y%m%d')}非交易日")
         return
     url = f"http://www.ine.cn/data/dailydata/kx/kx{day.strftime('%Y%m%d')}.dat"
-    r = requests.get(url, headers=cons.shfe_headers)
+    r = requests.get(url)
     result_df = pd.DataFrame()
     try:
         data_json = r.json()
     except:
         return
     temp_df = pd.DataFrame(data_json["o_curinstrument"]).iloc[:-1, :]
     temp_df = temp_df[temp_df["DELIVERYMONTH"] != "小计"]
@@ -740,15 +740,15 @@
 
     get_cffex_daily_df = get_cffex_daily(date="20210719")
     print(get_cffex_daily_df)
 
     get_ine_daily_df = get_ine_daily(date="20211201")
     print(get_ine_daily_df)
 
-    get_czce_daily_df = get_czce_daily(date="20230320")
+    get_czce_daily_df = get_czce_daily(date="20100825")
     print(get_czce_daily_df)
 
-    get_shfe_daily_df = get_shfe_daily(date="20230412")
+    get_shfe_daily_df = get_shfe_daily(date="20160104")
     print(get_shfe_daily_df)
 
     get_gfex_daily_df = get_gfex_daily(date="20221228")
     print(get_gfex_daily_df)
```

### Comparing `akshare-1.9.80/akshare/futures/futures_foreign.py` & `akshare-1.9.9/akshare/futures/futures_foreign.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_hq_sina.py` & `akshare-1.9.9/akshare/futures/futures_hq_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_index_ccidx.py` & `akshare-1.9.9/akshare/futures/futures_index_ccidx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_international.py` & `akshare-1.9.9/akshare/futures/futures_international.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_inventory_99.py` & `akshare-1.9.9/akshare/futures/futures_inventory_99.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_inventory_em.py` & `akshare-1.9.9/akshare/futures/futures_inventory_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_news_baidu.py` & `akshare-1.9.9/akshare/futures/futures_news_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_news_shmet.py` & `akshare-1.9.9/akshare/futures/futures_news_shmet.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_roll_yield.py` & `akshare-1.9.9/akshare/futures/futures_roll_yield.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_rule.py` & `akshare-1.9.9/akshare/futures/futures_rule.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_sgx_daily.py` & `akshare-1.9.9/akshare/futures/futures_sgx_daily.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_spot_stock_em.py` & `akshare-1.9.9/akshare/futures/futures_spot_stock_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_to_spot.py` & `akshare-1.9.9/akshare/futures/futures_to_spot.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_warehouse_receipt.py` & `akshare-1.9.9/akshare/futures/futures_warehouse_receipt.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/futures_zh_sina.py` & `akshare-1.9.9/akshare/futures/futures_zh_sina.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/30 20:20
+Date: 2022/6/2 15:20
 Desc: 新浪财经-国内期货-实时数据获取
 http://vip.stock.finance.sina.com.cn/quotes_service/view/qihuohangqing.html#titlePos_3
 P.S. 注意采集速度, 容易封禁 IP, 如果不能访问请稍后再试
 """
 import json
 import time
 from functools import lru_cache
@@ -37,43 +37,38 @@
     data_text = r.text
     raw_json = data_text[data_text.find("{") : data_text.find("}") + 1]
     data_json = demjson.decode(raw_json)
     czce_mark_list = [item[1] for item in data_json["czce"][1:]]
     dce_mark_list = [item[1] for item in data_json["dce"][1:]]
     shfe_mark_list = [item[1] for item in data_json["shfe"][1:]]
     cffex_mark_list = [item[1] for item in data_json["cffex"][1:]]
-    gfex_mark_list = [item[1] for item in data_json["gfex"][1:]]
     all_mark_list = (
-        czce_mark_list + dce_mark_list + shfe_mark_list + cffex_mark_list + gfex_mark_list
+        czce_mark_list + dce_mark_list + shfe_mark_list + cffex_mark_list
     )
 
     czce_market_name_list = [data_json["czce"][0]] * len(czce_mark_list)
     dce_market_name_list = [data_json["dce"][0]] * len(dce_mark_list)
     shfe_market_name_list = [data_json["shfe"][0]] * len(shfe_mark_list)
     cffex_market_name_list = [data_json["cffex"][0]] * len(cffex_mark_list)
-    gfex_market_name_list = [data_json["gfex"][0]] * len(gfex_mark_list)
     all_market_name_list = (
         czce_market_name_list
         + dce_market_name_list
         + shfe_market_name_list
         + cffex_market_name_list
-        + gfex_market_name_list
     )
 
     czce_symbol_list = [item[0] for item in data_json["czce"][1:]]
     dce_symbol_list = [item[0] for item in data_json["dce"][1:]]
     shfe_symbol_list = [item[0] for item in data_json["shfe"][1:]]
     cffex_symbol_list = [item[0] for item in data_json["cffex"][1:]]
-    gfex_symbol_list = [item[0] for item in data_json["gfex"][1:]]
     all_symbol_list = (
         czce_symbol_list
         + dce_symbol_list
         + shfe_symbol_list
         + cffex_symbol_list
-        + gfex_symbol_list
     )
 
     temp_df = pd.DataFrame(
         [all_market_name_list, all_symbol_list, all_mark_list]
     ).T
     temp_df.columns = [
         "exchange",
@@ -130,15 +125,15 @@
     return temp_df
 
 
 def zh_subscribe_exchange_symbol(symbol: str = "dce") -> dict:
     """
     交易所具体的可交易品种
     http://vip.stock.finance.sina.com.cn/quotes_service/view/qihuohangqing.html#titlePos_1
-    :param symbol: choice of {'czce', 'dce', 'shfe', 'cffex', 'gfex'}
+    :param symbol: choice of {'czce', 'dce', 'shfe', 'cffex'}
     :type symbol: str
     :return: 交易所具体的可交易品种
     :rtype: dict
     """
     r = requests.get(zh_subscribe_exchange_symbol_url)
     r.encoding = "gbk"
     data_text = r.text
@@ -153,24 +148,21 @@
         return pd.DataFrame(data_json["dce"])
     if symbol == "shfe":
         data_json["shfe"].remove("上海期货交易所")
         return pd.DataFrame(data_json["shfe"])
     if symbol == "cffex":
         data_json["cffex"].remove("中国金融期货交易所")
         return pd.DataFrame(data_json["cffex"])
-    if symbol == "gfex":
-        data_json["gfex"].remove("广期所")
-        return pd.DataFrame(data_json["gfex"])
 
 
 def match_main_contract(symbol: str = "cffex") -> str:
     """
     新浪财经-期货-主力合约
     http://vip.stock.finance.sina.com.cn/quotes_service/view/qihuohangqing.html#titlePos_1
-    :param symbol: choice of {'czce', 'dce', 'shfe', 'cffex', 'gfex'}
+    :param symbol: choice of {'czce', 'dce', 'shfe', 'cffex'}
     :type symbol: str
     :return: 主力合约的字符串
     :rtype: str
     """
     subscribe_exchange_list = []
     exchange_symbol_list = (
         zh_subscribe_exchange_symbol(symbol).iloc[:, 1].tolist()
@@ -195,15 +187,15 @@
                 print(item, "无主力合约")
             continue
     print(f"{symbol}主力合约获取成功")
     return ",".join([item for item in subscribe_exchange_list])
 
 
 def futures_zh_spot(
-    symbol: str = "V2309",
+    symbol: str = "V2209",
     market: str = "CF",
     adjust: str = "0",
 ) -> pd.DataFrame:
     """
     期货的实时行情数据
     http://vip.stock.finance.sina.com.cn/quotes_service/view/qihuohangqing.html#titlePos_1
     :param symbol: 合约名称的字符串组合
@@ -641,15 +633,15 @@
     temp_df["low"] = pd.to_numeric(temp_df["low"])
     temp_df["close"] = pd.to_numeric(temp_df["close"])
     temp_df["volume"] = pd.to_numeric(temp_df["volume"])
     temp_df["hold"] = pd.to_numeric(temp_df["hold"])
     return temp_df
 
 
-def futures_zh_daily_sina(symbol: str = "V2306") -> pd.DataFrame:
+def futures_zh_daily_sina(symbol: str = "V2105") -> pd.DataFrame:
     """
     中国各品种期货日频率数据
     https://finance.sina.com.cn/futures/quotes/V2105.shtml
     :param symbol: 可以通过 match_main_contract(symbol="cffex") 获取, 或者访问网页获取
     :type symbol: str
     :return: 指定 symbol 和 period 的数据
     :rtype: pandas.DataFrame
@@ -679,52 +671,39 @@
     temp_df["volume"] = pd.to_numeric(temp_df["volume"])
     temp_df["hold"] = pd.to_numeric(temp_df["hold"])
     temp_df["settle"] = pd.to_numeric(temp_df["settle"])
     return temp_df
 
 
 if __name__ == "__main__":
-    match_main_contract_df = match_main_contract(symbol="gfex")
+    match_main_contract_df = match_main_contract(symbol="dce")
     print(match_main_contract_df)
 
     futures_zh_spot_df = futures_zh_spot(
-        symbol="TA2309,P2309,B2309,M2309", market="CF", adjust="0"
+        symbol="TA2209,P2209,B2209,M2209", market="CF", adjust="0"
     )
     print(futures_zh_spot_df)
 
     futures_zh_spot_df = futures_zh_spot(
-        symbol="M2309", market="CF", adjust="0"
+        symbol="M2301", market="CF", adjust="0"
     )
     print(futures_zh_spot_df)
 
     futures_symbol_mark_df = futures_symbol_mark()
     print(futures_symbol_mark_df)
 
-    futures_zh_realtime_df = futures_zh_realtime(symbol="工业硅")
+    futures_zh_realtime_df = futures_zh_realtime(symbol="白糖")
     print(futures_zh_realtime_df)
 
     futures_zh_minute_sina_df = futures_zh_minute_sina(
-        symbol="SI2311", period="1"
+        symbol="M2301", period="1"
     )
     print(futures_zh_minute_sina_df)
 
-    futures_zh_daily_sina_df = futures_zh_daily_sina(symbol="SI2311")
+    futures_zh_daily_sina_df = futures_zh_daily_sina(symbol="IC2206")
     print(futures_zh_daily_sina_df)
 
-    futures_zh_daily_sina_df = futures_zh_daily_sina(symbol="V2306")
+    futures_zh_daily_sina_df = futures_zh_daily_sina(symbol="V2205")
     print(futures_zh_daily_sina_df)
 
     futures_zh_spot_df = futures_zh_spot()
     print(futures_zh_spot_df)
-
-    dce_text = match_main_contract(symbol="dce")
-    czce_text = match_main_contract(symbol="czce")
-    shfe_text = match_main_contract(symbol="shfe")
-    gfex_text = match_main_contract(symbol="gfex")
-
-    while True:
-        time.sleep(3)
-        futures_zh_spot_df = futures_zh_spot(
-            symbol=",".join([dce_text, czce_text, shfe_text, gfex_text]),
-            market="CF",
-            adjust='0')
-        print(futures_zh_spot_df)
```

### Comparing `akshare-1.9.80/akshare/futures/inventory_data.py` & `akshare-1.9.9/akshare/futures/inventory_data.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures/receipt.py` & `akshare-1.9.9/akshare/futures/receipt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/18 16:00
+Date: 2021/7/9 18:18
 Desc: 每日注册仓单数据
 大连商品交易所, 上海期货交易所, 郑州商品交易所
 """
 import datetime
 import re
 import warnings
 from typing import List
@@ -129,15 +129,15 @@
     if not isinstance(vars_list, list):
         return warnings.warn(f"symbol_list: 必须是列表")
     date = cons.convert_date(date).strftime('%Y%m%d') if date is not None else datetime.date.today()
     if date not in calendar:
         warnings.warn('%s非交易日' % date.strftime('%Y%m%d'))
         return None
     url = cons.SHFE_RECEIPT_URL_2 % date
-    r = requests_link(url, encoding='utf-8', headers=cons.shfe_headers)
+    r = requests_link(url, encoding='utf-8')
     try:
         context = r.json()
     except:
         return pd.DataFrame()
     data = pd.DataFrame(context['o_cursor'])
     if len(data.columns) < 1:
         return pd.DataFrame()
@@ -179,15 +179,15 @@
     date = cons.convert_date(date).strftime('%Y%m%d') if date is not None else datetime.date.today()
     if date not in calendar:
         warnings.warn('%s非交易日' % date.strftime('%Y%m%d'))
         return None
     if date == '20090820':
         return pd.DataFrame()
     url = cons.CZCE_RECEIPT_URL_1 % date
-    r = requests_link(url, encoding='utf-8', headers=cons.shfe_headers)
+    r = requests_link(url, encoding='utf-8')
     context = r.text
     data = pd.read_html(context)[1]
     records = pd.DataFrame()
     indexes = [x for x in data.index if '品种：' in str(data[0].tolist()[x])]
     ends = [x for x in data.index if '总计' in str(data[0].tolist()[x])]
     for i in list(range(len(indexes))):
         if i != len(indexes) - 1:
@@ -277,15 +277,15 @@
     if not isinstance(vars_list, list):
         return warnings.warn("vars_list: 必须是列表")
     date = cons.convert_date(date).strftime('%Y%m%d') if date is not None else datetime.date.today()
     if date not in calendar:
         warnings.warn('%s非交易日' % date.strftime('%Y%m%d'))
         return None
     url = f"http://www.czce.com.cn/cn/DFSStaticFiles/Future/{date[:4]}/{date}/FutureDataWhsheet.xls"
-    r = requests_link(url, encoding='utf-8', headers=cons.shfe_headers)
+    r = requests_link(url, encoding='utf-8')
     temp_df = pd.read_excel(BytesIO(r.content))
     temp_df = temp_df[[bool(1-item) for item in [item if item is not pd.NA else False for item in temp_df.iloc[:, 0].str.contains("非农产品")]]]
     temp_df.reset_index(inplace=True, drop=True)
     range_list_one = list(temp_df[[item if not pd.isnull(item) else False for item in temp_df.iloc[:, 0].str.contains("品种")]].index)
     range_list_two = list(temp_df[[item if not pd.isnull(item) else False for item in temp_df.iloc[:, 0].str.contains("品种")]].index)[1:]
     range_list_two.append(None)
     symbol_list = []
@@ -394,9 +394,9 @@
     if "MA" in records["var"].to_list():
         replace_index = records[records["var"] == "MA"]["receipt"].astype(str).str.split("0", expand=True)[0].index
         records.loc[replace_index, "receipt"] = records[records["var"] == "MA"]["receipt"].astype(str).str.split("0", expand=True)[0]
     return records
 
 
 if __name__ == '__main__':
-    get_receipt_df = get_receipt(start_day='20230411', end_day='20230412')
+    get_receipt_df = get_receipt(start_day='20210201', end_day='20210215')
     print(get_receipt_df)
```

### Comparing `akshare-1.9.80/akshare/futures/requests_fun.py` & `akshare-1.9.9/akshare/futures/requests_fun.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     :param headers: dict 游览器请求头: 键值对
     :return: requests.response 爬取返回内容: response
     """
     i = 0
     while True:
         try:
             if method == "get":
-                r = requests.get(url, timeout=20, headers=headers)
+                r = requests.get(url, timeout=20)
                 r.encoding = encoding
                 return r
             elif method == "post":
                 r = requests.post(url, timeout=20, data=data, headers=headers)
                 r.encoding = encoding
                 return r
             else:
```

### Comparing `akshare-1.9.80/akshare/futures/symbol_var.py` & `akshare-1.9.9/akshare/futures/symbol_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,14 @@
         "纸浆厂库",
         "低硫燃料油仓库",
         "低硫燃料油厂库",
         "短纤",
         '涤纶短纤',
         '生猪',
         '花生',
-        '工业硅',
     ]
     english_list = [
         "RU",
         "RU",
         "BU",
         "BU",
         "BU",
@@ -256,15 +255,14 @@
         "SP",
         "LU",
         "LU",
         "PF",
         "PF",
         "LH",
         "PK",
-        "SI",
     ]
     pos = chinese_list.index(chinese_var)
     return english_list[pos]
 
 
 if __name__ == "__main__":
     print(chinese_to_english("苹果"))
```

### Comparing `akshare-1.9.80/akshare/futures_derivative/cons.py` & `akshare-1.9.9/akshare/futures_derivative/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/futures_egg.py` & `akshare-1.9.9/akshare/futures_derivative/futures_egg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/futures_hog.py` & `akshare-1.9.9/akshare/futures_derivative/futures_hog.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/futures_index_price_nh.py` & `akshare-1.9.9/akshare/futures_derivative/futures_index_price_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/futures_index_return_nh.py` & `akshare-1.9.9/akshare/futures_derivative/futures_index_return_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/futures_index_volatility_nh.py` & `akshare-1.9.9/akshare/futures_derivative/futures_index_volatility_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/futures_other_index_nh.py` & `akshare-1.9.9/akshare/futures_derivative/futures_other_index_nh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/futures_sina_cot.py` & `akshare-1.9.9/akshare/futures_derivative/futures_sina_cot.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/futures_derivative/sina_futures_index.py` & `akshare-1.9.9/akshare/futures_derivative/sina_futures_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/30 20:41
+Date: 2021/12/22 15:41
 Desc: 新浪财经-期货的主力合约数据
 https://finance.sina.com.cn/futuremarket/index.shtml
 """
 import pandas as pd
 import requests
 
 from akshare.futures.cons import (
@@ -16,15 +16,15 @@
 from akshare.utils import demjson
 
 
 def zh_subscribe_exchange_symbol(symbol: str = "dce") -> pd.DataFrame:
     """
     订阅指定交易所品种的代码
     https://finance.sina.com.cn/futuremarket/index.shtml
-    :param symbol: choice of {"dce", "czce", "shfe", "cffex", "gfex"}
+    :param symbol: choice of {"dce", "czce", "shfe", "cffex"}
     :type symbol: str
     :return: 订阅指定交易所品种的代码
     :rtype: pandas.DataFrame
     """
     r = requests.get(zh_subscribe_exchange_symbol_url)
     r.encoding = "gb2312"
     data_json = demjson.decode(
@@ -38,24 +38,21 @@
         return pd.DataFrame(data_json["dce"])
     if symbol == "shfe":
         data_json["shfe"].remove("上海期货交易所")
         return pd.DataFrame(data_json["shfe"])
     if symbol == "cffex":
         data_json["cffex"].remove("中国金融期货交易所")
         return pd.DataFrame(data_json["cffex"])
-    if symbol == "gfex":
-        data_json["gfex"].remove("广期所")
-        return pd.DataFrame(data_json["gfex"])
 
 
 def match_main_contract(symbol: str = "shfe") -> pd.DataFrame:
     """
     指定交易所的所有可以提供数据的合约
     https://finance.sina.com.cn/futuremarket/index.shtml
-    :param symbol: choice of {"dce", "czce", "shfe", "cffex", "gfex"}
+    :param symbol: choice of {"dce", "czce", "shfe", "cffex"}
     :type symbol: str
     :return: 指定交易所的所有可以提供数据的合约
     :rtype: pandas.DataFrame
     """
     subscribe_list = []
     exchange_symbol_list = (
         zh_subscribe_exchange_symbol(symbol).iloc[:, 1].tolist()
@@ -88,15 +85,15 @@
     """
     新浪主力连续合约品种一览表
     https://finance.sina.com.cn/futuremarket/index.shtml
     :return: 新浪主力连续合约品种一览表
     :rtype: pandas.DataFrame
     """
     temp_df = pd.DataFrame()
-    for item in ["dce", "czce", "shfe", "cffex", "gfex"]:
+    for item in ["dce", "czce", "shfe", "cffex"]:
         temp_df = pd.concat([temp_df, match_main_contract(symbol=item)])
     temp_df.reset_index(inplace=True, drop=True)
     return temp_df
 
 
 def futures_main_sina(
     symbol: str = "V0",
```

### Comparing `akshare-1.9.80/akshare/futures_derivative/sys_spot_futures.py` & `akshare-1.9.9/akshare/futures_derivative/sys_spot_futures.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fx/cons.py` & `akshare-1.9.9/akshare/fx/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fx/currency_investing.py` & `akshare-1.9.9/akshare/fx/currency_investing.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding:utf-8 -*-
 """
 Date: 2022/8/8 20:33
 Desc: 英为财情-外汇-货币对历史数据
 https://cn.investing.com/currencies/
 https://cn.investing.com/currencies/eur-usd-historical-data
 """
+import cfscrape
 import json
 
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 
@@ -43,17 +44,18 @@
     指定 symbol 的所有指数和代码
     https://cn.investing.com/indices/
     :param symbol: 指定的国家或地区；ak._get_global_country_name_url() 函数返回的国家或地区的名称
     :type symbol: str
     :return: 指定 area 的所有指数和代码
     :rtype: dict
     """
+    scraper = cfscrape.create_scraper(delay=10)
     pd.set_option("mode.chained_assignment", None)
     url = f"https://cn.investing.com/currencies/{symbol}-historical-data"
-    r = requests.get(url)
+    r = scraper.get(url)
     soup = BeautifulSoup(r.text, "lxml")
     data_text = soup.find("script", attrs={"id": "__NEXT_DATA__"}).text
     data_json = json.loads(data_text)
     code = json.loads(data_json["props"]["pageProps"]["state"])["dataStore"][
         "pageInfoStore"
     ]["identifiers"]["instrument_id"]
     return code
```

### Comparing `akshare-1.9.80/akshare/fx/fx_quote.py` & `akshare-1.9.9/akshare/fx/fx_quote.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/fx/fx_quote_baidu.py` & `akshare-1.9.9/akshare/fx/fx_quote_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/hf/hf_sp500.py` & `akshare-1.9.9/akshare/hf/hf_sp500.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/cons.py` & `akshare-1.9.9/akshare/index/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/dailydata.py` & `akshare-1.9.9/akshare/index/dailydata.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/drewry_index.py` & `akshare-1.9.9/akshare/index/drewry_index.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_baidu.py` & `akshare-1.9.9/akshare/index/index_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_cflp.py` & `akshare-1.9.9/akshare/index/index_cflp.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_cni.py` & `akshare-1.9.9/akshare/index/index_cni.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_cons.py` & `akshare-1.9.9/akshare/index/index_cons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/10 16:19
+Date: 2021/12/31 13:19
 Desc: 股票指数成份股数据, 新浪有两个接口, 这里使用老接口:
 新接口：http://vip.stock.finance.sina.com.cn/mkt/#zhishu_000001
 老接口：http://vip.stock.finance.sina.com.cn/corp/view/vII_NewestComponent.php?page=1&indexid=399639
 """
 import math
 from io import BytesIO
 
@@ -41,17 +41,15 @@
                 "sort": "symbol",
                 "asc": "1",
                 "node": "hs300",
                 "symbol": "",
                 "_s_r_a": "init",
             }
             r = requests.get(url, params=params)
-            temp_df = pd.concat(
-                [temp_df, pd.DataFrame(demjson.decode(r.text))], ignore_index=True
-            )
+            temp_df = pd.concat([temp_df, pd.DataFrame(demjson.decode(r.text))], ignore_index=True)
         return temp_df
 
     url = "http://vip.stock.finance.sina.com.cn/quotes_service/api/json_v2.php/Market_Center.getHQNodeDataSimple"
     params = {
         "page": 1,
         "num": "3000",
         "sort": "symbol",
@@ -93,26 +91,24 @@
         soup.find(attrs={"class": "table2"})
         .find("td")
         .find_all("a")[-1]["href"]
         .split("page=")[-1]
         .split("&")[0]
     )
     if page_num == "#":
-        temp_df = pd.read_html(r.text, header=0, skiprows=1)[3].iloc[:, :3]
+        temp_df = pd.read_html(r.text, header=1)[3].iloc[:, :3]
         temp_df["品种代码"] = temp_df["品种代码"].astype(str).str.zfill(6)
         return temp_df
 
     temp_df = pd.DataFrame()
     for page in range(1, int(page_num) + 1):
         url = f"http://vip.stock.finance.sina.com.cn/corp/view/vII_NewestComponent.php?page={page}&indexid={symbol}"
         r = requests.get(url)
         r.encoding = "gb2312"
-        temp_df = pd.concat(
-            [temp_df, pd.read_html(r.text, header=1)[3]], ignore_index=True
-        )
+        temp_df = pd.concat([temp_df, pd.read_html(r.text, header=1)[3]], ignore_index=True)
     temp_df = temp_df.iloc[:, :3]
     temp_df["品种代码"] = temp_df["品种代码"].astype(str).str.zfill(6)
     return temp_df
 
 
 def index_stock_cons_csindex(symbol: str = "000300") -> pd.DataFrame:
     """
@@ -133,15 +129,15 @@
         "指数英文名称",
         "成分券代码",
         "成分券名称",
         "成分券英文名称",
         "交易所",
         "交易所英文名称",
     ]
-    temp_df["日期"] = pd.to_datetime(temp_df["日期"], format="%Y%m%d").dt.date
+    temp_df['日期'] = pd.to_datetime(temp_df['日期'], format="%Y%m%d").dt.date
     temp_df["指数代码"] = temp_df["指数代码"].astype(str).str.zfill(6)
     temp_df["成分券代码"] = temp_df["成分券代码"].astype(str).str.zfill(6)
     return temp_df
 
 
 def index_stock_cons_weight_csindex(symbol: str = "000300") -> pd.DataFrame:
     """
@@ -163,18 +159,18 @@
         "成分券代码",
         "成分券名称",
         "成分券英文名称",
         "交易所",
         "交易所英文名称",
         "权重",
     ]
-    temp_df["日期"] = pd.to_datetime(temp_df["日期"], format="%Y%m%d").dt.date
+    temp_df['日期'] = pd.to_datetime(temp_df['日期'], format="%Y%m%d").dt.date
     temp_df["指数代码"] = temp_df["指数代码"].astype(str).str.zfill(6)
     temp_df["成分券代码"] = temp_df["成分券代码"].astype(str).str.zfill(6)
-    temp_df["权重"] = pd.to_numeric(temp_df["权重"])
+    temp_df['权重'] = pd.to_numeric(temp_df['权重'])
     return temp_df
 
 
 def index_stock_hist(symbol: str = "sh000300") -> pd.DataFrame:
     """
     指数历史成份, 从 2005 年开始
     http://stock.jrj.com.cn/share,sh000300,2015nlscf_2.shtml
@@ -220,20 +216,18 @@
         return f"sz{symbol}"
 
 
 if __name__ == "__main__":
     index_stock_cons_csindex_df = index_stock_cons_csindex(symbol="000300")
     print(index_stock_cons_csindex_df)
 
-    index_stock_cons_weight_csindex_df = index_stock_cons_weight_csindex(
-        symbol="000300"
-    )
+    index_stock_cons_weight_csindex_df = index_stock_cons_weight_csindex(symbol="000300")
     print(index_stock_cons_weight_csindex_df)
 
     index_stock_cons_sina_df = index_stock_cons_sina(symbol="000300")
     print(index_stock_cons_sina_df)
 
-    index_stock_cons_df = index_stock_cons(symbol="000688")
+    index_stock_cons_df = index_stock_cons(symbol="000001")
     print(index_stock_cons_df)
 
     stock_index_hist_df = index_stock_hist(symbol="sh000300")
     print(stock_index_hist_df)
```

### Comparing `akshare-1.9.80/akshare/index/index_cx.py` & `akshare-1.9.9/akshare/index/index_cx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_eri.py` & `akshare-1.9.9/akshare/index/index_eri.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_google.py` & `akshare-1.9.9/akshare/index/index_google.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_hog.py` & `akshare-1.9.9/akshare/index/index_hog.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_investing.py` & `akshare-1.9.9/akshare/index/index_investing.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Date: 2022/8/8 19:53
 Desc: 英为财情-股票指数-全球股指与期货指数数据接口
 https://cn.investing.com/indices/volatility-s-p-500-historical-data
 """
 import json
 
+import cfscrape
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 
 from akshare.index.cons import short_headers
 from akshare.utils.ak_session import session
 
@@ -79,18 +80,19 @@
     指定 area 的所有指数和代码
     https://cn.investing.com/indices/
     :param area: 指定的国家或地区；ak._get_global_country_name_url() 函数返回的国家或地区的名称
     :type area: str
     :return: 指定 area 的所有指数和代码
     :rtype: dict
     """
+    scraper = cfscrape.create_scraper(delay=10)
     pd.set_option("mode.chained_assignment", None)
     name_url_dict = _get_global_country_name_url()
     url = f"https://cn.investing.com{name_url_dict[area]}?&majorIndices=on&primarySectors=on&additionalIndices=on&otherIndices=on"
-    r = requests.get(url)
+    r = scraper.get(url)
     soup = BeautifulSoup(r.text, "lxml")
     code_list = [
         item["data-id"]
         for item in soup.find_all("table")[1].find_all(
             "span", attrs={"class": "alertBellGrayPlus"}
         )
     ]
@@ -108,18 +110,19 @@
     指定 area 的所有指数和 URL 地址
     https://cn.investing.com/indices/
     :param area: 指定的国家或地区；ak._get_global_country_name_url() 函数返回的国家或地区的名称
     :type area: str
     :return: 指定 area 的所有指数和 URL 地址
     :rtype: dict
     """
+    scraper = cfscrape.create_scraper(delay=10)
     pd.set_option("mode.chained_assignment", None)
     name_url_dict = _get_global_country_name_url()
     url = f"https://cn.investing.com{name_url_dict[area]}?&majorIndices=on&primarySectors=on&additionalIndices=on&otherIndices=on"
-    r = requests.get(url)
+    r = scraper.get(url)
     soup = BeautifulSoup(r.text, "lxml")
     code_list = [
         item.find("a")["href"]
         for item in soup.find_all("td", attrs={"class": "plusIconTd"})
     ]
     name_list = [
         item.find("a").text
@@ -178,15 +181,16 @@
         "sec-ch-ua-platform": '"Windows"',
         "sec-fetch-dest": "empty",
         "sec-fetch-mode": "cors",
         "sec-fetch-site": "same-site",
         "authorization": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2NjM2NjQ1NzUsImp0aSI6IjIyODA4MDM5MSIsImlhdCI6MTY2MzY2MDk3NSwiaXNzIjoiaW52ZXN0aW5nLmNvbSIsInVzZXJfaWQiOjIyODA4MDM5MSwicHJpbWFyeV9kb21haW5faWQiOiIxIiwiQXV0aG5TeXN0ZW1Ub2tlbiI6IiIsIkF1dGhuU2Vzc2lvblRva2VuIjoiIiwiRGV2aWNlVG9rZW4iOiIiLCJVYXBpVG9rZW4iOiJObmclMkJmMlJyUHpjeWRtdHRaell5TW1JN1pUNWliV1prTURJMVB6czlNeVUySWpVN1lEYzNjV1ZxYWlSZ1kyVjVNamRsWWpRMFptWTFQMkk4TnpCdlBEWXlQbVJrWXo4M01tQnJaMmN3TW1aaU1HVm9ZbWRtWmpBNU5UWTdhRE0lMkJOalUxTW1Cdk56VmxPbW93WUR4bGJUSWdaWGswY0daM05XZGlNamQyYnlnMk9UNSUyRlpEUSUyRllESm1hMjluTURJeFlqRmxQV0l3Wmpjd1pUVXhPenN6S3paOSIsIkF1dGhuSWQiOiIiLCJJc0RvdWJsZUVuY3J5cHRlZCI6ZmFsc2UsIkRldmljZUlkIjoiIiwiUmVmcmVzaEV4cGlyZWRBdCI6MTY2NjE4MDk3NX0.uRLTP1IG3696uxHm3Qq0D8z4o3nfsD3CaIS9cZGjsV0",
         "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36",
     }
-    r = requests.get(url, params=params, headers=headers)
+    scraper = cfscrape.create_scraper(delay=10)
+    r = scraper.get(url, params=params, headers=headers)
     r.encoding = "utf-8"
     r = requests.get(url, params=params, headers=headers)
     data_json = r.json()
     df_data = pd.DataFrame(data_json["data"])
     df_data.columns = [
         "-",
         "-",
@@ -235,15 +239,16 @@
     :type start_date: str
     :param end_date: '20191017', 注意格式
     :type end_date: str
     :return: 指定参数的数据
     :rtype: pandas.DataFrame
     """
     url = url.replace("www", "cn")
-    r = requests.get(url)
+    scraper = cfscrape.create_scraper(delay=10)
+    r = scraper.get(url)
     soup = BeautifulSoup(r.text, "lxml")
     data_text = soup.find("script", attrs={"id": "__NEXT_DATA__"}).text
     data_json = json.loads(data_text)
     code = json.loads(data_json["props"]["pageProps"]["state"])["dataStore"][
         "pageInfoStore"
     ]["identifiers"]["instrument_id"]
     start_date = "-".join([start_date[:4], start_date[4:6], start_date[6:]])
```

### Comparing `akshare-1.9.80/akshare/index/index_kq_fz.py` & `akshare-1.9.9/akshare/index/index_kq_fz.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_kq_ss.py` & `akshare-1.9.9/akshare/index/index_kq_ss.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_spot.py` & `akshare-1.9.9/akshare/index/index_spot.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_stock_hk.py` & `akshare-1.9.9/akshare/news/news_cctv.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,184 +1,181 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/10 18:00
-Desc: 股票指数数据-新浪-东财
-所有指数-实时行情数据和历史行情数据
-https://finance.sina.com.cn/realstock/company/sz399552/nc.shtml
+Date: 2022/5/26 15:42
+Desc: 新闻联播文字稿
+https://tv.cctv.com/lm/xwlb/?spm=C52056131267.P4y8I53JvSWE.0.0
 """
 import re
 
 import pandas as pd
 import requests
-from py_mini_racer import py_mini_racer
+from bs4 import BeautifulSoup
+from tqdm import tqdm
 
-from akshare.index.cons import (
-    zh_sina_index_stock_hist_url,
-)
-from akshare.stock.cons import hk_js_decode
-from akshare.utils import demjson
 
-
-def _replace_comma(x):
-    """
-    去除单元格中的 ","
-    :param x: 单元格元素
-    :type x: str
-    :return: 处理后的值或原值
-    :rtype: str
-    """
-    if "," in str(x):
-        return str(x).replace(",", "")
-    else:
-        return x
-
-
-def get_hk_index_page_count() -> int:
-    """
-    指数的总页数
-    https://vip.stock.finance.sina.com.cn/mkt/#zs_hk
-    :return: 需要抓取的指数的总页数
-    :rtype: int
+def news_cctv(date: str = "20130308") -> pd.DataFrame:
     """
-    res = requests.get("https://vip.stock.finance.sina.com.cn/quotes_service/api/json_v2.php/Market_Center.getNameCount?node=zs_hk")
-    page_count = int(re.findall(re.compile(r"\d+"), res.text)[0]) / 80
-    if isinstance(page_count, int):
-        return page_count
-    else:
-        return int(page_count) + 1
-
-
-def stock_hk_index_spot() -> pd.DataFrame:
-    """
-    新浪财经-行情中心首页-港股-分类-所有指数
-    大量采集会被目标网站服务器封禁 IP, 如果被封禁 IP, 请 10 分钟后再试
-    https://vip.stock.finance.sina.com.cn/mkt/#zs_hk
-    :return: 所有指数的实时行情数据
+    新闻联播文字稿
+    https://tv.cctv.com/lm/xwlb/?spm=C52056131267.P4y8I53JvSWE.0.0
+    :param date: 需要获取数据的日期; 目前 20160203 年后
+    :type date: str
+    :return: 新闻联播文字稿
     :rtype: pandas.DataFrame
     """
-    url = "https://hq.sinajs.cn/rn=mtf2t&list=hkCES100,hkCES120,hkCES280,hkCES300,hkCESA80,hkCESG10,hkCESHKM,hkCSCMC,hkCSHK100,hkCSHKDIV,hkCSHKLC,hkCSHKLRE,hkCSHKMCS,hkCSHKME,hkCSHKPE,hkCSHKSE,hkCSI300,hkCSRHK50,hkGEM,hkHKL,hkHSCCI,hkHSCEI,hkHSI,hkHSMBI,hkHSMOGI,hkHSMPI,hkHSTECH,hkSSE180,hkSSE180GV,hkSSE380,hkSSE50,hkSSECEQT,hkSSECOMP,hkSSEDIV,hkSSEITOP,hkSSEMCAP,hkSSEMEGA,hkVHSI"
-    headers = {
-        "Referer": "https://vip.stock.finance.sina.com.cn/"
-    }
-    r = requests.get(url, headers=headers)
-    data_text = r.text
-    data_list = [item.split('"')[1].split(",") for item in data_text.split("\n") if len(item.split('"')) > 1]
-    temp_df = pd.DataFrame(data_list)
-    temp_df.columns = [
-        "代码",
-        "名称",
-        "今开",
-        "昨收",
-        "最高",
-        "最低",
-        "最新价",
-        "涨跌额",
-        "涨跌幅",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-    ]
-    temp_df = temp_df[
-        [
-            "代码",
-            "名称",
-            "最新价",
-            "涨跌额",
-            "涨跌幅",
-            "昨收",
-            "今开",
-            "最高",
-            "最低",
+    if int(date) <= int("20130708"):
+        url = f"http://cctv.cntv.cn/lm/xinwenlianbo/{date}.shtml"
+        r = requests.get(url)
+        r.encoding = "gbk"
+        raw_list = re.findall(r"title_array_01\((.*)", r.text)
+        page_url = [
+            re.findall("(http.*)", item)[0].split("'")[0]
+            for item in raw_list[1:]
         ]
-    ]
-    temp_df['最新价'] = pd.to_numeric(temp_df['最新价'], errors="coerce")
-    temp_df['涨跌额'] = pd.to_numeric(temp_df['涨跌额'], errors="coerce")
-    temp_df['涨跌幅'] = pd.to_numeric(temp_df['涨跌幅'], errors="coerce")
-    temp_df['昨收'] = pd.to_numeric(temp_df['昨收'], errors="coerce")
-    temp_df['今开'] = pd.to_numeric(temp_df['今开'], errors="coerce")
-    temp_df['最高'] = pd.to_numeric(temp_df['最高'], errors="coerce")
-    temp_df['最低'] = pd.to_numeric(temp_df['最低'], errors="coerce")
-    return temp_df
-
-
-def stock_hk_index_daily(symbol: str = "sh000922") -> pd.DataFrame:
-    """
-    新浪财经-指数-历史行情数据, 大量抓取容易封 IP
-    https://finance.sina.com.cn/realstock/company/sh000909/nc.shtml
-    :param symbol: sz399998, 指定指数代码
-    :type symbol: str
-    :return: 历史行情数据
-    :rtype: pandas.DataFrame
-    """
-    params = {"d": "2020_2_4"}
-    res = requests.get(zh_sina_index_stock_hist_url.format(symbol), params=params)
-    js_code = py_mini_racer.MiniRacer()
-    js_code.eval(hk_js_decode)
-    dict_list = js_code.call(
-        "d", res.text.split("=")[1].split(";")[0].replace('"', "")
-    )  # 执行js解密代码
-    temp_df = pd.DataFrame(dict_list)
-    temp_df["date"] = pd.to_datetime(temp_df["date"]).dt.date
-    temp_df["open"] = pd.to_numeric(temp_df["open"])
-    temp_df["close"] = pd.to_numeric(temp_df["close"])
-    temp_df["high"] = pd.to_numeric(temp_df["high"])
-    temp_df["low"] = pd.to_numeric(temp_df["low"])
-    temp_df["volume"] = pd.to_numeric(temp_df["volume"])
-    return temp_df
-
-
-def stock_hk_index_daily_em(symbol: str = "sh000913") -> pd.DataFrame:
-    """
-    东方财富网-股票指数数据
-    https://quote.eastmoney.com/center/hszs.html
-    :param symbol: 带市场标识的指数代码
-    :type symbol: str
-    :return: 指数数据
-    :rtype: pandas.DataFrame
-    """
-    market_map = {"sz": "0", "sh": "1"}
-    url = "http://push2his.eastmoney.com/api/qt/stock/kline/get"
-    params = {
-        "cb": "jQuery1124033485574041163946_1596700547000",
-        "secid": f"{market_map[symbol[:2]]}.{symbol[2:]}",
-        "ut": "fa5fd1943c7b386f172d6893dbfba10b",
-        "fields1": "f1,f2,f3,f4,f5",
-        "fields2": "f51,f52,f53,f54,f55,f56,f57,f58",
-        "klt": "101",  # 日频率
-        "fqt": "0",
-        "beg": "19900101",
-        "end": "20320101",
-        "_": "1596700547039",
-    }
-    r = requests.get(url, params=params)
-    data_text = r.text
-    data_json = demjson.decode(data_text[data_text.find("{") : -2])
-    temp_df = pd.DataFrame([item.split(",") for item in data_json["data"]["klines"]])
-    temp_df.columns = ["date", "open", "close", "high", "low", "volume", "amount", "_"]
-    temp_df = temp_df[["date", "open", "close", "high", "low", "volume", "amount"]]
-
-    temp_df["open"] = pd.to_numeric(temp_df["open"])
-    temp_df["close"] = pd.to_numeric(temp_df["close"])
-    temp_df["high"] = pd.to_numeric(temp_df["high"])
-    temp_df["low"] = pd.to_numeric(temp_df["low"])
-    temp_df["volume"] = pd.to_numeric(temp_df["volume"])
-    temp_df["amount"] = pd.to_numeric(temp_df["amount"])
-    return temp_df
+        title_list = []
+        content_list = []
+        headers = {
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
+            "Cache-Control": "no-cache",
+            "Cookie": "cna=DLYSGBDthG4CAbRVCNxSxGT6",
+            "Host": "tv.cctv.com",
+            "Pragma": "no-cache",
+            "Proxy-Connection": "keep-alive",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36",
+        }
+        for page in tqdm(page_url, leave=False):
+            try:
+                r = requests.get(page, headers=headers)
+                r.encoding = "utf-8"
+                soup = BeautifulSoup(r.text, "lxml")
+                title = soup.find("h3").text
+                content = soup.find("div", attrs={"class": "cnt_bd"}).text
+                title_list.append(
+                    title.strip("[视频]").strip().replace("\n", " ")
+                )
+                content_list.append(
+                    content.strip()
+                    .strip("央视网消息(新闻联播)：")
+                    .strip("央视网消息（新闻联播）：")
+                    .strip("(新闻联播)：")
+                    .strip()
+                    .replace("\n", " ")
+                )
+            except:
+                continue
+        temp_df = pd.DataFrame(
+            [[date] * len(title_list), title_list, content_list],
+            index=["date", "title", "content"],
+        ).T
+        return temp_df
+
+    elif int(date) < int("20160203"):
+        url = f"http://cctv.cntv.cn/lm/xinwenlianbo/{date}.shtml"
+        r = requests.get(url)
+        r.encoding = "utf-8"
+        soup = BeautifulSoup(r.text, "lxml")
+        page_url = [
+            item.find("a")["href"]
+            for item in soup.find(
+                "div", attrs={"id": "contentELMT1368521805488378"}
+            ).find_all("li")[1:]
+        ]
+        title_list = []
+        content_list = []
+        headers = {
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
+            "Cache-Control": "no-cache",
+            "Cookie": "cna=DLYSGBDthG4CAbRVCNxSxGT6",
+            "Host": "tv.cctv.com",
+            "Pragma": "no-cache",
+            "Proxy-Connection": "keep-alive",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36",
+        }
+        for page in tqdm(page_url, leave=False):
+            try:
+                r = requests.get(page, headers=headers)
+                r.encoding = "utf-8"
+                soup = BeautifulSoup(r.text, "lxml")
+                title = soup.find("h3").text
+                content = soup.find("div", attrs={"class": "cnt_bd"}).text
+                title_list.append(
+                    title.strip("[视频]").strip().replace("\n", " ")
+                )
+                content_list.append(
+                    content.strip()
+                    .strip("央视网消息(新闻联播)：")
+                    .strip("央视网消息（新闻联播）：")
+                    .strip("(新闻联播)：")
+                    .strip()
+                    .replace("\n", " ")
+                )
+            except:
+                continue
+        temp_df = pd.DataFrame(
+            [[date] * len(title_list), title_list, content_list],
+            index=["date", "title", "content"],
+        ).T
+        return temp_df
+    elif int(date) > int("20160203"):
+        url = f"https://tv.cctv.com/lm/xwlb/day/{date}.shtml"
+        r = requests.get(url)
+        r.encoding = "utf-8"
+        soup = BeautifulSoup(r.text, "lxml")
+        page_url = [item.find("a")["href"] for item in soup.find_all("li")[1:]]
+        title_list = []
+        content_list = []
+        headers = {
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
+            "Cache-Control": "no-cache",
+            "Cookie": "cna=DLYSGBDthG4CAbRVCNxSxGT6",
+            "Host": "tv.cctv.com",
+            "Pragma": "no-cache",
+            "Proxy-Connection": "keep-alive",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36",
+        }
+        for page in tqdm(page_url, leave=False):
+            try:
+                r = requests.get(page, headers=headers)
+                r.encoding = "utf-8"
+                soup = BeautifulSoup(r.text, "lxml")
+                if soup.find("h3"):
+                    title = soup.find("h3").text
+                else:
+                    title = soup.find("div", attrs={"class": "tit"}).text
+                if soup.find("div", attrs={"class": "cnt_bd"}):
+                    content = soup.find("div", attrs={"class": "cnt_bd"}).text
+                else:
+                    content = soup.find(
+                        "div", attrs={"class": "content_area"}
+                    ).text
+                title_list.append(
+                    title.strip("[视频]").strip().replace("\n", " ")
+                )
+                content_list.append(
+                    content.strip()
+                    .strip("央视网消息(新闻联播)：")
+                    .strip("央视网消息（新闻联播）：")
+                    .strip("(新闻联播)：")
+                    .strip()
+                    .replace("\n", " ")
+                )
+            except:
+                continue
+        temp_df = pd.DataFrame(
+            [[date] * len(title_list), title_list, content_list],
+            index=["date", "title", "content"],
+        ).T
+        return temp_df
 
 
 if __name__ == "__main__":
-    stock_zh_index_daily_df = stock_hk_index_daily(symbol="sz399905")
-    print(stock_zh_index_daily_df)
-
-    stock_zh_index_spot_df = stock_hk_index_spot()
-    print(stock_zh_index_spot_df)
-
-    stock_zh_index_daily_em_df = stock_hk_index_daily_em(symbol="sz399812")
-    print(stock_zh_index_daily_em_df)
+    news_cctv_df = news_cctv(date="20220525")
+    print(news_cctv_df)
```

### Comparing `akshare-1.9.80/akshare/index/index_stock_zh.py` & `akshare-1.9.9/akshare/index/index_stock_zh.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_sugar.py` & `akshare-1.9.9/akshare/index/index_sugar.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_sw.py` & `akshare-1.9.9/akshare/index/index_sw.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_sw_research.py` & `akshare-1.9.9/akshare/index/index_sw_research.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_weibo.py` & `akshare-1.9.9/akshare/index/index_weibo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_yw.py` & `akshare-1.9.9/akshare/index/index_yw.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/index_zh_em.py` & `akshare-1.9.9/akshare/index/index_zh_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/request.py` & `akshare-1.9.9/akshare/index/request.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/index/stock_zh_index_csindex.py` & `akshare-1.9.9/akshare/index/stock_zh_index_csindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,14 @@
             index_value_name_funddb_df["指数代码"],
         )
     )
     url = "https://api.jiucaishuo.com/v2/guzhi/newtubiaolinedata"
     payload = {
         "gu_code": name_code_map[symbol],
         "pe_category": indicator_map[indicator],
-        "year": -1,
     }
     r = requests.post(url, json=payload)
     data_json = r.json()
     big_df = pd.DataFrame()
     temp_df = pd.DataFrame(
         data_json["data"]["tubiao"]["series"][0]["data"],
         columns=["timestamp", "value"],
```

### Comparing `akshare-1.9.80/akshare/interest_rate/interbank_rate_em.py` & `akshare-1.9.9/akshare/interest_rate/interbank_rate_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/movie/artist_yien.py` & `akshare-1.9.9/akshare/movie/artist_yien.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/movie/jm.js` & `akshare-1.9.9/akshare/movie/jm.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/movie/movie_yien.py` & `akshare-1.9.9/akshare/movie/movie_yien.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/movie/video_yien.py` & `akshare-1.9.9/akshare/movie/video_yien.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/news/news_baidu.py` & `akshare-1.9.9/akshare/news/news_baidu.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 def news_trade_notify_dividend_baidu(date: str = "20220916") -> pd.DataFrame:
     """
     百度股市通-交易提醒-分红派息
     https://gushitong.baidu.com/calendar
     :param date: 查询日期
     :type date: str
-    :return: 交易提醒-分红派息
+    :return: 交易提醒-停复牌
     :rtype: pandas.DataFrame
     """
     start_date = "-".join([date[:4], date[4:6], date[6:]])
     end_date = "-".join([date[:4], date[4:6], date[6:]])
     url = "https://finance.pae.baidu.com/api/financecalendar"
     params = {
         "start_date": start_date,
@@ -227,15 +227,15 @@
             big_df = pd.concat([big_df, temp_df], ignore_index=True)
         else:
             continue
     return big_df
 
 
 if __name__ == "__main__":
-    news_economic_baidu_df = news_economic_baidu(date="20230317")
+    news_economic_baidu_df = news_economic_baidu(date="20220917")
     print(news_economic_baidu_df)
 
     news_trade_notify_suspend_baidu_df = news_trade_notify_suspend_baidu(date="20220916")
     print(news_trade_notify_suspend_baidu_df)
 
     news_trade_notify_dividend_baidu_df = news_trade_notify_dividend_baidu(date="20220916")
     print(news_trade_notify_dividend_baidu_df)
```

### Comparing `akshare-1.9.80/akshare/news/news_cctv.py` & `akshare-1.9.9/akshare/stock_feature/stock_us_hist_futunn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,195 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2022/5/26 15:42
-Desc: 新闻联播文字稿
-https://tv.cctv.com/lm/xwlb/?spm=C52056131267.P4y8I53JvSWE.0.0
+Date: 2022/3/21 15:26
+Desc: 富途牛牛-行情-美股-每日行情
+https://www.futunn.com/stock/HON-US?seo_redirect=1&channel=1244&subchannel=2&from=BaiduAladdin&utm_source=alading_user&utm_medium=website_growth
 """
-import re
+import json
 
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 
 
-def news_cctv(date: str = "20130308") -> pd.DataFrame:
+def stock_us_code_table_fu() -> pd.DataFrame:
     """
-    新闻联播文字稿
-    https://tv.cctv.com/lm/xwlb/?spm=C52056131267.P4y8I53JvSWE.0.0
-    :param date: 需要获取数据的日期; 目前 20160203 年后
-    :type date: str
-    :return: 新闻联播文字稿
+    富途牛牛-行情-美股-美股代码表
+    https://www.futunn.com/stock/HON-US
+    :return: 美股代码表
     :rtype: pandas.DataFrame
     """
-    if int(date) <= int("20130708"):
-        url = f"http://cctv.cntv.cn/lm/xinwenlianbo/{date}.shtml"
-        r = requests.get(url)
-        r.encoding = "gbk"
-        raw_list = re.findall(r"title_array_01\((.*)", r.text)
-        page_url = [
-            re.findall("(http.*)", item)[0].split("'")[0]
-            for item in raw_list[1:]
-        ]
-        title_list = []
-        content_list = []
+    url = "https://www.futunn.com/quote/list/us/1/694"
+    headers = {
+        "accept": "application/json, text/plain, */*",
+        "accept-encoding": "gzip, deflate, br",
+        "accept-language": "zh-CN,zh;q=0.9,en;q=0.8",
+        "cache-control": "no-cache",
+        "futu-x-csrf-token": "FM5ZhxYFQsZM4k9rXk3TMA==-O4oTw/tuNRp5DlJNWo/TNEEfMt8=",
+        "pragma": "no-cache",
+        "referer": "https://www.futunn.com/stock/HON-US?seo_redirect=1&channel=1244&subchannel=2&from=BaiduAladdin&utm_source=alading_user&utm_medium=website_growth",
+        "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.45 Safari/537.36",
+    }
+    r = requests.get(url, headers=headers)
+    data_text = r.text
+    data_json = json.loads(
+        data_text[data_text.find('{"prefetch') : data_text.find(",window._params")]
+    )
+    pd.DataFrame(data_json["prefetch"]["stockList"]["list"])
+    total_page = data_json["prefetch"]["stockList"]["page"]["page_count"]
+    big_df = pd.DataFrame()
+    for page in tqdm(range(1, total_page + 1), leave=False):
+        url = f"https://www.futunn.com/quote/list/us/1/{page}"
         headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
-            "Cache-Control": "no-cache",
-            "Cookie": "cna=DLYSGBDthG4CAbRVCNxSxGT6",
-            "Host": "tv.cctv.com",
-            "Pragma": "no-cache",
-            "Proxy-Connection": "keep-alive",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36",
+            "accept": "application/json, text/plain, */*",
+            "accept-encoding": "gzip, deflate, br",
+            "accept-language": "zh-CN,zh;q=0.9,en;q=0.8",
+            "cache-control": "no-cache",
+            "futu-x-csrf-token": "FM5ZhxYFQsZM4k9rXk3TMA==-O4oTw/tuNRp5DlJNWo/TNEEfMt8=",
+            "pragma": "no-cache",
+            "referer": "https://www.futunn.com/stock/HON-US?seo_redirect=1&channel=1244&subchannel=2&from=BaiduAladdin&utm_source=alading_user&utm_medium=website_growth",
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.45 Safari/537.36",
         }
-        for page in tqdm(page_url, leave=False):
-            try:
-                r = requests.get(page, headers=headers)
-                r.encoding = "utf-8"
-                soup = BeautifulSoup(r.text, "lxml")
-                title = soup.find("h3").text
-                content = soup.find("div", attrs={"class": "cnt_bd"}).text
-                title_list.append(
-                    title.strip("[视频]").strip().replace("\n", " ")
-                )
-                content_list.append(
-                    content.strip()
-                    .strip("央视网消息(新闻联播)：")
-                    .strip("央视网消息（新闻联播）：")
-                    .strip("(新闻联播)：")
-                    .strip()
-                    .replace("\n", " ")
-                )
-            except:
-                continue
-        temp_df = pd.DataFrame(
-            [[date] * len(title_list), title_list, content_list],
-            index=["date", "title", "content"],
-        ).T
-        return temp_df
-
-    elif int(date) < int("20160203"):
-        url = f"http://cctv.cntv.cn/lm/xinwenlianbo/{date}.shtml"
-        r = requests.get(url)
-        r.encoding = "utf-8"
-        soup = BeautifulSoup(r.text, "lxml")
-        page_url = [
-            item.find("a")["href"]
-            for item in soup.find(
-                "div", attrs={"id": "contentELMT1368521805488378"}
-            ).find_all("li")[1:]
+        r = requests.get(url, headers=headers)
+        data_text = r.text
+        data_json = json.loads(
+            data_text[data_text.find('{"prefetch') : data_text.find(",window._params")]
+        )
+        temp_df = pd.DataFrame(data_json["prefetch"]["stockList"]["list"])
+        big_df = pd.concat([big_df, temp_df], ignore_index=True)
+    big_df.columns = [
+        "代码",
+        "最新价",
+        "成交额",
+        "成交量",
+        "换手率",
+        "振幅",
+        "涨跌额",
+        "涨跌幅",
+        "-",
+        "股票名称",
+        "股票简称",
+        "-",
+    ]
+    big_df = big_df[
+        [
+            "代码",
+            "股票名称",
+            "股票简称",
+            "最新价",
+            "涨跌额",
+            "涨跌幅",
+            "成交量",
+            "成交额",
+            "换手率",
+            "振幅",
         ]
-        title_list = []
-        content_list = []
-        headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
-            "Cache-Control": "no-cache",
-            "Cookie": "cna=DLYSGBDthG4CAbRVCNxSxGT6",
-            "Host": "tv.cctv.com",
-            "Pragma": "no-cache",
-            "Proxy-Connection": "keep-alive",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36",
-        }
-        for page in tqdm(page_url, leave=False):
-            try:
-                r = requests.get(page, headers=headers)
-                r.encoding = "utf-8"
-                soup = BeautifulSoup(r.text, "lxml")
-                title = soup.find("h3").text
-                content = soup.find("div", attrs={"class": "cnt_bd"}).text
-                title_list.append(
-                    title.strip("[视频]").strip().replace("\n", " ")
-                )
-                content_list.append(
-                    content.strip()
-                    .strip("央视网消息(新闻联播)：")
-                    .strip("央视网消息（新闻联播）：")
-                    .strip("(新闻联播)：")
-                    .strip()
-                    .replace("\n", " ")
-                )
-            except:
-                continue
-        temp_df = pd.DataFrame(
-            [[date] * len(title_list), title_list, content_list],
-            index=["date", "title", "content"],
-        ).T
-        return temp_df
-    elif int(date) > int("20160203"):
-        url = f"https://tv.cctv.com/lm/xwlb/day/{date}.shtml"
-        r = requests.get(url)
-        r.encoding = "utf-8"
-        soup = BeautifulSoup(r.text, "lxml")
-        page_url = [item.find("a")["href"] for item in soup.find_all("li")[1:]]
-        title_list = []
-        content_list = []
-        headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
-            "Cache-Control": "no-cache",
-            "Cookie": "cna=DLYSGBDthG4CAbRVCNxSxGT6",
-            "Host": "tv.cctv.com",
-            "Pragma": "no-cache",
-            "Proxy-Connection": "keep-alive",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36",
-        }
-        for page in tqdm(page_url, leave=False):
-            try:
-                r = requests.get(page, headers=headers)
-                r.encoding = "utf-8"
-                soup = BeautifulSoup(r.text, "lxml")
-                if soup.find("h3"):
-                    title = soup.find("h3").text
-                else:
-                    title = soup.find("div", attrs={"class": "tit"}).text
-                if soup.find("div", attrs={"class": "cnt_bd"}):
-                    content = soup.find("div", attrs={"class": "cnt_bd"}).text
-                else:
-                    content = soup.find(
-                        "div", attrs={"class": "content_area"}
-                    ).text
-                title_list.append(
-                    title.strip("[视频]").strip().replace("\n", " ")
-                )
-                content_list.append(
-                    content.strip()
-                    .strip("央视网消息(新闻联播)：")
-                    .strip("央视网消息（新闻联播）：")
-                    .strip("(新闻联播)：")
-                    .strip()
-                    .replace("\n", " ")
-                )
-            except:
-                continue
-        temp_df = pd.DataFrame(
-            [[date] * len(title_list), title_list, content_list],
-            index=["date", "title", "content"],
-        ).T
-        return temp_df
+    ]
+    big_df["最新价"] = pd.to_numeric(big_df["最新价"])
+    big_df["涨跌额"] = pd.to_numeric(big_df["涨跌额"])
+    big_df["涨跌幅"] = big_df["涨跌幅"].str.strip("%")
+    big_df["涨跌幅"] = pd.to_numeric(big_df["涨跌幅"])
+    big_df["换手率"] = big_df["换手率"].str.strip("%")
+    big_df["换手率"] = pd.to_numeric(big_df["换手率"])
+    big_df["振幅"] = big_df["振幅"].str.strip("%")
+    big_df["振幅"] = pd.to_numeric(big_df["振幅"])
+    return big_df
+
+
+def stock_us_hist_fu(
+    symbol: str = "202545",
+    start_date: str = "19700101",
+    end_date: str = "22220101",
+) -> pd.DataFrame:
+    """
+    富途牛牛-行情-美股-每日行情
+    https://www.futunn.com/stock/HON-US
+    :param symbol: 股票代码; 此股票代码可以通过调用 ak.stock_us_code_table_fu() 的 `代码` 字段获取
+    :type symbol: str
+    :param start_date: 开始日期
+    :type start_date: str
+    :param end_date: 结束日期
+    :type end_date: str
+    :return: 每日行情
+    :rtype: pandas.DataFrame
+    """
+    url = "https://www.futunn.com/stock/HON-US?seo_redirect=1&channel=1244&subchannel=2&from=BaiduAladdin&utm_source=alading_user&utm_medium=website_growth"
+    headers = {
+        "accept": "application/json, text/plain, */*",
+        "accept-encoding": "gzip, deflate, br",
+        "accept-language": "zh-CN,zh;q=0.9,en;q=0.8",
+        "cache-control": "no-cache",
+        "futu-x-csrf-token": "FM5ZhxYFQsZM4k9rXk3TMA==-O4oTw/tuNRp5DlJNWo/TNEEfMt8=",
+        "pragma": "no-cache",
+        "referer": "https://www.futunn.com/stock/HON-US?seo_redirect=1&channel=1244&subchannel=2&from=BaiduAladdin&utm_source=alading_user&utm_medium=website_growth",
+        "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.45 Safari/537.36",
+    }
+    session_ = requests.session()
+    r = session_.get(url, headers=headers)
+    soup = BeautifulSoup(r.text, "lxml")
+    url = "https://www.futunn.com/quote-api/get-kline"
+    params = {
+        "stock_id": symbol,
+        "market_type": "2",
+        "type": "2",
+    }
+    headers = {
+        "accept": "application/json, text/plain, */*",
+        "accept-encoding": "gzip, deflate, br",
+        "accept-language": "zh-CN,zh;q=0.9,en;q=0.8",
+        "cache-control": "no-cache",
+        "futu-x-csrf-token": soup.find("meta")["content"],
+        "pragma": "no-cache",
+        "referer": "https://www.futunn.com/stock/HON-US?seo_redirect=1&channel=1244&subchannel=2&from=BaiduAladdin&utm_source=alading_user&utm_medium=website_growth",
+        "sec-fetch-dest": "empty",
+        "sec-fetch-mode": "cors",
+        "sec-fetch-site": "same-origin",
+        "user-agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Mobile/15E148 Safari/604.1",
+    }
+    r = session_.get(url, params=params, headers=headers)
+    data_json = r.json()
+    temp_df = pd.DataFrame(data_json["data"]["list"])
+    temp_df.columns = [
+        "日期",
+        "今开",
+        "今收",
+        "最高",
+        "最低",
+        "成交量",
+        "成交额",
+        "换手率",
+        "-",
+        "昨收",
+    ]
+    temp_df = temp_df[
+        [
+            "日期",
+            "今开",
+            "今收",
+            "最高",
+            "最低",
+            "成交量",
+            "成交额",
+            "换手率",
+            "昨收",
+        ]
+    ]
+    temp_df.index = pd.to_datetime(temp_df["日期"], unit="s")
+    temp_df = temp_df[start_date:end_date]
+    temp_df.reset_index(inplace=True, drop=True)
+    temp_df["日期"] = pd.to_datetime(temp_df["日期"], unit="s").dt.date
+    temp_df["今开"] = pd.to_numeric(temp_df["今开"]) / 100
+    temp_df["最高"] = pd.to_numeric(temp_df["最高"]) / 100
+    temp_df["最低"] = pd.to_numeric(temp_df["最低"]) / 100
+    temp_df["今收"] = pd.to_numeric(temp_df["今收"]) / 100
+    temp_df["昨收"] = pd.to_numeric(temp_df["昨收"]) / 100
+    return temp_df
 
 
 if __name__ == "__main__":
-    news_cctv_df = news_cctv(date="20220525")
-    print(news_cctv_df)
+    stock_us_hist_fu_df = stock_us_hist_fu(symbol="202545")
+    print(stock_us_hist_fu_df)
+
+    stock_us_code_table_fu_df = stock_us_code_table_fu()
+    print(stock_us_code_table_fu_df)
```

### Comparing `akshare-1.9.80/akshare/news/news_stock.py` & `akshare-1.9.9/akshare/news/news_stock.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/nlp/nlp_interface.py` & `akshare-1.9.9/akshare/nlp/nlp_interface.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/cons.py` & `akshare-1.9.9/akshare/option/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_commodity_sina.py` & `akshare-1.9.9/akshare/option/option_commodity_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_czce.py` & `akshare-1.9.9/akshare/option/option_czce.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_em.py` & `akshare-1.9.9/akshare/option/option_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_finance.py` & `akshare-1.9.9/akshare/option/option_finance.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_finance_sina.py` & `akshare-1.9.9/akshare/option/option_finance_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_lhb_em.py` & `akshare-1.9.9/akshare/option/option_lhb_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_premium_analysis_em.py` & `akshare-1.9.9/akshare/option/option_premium_analysis_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_qvix.py` & `akshare-1.9.9/akshare/option/option_qvix.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_risk_indicator_sse.py` & `akshare-1.9.9/akshare/option/option_risk_indicator_sse.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/option/option_value_analysis_em.py` & `akshare-1.9.9/akshare/option/option_value_analysis_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/other/other_car.py` & `akshare-1.9.9/akshare/other/other_car.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/other/other_game.py` & `akshare-1.9.9/akshare/other/other_game.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/pro/client.py` & `akshare-1.9.9/akshare/pro/client.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/pro/data_pro.py` & `akshare-1.9.9/akshare/pro/data_pro.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/qhkc/qhkc_api.py` & `akshare-1.9.9/akshare/qhkc/qhkc_api.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/qhkc_web/qhkc_fund.py` & `akshare-1.9.9/akshare/qhkc_web/qhkc_fund.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/qhkc_web/qhkc_index.py` & `akshare-1.9.9/akshare/qhkc_web/qhkc_index.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/qhkc_web/qhkc_tool.py` & `akshare-1.9.9/akshare/qhkc_web/qhkc_tool.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/rate/repo_rate.py` & `akshare-1.9.9/akshare/rate/repo_rate.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/reits/reits_basic.py` & `akshare-1.9.9/akshare/option/option_risk_analysis_em.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,82 @@
-#!/usr/bin/env python
 # -*- coding:utf-8 -*-
+# !/usr/bin/env python
 """
-Date: 2023/3/30 15:59
-Desc: REITs 行情及信息
-https://quote.eastmoney.com/center/gridlist.html#fund_reits_all
-https://www.jisilu.cn/data/cnreits/#CnReits
+Date: 2022/1/25 10:20
+Desc: 东方财富网-数据中心-特色数据-期权风险分析
+https://data.eastmoney.com/other/riskanal.html
 """
-import pandas as pd
 import requests
+import pandas as pd
 
 
-def reits_realtime_em() -> pd.DataFrame:
+def option_risk_analysis_em() -> pd.DataFrame:
     """
-    东方财富网-行情中心-REITs-沪深 REITs
-    https://quote.eastmoney.com/center/gridlist.html#fund_reits_all
-    :return: 沪深 REITs-实时行情
+    东方财富网-数据中心-特色数据-期权风险分析
+    https://data.eastmoney.com/other/riskanal.html
+    :return: 期权风险分析
     :rtype: pandas.DataFrame
     """
-    url = "http://95.push2.eastmoney.com/api/qt/clist/get"
+    url = "https://push2.eastmoney.com/api/qt/clist/get"
     params = {
-        "pn": "1",
-        "pz": "20",
-        "po": "1",
-        "np": "1",
-        "ut": "bd1d9ddb04089700cf9c27f6f7426281",
-        "fltt": "2",
-        "invt": "2",
-        "fid": "f3",
-        "fs": "m:1 t:9 e:97,m:0 t:10 e:97",
-        "fields": "f2,f3,f4,f5,f6,f12,f14,f15,f16,f17,f18",
-        "_": "1630048369992",
+        'fid': 'f3',
+        'po': '1',
+        'pz': '5000',
+        'pn': '1',
+        'np': '1',
+        'fltt': '2',
+        'invt': '2',
+        'ut': 'b2884a393a59ad64002292a3e90d46a5',
+        'fields': 'f1,f2,f3,f12,f13,f14,f302,f303,f325,f326,f327,f329,f328,f301,f152,f154',
+        'fs': 'm:10'
     }
     r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["data"]["diff"])
-    temp_df.reset_index(inplace=True)
-    temp_df["index"] = range(1, len(temp_df) + 1)
-    temp_df.rename(
-        columns={
-            "index": "序号",
-            "f2": "最新价",
-            "f3": "涨跌幅",
-            "f4": "涨跌额",
-            "f5": "成交量",
-            "f6": "成交额",
-            "f12": "代码",
-            "f14": "名称",
-            "f15": "最高价",
-            "f16": "最低价",
-            "f17": "开盘价",
-            "f18": "昨收",
-        },
-        inplace=True,
-    )
-    temp_df = temp_df[
-        [
-            "序号",
-            "代码",
-            "名称",
-            "最新价",
-            "涨跌额",
-            "涨跌幅",
-            "成交量",
-            "成交额",
-            "开盘价",
-            "最高价",
-            "最低价",
-            "昨收",
-        ]
+    temp_df.columns = [
+        '-',
+        '最新价',
+        '涨跌幅',
+        '期权代码',
+        '-',
+        '期权名称',
+        '-',
+        '-',
+        '到期日',
+        '杠杆比率',
+        '实际杠杆比率',
+        'Delta',
+        'Gamma',
+        'Vega',
+        'Theta',
+        'Rho',
     ]
+    temp_df = temp_df[[
+        '期权代码',
+        '期权名称',
+        '最新价',
+        '涨跌幅',
+        '杠杆比率',
+        '实际杠杆比率',
+        'Delta',
+        'Gamma',
+        'Vega',
+        'Rho',
+        'Theta',
+        '到期日',
+    ]]
     temp_df['最新价'] = pd.to_numeric(temp_df['最新价'], errors="coerce")
-    temp_df['涨跌额'] = pd.to_numeric(temp_df['涨跌额'], errors="coerce")
     temp_df['涨跌幅'] = pd.to_numeric(temp_df['涨跌幅'], errors="coerce")
-    temp_df['成交量'] = pd.to_numeric(temp_df['成交量'], errors="coerce")
-    temp_df['成交额'] = pd.to_numeric(temp_df['成交额'], errors="coerce")
-    temp_df['开盘价'] = pd.to_numeric(temp_df['开盘价'], errors="coerce")
-    temp_df['最高价'] = pd.to_numeric(temp_df['最高价'], errors="coerce")
-    temp_df['最低价'] = pd.to_numeric(temp_df['最低价'], errors="coerce")
-    temp_df['昨收'] = pd.to_numeric(temp_df['昨收'], errors="coerce")
+    temp_df['杠杆比率'] = pd.to_numeric(temp_df['杠杆比率'], errors="coerce")
+    temp_df['实际杠杆比率'] = pd.to_numeric(temp_df['实际杠杆比率'], errors="coerce")
+    temp_df['Delta'] = pd.to_numeric(temp_df['Delta'], errors="coerce")
+    temp_df['Gamma'] = pd.to_numeric(temp_df['Gamma'], errors="coerce")
+    temp_df['Vega'] = pd.to_numeric(temp_df['Vega'], errors="coerce")
+    temp_df['Rho'] = pd.to_numeric(temp_df['Rho'], errors="coerce")
+    temp_df['Theta'] = pd.to_numeric(temp_df['Theta'], errors="coerce")
+    temp_df['到期日'] = pd.to_datetime(temp_df['到期日'].astype(str)).dt.date
     return temp_df
 
 
 if __name__ == "__main__":
-    reits_realtime_em_df = reits_realtime_em()
-    print(reits_realtime_em_df)
+    option_risk_analysis_em_df = option_risk_analysis_em()
+    print(option_risk_analysis_em_df)
```

### Comparing `akshare-1.9.80/akshare/sport/sport_olympic.py` & `akshare-1.9.9/akshare/sport/sport_olympic.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/sport/sport_olympic_winter.py` & `akshare-1.9.9/akshare/sport/sport_olympic_winter.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/spot/spot_sge.py` & `akshare-1.9.9/akshare/spot/spot_sge.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/cons.py` & `akshare-1.9.9/akshare/stock/cons.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_allotment_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_allotment_cninfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2022/10/8 18:11
+Date: 2022/10/08 18:11
 Desc: 巨潮资讯-数据浏览器-筹资指标-公司配股实施方案
 http://webapi.cninfo.com.cn/#/dataBrowse
 """
 import time
 
 import pandas as pd
 import requests
```

### Comparing `akshare-1.9.80/akshare/stock/stock_board_concept_em.py` & `akshare-1.9.9/akshare/stock/stock_board_concept_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_board_industry_em.py` & `akshare-1.9.9/akshare/stock/stock_board_industry_em.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/3/21 22:27
+Date: 2022/6/22 17:27
 Desc: 东方财富-沪深板块-行业板块
-https://quote.eastmoney.com/center/boardlist.html#industry_board
+http://quote.eastmoney.com/center/boardlist.html#industry_board
 """
-import re
 import requests
 import pandas as pd
 
 
 def stock_board_industry_name_em() -> pd.DataFrame:
     """
     东方财富网-沪深板块-行业板块-名称
-    https://quote.eastmoney.com/center/boardlist.html#industry_board
+    http://quote.eastmoney.com/center/boardlist.html#industry_board
     :return: 行业板块-名称
     :rtype: pandas.DataFrame
     """
     url = "http://17.push2.eastmoney.com/api/qt/clist/get"
     params = {
         "pn": "1",
         "pz": "2000",
@@ -103,66 +102,14 @@
     temp_df["换手率"] = pd.to_numeric(temp_df["换手率"], errors="coerce")
     temp_df["上涨家数"] = pd.to_numeric(temp_df["上涨家数"], errors="coerce")
     temp_df["下跌家数"] = pd.to_numeric(temp_df["下跌家数"], errors="coerce")
     temp_df["领涨股票-涨跌幅"] = pd.to_numeric(temp_df["领涨股票-涨跌幅"], errors="coerce")
     return temp_df
 
 
-def stock_board_industry_spot_em(symbol: str = "小金属") -> pd.DataFrame:
-    """
-    东方财富网-沪深板块-行业板块-实时行情
-    https://quote.eastmoney.com/bk/90.BK1027.html
-    :param symbol: 板块名称 or 东财板块代码
-    :type symbol: str
-    :return: 实时行情
-    :rtype: pandas.DataFrame
-    """
-    url = "http://91.push2.eastmoney.com/api/qt/stock/get"
-    field_map = {
-        "f43": "最新",
-        "f44": "最高",
-        "f45": "最低",
-        "f46": "开盘",
-        "f47": "成交量",
-        "f48": "成交额",
-        "f170": "涨跌幅",
-        "f171": "振幅",
-        "f168": "换手率",
-        "f169": "涨跌额",
-    }
-
-    if re.match(r'^BK\d+', symbol):
-        em_code = symbol
-    else:
-        industry_listing = stock_board_industry_name_em()
-        em_code = industry_listing.query('板块名称 == @symbol')["板块代码"].values[0]
-
-    params = dict(
-        fields=','.join(field_map.keys()),
-        mpi="1000",
-        invt="2",
-        fltt="1",
-        secid=f"90.{em_code}",
-        ut="fa5fd1943c7b386f172d6893dbfba10b",
-    )
-    r = requests.get(url, params=params)
-    data_dict = r.json()
-    result = pd.DataFrame.from_dict(data_dict["data"], orient="index")
-    result.rename(field_map, inplace=True)
-    result.reset_index(inplace=True)
-    result.columns = ['item', "value"]
-    result['value'] = pd.to_numeric(result['value'], errors="coerce")
-
-    # 各项转换成正常单位. 除了成交量与成交额, 原始数据中已是正常单位(元)
-    result['value'] = result['value'] * 1e-2
-    result.iloc[4, 1] = result.iloc[4, 1] * 1e2
-    result.iloc[5, 1] = result.iloc[5, 1] * 1e2
-    return result
-
-
 def stock_board_industry_hist_em(
     symbol: str = "小金属",
     start_date: str = "20211201",
     end_date: str = "20220401",
     period: str = "日k",
     adjust: str = "",
 ) -> pd.DataFrame:
@@ -253,15 +200,15 @@
 
 
 def stock_board_industry_hist_min_em(
     symbol: str = "小金属", period: str = "5"
 ) -> pd.DataFrame:
     """
     东方财富网-沪深板块-行业板块-分时历史行情
-    https://quote.eastmoney.com/bk/90.BK1027.html
+    http://quote.eastmoney.com/bk/90.BK1027.html
     :param symbol: 板块名称
     :type symbol: str
     :param period: choice of {"1", "5", "15", "30", "60"}
     :type period: str
     :return: 分时历史行情
     :rtype: pandas.DataFrame
     """
@@ -432,17 +379,14 @@
     return temp_df
 
 
 if __name__ == "__main__":
     stock_board_industry_name_em_df = stock_board_industry_name_em()
     print(stock_board_industry_name_em_df)
 
-    stock_board_industry_spot_em_df = stock_board_industry_spot_em(symbol="小金属")
-    print(stock_board_industry_spot_em_df)
-
     stock_board_industry_hist_em_df = stock_board_industry_hist_em(
         symbol="小金属", start_date="20211201", end_date="20221110", period="月k", adjust=""
     )
     print(stock_board_industry_hist_em_df)
 
     stock_board_industry_hist_min_em_df = stock_board_industry_hist_min_em(
         symbol="小金属", period="60"
```

### Comparing `akshare-1.9.80/akshare/stock/stock_cg_equity_mortgage.py` & `akshare-1.9.9/akshare/stock/stock_cg_equity_mortgage.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_cg_guarantee.py` & `akshare-1.9.9/akshare/stock/stock_cg_guarantee.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_cg_lawsuit.py` & `akshare-1.9.9/akshare/stock/stock_cg_lawsuit.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_dividents_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_dividents_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_dzjy_em.py` & `akshare-1.9.9/akshare/stock/stock_dzjy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_fund_hold.py` & `akshare-1.9.9/akshare/stock/stock_fund_hold.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_hk_sina.py` & `akshare-1.9.9/akshare/stock/stock_hk_sina.py`

 * *Files 16% similar despite different names*

```diff
@@ -65,43 +65,40 @@
     :param symbol: 可以使用 stock_hk_spot 获取
     :type symbol: str
     :param adjust: "": 返回未复权的数据 ; qfq: 返回前复权后的数据; qfq-factor: 返回前复权因子和调整;
     :type adjust: str
     :return: 指定 adjust 的数据
     :rtype: pandas.DataFrame
     """
-    r = requests.get(hk_sina_stock_hist_url.format(symbol))
+    res = requests.get(hk_sina_stock_hist_url.format(symbol))
     js_code = py_mini_racer.MiniRacer()
     js_code.eval(hk_js_decode)
     dict_list = js_code.call(
-        "d", r.text.split("=")[1].split(";")[0].replace('"', "")
+        "d", res.text.split("=")[1].split(";")[0].replace('"', "")
     )  # 执行js解密代码
     data_df = pd.DataFrame(dict_list)
     data_df.index = pd.to_datetime(data_df["date"]).dt.date
     del data_df["date"]
     data_df = data_df.astype("float")
 
     if adjust == "":
         data_df.reset_index(inplace=True)
-        data_df['date'] = pd.to_datetime(data_df['date']).dt.date
         return data_df
 
     if adjust == "hfq":
-        r = requests.get(hk_sina_stock_hist_hfq_url.format(symbol))
+        res = requests.get(hk_sina_stock_hist_hfq_url.format(symbol))
         try:
             hfq_factor_df = pd.DataFrame(
-                eval(r.text.split("=")[1].split("\n")[0])["data"]
+                eval(res.text.split("=")[1].split("\n")[0])["data"]
             )
             if len(hfq_factor_df) == 1:
                 data_df.reset_index(inplace=True)
-                data_df['date'] = pd.to_datetime(data_df['date']).dt.date
                 return data_df
         except SyntaxError as e:
             data_df.reset_index(inplace=True)
-            data_df['date'] = pd.to_datetime(data_df['date']).dt.date
             return data_df
         hfq_factor_df.columns = ["date", "hfq_factor", "cash"]
         hfq_factor_df.index = pd.to_datetime(hfq_factor_df.date)
         del hfq_factor_df["date"]
 
         # 处理复权因子
         temp_date_range = pd.date_range(
@@ -127,31 +124,29 @@
         temp_df["close"] = temp_df["close"] * temp_df["hfq_factor"] + temp_df["cash"]
         temp_df["low"] = temp_df["low"] * temp_df["hfq_factor"] + temp_df["cash"]
         temp_df = temp_df.apply(lambda x: round(x, 4))
         temp_df.dropna(how="any", inplace=True)
         temp_df = temp_df.iloc[:, :-2]
         temp_df.reset_index(inplace=True)
         temp_df.rename({"index": "date"}, axis='columns', inplace=True)
-        temp_df['date'] = pd.to_datetime(temp_df['date']).dt.date
+        temp_df['date'] = temp_df['date'].astype(str)
         return temp_df
 
     if adjust == "qfq":
-        r = requests.get(hk_sina_stock_hist_qfq_url.format(symbol))
+        res = requests.get(hk_sina_stock_hist_qfq_url.format(symbol))
         try:
             qfq_factor_df = pd.DataFrame(
-                eval(r.text.split("=")[1].split("\n")[0])["data"]
+                eval(res.text.split("=")[1].split("\n")[0])["data"]
             )
             if len(qfq_factor_df) == 1:
                 data_df.reset_index(inplace=True)
-                data_df['date'] = pd.to_datetime(data_df['date']).dt.date
                 return data_df
 
         except SyntaxError as e:
             data_df.reset_index(inplace=True)
-            data_df['date'] = pd.to_datetime(data_df['date']).dt.date
             return data_df
         qfq_factor_df.columns = ["date", "qfq_factor"]
         qfq_factor_df.index = pd.to_datetime(qfq_factor_df.date)
         del qfq_factor_df["date"]
 
         temp_date_range = pd.date_range(
             "1900-01-01", qfq_factor_df.index[0].isoformat()
@@ -176,39 +171,39 @@
         temp_df["close"] = temp_df["close"] * temp_df["qfq_factor"]
         temp_df["low"] = temp_df["low"] * temp_df["qfq_factor"]
         temp_df = temp_df.apply(lambda x: round(x, 4))
         temp_df.dropna(how="any", inplace=True)
         temp_df = temp_df.iloc[:, :-1]
         temp_df.reset_index(inplace=True)
         temp_df.rename({"index": "date"}, axis='columns', inplace=True)
-        temp_df['date'] = pd.to_datetime(temp_df['date']).dt.date
+        temp_df['date'] = temp_df['date'].astype(str)
         return temp_df
 
     if adjust == "hfq-factor":
-        r = requests.get(hk_sina_stock_hist_hfq_url.format(symbol))
+        res = requests.get(hk_sina_stock_hist_hfq_url.format(symbol))
         hfq_factor_df = pd.DataFrame(
-            eval(r.text.split("=")[1].split("\n")[0])["data"]
+            eval(res.text.split("=")[1].split("\n")[0])["data"]
         )
         hfq_factor_df.columns = ["date", "hfq_factor", "cash"]
         hfq_factor_df.index = pd.to_datetime(hfq_factor_df.date)
         del hfq_factor_df["date"]
         hfq_factor_df.reset_index(inplace=True)
-        hfq_factor_df['date'] = pd.to_datetime(hfq_factor_df['date']).dt.date
+        hfq_factor_df['date'] = hfq_factor_df['date'].astype(str)
         return hfq_factor_df
 
     if adjust == "qfq-factor":
-        r = requests.get(hk_sina_stock_hist_qfq_url.format(symbol))
+        res = requests.get(hk_sina_stock_hist_qfq_url.format(symbol))
         qfq_factor_df = pd.DataFrame(
-            eval(r.text.split("=")[1].split("\n")[0])["data"]
+            eval(res.text.split("=")[1].split("\n")[0])["data"]
         )
         qfq_factor_df.columns = ["date", "qfq_factor"]
         qfq_factor_df.index = pd.to_datetime(qfq_factor_df.date)
         del qfq_factor_df["date"]
         qfq_factor_df.reset_index(inplace=True)
-        qfq_factor_df['date'] = pd.to_datetime(qfq_factor_df['date']).dt.date
+        qfq_factor_df['date'] = qfq_factor_df['date'].astype(str)
         return qfq_factor_df
 
 
 if __name__ == "__main__":
     stock_hk_daily_hfq_df = stock_hk_daily(symbol="00700", adjust="")
     print(stock_hk_daily_hfq_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_hold_control_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_hold_control_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_hold_num_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_hold_num_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_hot_rank_em.py` & `akshare-1.9.9/akshare/stock/stock_hot_rank_em.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-#!/usr/bin/env python
 # -*- coding:utf-8 -*-
+#!/usr/bin/env python
 """
-Date: 2023/3/25 15:15
+Date: 2022/5/12 15:15
 Desc: 东方财富个股人气榜
 https://guba.eastmoney.com/rank/
 """
-import pandas as pd
 import requests
+import pandas as pd
 
 
 def stock_hot_rank_em() -> pd.DataFrame:
     """
     东方财富-个股人气榜-人气榜
     https://guba.eastmoney.com/rank/
     :return: 人气榜
@@ -52,16 +52,16 @@
             "当前排名",
             "代码",
             "股票名称",
             "最新价",
             "涨跌幅",
         ]
     ]
-    temp_df["最新价"] = pd.to_numeric(temp_df["最新价"], errors="coerce")
-    temp_df["涨跌幅"] = pd.to_numeric(temp_df["涨跌幅"], errors="coerce")
+    temp_df['最新价'] = pd.to_numeric(temp_df['最新价'], errors="coerce")
+    temp_df['涨跌幅'] = pd.to_numeric(temp_df['涨跌幅'], errors="coerce")
     return temp_df
 
 
 def stock_hot_rank_detail_em(symbol: str = "SZ000665") -> pd.DataFrame:
     """
     东方财富-个股人气榜-历史趋势及粉丝特征
     https://guba.eastmoney.com/rank/stock?code=000665
@@ -110,16 +110,16 @@
         "appId": "appId01",
         "globalId": "786e4c21-70dc-435a-93bb-38",
         "marketType": "",
         "srcSecurityCode": symbol,
     }
     r = requests.post(url, json=payload)
     data_json = r.json()
-    temp_df = pd.DataFrame(data_json["data"])
-    temp_df.columns = ["时间", "排名"]
+    temp_df = pd.DataFrame(data_json['data'])
+    temp_df.columns = ['时间', '排名']
     return temp_df
 
 
 def stock_hot_keyword_em(symbol: str = "SZ000665") -> pd.DataFrame:
     """
     东方财富-个股人气榜-热门关键词
     https://guba.eastmoney.com/rank/stock?code=000665
@@ -132,17 +132,17 @@
     payload = {
         "appId": "appId01",
         "globalId": "786e4c21-70dc-435a-93bb-38",
         "srcSecurityCode": symbol,
     }
     r = requests.post(url, json=payload)
     data_json = r.json()
-    temp_df = pd.DataFrame(data_json["data"])
-    del temp_df["flag"]
-    temp_df.columns = ["时间", "股票代码", "概念名称", "概念代码", "热度"]
+    temp_df = pd.DataFrame(data_json['data'])
+    del temp_df['flag']
+    temp_df.columns = ['时间', '股票代码', '概念名称', '概念代码', '热度']
     return temp_df
 
 
 def stock_hot_rank_latest_em(symbol: str = "SZ000665") -> pd.DataFrame:
     """
     东方财富-个股人气榜-最新排名
     https://guba.eastmoney.com/rank/stock?code=000665
@@ -151,22 +151,22 @@
     :return: 最新排名
     :rtype: pandas.DataFrame
     """
     url = "https://emappdata.eastmoney.com/stockrank/getCurrentLatest"
     payload = {
         "appId": "appId01",
         "globalId": "786e4c21-70dc-435a-93bb-38",
-        "marketType": "",
+        'marketType': "",
         "srcSecurityCode": symbol,
     }
     r = requests.post(url, json=payload)
     data_json = r.json()
-    temp_df = pd.DataFrame.from_dict(data_json["data"], orient="index")
+    temp_df = pd.DataFrame.from_dict(data_json['data'], orient="index")
     temp_df.reset_index(inplace=True)
-    temp_df.columns = ["item", "value"]
+    temp_df.columns = ['item', 'value']
     return temp_df
 
 
 def stock_hot_rank_relate_em(symbol: str = "SZ000665") -> pd.DataFrame:
     """
     东方财富-个股人气榜-相关股票
     https://guba.eastmoney.com/rank/stock?code=000665
@@ -179,32 +179,30 @@
     payload = {
         "appId": "appId01",
         "globalId": "786e4c21-70dc-435a-93bb-38",
         "srcSecurityCode": symbol,
     }
     r = requests.post(url, json=payload)
     data_json = r.json()
-    temp_df = pd.DataFrame.from_dict(data_json["data"])
-    temp_df.columns = ["时间", "-", "股票代码", "-", "相关股票代码", "涨跌幅", "-"]
-    temp_df = temp_df[["时间", "股票代码", "相关股票代码", "涨跌幅"]]
-    temp_df["涨跌幅"] = temp_df["涨跌幅"].str.strip("%")
-    temp_df["涨跌幅"] = pd.to_numeric(temp_df["涨跌幅"])
+    temp_df = pd.DataFrame.from_dict(data_json['data'])
+    temp_df.columns = ['时间', '-', '股票代码', '-', '相关股票代码', '涨跌幅', '-']
+    temp_df = temp_df[['时间', '股票代码', '相关股票代码', '涨跌幅']]
+    temp_df['涨跌幅'] = temp_df['涨跌幅'].str.strip('%')
+    temp_df['涨跌幅'] = pd.to_numeric(temp_df['涨跌幅'])
     return temp_df
 
 
 if __name__ == "__main__":
     stock_hot_rank_em_df = stock_hot_rank_em()
     print(stock_hot_rank_em_df)
 
-    stock_hot_rank_detail_em_df = stock_hot_rank_detail_em(symbol="SZ871245")
+    stock_hot_rank_detail_em_df = stock_hot_rank_detail_em(symbol="SZ000665")
     print(stock_hot_rank_detail_em_df)
 
-    stock_hot_rank_detail_realtime_em_df = stock_hot_rank_detail_realtime_em(
-        symbol="SZ000665"
-    )
+    stock_hot_rank_detail_realtime_em_df = stock_hot_rank_detail_realtime_em(symbol="SZ000665")
     print(stock_hot_rank_detail_realtime_em_df)
 
     stock_hot_keyword_em_df = stock_hot_keyword_em(symbol="SZ000665")
     print(stock_hot_keyword_em_df)
 
     stock_hot_rank_latest_em_df = stock_hot_rank_latest_em(symbol="SZ000665")
     print(stock_hot_rank_latest_em_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_hot_search_baidu.py` & `akshare-1.9.9/akshare/stock/stock_hot_search_baidu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/21 14:19
+Date: 2022/10/14 18:19
 Desc: 百度股市通-热搜股票
 https://gushitong.baidu.com/expressnews
 """
 import pandas as pd
 import requests
-from datetime import datetime
 
 
-def stock_hot_search_baidu(symbol: str = "A股", date: str = "20230428", time: str = "今日"):
+def stock_hot_search_baidu(symbol: str = "A股", date: str = "20221014", time: str = "0"):
     """
     百度股市通-热搜股票
     https://gushitong.baidu.com/expressnews
     :param symbol: choice of {"全部", "A股", "港股", "美股"}
     :type symbol: str
     :param date: 日期
     :type date: str
-    :param time: time="今日"；choice of {"今日", "1小时"}
+    :param time: 默认 time=0，则为当天的排行；如 time="16"，则为 date 的 16 点的热门股票排行
     :type time: str
     :return: 股东人数及持股集中度
     :rtype: pandas.DataFrame
     """
-    hour_str = datetime.now().hour
     symbol_map = {
         "全部": "all",
         "A股": "ab",
         "港股": "hk",
         "美股": "us",
     }
     url = "https://finance.pae.baidu.com/vapi/v1/hotrank"
     params = {
         "tn": "wisexmlnew",
         "dsp": "iphone",
         "product": "stock",
         "day": date,
-        "hour": hour_str,
+        "hour": time,
         "pn": "0",
         "rn": "1000",
         "market": symbol_map[symbol],
-        "type": "day" if time == "今日" else "hour",
+        "type": "day" if time == 0 else "hour",
         "finClientType": "pc",
     }
     r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(
         data_json["Result"]["body"], columns=data_json["Result"]["header"]
     )
-    temp_df["现价"] = pd.to_numeric(temp_df["现价"], errors="coerce")
-    temp_df["排名变化"] = pd.to_numeric(temp_df["排名变化"], errors="coerce")
+    temp_df["综合热度"] = pd.to_numeric(temp_df["综合热度"])
+    temp_df["排名变化"] = pd.to_numeric(temp_df["排名变化"])
+    temp_df["是否连续上榜"] = pd.to_numeric(temp_df["是否连续上榜"])
     return temp_df
 
 
 if __name__ == "__main__":
     stock_hot_search_baidu_df = stock_hot_search_baidu(
-        symbol="A股", date="20230428", time="今日"
+        symbol="A股", date="20221025", time="19"
     )
     print(stock_hot_search_baidu_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_industry.py` & `akshare-1.9.9/akshare/stock/stock_industry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/9 17:06
+Date: 2021/10/30 16:06
 Desc: 新浪行业-板块行情
 http://finance.sina.com.cn/stock/sl/
 """
 import json
 import math
 
 import pandas as pd
@@ -29,26 +29,32 @@
         r = requests.get(url)
     if indicator == "启明星行业":
         url = "http://biz.finance.sina.com.cn/hq/qmxIndustryHq.php"
         r = requests.get(url)
         r.encoding = "gb2312"
     if indicator == "概念":
         url = "http://money.finance.sina.com.cn/q/view/newFLJK.php"
-        params = {"param": "class"}
+        params = {
+            "param": "class"
+        }
         r = requests.get(url, params=params)
     if indicator == "地域":
         url = "http://money.finance.sina.com.cn/q/view/newFLJK.php"
-        params = {"param": "area"}
+        params = {
+            "param": "area"
+        }
         r = requests.get(url, params=params)
     if indicator == "行业":
         url = "http://money.finance.sina.com.cn/q/view/newFLJK.php"
-        params = {"param": "industry"}
+        params = {
+            "param": "industry"
+        }
         r = requests.get(url, params=params)
     text_data = r.text
-    json_data = json.loads(text_data[text_data.find("{") :])
+    json_data = json.loads(text_data[text_data.find("{"):])
     temp_df = pd.DataFrame([value.split(",") for key, value in json_data.items()])
     temp_df.columns = [
         "label",
         "板块",
         "公司家数",
         "平均价格",
         "涨跌额",
@@ -57,77 +63,79 @@
         "总成交额",
         "股票代码",
         "个股-涨跌幅",
         "个股-当前价",
         "个股-涨跌额",
         "股票名称",
     ]
-    temp_df["公司家数"] = pd.to_numeric(temp_df["公司家数"])
-    temp_df["平均价格"] = pd.to_numeric(temp_df["平均价格"])
-    temp_df["涨跌额"] = pd.to_numeric(temp_df["涨跌额"])
-    temp_df["涨跌幅"] = pd.to_numeric(temp_df["涨跌幅"])
-    temp_df["总成交量"] = pd.to_numeric(temp_df["总成交量"])
-    temp_df["总成交额"] = pd.to_numeric(temp_df["总成交额"])
-    temp_df["个股-涨跌幅"] = pd.to_numeric(temp_df["个股-涨跌幅"])
-    temp_df["个股-当前价"] = pd.to_numeric(temp_df["个股-当前价"])
-    temp_df["个股-涨跌额"] = pd.to_numeric(temp_df["个股-涨跌额"])
+    temp_df['公司家数'] = pd.to_numeric(temp_df['公司家数'])
+    temp_df['平均价格'] = pd.to_numeric(temp_df['平均价格'])
+    temp_df['涨跌额'] = pd.to_numeric(temp_df['涨跌额'])
+    temp_df['涨跌幅'] = pd.to_numeric(temp_df['涨跌幅'])
+    temp_df['总成交量'] = pd.to_numeric(temp_df['总成交量'])
+    temp_df['总成交额'] = pd.to_numeric(temp_df['总成交额'])
+    temp_df['个股-涨跌幅'] = pd.to_numeric(temp_df['个股-涨跌幅'])
+    temp_df['个股-当前价'] = pd.to_numeric(temp_df['个股-当前价'])
+    temp_df['个股-涨跌额'] = pd.to_numeric(temp_df['个股-涨跌额'])
     return temp_df
 
 
 def stock_sector_detail(sector: str = "gn_gfgn") -> pd.DataFrame:
     """
     新浪行业-板块行情-成份详情
     http://finance.sina.com.cn/stock/sl/#area_1
     :param sector: stock_sector_spot 返回的 label 值, choice of {"新浪行业", "概念", "地域", "行业"}; "启明星行业" 无详情
     :type sector: str
     :return: 指定 sector 的板块详情
     :rtype: pandas.DataFrame
     """
     url = "http://vip.stock.finance.sina.com.cn/quotes_service/api/json_v2.php/Market_Center.getHQNodeStockCount"
-    params = {"node": sector}
+    params = {
+        "node": sector
+    }
     r = requests.get(url, params=params)
     total_num = int(r.json())
     total_page_num = math.ceil(int(total_num) / 80)
     big_df = pd.DataFrame()
     url = "http://vip.stock.finance.sina.com.cn/quotes_service/api/json_v2.php/Market_Center.getHQNodeData"
-    for page in tqdm(range(1, total_page_num + 1), leave=True):
+    for page in tqdm(range(1, total_page_num+1), leave=True):
         params = {
             "page": str(page),
             "num": "80",
             "sort": "symbol",
             "asc": "1",
             "node": sector,
             "symbol": "",
             "_s_r_a": "page",
         }
         r = requests.get(url, params=params)
         data_text = r.text
         data_json = demjson.decode(data_text)
         temp_df = pd.DataFrame(data_json)
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
-    big_df["trade"] = pd.to_numeric(big_df["trade"], errors="coerce")
-    big_df["pricechange"] = pd.to_numeric(big_df["pricechange"], errors="coerce")
-    big_df["changepercent"] = pd.to_numeric(big_df["changepercent"], errors="coerce")
-    big_df["buy"] = pd.to_numeric(big_df["buy"], errors="coerce")
-    big_df["sell"] = pd.to_numeric(big_df["sell"], errors="coerce")
-    big_df["settlement"] = pd.to_numeric(big_df["settlement"], errors="coerce")
-    big_df["open"] = pd.to_numeric(big_df["open"], errors="coerce")
-    big_df["high"] = pd.to_numeric(big_df["high"], errors="coerce")
-    big_df["low"] = pd.to_numeric(big_df["low"], errors="coerce")
-    big_df["volume"] = pd.to_numeric(big_df["volume"], errors="coerce")
-    big_df["amount"] = pd.to_numeric(big_df["amount"], errors="coerce")
-    big_df["per"] = pd.to_numeric(big_df["per"], errors="coerce")
-    big_df["pb"] = pd.to_numeric(big_df["pb"], errors="coerce")
-    big_df["mktcap"] = pd.to_numeric(big_df["mktcap"], errors="coerce")
-    big_df["nmc"] = pd.to_numeric(big_df["nmc"], errors="coerce")
-    big_df["turnoverratio"] = pd.to_numeric(big_df["turnoverratio"], errors="coerce")
+        big_df = big_df.append(temp_df, ignore_index=True)
+    big_df['trade'] = pd.to_numeric(big_df['trade'])
+    big_df['pricechange'] = pd.to_numeric(big_df['pricechange'])
+    big_df['changepercent'] = pd.to_numeric(big_df['changepercent'])
+    big_df['buy'] = pd.to_numeric(big_df['buy'])
+    big_df['sell'] = pd.to_numeric(big_df['sell'])
+    big_df['settlement'] = pd.to_numeric(big_df['settlement'])
+    big_df['open'] = pd.to_numeric(big_df['open'])
+    big_df['high'] = pd.to_numeric(big_df['high'])
+    big_df['low'] = pd.to_numeric(big_df['low'])
+    big_df['volume'] = pd.to_numeric(big_df['volume'])
+    big_df['amount'] = pd.to_numeric(big_df['amount'])
+    big_df['per'] = pd.to_numeric(big_df['per'])
+    big_df['pb'] = pd.to_numeric(big_df['pb'])
+    big_df['mktcap'] = pd.to_numeric(big_df['mktcap'])
+    big_df['nmc'] = pd.to_numeric(big_df['nmc'])
+    big_df['turnoverratio'] = pd.to_numeric(big_df['turnoverratio'])
     return big_df
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     stock_industry_sina_df = stock_sector_spot(indicator="新浪行业")
     print(stock_industry_sina_df)
 
     stock_industry_con_df = stock_sector_spot(indicator="概念")
     print(stock_industry_con_df)
 
     stock_industry_area_df = stock_sector_spot(indicator="地域")
```

### Comparing `akshare-1.9.80/akshare/stock/stock_industry_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_industry_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_industry_pe_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_industry_pe_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_info.py` & `akshare-1.9.9/akshare/stock/stock_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -441,17 +441,14 @@
 if __name__ == "__main__":
     stock_info_sh_name_code_df = stock_info_sh_name_code(symbol="主板A股")
     print(stock_info_sh_name_code_df)
 
     stock_info_sh_name_code_df = stock_info_sh_name_code(symbol="主板B股")
     print(stock_info_sh_name_code_df)
 
-    stock_info_sh_name_code_df = stock_info_sh_name_code(symbol="科创板")
-    print(stock_info_sh_name_code_df)
-
     stock_info_sz_name_code_df = stock_info_sz_name_code(indicator="A股列表")
     print(stock_info_sz_name_code_df)
 
     stock_info_sz_df = stock_info_sz_name_code(indicator="B股列表")
     print(stock_info_sz_df)
 
     stock_info_sz_df = stock_info_sz_name_code(indicator="AB股列表")
```

### Comparing `akshare-1.9.80/akshare/stock/stock_info_em.py` & `akshare-1.9.9/akshare/stock/stock_info_em.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,9 +58,9 @@
         "value",
     ]
     temp_df.reset_index(inplace=True, drop=True)
     return temp_df
 
 
 if __name__ == "__main__":
-    stock_individual_info_em_df = stock_individual_info_em(symbol="000001")
+    stock_individual_info_em_df = stock_individual_info_em(symbol="603777")
     print(stock_individual_info_em_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_new_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_new_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_profile_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_profile_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_rank_forecast.py` & `akshare-1.9.9/akshare/stock/stock_rank_forecast.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_repurchase_em.py` & `akshare-1.9.9/akshare/stock/stock_repurchase_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_share_changes_cninfo.py` & `akshare-1.9.9/akshare/stock/stock_share_changes_cninfo.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_stop.py` & `akshare-1.9.9/akshare/stock/stock_stop.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_summary.py` & `akshare-1.9.9/akshare/stock/stock_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/3 17:00
+Date: 2023/1/14 17:00
 Desc: 股票数据-总貌-市场总貌
 股票数据-总貌-成交概括
 https://www.szse.cn/market/overview/index.html
 https://www.sse.com.cn/market/stockdata/statistic/
 """
 import warnings
 from io import BytesIO
@@ -76,30 +76,30 @@
     temp_df["基金交易额"] = temp_df["基金交易额"].str.replace(",", "")
     temp_df["基金交易额"] = pd.to_numeric(temp_df["基金交易额"], errors="coerce")
     temp_df["债券交易额"] = temp_df["债券交易额"].str.replace(",", "")
     temp_df["债券交易额"] = pd.to_numeric(temp_df["债券交易额"], errors="coerce")
     return temp_df
 
 
-def stock_szse_sector_summary(symbol: str = "当月", date: str = "202303") -> pd.DataFrame:
+def stock_szse_sector_summary(symbol: str = "当月", date: str = "202203") -> pd.DataFrame:
     """
-    深圳证券交易所-统计资料-股票行业成交数据
+    深圳证券交易所-统计资料-股票行业成交
     https://docs.static.szse.cn/www/market/periodical/month/W020220511355248518608.html
     :param symbol: choice of {"当月", "当年"}
     :type symbol: str
     :param date: 交易年月
     :type date: str
-    :return: 股票行业成交数据
+    :return: 股票行业成交
     :rtype: pandas.DataFrame
     """
     url = "https://www.szse.cn/market/periodical/month/index.html"
     r = requests.get(url)
     r.encoding = "utf8"
     soup = BeautifulSoup(r.text, "lxml")
-    tags_list = soup.find_all("div", attrs={"class": "g-container"})[1].find_all(
+    tags_list = soup.find_all("div", attrs={"class": "g-container"})[4].find_all(
         "script"
     )
     tags_dict = [
         eval(
             item.string[item.string.find("{") : item.string.find("}") + 1]
             .replace("\n", "")
             .replace(" ", "")
@@ -115,16 +115,15 @@
         )
     )
     date_format = "-".join([date[:4], date[4:]])
     url = f"http://www.szse.cn/market/periodical/month/{date_url_dict[date_format]}"
     r = requests.get(url)
     r.encoding = "utf8"
     soup = BeautifulSoup(r.text, "lxml")
-    url = [item for item in soup.find_all("a") if item.get_text() == "股票行业成交数据"][0]["href"]
-
+    url = soup.find("a", text="股票行业成交数据")["href"]
     if symbol == "当月":
         temp_df = pd.read_html(url, encoding="gbk")[0]
         temp_df.columns = [
             "项目名称",
             "项目名称-英文",
             "交易天数",
             "成交金额-人民币元",
@@ -144,21 +143,21 @@
             "成交金额-占总计",
             "成交股数-股数",
             "成交股数-占总计",
             "成交笔数-笔",
             "成交笔数-占总计",
         ]
 
-    temp_df["交易天数"] = pd.to_numeric(temp_df["交易天数"], errors="coerce")
-    temp_df["成交金额-人民币元"] = pd.to_numeric(temp_df["成交金额-人民币元"], errors="coerce")
-    temp_df["成交金额-占总计"] = pd.to_numeric(temp_df["成交金额-占总计"], errors="coerce")
-    temp_df["成交股数-股数"] = pd.to_numeric(temp_df["成交股数-股数"], errors="coerce")
-    temp_df["成交股数-占总计"] = pd.to_numeric(temp_df["成交股数-占总计"], errors="coerce")
-    temp_df["成交笔数-笔"] = pd.to_numeric(temp_df["成交笔数-笔"], errors="coerce")
-    temp_df["成交笔数-占总计"] = pd.to_numeric(temp_df["成交笔数-占总计"], errors="coerce")
+    temp_df["交易天数"] = pd.to_numeric(temp_df["交易天数"])
+    temp_df["成交金额-人民币元"] = pd.to_numeric(temp_df["成交金额-人民币元"])
+    temp_df["成交金额-占总计"] = pd.to_numeric(temp_df["成交金额-占总计"])
+    temp_df["成交股数-股数"] = pd.to_numeric(temp_df["成交股数-股数"])
+    temp_df["成交股数-占总计"] = pd.to_numeric(temp_df["成交股数-占总计"])
+    temp_df["成交笔数-笔"] = pd.to_numeric(temp_df["成交笔数-笔"])
+    temp_df["成交笔数-占总计"] = pd.to_numeric(temp_df["成交笔数-占总计"])
     return temp_df
 
 
 def stock_sse_summary() -> pd.DataFrame:
     """
     上海证券交易所-总貌
     https://www.sse.com.cn/market/stockdata/statistic/
@@ -222,152 +221,78 @@
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36",
         }
         r = requests.get(url, params=params, headers=headers)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["result"])
         temp_df = temp_df.T
         temp_df.reset_index(inplace=True)
-        if len(temp_df.columns) == 6:
-            temp_df.columns = [
+        temp_df.columns = [
+            "单日情况",
+            "主板A",
+            "股票",
+            "主板B",
+            "_",
+            "股票回购",
+            "科创板",
+        ]
+        temp_df = temp_df[
+            [
                 "单日情况",
-                "-",
                 "股票",
-                "主板B",
                 "主板A",
-                "股票回购",
-            ]
-            temp_df = temp_df[
-                [
-                    "单日情况",
-                    "股票",
-                    "主板A",
-                    "主板B",
-                    "股票回购",
-                ]
-            ]
-            temp_df["单日情况"] = [
-                "流通市值",
-                "流通换手率",
-                "平均市盈率",
-                "_",
-                "市价总值",
-                "_",
-                "换手率",
-                "_",
-                "挂牌数",
-                "_",
-                "_",
-                "_",
-                "_",
-                "_",
-                "成交笔数",
-                "成交金额",
-                "成交量",
-                "次新股换手率",
-                "_",
-                "_",
-            ]
-            temp_df = temp_df[temp_df["单日情况"] != "_"]
-            temp_df["单日情况"] = temp_df["单日情况"].astype("category")
-            list_custom_new = [
-                "挂牌数",
-                "市价总值",
-                "流通市值",
-                "成交金额",
-                "成交量",
-                "成交笔数",
-                "平均市盈率",
-                "换手率",
-                "次新股换手率",
-                "流通换手率",
-            ]
-            temp_df["单日情况"].cat.set_categories(list_custom_new)
-            temp_df.sort_values("单日情况", ascending=True, inplace=True)
-            temp_df.reset_index(drop=True, inplace=True)
-            temp_df["股票"] = pd.to_numeric(temp_df["股票"], errors="coerce")
-            temp_df["主板A"] = pd.to_numeric(temp_df["主板A"], errors="coerce")
-            temp_df["主板B"] = pd.to_numeric(temp_df["主板B"], errors="coerce")
-            temp_df["科创板"] = pd.to_numeric("-", errors="coerce")  # 默认位空
-            temp_df["股票回购"] = pd.to_numeric(temp_df["股票回购"], errors="coerce")
-            temp_df = temp_df[
-                [
-                    "单日情况",
-                    "股票",
-                    "主板A",
-                    "主板B",
-                    "科创板",
-                    "股票回购",
-                ]
-            ]
-            return temp_df
-        else:
-            temp_df.columns = [
-                "单日情况",
-                "主板A",
-                "股票",
                 "主板B",
-                "_",
-                "股票回购",
                 "科创板",
+                "股票回购",
             ]
-            temp_df = temp_df[
-                [
-                    "单日情况",
-                    "股票",
-                    "主板A",
-                    "主板B",
-                    "科创板",
-                    "股票回购",
-                ]
-            ]
-            temp_df["单日情况"] = [
-                "流通市值",
-                "流通换手率",
-                "平均市盈率",
-                "_",
-                "市价总值",
-                "_",
-                "换手率",
-                "_",
-                "挂牌数",
-                "_",
-                "_",
-                "_",
-                "_",
-                "_",
-                "成交笔数",
-                "成交金额",
-                "成交量",
-                "次新股换手率",
-                "_",
-                "_",
-            ]
-            temp_df = temp_df[temp_df["单日情况"] != "_"]
-            temp_df["单日情况"] = temp_df["单日情况"].astype("category")
-            list_custom_new = [
-                "挂牌数",
-                "市价总值",
-                "流通市值",
-                "成交金额",
-                "成交量",
-                "成交笔数",
-                "平均市盈率",
-                "换手率",
-                "次新股换手率",
-                "流通换手率",
-            ]
-            temp_df["单日情况"].cat.set_categories(list_custom_new)
-            temp_df.sort_values("单日情况", ascending=True, inplace=True)
-            temp_df.reset_index(drop=True, inplace=True)
-            temp_df["股票"] = pd.to_numeric(temp_df["股票"], errors="coerce")
-            temp_df["主板A"] = pd.to_numeric(temp_df["主板A"], errors="coerce")
-            temp_df["主板B"] = pd.to_numeric(temp_df["主板B"], errors="coerce")
-            temp_df["科创板"] = pd.to_numeric(temp_df["科创板"], errors="coerce")
-            temp_df["股票回购"] = pd.to_numeric(temp_df["股票回购"], errors="coerce")
-            return temp_df
+        ]
+        temp_df["单日情况"] = [
+            "流通市值",
+            "流通换手率",
+            "平均市盈率",
+            "_",
+            "市价总值",
+            "_",
+            "换手率",
+            "_",
+            "挂牌数",
+            "_",
+            "_",
+            "_",
+            "_",
+            "_",
+            "成交笔数",
+            "成交金额",
+            "成交量",
+            "次新股换手率",
+            "_",
+            "_",
+        ]
+        temp_df = temp_df[temp_df["单日情况"] != "_"]
+        temp_df["单日情况"] = temp_df["单日情况"].astype("category")
+        list_custom_new = [
+            "挂牌数",
+            "市价总值",
+            "流通市值",
+            "成交金额",
+            "成交量",
+            "成交笔数",
+            "平均市盈率",
+            "换手率",
+            "次新股换手率",
+            "流通换手率",
+        ]
+        temp_df["单日情况"].cat.set_categories(list_custom_new)
+        temp_df.sort_values("单日情况", ascending=True, inplace=True)
+        temp_df.reset_index(drop=True, inplace=True)
+        temp_df["股票"] = pd.to_numeric(temp_df["股票"], errors="coerce")
+        temp_df["主板A"] = pd.to_numeric(temp_df["主板A"], errors="coerce")
+        temp_df["主板B"] = pd.to_numeric(temp_df["主板B"], errors="coerce")
+        temp_df["科创板"] = pd.to_numeric(temp_df["科创板"], errors="coerce")
+        temp_df["股票回购"] = pd.to_numeric(temp_df["股票回购"], errors="coerce")
+        return temp_df
     elif int(date) <= 20220224:
         url = "http://query.sse.com.cn/commonQuery.do"
         params = {
             "sqlId": "COMMON_SSE_SJ_GPSJ_CJGK_MRGK_C",
             "SEARCH_DATE": "-".join([date[:4], date[4:6], date[6:]]),
             "_": "1640836561673",
         }
@@ -510,27 +435,27 @@
         temp_df["科创板"] = pd.to_numeric(temp_df["科创板"], errors="coerce")
         temp_df["股票"] = pd.to_numeric(temp_df["股票"], errors="coerce")
         temp_df["股票回购"] = pd.to_numeric(temp_df["股票回购"], errors="coerce")
         return temp_df
 
 
 if __name__ == "__main__":
-    stock_szse_summary_df = stock_szse_summary(date="20070511")
+    stock_szse_summary_df = stock_szse_summary(date="20230113")
     print(stock_szse_summary_df)
 
     stock_szse_area_summary_df = stock_szse_area_summary(date="202203")
     print(stock_szse_area_summary_df)
 
-    stock_szse_sector_summary_df = stock_szse_sector_summary(symbol="当月", date="202303")
+    stock_szse_sector_summary_df = stock_szse_sector_summary(symbol="当年", date="202210")
     print(stock_szse_sector_summary_df)
 
     stock_sse_summary_df = stock_sse_summary()
     print(stock_sse_summary_df)
 
     stock_sse_deal_daily_df = stock_sse_deal_daily(date="20211221")
     print(stock_sse_deal_daily_df)
 
     stock_sse_deal_daily_df = stock_sse_deal_daily(date="20211227")
     print(stock_sse_deal_daily_df)
 
-    stock_sse_deal_daily_df = stock_sse_deal_daily(date="20190613")
+    stock_sse_deal_daily_df = stock_sse_deal_daily(date="20221114")
     print(stock_sse_deal_daily_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_us_famous.py` & `akshare-1.9.9/akshare/stock/stock_us_famous.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_us_js.py` & `akshare-1.9.9/akshare/stock/stock_us_js.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_us_pink.py` & `akshare-1.9.9/akshare/stock/stock_us_pink.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_us_sina.py` & `akshare-1.9.9/akshare/stock/stock_us_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_us_zh_hx.py` & `akshare-1.9.9/akshare/stock/stock_us_zh_hx.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_weibo_nlp.py` & `akshare-1.9.9/akshare/stock/stock_weibo_nlp.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_zh_a_sina.py` & `akshare-1.9.9/akshare/stock/stock_zh_a_sina.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,15 +498,15 @@
     )
     print(stock_zh_a_cdr_daily_df)
 
     stock_zh_a_spot_df = stock_zh_a_spot()
     print(stock_zh_a_spot_df)
 
     stock_zh_a_minute_df = stock_zh_a_minute(
-        symbol="sh600751", period="1", adjust="qfq"
+        symbol="sz000001", period="1", adjust=""
     )
     print(stock_zh_a_minute_df)
 
     stock_zh_a_minute_df = stock_zh_a_minute(
         symbol="sh600519", period="1", adjust="hfq"
     )
     print(stock_zh_a_minute_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_zh_a_special.py` & `akshare-1.9.9/akshare/stock/stock_zh_a_special.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_zh_a_tick_tx.py` & `akshare-1.9.9/akshare/stock_feature/stock_wencai.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,117 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/3 22:08
-Desc: 腾讯-股票-实时行情-成交明细
-成交明细-每个交易日 16:00 提供当日数据
-港股报价延时 15 分钟
+Date: 2023/1/11 16:11
+Desc: 问财-热门股票排名
+https://www.iwencai.com/unifiedwap/home/index
 """
-import warnings
-from io import StringIO
-
 import pandas as pd
 import requests
+from py_mini_racer import py_mini_racer
+from tqdm import tqdm
+
+from akshare.datasets import get_ths_js
 
 
-def stock_zh_a_tick_tx_js(symbol: str = "sz000001") -> pd.DataFrame:
+def _get_file_content_ths(file: str = "ths.js") -> str:
     """
-    腾讯财经-历史分笔数据
-    https://gu.qq.com/sz300494/gp/detail
-    :param symbol: 股票代码
-    :type symbol: str
-    :return: 历史分笔数据
-    :rtype: pandas.DataFrame
+    获取 JS 文件的内容
+    :param file:  JS 文件名
+    :type file: str
+    :return: 文件内容
+    :rtype: str
     """
-    big_df = pd.DataFrame()
-    page = 0
-    warnings.warn("正在下载数据，请稍等")
-    while True:
-        try:
-            url = "http://stock.gtimg.cn/data/index.php"
-            params = {
-                "appn": "detail",
-                "action": "data",
-                "c": symbol,
-                "p": page,
-            }
-            r = requests.get(url, params=params)
-            text_data = r.text
-            temp_df = (
-                pd.DataFrame(eval(text_data[text_data.find("[") :])[1].split("|"))
-                .iloc[:, 0]
-                .str.split("/", expand=True)
-            )
-            page += 1
-            big_df = pd.concat([big_df, temp_df], ignore_index=True)
-        except:
-            break
-    if not big_df.empty:
-        big_df = big_df.iloc[:, 1:].copy()
-        big_df.columns = ["成交时间", "成交价格", "价格变动", "成交量", "成交金额", "性质"]
-        big_df.reset_index(drop=True, inplace=True)
-        property_map = {
-            "S": "卖盘",
-            "B": "买盘",
-            "M": "中性盘",
-        }
-        big_df["性质"] = big_df["性质"].map(property_map)
-        big_df = big_df.astype(
-            {
-                "成交时间": str,
-                "成交价格": float,
-                "价格变动": float,
-                "成交量": int,
-                "成交金额": int,
-                "性质": str,
-            }
-        )
-    return big_df
+    setting_file_path = get_ths_js(file)
+    with open(setting_file_path) as f:
+        file_data = f.read()
+    return file_data
 
 
-def stock_zh_a_tick_tx(
-    symbol: str = "sz000001", trade_date: str = "20210316"
-) -> pd.DataFrame:
+def stock_hot_rank_wc(date: str = "20210430") -> pd.DataFrame:
     """
-    https://gu.qq.com/sz000001/gp/detail
-    成交明细-每个交易日 16:00 提供当日数据
-    :param symbol: 带市场标识的股票代码
-    :type symbol: str
-    :param trade_date: 需要提取数据的日期
-    :type trade_date: str
-    :return: 返回当日股票成交明细的数据
+    问财-热门股票排名
+    https://www.iwencai.com/unifiedwap/result?w=%E7%83%AD%E9%97%A85000%E8%82%A1%E7%A5%A8&querytype=stock&issugs&sign=1620126514335
+    :param date: 查询日期
+    :type date: str
+    :return: 热门股票排名
     :rtype: pandas.DataFrame
     """
-    url = "http://stock.gtimg.cn/data/index.php"
+    url = "http://www.iwencai.com/unifiedwap/unified-wap/v2/result/get-robot-data"
+    js_code = py_mini_racer.MiniRacer()
+    js_content = _get_file_content_ths("ths.js")
+    js_code.eval(js_content)
+    v_code = js_code.call("v")
+    headers = {
+        "hexin-v": v_code,
+        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.93 Safari/537.36",
+    }
     params = {
-        "appn": "detail",
-        "action": "download",
-        "c": symbol,
-        "d": trade_date,
+        "question": f"{date}热门5000股票",
+        "perpage": "5000",
+        "page": "1",
+        "secondary_intent": "",
+        "log_info": '{"input_type":"click"}',
+        "source": "Ths_iwencai_Xuangu",
+        "version": "2.0",
+        "query_area": "",
+        "block_list": "",
+        "add_info": '{"urp":{"scene":1,"company":1,"business":1},"contentType":"json"}',
     }
-    r = requests.get(url, params=params)
-    r.encoding = "gbk"
-    temp_df = pd.read_table(StringIO(r.text))
-    return temp_df
-
+    big_df = pd.DataFrame()
+    for page in tqdm(range(1, 11), leave=False):
+        params.update(
+            {
+                "page": page,
+            }
+        )
+        r = requests.post(url, data=params, headers=headers)
+        data_json = r.json()
+        temp_df = pd.DataFrame(
+            data_json["data"]["answer"][0]["txt"][0]["content"]["components"][0][
+                "data"
+            ]["datas"]
+        )
+        big_df = pd.concat([big_df, temp_df], ignore_index=True)
 
-if __name__ == "__main__":
-    stock_zh_a_tick_tx_js_df = stock_zh_a_tick_tx_js(symbol="sz000001")
-    print(stock_zh_a_tick_tx_js_df)
+    big_df.reset_index(inplace=True)
+    big_df["index"] = range(1, len(big_df) + 1)
+    try:
+        rank_date_str = big_df.columns[1].split("[")[1].strip("]")
+    except:
+        try:
+            rank_date_str = big_df.columns[2].split("[")[1].strip("]")
+        except:
+            rank_date_str = date
+    big_df.rename(
+        columns={
+            "index": "序号",
+            f"个股热度排名[{rank_date_str}]": "个股热度排名",
+            f"个股热度[{rank_date_str}]": "个股热度",
+            "code": "股票代码",
+            "market_code": "_",
+            "最新涨跌幅": "涨跌幅",
+            "最新价": "现价",
+            "股票代码": "_",
+        },
+        inplace=True,
+    )
+    big_df = big_df[
+        [
+            "序号",
+            "股票代码",
+            "股票简称",
+            "现价",
+            "涨跌幅",
+            "个股热度",
+            "个股热度排名",
+        ]
+    ]
+    big_df["涨跌幅"] = big_df["涨跌幅"].astype(float).round(2)
+    big_df["排名日期"] = rank_date_str
+    big_df["现价"] = pd.to_numeric(big_df["现价"], errors="coerce")
+    return big_df
 
-    stock_zh_a_tick_tx_df = stock_zh_a_tick_tx(symbol="sz300494", trade_date="20230329")
-    print(stock_zh_a_tick_tx_df)
 
-    date_list = pd.date_range(start="20210601", end="20210613").tolist()
-    date_list = [item.strftime("%Y%m%d") for item in date_list]
-    for item in date_list:
-        print(item)
-        data = stock_zh_a_tick_tx(symbol="sh601699", trade_date=f"{item}")
-        if not data.empty:
-            print(data)
+if __name__ == "__main__":
+    stock_hot_rank_wc_df = stock_hot_rank_wc(date="20230129")
+    print(stock_hot_rank_wc_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_zh_ah_tx.py` & `akshare-1.9.9/akshare/stock/stock_zh_ah_tx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/5 22:10
+Date: 2022/9/28 16:10
 Desc: 腾讯财经-A+H股数据, 实时行情数据和历史行情数据(后复权)
 https://stockapp.finance.qq.com/mstats/#mod=list&id=hk_ah&module=HK&type=AH&sort=3&page=3&max=20
 """
 import random
 
 import requests
 import pandas as pd
@@ -26,17 +26,17 @@
     腾讯财经-港股-AH-总页数
     https://stockapp.finance.qq.com/mstats/#mod=list&id=hk_ah&module=HK&type=AH&sort=3&page=3&max=20
     :return: 总页数
     :rtype: int
     """
     hk_payload_copy = hk_payload.copy()
     hk_payload_copy.update({"reqPage": 1})
-    r = requests.get(hk_url, params=hk_payload_copy, headers=hk_headers)
+    res = requests.get(hk_url, params=hk_payload_copy, headers=hk_headers)
     data_json = demjson.decode(
-        r.text[r.text.find("{"): r.text.rfind("}") + 1]
+        res.text[res.text.find("{") : res.text.rfind("}") + 1]
     )
     page_count = data_json["data"]["page_count"]
     return page_count
 
 
 def stock_zh_ah_spot() -> pd.DataFrame:
     """
@@ -45,17 +45,17 @@
     :return: 腾讯财经-港股-AH-实时行情
     :rtype: pandas.DataFrame
     """
     big_df = pd.DataFrame()
     page_count = _get_zh_stock_ah_page_count() + 1
     for i in tqdm(range(1, page_count), leave=False):
         hk_payload.update({"reqPage": i})
-        r = requests.get(hk_url, params=hk_payload, headers=hk_headers)
+        res = requests.get(hk_url, params=hk_payload, headers=hk_headers)
         data_json = demjson.decode(
-            r.text[r.text.find("{") : r.text.rfind("}") + 1]
+            res.text[res.text.find("{") : res.text.rfind("}") + 1]
         )
         big_df = pd.concat(
             [
                 big_df,
                 pd.DataFrame(data_json["data"]["page_data"])
                 .iloc[:, 0]
                 .str.split("~", expand=True),
@@ -115,17 +115,17 @@
     :return: 股票代码和股票名称的字典
     :rtype: dict
     """
     big_df = pd.DataFrame()
     page_count = _get_zh_stock_ah_page_count() + 1
     for i in tqdm(range(1, page_count), leave=False):
         hk_payload.update({"reqPage": i})
-        r = requests.get(hk_url, params=hk_payload, headers=hk_headers)
+        res = requests.get(hk_url, params=hk_payload, headers=hk_headers)
         data_json = demjson.decode(
-            r.text[r.text.find("{") : r.text.rfind("}") + 1]
+            res.text[res.text.find("{") : res.text.rfind("}") + 1]
         )
         big_df = pd.concat(
             [
                 big_df,
                 pd.DataFrame(data_json["data"]["page_data"])
                 .iloc[:, 0]
                 .str.split("~", expand=True),
@@ -160,15 +160,15 @@
     symbol: str = "02318",
     start_year: str = "2000",
     end_year: str = "2019",
     adjust: str = "",
 ) -> pd.DataFrame:
     """
     腾讯财经-港股-AH-股票历史行情
-    https://gu.qq.com/hk01033/gp
+    http://gu.qq.com/hk01033/gp
     :param symbol: 股票代码
     :type symbol: str
     :param start_year: 开始年份; e.g., “2000”
     :type start_year: str
     :param end_year: 结束年份; e.g., “2019”
     :type end_year: str
     :param adjust: 'qfq': 前复权, 'hfq': 后复权
@@ -202,27 +202,27 @@
                 "Cache-Control": "no-cache",
                 "Connection": "keep-alive",
                 "Host": "web.ifzq.gtimg.cn",
                 "Pragma": "no-cache",
                 "Referer": "http://gu.qq.com/hk01033/gp",
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.125 Safari/537.36",
             }
-            r = requests.get(
+            res = requests.get(
                 "http://web.ifzq.gtimg.cn/appstock/app/kline/kline",
                 params=hk_stock_payload_copy,
                 headers=headers,
             )
         else:
-            r = requests.get(
-                "https://web.ifzq.gtimg.cn/appstock/app/hkfqkline/get",
+            res = requests.get(
+                "http://web.ifzq.gtimg.cn/appstock/app/hkfqkline/get",
                 params=hk_stock_payload_copy,
                 headers=hk_stock_headers,
             )
         data_json = demjson.decode(
-            r.text[r.text.find("{") : r.text.rfind("}") + 1]
+            res.text[res.text.find("{") : res.text.rfind("}") + 1]
         )
         try:
             if adjust == "":
                 temp_df = pd.DataFrame(data_json["data"][f"hk{symbol}"]["day"])
             else:
                 temp_df = pd.DataFrame(
                     data_json["data"][f"hk{symbol}"][f"{adjust}day"]
@@ -262,10 +262,10 @@
     stock_zh_ah_spot_df = stock_zh_ah_spot()
     print(stock_zh_ah_spot_df)
 
     stock_zh_ah_name_df = stock_zh_ah_name()
     print(stock_zh_ah_name_df)
 
     stock_zh_ah_daily_df = stock_zh_ah_daily(
-        symbol="00241", start_year="2000", end_year="2022", adjust="qfq"
+        symbol="02318", start_year="2000", end_year="2022", adjust=""
     )
     print(stock_zh_ah_daily_df)
```

### Comparing `akshare-1.9.80/akshare/stock/stock_zh_b_sina.py` & `akshare-1.9.9/akshare/stock/stock_zh_b_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_zh_kcb_report.py` & `akshare-1.9.9/akshare/stock/stock_zh_kcb_report.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock/stock_zh_kcb_sina.py` & `akshare-1.9.9/akshare/stock/stock_zh_kcb_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_a_below_net_asset_statistics.py` & `akshare-1.9.9/akshare/stock_feature/stock_a_below_net_asset_statistics.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_a_high_low.py` & `akshare-1.9.9/akshare/stock_feature/stock_a_high_low.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_a_indicator.py` & `akshare-1.9.9/akshare/stock_feature/stock_a_indicator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,20 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/6 20:20
+Date: 2022/11/22 1:05
 Desc: 市盈率, 市净率和股息率查询
 https://www.legulegu.com/stocklist
 https://www.legulegu.com/s/000001
 """
-from datetime import datetime
-from hashlib import md5
-
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
-
-
-def get_cookie_csrf(url: str = "") -> dict:
-    """
-    乐咕乐股-主板市盈率
-    https://legulegu.com/stockdata/shanghaiPE
-    :return: 指定市场的市盈率数据
-    :rtype: pandas.DataFrame
-    """
-    r = requests.get(url)
-    soup = BeautifulSoup(r.text, "lxml")
-    csrf_tag = soup.find("meta", attrs={"name": "_csrf"})
-    csrf_token = csrf_tag.attrs["content"]
-    headers = {"X-CSRF-Token": csrf_token}
-    return {"cookies": r.cookies, "headers": headers}
+from hashlib import md5
+from datetime import datetime
 
 
 def get_token_lg() -> str:
     """
     生成乐咕的 token
     https://legulegu.com/s/002488
     :return: token
@@ -39,19 +23,19 @@
     current_date_str = datetime.now().date().isoformat()
     obj = md5()
     obj.update(current_date_str.encode("utf-8"))
     token = obj.hexdigest()
     return token
 
 
-def stock_a_indicator_lg(symbol: str = "002174") -> pd.DataFrame:
+def stock_a_lg_indicator(symbol: str = "000001") -> pd.DataFrame:
     """
     市盈率, 市净率, 股息率数据接口
     https://legulegu.com/stocklist
-    :param symbol: 通过 ak.stock_a_indicator_lg(symbol="all") 来获取所有股票的代码
+    :param symbol: 通过 ak.stock_a_lg_indicator(symbol="all") 来获取所有股票的代码
     :type symbol: str
     :return: 市盈率, 市净率, 股息率查询
     :rtype: pandas.DataFrame
     """
     if symbol == "all":
         url = "https://legulegu.com/stocklist"
         r = requests.get(url)
@@ -65,31 +49,27 @@
         del temp_df["short_url"]
         temp_df = temp_df[["code", "stock_name"]]
         return temp_df
     else:
         url = "https://legulegu.com/api/s/base-info/"
         token = get_token_lg()
         params = {"token": token, "id": symbol}
-        r = requests.post(
-            url,
-            params=params,
-            **get_cookie_csrf(url="https://legulegu.com/"),
-        )
+        r = requests.get(url, params=params)
         temp_json = r.json()
         temp_df = pd.DataFrame(
-            temp_json["data"]["items"],
-            columns=temp_json["data"]["fields"],
+            temp_json["data"]["items"], columns=temp_json["data"]["fields"]
         )
         temp_df["trade_date"] = pd.to_datetime(temp_df["trade_date"]).dt.date
+        # temp_df.iloc[:, 1:] = temp_df.iloc[:, 1:].astype(float)
         temp_df[temp_df.columns[1:]] = temp_df[temp_df.columns[1:]].astype(float)
         temp_df.sort_values(["trade_date"], inplace=True, ignore_index=True)
         return temp_df
 
 
-def stock_hk_indicator_eniu(
+def stock_hk_eniu_indicator(
     symbol: str = "hk01093", indicator: str = "市盈率"
 ) -> pd.DataFrame:
     """
     亿牛网-港股指标
     https://eniu.com/gu/hk01093/roe
     :param symbol: 港股代码
     :type symbol: str
@@ -99,17 +79,15 @@
     :rtype: pandas.DataFrame
     """
     if indicator == "港股":
         url = "https://eniu.com/static/data/stock_list.json"
         r = requests.get(url)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json)
-        temp_df = temp_df[temp_df["stock_id"].str.contains("hk")]
-        temp_df.reset_index(inplace=True, drop=True)
-        return temp_df
+        return temp_df[temp_df["stock_id"].str.contains("hk")]
     if indicator == "市盈率":
         url = f"https://eniu.com/chart/peh/{symbol}"
     elif indicator == "市净率":
         url = f"https://eniu.com/chart/pbh/{symbol}"
     elif indicator == "股息率":
         url = f"https://eniu.com/chart/dvh/{symbol}"
     elif indicator == "ROE":
@@ -119,17 +97,17 @@
     r = requests.get(url)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json)
     return temp_df
 
 
 if __name__ == "__main__":
-    stock_a_indicator_lg_all_df = stock_a_indicator_lg(symbol="all")
-    print(stock_a_indicator_lg_all_df)
+    stock_a_lg_indicator_all_df = stock_a_lg_indicator(symbol="all")
+    print(stock_a_lg_indicator_all_df)
 
-    stock_a_indicator_lg_df = stock_a_indicator_lg(symbol="000001")
-    print(stock_a_indicator_lg_df)
+    stock_a_lg_indicator_df = stock_a_lg_indicator(symbol="831526")
+    print(stock_a_lg_indicator_df)
 
-    stock_hk_indicator_eniu_df = stock_hk_indicator_eniu(
-        symbol="hk01093", indicator="市盈率"
+    stock_hk_eniu_indicator_df = stock_hk_eniu_indicator(
+        symbol="hk01093", indicator="市净率"
     )
-    print(stock_hk_indicator_eniu_df)
+    print(stock_hk_eniu_indicator_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_a_pe_and_pb.py` & `akshare-1.9.9/akshare/stock_feature/stock_a_pe_and_pb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/6 16:24
+Date: 2023/1/30 9:24
 Desc: 乐咕乐股-A 股市盈率和市净率
 https://legulegu.com/stockdata/shanghaiPE
 """
 from datetime import datetime
 
 import pandas as pd
 import requests
 from py_mini_racer import py_mini_racer
 
-from akshare.stock_feature.stock_a_indicator import get_cookie_csrf
-
 hash_code = """
 function e(n) {
     var e, t, r = "", o = -1, f;
     if (n && n.length) {
         f = n.length;
         while ((o += 1) < f) {
             e = n.charCodeAt(o);
@@ -317,15 +315,15 @@
 }
 """
 js_functions = py_mini_racer.MiniRacer()
 js_functions.eval(hash_code)
 token = js_functions.call("hex", datetime.now().date().isoformat()).lower()
 
 
-def stock_market_pe_lg(symbol: str = "深证") -> pd.DataFrame:
+def stock_market_pe_lg(symbol: str = "上证") -> pd.DataFrame:
     """
     乐咕乐股-主板市盈率
     https://legulegu.com/stockdata/shanghaiPE
     :param symbol: choice of {"上证", "深证", "创业板", "科创版"}
     :type symbol: str
     :return: 指定市场的市盈率数据
     :rtype: pandas.DataFrame
@@ -333,21 +331,16 @@
     if symbol in {"上证", "深证", "创业板"}:
         url = "https://legulegu.com/api/stock-data/market-pe"
         symbol_map = {
             "上证": "1",
             "深证": "2",
             "创业板": "4",
         }
-        url_map = {
-            "上证": "https://legulegu.com/stockdata/shanghaiPE",
-            "深证": "https://legulegu.com/stockdata/shenzhenPE",
-            "创业板": "https://legulegu.com/stockdata/cybPE",
-        }
         params = {"token": token, "marketId": symbol_map[symbol]}
-        r = requests.get(url, params=params, **get_cookie_csrf(url=url_map[symbol]))
+        r = requests.get(url, params=params)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["data"])
         temp_df["date"] = (
             pd.to_datetime(temp_df["date"], unit="ms", utc=True)
             .dt.tz_convert("Asia/Shanghai")
             .dt.date
         )
@@ -363,15 +356,15 @@
             "指数",
             "平均市盈率",
         ]
         return temp_df
     else:
         url = "https://legulegu.com/api/stockdata/get-ke-chuang-ban-pe"
         params = {"token": token}
-        r = requests.get(url, params=params, **get_cookie_csrf(url="https://legulegu.com/stockdata/ke-chuang-ban-pe"))
+        r = requests.get(url, params=params)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["data"])
         temp_df["date"] = (
             pd.to_datetime(temp_df["date"], unit="ms", utc=True)
             .dt.tz_convert("Asia/Shanghai")
             .dt.date
         )
@@ -386,15 +379,15 @@
             "日期",
             "总市值",
             "市盈率",
         ]
         return temp_df
 
 
-def stock_index_pe_lg(symbol: str = "沪深300") -> pd.DataFrame:
+def stock_index_pe_lg(symbol: str = "上证50") -> pd.DataFrame:
     """
     乐咕乐股-指数市盈率
     https://legulegu.com/stockdata/sz50-ttm-lyr
     :param symbol: choice of {"上证50", "沪深300", "上证380", "创业板50", "中证500", "上证180", "深证红利", "深证100", "中证1000", "上证红利", "中证100", "中证800"}
     :type symbol: str
     :return: 指定指数的市盈率数据
     :rtype: pandas.DataFrame
@@ -411,15 +404,15 @@
         "中证1000": "000852.SH",
         "上证红利": "000015.SH",
         "中证100": "000903.SH",
         "中证800": "000906.SH",
     }
     url = "https://legulegu.com/api/stockdata/index-basic-pe"
     params = {"token": token, "indexCode": symbol_map[symbol]}
-    r = requests.get(url, params=params, **get_cookie_csrf(url="https://legulegu.com/stockdata/sz50-ttm-lyr"))
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["data"])
     temp_df["date"] = (
         pd.to_datetime(temp_df["date"], unit="ms", utc=True)
         .dt.tz_convert("Asia/Shanghai")
         .dt.date
     )
@@ -455,22 +448,16 @@
     :param symbol: choice of {"上证", "深证", "创业板", "科创版"}
     :type symbol: str
     :return: 指定市场的市净率数据
     :rtype: pandas.DataFrame
     """
     url = "https://legulegu.com/api/stockdata/index-basic-pb"
     symbol_map = {"上证": "1", "深证": "2", "创业板": "4", "科创版": "7"}
-    url_map = {
-        "上证": "https://legulegu.com/stockdata/shanghaiPB",
-        "深证": "https://legulegu.com/stockdata/shenzhenPB",
-        "创业板": "https://legulegu.com/stockdata/cybPB",
-        "科创版": "https://legulegu.com/stockdata/ke-chuang-ban-pb",
-    }
     params = {"token": token, "indexCode": symbol_map[symbol]}
-    r = requests.get(url, params=params, **get_cookie_csrf(url=url_map[symbol]))
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["data"])
     temp_df["date"] = (
         pd.to_datetime(temp_df["date"], unit="ms", utc=True)
         .dt.tz_convert("Asia/Shanghai")
         .dt.date
     )
@@ -514,15 +501,15 @@
         "中证1000": "000852.SH",
         "上证红利": "000015.SH",
         "中证100": "000903.SH",
         "中证800": "000906.SH",
     }
     url = "https://legulegu.com/api/stockdata/index-basic-pb"
     params = {"token": token, "indexCode": symbol_map[symbol]}
-    r = requests.get(url, params=params, **get_cookie_csrf(url="https://legulegu.com/stockdata/zz500-ttm-lyr"))
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["data"])
     temp_df["date"] = (
         pd.to_datetime(temp_df["date"], unit="ms", utc=True)
         .dt.tz_convert("Asia/Shanghai")
         .dt.date
     )
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_account_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_account_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_analyst_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_analyst_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_average_position_lg.py` & `akshare-1.9.9/akshare/stock_feature/stock_average_position_lg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_board_concept_ths.py` & `akshare-1.9.9/akshare/stock_feature/stock_board_concept_ths.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,14 @@
             "振幅(%)": "振幅",
         },
         inplace=True,
         axis=1,
     )
     del big_df["加自选"]
     big_df["代码"] = big_df["代码"].astype(str).str.zfill(6)
-    big_df = big_df[big_df["代码"] != "暂无成份股数据"]
     return big_df
 
 
 def stock_board_concept_info_ths(symbol: str = "阿里巴巴概念") -> pd.DataFrame:
     """
     同花顺-板块-概念板块-板块简介
     http://q.10jqka.com.cn/gn/detail/code/301558/
@@ -380,23 +379,23 @@
 
 
 if __name__ == "__main__":
     stock_board_concept_name_ths_df = stock_board_concept_name_ths()
     print(stock_board_concept_name_ths_df)
 
     stock_board_concept_cons_ths_df = stock_board_concept_cons_ths(
-        symbol="小米概念"
+        symbol="人脸识别"
     )
     print(stock_board_concept_cons_ths_df)
 
     stock_board_concept_info_ths_df = stock_board_concept_info_ths(
         symbol="PVDF概念"
     )
     print(stock_board_concept_info_ths_df)
 
     stock_board_concept_hist_ths_df = stock_board_concept_hist_ths(
         start_year="2022", symbol="阿里巴巴概念"
     )
     print(stock_board_concept_hist_ths_df)
 
-    stock_board_cons_ths_df = stock_board_cons_ths(symbol="881121")
+    stock_board_cons_ths_df = stock_board_cons_ths(symbol="301558")
     print(stock_board_cons_ths_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_board_industry_ths.py` & `akshare-1.9.9/akshare/stock_feature/stock_board_industry_ths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/9 17:20
+Date: 2022/12/2 22:48
 Desc: 同花顺-板块-行业板块
 https://q.10jqka.com.cn/thshy/
 """
 from datetime import datetime
 
 import pandas as pd
 import requests
@@ -528,23 +528,23 @@
             "最低价",
             "收盘价",
             "成交量",
             "成交额",
         ]
     ]
     big_df["日期"] = pd.to_datetime(big_df["日期"]).dt.date
-    big_df.index = pd.to_datetime(big_df["日期"])
-    big_df = big_df[start_date:end_date]
-    big_df.reset_index(drop=True, inplace=True)
-    big_df["开盘价"] = pd.to_numeric(big_df["开盘价"], errors="coerce")
-    big_df["最高价"] = pd.to_numeric(big_df["最高价"], errors="coerce")
-    big_df["最低价"] = pd.to_numeric(big_df["最低价"], errors="coerce")
-    big_df["收盘价"] = pd.to_numeric(big_df["收盘价"], errors="coerce")
-    big_df["成交量"] = pd.to_numeric(big_df["成交量"], errors="coerce")
-    big_df["成交额"] = pd.to_numeric(big_df["成交额"], errors="coerce")
+    condition_one = pd.Timestamp(start_date) < big_df["日期"]
+    condition_two = pd.Timestamp(end_date) > big_df["日期"]
+    big_df = big_df[condition_one & condition_two]
+    big_df["开盘价"] = pd.to_numeric(big_df["开盘价"])
+    big_df["最高价"] = pd.to_numeric(big_df["最高价"])
+    big_df["最低价"] = pd.to_numeric(big_df["最低价"])
+    big_df["收盘价"] = pd.to_numeric(big_df["收盘价"])
+    big_df["成交量"] = pd.to_numeric(big_df["成交量"])
+    big_df["成交额"] = pd.to_numeric(big_df["成交额"])
     return big_df
 
 
 def stock_ipo_benefit_ths() -> pd.DataFrame:
     """
     同花顺-数据中心-新股数据-IPO受益股
     https://data.10jqka.com.cn/ipo/syg/
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_buffett_index_lg.py` & `akshare-1.9.9/akshare/stock_feature/stock_buffett_index_lg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/5 22:05
+Date: 2022/10/15 16:16
 Desc: 乐估乐股-底部研究-巴菲特指标
 https://legulegu.com/stockdata/marketcap-gdp
 """
 import pandas as pd
 import requests
 
-from akshare.stock_feature.stock_a_indicator import get_token_lg, get_cookie_csrf
+from akshare.stock_feature.stock_a_indicator import get_token_lg
 
 
 def stock_buffett_index_lg() -> pd.DataFrame:
     """
     乐估乐股-底部研究-巴菲特指标
     https://legulegu.com/stockdata/marketcap-gdp
     :return: 巴菲特指标
     :rtype: pandas.DataFrame
     """
     token = get_token_lg()
     url = "https://legulegu.com/api/stockdata/marketcap-gdp/get-marketcap-gdp"
     params = {"token": token}
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(url="https://legulegu.com/stockdata/marketcap-gdp")
-    )
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["data"])
     temp_df.rename(
         columns={
             "marketCap": "总市值",
             "gdp": "GDP",
             "close": "收盘价",
@@ -46,18 +42,13 @@
             "总市值",
             "GDP",
             "近十年分位数",
             "总历史分位数",
         ]
     ]
     temp_df["日期"] = pd.to_datetime(temp_df["日期"], unit="ms").dt.date
-    temp_df['收盘价'] = pd.to_numeric(temp_df['收盘价'], errors="coerce")
-    temp_df['总市值'] = pd.to_numeric(temp_df['总市值'], errors="coerce")
-    temp_df['GDP'] = pd.to_numeric(temp_df['GDP'], errors="coerce")
-    temp_df['近十年分位数'] = pd.to_numeric(temp_df['近十年分位数'], errors="coerce")
-    temp_df['总历史分位数'] = pd.to_numeric(temp_df['总历史分位数'], errors="coerce")
     return temp_df
 
 
 if __name__ == "__main__":
     stock_buffett_index_lg_df = stock_buffett_index_lg()
     print(stock_buffett_index_lg_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_classify_sina.py` & `akshare-1.9.9/akshare/stock_feature/stock_classify_sina.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_cls_alerts.py` & `akshare-1.9.9/akshare/stock_feature/stock_cls_alerts.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_cninfo_yjyg.py` & `akshare-1.9.9/akshare/stock_feature/stock_cninfo_yjyg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_comment_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_comment_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_congestion_lg.py` & `akshare-1.9.9/akshare/stock_feature/stock_congestion_lg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/7 15:05
+Date: 2022/12/27 17:05
 Desc: 乐咕乐股-大盘拥挤度
 https://legulegu.com/stockdata/ashares-congestion
 """
 import pandas as pd
 import requests
 
-from akshare.stock_feature.stock_a_indicator import get_token_lg, get_cookie_csrf
+from akshare.stock_feature.stock_a_indicator import get_token_lg
 
 
 def stock_a_congestion_lg() -> pd.DataFrame:
     """
     乐咕乐股-大盘拥挤度
     https://legulegu.com/stockdata/ashares-congestion
     :return: 大盘拥挤度
     :rtype: pandas.DataFrame
     """
     url = "https://legulegu.com/api/stockdata/ashares-congestion"
     token = get_token_lg()
     params = {"token": token}
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(url="https://legulegu.com/stockdata/ashares-congestion")
-    )
+    r = requests.get(url, params=params)
     data_json = r.json()
-    temp_df = pd.DataFrame(data_json["items"])
-    temp_df["date"] = pd.to_datetime(temp_df["date"]).dt.date
-    temp_df = temp_df[
-        [
-            "date",
-            "close",
-            "congestion",
-        ]
-    ]
-    temp_df["close"] = pd.to_numeric(temp_df["close"], errors="coerce")
-    temp_df["congestion"] = pd.to_numeric(temp_df["congestion"], errors="coerce")
+    temp_df = pd.DataFrame(data_json['items'])
+    temp_df['date'] = pd.to_datetime(temp_df['date']).dt.date
+    temp_df = temp_df[[
+        'date',
+        'close',
+        'congestion',
+    ]]
+    temp_df['close'] = pd.to_numeric(temp_df['close'], errors="coerce")
+    temp_df['congestion'] = pd.to_numeric(temp_df['congestion'], errors="coerce")
     return temp_df
 
 
 if __name__ == "__main__":
     stock_a_congestion_lg_df = stock_a_congestion_lg()
     print(stock_a_congestion_lg_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_dxsyl_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_dxsyl_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_ebs_lg.py` & `akshare-1.9.9/akshare/stock_feature/stock_ebs_lg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/5 22:05
+Date: 2022/12/29 16:05
 Desc: 乐咕乐股-股债利差
 https://legulegu.com/stockdata/equity-bond-spread
 """
 import pandas as pd
 import requests
 
-from akshare.stock_feature.stock_a_indicator import get_token_lg, get_cookie_csrf
+from akshare.stock_feature.stock_a_indicator import get_token_lg
 
 
 def stock_ebs_lg() -> pd.DataFrame:
     """
     乐咕乐股-股债利差
     https://legulegu.com/stockdata/equity-bond-spread
     :return: 股债利差
     :rtype: pandas.DataFrame
     """
     url = "https://legulegu.com/api/stockdata/equity-bond-spread"
     token = get_token_lg()
     params = {"token": token, "code": "000300.SH"}
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(url="https://legulegu.com/stockdata/equity-bond-spread")
-    )
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json["data"])
     temp_df["date"] = pd.to_datetime(temp_df["date"]).dt.date
     temp_df.rename(
         columns={
             "date": "日期",
             "close": "沪深300指数",
@@ -42,15 +38,14 @@
         [
             "日期",
             "沪深300指数",
             "股债利差",
             "股债利差均线",
         ]
     ]
-    temp_df['日期'] = pd.to_datetime(temp_df['日期']).dt.date
     temp_df["沪深300指数"] = pd.to_numeric(temp_df["沪深300指数"], errors="coerce")
     temp_df["股债利差"] = pd.to_numeric(temp_df["股债利差"], errors="coerce")
     temp_df["股债利差均线"] = pd.to_numeric(temp_df["股债利差均线"], errors="coerce")
     return temp_df
 
 
 if __name__ == "__main__":
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_fhps_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_gdhs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,237 +1,208 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/7 15:22
-Desc: 东方财富网-数据中心-年报季报-分红送配
-https://data.eastmoney.com/yjfp/
+Date: 2022/11/19 11:20
+Desc: 东方财富网-数据中心-特色数据-股东户数
+https://data.eastmoney.com/gdhs/
 """
 import pandas as pd
 import requests
 from tqdm import tqdm
 
 
-def stock_fhps_em(date: str = "20210630") -> pd.DataFrame:
+def stock_zh_a_gdhs(symbol: str = "20210930") -> pd.DataFrame:
     """
-    东方财富网-数据中心-年报季报-分红送配
-    https://data.eastmoney.com/yjfp/
-    :param date: 分红送配报告期
-    :type date: str
-    :return: 分红送配
+    东方财富网-数据中心-特色数据-股东户数
+    https://data.eastmoney.com/gdhs/
+    :param symbol: choice of {"最新", "每个季度末"}
+    :type symbol: str
+    :return: 股东户数
     :rtype: pandas.DataFrame
     """
     url = "https://datacenter-web.eastmoney.com/api/data/v1/get"
-    params = {
-        "sortColumns": "PLAN_NOTICE_DATE",
-        "sortTypes": "-1",
-        "pageSize": "500",
-        "pageNumber": "1",
-        "reportName": "RPT_SHAREBONUS_DET",
-        "columns": "ALL",
-        "quoteColumns": "",
-        "js": '{"data":(x),"pages":(tp)}',
-        "source": "WEB",
-        "client": "WEB",
-        "filter": f"""(REPORT_DATE='{"-".join([date[:4], date[4:6], date[6:]])}')""",
-    }
-
+    if symbol == "最新":
+        params = {
+            "sortColumns": "HOLD_NOTICE_DATE,SECURITY_CODE",
+            "sortTypes": "-1,-1",
+            "pageSize": "500",
+            "pageNumber": "1",
+            "reportName": "RPT_HOLDERNUMLATEST",
+            "columns": "SECURITY_CODE,SECURITY_NAME_ABBR,END_DATE,INTERVAL_CHRATE,AVG_MARKET_CAP,AVG_HOLD_NUM,TOTAL_MARKET_CAP,TOTAL_A_SHARES,HOLD_NOTICE_DATE,HOLDER_NUM,PRE_HOLDER_NUM,HOLDER_NUM_CHANGE,HOLDER_NUM_RATIO,END_DATE,PRE_END_DATE",
+            "quoteColumns": "f2,f3",
+            "source": "WEB",
+            "client": "WEB",
+        }
+    else:
+        params = {
+            "sortColumns": "HOLD_NOTICE_DATE,SECURITY_CODE",
+            "sortTypes": "-1,-1",
+            "pageSize": "500",
+            "pageNumber": "1",
+            "reportName": "RPT_HOLDERNUM_DET",
+            "columns": "SECURITY_CODE,SECURITY_NAME_ABBR,END_DATE,INTERVAL_CHRATE,AVG_MARKET_CAP,AVG_HOLD_NUM,TOTAL_MARKET_CAP,TOTAL_A_SHARES,HOLD_NOTICE_DATE,HOLDER_NUM,PRE_HOLDER_NUM,HOLDER_NUM_CHANGE,HOLDER_NUM_RATIO,END_DATE,PRE_END_DATE",
+            "quoteColumns": "f2,f3",
+            "source": "WEB",
+            "client": "WEB",
+            'filter': f"(END_DATE='{symbol[:4] + '-' +  symbol[4:6] + '-' +  symbol[6:]}')",
+        }
     r = requests.get(url, params=params)
     data_json = r.json()
-    total_pages = int(data_json["result"]["pages"])
+    total_page_num = data_json["result"]["pages"]
     big_df = pd.DataFrame()
-    for page in tqdm(range(1, total_pages + 1), leave=False):
-        params.update({"pageNumber": page})
+    for page_num in tqdm(range(1, total_page_num + 1), leave=False):
+        params.update({
+            "pageNumber": page_num,
+        })
         r = requests.get(url, params=params)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["result"]["data"])
         big_df = pd.concat([big_df, temp_df], ignore_index=True)
-
     big_df.columns = [
-        "_",
-        "名称",
-        "_",
-        "_",
         "代码",
-        "送转股份-送转总比例",
-        "送转股份-送转比例",
-        "送转股份-转股比例",
-        "现金分红-现金分红比例",
-        "预案公告日",
-        "股权登记日",
-        "除权除息日",
-        "_",
-        "方案进度",
-        "_",
-        "最新公告日期",
-        "_",
-        "_",
-        "_",
-        "每股收益",
-        "每股净资产",
-        "每股公积金",
-        "每股未分配利润",
-        "净利润同比增长",
+        "名称",
+        "股东户数统计截止日-本次",
+        "区间涨跌幅",
+        "户均持股市值",
+        "户均持股数量",
+        "总市值",
         "总股本",
-        "_",
-        "现金分红-股息率",
-        "-",
-        "-",
-        "-",
+        "公告日期",
+        "股东户数-本次",
+        "股东户数-上次",
+        "股东户数-增减",
+        "股东户数-增减比例",
+        "股东户数统计截止日-上次",
+        "最新价",
+        "涨跌幅",
     ]
     big_df = big_df[
         [
             "代码",
             "名称",
-            "送转股份-送转总比例",
-            "送转股份-送转比例",
-            "送转股份-转股比例",
-            "现金分红-现金分红比例",
-            "现金分红-股息率",
-            "每股收益",
-            "每股净资产",
-            "每股公积金",
-            "每股未分配利润",
-            "净利润同比增长",
+            "最新价",
+            "涨跌幅",
+            "股东户数-本次",
+            "股东户数-上次",
+            "股东户数-增减",
+            "股东户数-增减比例",
+            "区间涨跌幅",
+            "股东户数统计截止日-本次",
+            "股东户数统计截止日-上次",
+            "户均持股市值",
+            "户均持股数量",
+            "总市值",
             "总股本",
-            "预案公告日",
-            "股权登记日",
-            "除权除息日",
-            "方案进度",
-            "最新公告日期",
+            "公告日期",
         ]
     ]
-    big_df["送转股份-送转总比例"] = pd.to_numeric(big_df["送转股份-送转总比例"])
-    big_df["送转股份-送转比例"] = pd.to_numeric(big_df["送转股份-送转比例"])
-    big_df["送转股份-转股比例"] = pd.to_numeric(big_df["送转股份-转股比例"])
-    big_df["现金分红-现金分红比例"] = pd.to_numeric(big_df["现金分红-现金分红比例"])
-    big_df["现金分红-股息率"] = pd.to_numeric(big_df["现金分红-股息率"])
-    big_df["每股收益"] = pd.to_numeric(big_df["每股收益"])
-    big_df["每股净资产"] = pd.to_numeric(big_df["每股净资产"])
-    big_df["每股公积金"] = pd.to_numeric(big_df["每股公积金"])
-    big_df["每股未分配利润"] = pd.to_numeric(big_df["每股未分配利润"])
-    big_df["净利润同比增长"] = pd.to_numeric(big_df["净利润同比增长"])
-    big_df["总股本"] = pd.to_numeric(big_df["总股本"])
-
-    big_df["预案公告日"] = pd.to_datetime(big_df["预案公告日"], errors="coerce").dt.date
-    big_df["股权登记日"] = pd.to_datetime(big_df["股权登记日"], errors="coerce").dt.date
-    big_df["除权除息日"] = pd.to_datetime(big_df["除权除息日"], errors="coerce").dt.date
-    big_df["最新公告日期"] = pd.to_datetime(big_df["最新公告日期"], errors="coerce").dt.date
+    big_df['最新价'] = pd.to_numeric(big_df['最新价'], errors="coerce")
+    big_df['涨跌幅'] = pd.to_numeric(big_df['涨跌幅'], errors="coerce")
+    big_df['股东户数-本次'] = pd.to_numeric(big_df['股东户数-本次'], errors="coerce")
+    big_df['股东户数-上次'] = pd.to_numeric(big_df['股东户数-上次'], errors="coerce")
+    big_df['股东户数-增减'] = pd.to_numeric(big_df['股东户数-增减'], errors="coerce")
+    big_df['股东户数-增减比例'] = pd.to_numeric(big_df['股东户数-增减比例'], errors="coerce")
+    big_df['区间涨跌幅'] = pd.to_numeric(big_df['区间涨跌幅'], errors="coerce")
+    big_df['股东户数统计截止日-本次'] = pd.to_datetime(big_df['股东户数统计截止日-本次']).dt.date
+    big_df['股东户数统计截止日-上次'] = pd.to_datetime(big_df['股东户数统计截止日-上次']).dt.date
+    big_df['户均持股市值'] = pd.to_numeric(big_df['户均持股市值'])
+    big_df['户均持股数量'] = pd.to_numeric(big_df['户均持股数量'])
+    big_df['总市值'] = pd.to_numeric(big_df['总市值'])
+    big_df['总股本'] = pd.to_numeric(big_df['总股本'])
+    big_df['公告日期'] = pd.to_datetime(big_df['公告日期']).dt.date
     return big_df
 
 
-def stock_fhps_detail_em(symbol: str = "300073") -> pd.DataFrame:
+def stock_zh_a_gdhs_detail_em(symbol: str = "000002") -> pd.DataFrame:
     """
-    东方财富网-数据中心-分红送配-分红送配详情
-    https://data.eastmoney.com/yjfp/detail/300073.html
+    东方财富网-数据中心-特色数据-股东户数详情
+    https://data.eastmoney.com/gdhs/detail/000002.html
     :param symbol: 股票代码
     :type symbol: str
-    :return: 分红送配详情
+    :return: 股东户数
     :rtype: pandas.DataFrame
     """
     url = "https://datacenter-web.eastmoney.com/api/data/v1/get"
     params = {
-        "sortColumns": "REPORT_DATE",
-        "sortTypes": "-1",
-        "pageSize": "500",
-        "pageNumber": "1",
-        "reportName": "RPT_SHAREBONUS_DET",
-        "columns": "ALL",
-        "quoteColumns": "",
-        "js": '{"data":(x),"pages":(tp)}',
-        "source": "WEB",
-        "client": "WEB",
-        "filter": f"""(SECURITY_CODE="{symbol}")""",
+        'sortColumns': 'END_DATE',
+        'sortTypes': '-1',
+        'pageSize': '500',
+        'pageNumber': '1',
+        'reportName': 'RPT_HOLDERNUM_DET',
+        'columns': 'SECURITY_CODE,SECURITY_NAME_ABBR,CHANGE_SHARES,CHANGE_REASON,END_DATE,INTERVAL_CHRATE,AVG_MARKET_CAP,AVG_HOLD_NUM,TOTAL_MARKET_CAP,TOTAL_A_SHARES,HOLD_NOTICE_DATE,HOLDER_NUM,PRE_HOLDER_NUM,HOLDER_NUM_CHANGE,HOLDER_NUM_RATIO,END_DATE,PRE_END_DATE',
+        'quoteColumns': 'f2,f3',
+        'filter': f'(SECURITY_CODE="{symbol}")',
+        'source': 'WEB',
+        'client': 'WEB',
     }
-
     r = requests.get(url, params=params)
     data_json = r.json()
-    total_pages = int(data_json["result"]["pages"])
+    total_page_num = data_json["result"]["pages"]
     big_df = pd.DataFrame()
-    for page in tqdm(range(1, total_pages + 1), leave=False):
-        params.update({"pageNumber": page})
+    for page_num in tqdm(range(1, total_page_num + 1), leave=False):
+        params.update({
+            "pageNumber": page_num,
+        })
         r = requests.get(url, params=params)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["result"]["data"])
         big_df = pd.concat([big_df, temp_df], ignore_index=True)
-
     big_df.columns = [
-        "_",
-        "-",
-        "_",
-        "_",
-        "-",
-        "送转股份-送转总比例",
-        "送转股份-送股比例",
-        "送转股份-转股比例",
-        "现金分红-现金分红比例",
-        "业绩披露日期",
-        "股权登记日",
-        "除权除息日",
-        "报告期",
-        "方案进度",
-        "现金分红-现金分红比例描述",
-        "最新公告日期",
-        "-",
-        "-",
-        "-",
-        "每股收益",
-        "每股净资产",
-        "每股公积金",
-        "每股未分配利润",
-        "净利润同比增长",
+        "代码",
+        "名称",
+        "股本变动",
+        "股本变动原因",
+        "股东户数统计截止日",
+        "区间涨跌幅",
+        "户均持股市值",
+        "户均持股数量",
+        "总市值",
         "总股本",
-        "预案公告日",
-        "现金分红-股息率",
+        "股东户数公告日期",
+        "股东户数-本次",
+        "股东户数-上次",
+        "股东户数-增减",
+        "股东户数-增减比例",
         "-",
         "-",
         "-",
     ]
     big_df = big_df[
         [
-            "报告期",
-            "业绩披露日期",
-            "送转股份-送转总比例",
-            "送转股份-送股比例",
-            "送转股份-转股比例",
-            "现金分红-现金分红比例",
-            "现金分红-现金分红比例描述",
-            "现金分红-股息率",
-            "每股收益",
-            "每股净资产",
-            "每股公积金",
-            "每股未分配利润",
-            "净利润同比增长",
+            "股东户数统计截止日",
+            "区间涨跌幅",
+            "股东户数-本次",
+            "股东户数-上次",
+            "股东户数-增减",
+            "股东户数-增减比例",
+            "户均持股市值",
+            "户均持股数量",
+            "总市值",
             "总股本",
-            "预案公告日",
-            "股权登记日",
-            "除权除息日",
-            "方案进度",
-            "最新公告日期",
+            "股本变动",
+            "股本变动原因",
+            "股东户数公告日期",
+            "代码",
+            "名称",
         ]
     ]
-    big_df["报告期"] = pd.to_datetime(big_df["报告期"], errors="coerce").dt.date
-    big_df["业绩披露日期"] = pd.to_datetime(big_df["业绩披露日期"], errors="coerce").dt.date
-    big_df["预案公告日"] = pd.to_datetime(big_df["预案公告日"], errors="coerce").dt.date
-    big_df["股权登记日"] = pd.to_datetime(big_df["股权登记日"], errors="coerce").dt.date
-    big_df["除权除息日"] = pd.to_datetime(big_df["除权除息日"], errors="coerce").dt.date
-    big_df["最新公告日期"] = pd.to_datetime(big_df["最新公告日期"], errors="coerce").dt.date
-
-    big_df["送转股份-送转总比例"] = pd.to_numeric(big_df["送转股份-送转总比例"], errors="coerce")
-    big_df["送转股份-送股比例"] = pd.to_numeric(big_df["送转股份-送股比例"], errors="coerce")
-    big_df["送转股份-转股比例"] = pd.to_numeric(big_df["送转股份-转股比例"], errors="coerce")
-    big_df["现金分红-现金分红比例"] = pd.to_numeric(big_df["现金分红-现金分红比例"], errors="coerce")
-    big_df["现金分红-股息率"] = pd.to_numeric(big_df["现金分红-股息率"], errors="coerce")
-    big_df["每股收益"] = pd.to_numeric(big_df["每股收益"], errors="coerce")
-    big_df["每股净资产"] = pd.to_numeric(big_df["每股净资产"], errors="coerce")
-    big_df["每股公积金"] = pd.to_numeric(big_df["每股公积金"], errors="coerce")
-    big_df["每股未分配利润"] = pd.to_numeric(big_df["每股未分配利润"], errors="coerce")
-    big_df["净利润同比增长"] = pd.to_numeric(big_df["净利润同比增长"], errors="coerce")
-    big_df["总股本"] = pd.to_numeric(big_df["总股本"], errors="coerce")
+    big_df['区间涨跌幅'] = pd.to_numeric(big_df['区间涨跌幅'], errors="coerce")
+    big_df['股东户数-本次'] = pd.to_numeric(big_df['股东户数-本次'], errors="coerce")
+    big_df['股东户数-上次'] = pd.to_numeric(big_df['股东户数-上次'], errors="coerce")
+    big_df['股东户数-增减'] = pd.to_numeric(big_df['股东户数-增减'], errors="coerce")
+    big_df['股东户数-增减比例'] = pd.to_numeric(big_df['股东户数-增减比例'], errors="coerce")
+    big_df['户均持股市值'] = pd.to_numeric(big_df['户均持股市值'])
+    big_df['户均持股数量'] = pd.to_numeric(big_df['户均持股数量'])
+    big_df['总市值'] = pd.to_numeric(big_df['总市值'])
+    big_df['总股本'] = pd.to_numeric(big_df['总股本'])
+    big_df['股本变动'] = pd.to_numeric(big_df['股本变动'])
+    big_df['股东户数统计截止日'] = pd.to_datetime(big_df['股东户数统计截止日']).dt.date
+    big_df['股东户数公告日期'] = pd.to_datetime(big_df['股东户数公告日期']).dt.date
     return big_df
 
 
 if __name__ == "__main__":
-    stock_fhps_em_df = stock_fhps_em(date="20221231")
-    print(stock_fhps_em_df)
+    stock_zh_a_gdhs_df = stock_zh_a_gdhs(symbol='20210930')
+    print(stock_zh_a_gdhs_df)
 
-    stock_fhps_detail_em_df = stock_fhps_detail_em(symbol="300073")
-    print(stock_fhps_detail_em_df)
+    stock_zh_a_gdhs_detail_em_df = stock_zh_a_gdhs_detail_em(symbol="000002")
+    print(stock_zh_a_gdhs_detail_em_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_fund_flow.py` & `akshare-1.9.9/akshare/stock_feature/stock_fund_flow.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_gdfx_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_gdfx_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_gdzjc_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_gdzjc_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_gpzy_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_gpzy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_gxl_lg.py` & `akshare-1.9.9/akshare/stock_feature/stock_gxl_lg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/10 16:05
+Date: 2022/12/23 16:05
 Desc: 乐咕乐股-股息率-A 股股息率
 https://legulegu.com/stockdata/guxilv
 """
 import pandas as pd
 import requests
 
-from akshare.stock_feature.stock_a_indicator import get_token_lg, get_cookie_csrf
+from akshare.stock_feature.stock_a_indicator import get_token_lg
 
 
 def stock_a_gxl_lg(symbol: str = "上证A股") -> pd.DataFrame:
     """
     乐咕乐股-股息率-A 股股息率
     https://legulegu.com/stockdata/guxilv
     :param symbol: choice of {"上证A股", "深证A股", "创业板", "科创板"}
@@ -25,63 +25,47 @@
         "深证A股": "shenzheng",
         "创业板": "chuangyeban",
         "科创板": "kechuangban",
     }
     url = "https://legulegu.com/api/stockdata/guxilv"
     token = get_token_lg()
     params = {"token": token}
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(url="https://legulegu.com/stockdata/guxilv")
-    )
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json[symbol_map[symbol]])
-    temp_df["date"] = (
-        pd.to_datetime(temp_df["date"], unit="ms") + pd.Timedelta(hours=8)
-    ).dt.date
+    temp_df['date'] = (pd.to_datetime(temp_df['date'], unit="ms") + pd.Timedelta(hours=8)).dt.date
     temp_df.rename(columns={"addDvTtm": "股息率", "date": "日期"}, inplace=True)
-    temp_df = temp_df[
-        [
-            "日期",
-            "股息率",
-        ]
-    ]
-    temp_df["股息率"] = pd.to_numeric(temp_df["股息率"], errors="coerce")
+    temp_df = temp_df[[
+        '日期',
+        '股息率',
+    ]]
+    temp_df['股息率'] = pd.to_numeric(temp_df['股息率'], errors="coerce")
     return temp_df
 
 
 def stock_hk_gxl_lg() -> pd.DataFrame:
     """
     乐咕乐股-股息率-恒生指数股息率
     https://legulegu.com/stockdata/market/hk/dv/hsi
     :return: 恒生指数股息率
     :rtype: pandas.DataFrame
     """
     url = "https://legulegu.com/api/stockdata/hs"
     token = get_token_lg()
     params = {"token": token, "indexCode": "HSI"}
-    r = requests.get(
-        url,
-        params=params,
-        **get_cookie_csrf(url="https://legulegu.com/stockdata/market/hk/dv/hsi")
-    )
+    r = requests.get(url, params=params)
     data_json = r.json()
     temp_df = pd.DataFrame(data_json)
-    temp_df["date"] = (
-        pd.to_datetime(temp_df["date"], unit="ms") + pd.Timedelta(hours=8)
-    ).dt.date
+    temp_df['date'] = (pd.to_datetime(temp_df['date'], unit="ms") + pd.Timedelta(hours=8)).dt.date
     temp_df.rename(columns={"addDvRatio": "股息率", "date": "日期"}, inplace=True)
-    temp_df = temp_df[
-        [
-            "日期",
-            "股息率",
-        ]
-    ]
-    temp_df["股息率"] = pd.to_numeric(temp_df["股息率"], errors="coerce")
+    temp_df = temp_df[[
+        '日期',
+        '股息率',
+    ]]
+    temp_df['股息率'] = pd.to_numeric(temp_df['股息率'], errors="coerce")
     return temp_df
 
 
 if __name__ == "__main__":
     stock_a_gxl_lg_df = stock_a_gxl_lg(symbol="上证A股")
     print(stock_a_gxl_lg_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_hist_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_hist_em.py`

 * *Files 0% similar despite different names*

```diff
@@ -1251,15 +1251,15 @@
     temp_df["时间"] = pd.to_datetime(temp_df["时间"]).astype(str)
     return temp_df
 
 
 def stock_hk_spot_em() -> pd.DataFrame:
     """
     东方财富网-港股-实时行情
-    https://quote.eastmoney.com/center/gridlist.html#hk_stocks
+    http://quote.eastmoney.com/center/gridlist.html#hk_stocks
     :return: 港股-实时行情
     :rtype: pandas.DataFrame
     """
     url = "http://72.push2.eastmoney.com/api/qt/clist/get"
     params = {
         "pn": "1",
         "pz": "50000",
@@ -1337,103 +1337,14 @@
     temp_df["最低"] = pd.to_numeric(temp_df["最低"], errors="coerce")
     temp_df["昨收"] = pd.to_numeric(temp_df["昨收"], errors="coerce")
     temp_df["成交量"] = pd.to_numeric(temp_df["成交量"], errors="coerce")
     temp_df["成交额"] = pd.to_numeric(temp_df["成交额"], errors="coerce")
     return temp_df
 
 
-def stock_hk_main_board_spot_em() -> pd.DataFrame:
-    """
-    东方财富网-港股-主板-实时行情
-    https://quote.eastmoney.com/center/gridlist.html#hk_mainboard
-    :return: 港股-主板-实时行情
-    :rtype: pandas.DataFrame
-    """
-    url = "http://81.push2.eastmoney.com/api/qt/clist/get"
-    params = {
-        "pn": "1",
-        "pz": "50000",
-        "po": "1",
-        "np": "1",
-        "ut": "bd1d9ddb04089700cf9c27f6f7426281",
-        "fltt": "2",
-        "invt": "2",
-        "fid": "f3",
-        "fs": "m:128 t:3",
-        "fields": "f1,f2,f3,f4,f5,f6,f7,f8,f9,f10,f12,f13,f14,f15,f16,f17,f18,f20,f21,f23,f24,f25,f22,f11,f62,f128,f136,f115,f152",
-        "_": "1624010056945",
-    }
-    r = requests.get(url, params=params)
-    data_json = r.json()
-    temp_df = pd.DataFrame(data_json["data"]["diff"])
-    temp_df.columns = [
-        "_",
-        "最新价",
-        "涨跌幅",
-        "涨跌额",
-        "成交量",
-        "成交额",
-        "振幅",
-        "换手率",
-        "市盈率-动态",
-        "量比",
-        "_",
-        "代码",
-        "_",
-        "名称",
-        "最高",
-        "最低",
-        "今开",
-        "昨收",
-        "_",
-        "_",
-        "_",
-        "市净率",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-        "_",
-    ]
-    temp_df.reset_index(inplace=True)
-    temp_df["index"] = temp_df.index + 1
-    temp_df.rename(columns={"index": "序号"}, inplace=True)
-    temp_df = temp_df[
-        [
-            "序号",
-            "代码",
-            "名称",
-            "最新价",
-            "涨跌额",
-            "涨跌幅",
-            "今开",
-            "最高",
-            "最低",
-            "昨收",
-            "成交量",
-            "成交额",
-        ]
-    ]
-    temp_df["序号"] = pd.to_numeric(temp_df["序号"])
-    temp_df["最新价"] = pd.to_numeric(temp_df["最新价"], errors="coerce")
-    temp_df["涨跌额"] = pd.to_numeric(temp_df["涨跌额"], errors="coerce")
-    temp_df["涨跌幅"] = pd.to_numeric(temp_df["涨跌幅"], errors="coerce")
-    temp_df["今开"] = pd.to_numeric(temp_df["今开"], errors="coerce")
-    temp_df["最高"] = pd.to_numeric(temp_df["最高"], errors="coerce")
-    temp_df["最低"] = pd.to_numeric(temp_df["最低"], errors="coerce")
-    temp_df["昨收"] = pd.to_numeric(temp_df["昨收"], errors="coerce")
-    temp_df["成交量"] = pd.to_numeric(temp_df["成交量"], errors="coerce")
-    temp_df["成交额"] = pd.to_numeric(temp_df["成交额"], errors="coerce")
-    return temp_df
-
-
 def stock_hk_hist(
     symbol: str = "40224",
     period: str = "daily",
     start_date: str = "19700101",
     end_date: str = "22220101",
     adjust: str = "",
 ) -> pd.DataFrame:
@@ -1892,17 +1803,14 @@
 
     code_id_map_em_df = code_id_map_em()
     print(code_id_map_em_df)
 
     stock_hk_spot_em_df = stock_hk_spot_em()
     print(stock_hk_spot_em_df)
 
-    stock_hk_main_board_spot_em_df = stock_hk_main_board_spot_em()
-    print(stock_hk_main_board_spot_em_df)
-
     stock_zh_a_hist_df = stock_zh_a_hist(
         symbol="430090",
         period="daily",
         start_date="20220516",
         end_date="20220722",
         adjust="hfq",
     )
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_hk_valuation_baidu.py` & `akshare-1.9.9/akshare/stock_feature/stock_hk_valuation_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_hot_tgb.py` & `akshare-1.9.9/akshare/stock_feature/stock_hot_tgb.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_hot_xq.py` & `akshare-1.9.9/akshare/stock_feature/stock_hot_xq.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_hsgt_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_hsgt_em.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 # !/usr/bin/env python
 """
-Date: 2023/3/10 16:32
+Date: 2022/11/27 20:32
 Desc: 东方财富网-数据中心-沪深港通持股
 https://data.eastmoney.com/hsgtcg/
 沪深港通详情: https://finance.eastmoney.com/news/1622,20161118685370149.html
 """
 import json
 
 import pandas as pd
@@ -1397,15 +1397,15 @@
 
 
 def stock_hsgt_board_rank_em(
     symbol: str = "北向资金增持行业板块排行", indicator: str = "今日"
 ) -> pd.DataFrame:
     """
     东方财富网-数据中心-沪深港通持股-行业板块排行-北向资金增持行业板块排行
-    https://data.eastmoney.com/hsgtcg/hy.html
+    http://data.eastmoney.com/hsgtcg/hy.html
     :param symbol: choice of {"北向资金增持行业板块排行", "北向资金增持概念板块排行", "北向资金增持地域板块排行"}
     :type symbol: str
     :param indicator: choice of {"今日", "3日", "5日", "10日", "1月", "1季", "1年"}
     :type indicator: str
     :return: 北向资金增持行业板块排行
     :rtype: pandas.DataFrame
     """
@@ -1519,15 +1519,15 @@
     temp_df["报告时间"] = pd.to_datetime(temp_df["报告时间"]).dt.date
     return temp_df
 
 
 def stock_hsgt_individual_em(stock: str = "002008") -> pd.DataFrame:
     """
     东方财富-数据中心-沪深港通-沪深港通持股-具体股票
-    https://data.eastmoney.com/hsgtcg/StockHdStatistics/002008.html
+    http://data.eastmoney.com/hsgtcg/StockHdStatistics/002008.html
     :param stock: 股票代码
     :type stock: str
     :return: 具体股票-沪深港通持股
     :rtype: pandas.DataFrame
     """
     url = "http://datacenter-web.eastmoney.com/api/data/v1/get"
     params = {
@@ -1594,15 +1594,15 @@
 def stock_hsgt_individual_detail_em(
     symbol: str = "002008",
     start_date: str = "20220130",
     end_date: str = "20220330",
 ) -> pd.DataFrame:
     """
     东方财富-数据中心-沪深港通-沪深港通持股-具体股票详情
-    https://data.eastmoney.com/hsgtcg/StockHdStatistics/002008.html
+    http://data.eastmoney.com/hsgtcg/StockHdStatistics/002008.html
     :param symbol: 股票代码
     :type symbol: str
     :param start_date: 开始时间
     :type start_date: str
     :param end_date: 结束时间
     :type end_date: str
     :return: 沪深港通持股-具体股票详情
@@ -1748,15 +1748,15 @@
 
     stock_hsgt_hold_stock_em_df = stock_hsgt_hold_stock_em(
         market="沪股通", indicator="10日排行"
     )
     print(stock_hsgt_hold_stock_em_df)
 
     stock_hsgt_stock_statistics_em_df = stock_hsgt_stock_statistics_em(
-        symbol="北向持股", start_date="20221216", end_date="20230315"
+        symbol="北向持股", start_date="20230213", end_date="20230213"
     )
     print(stock_hsgt_stock_statistics_em_df)
 
     stock_hsgt_stock_statistics_em_df = stock_hsgt_stock_statistics_em(
         symbol="南向持股", start_date="20220601", end_date="20220615"
     )
     print(stock_hsgt_stock_statistics_em_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_hsgt_exchange_rate.py` & `akshare-1.9.9/akshare/stock_feature/stock_hsgt_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_inner_trade_xq.py` & `akshare-1.9.9/akshare/stock_feature/stock_inner_trade_xq.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_jgdy_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_jgdy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_lh_yybpm.py` & `akshare-1.9.9/akshare/stock_feature/stock_lh_yybpm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,80 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/5/3 20:30
+Date: 2021/4/19 16:56
 Desc: 同花顺-数据中心-营业部排名
 http://data.10jqka.com.cn/market/longhu/
 """
 import requests
 import pandas as pd
 from tqdm import tqdm
-from bs4 import BeautifulSoup
 
 
 def stock_lh_yyb_most() -> pd.DataFrame:
     """
     同花顺-数据中心-营业部排名-上榜次数最多
     http://data.10jqka.com.cn/market/longhu/
     :return: 上榜次数最多
     :rtype: pandas.DataFrame
     """
-    url = "http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/sbcs/field/sbcs/sort/desc/page/1/"
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36"
-    }
-    r = requests.get(url, headers=headers)
-    soup = BeautifulSoup(r.text, "lxml")
-    page_str = soup.find("span", attrs={"class": "page_info"}).text
-    total_page = int(page_str.split("/")[1]) + 1
     big_df = pd.DataFrame()
-    for page in tqdm(range(1, total_page)):
-        url = f"http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/sbcs/field/sbcs/sort/desc/page/{page}/"
+    for page in tqdm(range(1, 11)):
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36'
+        }
+        url = f'http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/sbcs/field/sbcs/sort/desc/page/{page}/'
         r = requests.get(url, headers=headers)
         temp_df = pd.read_html(r.text)[0]
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
+        big_df = big_df.append(temp_df)
     big_df.reset_index(inplace=True, drop=True)
     return big_df
 
 
 def stock_lh_yyb_capital() -> pd.DataFrame:
     """
     同花顺-数据中心-营业部排名-资金实力最强
     http://data.10jqka.com.cn/market/longhu/
     :return: 资金实力最强
     :rtype: pandas.DataFrame
     """
-    url = "http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/zjsl/field/zgczje/sort/desc/page/1/"
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36"
-    }
-    r = requests.get(url, headers=headers)
-    soup = BeautifulSoup(r.text, "lxml")
-    page_str = soup.find("span", attrs={"class": "page_info"}).text
-    total_page = int(page_str.split("/")[1]) + 1
     big_df = pd.DataFrame()
-    for page in tqdm(range(1, total_page)):
-        url = f"http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/zjsl/field/zgczje/sort/desc/page/{page}/"
+    for page in tqdm(range(1, 11)):
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36'
+        }
+        url = f'http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/zjsl/field/zgczje/sort/desc/page/{page}/'
         r = requests.get(url, headers=headers)
         temp_df = pd.read_html(r.text)[0]
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
+        big_df = big_df.append(temp_df)
     big_df.reset_index(inplace=True, drop=True)
     return big_df
 
 
 def stock_lh_yyb_control() -> pd.DataFrame:
     """
     同花顺-数据中心-营业部排名-抱团操作实力
     http://data.10jqka.com.cn/market/longhu/
     :return: 抱团操作实力
     :rtype: pandas.DataFrame
     """
-    url = "http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/btcz/field/xsjs/sort/desc/page/1/"
-    headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36"
-    }
-    r = requests.get(url, headers=headers)
-    soup = BeautifulSoup(r.text, "lxml")
-    page_str = soup.find("span", attrs={"class": "page_info"}).text
-    total_page = int(page_str.split("/")[1]) + 1
     big_df = pd.DataFrame()
-    for page in tqdm(range(1, total_page)):
-        url = f"http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/btcz/field/xsjs/sort/desc/page/{page}/"
+    for page in tqdm(range(1, 11)):
+        headers = {
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36'
+        }
+        url = f'http://data.10jqka.com.cn/ifmarket/lhbyyb/type/1/tab/btcz/field/xsjs/sort/desc/page/{page}/'
         r = requests.get(url, headers=headers)
         temp_df = pd.read_html(r.text)[0]
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
+        big_df = big_df.append(temp_df)
     big_df.reset_index(inplace=True, drop=True)
     return big_df
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     stock_lh_yyb_most_df = stock_lh_yyb_most()
     print(stock_lh_yyb_most_df)
 
     stock_lh_yyb_capital_df = stock_lh_yyb_capital()
     print(stock_lh_yyb_capital_df)
 
     stock_lh_yyb_control_df = stock_lh_yyb_control()
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_lhb_sina.py` & `akshare-1.9.9/akshare/stock_feature/stock_lhb_sina.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,45 +7,54 @@
 """
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 
 
-def stock_lhb_detail_daily_sina(date: str = "20230420") -> pd.DataFrame:
+def stock_lhb_detail_daily_sina(
+    trade_date: str = "20200730", symbol: str = "当日无价格涨跌幅限制的A股，出现异常波动停牌的股票"
+) -> pd.DataFrame:
     """
     龙虎榜-每日详情
     http://vip.stock.finance.sina.com.cn/q/go.php/vInvestConsult/kind/lhb/index.phtml
-    :param date: 交易日
-    :type date: str
+    :param trade_date: 交易日, e.g., trade_date="20200729"
+    :type trade_date: str
+    :param symbol: 指定标题
+    :type symbol: str
     :return: 龙虎榜-每日详情
     :rtype: pandas.DataFrame
     """
-    date = "-".join([date[:4], date[4:6], date[6:]])
+    trade_date = "-".join([trade_date[:4], trade_date[4:6], trade_date[6:]])
     url = "http://vip.stock.finance.sina.com.cn/q/go.php/vInvestConsult/kind/lhb/index.phtml"
-    params = {"tradedate": date}
+    params = {"tradedate": trade_date}
     r = requests.get(url, params=params)
     soup = BeautifulSoup(r.text, "lxml")
-    selected_html = soup.find("div", attrs={"class": "list"}).find_all(
-        "table", attrs={"class": "list_table"}
-    )
-    big_df = pd.DataFrame()
-    for table in selected_html:
-        temp_df = pd.read_html(table.prettify(), header=0, skiprows=1)[0]
-        temp_symbol = pd.read_html(table.prettify())[0].iat[0, 0]
-        temp_df["指标"] = temp_symbol
-        big_df = pd.concat([big_df, temp_df], ignore_index=True)
-    big_df["股票代码"] = big_df["股票代码"].astype(str).str.zfill(6)
-    del big_df["查看详情"]
-    big_df.columns = ["序号", "股票代码", "股票名称", "收盘价", "对应值", "成交量", "成交额", "指标"]
-    big_df['收盘价'] = pd.to_numeric(big_df['收盘价'], errors="coerce")
-    big_df['对应值'] = pd.to_numeric(big_df['对应值'], errors="coerce")
-    big_df['成交量'] = pd.to_numeric(big_df['成交量'], errors="coerce")
-    big_df['成交额'] = pd.to_numeric(big_df['成交额'], errors="coerce")
-    return big_df
+    table_name_list = [
+        item.get_text().strip()
+        for item in soup.find_all(
+            "span", attrs={"style": "font-weight:bold;font-size:14px;"}
+        )
+        if item.get_text().strip() != ""
+    ]
+    if symbol == "返回当前交易日所有可查询的指标":
+        return table_name_list
+    else:
+        position_num = table_name_list.index(symbol)
+        if len(table_name_list) == position_num + 1:
+            temp_df_1 = pd.read_html(r.text, flavor='bs4', header=1)[position_num].iloc[0:, :]
+            temp_df_2 = pd.read_html(r.text, flavor='bs4', header=1)[position_num + 1].iloc[0:, :]
+            temp_df_3 = pd.read_html(r.text, flavor='bs4', header=1)[position_num + 2].iloc[0:, :]
+            temp_df = pd.concat([temp_df_1, temp_df_2, temp_df_3], ignore_index=True)
+        else:
+            temp_df = pd.read_html(r.text, flavor='bs4', header=1)[position_num].iloc[0:, :]
+    temp_df["股票代码"] = temp_df["股票代码"].astype(str).str.zfill(6)
+    del temp_df["查看详情"]
+    temp_df.columns = ["序号", "股票代码", "股票名称", "收盘价", "对应值", "成交量", "成交额"]
+    return temp_df
 
 
 def _find_last_page(url: str = None, recent_day: str = "60"):
     url = "http://vip.stock.finance.sina.com.cn/q/go.php/vLHBData/kind/ggtj/index.phtml"
     params = {
         "last": recent_day,
         "p": "1",
@@ -115,17 +124,17 @@
             "last": "5",
             "p": page,
         }
         r = requests.get(url, params=params)
         temp_df = pd.read_html(r.text)[0].iloc[0:, :]
         big_df = pd.concat([big_df, temp_df], ignore_index=True)
     big_df.columns = ["营业部名称", "上榜次数", "累积购买额", "买入席位数", "累积卖出额", "卖出席位数", "买入前三股票"]
-    big_df["上榜次数"] = pd.to_numeric(big_df["上榜次数"], errors="coerce")
-    big_df["买入席位数"] = pd.to_numeric(big_df["买入席位数"], errors="coerce")
-    big_df["卖出席位数"] = pd.to_numeric(big_df["卖出席位数"], errors="coerce")
+    big_df['上榜次数'] = pd.to_numeric(big_df['上榜次数'], errors="coerce")
+    big_df['买入席位数'] = pd.to_numeric(big_df['买入席位数'], errors="coerce")
+    big_df['卖出席位数'] = pd.to_numeric(big_df['卖出席位数'], errors="coerce")
     return big_df
 
 
 def stock_lhb_jgzz_sina(recent_day: str = "5") -> pd.DataFrame:
     """
     龙虎榜-机构席位追踪
     http://vip.stock.finance.sina.com.cn/q/go.php/vLHBData/kind/jgzz/index.phtml
@@ -145,16 +154,16 @@
         r = requests.get(url, params=params)
         temp_df = pd.read_html(r.text)[0].iloc[0:, :]
         big_df = pd.concat([big_df, temp_df], ignore_index=True)
     big_df["股票代码"] = big_df["股票代码"].astype(str).str.zfill(6)
     del big_df["当前价"]
     del big_df["涨跌幅"]
     big_df.columns = ["股票代码", "股票名称", "累积买入额", "买入次数", "累积卖出额", "卖出次数", "净额"]
-    big_df["买入次数"] = pd.to_numeric(big_df["买入次数"], errors="coerce")
-    big_df["卖出次数"] = pd.to_numeric(big_df["卖出次数"], errors="coerce")
+    big_df['买入次数'] = pd.to_numeric(big_df['买入次数'], errors="coerce")
+    big_df['卖出次数'] = pd.to_numeric(big_df['卖出次数'], errors="coerce")
     return big_df
 
 
 def stock_lhb_jgmx_sina() -> pd.DataFrame:
     """
     龙虎榜-机构席位成交明细
     http://vip.stock.finance.sina.com.cn/q/go.php/vLHBData/kind/jgmx/index.phtml
@@ -180,16 +189,21 @@
         temp_df = pd.read_html(r.text)[0].iloc[0:, :]
         big_df = pd.concat([big_df, temp_df], ignore_index=True)
     big_df["股票代码"] = big_df["股票代码"].astype(str).str.zfill(6)
     return big_df
 
 
 if __name__ == "__main__":
+    indicator_name_list = stock_lhb_detail_daily_sina(
+        trade_date="20221118", symbol="返回当前交易日所有可查询的指标"
+    )
+    print(indicator_name_list)
+
     stock_lhb_detail_daily_sina_df = stock_lhb_detail_daily_sina(
-        date="20230420"
+        trade_date="20221118", symbol="换手率达20%的证券"
     )
     print(stock_lhb_detail_daily_sina_df)
 
     stock_lhb_ggtj_sina_df = stock_lhb_ggtj_sina(recent_day="60")
     print(stock_lhb_ggtj_sina_df)
 
     stock_lhb_yytj_sina_df = stock_lhb_yytj_sina(recent_day="60")
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_market_legu.py` & `akshare-1.9.9/akshare/stock_feature/stock_market_legu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_pankou_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_pankou_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_qsjy_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_qsjy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_report_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_report_em.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,18 +143,18 @@
     big_df["资产负债率"] = pd.to_numeric(big_df["资产负债率"])
     big_df["股东权益合计"] = pd.to_numeric(big_df["股东权益合计"])
     big_df["股东权益合计"] = pd.to_numeric(big_df["股东权益合计"])
     big_df["公告日期"] = pd.to_datetime(big_df["公告日期"]).dt.date
     return big_df
 
 
-def stock_lrb_em(date: str = "20081231") -> pd.DataFrame:
+def stock_lrb_em(date: str = "20220331") -> pd.DataFrame:
     """
     东方财富-数据中心-年报季报-业绩快报-利润表
-    https://data.eastmoney.com/bbsj/202003/lrb.html
+    http://data.eastmoney.com/bbsj/202003/lrb.html
     :param date: choice of {"20200331", "20200630", "20200930", "20201231", "..."}; 从 20100331 开始
     :type date: str
     :return: 利润表
     :rtype: pandas.DataFrame
     """
     url = "https://datacenter-web.eastmoney.com/api/data/v1/get"
     params = {
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_sse_margin.py` & `akshare-1.9.9/akshare/stock_feature/stock_sse_margin.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_sy_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_sy_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_szse_margin.py` & `akshare-1.9.9/akshare/stock_feature/stock_szse_margin.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_technology_ths.py` & `akshare-1.9.9/akshare/stock_feature/stock_technology_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_tfp_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_tfp_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_three_report_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_three_report_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_yjbb_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_yjbb_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_yjyg_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_yjyg_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_yzxdr_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_yzxdr_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_zf_pg.py` & `akshare-1.9.9/akshare/stock_feature/stock_zf_pg.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_zh_valuation_baidu.py` & `akshare-1.9.9/akshare/stock_feature/stock_zh_valuation_baidu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/17 14:26
+Date: 2023/1/14 20:26
 Desc: 百度股市通- A 股-财务报表-估值数据
 https://gushitong.baidu.com/stock/ab-002044
 """
-import pandas as pd
 import requests
+import pandas as pd
 
 
 def stock_zh_valuation_baidu(
     symbol: str = "002044", indicator: str = "总市值", period: str = "近一年"
 ) -> pd.DataFrame:
     """
     百度股市通- A 股-财务报表-估值数据
@@ -20,38 +20,27 @@
     :param indicator: choice of {"总市值", "市盈率(TTM)", "市盈率(静)", "市净率", "市现率"}
     :type indicator: str
     :param period: choice of {"近一年", "近三年", "近五年", "近十年", "全部"}
     :type period: str
     :return: 估值数据
     :rtype: pandas.DataFrame
     """
-    url = "https://gushitong.baidu.com/opendata"
+    url = "https://finance.pae.baidu.com/selfselect/openapi"
     params = {
-        "openapi": "1",
-        "dspName": "iphone",
-        "tn": "tangram",
-        "client": "app",
-        "query": indicator,
+        "srcid": "51171",
         "code": symbol,
-        "word": "",
-        "resource_id": "51171",
         "market": "ab",
-        "tag": indicator,
+        "tag": f"{indicator}",
         "chart_select": period,
-        "industry_select": "",
-        "skip_industry": "1",
+        "skip_industry": "0",
         "finClientType": "pc",
     }
     r = requests.get(url, params=params)
     data_json = r.json()
-    temp_df = pd.DataFrame(
-        data_json["Result"][0]["DisplayData"]["resultData"]["tplData"]["result"][
-            "chartInfo"
-        ][0]["body"]
-    )
+    temp_df = pd.DataFrame(data_json["Result"]["chartInfo"][0]["body"])
     temp_df.columns = ["date", "value"]
     temp_df["date"] = pd.to_datetime(temp_df["date"]).dt.date
     temp_df["value"] = pd.to_numeric(temp_df["value"])
     return temp_df
 
 
 if __name__ == "__main__":
```

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_zh_vote_baidu.py` & `akshare-1.9.9/akshare/stock_feature/stock_zh_vote_baidu.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_feature/stock_ztb_em.py` & `akshare-1.9.9/akshare/stock_feature/stock_ztb_em.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/19 17:20
+Date: 2022/4/26 15:30
 Desc: 首页-行情中心-涨停板行情-涨停股池
-https://quote.eastmoney.com/ztb/detail#type=ztgc
+http://quote.eastmoney.com/ztb/detail#type=ztgc
 
 涨停板行情专题为您展示了6个股票池，分别为
 涨停股池：包含当日当前涨停的所有A股股票(不含未中断连续一字涨停板的新股)；
 昨日涨停股池：包含上一交易日收盘时涨停的所有A股股票(不含未中断连续一字涨停板的新股)；
 强势股池：包含创下60日新高或近期多次涨停的A股股票；
 次新股池：包含上市一年以内且中断了连续一字涨停板的A股股票；
 炸板股池：包含当日触及过涨停板且当前未封板的A股股票；
@@ -17,15 +17,15 @@
 import pandas as pd
 import requests
 
 
 def stock_zt_pool_em(date: str = "20220426") -> pd.DataFrame:
     """
     东方财富网-行情中心-涨停板行情-涨停股池
-    https://quote.eastmoney.com/ztb/detail#type=ztgc
+    http://quote.eastmoney.com/ztb/detail#type=ztgc
     :return: 涨停股池
     :rtype: pandas.DataFrame
     """
     url = "http://push2ex.eastmoney.com/getTopicZTPool"
     params = {
         "ut": "7eea3edcaed734bea9cbfc24409ed989",
         "dpt": "wz.ztzt",
@@ -101,15 +101,15 @@
 
     return temp_df
 
 
 def stock_zt_pool_previous_em(date: str = "20210521") -> pd.DataFrame:
     """
     东方财富网-行情中心-涨停板行情-昨日涨停股池
-    https://quote.eastmoney.com/ztb/detail#type=zrzt
+    http://quote.eastmoney.com/ztb/detail#type=zrzt
     :return: 昨日涨停股池
     :rtype: pandas.DataFrame
     """
     url = "http://push2ex.eastmoney.com/getYesterdayZTPool"
     params = {
         "ut": "7eea3edcaed734bea9cbfc24409ed989",
         "dpt": "wz.ztzt",
@@ -175,15 +175,15 @@
     temp_df["昨日封板时间"] = temp_df["昨日封板时间"].astype(str).str.zfill(6)
     return temp_df
 
 
 def stock_zt_pool_strong_em(date: str = "20210521") -> pd.DataFrame:
     """
     东方财富网-行情中心-涨停板行情-强势股池
-    https://quote.eastmoney.com/ztb/detail#type=qsgc
+    http://quote.eastmoney.com/ztb/detail#type=qsgc
     :return: 强势股池
     :rtype: pandas.DataFrame
     """
     url = "http://push2ex.eastmoney.com/getTopicQSPool"
     params = {
         "ut": "7eea3edcaed734bea9cbfc24409ed989",
         "dpt": "wz.ztzt",
@@ -249,15 +249,15 @@
     temp_df["涨停价"] = temp_df["涨停价"] / 1000
     return temp_df
 
 
 def stock_zt_pool_sub_new_em(date: str = "20210525") -> pd.DataFrame:
     """
     东方财富网-行情中心-涨停板行情-次新股池
-    https://quote.eastmoney.com/ztb/detail#type=cxgc
+    http://quote.eastmoney.com/ztb/detail#type=cxgc
     :return: 次新股池
     :rtype: pandas.DataFrame
     """
     url = "http://push2ex.eastmoney.com/getTopicCXPooll"
     params = {
         "ut": "7eea3edcaed734bea9cbfc24409ed989",
         "dpt": "wz.ztzt",
@@ -326,15 +326,15 @@
     temp_df.loc[temp_df["上市日期"] == 0, "上市日期"] = "-"
     return temp_df
 
 
 def stock_zt_pool_zbgc_em(date: str = "20210525") -> pd.DataFrame:
     """
     东方财富网-行情中心-涨停板行情-炸板股池
-    https://quote.eastmoney.com/ztb/detail#type=zbgc
+    http://quote.eastmoney.com/ztb/detail#type=zbgc
     :return: 炸板股池
     :rtype: pandas.DataFrame
     """
     url = "http://push2ex.eastmoney.com/getTopicZBPool"
     params = {
         "ut": "7eea3edcaed734bea9cbfc24409ed989",
         "dpt": "wz.ztzt",
@@ -400,15 +400,15 @@
     temp_df["首次封板时间"] = temp_df["首次封板时间"].astype(str).str.zfill(6)
     return temp_df
 
 
 def stock_zt_pool_dtgc_em(date: str = "20220425") -> pd.DataFrame:
     """
     东方财富网-行情中心-涨停板行情-跌停股池
-    https://quote.eastmoney.com/ztb/detail#type=dtgc
+    http://quote.eastmoney.com/ztb/detail#type=dtgc
     :param date: 交易日
     :type date: str
     :return: 跌停股池
     :rtype: pandas.DataFrame
     """
     url = "http://push2ex.eastmoney.com/getTopicDTPool"
     params = {
@@ -497,9 +497,9 @@
 
     stock_zt_pool_sub_new_em_df = stock_zt_pool_sub_new_em(date="20211224")
     print(stock_zt_pool_sub_new_em_df)
 
     stock_zt_pool_zbgc_em_df = stock_zt_pool_zbgc_em(date="20211224")
     print(stock_zt_pool_zbgc_em_df)
 
-    stock_zt_pool_dtgc_em_df = stock_zt_pool_dtgc_em(date="20230419")
+    stock_zt_pool_dtgc_em_df = stock_zt_pool_dtgc_em(date="20220426")
     print(stock_zt_pool_dtgc_em_df)
```

### Comparing `akshare-1.9.80/akshare/stock_feature/ths.js` & `akshare-1.9.9/akshare/stock_feature/ths.js`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_finance.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_finance.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,175 +7,73 @@
 https://vip.stock.finance.sina.com.cn/corp/go.php/vFD_FinanceSummary/stockid/600004.phtml
 新浪财经-财务分析-财务指标
 https://money.finance.sina.com.cn/corp/go.php/vFD_FinancialGuideLine/stockid/600004/displaytype/4.phtml
 新浪财经-发行与分配
 https://money.finance.sina.com.cn/corp/go.php/vISSUE_ShareBonus/stockid/600004.phtml
 """
 from io import BytesIO
-from datetime import datetime
 
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 
 
 def stock_financial_report_sina(
-    stock: str = "sh600600", symbol: str = "资产负债表"
+    stock: str = "600004", symbol: str = "现金流量表"
 ) -> pd.DataFrame:
     """
     新浪财经-财务报表-三大报表
-    https://vip.stock.finance.sina.com.cn/corp/go.php/vFD_FinanceSummary/stockid/600600/displaytype/4.phtml?source=fzb&qq-pf-to=pcqq.group
+    https://vip.stock.finance.sina.com.cn/corp/go.php/vFD_BalanceSheet/stockid/600004/ctrl/part/displaytype/4.phtml
     :param stock: 股票代码
     :type stock: str
     :param symbol: choice of {"资产负债表", "利润表", "现金流量表"}
-    :type symbol: str
+    :type symbol:
     :return: 新浪财经-财务报表-三大报表
     :rtype: pandas.DataFrame
     """
-    symbol_map = {
-        "资产负债表": "fzb",
-        "利润表": "lrb",
-        "现金流量表": "llb"
-    }
-    url = "https://quotes.sina.cn/cn/api/openapi.php/CompanyFinanceService.getFinanceReport2022"
-    params = {
-        "paperCode": f"{stock}",
-        "source": symbol_map[symbol],
-        "type": "0",
-        "page": "1",
-        "num": "100",
-    }
-    r = requests.get(url, params=params)
-    data_json = r.json()
-    df_columns = [item['date_value'] for item in data_json["result"]["data"]["report_date"]]
-    big_df = pd.DataFrame()
-    for date_str in df_columns:
-        temp_df = pd.DataFrame(
-            data_json["result"]["data"]["report_list"][date_str]["data"]
-        )
-        temp_df = temp_df[["item_title", "item_value"]]
-        temp_df['item_value'] = pd.to_numeric(temp_df['item_value'], errors="coerce")
-        temp_tail_df = pd.DataFrame.from_dict(
-            {
-                "数据源": data_json["result"]["data"]["report_list"][date_str][
-                    "data_source"
-                ],
-                "是否审计": data_json["result"]["data"]["report_list"][date_str][
-                    "is_audit"
-                ],
-                "公告日期": data_json["result"]["data"]["report_list"][date_str][
-                    "publish_date"
-                ],
-                "币种": data_json["result"]["data"]["report_list"][date_str][
-                    "rCurrency"
-                ],
-                "类型": data_json["result"]["data"]["report_list"][date_str]["rType"],
-                "更新日期": datetime.fromtimestamp(
-                    data_json["result"]["data"]["report_list"][date_str][
-                        "update_time"
-                    ]
-                ).isoformat(),
-            }, orient="index"
-        )
-        temp_tail_df.reset_index(inplace=True)
-        temp_tail_df.columns = ["item_title", "item_value"]
-        temp_df = pd.concat([temp_df, temp_tail_df], ignore_index=True)
-        temp_df.columns = ["项目", date_str]
-        big_df = pd.concat([big_df, temp_df[date_str]], axis=1, ignore_index=True)
-
-    big_df = big_df.T
-    big_df.columns = temp_df["项目"]
-    big_df = pd.concat([pd.DataFrame({"报告日": df_columns}), big_df], axis=1)
-    return big_df
+    if symbol == "资产负债表":
+        url = f"http://money.finance.sina.com.cn/corp/go.php/vDOWN_BalanceSheet/displaytype/4/stockid/{stock}/ctrl/all.phtml"  # 资产负债表
+    elif symbol == "利润表":
+        url = f"http://money.finance.sina.com.cn/corp/go.php/vDOWN_ProfitStatement/displaytype/4/stockid/{stock}/ctrl/all.phtml"  # 利润表
+    elif symbol == "现金流量表":
+        url = f"http://money.finance.sina.com.cn/corp/go.php/vDOWN_CashFlow/displaytype/4/stockid/{stock}/ctrl/all.phtml"  # 现金流量表
+    r = requests.get(url)
+    temp_df = pd.read_table(BytesIO(r.content), encoding="gb2312", header=None).iloc[
+        :, :-2
+    ]
+    temp_df = temp_df.T
+    temp_df.columns = temp_df.iloc[0, :]
+    temp_df = temp_df.iloc[1:, :]
+    temp_df.index.name = None
+    temp_df.columns.name = None
+    return temp_df
 
 
-def stock_financial_abstract(symbol: str = "600004") -> pd.DataFrame:
+def stock_financial_abstract(stock: str = "600004") -> pd.DataFrame:
     """
-    新浪财经-财务报表-关键指标
+    新浪财经-财务报表-财务摘要
     https://vip.stock.finance.sina.com.cn/corp/go.php/vFD_FinanceSummary/stockid/600004.phtml
-    :param symbol: 股票代码
-    :type symbol: str
-    :return: 新浪财经-财务报表-关键指标
+    :param stock: 股票代码
+    :type stock: str
+    :return: 新浪财经-财务报表-财务摘要
     :rtype: pandas.DataFrame
     """
-    url = "https://quotes.sina.cn/cn/api/openapi.php/CompanyFinanceService.getFinanceReport2022"
-    params = {
-        "paperCode": f"sh{symbol}",
-        "source": "gjzb",
-        "type": "0",
-        "page": "1",
-        "num": "100",
-    }
-    r = requests.get(url, params=params)
-    data_json = r.json()
-    key_list = list(data_json["result"]["data"]["report_list"].keys())
-    temp_df = pd.DataFrame(
-        data_json["result"]["data"]["report_list"][key_list[0]]["data"]
-    )
-    big_df = temp_df["item_title"]
-    for item in key_list:
-        temp_df = pd.DataFrame(data_json["result"]["data"]["report_list"][item]["data"])
-        big_df = pd.concat([big_df, temp_df["item_value"]], axis=1, ignore_index=True)
-    big_df.index = big_df.iloc[:, 0]
-    big_df = big_df.iloc[:, 1:]
-
-    big_one_df = big_df.loc["常用指标":"每股指标"]
-    big_one_df = big_one_df.iloc[1:-1, :]
-    big_one_df.reset_index(inplace=True)
-    big_one_df.insert(0, "选项", "常用指标")
-
-    big_two_df = big_df.loc["每股指标":"盈利能力"]
-    big_two_df = big_two_df.iloc[1:-1, :]
-    big_two_df.reset_index(inplace=True)
-    big_two_df.insert(0, "选项", "每股指标")
-
-    big_three_df = big_df.loc["盈利能力":"成长能力"]
-    big_three_df = big_three_df.iloc[1:-1, :]
-    big_three_df.reset_index(inplace=True)
-    big_three_df.insert(0, "选项", "盈利能力")
-
-    big_four_df = big_df.loc["成长能力":"收益质量"]
-    big_four_df = big_four_df.iloc[1:-1, :]
-    big_four_df.reset_index(inplace=True)
-    big_four_df.insert(0, "选项", "成长能力")
-
-    big_five_df = big_df.loc["收益质量":"财务风险"]
-    big_five_df = big_five_df.iloc[1:-1, :]
-    big_five_df.reset_index(inplace=True)
-    big_five_df.insert(0, "选项", "收益质量")
-
-    big_six_df = big_df.loc["财务风险":"营运能力"]
-    big_six_df = big_six_df.iloc[1:-1, :]
-    big_six_df.reset_index(inplace=True)
-    big_six_df.insert(0, "选项", "财务风险")
-
-    big_seven_df = big_df.loc["营运能力":]
-    big_seven_df = big_seven_df.iloc[1:-1, :]
-    big_seven_df.reset_index(inplace=True)
-    big_seven_df.insert(0, "选项", "营运能力")
-
-    big_df = pd.concat(
-        [
-            big_one_df,
-            big_two_df,
-            big_three_df,
-            big_four_df,
-            big_five_df,
-            big_six_df,
-            big_seven_df,
-        ],
-        ignore_index=True,
-    )
-    key_list.insert(0, "选项")
-    key_list.insert(1, "指标")
-    big_df.columns = key_list
-    for item in big_df.columns[2:]:
-        big_df[item] = pd.to_numeric(big_df[item], errors="coerce")
-    return big_df
+    url = f"https://vip.stock.finance.sina.com.cn/corp/go.php/vFD_FinanceSummary/stockid/{stock}.phtml"
+    r = requests.get(url)
+    temp_df = pd.read_html(r.text)[13].iloc[:, :2]
+    big_df = pd.DataFrame()
+    for i in range(0, len(temp_df), 12):
+        truncated_df = temp_df.iloc[i : i + 11, 1]
+        big_df = pd.concat(
+            [big_df, truncated_df.reset_index(drop=True)], axis=1, ignore_index=True
+        )
+    data_df = big_df.T
+    data_df.columns = temp_df.iloc[:11, 0].tolist()
+    return data_df
 
 
 def stock_financial_analysis_indicator(symbol: str = "600004") -> pd.DataFrame:
     """
     新浪财经-财务分析-财务指标
     https://money.finance.sina.com.cn/corp/go.php/vFD_FinancialGuideLine/stockid/600004/ctrl/2019/displaytype/4.phtml
     :param symbol: 股票代码
@@ -536,41 +434,37 @@
         concat_df["股东总数"] = concat_df["股东总数"].str.strip("查看变化趋势")
         concat_df["平均持股数"] = concat_df["平均持股数"].str.strip("(按总股本计算) 查看变化趋势")
         big_df = pd.concat([big_df, concat_df], axis=0, ignore_index=True)
     big_df.dropna(inplace=True, how="all")
     big_df.reset_index(inplace=True, drop=True)
     big_df.rename(columns={"持股数量(股)": "持股数量", "持股比例(%)": "持股比例"}, inplace=True)
     big_df.columns.name = None
-    big_df["持股数量"] = pd.to_numeric(big_df["持股数量"], errors="coerce")
-    big_df["持股比例"] = big_df["持股比例"].str.strip("↓")
-    big_df["持股比例"] = pd.to_numeric(big_df["持股比例"], errors="coerce")
-    big_df["截至日期"] = pd.to_datetime(big_df["截至日期"]).dt.date
-    big_df["公告日期"] = pd.to_datetime(big_df["公告日期"]).dt.date
-    big_df["股东总数"] = pd.to_numeric(big_df["股东总数"], errors="coerce")
-    big_df["平均持股数"] = pd.to_numeric(big_df["平均持股数"], errors="coerce")
+    big_df.columns
+    big_df['持股数量'] = pd.to_numeric(big_df['持股数量'], errors="coerce")
+    big_df['持股比例'] = big_df['持股比例'].str.strip("↓")
+    big_df['持股比例'] = pd.to_numeric(big_df['持股比例'], errors="coerce")
+    big_df['截至日期'] = pd.to_datetime(big_df['截至日期']).dt.date
+    big_df['公告日期'] = pd.to_datetime(big_df['公告日期']).dt.date
+    big_df['股东总数'] = pd.to_numeric(big_df['股东总数'], errors="coerce")
+    big_df['平均持股数'] = pd.to_numeric(big_df['平均持股数'], errors="coerce")
     return big_df
 
 
 if __name__ == "__main__":
     stock_financial_report_sina_df = stock_financial_report_sina(
-        stock="sh600600", symbol="现金流量表"
-    )
-    print(stock_financial_report_sina_df)
-
-    stock_financial_report_sina_df = stock_financial_report_sina(
-        stock="sh600600", symbol="资产负债表"
+        stock="600009", symbol="现金流量表"
     )
     print(stock_financial_report_sina_df)
 
     stock_financial_report_sina_df = stock_financial_report_sina(
-        stock="sh600600", symbol="利润表"
+        stock="600004", symbol="资产负债表"
     )
     print(stock_financial_report_sina_df)
 
-    stock_financial_abstract_df = stock_financial_abstract(symbol="600004")
+    stock_financial_abstract_df = stock_financial_abstract(stock="000958")
     print(stock_financial_abstract_df)
 
     stock_financial_analysis_indicator_df = stock_financial_analysis_indicator(
         symbol="300168"
     )
     print(stock_financial_analysis_indicator_df)
```

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_finance_hk.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_finance_hk.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_hold.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_hold.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_ipo_declare.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_ipo_declare.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_kcb_detail_sse.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_kcb_detail_sse.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_kcb_sse.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_kcb_sse.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_mda_ym.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_mda_ym.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_notice.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_notice.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_profit_forecast_em.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_profit_forecast_em.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/6 16:44
+Date: 2023/2/10 17:44
 Desc: 东方财富网-数据中心-研究报告-盈利预测
 https://data.eastmoney.com/report/profitforecast.jshtml
 """
 import pandas as pd
 import requests
 from tqdm import tqdm
 
@@ -17,52 +17,49 @@
     :param symbol: "", 默认为获取全部数据; symbol="船舶制造", 则获取具体行业板块的数据; 行业板块可以通过 ak.stock_board_industry_name_em() 接口获取
     :type symbol: str
     :return: 盈利预测
     :rtype: pandas.DataFrame
     """
     url = "https://datacenter-web.eastmoney.com/api/data/v1/get"
     params = {
-        "reportName": "RPT_WEB_RESPREDICT",
-        "columns": "WEB_RESPREDICT",
-        "pageNumber": "1",
-        "pageSize": "500",
-        "sortTypes": "-1",
-        "sortColumns": "RATING_ORG_NUM",
-        "p": "1",
-        "pageNo": "1",
-        "pageNum": "1",
+        'reportName': 'RPT_WEB_RESPREDICT',
+        'columns': 'WEB_RESPREDICT',
+        'pageNumber': '1',
+        'pageSize': '500',
+        'p': '1',
+        'pageNo': '1',
+        'pageNum': '1',
+        'filter': '',
     }
     if symbol:
-        params.update({"filter": f'(INDUSTRY_BOARD="{symbol}")'})
+        params.update({'filter': f'(INDUSTRY_BOARD="{symbol}")'})
 
     r = requests.get(url, params=params)
     data_json = r.json()
-    page_num = int(data_json["result"]["pages"])
+    page_num = int(data_json['result']['pages'])
     big_df = pd.DataFrame()
     for page in tqdm(range(1, page_num + 1), leave=False):
-        params.update(
-            {
-                "pageNumber": page,
-                "p": page,
-                "pageNo": page,
-                "pageNum": page,
-            }
-        )
+        params.update({
+            'pageNumber': page,
+            'p': page,
+            'pageNo': page,
+            'pageNum': page,
+        })
         r = requests.get(url, params=params)
         data_json = r.json()
-        temp_df = pd.DataFrame(data_json["result"]["data"])
+        temp_df = pd.DataFrame(data_json['result']['data'])
         big_df = pd.concat([big_df, temp_df], ignore_index=True)
 
     big_df.reset_index(inplace=True)
     big_df["index"] = big_df.index + 1
 
-    year1 = str(big_df["YEAR1"].mode().values[0])
-    year2 = str(big_df["YEAR2"].mode().values[0])
-    year3 = str(big_df["YEAR3"].mode().values[0])
-    year4 = str(big_df["YEAR4"].mode().values[0])
+    year1 = str(big_df['YEAR1'].mode().values[0])
+    year2 = str(big_df['YEAR2'].mode().values[0])
+    year3 = str(big_df['YEAR3'].mode().values[0])
+    year4 = str(big_df['YEAR4'].mode().values[0])
     big_df.columns = [
         "序号",
         "-",
         "代码",
         "名称",
         "研报数",
         "机构投资评级(近六个月)-买入",
@@ -107,40 +104,30 @@
             "机构投资评级(近六个月)-卖出",
             f"{year1}预测每股收益",
             f"{year2}预测每股收益",
             f"{year3}预测每股收益",
             f"{year4}预测每股收益",
         ]
     ]
-    big_df["机构投资评级(近六个月)-买入"].fillna(0, inplace=True)
-    big_df["机构投资评级(近六个月)-增持"].fillna(0, inplace=True)
-    big_df["机构投资评级(近六个月)-中性"].fillna(0, inplace=True)
-    big_df["机构投资评级(近六个月)-减持"].fillna(0, inplace=True)
-    big_df["机构投资评级(近六个月)-卖出"].fillna(0, inplace=True)
-    big_df["研报数"] = pd.to_numeric(big_df["研报数"], errors="coerce")
-    big_df["机构投资评级(近六个月)-买入"] = pd.to_numeric(
-        big_df["机构投资评级(近六个月)-买入"], errors="coerce"
-    )
-    big_df["机构投资评级(近六个月)-增持"] = pd.to_numeric(
-        big_df["机构投资评级(近六个月)-增持"], errors="coerce"
-    )
-    big_df["机构投资评级(近六个月)-中性"] = pd.to_numeric(
-        big_df["机构投资评级(近六个月)-中性"], errors="coerce"
-    )
-    big_df["机构投资评级(近六个月)-减持"] = pd.to_numeric(
-        big_df["机构投资评级(近六个月)-减持"], errors="coerce"
-    )
-    big_df["机构投资评级(近六个月)-卖出"] = pd.to_numeric(
-        big_df["机构投资评级(近六个月)-卖出"], errors="coerce"
-    )
+    big_df['机构投资评级(近六个月)-买入'].fillna(0, inplace=True)
+    big_df['机构投资评级(近六个月)-增持'].fillna(0, inplace=True)
+    big_df['机构投资评级(近六个月)-中性'].fillna(0, inplace=True)
+    big_df['机构投资评级(近六个月)-减持'].fillna(0, inplace=True)
+    big_df['机构投资评级(近六个月)-卖出'].fillna(0, inplace=True)
+    big_df['研报数'] = pd.to_numeric(big_df['研报数'], errors="coerce")
+    big_df['机构投资评级(近六个月)-买入'] = pd.to_numeric(big_df['机构投资评级(近六个月)-买入'], errors="coerce")
+    big_df['机构投资评级(近六个月)-增持'] = pd.to_numeric(big_df['机构投资评级(近六个月)-增持'], errors="coerce")
+    big_df['机构投资评级(近六个月)-中性'] = pd.to_numeric(big_df['机构投资评级(近六个月)-中性'], errors="coerce")
+    big_df['机构投资评级(近六个月)-减持'] = pd.to_numeric(big_df['机构投资评级(近六个月)-减持'], errors="coerce")
+    big_df['机构投资评级(近六个月)-卖出'] = pd.to_numeric(big_df['机构投资评级(近六个月)-卖出'], errors="coerce")
     big_df[f"{year1}预测每股收益"] = pd.to_numeric(big_df[f"{year1}预测每股收益"], errors="coerce")
     big_df[f"{year2}预测每股收益"] = pd.to_numeric(big_df[f"{year2}预测每股收益"], errors="coerce")
     big_df[f"{year3}预测每股收益"] = pd.to_numeric(big_df[f"{year3}预测每股收益"], errors="coerce")
     big_df[f"{year4}预测每股收益"] = pd.to_numeric(big_df[f"{year4}预测每股收益"], errors="coerce")
-    big_df.sort_values(["研报数"], ascending=False, inplace=True, ignore_index=True)
-    big_df["序号"] = range(1, len(big_df) + 1)
+    big_df.sort_values(['研报数'], ascending=False, inplace=True, ignore_index=True)
+    big_df['序号'] = range(1, len(big_df)+1)
     return big_df
 
 
 if __name__ == "__main__":
-    stock_profit_forecast_em_df = stock_profit_forecast_em(symbol="航运港口")
+    stock_profit_forecast_em_df = stock_profit_forecast_em(symbol="")
     print(stock_profit_forecast_em_df)
```

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_profit_forecast_ths.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_profit_forecast_ths.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 """
-Date: 2023/4/9 21:44
+Date: 2023/3/9 21:44
 Desc: 同花顺-盈利预测
-https://basic.10jqka.com.cn/new/600519/worth.html
+http://basic.10jqka.com.cn/new/600519/worth.html
 """
 import pandas as pd
 import requests
 
 
 def stock_profit_forecast_ths(
     symbol: str = "600519", indicator: str = "预测年报每股收益"
 ) -> pd.DataFrame:
     """
     同花顺-盈利预测
-    https://basic.10jqka.com.cn/new/600519/worth.html
+    http://basic.10jqka.com.cn/new/600519/worth.html
     :param symbol: 股票代码
     :type symbol: str
     :param indicator: choice of {"预测年报每股收益", "预测年报净利润", "业绩预测详表-机构", "业绩预测详表-详细指标预测"}
     :type indicator: str
     :return: 盈利预测
     :rtype: pandas.DataFrame
     """
-    url = f"https://basic.10jqka.com.cn/new/{symbol}/worth.html"
+    url = f"http://basic.10jqka.com.cn/new/{symbol}/worth.html"
     headers = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.90 Safari/537.36",
     }
     r = requests.get(url, headers=headers)
     r.encoding = "gbk"
     if indicator == "预测年报每股收益":
         temp_df = pd.read_html(r.text)[0]
@@ -57,8 +57,10 @@
         ]
         return temp_df
 
 
 if __name__ == "__main__":
     for item in ["预测年报每股收益", "预测年报净利润", "业绩预测详表-机构", "业绩预测详表-详细指标预测"]:
         stock_profit_forecast_ths_df = stock_profit_forecast_ths(symbol="600519", indicator=item)
+        print(item)
         print(stock_profit_forecast_ths_df)
+        print(stock_profit_forecast_ths_df.dtypes)
```

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_recommend.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_recommend.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_register.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_register.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_restricted_em.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_restricted_em.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_zygc.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_zygc.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/stock_fundamental/stock_zyjs_ths.py` & `akshare-1.9.9/akshare/stock_fundamental/stock_zyjs_ths.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/tool/trade_date_hist.py` & `akshare-1.9.9/akshare/tool/trade_date_hist.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/utils/ak_session.py` & `akshare-1.9.9/akshare/utils/ak_session.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/utils/demjson.py` & `akshare-1.9.9/akshare/utils/demjson.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare/utils/token_process.py` & `akshare-1.9.9/akshare/utils/token_process.py`

 * *Files identical despite different names*

### Comparing `akshare-1.9.80/akshare.egg-info/PKG-INFO` & `akshare-1.9.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: akshare
-Version: 1.9.80
-Summary: AKShare is an elegant and simple financial data interface library for Python, built for human beings!
-Home-page: https://github.com/akfamily/akshare
-Author: AKFamily
-Author-email: akfamily.akshare@gmail.com
-License: MIT
-Keywords: stock,option,futures,fund,bond,index,air,finance,spider,quant,quantitative,investment,trading,algotrading,data
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 **AKShare VIP 交流群欢迎大家的加入，加群方式请点击[【加群】](https://zmj.xet.tech/s/28gOeh)**
 
 **相关视频教程已经发布：《AKShare-初阶-使用教学》、《AKShare-初阶-实战应用》、《AKShare-源码解析》、《开源项目巡礼》**，详情请访问[课程](https://app3rqjh1z21630.h5.xiaoeknow.com)查看更多课程信息！
 
 **本次发布 [AKTools](https://github.com/akfamily/aktools) 作为 AKShare 的 HTTP API 版本，突破 Python 语言的限制，欢迎各位小伙伴试用并提出更好的意见或建议！ 点击 [AKTools](https://github.com/akfamily/aktools) 查看使用指南。另外提供 [awesome-data](https://github.com/akfamily/awesome-data) 方便各位小伙伴查询各种数据源。**
 
 ![](https://github.com/akfamily/akshare/blob/master/example/images/AKShare_logo.jpg)
@@ -41,15 +21,15 @@
 
 ## Overview
 
 [AKShare](https://github.com/akfamily/akshare) requires Python(64 bit) 3.8 or greater, aims to make fetch financial data as convenient as possible.
 
 **Write less, get more!**
 
-- Documentation: [中文文档](https://akshare.akfamily.xyz/)
+- Documentation: [中文文档](https://www.akshare.xyz/)
 
 ![](https://github.com/akfamily/akshare/blob/master/example/images/AKShare.svg)
 
 ## Installation
 
 ### General
 
@@ -61,31 +41,31 @@
 
 ```shell
 pip install akshare -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host=mirrors.aliyun.com  --upgrade
 ```
 
 ### PR
 
-Please check out [documentation](https://akshare.akfamily.xyz/contributor.html) if you want to contribute to AKShare
+Please check out [documentation](https://www.akshare.xyz/zh_CN/latest/contributor.html) if you want to contribute to AKShare
 
 ### Docker
 
 #### Pull images
 
 ```shell
-docker pull registry.cn-shanghai.aliyuncs.com/akfamily/aktools:jupyter
+docker pull registry.cn-hangzhou.aliyuncs.com/akshare/akdocker
 ```
 
-#### Run Container
+#### Run AKDocker
 
 ```shell
-docker run -it registry.cn-shanghai.aliyuncs.com/akfamily/aktools:jupyter python
+docker run -it registry.cn-hangzhou.aliyuncs.com/akshare/akdocker python
 ```
 
-#### Test
+#### Test AKDocker
 
 ```python
 import akshare as ak
 
 print(ak.__version__)
 ```
 
@@ -161,19 +141,19 @@
 
 - **Easy of use**: Just one line code to fetch the data;
 - **Extensible**: Easy to customize your own code with other application;
 - **Powerful**: Python ecosystem.
 
 ## Tutorials
 
-1. [Overview](https://akshare.akfamily.xyz/introduction.html)
-2. [Installation](https://akshare.akfamily.xyz/installation.html)
-3. [Tutorial](https://akshare.akfamily.xyz/tutorial.html)
-4. [Data Dict](https://akshare.akfamily.xyz/data/index.html)
-5. [Subjects](https://akshare.akfamily.xyz/topic/index.html)
+1. [Overview](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-introduction.html)
+2. [Installation](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-installation.html)
+3. [Tutorial](https://akshare.readthedocs.io/zh_CN/latest/akshare/ak-tutorial.html)
+4. [Data Dict](https://akshare.readthedocs.io/zh_CN/latest/README.html)
+5. [Subjects](https://akshare.readthedocs.io/zh_CN/latest/subjects/index.html)
 
 ## Contribution
 
 [AKShare](https://github.com/akfamily/akshare) is still under developing, feel free to open issues and pull requests:
 
 - Report or fix bugs
 - Require or publish interface
```

### Comparing `akshare-1.9.80/akshare.egg-info/SOURCES.txt` & `akshare-1.9.9/akshare.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 akshare/article/fred_md.py
 akshare/article/risk_rv.py
 akshare/bank/__init__.py
 akshare/bank/bank_cbirc_2020.py
 akshare/bank/cons.py
 akshare/bond/__init__.py
 akshare/bond/bond_bank.py
-akshare/bond/bond_cb_ths.py
 akshare/bond/bond_cbond.py
 akshare/bond/bond_china_money.py
 akshare/bond/bond_convert.py
 akshare/bond/bond_em.py
 akshare/bond/bond_futures.py
 akshare/bond/bond_info_cm.py
 akshare/bond/bond_investing.py
@@ -162,15 +161,14 @@
 akshare/index/index_eri.py
 akshare/index/index_google.py
 akshare/index/index_hog.py
 akshare/index/index_investing.py
 akshare/index/index_kq_fz.py
 akshare/index/index_kq_ss.py
 akshare/index/index_spot.py
-akshare/index/index_stock_hk.py
 akshare/index/index_stock_zh.py
 akshare/index/index_sugar.py
 akshare/index/index_sw.py
 akshare/index/index_sw_research.py
 akshare/index/index_weibo.py
 akshare/index/index_yw.py
 akshare/index/index_zh_em.py
@@ -224,26 +222,24 @@
 akshare/sport/sport_olympic.py
 akshare/sport/sport_olympic_winter.py
 akshare/spot/__init__.py
 akshare/spot/spot_sge.py
 akshare/stock/__init__.py
 akshare/stock/cons.py
 akshare/stock/stock_allotment_cninfo.py
-akshare/stock/stock_ask_bid_em.py
 akshare/stock/stock_board_concept_em.py
 akshare/stock/stock_board_industry_em.py
 akshare/stock/stock_cg_equity_mortgage.py
 akshare/stock/stock_cg_guarantee.py
 akshare/stock/stock_cg_lawsuit.py
 akshare/stock/stock_dividents_cninfo.py
 akshare/stock/stock_dzjy_em.py
 akshare/stock/stock_fund.py
 akshare/stock/stock_fund_hold.py
-akshare/stock/stock_hk_fhpx_ths.py
-akshare/stock/stock_hk_hot_rank_em.py
+akshare/stock/stock_hist_163.py
 akshare/stock/stock_hk_sina.py
 akshare/stock/stock_hold_control_cninfo.py
 akshare/stock/stock_hold_num_cninfo.py
 akshare/stock/stock_hot_rank_em.py
 akshare/stock/stock_hot_search_baidu.py
 akshare/stock/stock_industry.py
 akshare/stock/stock_industry_cninfo.py
@@ -261,24 +257,26 @@
 akshare/stock/stock_us_js.py
 akshare/stock/stock_us_pink.py
 akshare/stock/stock_us_sina.py
 akshare/stock/stock_us_zh_hx.py
 akshare/stock/stock_weibo_nlp.py
 akshare/stock/stock_zh_a_sina.py
 akshare/stock/stock_zh_a_special.py
-akshare/stock/stock_zh_a_tick_tx.py
+akshare/stock/stock_zh_a_tick_tx_163.py
 akshare/stock/stock_zh_ah_tx.py
 akshare/stock/stock_zh_b_sina.py
 akshare/stock/stock_zh_kcb_report.py
 akshare/stock/stock_zh_kcb_sina.py
 akshare/stock_feature/__init__.py
 akshare/stock_feature/cons.py
 akshare/stock_feature/stock_a_below_net_asset_statistics.py
 akshare/stock_feature/stock_a_high_low.py
 akshare/stock_feature/stock_a_indicator.py
+akshare/stock_feature/stock_a_pb.py
+akshare/stock_feature/stock_a_pe.py
 akshare/stock_feature/stock_a_pe_and_pb.py
 akshare/stock_feature/stock_account_em.py
 akshare/stock_feature/stock_all_pb.py
 akshare/stock_feature/stock_analyst_em.py
 akshare/stock_feature/stock_average_position_lg.py
 akshare/stock_feature/stock_board_concept_ths.py
 akshare/stock_feature/stock_board_industry_ths.py
@@ -287,15 +285,14 @@
 akshare/stock_feature/stock_cls_alerts.py
 akshare/stock_feature/stock_cninfo_yjyg.py
 akshare/stock_feature/stock_comment_em.py
 akshare/stock_feature/stock_congestion_lg.py
 akshare/stock_feature/stock_dxsyl_em.py
 akshare/stock_feature/stock_ebs_lg.py
 akshare/stock_feature/stock_fhps_em.py
-akshare/stock_feature/stock_fhps_ths.py
 akshare/stock_feature/stock_fund_flow.py
 akshare/stock_feature/stock_gdfx_em.py
 akshare/stock_feature/stock_gdhs.py
 akshare/stock_feature/stock_gdzjc_em.py
 akshare/stock_feature/stock_gpzy_em.py
 akshare/stock_feature/stock_gxl_lg.py
 akshare/stock_feature/stock_hist_em.py
```

### Comparing `akshare-1.9.80/setup.py` & `akshare-1.9.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         "tqdm>=4.43.0",
         "openpyxl>=3.0.3",
         "jsonpath>=0.82",
         "tabulate>=0.8.6",
         "decorator>=4.4.2",
         "py_mini_racer>=0.6.0",
         "requests-cache>=0.9.3",
+        "cfscrape>=2.1.1",
     ],
     package_data={"": ["*.py", "*.json", "*.pk", "*.js", "*.zip"]},
     keywords=[
         "stock",
         "option",
         "futures",
         "fund",
```

### Comparing `akshare-1.9.80/tests/test_func.py` & `akshare-1.9.9/tests/test_func.py`

 * *Files identical despite different names*

