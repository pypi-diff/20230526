# Comparing `tmp/web3cli-1.0.1.tar.gz` & `tmp/web3cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-1.0.1.tar", last modified: Thu May 25 16:15:42 2023, max compression
+gzip compressed data, was "web3cli-1.0.2.tar", last modified: Fri May 26 15:32:22 2023, max compression
```

## Comparing `web3cli-1.0.1.tar` & `web3cli-1.0.2.tar`

### file list

```diff
@@ -1,166 +1,167 @@
--rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.0.1/LICENSE
--rw-r--r--   0        0        0    10684 2023-05-20 18:28:19.647207 web3cli-1.0.1/README.md
--rw-r--r--   0        0        0     3765 2023-05-25 16:15:08.253828 web3cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.0.1/src/web3cli/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.0.1/src/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.0.1/src/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.0.1/src/web3cli/controllers/abi_controller.py
--rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.0.1/src/web3cli/controllers/app_key_controller.py
--rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.0.1/src/web3cli/controllers/base_controller.py
--rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.0.1/src/web3cli/controllers/call_controller.py
--rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.0.1/src/web3cli/controllers/config_controller.py
--rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.0.1/src/web3cli/controllers/controller.py
--rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.0.1/src/web3cli/controllers/crud/__init__.py
--rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.0.1/src/web3cli/controllers/crud/address_controller.py
--rw-r--r--   0        0        0     4429 2023-05-20 18:17:47.040993 web3cli-1.0.1/src/web3cli/controllers/crud/chain_controller.py
--rw-r--r--   0        0        0     4795 2023-05-20 18:17:47.041550 web3cli-1.0.1/src/web3cli/controllers/crud/contract_controller.py
--rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.0.1/src/web3cli/controllers/crud/history_controller.py
--rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.0.1/src/web3cli/controllers/crud/rpc_controller.py
--rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.0.1/src/web3cli/controllers/crud/signer_controller.py
--rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.0.1/src/web3cli/controllers/db_controller.py
--rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.0.1/src/web3cli/controllers/keyfile_controller.py
--rw-r--r--   0        0        0     3717 2023-05-25 15:47:06.197106 web3cli-1.0.1/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.0.1/src/web3cli/controllers/send_controller.py
--rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.0.1/src/web3cli/controllers/swap_controller.py
--rw-r--r--   0        0        0     4125 2023-05-25 16:14:33.665697 web3cli-1.0.1/src/web3cli/controllers/token_controller.py
--rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.0.1/src/web3cli/controllers/transact_controller.py
--rw-r--r--   0        0        0     1408 2023-05-20 18:17:47.048248 web3cli-1.0.1/src/web3cli/controllers/tx_controller.py
--rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.0.1/src/web3cli/exceptions.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.0.1/src/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0    15889 2023-05-20 18:17:47.050167 web3cli-1.0.1/src/web3cli/helpers/args.py
--rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.0.1/src/web3cli/helpers/client_factory.py
--rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.0.1/src/web3cli/helpers/config.py
--rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.0.1/src/web3cli/helpers/crypto.py
--rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.0.1/src/web3cli/helpers/database.py
--rw-r--r--   0        0        0     1704 2023-05-25 16:11:59.963864 web3cli-1.0.1/src/web3cli/helpers/render.py
--rw-r--r--   0        0        0     4548 2023-05-20 18:17:47.052264 web3cli-1.0.1/src/web3cli/helpers/send.py
--rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.0.1/src/web3cli/helpers/signer.py
--rw-r--r--   0        0        0     2132 2023-04-07 18:14:01.616983 web3cli-1.0.1/src/web3cli/helpers/tx.py
--rw-r--r--   0        0        0      435 2023-05-25 16:14:58.524675 web3cli-1.0.1/src/web3cli/helpers/version.py
--rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.0.1/src/web3cli/hooks.py
--rw-r--r--   0        0        0     7036 2023-05-20 18:17:47.054261 web3cli-1.0.1/src/web3cli/main.py
--rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.0.1/src/web3cli/templates/__init__.py
--rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.0.1/src/web3cli/templates/balance.jinja2
--rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.0.1/src/web3core/__init__.py
--rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.0.1/src/web3core/constants.py
--rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.0.1/src/web3core/db.py
--rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.0.1/src/web3core/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.0.1/src/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.0.1/src/web3core/helpers/abi.py
--rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.0.1/src/web3core/helpers/blocks.py
--rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.0.1/src/web3core/helpers/client_factory.py
--rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.0.1/src/web3core/helpers/crypto.py
--rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.0.1/src/web3core/helpers/database.py
--rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.0.1/src/web3core/helpers/dex.py
--rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.0.1/src/web3core/helpers/format.py
--rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.0.1/src/web3core/helpers/misc.py
--rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.0.1/src/web3core/helpers/os.py
--rw-r--r--   0        0        0     1790 2023-04-07 18:14:01.619658 web3cli-1.0.1/src/web3core/helpers/resolve.py
--rw-r--r--   0        0        0      515 2022-12-17 18:21:46.708465 web3cli-1.0.1/src/web3core/helpers/rpc.py
--rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.0.1/src/web3core/helpers/seed.py
--rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.0.1/src/web3core/helpers/tx.py
--rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.0.1/src/web3core/helpers/validation.py
--rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.0.1/src/web3core/helpers/yaml.py
--rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.0.1/src/web3core/models/__init__.py
--rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.0.1/src/web3core/models/address.py
--rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.0.1/src/web3core/models/base_model.py
--rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.0.1/src/web3core/models/chain.py
--rw-r--r--   0        0        0     4255 2023-02-19 09:09:21.024153 web3cli-1.0.1/src/web3core/models/contract.py
--rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.0.1/src/web3core/models/signer.py
--rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.0.1/src/web3core/models/timestamps_model.py
--rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.0.1/src/web3core/models/tx.py
--rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.0.1/src/web3core/models/types.py
--rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.0.1/src/web3core/seeds/__init__.py
--rw-r--r--   0        0        0     2663 2023-04-07 18:14:01.620586 web3cli-1.0.1/src/web3core/seeds/chain_seeds.py
--rw-r--r--   0        0        0      413 2023-05-25 14:20:16.150600 web3cli-1.0.1/src/web3core/seeds/contract_seeds.py
--rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.0.1/src/web3core/seeds/contract_type_seeds.py
--rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.0.1/src/web3core/seeds/contracts/arb_contract_seeds.py
--rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.0.1/src/web3core/seeds/contracts/avax_contract_seeds.py
--rw-r--r--   0        0        0      480 2023-02-27 16:48:16.132079 web3cli-1.0.1/src/web3core/seeds/contracts/bnb_contract_seeds.py
--rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.0.1/src/web3core/seeds/contracts/era_contract_seeds.py
--rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.0.1/src/web3core/seeds/contracts/eth_contract_seeds.py
--rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.0.1/src/web3core/types.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.0.1/tests/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.0.1/tests/ape/.DS_Store
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.0.1/tests/ape/.build/Factory_IERC20.json
--rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2Callee.json
--rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2ERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2Pair.json
--rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.0.1/tests/ape/.build/Factory_Math.json
--rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.0.1/tests/ape/.build/Factory_SafeMath.json
--rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.0.1/tests/ape/.build/Factory_UQ112x112.json
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.0.1/tests/ape/.build/Router_IERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Pair.json
--rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Router01.json
--rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Router02.json
--rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.0.1/tests/ape/.build/Router_IWETH.json
--rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.0.1/tests/ape/.build/Router_SafeMath.json
--rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.0.1/tests/ape/.build/Router_TransferHelper.json
--rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.0.1/tests/ape/.build/Router_UniswapV2Library.json
--rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.0.1/tests/ape/.build/Token.json
--rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.0.1/tests/ape/.build/Token_SafeMath.json
--rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.0.1/tests/ape/.build/UniswapV2ERC20.json
--rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.0.1/tests/ape/.build/UniswapV2Factory.json
--rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.0.1/tests/ape/.build/UniswapV2Pair.json
--rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.0.1/tests/ape/.build/UniswapV2Router02.json
--rw-r--r--   0        0        0   324962 2023-05-25 16:15:13.303714 web3cli-1.0.1/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.0.1/tests/ape/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.0.1/tests/ape/contracts/.DS_Store
--rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.0.1/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.0.1/tests/ape/contracts/token/Token_SafeMath.sol
--rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.0.1/tests/ape/contracts/uniswap/.DS_Store
--rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.0.1/tests/ape/contracts/uniswap/UniswapV2Factory.sol
--rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.0.1/tests/ape/contracts/uniswap/UniswapV2Router02.sol
--rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.0.1/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.0.1/tests/ape/scripts/db.py
--rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.0.1/tests/ape/scripts/token.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.0.1/tests/ape/tests/__init__.py
--rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.0.1/tests/ape/tests/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.0.1/tests/ape/tests/helpers/__init__.py
--rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.0.1/tests/ape/tests/helpers/ape.py
--rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.0.1/tests/ape/tests/helpers/token.py
--rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.0.1/tests/ape/tests/helpers/uniswap.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.0.1/tests/ape/tests/token/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.0.1/tests/ape/tests/token/test_token_approve.py
--rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.0.1/tests/ape/tests/token/test_token_transfer.py
--rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.0.1/tests/ape/tests/token/test_token_transferFrom.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.0.1/tests/ape/tests/uniswap/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.0.1/tests/ape/tests/uniswap/test_v2_add_liquidity.py
--rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.0.1/tests/ape/tests/uniswap/test_v2_create_pair.py
--rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.0.1/tests/helper.py
--rw-r--r--   0        0        0     3240 2023-04-07 18:14:01.629815 web3cli-1.0.1/tests/seed.py
--rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.0.1/tests/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.0.1/tests/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.0.1/tests/web3cli/controllers/crud/test_address_controller.py
--rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.0.1/tests/web3cli/controllers/crud/test_chain_controller.py
--rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.0.1/tests/web3cli/controllers/crud/test_contract_controller.py
--rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.0.1/tests/web3cli/controllers/crud/test_history_controller.py
--rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.0.1/tests/web3cli/controllers/crud/test_rpc_controller.py
--rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.0.1/tests/web3cli/controllers/crud/test_signer_controller.py
--rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.0.1/tests/web3cli/controllers/test_appkey_controller.py
--rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.0.1/tests/web3cli/controllers/test_call_controller.py
--rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.0.1/tests/web3cli/controllers/test_db_controller.py
--rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.0.1/tests/web3cli/controllers/test_keyfile_controller.py
--rw-r--r--   0        0        0     5688 2023-05-20 18:17:47.062163 web3cli-1.0.1/tests/web3cli/controllers/test_misc_controller.py
--rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.0.1/tests/web3cli/controllers/test_send_controller.py
--rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.0.1/tests/web3cli/controllers/test_transact_controller.py
--rw-r--r--   0        0        0     1265 2023-04-07 18:14:01.631776 web3cli-1.0.1/tests/web3cli/controllers/test_tx_controller.py
--rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.0.1/tests/web3cli/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.0.1/tests/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.0.1/tests/web3cli/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.0.1/tests/web3cli/main.py
--rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.0.1/tests/web3cli/test_db.py
--rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.0.1/tests/web3cli/test_main.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.0.1/tests/web3core/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.0.1/tests/web3core/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.0.1/tests/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.0.1/tests/web3core/helpers/test_abi_helper.py
--rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.0.1/tests/web3core/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.0.1/tests/web3core/helpers/test_resolve_address_helper.py
--rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.0.1/tests/web3core/helpers/test_validation_helper.py
--rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.0.1/tests/web3core/models/test_contract_model.py
--rw-r--r--   0        0        0    11141 1970-01-01 00:00:00.000000 web3cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.0.2/LICENSE
+-rw-r--r--   0        0        0    10697 2023-05-26 15:28:32.491886 web3cli-1.0.2/README.md
+-rw-r--r--   0        0        0     3891 2023-05-26 15:32:09.292024 web3cli-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.0.2/src/web3cli/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.0.2/src/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.0.2/src/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     4699 2023-05-20 18:26:40.921508 web3cli-1.0.2/src/web3cli/controllers/abi_controller.py
+-rw-r--r--   0        0        0     2005 2023-05-17 11:19:52.195517 web3cli-1.0.2/src/web3cli/controllers/app_key_controller.py
+-rw-r--r--   0        0        0     1171 2023-05-20 18:17:47.037441 web3cli-1.0.2/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0        0        0     3116 2023-05-20 18:17:47.038161 web3cli-1.0.2/src/web3cli/controllers/call_controller.py
+-rw-r--r--   0        0        0     2372 2023-05-20 18:17:47.039146 web3cli-1.0.2/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.0.2/src/web3cli/controllers/controller.py
+-rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.0.2/src/web3cli/controllers/crud/__init__.py
+-rw-r--r--   0        0        0     2540 2023-05-20 18:17:47.040161 web3cli-1.0.2/src/web3cli/controllers/crud/address_controller.py
+-rw-r--r--   0        0        0     4421 2023-05-26 15:30:25.886766 web3cli-1.0.2/src/web3cli/controllers/crud/chain_controller.py
+-rw-r--r--   0        0        0     4795 2023-05-20 18:17:47.041550 web3cli-1.0.2/src/web3cli/controllers/crud/contract_controller.py
+-rw-r--r--   0        0        0     3052 2023-05-20 18:17:47.042307 web3cli-1.0.2/src/web3cli/controllers/crud/history_controller.py
+-rw-r--r--   0        0        0     2958 2023-05-20 18:17:47.043048 web3cli-1.0.2/src/web3cli/controllers/crud/rpc_controller.py
+-rw-r--r--   0        0        0     5286 2023-05-20 18:17:47.043661 web3cli-1.0.2/src/web3cli/controllers/crud/signer_controller.py
+-rw-r--r--   0        0        0     1346 2023-04-30 17:34:17.185968 web3cli-1.0.2/src/web3cli/controllers/db_controller.py
+-rw-r--r--   0        0        0     1433 2023-05-18 10:41:28.547083 web3cli-1.0.2/src/web3cli/controllers/keyfile_controller.py
+-rw-r--r--   0        0        0     3717 2023-05-25 15:47:06.197106 web3cli-1.0.2/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0        0        0     2359 2023-05-20 18:17:47.045353 web3cli-1.0.2/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.0.2/src/web3cli/controllers/swap_controller.py
+-rw-r--r--   0        0        0     4125 2023-05-25 16:14:33.665697 web3cli-1.0.2/src/web3cli/controllers/token_controller.py
+-rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.0.2/src/web3cli/controllers/transact_controller.py
+-rw-r--r--   0        0        0     1408 2023-05-20 18:17:47.048248 web3cli-1.0.2/src/web3cli/controllers/tx_controller.py
+-rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.0.2/src/web3cli/exceptions.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.0.2/src/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0    15889 2023-05-20 18:17:47.050167 web3cli-1.0.2/src/web3cli/helpers/args.py
+-rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.0.2/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.0.2/src/web3cli/helpers/config.py
+-rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.0.2/src/web3cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.0.2/src/web3cli/helpers/database.py
+-rw-r--r--   0        0        0     1704 2023-05-25 16:11:59.963864 web3cli-1.0.2/src/web3cli/helpers/render.py
+-rw-r--r--   0        0        0     4548 2023-05-20 18:17:47.052264 web3cli-1.0.2/src/web3cli/helpers/send.py
+-rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.0.2/src/web3cli/helpers/signer.py
+-rw-r--r--   0        0        0     2132 2023-04-07 18:14:01.616983 web3cli-1.0.2/src/web3cli/helpers/tx.py
+-rw-r--r--   0        0        0      435 2023-05-26 15:31:50.780055 web3cli-1.0.2/src/web3cli/helpers/version.py
+-rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.0.2/src/web3cli/hooks.py
+-rw-r--r--   0        0        0     7124 2023-05-26 15:21:32.365497 web3cli-1.0.2/src/web3cli/main.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.0.2/src/web3cli/templates/__init__.py
+-rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.0.2/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.0.2/src/web3core/__init__.py
+-rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.0.2/src/web3core/constants.py
+-rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.0.2/src/web3core/db.py
+-rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.0.2/src/web3core/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.0.2/src/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.0.2/src/web3core/helpers/abi.py
+-rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.0.2/src/web3core/helpers/blocks.py
+-rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.0.2/src/web3core/helpers/client_factory.py
+-rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.0.2/src/web3core/helpers/crypto.py
+-rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.0.2/src/web3core/helpers/database.py
+-rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.0.2/src/web3core/helpers/dex.py
+-rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.0.2/src/web3core/helpers/format.py
+-rw-r--r--   0        0        0     2413 2023-05-18 08:42:25.689036 web3cli-1.0.2/src/web3core/helpers/misc.py
+-rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.0.2/src/web3core/helpers/os.py
+-rw-r--r--   0        0        0     1790 2023-04-07 18:14:01.619658 web3cli-1.0.2/src/web3core/helpers/resolve.py
+-rw-r--r--   0        0        0      515 2022-12-17 18:21:46.708465 web3cli-1.0.2/src/web3core/helpers/rpc.py
+-rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.0.2/src/web3core/helpers/seed.py
+-rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.0.2/src/web3core/helpers/tx.py
+-rw-r--r--   0        0        0      345 2023-01-29 18:12:45.184768 web3cli-1.0.2/src/web3core/helpers/validation.py
+-rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.0.2/src/web3core/helpers/yaml.py
+-rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.0.2/src/web3core/models/__init__.py
+-rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.0.2/src/web3core/models/address.py
+-rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.0.2/src/web3core/models/base_model.py
+-rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.0.2/src/web3core/models/chain.py
+-rw-r--r--   0        0        0     4255 2023-02-19 09:09:21.024153 web3cli-1.0.2/src/web3core/models/contract.py
+-rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.0.2/src/web3core/models/signer.py
+-rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.0.2/src/web3core/models/timestamps_model.py
+-rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.0.2/src/web3core/models/tx.py
+-rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.0.2/src/web3core/models/types.py
+-rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.0.2/src/web3core/seeds/__init__.py
+-rw-r--r--   0        0        0     3071 2023-05-26 15:12:06.303278 web3cli-1.0.2/src/web3core/seeds/chain_seeds.py
+-rw-r--r--   0        0        0      466 2023-05-26 15:26:11.248665 web3cli-1.0.2/src/web3core/seeds/contract_seeds.py
+-rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.0.2/src/web3core/seeds/contract_type_seeds.py
+-rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.0.2/src/web3core/seeds/contracts/arb_contract_seeds.py
+-rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.0.2/src/web3core/seeds/contracts/avax_contract_seeds.py
+-rw-r--r--   0        0        0      480 2023-02-27 16:48:16.132079 web3cli-1.0.2/src/web3core/seeds/contracts/bnb_contract_seeds.py
+-rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.0.2/src/web3core/seeds/contracts/era_contract_seeds.py
+-rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.0.2/src/web3core/seeds/contracts/eth_contract_seeds.py
+-rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.0.2/src/web3core/seeds/contracts/gno_contract_seeds.py
+-rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.0.2/src/web3core/types.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:46.901853 web3cli-1.0.2/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.0.2/tests/ape/.DS_Store
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.0.2/tests/ape/.build/Factory_IERC20.json
+-rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2Callee.json
+-rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2Pair.json
+-rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.0.2/tests/ape/.build/Factory_Math.json
+-rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.0.2/tests/ape/.build/Factory_SafeMath.json
+-rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.0.2/tests/ape/.build/Factory_UQ112x112.json
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.0.2/tests/ape/.build/Router_IERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Pair.json
+-rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Router01.json
+-rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Router02.json
+-rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.0.2/tests/ape/.build/Router_IWETH.json
+-rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.0.2/tests/ape/.build/Router_SafeMath.json
+-rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.0.2/tests/ape/.build/Router_TransferHelper.json
+-rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.0.2/tests/ape/.build/Router_UniswapV2Library.json
+-rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.0.2/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.0.2/tests/ape/.build/Token_SafeMath.json
+-rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.0.2/tests/ape/.build/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.0.2/tests/ape/.build/UniswapV2Factory.json
+-rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.0.2/tests/ape/.build/UniswapV2Pair.json
+-rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.0.2/tests/ape/.build/UniswapV2Router02.json
+-rw-r--r--   0        0        0   324962 2023-05-26 15:32:15.032666 web3cli-1.0.2/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.0.2/tests/ape/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.0.2/tests/ape/contracts/.DS_Store
+-rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.0.2/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.0.2/tests/ape/contracts/token/Token_SafeMath.sol
+-rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.0.2/tests/ape/contracts/uniswap/.DS_Store
+-rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.0.2/tests/ape/contracts/uniswap/UniswapV2Factory.sol
+-rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.0.2/tests/ape/contracts/uniswap/UniswapV2Router02.sol
+-rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.0.2/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.0.2/tests/ape/scripts/db.py
+-rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.0.2/tests/ape/scripts/token.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.0.2/tests/ape/tests/__init__.py
+-rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.0.2/tests/ape/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.0.2/tests/ape/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.0.2/tests/ape/tests/helpers/ape.py
+-rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.0.2/tests/ape/tests/helpers/token.py
+-rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.0.2/tests/ape/tests/helpers/uniswap.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.0.2/tests/ape/tests/token/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.0.2/tests/ape/tests/token/test_token_approve.py
+-rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.0.2/tests/ape/tests/token/test_token_transfer.py
+-rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.0.2/tests/ape/tests/token/test_token_transferFrom.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.0.2/tests/ape/tests/uniswap/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.0.2/tests/ape/tests/uniswap/test_v2_add_liquidity.py
+-rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.0.2/tests/ape/tests/uniswap/test_v2_create_pair.py
+-rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.0.2/tests/helper.py
+-rw-r--r--   0        0        0     3240 2023-04-07 18:14:01.629815 web3cli-1.0.2/tests/seed.py
+-rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.0.2/tests/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.0.2/tests/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.0.2/tests/web3cli/controllers/crud/test_address_controller.py
+-rw-r--r--   0        0        0     3517 2023-05-20 18:17:47.057300 web3cli-1.0.2/tests/web3cli/controllers/crud/test_chain_controller.py
+-rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.0.2/tests/web3cli/controllers/crud/test_contract_controller.py
+-rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.0.2/tests/web3cli/controllers/crud/test_history_controller.py
+-rw-r--r--   0        0        0     3762 2023-05-20 18:17:47.059822 web3cli-1.0.2/tests/web3cli/controllers/crud/test_rpc_controller.py
+-rw-r--r--   0        0        0     4933 2023-05-20 18:17:47.060483 web3cli-1.0.2/tests/web3cli/controllers/crud/test_signer_controller.py
+-rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.0.2/tests/web3cli/controllers/test_appkey_controller.py
+-rw-r--r--   0        0        0     6339 2023-05-20 18:17:47.061301 web3cli-1.0.2/tests/web3cli/controllers/test_call_controller.py
+-rw-r--r--   0        0        0     1041 2023-03-25 21:24:05.581746 web3cli-1.0.2/tests/web3cli/controllers/test_db_controller.py
+-rw-r--r--   0        0        0     1702 2023-05-18 11:14:40.025134 web3cli-1.0.2/tests/web3cli/controllers/test_keyfile_controller.py
+-rw-r--r--   0        0        0     5688 2023-05-20 18:17:47.062163 web3cli-1.0.2/tests/web3cli/controllers/test_misc_controller.py
+-rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.0.2/tests/web3cli/controllers/test_send_controller.py
+-rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.0.2/tests/web3cli/controllers/test_transact_controller.py
+-rw-r--r--   0        0        0     1265 2023-04-07 18:14:01.631776 web3cli-1.0.2/tests/web3cli/controllers/test_tx_controller.py
+-rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.0.2/tests/web3cli/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.0.2/tests/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.0.2/tests/web3cli/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.0.2/tests/web3cli/main.py
+-rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.0.2/tests/web3cli/test_db.py
+-rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.0.2/tests/web3cli/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.0.2/tests/web3core/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.0.2/tests/web3core/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.0.2/tests/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.0.2/tests/web3core/helpers/test_abi_helper.py
+-rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.0.2/tests/web3core/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.0.2/tests/web3core/helpers/test_resolve_address_helper.py
+-rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.0.2/tests/web3core/helpers/test_validation_helper.py
+-rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.0.2/tests/web3core/models/test_contract_model.py
+-rw-r--r--   0        0        0    11154 1970-01-01 00:00:00.000000 web3cli-1.0.2/PKG-INFO
```

### Comparing `web3cli-1.0.1/LICENSE` & `web3cli-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/README.md` & `web3cli-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 You can also do more complex stuff like:
 
 ```bash
 # get the amount of USDT you get for 100 USDC
 w3 call uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' 
 ```
 
-### Write to a smart contract
+### Send a transaction to a smart contract
 
 To write to the blockchain, use `w3 transact`. For example, to transfer 1 ETH to 
 address, run:
 
 ```
 w3 transact weth transfer <address> 1e18
 ```
```

#### html2text {}

```diff
@@ -54,10 +54,10 @@
 w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
 functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
 smart contract, use `w3 call`. For example, to get the total supply of the WETH
 token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
 automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
-uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Write to a
-smart contract To write to the blockchain, use `w3 transact`. For example, to
-transfer 1 ETH to address, run: ``` w3 transact weth transfer
+uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
+transaction to a smart contract To write to the blockchain, use `w3 transact`.
+For example, to transfer 1 ETH to address, run: ``` w3 transact weth transfer
```

### Comparing `web3cli-1.0.1/pyproject.toml` & `web3cli-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3cli"
-version = "1.0.1"
+version = "1.0.2"
 description = "Interact with blockchains and smart contracts using the command line"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
@@ -40,14 +40,15 @@
 w3eth = "web3cli.main:w3eth"
 w3bnb = "web3cli.main:w3bnb"
 w3avax = "web3cli.main:w3avax"
 w3matic = "web3cli.main:w3matic"
 w3cro = "web3cli.main:w3cro"
 w3arb = "web3cli.main:w3arb"
 w3era = "web3cli.main:w3era"
+w3gno = "web3cli.main:w3gno"
 
 [project.urls]
 homepage = "https://github.com/coccoinomane/web3cli"
 repository = "https://github.com/coccoinomane/web3cli"
 
 [tool.pdm.dev-dependencies]
 dev = [
@@ -97,14 +98,18 @@
 cmd = "w3arb"
 help = "Run the CLI in dev mode, on Arbitrum One chain"
 
 [tool.pdm.scripts.w3era]
 cmd = "w3era"
 help = "Run the CLI in dev mode, on zkSync Era chain"
 
+[tool.pdm.scripts.w3gno]
+cmd = "w3gno"
+help = "Run the CLI in dev mode, on Gnosis (xDAI) chain"
+
 [tool.pdm.build]
 includes = [
     "src",
 ]
 
 [tool.black]
 line-length = 88
```

### Comparing `web3cli-1.0.1/src/web3cli/.DS_Store` & `web3cli-1.0.2/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/abi_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/abi_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/app_key_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/app_key_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/base_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/call_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/config_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/config_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/controller.py` & `web3cli-1.0.2/src/web3cli/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/crud/address_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/crud/address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/crud/chain_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/crud/chain_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         chain = Chain.get_by_name(self.app.pargs.name)
         if not chain or self.app.pargs.update:
             chain = Chain.upsert(
                 {
                     "name": self.app.pargs.name,
                     "desc": self.app.pargs.desc,
                     "chain_id": self.app.pargs.chain_id,
-                    "coin": self.app.pargs.coin.upper(),
+                    "coin": self.app.pargs.coin,
                     "tx_type": self.app.pargs.tx_type,
                     "middlewares": None
                     if self.app.pargs.poa
                     else "geth_poa_middleware",
                 },
                 logger=self.app.log.info,
             )
```

### Comparing `web3cli-1.0.1/src/web3cli/controllers/crud/contract_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/crud/contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/crud/history_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/crud/history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/crud/rpc_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/crud/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/crud/signer_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/crud/signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/db_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/keyfile_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/misc_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/send_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/swap_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/swap_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/token_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/token_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/transact_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/controllers/tx_controller.py` & `web3cli-1.0.2/src/web3cli/controllers/tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/args.py` & `web3cli-1.0.2/src/web3cli/helpers/args.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/client_factory.py` & `web3cli-1.0.2/src/web3cli/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/config.py` & `web3cli-1.0.2/src/web3cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/crypto.py` & `web3cli-1.0.2/src/web3cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/database.py` & `web3cli-1.0.2/src/web3cli/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/render.py` & `web3cli-1.0.2/src/web3cli/helpers/render.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/send.py` & `web3cli-1.0.2/src/web3cli/helpers/send.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/signer.py` & `web3cli-1.0.2/src/web3cli/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/helpers/tx.py` & `web3cli-1.0.2/src/web3cli/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/hooks.py` & `web3cli-1.0.2/src/web3cli/hooks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3cli/main.py` & `web3cli-1.0.2/src/web3cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,39 +186,44 @@
 
 
 if __name__ == "__main__":
     main()
 
 
 def w3eth() -> None:
-    """Shorthand command w3eth that uses eth chain"""
+    """Shorthand command to use ethereum chain"""
     main(lambda a: override_arg(a, "chain", "eth"))
 
 
 def w3bnb() -> None:
-    """Shorthand command that uses bnb chain"""
+    """Shorthand command to use binance chain"""
     main(lambda a: override_arg(a, "chain", "bnb"))
 
 
 def w3avax() -> None:
-    """Shorthand command w3eth that uses avax chain"""
+    """Shorthand command to use avalanche chain"""
     main(lambda a: override_arg(a, "chain", "avax"))
 
 
 def w3matic() -> None:
-    """Shorthand command w3eth that uses matic chain"""
+    """Shorthand command to use matic chain"""
     main(lambda a: override_arg(a, "chain", "matic"))
 
 
 def w3cro() -> None:
-    """Shorthand command w3eth that uses cro chain"""
+    """Shorthand command to use cronos chain"""
     main(lambda a: override_arg(a, "chain", "cro"))
 
 
 def w3arb() -> None:
-    """Shorthand command w3eth that uses arb chain"""
+    """Shorthand command to use arbitrum chain"""
     main(lambda a: override_arg(a, "chain", "arb"))
 
 
 def w3era() -> None:
-    """Shorthand command w3eth that uses zkSync Era chain"""
+    """Shorthand command to use zkSync Era chain"""
     main(lambda a: override_arg(a, "chain", "era"))
+
+
+def w3gno() -> None:
+    """Shorthand command to use gnosis chain"""
+    main(lambda a: override_arg(a, "chain", "gno"))
```

### Comparing `web3cli-1.0.1/src/web3core/exceptions.py` & `web3cli-1.0.2/src/web3core/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/abi.py` & `web3cli-1.0.2/src/web3core/helpers/abi.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/blocks.py` & `web3cli-1.0.2/src/web3core/helpers/blocks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/client_factory.py` & `web3cli-1.0.2/src/web3core/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/crypto.py` & `web3cli-1.0.2/src/web3core/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/database.py` & `web3cli-1.0.2/src/web3core/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/dex.py` & `web3cli-1.0.2/src/web3core/helpers/dex.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/misc.py` & `web3cli-1.0.2/src/web3core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/os.py` & `web3cli-1.0.2/src/web3core/helpers/os.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/resolve.py` & `web3cli-1.0.2/src/web3core/helpers/resolve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/rpc.py` & `web3cli-1.0.2/src/web3core/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/seed.py` & `web3cli-1.0.2/src/web3core/helpers/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/tx.py` & `web3cli-1.0.2/src/web3core/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/helpers/yaml.py` & `web3cli-1.0.2/src/web3core/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/address.py` & `web3cli-1.0.2/src/web3core/models/address.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/base_model.py` & `web3cli-1.0.2/src/web3core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/chain.py` & `web3cli-1.0.2/src/web3core/models/chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/contract.py` & `web3cli-1.0.2/src/web3core/models/contract.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/signer.py` & `web3cli-1.0.2/src/web3core/models/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/timestamps_model.py` & `web3cli-1.0.2/src/web3core/models/timestamps_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/tx.py` & `web3cli-1.0.2/src/web3core/models/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/models/types.py` & `web3cli-1.0.2/src/web3core/models/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/seeds/chain_seeds.py` & `web3cli-1.0.2/src/web3core/seeds/chain_seeds.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,14 +103,35 @@
     "rpcs": [
         {
             "url": "https://mainnet.era.zksync.io",
         },
     ],
 }
 
+# Gnosis chain
+gno: ChainFields = {
+    "name": "gno",
+    "desc": "Gnosis",
+    "chain_id": 100,
+    "coin": "xDAI",
+    "tx_type": 2,
+    "middlewares": "",
+    "rpcs": [
+        {
+            "url": "https://rpc.gnosischain.com/",
+        },
+        {
+            "url": "https://rpc.gnosis.gateway.fm",
+        },
+        {
+            "url": "https://rpc.ankr.com/gnosis",
+        },
+    ],
+}
+
 
 # Ganache local chain
 ganache: ChainFields = {
     "name": "ganache",
     "desc": "Ganache local chain",
     "chain_id": 1337,
     "coin": "ETH",
@@ -142,10 +163,11 @@
     eth,
     bnb,
     avax,
     matic,
     cro,
     arb,
     era,
+    gno,
     ganache,
     anvil,
 ]
```

### Comparing `web3cli-1.0.1/src/web3core/seeds/contract_type_seeds.py` & `web3cli-1.0.2/src/web3core/seeds/contract_type_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/seeds/contracts/arb_contract_seeds.py` & `web3cli-1.0.2/src/web3core/seeds/contracts/arb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/seeds/contracts/avax_contract_seeds.py` & `web3cli-1.0.2/src/web3core/seeds/contracts/avax_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/seeds/contracts/era_contract_seeds.py` & `web3cli-1.0.2/src/web3core/seeds/contracts/era_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/seeds/contracts/eth_contract_seeds.py` & `web3cli-1.0.2/src/web3core/seeds/contracts/eth_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/src/web3core/types.py` & `web3cli-1.0.2/src/web3core/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/.DS_Store` & `web3cli-1.0.2/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.DS_Store` & `web3cli-1.0.2/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_IERC20.json` & `web3cli-1.0.2/tests/ape/.build/Factory_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2Callee.json` & `web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2Callee.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2ERC20.json` & `web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2Factory.json` & `web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_IUniswapV2Pair.json` & `web3cli-1.0.2/tests/ape/.build/Factory_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_Math.json` & `web3cli-1.0.2/tests/ape/.build/Factory_Math.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_SafeMath.json` & `web3cli-1.0.2/tests/ape/.build/Factory_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Factory_UQ112x112.json` & `web3cli-1.0.2/tests/ape/.build/Factory_UQ112x112.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_IERC20.json` & `web3cli-1.0.2/tests/ape/.build/Router_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Factory.json` & `web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Pair.json` & `web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Router01.json` & `web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Router01.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_IUniswapV2Router02.json` & `web3cli-1.0.2/tests/ape/.build/Router_IUniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_IWETH.json` & `web3cli-1.0.2/tests/ape/.build/Router_IWETH.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_SafeMath.json` & `web3cli-1.0.2/tests/ape/.build/Router_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_TransferHelper.json` & `web3cli-1.0.2/tests/ape/.build/Router_TransferHelper.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Router_UniswapV2Library.json` & `web3cli-1.0.2/tests/ape/.build/Router_UniswapV2Library.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Token.json` & `web3cli-1.0.2/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/Token_SafeMath.json` & `web3cli-1.0.2/tests/ape/.build/Token_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/UniswapV2ERC20.json` & `web3cli-1.0.2/tests/ape/.build/UniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/UniswapV2Factory.json` & `web3cli-1.0.2/tests/ape/.build/UniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/UniswapV2Pair.json` & `web3cli-1.0.2/tests/ape/.build/UniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/UniswapV2Router02.json` & `web3cli-1.0.2/tests/ape/.build/UniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/.build/__local__.json` & `web3cli-1.0.2/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/contracts/.DS_Store` & `web3cli-1.0.2/tests/ape/contracts/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/contracts/token/Token.sol` & `web3cli-1.0.2/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/contracts/token/Token_SafeMath.sol` & `web3cli-1.0.2/tests/ape/contracts/token/Token_SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/contracts/uniswap/.DS_Store` & `web3cli-1.0.2/tests/ape/contracts/uniswap/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/contracts/uniswap/UniswapV2Factory.sol` & `web3cli-1.0.2/tests/ape/contracts/uniswap/UniswapV2Factory.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/contracts/uniswap/UniswapV2Router02.sol` & `web3cli-1.0.2/tests/ape/contracts/uniswap/UniswapV2Router02.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/fixtures.py` & `web3cli-1.0.2/tests/ape/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/helpers/token.py` & `web3cli-1.0.2/tests/ape/tests/helpers/token.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/helpers/uniswap.py` & `web3cli-1.0.2/tests/ape/tests/helpers/uniswap.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/token/test_token_approve.py` & `web3cli-1.0.2/tests/ape/tests/token/test_token_approve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/token/test_token_transfer.py` & `web3cli-1.0.2/tests/ape/tests/token/test_token_transfer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/token/test_token_transferFrom.py` & `web3cli-1.0.2/tests/ape/tests/token/test_token_transferFrom.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/uniswap/test_v2_add_liquidity.py` & `web3cli-1.0.2/tests/ape/tests/uniswap/test_v2_add_liquidity.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/ape/tests/uniswap/test_v2_create_pair.py` & `web3cli-1.0.2/tests/ape/tests/uniswap/test_v2_create_pair.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/helper.py` & `web3cli-1.0.2/tests/helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/seed.py` & `web3cli-1.0.2/tests/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/crud/test_address_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/crud/test_address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/crud/test_chain_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/crud/test_chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/crud/test_contract_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/crud/test_contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/crud/test_history_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/crud/test_history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/crud/test_rpc_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/crud/test_rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/crud/test_signer_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/crud/test_signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_appkey_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_appkey_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_call_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_db_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_keyfile_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_misc_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_send_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_transact_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/controllers/test_tx_controller.py` & `web3cli-1.0.2/tests/web3cli/controllers/test_tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/fixtures.py` & `web3cli-1.0.2/tests/web3cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/helpers/test_crypto_helper.py` & `web3cli-1.0.2/tests/web3cli/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/main.py` & `web3cli-1.0.2/tests/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3cli/test_db.py` & `web3cli-1.0.2/tests/web3cli/test_db.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3core/fixtures.py` & `web3cli-1.0.2/tests/web3core/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3core/helpers/test_abi_helper.py` & `web3cli-1.0.2/tests/web3core/helpers/test_abi_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3core/helpers/test_crypto_helper.py` & `web3cli-1.0.2/tests/web3core/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3core/helpers/test_resolve_address_helper.py` & `web3cli-1.0.2/tests/web3core/helpers/test_resolve_address_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3core/helpers/test_validation_helper.py` & `web3cli-1.0.2/tests/web3core/helpers/test_validation_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/tests/web3core/models/test_contract_model.py` & `web3cli-1.0.2/tests/web3core/models/test_contract_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.0.1/PKG-INFO` & `web3cli-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: Interact with blockchains and smart contracts using the command line
 License: MIT
 Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3cli
 Project-URL: repository, https://github.com/coccoinomane/web3cli
@@ -170,15 +170,15 @@
 You can also do more complex stuff like:
 
 ```bash
 # get the amount of USDT you get for 100 USDC
 w3 call uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' 
 ```
 
-### Write to a smart contract
+### Send a transaction to a smart contract
 
 To write to the blockchain, use `w3 transact`. For example, to transfer 1 ETH to 
 address, run:
 
 ```
 w3 transact weth transfer <address> 1e18
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: web3cli Version: 1.0.1 Summary: Interact with
+Metadata-Version: 2.1 Name: web3cli Version: 1.0.2 Summary: Interact with
 blockchains and smart contracts using the command line License: MIT Keywords:
 web3,w3,cli,evm,blockchain,ethereum,binance,avalanche Author-email:
 coccoinomane
 gmail.com> Requires-Python: >=3.9,<3.11 Project-URL: homepage, https://
 github.com/coccoinomane/web3cli Project-URL: repository, https://github.com/
 coccoinomane/web3cli Description-Content-Type: text/markdown
 [https://img.shields.io/github/commit-activity/m/badges/shields?color=009051]
@@ -61,10 +61,10 @@
 w3 abi evs uniswap_v2 # events on Uniswap V2 w3 abi fns --abi abi.json #
 functions of an arbitrary ABI ``` ### Read from a smart contract To read from a
 smart contract, use `w3 call`. For example, to get the total supply of the WETH
 token, run: ``` w3 call weth totalSupply ``` Function arguments are parsed
 automatically, so you can call `balanceOf` with: ``` w3 call weth balanceOf
 0xA59B29d7dbC9794d1e7f45123C48b2b8d0a34636 ``` You can also do more complex
 stuff like: ```bash # get the amount of USDT you get for 100 USDC w3 call
-uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Write to a
-smart contract To write to the blockchain, use `w3 transact`. For example, to
-transfer 1 ETH to address, run: ``` w3 transact weth transfer
+uniswap_v2 getAmountsOut 100e6 usdc,usdt | jq -r '.[1]' ``` ### Send a
+transaction to a smart contract To write to the blockchain, use `w3 transact`.
+For example, to transfer 1 ETH to address, run: ``` w3 transact weth transfer
```

