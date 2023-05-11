# Comparing `tmp/trademasterntu-0.0.1.tar.gz` & `tmp/trademasterntu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trademasterntu-0.0.1.tar", last modified: Thu May 11 12:15:50 2023, max compression
+gzip compressed data, was "trademasterntu-1.0.1.tar", last modified: Thu May 11 14:14:36 2023, max compression
```

## Comparing `trademasterntu-0.0.1.tar` & `trademasterntu-1.0.1.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.359426 trademasterntu-0.0.1/
--rwxr-xr-x   0 root         (0) root         (0)    11558 2023-05-11 12:14:30.000000 trademasterntu-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    16320 2023-05-11 12:15:50.360426 trademasterntu-0.0.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    16064 2023-05-11 12:14:30.000000 trademasterntu-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      511 2023-05-11 12:15:50.360426 trademasterntu-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      732 2023-05-11 12:15:48.000000 trademasterntu-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.331423 trademasterntu-0.0.1/trademaster/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.332424 trademasterntu-0.0.1/trademaster/agents/
--rwxr-xr-x   0 root         (0) root         (0)      523 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.332424 trademasterntu-0.0.1/trademaster/agents/algorithmic_trading/
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/algorithmic_trading/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8135 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/algorithmic_trading/dqn.py
--rwxr-xr-x   0 root         (0) root         (0)      281 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      125 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.333423 trademasterntu-0.0.1/trademaster/agents/high_frequency_trading/
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/high_frequency_trading/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9993 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/high_frequency_trading/ddqn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.334424 trademasterntu-0.0.1/trademaster/agents/order_execution/
--rwxr-xr-x   0 root         (0) root         (0)       70 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/order_execution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8536 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/order_execution/eteo.py
--rwxr-xr-x   0 root         (0) root         (0)    15383 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/order_execution/pd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.334424 trademasterntu-0.0.1/trademaster/agents/portfolio_management/
--rwxr-xr-x   0 root         (0) root         (0)      164 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/portfolio_management/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    15287 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/portfolio_management/deeptrader.py
--rwxr-xr-x   0 root         (0) root         (0)     6631 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/portfolio_management/eiie.py
--rwxr-xr-x   0 root         (0) root         (0)     2239 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/agents/portfolio_management/investor_imitator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.335424 trademasterntu-0.0.1/trademaster/collector/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/__init__.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/binance.py
--rwxr-xr-x   0 root         (0) root         (0)      300 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      130 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.337424 trademasterntu-0.0.1/trademaster/collector/helper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/helper/__init__.py
--rw-r--r--   0 root         (0) root         (0)       95 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/helper/celery_app.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/helper/celery_config.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/helper/pika_connection.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/helper/run_celery.py
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/helper/websocket_consumer.py
--rw-r--r--   0 root         (0) root         (0)     3391 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/collector/helper/websocket_producer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.337424 trademasterntu-0.0.1/trademaster/datasets/
--rwxr-xr-x   0 root         (0) root         (0)      340 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.338424 trademasterntu-0.0.1/trademaster/datasets/algorithmic_trading/
--rwxr-xr-x   0 root         (0) root         (0)       46 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/algorithmic_trading/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3502 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/algorithmic_trading/dataset.py
--rwxr-xr-x   0 root         (0) root         (0)      290 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      320 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.338424 trademasterntu-0.0.1/trademaster/datasets/high_frequency_trading/
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/high_frequency_trading/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3693 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/high_frequency_trading/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.338424 trademasterntu-0.0.1/trademaster/datasets/order_execution/
--rwxr-xr-x   0 root         (0) root         (0)       42 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/order_execution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3963 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/order_execution/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.339424 trademasterntu-0.0.1/trademaster/datasets/portfolio_management/
--rwxr-xr-x   0 root         (0) root         (0)       47 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/portfolio_management/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4053 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/datasets/portfolio_management/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.339424 trademasterntu-0.0.1/trademaster/environments/
--rwxr-xr-x   0 root         (0) root         (0)      855 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.340424 trademasterntu-0.0.1/trademaster/environments/algorithmic_trading/
--rwxr-xr-x   0 root         (0) root         (0)       54 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/algorithmic_trading/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14512 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/algorithmic_trading/environment.py
--rwxr-xr-x   0 root         (0) root         (0)      321 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      191 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.340424 trademasterntu-0.0.1/trademaster/environments/high_frequency_trading/
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/high_frequency_trading/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32810 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/high_frequency_trading/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.341424 trademasterntu-0.0.1/trademaster/environments/order_execution/
--rwxr-xr-x   0 root         (0) root         (0)      116 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/order_execution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    21527 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/order_execution/eteo_environment.py
--rwxr-xr-x   0 root         (0) root         (0)     8469 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/order_execution/pd_environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.342424 trademasterntu-0.0.1/trademaster/environments/portfolio_management/
--rwxr-xr-x   0 root         (0) root         (0)      357 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/portfolio_management/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10053 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/portfolio_management/deeptrader_environment.py
--rwxr-xr-x   0 root         (0) root         (0)    11513 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/portfolio_management/eiie_environment.py
--rwxr-xr-x   0 root         (0) root         (0)    10348 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/portfolio_management/environment.py
--rwxr-xr-x   0 root         (0) root         (0)    19345 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/portfolio_management/inverstor_imitator_environment.py
--rwxr-xr-x   0 root         (0) root         (0)    14016 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/environments/portfolio_management/sarl_environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.342424 trademasterntu-0.0.1/trademaster/evaluation/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.343425 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/__init__.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/builder.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.344425 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/model/
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4479 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/model/linear_model.py
--rw-r--r--   0 root         (0) root         (0)     4332 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/model/run_linear_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.344425 trademasterntu-0.0.1/trademaster/imputation/
--rw-r--r--   0 root         (0) root         (0)      128 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/imputation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      309 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/imputation/builder.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/imputation/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.345425 trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7601 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/dataset.py
--rw-r--r--   0 root         (0) root         (0)    11328 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/imputation.py
--rw-r--r--   0 root         (0) root         (0)     6923 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.346425 trademasterntu-0.0.1/trademaster/losses/
--rwxr-xr-x   0 root         (0) root         (0)      118 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/losses/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      274 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/losses/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      381 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/losses/custom.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/losses/hft_loss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.350425 trademasterntu-0.0.1/trademaster/nets/
--rwxr-xr-x   0 root         (0) root         (0)     9591 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/ASU.py
--rwxr-xr-x   0 root         (0) root         (0)     1570 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/MSU.py
--rwxr-xr-x   0 root         (0) root         (0)      366 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      263 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      159 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/custom.py
--rwxr-xr-x   0 root         (0) root         (0)    10598 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/deeptrader.py
--rwxr-xr-x   0 root         (0) root         (0)     1179 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/dqn.py
--rwxr-xr-x   0 root         (0) root         (0)     2423 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/eiie.py
--rwxr-xr-x   0 root         (0) root         (0)     1615 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/eteo.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/high_frequency_trading_dqn.py
--rwxr-xr-x   0 root         (0) root         (0)     1401 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/investor_imitator.py
--rwxr-xr-x   0 root         (0) root         (0)     1393 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/pd.py
--rwxr-xr-x   0 root         (0) root         (0)     1930 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/nets/sarl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.351425 trademasterntu-0.0.1/trademaster/optimizers/
--rwxr-xr-x   0 root         (0) root         (0)      166 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/optimizers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      307 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/optimizers/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      708 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/optimizers/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.351425 trademasterntu-0.0.1/trademaster/preprocessor/
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/preprocessor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      308 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/preprocessor/builder.py
--rw-r--r--   0 root         (0) root         (0)      299 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/preprocessor/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.352425 trademasterntu-0.0.1/trademaster/preprocessor/yfinance_preprocessor/
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/preprocessor/yfinance_preprocessor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34430 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/preprocessor/yfinance_preprocessor/processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.352425 trademasterntu-0.0.1/trademaster/pretrained/
--rwxr-xr-x   0 root         (0) root         (0)      335 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/pretrained/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.353426 trademasterntu-0.0.1/trademaster/trainers/
--rwxr-xr-x   0 root         (0) root         (0)      761 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.353426 trademasterntu-0.0.1/trademaster/trainers/algorithmic_trading/
--rwxr-xr-x   0 root         (0) root         (0)       46 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/algorithmic_trading/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    16027 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/algorithmic_trading/trainer.py
--rwxr-xr-x   0 root         (0) root         (0)      271 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/builder.py
--rwxr-xr-x   0 root         (0) root         (0)      154 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.354426 trademasterntu-0.0.1/trademaster/trainers/high_frequency_trading/
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/high_frequency_trading/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9153 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/high_frequency_trading/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.354426 trademasterntu-0.0.1/trademaster/trainers/order_execution/
--rwxr-xr-x   0 root         (0) root         (0)      100 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/order_execution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10583 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/order_execution/eteo_trainer.py
--rwxr-xr-x   0 root         (0) root         (0)    12102 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/order_execution/pd_trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.356426 trademasterntu-0.0.1/trademaster/trainers/portfolio_management/
--rwxr-xr-x   0 root         (0) root         (0)      316 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/portfolio_management/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    13698 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/portfolio_management/deeptrader_trainer.py
--rwxr-xr-x   0 root         (0) root         (0)    10768 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/portfolio_management/eiie_trainer.py
--rwxr-xr-x   0 root         (0) root         (0)     7023 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/portfolio_management/investor_imitator_trainer.py
--rwxr-xr-x   0 root         (0) root         (0)    11751 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/portfolio_management/sarl_trainer.py
--rwxr-xr-x   0 root         (0) root         (0)     6885 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/trainers/portfolio_management/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.356426 trademasterntu-0.0.1/trademaster/transition/
--rwxr-xr-x   0 root         (0) root         (0)      106 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/transition/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      314 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/transition/builder.py
--rwxr-xr-x   0 root         (0) root         (0)     1520 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/transition/custom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.358426 trademasterntu-0.0.1/trademaster/utils/
--rwxr-xr-x   0 root         (0) root         (0)      879 2023-05-11 12:15:20.000000 trademasterntu-0.0.1/trademaster/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4048 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/utils/general_replay_buffer.py
--rw-r--r--   0 root         (0) root         (0)    18681 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/utils/labeling_util.py
--rwxr-xr-x   0 root         (0) root         (0)     1057 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/utils/layers.py
--rwxr-xr-x   0 root         (0) root         (0)    17410 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)    13758 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/utils/replay_buffer.py
--rwxr-xr-x   0 root         (0) root         (0)    19116 2023-05-11 12:14:34.000000 trademasterntu-0.0.1/trademaster/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 12:15:50.359426 trademasterntu-0.0.1/trademasterntu.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16320 2023-05-11 12:15:50.000000 trademasterntu-0.0.1/trademasterntu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5547 2023-05-11 12:15:50.000000 trademasterntu-0.0.1/trademasterntu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 12:15:50.000000 trademasterntu-0.0.1/trademasterntu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-11 12:15:50.000000 trademasterntu-0.0.1/trademasterntu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-11 12:15:50.000000 trademasterntu-0.0.1/trademasterntu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.576610 trademasterntu-1.0.1/
+-rwxr-xr-x   0 root         (0) root         (0)    11558 2023-05-11 14:12:54.000000 trademasterntu-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-11 14:14:36.576610 trademasterntu-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-11 14:13:49.000000 trademasterntu-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      511 2023-05-11 14:14:36.577610 trademasterntu-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      735 2023-05-11 14:14:35.000000 trademasterntu-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.551607 trademasterntu-1.0.1/trademasterntu/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.552608 trademasterntu-1.0.1/trademasterntu/agents/
+-rwxr-xr-x   0 root         (0) root         (0)      523 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.553608 trademasterntu-1.0.1/trademasterntu/agents/algorithmic_trading/
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/algorithmic_trading/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8138 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/algorithmic_trading/dqn.py
+-rwxr-xr-x   0 root         (0) root         (0)      284 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      125 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.553608 trademasterntu-1.0.1/trademasterntu/agents/high_frequency_trading/
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/high_frequency_trading/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9996 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/high_frequency_trading/ddqn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.553608 trademasterntu-1.0.1/trademasterntu/agents/order_execution/
+-rwxr-xr-x   0 root         (0) root         (0)       70 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/order_execution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8539 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/order_execution/eteo.py
+-rwxr-xr-x   0 root         (0) root         (0)    15386 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/order_execution/pd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.554608 trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/
+-rwxr-xr-x   0 root         (0) root         (0)      164 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15290 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/deeptrader.py
+-rwxr-xr-x   0 root         (0) root         (0)     6634 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/eiie.py
+-rwxr-xr-x   0 root         (0) root         (0)     2242 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/investor_imitator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.555608 trademasterntu-1.0.1/trademasterntu/collector/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      421 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/binance.py
+-rwxr-xr-x   0 root         (0) root         (0)      303 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      130 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.557608 trademasterntu-1.0.1/trademasterntu/collector/helper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/helper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       95 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/helper/celery_app.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/helper/celery_config.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/helper/pika_connection.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/helper/run_celery.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/helper/websocket_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/collector/helper/websocket_producer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.557608 trademasterntu-1.0.1/trademasterntu/datasets/
+-rwxr-xr-x   0 root         (0) root         (0)      340 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.558608 trademasterntu-1.0.1/trademasterntu/datasets/algorithmic_trading/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/datasets/algorithmic_trading/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3505 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/datasets/algorithmic_trading/dataset.py
+-rwxr-xr-x   0 root         (0) root         (0)      293 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      320 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.558608 trademasterntu-1.0.1/trademasterntu/datasets/high_frequency_trading/
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/high_frequency_trading/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/high_frequency_trading/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.558608 trademasterntu-1.0.1/trademasterntu/datasets/order_execution/
+-rwxr-xr-x   0 root         (0) root         (0)       42 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/order_execution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3966 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/datasets/order_execution/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.559608 trademasterntu-1.0.1/trademasterntu/datasets/portfolio_management/
+-rwxr-xr-x   0 root         (0) root         (0)       47 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/portfolio_management/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4056 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/datasets/portfolio_management/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.559608 trademasterntu-1.0.1/trademasterntu/environments/
+-rwxr-xr-x   0 root         (0) root         (0)      855 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.559608 trademasterntu-1.0.1/trademasterntu/environments/algorithmic_trading/
+-rwxr-xr-x   0 root         (0) root         (0)       54 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/algorithmic_trading/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14515 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/algorithmic_trading/environment.py
+-rwxr-xr-x   0 root         (0) root         (0)      324 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      191 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.560608 trademasterntu-1.0.1/trademasterntu/environments/high_frequency_trading/
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/high_frequency_trading/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32813 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/high_frequency_trading/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.561608 trademasterntu-1.0.1/trademasterntu/environments/order_execution/
+-rwxr-xr-x   0 root         (0) root         (0)      116 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/order_execution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21530 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/order_execution/eteo_environment.py
+-rwxr-xr-x   0 root         (0) root         (0)     8472 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/order_execution/pd_environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.562609 trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/
+-rwxr-xr-x   0 root         (0) root         (0)      357 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10056 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/deeptrader_environment.py
+-rwxr-xr-x   0 root         (0) root         (0)    11516 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/eiie_environment.py
+-rwxr-xr-x   0 root         (0) root         (0)    10351 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/environment.py
+-rwxr-xr-x   0 root         (0) root         (0)    19354 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/inverstor_imitator_environment.py
+-rwxr-xr-x   0 root         (0) root         (0)    14025 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/sarl_environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.563609 trademasterntu-1.0.1/trademasterntu/evaluation/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.563609 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/builder.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.564609 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/model/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4482 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/model/linear_model.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/model/run_linear_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.564609 trademasterntu-1.0.1/trademasterntu/imputation/
+-rw-r--r--   0 root         (0) root         (0)      128 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/imputation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/imputation/builder.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/imputation/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.565609 trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7601 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11340 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/imputation.py
+-rw-r--r--   0 root         (0) root         (0)     6923 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.566609 trademasterntu-1.0.1/trademasterntu/losses/
+-rwxr-xr-x   0 root         (0) root         (0)      118 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/losses/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      277 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/losses/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      381 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/losses/custom.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/losses/hft_loss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.569609 trademasterntu-1.0.1/trademasterntu/nets/
+-rwxr-xr-x   0 root         (0) root         (0)     9591 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/ASU.py
+-rwxr-xr-x   0 root         (0) root         (0)     1570 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/MSU.py
+-rwxr-xr-x   0 root         (0) root         (0)      366 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      266 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      159 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/custom.py
+-rwxr-xr-x   0 root         (0) root         (0)    10598 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/deeptrader.py
+-rwxr-xr-x   0 root         (0) root         (0)     1182 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/dqn.py
+-rwxr-xr-x   0 root         (0) root         (0)     2426 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/eiie.py
+-rwxr-xr-x   0 root         (0) root         (0)     1615 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/eteo.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/high_frequency_trading_dqn.py
+-rwxr-xr-x   0 root         (0) root         (0)     1401 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/investor_imitator.py
+-rwxr-xr-x   0 root         (0) root         (0)     1393 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/pd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1930 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/nets/sarl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.569609 trademasterntu-1.0.1/trademasterntu/optimizers/
+-rwxr-xr-x   0 root         (0) root         (0)      166 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/optimizers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      310 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/optimizers/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      708 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/optimizers/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.570609 trademasterntu-1.0.1/trademasterntu/preprocessor/
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/preprocessor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/preprocessor/builder.py
+-rw-r--r--   0 root         (0) root         (0)      299 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/preprocessor/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.570609 trademasterntu-1.0.1/trademasterntu/preprocessor/yfinance_preprocessor/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/preprocessor/yfinance_preprocessor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34433 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/preprocessor/yfinance_preprocessor/processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.570609 trademasterntu-1.0.1/trademasterntu/pretrained/
+-rwxr-xr-x   0 root         (0) root         (0)      335 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/pretrained/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.571609 trademasterntu-1.0.1/trademasterntu/trainers/
+-rwxr-xr-x   0 root         (0) root         (0)      761 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.572610 trademasterntu-1.0.1/trademasterntu/trainers/algorithmic_trading/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/algorithmic_trading/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16030 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/algorithmic_trading/trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)      274 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)      154 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.572610 trademasterntu-1.0.1/trademasterntu/trainers/high_frequency_trading/
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/high_frequency_trading/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9156 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/high_frequency_trading/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.573609 trademasterntu-1.0.1/trademasterntu/trainers/order_execution/
+-rwxr-xr-x   0 root         (0) root         (0)      100 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/order_execution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10586 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/order_execution/eteo_trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)    12108 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/order_execution/pd_trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.574610 trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/
+-rwxr-xr-x   0 root         (0) root         (0)      316 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13701 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/deeptrader_trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)    10771 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/eiie_trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)     7026 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/investor_imitator_trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)    11757 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/sarl_trainer.py
+-rwxr-xr-x   0 root         (0) root         (0)     6891 2023-05-11 14:14:28.000000 trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.574610 trademasterntu-1.0.1/trademasterntu/transition/
+-rwxr-xr-x   0 root         (0) root         (0)      106 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/transition/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      317 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/transition/builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     1520 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/transition/custom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.576610 trademasterntu-1.0.1/trademasterntu/utils/
+-rwxr-xr-x   0 root         (0) root         (0)      879 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/utils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4048 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/utils/general_replay_buffer.py
+-rw-r--r--   0 root         (0) root         (0)    18681 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/utils/labeling_util.py
+-rwxr-xr-x   0 root         (0) root         (0)     1057 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/utils/layers.py
+-rwxr-xr-x   0 root         (0) root         (0)    17410 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)    13758 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/utils/replay_buffer.py
+-rwxr-xr-x   0 root         (0) root         (0)    19116 2023-05-11 14:14:29.000000 trademasterntu-1.0.1/trademasterntu/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 14:14:36.552608 trademasterntu-1.0.1/trademasterntu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      936 2023-05-11 14:14:36.000000 trademasterntu-1.0.1/trademasterntu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-05-11 14:14:36.000000 trademasterntu-1.0.1/trademasterntu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 14:14:36.000000 trademasterntu-1.0.1/trademasterntu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-11 14:14:36.000000 trademasterntu-1.0.1/trademasterntu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-11 14:14:36.000000 trademasterntu-1.0.1/trademasterntu.egg-info/top_level.txt
```

### Comparing `trademasterntu-0.0.1/LICENSE` & `trademasterntu-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/setup.py` & `trademasterntu-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('README.md', "r") as fh:
     long_description = fh.read()
 
 setup(
     name='trademasterntu',
-    version='0.0.1',
+    version='1.0.1',
     description='TradeMaster - A platform for algorithmic trading',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='NTU_trademaster',
     author_email='TradeMaster.NTU@gmail.com',
     url='https://github.com/TradeMaster-NTU/TradeMaster',
-    packages=find_packages(include=["trademaster*"]),
+    packages=find_packages(include=["trademasterntu*"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[],
 )
```

### Comparing `trademasterntu-0.0.1/trademaster/agents/__init__.py` & `trademasterntu-1.0.1/trademasterntu/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/agents/algorithmic_trading/dqn.py` & `trademasterntu-1.0.1/trademasterntu/agents/algorithmic_trading/dqn.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 
 from ..builder import AGENTS
 from ..custom import AgentBase
-from trademaster.utils import get_attr, GeneralReplayBuffer, get_optim_param
+from trademasterntu.utils import get_attr, GeneralReplayBuffer, get_optim_param
 import torch
 from torch import Tensor
 from typing import Tuple
 from copy import deepcopy
 from torch.nn.utils import clip_grad_norm_
 from types import MethodType
 from collections import namedtuple
```

### Comparing `trademasterntu-0.0.1/trademaster/agents/high_frequency_trading/ddqn.py` & `trademasterntu-1.0.1/trademasterntu/agents/high_frequency_trading/ddqn.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 
 from ..builder import AGENTS
 from ..custom import AgentBase
-from trademaster.utils import get_attr, get_optim_param, ReplayBufferHFT
+from trademasterntu.utils import get_attr, get_optim_param, ReplayBufferHFT
 import torch
 from torch import Tensor
 from typing import Tuple
 from copy import deepcopy
 from torch.nn.utils import clip_grad_norm_
 from types import MethodType
 import torch.nn.functional as F
```

### Comparing `trademasterntu-0.0.1/trademaster/agents/order_execution/eteo.py` & `trademasterntu-1.0.1/trademasterntu/agents/order_execution/eteo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 
 from ..builder import AGENTS
 from ..custom import AgentBase
-from trademaster.utils import get_attr, ReplayBuffer, get_optim_param
+from trademasterntu.utils import get_attr, ReplayBuffer, get_optim_param
 import numpy as np
 import torch
 from random import sample
 from types import MethodType
 from copy import deepcopy
 from torch import Tensor
 from typing import Tuple
```

### Comparing `trademasterntu-0.0.1/trademaster/agents/order_execution/pd.py` & `trademasterntu-1.0.1/trademasterntu/agents/order_execution/pd.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 
 from ..builder import AGENTS
 from ..custom import AgentBase
-from trademaster.utils import get_attr, get_optim_param
+from trademasterntu.utils import get_attr, get_optim_param
 import numpy as np
 import torch
 from types import MethodType
 from copy import deepcopy
 from collections import namedtuple
 from torch import Tensor
 from typing import Tuple
```

### Comparing `trademasterntu-0.0.1/trademaster/agents/portfolio_management/deeptrader.py` & `trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/deeptrader.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 
 from ..builder import AGENTS
 from ..custom import AgentBase
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import torch
 from torch.distributions import Normal
 import random
 import pandas as pd
 import numpy as np
 from collections import namedtuple
 from torch import Tensor
```

### Comparing `trademasterntu-0.0.1/trademaster/agents/portfolio_management/eiie.py` & `trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/eiie.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch
 from torch import Tensor
 from typing import Tuple
 from ..builder import AGENTS
 from ..custom import AgentBase
 import random
 from collections import namedtuple
-from trademaster.utils import get_attr, GeneralReplayBuffer, get_optim_param
+from trademasterntu.utils import get_attr, GeneralReplayBuffer, get_optim_param
 
 
 
 @AGENTS.register_module()
 class PortfolioManagementEIIE(AgentBase):
     def __init__(self, **kwargs):
         super(PortfolioManagementEIIE, self).__init__()
```

### Comparing `trademasterntu-0.0.1/trademaster/agents/portfolio_management/investor_imitator.py` & `trademasterntu-1.0.1/trademasterntu/agents/portfolio_management/investor_imitator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 
 from ..builder import AGENTS
 from ..custom import AgentBase
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import torch
 from torch.distributions import Normal
 import random
 import pandas as pd
 import numpy as np
 from torch.distributions import Categorical
```

### Comparing `trademasterntu-0.0.1/trademaster/collector/helper/pika_connection.py` & `trademasterntu-1.0.1/trademasterntu/collector/helper/pika_connection.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/collector/helper/websocket_consumer.py` & `trademasterntu-1.0.1/trademasterntu/collector/helper/websocket_consumer.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/collector/helper/websocket_producer.py` & `trademasterntu-1.0.1/trademasterntu/collector/helper/websocket_producer.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/datasets/algorithmic_trading/dataset.py` & `trademasterntu-1.0.1/trademasterntu/datasets/algorithmic_trading/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 ROOT = str(Path(__file__).resolve().parents[3])
 sys.path.append(ROOT)
 
 import os.path as osp
 from ..custom import CustomDataset
 from ..builder import DATASETS
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import pandas as pd
 import os
 
 @DATASETS.register_module()
 class AlgorithmicTradingDataset(CustomDataset):
     def __init__(self, **kwargs):
         super(AlgorithmicTradingDataset, self).__init__()
```

### Comparing `trademasterntu-0.0.1/trademaster/datasets/high_frequency_trading/dataset.py` & `trademasterntu-1.0.1/trademasterntu/datasets/high_frequency_trading/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 ROOT = str(Path(__file__).resolve().parents[3])
 sys.path.append(ROOT)
 
 import os.path as osp
 from ..custom import CustomDataset
 from ..builder import DATASETS
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import pandas as pd
 import os
 
 @DATASETS.register_module()
 class HighFrequencyTradingDataset(CustomDataset):
     def __init__(self, **kwargs):
         super(HighFrequencyTradingDataset, self).__init__()
```

### Comparing `trademasterntu-0.0.1/trademaster/datasets/order_execution/dataset.py` & `trademasterntu-1.0.1/trademasterntu/datasets/order_execution/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 ROOT = str(Path(__file__).resolve().parents[3])
 sys.path.append(ROOT)
 
 import os.path as osp
 from ..custom import CustomDataset
 from ..builder import DATASETS
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import pandas as pd
 import os
 @DATASETS.register_module()
 class OrderExecutionDataset(CustomDataset):
     def __init__(self, **kwargs):
         super(OrderExecutionDataset, self).__init__()
```

### Comparing `trademasterntu-0.0.1/trademaster/datasets/portfolio_management/dataset.py` & `trademasterntu-1.0.1/trademasterntu/datasets/portfolio_management/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 ROOT = str(Path(__file__).resolve().parents[3])
 sys.path.append(ROOT)
 
 import os.path as osp
 from ..custom import CustomDataset
 from ..builder import DATASETS
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import pandas as pd
 import os
 
 @DATASETS.register_module()
 class PortfolioManagementDataset(CustomDataset):
     def __init__(self, **kwargs):
         super(PortfolioManagementDataset, self).__init__()
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/__init__.py` & `trademasterntu-1.0.1/trademasterntu/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/environments/algorithmic_trading/environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/algorithmic_trading/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
 from gym import spaces
 from collections import OrderedDict
 import pickle
 import os.path as osp
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/high_frequency_trading/environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/high_frequency_trading/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import torch
 from collections import OrderedDict
 from gym import spaces
 from ..builder import ENVIRONMENTS
 from ..custom import Environments
 import pandas as pd
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import numpy as np
 
 import sys
 from pathlib import Path
 import pickle
 import os.path as osp
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/order_execution/eteo_environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/order_execution/eteo_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from logging import raiseExceptions
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
 from gym import spaces
 from collections import OrderedDict
 
 @ENVIRONMENTS.register_module()
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/order_execution/pd_environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/order_execution/pd_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from logging import raiseExceptions
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
 from gym import spaces
 from collections import OrderedDict
 
 @ENVIRONMENTS.register_module()
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/portfolio_management/deeptrader_environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/deeptrader_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
 from gym import spaces
 from collections import OrderedDict
 
 @ENVIRONMENTS.register_module()
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/portfolio_management/eiie_environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/eiie_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
 from gym import spaces
 from collections import OrderedDict
 import pickle
 import os.path as osp
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/portfolio_management/environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
 from gym import spaces
 from collections import OrderedDict
 """this environment is based on https://github.com/AI4Finance-Foundation/FinRL/blob/master/finrl/meta/env_portfolio_allocation/env_portfolio.py but 
 adding 2 additional features and 1 modification:
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/portfolio_management/inverstor_imitator_environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/inverstor_imitator_environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import torch
 import sys
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
-from trademaster.pretrained import pretrained
+from trademasterntu.pretrained import pretrained
 from gym import spaces
-from trademaster.nets.investor_imitator import MLPReg
+from trademasterntu.nets.investor_imitator import MLPReg
 from collections import OrderedDict
 import pickle
 import os.path as osp
 
 
 @ENVIRONMENTS.register_module()
 class PortfolioManagementInvestorImitatorEnvironment(Environments):
```

### Comparing `trademasterntu-0.0.1/trademaster/environments/portfolio_management/sarl_environment.py` & `trademasterntu-1.0.1/trademasterntu/environments/portfolio_management/sarl_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import torch
 import sys
 from pathlib import Path
 
 ROOT = str(Path(__file__).resolve().parents[2])
 sys.path.append(ROOT)
 import numpy as np
-from trademaster.utils import get_attr, print_metrics
+from trademasterntu.utils import get_attr, print_metrics
 import pandas as pd
 from ..custom import Environments
 from ..builder import ENVIRONMENTS
-from trademaster.pretrained import pretrained
+from trademasterntu.pretrained import pretrained
 from gym import spaces
 from collections import OrderedDict
 import pickle
 import os.path as osp
 
 @ENVIRONMENTS.register_module()
 class PortfolioManagementSARLEnvironment(Environments):
@@ -49,15 +49,15 @@
         self.stock_dim = len(self.df.tic.unique())
         self.tic_list = self.df.tic.unique()
         self.state_space_shape = self.stock_dim
         self.action_space_shape = self.stock_dim + 1
         self.length_day = length_day
 
         ##############################################################
-        from trademaster.nets import mLSTMClf
+        from trademasterntu.nets import mLSTMClf
         self.network_dict = torch.load(get_attr(pretrained, "sarl_encoder", None))
         self.net = mLSTMClf(n_features = len(self.tech_indicator_list), layer_num = 1, n_hidden = 128, tic_number = len(self.tic_list)).cuda()
         self.net.load_state_dict(self.network_dict)
         ##############################################################
 
         self.action_space = spaces.Box(low=-5,
                                        high=5,
```

### Comparing `trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/model/linear_model.py` & `trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/model/linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from pathlib import Path
 ROOT = str(Path(__file__).resolve().parents[3])
 sys.path.append(ROOT)
 import pandas as pd
 from ..builder import Market_Dynamics_Model
 from ..custom import Market_dynamics_model
-from trademaster.utils import get_attr, labeling_util as util
+from trademasterntu.utils import get_attr, labeling_util as util
 from pathlib import Path
 import warnings
 
 @Market_Dynamics_Model.register_module()
 
 class Linear_Market_Dynamics_Model(Market_dynamics_model):
     def __init__(self,**kwargs):
```

### Comparing `trademasterntu-0.0.1/trademaster/evaluation/market_dynamics_labeling/model/run_linear_model.py` & `trademasterntu-1.0.1/trademasterntu/evaluation/market_dynamics_labeling/model/run_linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from pathlib import Path
 ROOT = str(Path(__file__).resolve().parents[4])
 sys.path.append(ROOT)
 import argparse
 import pandas as pd
-from trademaster.utils import  labeling_util as util
+from trademasterntu.utils import  labeling_util as util
 from pathlib import Path
 import warnings
 
 
 def main(args):
     warnings.warn("running this script as main is deprecated, you should run the run.py in "
                   "tool/market_dynamics_labeling/ to use the latest version ")
```

### Comparing `trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/dataset.py` & `trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/dataset.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/imputation.py` & `trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/imputation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 ROOT = str(Path(__file__).resolve().parents[3])
 sys.path.append(ROOT)
 
 import os
 import os.path as osp
 from ..custom import CustomImputation
 from ..builder import IMPUTATION
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 
 import argparse
 import torch
 import json
 import yaml
 import matplotlib.pyplot as plt
 import mplfinance as mpf
 import pandas as pd
 import numpy as np
 import pickle
 
-from trademaster.imputation.missing_value_imputation.model.main_model import CSDI_own
-from trademaster.imputation.missing_value_imputation.dataset import get_dataloader
-from trademaster.imputation.missing_value_imputation.utils import train, evaluate
+from trademasterntu.imputation.missing_value_imputation.model.main_model import CSDI_own
+from trademasterntu.imputation.missing_value_imputation.dataset import get_dataloader
+from trademasterntu.imputation.missing_value_imputation.utils import train, evaluate
 
 
 @IMPUTATION.register_module()
 class CSDI_Imputation(CustomImputation):
     def __init__(self, **kwargs):
         super(CSDI_Imputation, self).__init__()
         self.kwargs = kwargs
```

### Comparing `trademasterntu-0.0.1/trademaster/imputation/missing_value_imputation/utils.py` & `trademasterntu-1.0.1/trademasterntu/imputation/missing_value_imputation/utils.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/losses/hft_loss.py` & `trademasterntu-1.0.1/trademasterntu/losses/hft_loss.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/ASU.py` & `trademasterntu-1.0.1/trademasterntu/nets/ASU.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/MSU.py` & `trademasterntu-1.0.1/trademasterntu/nets/MSU.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/deeptrader.py` & `trademasterntu-1.0.1/trademasterntu/nets/deeptrader.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/dqn.py` & `trademasterntu-1.0.1/trademasterntu/nets/dqn.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 
 from .builder import NETS
 from .custom import Net
 from torch import Tensor
-from trademaster.utils import build_mlp
+from trademasterntu.utils import build_mlp
 
 @NETS.register_module()
 class QNet(Net):
     def __init__(self, dims: [int], state_dim: int, action_dim: int, explore_rate = 0.25):
         super().__init__()
         self.net = build_mlp(dims=[state_dim, *dims, action_dim])
         self.explore_rate = explore_rate
```

### Comparing `trademasterntu-0.0.1/trademaster/nets/eiie.py` & `trademasterntu-1.0.1/trademasterntu/nets/eiie.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import torch.nn as nn
 from .builder import NETS
 from .custom import Net
-from trademaster.utils import build_conv2d
+from trademasterntu.utils import build_conv2d
 from torch import Tensor
 
 @NETS.register_module()
 class EIIEConv(Net):
     def __init__(self,
                  input_dim,
                  output_dim = 1,
```

### Comparing `trademasterntu-0.0.1/trademaster/nets/eteo.py` & `trademasterntu-1.0.1/trademasterntu/nets/eteo.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/high_frequency_trading_dqn.py` & `trademasterntu-1.0.1/trademasterntu/nets/high_frequency_trading_dqn.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/investor_imitator.py` & `trademasterntu-1.0.1/trademasterntu/nets/investor_imitator.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/pd.py` & `trademasterntu-1.0.1/trademasterntu/nets/pd.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/nets/sarl.py` & `trademasterntu-1.0.1/trademasterntu/nets/sarl.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/optimizers/custom.py` & `trademasterntu-1.0.1/trademasterntu/optimizers/custom.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/preprocessor/yfinance_preprocessor/processor.py` & `trademasterntu-1.0.1/trademasterntu/preprocessor/yfinance_preprocessor/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ROOT = str(Path(__file__).resolve().parents[3])
 sys.path.append(ROOT)
 
 import os.path as osp
 from ..custom import CustomPreprocessor
 from ..builder import PREPROCESSOR
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import pandas as pd
 import os
 import yfinance as yf
 from tqdm import tqdm
 import numpy as np
 from sklearn.linear_model import LinearRegression
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/__init__.py` & `trademasterntu-1.0.1/trademasterntu/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/trainers/algorithmic_trading/trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/algorithmic_trading/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import torch
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
-from trademaster.utils import get_attr, save_model, load_model, load_best_model, save_best_model, save_best_model_trial, ReplayBuffer, GeneralReplayBuffer
+from trademasterntu.utils import get_attr, save_model, load_model, load_best_model, save_best_model, save_best_model_trial, ReplayBuffer, GeneralReplayBuffer
 import numpy as np
 import os
 import pandas as pd
 from collections import namedtuple, OrderedDict
 """the Algorithm trading DeepScalper is based on the paper  'DeepScalper: A Risk-Aware Reinforcement Learning Framework
 to Capture Fleeting Intraday Trading Opportunities'(https://arxiv.org/pdf/2201.09058.pdf)"""
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/high_frequency_trading/trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/high_frequency_trading/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import torch
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
-from trademaster.utils import get_attr, save_model,load_model, load_best_model, save_best_model, ReplayBufferHFT
+from trademasterntu.utils import get_attr, save_model,load_model, load_best_model, save_best_model, ReplayBufferHFT
 import numpy as np
 import os
 import pandas as pd
 @TRAINERS.register_module()
 class HighFrequencyTradingTrainer(Trainer):
     def __init__(self, **kwargs):
         super(HighFrequencyTradingTrainer, self).__init__()
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/order_execution/eteo_trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/order_execution/eteo_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import torch
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
 
-from trademaster.utils import get_attr, save_model, load_model, load_best_model, save_best_model, GeneralReplayBuffer
+from trademasterntu.utils import get_attr, save_model, load_model, load_best_model, save_best_model, GeneralReplayBuffer
 import numpy as np
 import os
 import pandas as pd
 from collections import OrderedDict
 
 @TRAINERS.register_module()
 class OrderExecutionETEOTrainer(Trainer):
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/order_execution/pd_trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/order_execution/pd_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from pathlib import Path
 
 import torch
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
-from trademaster.utils import get_attr
+from trademasterntu.utils import get_attr
 import numpy as np
 import os
 import pandas as pd
 import random
 from collections import OrderedDict, namedtuple
-from trademaster.utils import get_attr, save_model, load_model, load_best_model, save_best_model, ReplayBuffer, GeneralReplayBuffer
+from trademasterntu.utils import get_attr, save_model, load_model, load_best_model, save_best_model, ReplayBuffer, GeneralReplayBuffer
 
 
 @TRAINERS.register_module()
 class OrderExecutionPDTrainer(Trainer):
     def __init__(self, **kwargs):
         super(OrderExecutionPDTrainer, self).__init__()
         self.num_envs = int(get_attr(kwargs, "num_envs", 1))
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/portfolio_management/deeptrader_trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/deeptrader_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import torch
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
-from trademaster.utils import get_attr, \
+from trademasterntu.utils import get_attr, \
     save_model, save_best_model, load_model, \
     load_best_model, GeneralReplayBuffer
 import numpy as np
 import os
 import pandas as pd
 from collections import OrderedDict
 """this algorithms is based on the paper 'DeepTrader: A Deep Reinforcement Learning Approach for Risk-Return Balanced Portfolio Management with Market Conditions Embedding'
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/portfolio_management/eiie_trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/eiie_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import torch
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
-from trademaster.utils import get_attr, save_model, \
+from trademasterntu.utils import get_attr, save_model, \
     save_best_model, load_model, \
     load_best_model, GeneralReplayBuffer
 import numpy as np
 import os
 import pandas as pd
 import random
 from collections import OrderedDict
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/portfolio_management/investor_imitator_trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/investor_imitator_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import torch
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
-from trademaster.utils import get_attr, save_model, save_best_model, load_model, load_best_model
+from trademasterntu.utils import get_attr, save_model, save_best_model, load_model, load_best_model
 import os
 import pandas as pd
 import random
 import numpy as np
 from collections import OrderedDict
 
 @TRAINERS.register_module()
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/portfolio_management/sarl_trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/sarl_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 
 ROOT = Path(__file__).resolve().parents[3]
 from ..custom import Trainer
 from ..builder import TRAINERS
-from trademaster.utils import get_attr, save_object, load_object,create_radar_score_baseline, calculate_radar_score, plot_radar_chart
+from trademasterntu.utils import get_attr, save_object, load_object,create_radar_score_baseline, calculate_radar_score, plot_radar_chart
 import os
 import ray
 from ray.tune.registry import register_env
-from trademaster.environments.portfolio_management.sarl_environment import PortfolioManagementSARLEnvironment
+from trademasterntu.environments.portfolio_management.sarl_environment import PortfolioManagementSARLEnvironment
 import pandas as pd
 import numpy as np
 import random
 import torch
 
 
 def env_creator(env_name):
```

### Comparing `trademasterntu-0.0.1/trademaster/trainers/portfolio_management/trainer.py` & `trademasterntu-1.0.1/trademasterntu/trainers/portfolio_management/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 import numpy as np
 import pandas as pd
-from trademaster.environments.portfolio_management.environment import PortfolioManagementEnvironment
+from trademasterntu.environments.portfolio_management.environment import PortfolioManagementEnvironment
 from ray.tune.registry import register_env
 import ray
 import os
-from trademaster.utils import get_attr, save_object, load_object
+from trademasterntu.utils import get_attr, save_object, load_object
 from ..builder import TRAINERS
 from ..custom import Trainer
 import random
 import shutil
 from pathlib import Path
 
 ROOT = Path(__file__).resolve().parents[3]
```

### Comparing `trademasterntu-0.0.1/trademaster/transition/custom.py` & `trademasterntu-1.0.1/trademasterntu/transition/custom.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/utils/__init__.py` & `trademasterntu-1.0.1/trademasterntu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/utils/general_replay_buffer.py` & `trademasterntu-1.0.1/trademasterntu/utils/general_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/utils/labeling_util.py` & `trademasterntu-1.0.1/trademasterntu/utils/labeling_util.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/utils/layers.py` & `trademasterntu-1.0.1/trademasterntu/utils/layers.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/utils/misc.py` & `trademasterntu-1.0.1/trademasterntu/utils/misc.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/utils/replay_buffer.py` & `trademasterntu-1.0.1/trademasterntu/utils/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `trademasterntu-0.0.1/trademaster/utils/utils.py` & `trademasterntu-1.0.1/trademasterntu/utils/utils.py`

 * *Files identical despite different names*

