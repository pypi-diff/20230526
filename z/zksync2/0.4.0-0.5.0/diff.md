# Comparing `tmp/zksync2-0.4.0.tar.gz` & `tmp/zksync2-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zksync2-0.4.0.tar", last modified: Sun Apr  2 15:48:17 2023, max compression
+gzip compressed data, was "zksync2-0.5.0.tar", last modified: Fri May 26 13:16:39 2023, max compression
```

## Comparing `zksync2-0.4.0.tar` & `zksync2-0.5.0.tar`

### file list

```diff
@@ -1,99 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.288076 zksync2-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.276075 zksync2-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.276075 zksync2-0.4.0/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-04-02 15:47:58.000000 zksync2-0.4.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-02 15:47:58.000000 zksync2-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-02 15:47:58.000000 zksync2-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16255 2023-04-02 15:48:17.288076 zksync2-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-02 15:47:58.000000 zksync2-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.280075 zksync2-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/01_deposit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/02_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/03_transfer_erc20_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/04_deploy_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/05_deploy_create_with_ctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/06_deploy_create_with_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/07_deploy_create2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/08_deploy_create2_deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/09_execute_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/10_execute_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/11_withdrawal.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-02 15:47:58.000000 zksync2-0.4.0/examples/12_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-02 15:47:58.000000 zksync2-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-02 15:47:58.000000 zksync2-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-02 15:48:17.288076 zksync2-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-02 15:47:58.000000 zksync2-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.280075 zksync2-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.280075 zksync2-0.4.0/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/Counter.json
--rw-r--r--   0 runner    (1001) docker     (123)   103076 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/CustomAccount.json
--rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/CustomPaymaster.json
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/Foo.json
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/Import.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/SimpleConstructor.json
--rw-r--r--   0 runner    (1001) docker     (123)    50646 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/SomeERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/contracts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_contract_deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_eip712_structed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_eth_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_eth_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_paymaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_transaction712.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_zksync_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)    42387 2023-04-02 15:47:58.000000 zksync2-0.4.0/tests/test_zksync_web3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.280075 zksync2-0.4.0/zksync2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.284076 zksync2-0.4.0/zksync2/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.284076 zksync2-0.4.0/zksync2/manage_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.284076 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IEthToken.json
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/INonceHolder.json
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json
--rw-r--r--   0 runner    (1001) docker     (123)    52473 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IZkSync.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_abi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/contract_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/deploy_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/erc20_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/eth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/l1_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/l2_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/nonce_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/paymaster_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/precompute_contract_deployer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/manage_contracts/zksync_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.284076 zksync2-0.4.0/zksync2/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/module/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/module/module_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/module/request_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/module/response_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/module/zksync_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/module/zksync_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.284076 zksync2-0.4.0/zksync2/provider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/provider/eth_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.288076 zksync2-0.4.0/zksync2/signer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/signer/eth_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.288076 zksync2-0.4.0/zksync2/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/transaction/transaction712.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-02 15:47:58.000000 zksync2-0.4.0/zksync2/transaction/transaction_builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 15:48:17.280075 zksync2-0.4.0/zksync2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16255 2023-04-02 15:48:17.000000 zksync2-0.4.0/zksync2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-02 15:48:17.000000 zksync2-0.4.0/zksync2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 15:48:17.000000 zksync2-0.4.0/zksync2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-02 15:48:17.000000 zksync2-0.4.0/zksync2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-02 15:48:17.000000 zksync2-0.4.0/zksync2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.838590 zksync2-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.802590 zksync2-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.810590 zksync2-0.5.0/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-05-26 13:16:23.000000 zksync2-0.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-26 13:16:23.000000 zksync2-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 13:16:23.000000 zksync2-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-26 13:16:39.838590 zksync2-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15696 2023-05-26 13:16:23.000000 zksync2-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/01_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/02_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/03_transfer_erc20_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/04_deploy_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/05_deploy_create_with_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/06_deploy_create_with_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/07_deploy_create2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/08_deploy_create2_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/09_withdrawal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/10_finalize_withdrawal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/11_check_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.806590 zksync2-0.5.0/examples/solidity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/demo/Demo.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/demo/Foo.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/demo/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/demo/build/combined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/incrementer/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/incrementer/Incrementer.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.814590 zksync2-0.5.0/examples/solidity/incrementer/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/incrementer/build/combined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/examples/solidity/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/storage/Storage.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/examples/solidity/storage/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/solidity/storage/build/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 13:16:23.000000 zksync2-0.5.0/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-26 13:16:23.000000 zksync2-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 13:16:23.000000 zksync2-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 13:16:39.838590 zksync2-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 13:16:23.000000 zksync2-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.818590 zksync2-0.5.0/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/Counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103076 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/CustomAccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48494 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/CustomPaymaster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/Foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/Import.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/SimpleConstructor.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50646 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/SomeERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/contracts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.822590 zksync2-0.5.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_deposit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_paymaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_withdraw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_zksync_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42460 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/integration/test_zksync_web3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.822590 zksync2-0.5.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_contract_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_eth_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-26 13:16:23.000000 zksync2-0.5.0/tests/unit/test_transaction712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.822590 zksync2-0.5.0/zksync2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.826590 zksync2-0.5.0/zksync2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.830590 zksync2-0.5.0/zksync2/manage_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IEthToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/INonceHolder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49698 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IZkSync.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_abi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/contract_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/deploy_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/erc20_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/eth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/l1_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/l2_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/nonce_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/paymaster_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/precompute_contract_deployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/manage_contracts/zksync_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/module_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/request_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/response_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/zksync_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/module/zksync_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/provider/eth_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.834590 zksync2-0.5.0/zksync2/signer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/signer/eth_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.838590 zksync2-0.5.0/zksync2/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/transaction/transaction712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-05-26 13:16:23.000000 zksync2-0.5.0/zksync2/transaction/transaction_builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:16:39.826590 zksync2-0.5.0/zksync2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 13:16:39.000000 zksync2-0.5.0/zksync2.egg-info/top_level.txt
```

### Comparing `zksync2-0.4.0/.github/workflows/release.yaml` & `zksync2-0.5.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/.gitignore` & `zksync2-0.5.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -153,9 +153,10 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
+.idea/
 
+!examples/*/*/build
```

### Comparing `zksync2-0.4.0/PKG-INFO` & `zksync2-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: zksync2
-Version: 0.4.0
+Version: 0.5.0
 Summary: zkSync2 python client sdk
 Home-page: https://zksync.io
-Author: Viktor Yastrebov
-Author-email: Viktor Yastrebov <vyastrebov@vareger.com>
+Author: Danijel Radakovic
+Author-email: Danijel Radakovic <danijel@txfusion.io>
 License: MIT
 Project-URL: Homepage, https://github.com/zksync-sdk/zksync2-python
 Project-URL: Bug Tracker, https://github.com/zksync-sdk/zksync2-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -26,18 +26,18 @@
 - [Contract interfaces](#contract-interfaces)
 - [Examples](#examples)
 
 
 ### Getting started
 
 #### Requirements
-| Tool            | Required |
-|-----------------|----------|
-| python          | >= 3.10  |
-| package manager | pip      |
+| Tool            | Required       |
+|-----------------|----------------|
+| python          | 3.8, 3.9, 3.10 |
+| package manager | pip            |
 
 ### how to install
 
 ```console
 pip install zksync2
 ```
 
@@ -328,19 +328,20 @@
 * encode_general
 
 For example and usage, please have a look into example [section](#examples)
 
 
 ### Examples
 
+* [check balance](./examples/11_check_balance.py)
 * [deposit funds](./examples/01_deposit.py)
-* [check balance](./examples/12_misc.py)
 * [transfer](./examples/02_transfer.py)
 * [transfer erc20 tokens](./examples/03_transfer_erc20_token.py)
-* [withdraw funds](./examples/11_withdrawal.py)
+* [withdraw funds](./examples/09_withdrawal.py)
+* [finalize withdrawal](./examples/10_finalize_withdrawal.py)
 * [deploy contract, precompute address by create](./examples/04_deploy_create.py)
-* [deploy contract with constructor(create method)](./examples/05_deploy_create_with_ctor.py)
+* [deploy contract with constructor(create method) and interact with contract](./examples/05_deploy_create_with_constructor.py)
 * [deploy contract with dependent contract(create method)](./examples/06_deploy_create_with_deps.py)
 * [deploy contract, precompute address by create2](./examples/07_deploy_create2.py)
 * [deploy contract with dependency, precompute address by create2](./examples/08_deploy_create2_deps.py)
-* [execute contracts method](./examples/09_execute_contract.py)
-* [support legacy transaction for call/execute contracts methods](./examples/10_execute_legacy.py)
+* [how to compile solidity contracts](./examples/README.md)
+
```

### Comparing `zksync2-0.4.0/README.md` & `zksync2-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 - [Contract interfaces](#contract-interfaces)
 - [Examples](#examples)
 
 
 ### Getting started
 
 #### Requirements
-| Tool            | Required |
-|-----------------|----------|
-| python          | >= 3.10  |
-| package manager | pip      |
+| Tool            | Required       |
+|-----------------|----------------|
+| python          | 3.8, 3.9, 3.10 |
+| package manager | pip            |
 
 ### how to install
 
 ```console
 pip install zksync2
 ```
 
@@ -311,19 +311,20 @@
 * encode_general
 
 For example and usage, please have a look into example [section](#examples)
 
 
 ### Examples
 
+* [check balance](./examples/11_check_balance.py)
 * [deposit funds](./examples/01_deposit.py)
-* [check balance](./examples/12_misc.py)
 * [transfer](./examples/02_transfer.py)
 * [transfer erc20 tokens](./examples/03_transfer_erc20_token.py)
-* [withdraw funds](./examples/11_withdrawal.py)
+* [withdraw funds](./examples/09_withdrawal.py)
+* [finalize withdrawal](./examples/10_finalize_withdrawal.py)
 * [deploy contract, precompute address by create](./examples/04_deploy_create.py)
-* [deploy contract with constructor(create method)](./examples/05_deploy_create_with_ctor.py)
+* [deploy contract with constructor(create method) and interact with contract](./examples/05_deploy_create_with_constructor.py)
 * [deploy contract with dependent contract(create method)](./examples/06_deploy_create_with_deps.py)
 * [deploy contract, precompute address by create2](./examples/07_deploy_create2.py)
 * [deploy contract with dependency, precompute address by create2](./examples/08_deploy_create2_deps.py)
-* [execute contracts method](./examples/09_execute_contract.py)
-* [support legacy transaction for call/execute contracts methods](./examples/10_execute_legacy.py)
+* [how to compile solidity contracts](./examples/README.md)
+
```

### Comparing `zksync2-0.4.0/examples/03_transfer_erc20_token.py` & `zksync2-0.5.0/examples/03_transfer_erc20_token.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
 from web3 import Web3
+
+from examples.utils import EnvPrivateKey
 from zksync2.core.types import ZkBlockParams, ADDRESS_DEFAULT, Token
 from zksync2.manage_contracts.erc20_contract import ERC20Contract, ERC20Encoder
 from zksync2.module.module_builder import ZkSyncBuilder
 from zksync2.signer.eth_signer import PrivateKeyEthSigner
 from zksync2.transaction.transaction_builders import TxFunctionCall
 
-ZKSYNC_TEST_URL = "https://zksync2-testnet.zksync.dev"
+ZKSYNC_TEST_URL = "https://testnet.era.zksync.dev"
 ETH_TEST_URL = "https://rpc.ankr.com/eth_goerli"
-PRIVATE_KEY = bytes.fromhex("fd1f96220fa3a40c46d65f81d61dd90af600746fd47e5c82673da937a48b38ef")
-PRIVATE_KEY2 = bytes.fromhex("ba6852a8a14cd3c72f6cab8c08f70d033d5d1a56646ab04b4cf54c01cb7204dc")
 SERC20_Address = Web3.to_checksum_address("0xd782e03F4818A7eDb0bc5f70748F67B4e59CdB33")
 
 
 class Colors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
@@ -23,17 +23,19 @@
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
 
 def transfer_erc20(amount: float):
+    env1 = EnvPrivateKey("ZKSYNC_TEST_KEY")
+    env2 = EnvPrivateKey("ZKSYNC_TEST_KEY2")
     web3 = ZkSyncBuilder.build(ZKSYNC_TEST_URL)
-    alice: LocalAccount = Account.from_key(PRIVATE_KEY)
-    bob: LocalAccount = Account.from_key(PRIVATE_KEY2)
+    alice: LocalAccount = Account.from_key(env1.key)
+    bob: LocalAccount = Account.from_key(env2.key)
     chain_id = web3.zksync.chain_id
     signer = PrivateKeyEthSigner(alice, chain_id)
 
     erc20_token = Token(l1_address=ADDRESS_DEFAULT,
                         l2_address=SERC20_Address,
                         symbol="SERC20",
                         decimals=18)
```

### Comparing `zksync2-0.4.0/examples/04_deploy_create.py` & `zksync2-0.5.0/examples/06_deploy_create_with_deps.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,121 @@
 import os
 from pathlib import Path
+
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
+from web3 import Web3
+
 from zksync2.core.types import EthBlockParams
 from zksync2.manage_contracts.contract_encoder_base import ContractEncoder
 from zksync2.manage_contracts.nonce_holder import NonceHolder
 from zksync2.manage_contracts.precompute_contract_deployer import PrecomputeContractDeployer
 from zksync2.module.module_builder import ZkSyncBuilder
 from zksync2.signer.eth_signer import PrivateKeyEthSigner
 from zksync2.transaction.transaction_builders import TxCreateContract
 
-ZKSYNC_TEST_URL = "http://127.0.0.1:3050"
-ETH_TEST_URL = "http://127.0.0.1:8545"
-PRIVATE_KEY2 = bytes.fromhex("fd1f96220fa3a40c46d65f81d61dd90af600746fd47e5c82673da937a48b38ef")
-
-
-class Colors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKCYAN = '\033[96m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
 
 def generate_random_salt() -> bytes:
     return os.urandom(32)
 
 
-def deploy_contract(compiled_contract: Path):
-    web3 = ZkSyncBuilder.build(ZKSYNC_TEST_URL)
-    account: LocalAccount = Account.from_key(PRIVATE_KEY2)
-    chain_id = web3.zksync.chain_id
+def deploy_contract(
+        zk_web3: Web3, account: LocalAccount, compiled_contract: Path
+):
+    """Deploy compiled contract with dependency on zkSync network using create() opcode
+
+    :param zk_web3:
+        Instance of ZkSyncBuilder that interacts with zkSync network
+
+    :param account:
+        From which account the deployment contract tx will be made
+
+    :param compiled_contract:
+        Compiled contract source.
+
+    :return:
+        Address of deployed contract.
+    """
+    # Get chain id of zkSync network
+    chain_id = zk_web3.zksync.chain_id
+
+    # Signer is used to generate signature of provided transaction
     signer = PrivateKeyEthSigner(account, chain_id)
 
-    random_salt = generate_random_salt()
-    nonce = web3.zksync.get_transaction_count(account.address, EthBlockParams.PENDING.value)
-    nonce_holder = NonceHolder(web3, account)
+    # Get nonce of ETH address on zkSync network
+    nonce = zk_web3.zksync.get_transaction_count(
+        account.address, EthBlockParams.PENDING.value
+    )
+
+    # Get deployment nonce
+    nonce_holder = NonceHolder(zk_web3, account)
     deployment_nonce = nonce_holder.get_deployment_nonce(account.address)
-    deployer = PrecomputeContractDeployer(web3)
+
+    # Precompute the address of smart contract
+    # Use this if there is a case where contract address should be known before deployment
+    deployer = PrecomputeContractDeployer(zk_web3)
     precomputed_address = deployer.compute_l2_create_address(account.address, deployment_nonce)
-    counter_contract = ContractEncoder.from_json(web3, compiled_contract)
 
-    print(f"precomputed address: {precomputed_address}")
+    # Get ABI and bytecode of demo and foo contracts
+    demo_contract, foo_contract = ContractEncoder.from_json(zk_web3, compiled_contract)
+
+    # Get current gas price in Wei
+    gas_price = zk_web3.zksync.gas_price
 
-    gas_price = web3.zksync.gas_price
-    create_contract = TxCreateContract(web3=web3,
+    # Create deployment contract transaction
+    create_contract = TxCreateContract(web3=zk_web3,
                                        chain_id=chain_id,
                                        nonce=nonce,
                                        from_=account.address,
-                                       gas_limit=0,  # UNKNOWN AT THIS STATE
+                                       gas_limit=0,
                                        gas_price=gas_price,
-                                       bytecode=counter_contract.bytecode,
-                                       salt=random_salt)
-    estimate_gas = web3.zksync.eth_estimate_gas(create_contract.tx)
-    print(f"Fee for transaction is: {estimate_gas * gas_price}")
+                                       bytecode=demo_contract.bytecode,
+                                       deps=[foo_contract.bytecode])
+
+    # ZkSync transaction gas estimation
+    estimate_gas = zk_web3.zksync.eth_estimate_gas(create_contract.tx)
+    print(f"Fee for transaction is: {Web3.from_wei(estimate_gas * gas_price, 'ether')} ETH")
+
+    # Convert transaction to EIP-712 format
     tx_712 = create_contract.tx712(estimate_gas)
-    singed_message = signer.sign_typed_data(tx_712.to_eip712_struct())
-    msg = tx_712.encode(singed_message)
-    tx_hash = web3.zksync.send_raw_transaction(msg)
-    tx_receipt = web3.zksync.wait_for_transaction_receipt(tx_hash, timeout=240, poll_latency=0.5)
+
+    # Sign message
+    signed_message = signer.sign_typed_data(tx_712.to_eip712_struct())
+
+    # Encode signed message
+    msg = tx_712.encode(signed_message)
+
+    # Deploy contract
+    tx_hash = zk_web3.zksync.send_raw_transaction(msg)
+
+    # Wait for deployment contract transaction to be included in a block
+    tx_receipt = zk_web3.zksync.wait_for_transaction_receipt(
+        tx_hash, timeout=240, poll_latency=0.5
+    )
 
     print(f"Tx status: {tx_receipt['status']}")
     contract_address = tx_receipt["contractAddress"]
-
     print(f"contract address: {contract_address}")
-    if precomputed_address.lower() == contract_address.lower():
-        print(f"{Colors.OKGREEN}Precomputed address is eqaul to deployed: {contract_address}{Colors.ENDC}")
-    else:
-        print(f"{Colors.FAIL}Precomputed address does not equal to deployed{Colors.ENDC}")
-
-    value = counter_contract.contract.functions.get().call(
-        {
-            "from": account.address,
-            "to": contract_address
-        })
-    print(f"Call method for deployed contract, address: {contract_address}, value: {value}")
+
+    # Check does precompute address match with deployed address
+    if precomputed_address.lower() != contract_address.lower():
+        raise RuntimeError("Precomputed contract address does now match with deployed contract address")
 
 
 if __name__ == "__main__":
-    contract_path = Path("../tests/contracts/Counter.json")
-    deploy_contract(contract_path)
+    # Set a provider
+    PROVIDER = "https://testnet.era.zksync.dev"
+
+    # Byte-format private key
+    PRIVATE_KEY = bytes.fromhex(os.environ.get("PRIVATE_KEY"))
+
+    # Connect to zkSync network
+    zk_web3 = ZkSyncBuilder.build(PROVIDER)
+
+    # Get account object by providing from private key
+    account: LocalAccount = Account.from_key(PRIVATE_KEY)
+
+    # Provide a compiled JSON source contract
+    contract_path = Path("solidity/demo/build/combined.json")
+
+    # Perform contract deployment
+    deploy_contract(zk_web3, account, contract_path)
```

### Comparing `zksync2-0.4.0/examples/05_deploy_create_with_ctor.py` & `zksync2-0.5.0/examples/04_deploy_create.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,108 @@
 import os
 from pathlib import Path
 
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
+from eth_typing import HexAddress
+from web3 import Web3
 
 from zksync2.core.types import EthBlockParams
 from zksync2.manage_contracts.contract_encoder_base import ContractEncoder
-from zksync2.manage_contracts.nonce_holder import NonceHolder
-from zksync2.manage_contracts.precompute_contract_deployer import PrecomputeContractDeployer
 from zksync2.module.module_builder import ZkSyncBuilder
 from zksync2.signer.eth_signer import PrivateKeyEthSigner
 from zksync2.transaction.transaction_builders import TxCreateContract
 
-ZKSYNC_TEST_URL = "http://127.0.0.1:3050"
-ETH_TEST_URL = "http://127.0.0.1:8545"
-PRIVATE_KEY2 = bytes.fromhex("fd1f96220fa3a40c46d65f81d61dd90af600746fd47e5c82673da937a48b38ef")
-
-
-class Colors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKCYAN = '\033[96m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
-
-def generate_random_salt() -> bytes:
-    return os.urandom(32)
-
-
-def deploy_contract_ctor(compiled_contract: Path, ctor_args: tuple):
-    web3 = ZkSyncBuilder.build(ZKSYNC_TEST_URL)
-    account: LocalAccount = Account.from_key(PRIVATE_KEY2)
-    chain_id = web3.zksync.chain_id
-    signer = PrivateKeyEthSigner(account, chain_id)
 
-    random_salt = generate_random_salt()
-    nonce = web3.zksync.get_transaction_count(account.address, EthBlockParams.PENDING.value)
-    gas_price = web3.zksync.gas_price
-
-    nonce_holder = NonceHolder(web3, account)
-    deployment_nonce = nonce_holder.get_deployment_nonce(account.address)
-
-    deployer = PrecomputeContractDeployer(web3)
-    precomputed_address = deployer.compute_l2_create_address(account.address, deployment_nonce)
-
-    constructor_encoder = ContractEncoder.from_json(web3, compiled_contract)
-    # a = 2
-    # b = 3
-    encoded_ctor = constructor_encoder.encode_constructor(args=ctor_args)
-
-    create_contract = TxCreateContract(web3=web3,
-                                       chain_id=chain_id,
-                                       nonce=nonce,
-                                       from_=account.address,
-                                       gas_limit=0,  # UNKNOWN AT THIS STATE,
-                                       gas_price=gas_price,
-                                       bytecode=constructor_encoder.bytecode,
-                                       call_data=encoded_ctor
-                                       , salt=random_salt)
+def deploy_contract(
+    zk_web3: Web3, account: LocalAccount, compiled_contract: Path
+) -> HexAddress:
+    """Deploy compiled contract on zkSync network using create() opcode
+
+    :param zk_web3:
+        Instance of ZkSyncBuilder that interacts with zkSync network
+
+    :param account:
+        From which account the deployment contract tx will be made
+
+    :param compiled_contract:
+        Compiled contract source.
+
+    :return:
+        Address of deployed contract.
+    """
+    # Get chain id of zkSync network
+    chain_id = zk_web3.zksync.chain_id
 
-    estimate_gas = web3.zksync.eth_estimate_gas(create_contract.tx)
+    # Signer is used to generate signature of provided transaction
+    signer = PrivateKeyEthSigner(account, chain_id)
 
-    print(f"Fee for transaction is: {estimate_gas * gas_price}")
+    # Get nonce of ETH address on zkSync network
+    nonce = zk_web3.zksync.get_transaction_count(
+        account.address, EthBlockParams.PENDING.value
+    )
+
+    # Get contract ABI and bytecode information
+    storage_contract = ContractEncoder.from_json(zk_web3, compiled_contract)[0]
+
+    # Get current gas price in Wei
+    gas_price = zk_web3.zksync.gas_price
+
+    # Create deployment contract transaction
+    create_contract = TxCreateContract(
+        web3=zk_web3,
+        chain_id=chain_id,
+        nonce=nonce,
+        from_=account.address,
+        gas_limit=0,  # UNKNOWN AT THIS STATE
+        gas_price=gas_price,
+        bytecode=storage_contract.bytecode,
+    )
+
+    # ZkSync transaction gas estimation
+    estimate_gas = zk_web3.zksync.eth_estimate_gas(create_contract.tx)
+    print(f"Fee for transaction is: {Web3.from_wei(estimate_gas * gas_price, 'ether')} ETH")
 
+    # Convert transaction to EIP-712 format
     tx_712 = create_contract.tx712(estimate_gas)
 
-    singed_message = signer.sign_typed_data(tx_712.to_eip712_struct())
-    msg = tx_712.encode(singed_message)
-    tx_hash = web3.zksync.send_raw_transaction(msg)
-    tx_receipt = web3.zksync.wait_for_transaction_receipt(tx_hash, timeout=240, poll_latency=0.5)
-    print(f"Tx status: {tx_receipt['status']}")
+    # Sign message
+    signed_message = signer.sign_typed_data(tx_712.to_eip712_struct())
+
+    # Encode signed message
+    msg = tx_712.encode(signed_message)
 
+    # Deploy contract
+    tx_hash = zk_web3.zksync.send_raw_transaction(msg)
+
+    # Wait for deployment contract transaction to be included in a block
+    tx_receipt = zk_web3.zksync.wait_for_transaction_receipt(
+        tx_hash, timeout=240, poll_latency=0.5
+    )
+
+    print(f"Tx status: {tx_receipt['status']}")
     contract_address = tx_receipt["contractAddress"]
-    print(f"contract address: {contract_address}")
-    if precomputed_address.lower() == contract_address.lower():
-        print(f"{Colors.OKGREEN}Precomputed address is eqaul to deployed: {contract_address}{Colors.ENDC}")
-    else:
-        print(f"{Colors.FAIL}Precomputed address does not equal to deployed{Colors.ENDC}")
-
-    value = constructor_encoder.contract.functions.get().call(
-        {
-            "from": account.address,
-            "to": contract_address
-        })
-    print(f"Call method for deployed contract, address: {contract_address}, value: {value}")
+
+    print(f"Deployed contract address: {contract_address}")
+
+    # Return the contract deployed address
+    return contract_address
 
 
 if __name__ == "__main__":
-    contract = Path("../tests/contracts/Counter.json")
-    args = (2, 3, False)
-    deploy_contract_ctor(contract, args)
+    # Set a provider
+    PROVIDER = "https://testnet.era.zksync.dev"
+
+    # Byte-format private key
+    PRIVATE_KEY = bytes.fromhex(os.environ.get("PRIVATE_KEY"))
+
+    # Connect to zkSync network
+    zk_web3 = ZkSyncBuilder.build(PROVIDER)
+
+    # Get account object by providing from private key
+    account: LocalAccount = Account.from_key(PRIVATE_KEY)
+
+    # Provide a compiled JSON source contract
+    contract_path = Path("solidity/storage/build/combined.json")
+
+    # Perform contract deployment
+    deploy_contract(zk_web3, account, contract_path)
```

### Comparing `zksync2-0.4.0/examples/07_deploy_create2.py` & `zksync2-0.5.0/examples/08_deploy_create2_deps.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,129 @@
 import os
 from pathlib import Path
 
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
+from eth_typing import HexAddress
+from web3 import Web3
 
 from zksync2.core.types import EthBlockParams
 from zksync2.manage_contracts.contract_encoder_base import ContractEncoder
 from zksync2.manage_contracts.precompute_contract_deployer import PrecomputeContractDeployer
 from zksync2.module.module_builder import ZkSyncBuilder
 from zksync2.signer.eth_signer import PrivateKeyEthSigner
 from zksync2.transaction.transaction_builders import TxCreate2Contract
 
-ZKSYNC_TEST_URL = "http://127.0.0.1:3050"
-ETH_TEST_URL = "http://127.0.0.1:8545"
-PRIVATE_KEY2 = bytes.fromhex("fd1f96220fa3a40c46d65f81d61dd90af600746fd47e5c82673da937a48b38ef")
 
+def generate_random_salt() -> bytes:
+    return os.urandom(32)
 
-class Colors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKCYAN = '\033[96m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
 
+def deploy_contract(
+        zk_web3: Web3, account: LocalAccount, compiled_contract: Path
+) -> HexAddress:
+    """Deploy compiled contract with dependency on zkSync network using create2() opcode
 
-def generate_random_salt() -> bytes:
-    return os.urandom(32)
+    :param zk_web3:
+        Instance of ZkSyncBuilder that interacts with zkSync network
+
+    :param account:
+        From which account the deployment contract tx will be made
+
+    :param compiled_contract:
+        Compiled contract source.
 
+    :return:
+        Address of deployed contract.
 
-def deploy_create2(contract: Path):
-    web3 = ZkSyncBuilder.build(ZKSYNC_TEST_URL)
-    account: LocalAccount = Account.from_key(PRIVATE_KEY2)
-    chain_id = web3.zksync.chain_id
+    """
+    # Get chain id of zkSync network
+    chain_id = zk_web3.zksync.chain_id
+
+    # Signer is used to generate signature of provided transaction
     signer = PrivateKeyEthSigner(account, chain_id)
 
+    # Get nonce of ETH address on zkSync network
+    nonce = zk_web3.zksync.get_transaction_count(
+        account.address, EthBlockParams.PENDING.value
+    )
+
+    # Deployment of same smart contract (same bytecode) without salt cannot be done twice
+    # Remove salt if you want to deploy contract only once
     random_salt = generate_random_salt()
-    nonce = web3.zksync.get_transaction_count(account.address, EthBlockParams.PENDING.value)
-    gas_price = web3.zksync.gas_price
-    deployer = PrecomputeContractDeployer(web3)
 
-    counter_contract_encoder = ContractEncoder.from_json(web3, contract)
+    # Precompute the address of smart contract
+    # Use this if there is a case where contract address should be known before deployment
+    deployer = PrecomputeContractDeployer(zk_web3)
+
+    # Get ABI and bytecode of demo and foo contracts
+    demo_contract, foo_contract = ContractEncoder.from_json(zk_web3, compiled_contract)
+
+    # Get precomputed contract address
     precomputed_address = deployer.compute_l2_create2_address(sender=account.address,
-                                                              bytecode=counter_contract_encoder.bytecode,
+                                                              bytecode=demo_contract.bytecode,
                                                               constructor=b'',
                                                               salt=random_salt)
-    create2_contract = TxCreate2Contract(web3=web3,
+
+    # Get current gas price in Wei
+    gas_price = zk_web3.zksync.gas_price
+
+    # Create2 deployment contract transaction
+    create2_contract = TxCreate2Contract(web3=zk_web3,
                                          chain_id=chain_id,
                                          nonce=nonce,
                                          from_=account.address,
                                          gas_limit=0,
                                          gas_price=gas_price,
-                                         bytecode=counter_contract_encoder.bytecode,
+                                         bytecode=demo_contract.bytecode,
+                                         deps=[foo_contract.bytecode],
                                          salt=random_salt)
-    estimate_gas = web3.zksync.eth_estimate_gas(create2_contract.tx)
-    print(f"Fee for transaction is: {estimate_gas * gas_price}")
+    # ZkSync transaction gas estimation
+    estimate_gas = zk_web3.zksync.eth_estimate_gas(create2_contract.tx)
+    print(f"Fee for transaction is: {Web3.from_wei(estimate_gas * gas_price, 'ether')} ETH")
 
+    # Convert transaction to EIP-712 format
     tx_712 = create2_contract.tx712(estimate_gas)
-    singed_message = signer.sign_typed_data(tx_712.to_eip712_struct())
-    msg = tx_712.encode(singed_message)
-    tx_hash = web3.zksync.send_raw_transaction(msg)
-    tx_receipt = web3.zksync.wait_for_transaction_receipt(tx_hash, timeout=240, poll_latency=1.0)
+
+    # Sign message
+    signed_message = signer.sign_typed_data(tx_712.to_eip712_struct())
+
+    # Encode signed message
+    msg = tx_712.encode(signed_message)
+
+    # Deploy contract
+    tx_hash = zk_web3.zksync.send_raw_transaction(msg)
+
+    # Wait for deployment contract transaction to be included in a block
+    tx_receipt = zk_web3.zksync.wait_for_transaction_receipt(
+        tx_hash, timeout=240, poll_latency=0.5
+    )
 
     print(f"Tx status: {tx_receipt['status']}")
     contract_address = tx_receipt["contractAddress"]
     print(f"contract address: {contract_address}")
-    if precomputed_address.lower() == contract_address.lower():
-        print(f"{Colors.OKGREEN}Precomputed address is eqaul to deployed: {contract_address}{Colors.ENDC}")
-    else:
-        print(f"{Colors.FAIL}Precomputed address does not equal to deployed{Colors.ENDC}")
-
-    value = counter_contract_encoder.contract.functions.get().call(
-        {
-            "from": account.address,
-            "to": contract_address
-        })
-    print(f"Call method for deployed contract, address: {contract_address}, value: {value}")
+
+    # Check does precompute address match with deployed address
+    if precomputed_address.lower() != contract_address.lower():
+        raise RuntimeError("Precomputed contract address does now match with deployed contract address")
+
+    return contract_address
 
 
 if __name__ == "__main__":
-    contract_path = Path("../tests/contracts/Counter.json")
-    deploy_create2(contract_path)
+    # Set a provider
+    PROVIDER = "https://testnet.era.zksync.dev"
+
+    # Byte-format private key
+    PRIVATE_KEY = bytes.fromhex(os.environ.get("PRIVATE_KEY"))
+
+    # Connect to zkSync network
+    zk_web3 = ZkSyncBuilder.build(PROVIDER)
+
+    # Get account object by providing from private key
+    account: LocalAccount = Account.from_key(PRIVATE_KEY)
+
+    # Provide a compiled JSON source contract
+    contract_path = Path("solidity/demo/build/combined.json")
+
+    # Perform contract deployment
+    deploy_contract(zk_web3, account, contract_path)
```

### Comparing `zksync2-0.4.0/examples/11_withdrawal.py` & `zksync2-0.5.0/examples/10_finalize_withdrawal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,73 @@
+import os
+
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
+from hexbytes import HexBytes
 from web3 import Web3
 from web3.middleware import geth_poa_middleware
+from web3.types import TxReceipt
 
-from zksync2.core.types import Token
 from zksync2.module.module_builder import ZkSyncBuilder
 from zksync2.provider.eth_provider import EthereumProvider
-from zksync2.transaction.transaction_builders import TxWithdraw
 
-ZKSYNC_TEST_URL = "http://127.0.0.1:3050"
-ETH_TEST_URL = "http://127.0.0.1:8545"
-PRIVATE_KEY2 = bytes.fromhex("fd1f96220fa3a40c46d65f81d61dd90af600746fd47e5c82673da937a48b38ef")
-
-
-class Colors:
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKCYAN = '\033[96m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
-
-def example_withdrawal(amount: float):
-    web3 = ZkSyncBuilder.build(ZKSYNC_TEST_URL)
-    account: LocalAccount = Account.from_key(PRIVATE_KEY2)
 
-    eth_web3 = Web3(Web3.HTTPProvider(ETH_TEST_URL))
+def finalize_withdraw(
+        zksync_provider: Web3, ethereum_provider: EthereumProvider, withdraw_tx_hash: HexBytes
+) -> TxReceipt:
+    """
+    Execute finalize withdraw transaction on L1 network
+    :type zksync_provider:
+         Instance of ZkSync provider
+    :param ethereum_provider
+        Instance of EthereumProvider
+    :param withdraw_tx_hash
+        Hash of withdraw transaction on L2 network
+    :return:
+        TxReceipt of finalize withdraw transaction on L1 network
+    """
+    zks_receipt = zksync_provider.zksync.wait_finalized(withdraw_tx_hash)
+
+    # Check if withdraw transaction was successful
+    if not zks_receipt["status"]:
+        raise RuntimeError("Withdraw transaction on L2 network failed")
+
+    # Execute finalize withdraw
+    tx_receipt = ethereum_provider.finalize_withdrawal(zks_receipt["transactionHash"])
+
+    # Check if finalize withdraw transaction was successful
+    if not tx_receipt["status"]:
+        raise RuntimeError("Finalize withdraw transaction L1 network failed")
+    return tx_receipt
+
+
+if __name__ == "__main__":
+    # Get the private key from OS environment variables
+    PRIVATE_KEY = bytes.fromhex(os.environ.get("PRIVATE_KEY"))
+
+    # Get the withdrawal transaction hash from OS environment variables
+    WITHDRAW_TX_HASH = HexBytes.fromhex(os.environ.get("WITHDRAW_TX_HASH"))
+
+    # Set a provider
+    ZKSYNC_PROVIDER = "https://testnet.era.zksync.dev"
+    ETH_PROVIDER = "https://rpc.ankr.com/eth_goerli"
+
+    # Connect to zkSync network
+    zk_web3 = ZkSyncBuilder.build(ZKSYNC_PROVIDER)
+
+    # Connect to Ethereum network
+    eth_web3 = Web3(Web3.HTTPProvider(ETH_PROVIDER))
     eth_web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
-    eth_balance = eth_web3.eth.get_balance(account.address)
-    print(f"Eth: balance: {Web3.from_wei(eth_balance, 'ether')}")
+    # Get account object by providing from private key
+    account: LocalAccount = Account.from_key(PRIVATE_KEY)
 
-    eth_provider = EthereumProvider(web3,
-                                    eth_web3,
-                                    account)
-    withdrawal = TxWithdraw(web3=web3,
-                            token=Token.create_eth(),
-                            amount=Web3.to_wei(amount, "ether"),
-                            gas_limit=0,  # unknown
-                            account=account)
-    estimated_gas = web3.zksync.eth_estimate_gas(withdrawal.tx)
-    tx = withdrawal.estimated_gas(estimated_gas)
-    signed = account.sign_transaction(tx)
-    tx_hash = web3.zksync.send_raw_transaction(signed.rawTransaction)
-    zks_receipt = web3.zksync.wait_finalized(tx_hash, timeout=240, poll_latency=0.5)
-    print(f"ZkSync Tx status: {zks_receipt['status']}")
-    tx_receipt = eth_provider.finalize_withdrawal(zks_receipt["transactionHash"])
-    print(f"Finalize withdrawal, Tx status: {tx_receipt['status']}")
-
-    prev = eth_balance
-    eth_balance = eth_web3.eth.get_balance(account.address)
-    print(f"Eth: balance: {Web3.from_wei(eth_balance, 'ether')}")
-
-    fee = tx_receipt['gasUsed'] * tx_receipt['effectiveGasPrice']
-    withdraw_absolute = Web3.to_wei(amount, 'ether') - fee
-    diff = eth_balance - prev
-    if withdraw_absolute == diff:
-        print(f"{Colors.OKGREEN}Withdrawal including tx fee is passed{Colors.ENDC}")
-        print(f"{Colors.OKGREEN}Eth diff with fee included: {Web3.from_wei(diff, 'ether')}{Colors.ENDC}")
-    else:
-        print(f"P{Colors.FAIL}Withdrawal failed{Colors.ENDC}")
-        print(f"{Colors.FAIL}Eth diff with fee included: {Web3.from_wei(diff, 'ether')}{Colors.ENDC}")
+    # Create Ethereum provider
+    eth_provider = EthereumProvider(zk_web3, eth_web3, account)
 
+    # Finalize withdraw of previous successful withdraw transaction
+    eth_tx_receipt = finalize_withdraw(zk_web3, eth_provider, WITHDRAW_TX_HASH)
 
-if __name__ == "__main__":
-    example_withdrawal(0.1)
+    fee = eth_tx_receipt["gasUsed"] * eth_tx_receipt["effectiveGasPrice"]
+    amount = 0.01
+    print(f"Finalize withdraw transaction: {eth_tx_receipt['transactionHash'].hex()}")
+    print(f"Effective ETH withdraw (paid fee): {Web3.from_wei(Web3.to_wei(amount, 'ether') - fee, 'ether')}")
```

### Comparing `zksync2-0.4.0/pyproject.toml` & `zksync2-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zksync2"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
-  { name="Viktor Yastrebov", email="vyastrebov@vareger.com" },
+  { name="Danijel Radakovic", email="danijel@txfusion.io" },
 ]
 description = "zkSync2 python client sdk"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `zksync2-0.4.0/setup.cfg` & `zksync2-0.5.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = zksync2
 description = zkSync2 python client sdk
 long_description = file: README.md
-author = Viktor Yastrebov
+author = Danijel Radakovic
 url = https://zksync.io
 license = MIT
 
 [options]
 packages = find:
 install_requires = 
 	eip712_structs == 1.1.0
```

### Comparing `zksync2-0.4.0/tests/contracts/Counter.json` & `zksync2-0.5.0/tests/contracts/Counter.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/contracts/CustomAccount.json` & `zksync2-0.5.0/tests/contracts/CustomAccount.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/contracts/CustomPaymaster.json` & `zksync2-0.5.0/tests/contracts/CustomPaymaster.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/contracts/Foo.json` & `zksync2-0.5.0/tests/contracts/Foo.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/contracts/Import.json` & `zksync2-0.5.0/tests/contracts/Import.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/contracts/SimpleConstructor.json` & `zksync2-0.5.0/tests/contracts/SimpleConstructor.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/contracts/SomeERC20.json` & `zksync2-0.5.0/tests/contracts/SomeERC20.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/test_config.py` & `zksync2-0.5.0/tests/integration/test_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,24 @@
+import os
 from dataclasses import dataclass
 from enum import IntEnum, auto
+from eth_typing import HexStr
+from eth_utils import remove_0x_prefix
 
-PRIVATE_KEY2 = bytes.fromhex("fd1f96220fa3a40c46d65f81d61dd90af600746fd47e5c82673da937a48b38ef")
-PRIVATE_KEY_BOB = bytes.fromhex("ba6852a8a14cd3c72f6cab8c08f70d033d5d1a56646ab04b4cf54c01cb7204dc")
+
+class EnvPrivateKey:
+    def __init__(self, env: str):
+        env = os.getenv(env, None)
+        if env is None:
+            raise LookupError(f"Can't build key from {env}")
+        self._key = bytes.fromhex(remove_0x_prefix(HexStr(env)))
+
+    @property
+    def key(self) -> bytes:
+        return self._key
 
 
 class EnvType(IntEnum):
     LOCAL_HOST = auto()
     TESTNET = auto()
     UNKNOWN = auto()
```

### Comparing `zksync2-0.4.0/tests/test_contract_deployer.py` & `zksync2-0.5.0/tests/unit/test_contract_deploy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from unittest import TestCase
 from eth_typing import HexStr
 from eth_utils import add_0x_prefix
 from web3 import Web3
 from web3.types import Nonce
-from tests.test_config import ZKSYNC_TEST_URL
+from test_config import LOCAL_ENV
 from zksync2.core.utils import hash_byte_code
 from tests.contracts.utils import contract_path
 from zksync2.manage_contracts.precompute_contract_deployer import PrecomputeContractDeployer
 from zksync2.manage_contracts.contract_encoder_base import ContractEncoder
 from zksync2.module.module_builder import ZkSyncBuilder
 
 
 class ContractDeployerTests(TestCase):
 
     def setUp(self) -> None:
-        self.web3 = ZkSyncBuilder.build(ZKSYNC_TEST_URL)
+        env = LOCAL_ENV
+        self.web3 = ZkSyncBuilder.build(env.zksync_server)
         self.contract_deployer = PrecomputeContractDeployer(self.web3)
         counter_contract = ContractEncoder.from_json(self.web3, contract_path("Counter.json"))
         self.counter_contract_bin = counter_contract.bytecode
 
     def test_compute_l2_create2(self):
         expected = Web3.to_checksum_address("0xf7671F9178dF17CF2F94a51d5a97bF54f6dff25a")
         sender = HexStr("0xa909312acfc0ed4370b8bd20dfe41c8ff6595194")
```

### Comparing `zksync2-0.4.0/tests/test_eip712_structed.py` & `zksync2-0.5.0/tests/unit/test_eip712.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         'to': to,
         'from': from_,
         'contents': content
     }
     return Mail(**kwargs)
 
 
-class TestEIP712Structured(TestCase):
+class EIP712Tests(TestCase):
 
     def setUp(self) -> None:
         self.person_from = Person(name="Cow", wallet="0xCD2a3d9F938E13CD947Ec05AbC7FE734Df8DD826")
         self.person_to = Person(name="Bob", wallet="0xbBbBBBBbbBBBbbbBbbBbbbbBBbBbbbbBbBbbBBbB")
         self.mail = make_mail(from_=self.person_from, to=self.person_to, content="Hello, Bob!")
         self.domain = make_domain(name="Ether Mail",
                                   version="1",
```

### Comparing `zksync2-0.4.0/tests/test_eth_signer.py` & `zksync2-0.5.0/tests/unit/test_eth_signer.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         'to': to,
         'from': from_,
         'contents': content
     }
     return Mail(**kwargs)
 
 
-class TestEthSigner(TestCase):
+class EthSignerTests(TestCase):
     _TEST_TYPED_EXPECTED_SIGNATURE = HexStr("0x4355c47d63924e8a72e509b65029052eb6c299d53a04e167c5775fd466751"
                                             "c9d07299936d304c153f6443dfa05f40ff007d72911b6f72307f996231605b915621c")
 
     def setUp(self) -> None:
         self.domain = make_domain(name="Ether Mail",
                                   version="1",
                                   chainId=1,
```

### Comparing `zksync2-0.4.0/tests/test_paymaster.py` & `zksync2-0.5.0/tests/integration/test_paymaster.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/tests/test_transaction712.py` & `zksync2-0.5.0/tests/unit/test_transaction712.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from unittest import TestCase
+
+from eip712_structs import make_domain
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
-from eth_utils.crypto import keccak
-from eip712_structs import make_domain
-from eth_tester import PyEVMBackend
 from eth_typing import HexStr
-from web3 import Web3, EthereumTesterProvider
+from eth_utils.crypto import keccak
+from web3 import Web3
 from web3.types import Nonce
+
 from tests.contracts.utils import contract_path
-from tests.test_config import PRIVATE_KEY2
+from test_config import LOCAL_ENV
 from zksync2.manage_contracts.contract_encoder_base import ContractEncoder
 from zksync2.module.request_types import EIP712Meta
-from zksync2.transaction.transaction_builders import TxCreateContract
 from zksync2.transaction.transaction712 import Transaction712
+from zksync2.transaction.transaction_builders import TxCreateContract
+
+PRIVATE_KEY2 = bytes.fromhex("fd1f96220fa3a40c46d65f81d61dd90af600746fd47e5c82673da937a48b38ef")
 
 
-class TestTransaction712(TestCase):
+class Transaction712Tests(TestCase):
     NONCE = Nonce(42)
     CHAIN_ID = 42
     GAS_LIMIT = 54321
     SENDER = HexStr("0x1234512345123451234512345123451234512345")
     RECEIVER = HexStr("0xCcCCccccCCCCcCCCCCCcCcCccCcCCCcCcccccccC")
 
     TRANSACTION_SIGNATURE = "Transaction(uint256 txType,uint256 from,uint256 to,uint256 gasLimit,uint256 " \
@@ -27,15 +30,17 @@
                             "uint256 paymaster,uint256 nonce,uint256 value,bytes data,bytes32[] factoryDeps," \
                             "bytes paymasterInput)"
 
     EXPECTED_ENCODED_VALUE = '0x1e40bcee418db11047ffefb27b304f8ec1b5d644c35c56878f5cc12988b3162d'
     EXPECTED_ENCODED_BYTES = "0x7519adb6e67031ee048d921120687e4fbdf83961bcf43756f349d689eed2b80c"
 
     def setUp(self) -> None:
-        self.web3 = Web3(EthereumTesterProvider(PyEVMBackend()))
+        # self.web3 = Web3(EthereumTesterProvider(PyEVMBackend()))
+        self.env = LOCAL_ENV
+        self.web3 = Web3(Web3.HTTPProvider(self.env.eth_server))
         self.account: LocalAccount = Account.from_key(PRIVATE_KEY2)
         self.counter_contract_encoder = ContractEncoder.from_json(self.web3, contract_path("Counter.json"))
         self.tx712 = Transaction712(chain_id=self.CHAIN_ID,
                                     nonce=self.NONCE,
                                     gas_limit=self.GAS_LIMIT,
                                     to=self.RECEIVER,
                                     value=0,
```

### Comparing `zksync2-0.4.0/tests/test_zksync_contract.py` & `zksync2-0.5.0/tests/integration/test_zksync_contract.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import os
 from unittest import TestCase
+
+from eth_account import Account
+from eth_account.signers.local import LocalAccount
 from web3 import Web3
-from tests.test_config import ZKSYNC_TEST_URL, ETH_TEST_URL, PRIVATE_KEY2
+
+from test_config import LOCAL_ENV, EnvPrivateKey
 from zksync2.core.utils import RecommendedGasLimit
 from zksync2.manage_contracts.zksync_contract import ZkSyncContract
 from zksync2.module.module_builder import ZkSyncBuilder
-from eth_account import Account
-from eth_account.signers.local import LocalAccount
 from zksync2.signer.eth_signer import PrivateKeyEthSigner
 
 
 def generate_random_salt() -> bytes:
     return os.urandom(32)
 
 
 class ZkSyncWeb3Tests(TestCase):
 
     def setUp(self) -> None:
-        self.zksync = ZkSyncBuilder.build(ZKSYNC_TEST_URL)
-        self.eth_web3 = Web3(Web3.HTTPProvider(ETH_TEST_URL))
-        self.account: LocalAccount = Account.from_key(PRIVATE_KEY2)
+        env = LOCAL_ENV
+        env_key = EnvPrivateKey("ZKSYNC_KEY1")
+        self.zksync = ZkSyncBuilder.build(env.zksync_server)
+        self.eth_web3 = Web3(Web3.HTTPProvider(env.eth_server))
+        self.account: LocalAccount = Account.from_key(env_key.key)
         self.chain_id = self.zksync.zksync.chain_id
         self.signer = PrivateKeyEthSigner(self.account, self.chain_id)
         self.zksync_contract = ZkSyncContract(self.zksync.zksync.zks_main_contract(),
                                               self.eth_web3,
                                               self.account)
 
     def test_facet_addresses_call(self):
```

### Comparing `zksync2-0.4.0/tests/test_zksync_web3.py` & `zksync2-0.5.0/tests/integration/test_zksync_web3.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 from zksync2.core.types import Token, ZkBlockParams, EthBlockParams, ADDRESS_DEFAULT
 from eth_account import Account
 from eth_account.signers.local import LocalAccount
 from zksync2.provider.eth_provider import EthereumProvider
 from zksync2.signer.eth_signer import PrivateKeyEthSigner
 from tests.contracts.utils import contract_path
 from zksync2.transaction.transaction_builders import TxFunctionCall, TxCreateContract, TxCreate2Contract, TxWithdraw
-from test_config import LOCAL_ENV, PRIVATE_KEY2, PRIVATE_KEY_BOB, EnvType
+from test_config import LOCAL_ENV, EnvType, EnvPrivateKey
 
 
 def generate_random_salt() -> bytes:
     return os.urandom(32)
 
 
 class ZkSyncWeb3Tests(TestCase):
     ETH_TOKEN = Token.create_eth()
     ETH_TEST_NET_AMOUNT_BALANCE = Decimal(1)
 
     def setUp(self) -> None:
         self.env = LOCAL_ENV
         self.web3 = ZkSyncBuilder.build(self.env.zksync_server)
-        self.account: LocalAccount = Account.from_key(PRIVATE_KEY2)
+        env_key = EnvPrivateKey("ZKSYNC_KEY1")
+        self.account: LocalAccount = Account.from_key(env_key.key)
         self.chain_id = self.web3.zksync.chain_id
         self.signer = PrivateKeyEthSigner(self.account, self.chain_id)
         self.counter_address = None
         self.test_tx_hash = None
         # INFO: use deploy_erc20_token_builder to get new address
         if self.env.type == EnvType.LOCAL_HOST:
             self.some_erc20_address = Web3.to_checksum_address("0x37b96512962FC7773E06237116BE693Eb2b3cD51")
@@ -282,16 +283,17 @@
         self.assertEqual(1, tx_receipt["status"])
 
         balance_after = erc20.balance_of(self.account.address)
         print(f"{self.ERC20_Token.symbol} balance before : {self.ERC20_Token.format_token(balance_after)}")
         self.assertEqual(balance_before, balance_after)
 
     def test_transfer_erc20_token(self):
+        env_bob = EnvPrivateKey("ZKSYNC_KEY2")
         alice = self.account
-        bob: LocalAccount = Account.from_key(PRIVATE_KEY_BOB)
+        bob: LocalAccount = Account.from_key(env_bob.key)
 
         erc20 = ERC20Contract(web3=self.web3.zksync,
                               contract_address=self.some_erc20_address,
                               account=alice)
         alice_balance_before = erc20.balance_of(alice.address)
         bob_balance_before = erc20.balance_of(bob.address)
         print(f"Alice {self.ERC20_Token.symbol} balance before : {self.ERC20_Token.format_token(alice_balance_before)}")
```

### Comparing `zksync2-0.4.0/zksync2/core/types.py` & `zksync2-0.5.0/zksync2/core/types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/core/utils.py` & `zksync2-0.5.0/zksync2/core/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,10 +45,10 @@
 
 def pad_front_bytes(bs: bytes, needed_length: int):
     padded = b'\0' * (needed_length - len(bs)) + bs
     return padded
 
 
 class RecommendedGasLimit(IntEnum):
-    DEPOSIT = 600000
+    DEPOSIT = 10000000
     EXECUTE = 620000
     ERC20_APPROVE = 50000
```

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/ContractDeployer.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IERC20.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IERC20.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IEthToken.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IEthToken.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL1Bridge.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IL2Bridge.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/INonceHolder.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/INonceHolder.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IPaymasterFlow.json`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_abi/IZkSync.json` & `zksync2-0.5.0/zksync2/manage_contracts/contract_abi/IZkSync.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9738492063492064%*

 * *Differences: {"'abi'": "{71: {'inputs': {0: {'internalType': 'contract IAllowList', 'name': '_newAllowList'}, "*

 * *          "delete: [8, 7, 6, 5, 4, 3, 2, 1, 0]}, 'name': 'setAllowList', 'outputs': [], "*

 * *          "'stateMutability': 'nonpayable'}, insert: [(9, OrderedDict([('anonymous', False), "*

 * *          "('inputs', [OrderedDict([('indexed', True), ('internalType', 'address'), ('name', "*

 * *          "'oldAllowList'), ('type', 'address')]), OrderedDict([('indexed', True), "*

 * *          "('internalType', 'address'), ('name', […]*

```diff
@@ -178,14 +178,33 @@
         },
         {
             "anonymous": false,
             "inputs": [
                 {
                     "indexed": true,
                     "internalType": "address",
+                    "name": "oldAllowList",
+                    "type": "address"
+                },
+                {
+                    "indexed": true,
+                    "internalType": "address",
+                    "name": "newAllowList",
+                    "type": "address"
+                }
+            ],
+            "name": "NewAllowList",
+            "type": "event"
+        },
+        {
+            "anonymous": false,
+            "inputs": [
+                {
+                    "indexed": true,
+                    "internalType": "address",
                     "name": "oldGovernor",
                     "type": "address"
                 },
                 {
                     "indexed": true,
                     "internalType": "address",
                     "name": "newGovernor",
@@ -957,14 +976,27 @@
             "name": "freezeDiamond",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
+            "name": "getAllowList",
+            "outputs": [
+                {
+                    "internalType": "address",
+                    "name": "",
+                    "type": "address"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [],
             "name": "getCurrentProposalId",
             "outputs": [
                 {
                     "internalType": "uint256",
                     "name": "",
                     "type": "uint256"
                 }
@@ -1048,14 +1080,27 @@
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
+            "name": "getPriorityTxMaxGasLimit",
+            "outputs": [
+                {
+                    "internalType": "uint256",
+                    "name": "",
+                    "type": "uint256"
+                }
+            ],
+            "stateMutability": "view",
+            "type": "function"
+        },
+        {
+            "inputs": [],
             "name": "getProposedUpgradeHash",
             "outputs": [
                 {
                     "internalType": "bytes32",
                     "name": "",
                     "type": "bytes32"
                 }
@@ -1195,27 +1240,14 @@
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
             "inputs": [],
-            "name": "getpriorityTxMaxGasLimit",
-            "outputs": [
-                {
-                    "internalType": "uint256",
-                    "name": "",
-                    "type": "uint256"
-                }
-            ],
-            "stateMutability": "view",
-            "type": "function"
-        },
-        {
-            "inputs": [],
             "name": "isApprovedBySecurityCouncil",
             "outputs": [
                 {
                     "internalType": "bool",
                     "name": "",
                     "type": "bool"
                 }
@@ -1824,155 +1856,22 @@
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
-                    "internalType": "uint256",
-                    "name": "_txId",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_l2Value",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_sender",
-                    "type": "address"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_contractAddressL2",
-                    "type": "address"
-                },
-                {
-                    "internalType": "bytes",
-                    "name": "_calldata",
-                    "type": "bytes"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_l2GasLimit",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_l2GasPerPubdataByteLimit",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "bytes[]",
-                    "name": "_factoryDeps",
-                    "type": "bytes[]"
-                },
-                {
-                    "internalType": "uint256",
-                    "name": "_toMint",
-                    "type": "uint256"
-                },
-                {
-                    "internalType": "address",
-                    "name": "_refundRecipient",
+                    "internalType": "contract IAllowList",
+                    "name": "_newAllowList",
                     "type": "address"
                 }
             ],
-            "name": "serializeL2Transaction",
-            "outputs": [
-                {
-                    "components": [
-                        {
-                            "internalType": "uint256",
-                            "name": "txType",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "from",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "to",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "gasLimit",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "gasPerPubdataByteLimit",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "maxFeePerGas",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "maxPriorityFeePerGas",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "paymaster",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "nonce",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256",
-                            "name": "value",
-                            "type": "uint256"
-                        },
-                        {
-                            "internalType": "uint256[4]",
-                            "name": "reserved",
-                            "type": "uint256[4]"
-                        },
-                        {
-                            "internalType": "bytes",
-                            "name": "data",
-                            "type": "bytes"
-                        },
-                        {
-                            "internalType": "bytes",
-                            "name": "signature",
-                            "type": "bytes"
-                        },
-                        {
-                            "internalType": "uint256[]",
-                            "name": "factoryDeps",
-                            "type": "uint256[]"
-                        },
-                        {
-                            "internalType": "bytes",
-                            "name": "paymasterInput",
-                            "type": "bytes"
-                        },
-                        {
-                            "internalType": "bytes",
-                            "name": "reservedDynamic",
-                            "type": "bytes"
-                        }
-                    ],
-                    "internalType": "struct IMailbox.L2CanonicalTransaction",
-                    "name": "",
-                    "type": "tuple"
-                }
-            ],
-            "stateMutability": "pure",
+            "name": "setAllowList",
+            "outputs": [],
+            "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [
                 {
                     "internalType": "bytes32",
                     "name": "_l2BootloaderBytecodeHash",
```

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_encoder_base.py` & `zksync2-0.5.0/zksync2/manage_contracts/contract_encoder_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,16 +34,17 @@
 
 class ContractEncoder(BaseContractEncoder):
 
     @classmethod
     def from_json(cls, web3: Web3, compiled_contract: Path):
         with compiled_contract.open(mode='r') as json_f:
             data = json.load(json_f)
-            bytecode = bytes.fromhex(remove_0x_prefix(data["bytecode"]))
-            return cls(web3, abi=data["abi"], bytecode=bytecode)
+            # bytecode = bytes.fromhex(remove_0x_prefix(data["bytecode"]))
+            # return cls(web3, abi=data["abi"], bytecode=bytecode)
+            return [cls(web3, abi=v["abi"], bytecode=v["bin"]) for k, v in data["contracts"].items()]
 
     def __init__(self, web3: Web3, abi, bytecode):
         super(ContractEncoder, self).__init__(web3, abi, bytecode)
 
     def encode_constructor(self, *args: Any, **kwargs: Any) -> bytes:
         constructor_abi = get_constructor_abi(self.abi)
```

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/contract_factory.py` & `zksync2-0.5.0/zksync2/manage_contracts/contract_factory.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/erc20_contract.py` & `zksync2-0.5.0/zksync2/manage_contracts/erc20_contract.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/eth_token.py` & `zksync2-0.5.0/zksync2/manage_contracts/eth_token.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/l1_bridge.py` & `zksync2-0.5.0/zksync2/manage_contracts/l1_bridge.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/l2_bridge.py` & `zksync2-0.5.0/zksync2/manage_contracts/l2_bridge.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/nonce_holder.py` & `zksync2-0.5.0/zksync2/manage_contracts/nonce_holder.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/paymaster_utils.py` & `zksync2-0.5.0/zksync2/manage_contracts/paymaster_utils.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/precompute_contract_deployer.py` & `zksync2-0.5.0/zksync2/manage_contracts/precompute_contract_deployer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import importlib.resources as pkg_resources
 from eth_typing import HexStr
 from web3 import Web3
 from typing import Optional
 import json
+
+from web3.logs import DISCARD
 from web3.types import Nonce, TxReceipt
 from eth_utils.crypto import keccak
 from zksync2.manage_contracts import contract_abi
 from zksync2.core.utils import pad_front_bytes, to_bytes, int_to_bytes, hash_byte_code
 from zksync2.manage_contracts.contract_encoder_base import BaseContractEncoder
 
 icontract_deployer_abi_cache = None
@@ -48,36 +50,30 @@
         if call_data is None:
             call_data = self.EMPTY_BYTES
 
         if len(salt) != 32:
             raise OverflowError("Salt data must be 32 length")
 
         bytecode_hash = hash_byte_code(bytecode)
-        args = [
-            salt,
-            bytecode_hash,
-            call_data
-        ]
+        args = salt, bytecode_hash, call_data
+
         return self.contract_encoder.encode_method(fn_name=self.CREATE2_FUNC, args=args)
 
     def encode_create(self, bytecode: bytes, call_data: Optional[bytes] = None, salt_data: Optional[bytes] = None):
         if salt_data is None:
             salt_data = self.DEFAULT_SALT
         if call_data is None:
             call_data = self.EMPTY_BYTES
 
         if len(salt_data) != 32:
             raise OverflowError("Salt data must be 32 length")
 
         bytecode_hash = hash_byte_code(bytecode)
-        args = [
-            salt_data,
-            bytecode_hash,
-            call_data
-        ]
+        args = salt_data, bytecode_hash, call_data
+
         return self.contract_encoder.encode_method(fn_name=self.CREATE_FUNC, args=args)
 
     def compute_l2_create_address(self, sender: HexStr, nonce: Nonce) -> HexStr:
         sender_bytes = to_bytes(sender)
         sender_bytes = pad_front_bytes(sender_bytes, 32)
         nonce = int_to_bytes(nonce)
         nonce_bytes = pad_front_bytes(nonce, 32)
@@ -102,12 +98,12 @@
         result = self.CREATE2_PREFIX + sender_bytes + salt + bytecode_hash + ctor_hash
         sha_result = keccak(result)
         address = sha_result[12:]
         address = "0x" + address.hex()
         return HexStr(Web3.to_checksum_address(address))
 
     def extract_contract_address(self, receipt: TxReceipt) -> HexStr:
-        result = self.contract_encoder.contract.events.ContractDeployed().process_receipt(receipt)
+        result = self.contract_encoder.contract.events.ContractDeployed().process_receipt(receipt, errors=DISCARD)
         entry = result[1]["args"]
         addr = entry["contractAddress"]
         return addr
```

### Comparing `zksync2-0.4.0/zksync2/manage_contracts/zksync_contract.py` & `zksync2-0.5.0/zksync2/manage_contracts/zksync_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
                 "chainId": self.chain_id,
                 "from": self.account.address,
                 'nonce': self._nonce(),
             })
         return VerifierParams(ret[0], ret[1], ret[2])
 
     def get_priority_tx_max_gas_limit(self) -> int:
-        return self._method_("getpriorityTxMaxGasLimit")().call(
+        return self._method_("getPriorityTxMaxGasLimit")().call(
             {
                 "chainId": self.chain_id,
                 "from": self.account.address,
                 'nonce': self._nonce(),
             })
 
     def is_approved_by_security_council(self) -> bool:
@@ -429,7 +429,10 @@
                                                       l2_gas_limit,
                                                       l2_gas_per_pubdata_byte_limit).call(
             {
                 "chainId": self.chain_id,
                 "from": self.account.address,
                 'nonce': self._nonce(),
             })
+
+    def parse_events(self, tx_receipt: TxReceipt, event: str):
+        return self.contract.events[event]().process_receipt(tx_receipt)
```

### Comparing `zksync2-0.4.0/zksync2/module/middleware.py` & `zksync2-0.5.0/zksync2/module/middleware.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/module/module_builder.py` & `zksync2-0.5.0/zksync2/module/module_builder.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/module/request_types.py` & `zksync2-0.5.0/zksync2/module/request_types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/module/response_types.py` & `zksync2-0.5.0/zksync2/module/response_types.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/module/zksync_module.py` & `zksync2-0.5.0/zksync2/module/zksync_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,27 +317,22 @@
         return Web3.to_checksum_address(self._zks_get_testnet_paymaster_address())
 
     def eth_estimate_gas(self, tx: Transaction) -> int:
         return self._eth_estimate_gas(tx)
 
     @staticmethod
     def get_l2_hash_from_priority_op(tx_receipt: TxReceipt, main_contract: ZkSyncContract):
-        # TODO: wrong tx hash log extraction, wait transaction on ZkSync side provides timeout error
-        tx_hash = None
-        for log in tx_receipt["logs"]:
-            if log.address.lower() == main_contract.address.lower():
-                tx_hash = log.transactionHash
-                break
-        if tx_hash is None:
-            raise RuntimeError("Failed to parse tx logs")
-        return tx_hash
+        logs = main_contract.parse_events(tx_receipt, "NewPriorityRequest")
+        if len(logs):
+            return logs[0].args.txHash
+        else:
+            raise RuntimeError("Wrong transaction received")
 
     def get_l2_transaction_from_priority_op(self, tx_receipt, main_contract: ZkSyncContract):
         l2_hash = self.get_l2_hash_from_priority_op(tx_receipt, main_contract)
-        # INFO: loop to get the transaction in chain
         self.wait_for_transaction_receipt(l2_hash)
         return self.get_transaction(l2_hash)
 
     def get_priority_op_response(self, tx_receipt, main_contract: ZkSyncContract):
         tx = self.get_l2_transaction_from_priority_op(tx_receipt, main_contract)
         return tx
 
@@ -356,35 +351,33 @@
                             tx_receipt["blockHash"] is not None:
                         break
                     _timeout.sleep(poll_latency)
             return tx_receipt
 
         except Timeout:
             raise TimeExhausted(
-                f"Transaction {HexBytes(transaction_hash) !r} is not in the chain "
-                f"after {timeout} seconds"
+                f"Transaction {HexBytes(transaction_hash) !r} is not in the chain after {timeout} seconds"
             )
 
     def wait_finalized(self,
                        transaction_hash: _Hash32,
                        timeout: float = 120,
                        poll_latency: float = 0.1) -> TxReceipt:
         try:
             with Timeout(timeout) as _timeout:
                 while True:
                     try:
-                        block = self.get_block('finalized')
+                        block = self.get_block("finalized")
                         tx_receipt = self.get_transaction_receipt(transaction_hash)
                     except TransactionNotFound:
                         tx_receipt = None
                     if tx_receipt is not None and \
                             tx_receipt["blockHash"] is not None and \
-                            block['number'] >= tx_receipt['blockNumber']:
+                            block["number"] >= tx_receipt["blockNumber"]:
                         break
                     _timeout.sleep(poll_latency)
             return tx_receipt
 
         except Timeout:
             raise TimeExhausted(
-                f"Transaction {HexBytes(transaction_hash) !r} is not in the chain "
-                f"after {timeout} seconds"
+                f"Transaction {HexBytes(transaction_hash) !r} is not in the chain after {timeout} seconds"
             )
```

### Comparing `zksync2-0.4.0/zksync2/module/zksync_provider.py` & `zksync2-0.5.0/zksync2/module/zksync_provider.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/provider/eth_provider.py` & `zksync2-0.5.0/zksync2/provider/eth_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                            f" for the transaction: base_cost: ${base_cost},"
                            f" provided value: ${value}`")
 
 
 class EthereumProvider:
     # GAS_LIMIT = 21000
     # DEFAULT_THRESHOLD = 2 ** 255
-    DEPOSIT_GAS_PER_PUBDATA_LIMIT = 50000
+    DEPOSIT_GAS_PER_PUBDATA_LIMIT = 800
     RECOMMENDED_DEPOSIT_L2_GAS_LIMIT = 10000000
     L1_MESSENGER_ADDRESS = '0x0000000000000000000000000000000000008008'
 
     def __init__(self,
                  zksync_web3: Web3,
                  eth_web3: Web3,
                  l1_account: BaseAccount):
@@ -121,15 +121,17 @@
             to = self.address
 
         if gas_price is None:
             gas_price = self._eth_web3.eth.gas_price
         if gas_limit is None:
             gas_limit = RecommendedGasLimit.DEPOSIT.value
 
-        base_cost = 0
+        base_cost = self.get_base_cost(gas_price=gas_price,
+                                       gas_per_pubdata_byte=gas_per_pubdata_byte,
+                                       gas_limit=gas_limit)
 
         if token.is_eth():
             value = base_cost + operator_tip + amount
             return self.request_execute(
                 contract_address=to,
                 call_data=HexStr("0x"),
                 l2_gas_limit=l2_gas_limit,
@@ -139,25 +141,23 @@
                 gas_limit=gas_limit,
                 l1_value=value)
         else:
             value = base_cost + operator_tip
             check_base_cost(base_cost, value)
 
             if approve_erc20:
-                approve_tx = self.approve_erc20(token,
-                                                amount,
-                                                bridge_address,
-                                                gas_limit)
+                self.approve_erc20(token,
+                                   amount,
+                                   bridge_address,
+                                   gas_limit)
             tx_receipt = bridge_contract.deposit(l2_receiver=to,
                                                  l1_token=token.l1_address,
                                                  amount=amount,
                                                  l2_tx_gas_limit=l2_gas_limit,
                                                  l2_tx_gas_per_pubdata_byte=gas_per_pubdata_byte)
-            # TODO: resolve issue with getting L2 tx_hash from logs
-            # return self._zksync_web3.zksync.get_priority_op_response(tx_receipt, self.main_contract)
             return tx_receipt
 
     def request_execute(self,
                         contract_address: HexStr,
                         call_data: Union[bytes, HexStr],
                         l2_gas_limit: int,
                         l1_value: int,
@@ -190,16 +190,14 @@
                                                                l2_gas_limit=l2_gas_limit,
                                                                l2_gas_per_pubdata_byte_limit=gas_per_pubdata_byte,
                                                                factory_deps=factory_deps,
                                                                refund_recipient=refund_recipient,
                                                                gas_price=gas_price,
                                                                gas_limit=gas_limit,
                                                                l1_value=l1_value)
-        # TODO: resolve issue with getting L2 tx_hash from logs
-        # return self._zksync_web3.zksync.get_priority_op_response(tx_receipt, self.main_contract)
         return tx_receipt
 
     def _get_withdraw_log(self, tx_receipt: TxReceipt, index: int = 0):
         topic = event_signature_to_log_topic("L1MessageSent(address,bytes32,bytes)")
 
         def impl_filter(log):
             return log['address'] == self.L1_MESSENGER_ADDRESS and \
```

### Comparing `zksync2-0.4.0/zksync2/signer/eth_signer.py` & `zksync2-0.5.0/zksync2/signer/eth_signer.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/transaction/transaction712.py` & `zksync2-0.5.0/zksync2/transaction/transaction712.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2/transaction/transaction_builders.py` & `zksync2-0.5.0/zksync2/transaction/transaction_builders.py`

 * *Files identical despite different names*

### Comparing `zksync2-0.4.0/zksync2.egg-info/PKG-INFO` & `zksync2-0.5.0/zksync2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: zksync2
-Version: 0.4.0
+Version: 0.5.0
 Summary: zkSync2 python client sdk
 Home-page: https://zksync.io
-Author: Viktor Yastrebov
-Author-email: Viktor Yastrebov <vyastrebov@vareger.com>
+Author: Danijel Radakovic
+Author-email: Danijel Radakovic <danijel@txfusion.io>
 License: MIT
 Project-URL: Homepage, https://github.com/zksync-sdk/zksync2-python
 Project-URL: Bug Tracker, https://github.com/zksync-sdk/zksync2-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -26,18 +26,18 @@
 - [Contract interfaces](#contract-interfaces)
 - [Examples](#examples)
 
 
 ### Getting started
 
 #### Requirements
-| Tool            | Required |
-|-----------------|----------|
-| python          | >= 3.10  |
-| package manager | pip      |
+| Tool            | Required       |
+|-----------------|----------------|
+| python          | 3.8, 3.9, 3.10 |
+| package manager | pip            |
 
 ### how to install
 
 ```console
 pip install zksync2
 ```
 
@@ -328,19 +328,20 @@
 * encode_general
 
 For example and usage, please have a look into example [section](#examples)
 
 
 ### Examples
 
+* [check balance](./examples/11_check_balance.py)
 * [deposit funds](./examples/01_deposit.py)
-* [check balance](./examples/12_misc.py)
 * [transfer](./examples/02_transfer.py)
 * [transfer erc20 tokens](./examples/03_transfer_erc20_token.py)
-* [withdraw funds](./examples/11_withdrawal.py)
+* [withdraw funds](./examples/09_withdrawal.py)
+* [finalize withdrawal](./examples/10_finalize_withdrawal.py)
 * [deploy contract, precompute address by create](./examples/04_deploy_create.py)
-* [deploy contract with constructor(create method)](./examples/05_deploy_create_with_ctor.py)
+* [deploy contract with constructor(create method) and interact with contract](./examples/05_deploy_create_with_constructor.py)
 * [deploy contract with dependent contract(create method)](./examples/06_deploy_create_with_deps.py)
 * [deploy contract, precompute address by create2](./examples/07_deploy_create2.py)
 * [deploy contract with dependency, precompute address by create2](./examples/08_deploy_create2_deps.py)
-* [execute contracts method](./examples/09_execute_contract.py)
-* [support legacy transaction for call/execute contracts methods](./examples/10_execute_legacy.py)
+* [how to compile solidity contracts](./examples/README.md)
+
```

