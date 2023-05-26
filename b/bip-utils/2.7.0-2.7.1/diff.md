# Comparing `tmp/bip_utils-2.7.0.tar.gz` & `tmp/bip_utils-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bip_utils-2.7.0.tar", last modified: Thu Oct  6 12:40:42 2022, max compression
+gzip compressed data, was "bip_utils-2.7.1.tar", last modified: Fri May 26 12:02:28 2023, max compression
```

## Comparing `bip_utils-2.7.0.tar` & `bip_utils-2.7.1.tar`

### file list

```diff
@@ -1,444 +1,445 @@
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.332033 bip_utils-2.7.0/
--rw-rw-rw-   0        0        0     1085 2022-07-29 18:35:18.000000 bip_utils-2.7.0/LICENSE
--rw-rw-rw-   0        0        0      122 2022-08-23 19:50:06.000000 bip_utils-2.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11665 2022-10-06 12:40:42.333032 bip_utils-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     9816 2022-08-11 20:10:26.000000 bip_utils-2.7.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.369070 bip_utils-2.7.0/bip_utils/
--rw-rw-rw-   0        0        0     8531 2022-09-13 12:39:13.000000 bip_utils-2.7.0/bip_utils/__init__.py
--rw-rw-rw-   0        0        0       28 2022-10-06 12:22:26.000000 bip_utils-2.7.0/bip_utils/_version.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.598231 bip_utils-2.7.0/bip_utils/addr/
--rw-rw-rw-   0        0        0     7500 2022-09-13 12:39:23.000000 bip_utils-2.7.0/bip_utils/addr/P2PKH_addr.py
--rw-rw-rw-   0        0        0     6130 2022-09-13 12:39:23.000000 bip_utils-2.7.0/bip_utils/addr/P2SH_addr.py
--rw-rw-rw-   0        0        0     7281 2022-09-13 12:39:24.000000 bip_utils-2.7.0/bip_utils/addr/P2TR_addr.py
--rw-rw-rw-   0        0        0     4204 2022-09-13 12:39:24.000000 bip_utils-2.7.0/bip_utils/addr/P2WPKH_addr.py
--rw-rw-rw-   0        0        0     3247 2022-09-13 12:39:14.000000 bip_utils-2.7.0/bip_utils/addr/__init__.py
--rw-rw-rw-   0        0        0    18494 2022-09-13 12:39:14.000000 bip_utils-2.7.0/bip_utils/addr/ada_byron_addr.py
--rw-rw-rw-   0        0        0    11262 2022-09-13 12:39:15.000000 bip_utils-2.7.0/bip_utils/addr/ada_shelley_addr.py
--rw-rw-rw-   0        0        0     4791 2022-09-13 12:39:15.000000 bip_utils-2.7.0/bip_utils/addr/addr_dec_utils.py
--rw-rw-rw-   0        0        0     6010 2022-09-13 12:39:16.000000 bip_utils-2.7.0/bip_utils/addr/addr_key_validator.py
--rw-rw-rw-   0        0        0     4658 2022-09-13 12:39:16.000000 bip_utils-2.7.0/bip_utils/addr/algo_addr.py
--rw-rw-rw-   0        0        0     3572 2022-09-13 12:39:17.000000 bip_utils-2.7.0/bip_utils/addr/atom_addr.py
--rw-rw-rw-   0        0        0     5774 2022-09-13 12:39:18.000000 bip_utils-2.7.0/bip_utils/addr/avax_addr.py
--rw-rw-rw-   0        0        0     2377 2022-09-13 12:39:18.000000 bip_utils-2.7.0/bip_utils/addr/bch_addr_converter.py
--rw-rw-rw-   0        0        0     3695 2022-09-13 12:39:19.000000 bip_utils-2.7.0/bip_utils/addr/egld_addr.py
--rw-rw-rw-   0        0        0     4831 2022-09-13 12:39:19.000000 bip_utils-2.7.0/bip_utils/addr/eos_addr.py
--rw-rw-rw-   0        0        0     6397 2022-09-13 12:39:19.000000 bip_utils-2.7.0/bip_utils/addr/ergo_addr.py
--rw-rw-rw-   0        0        0     5227 2022-09-13 12:39:20.000000 bip_utils-2.7.0/bip_utils/addr/eth_addr.py
--rw-rw-rw-   0        0        0     6871 2022-09-13 12:39:20.000000 bip_utils-2.7.0/bip_utils/addr/fil_addr.py
--rw-rw-rw-   0        0        0     1881 2022-09-13 12:39:20.000000 bip_utils-2.7.0/bip_utils/addr/iaddr_decoder.py
--rw-rw-rw-   0        0        0     1982 2022-09-13 12:39:21.000000 bip_utils-2.7.0/bip_utils/addr/iaddr_encoder.py
--rw-rw-rw-   0        0        0     3824 2022-09-13 12:39:21.000000 bip_utils-2.7.0/bip_utils/addr/icx_addr.py
--rw-rw-rw-   0        0        0     5459 2022-09-13 12:39:21.000000 bip_utils-2.7.0/bip_utils/addr/nano_addr.py
--rw-rw-rw-   0        0        0     3416 2022-09-13 12:39:22.000000 bip_utils-2.7.0/bip_utils/addr/near_addr.py
--rw-rw-rw-   0        0        0     4380 2022-09-13 12:39:22.000000 bip_utils-2.7.0/bip_utils/addr/neo_addr.py
--rw-rw-rw-   0        0        0     3742 2022-09-13 12:39:22.000000 bip_utils-2.7.0/bip_utils/addr/okex_addr.py
--rw-rw-rw-   0        0        0     3731 2022-09-13 12:39:23.000000 bip_utils-2.7.0/bip_utils/addr/one_addr.py
--rw-rw-rw-   0        0        0     3387 2022-09-13 12:39:25.000000 bip_utils-2.7.0/bip_utils/addr/sol_addr.py
--rw-rw-rw-   0        0        0     6173 2022-09-13 12:39:25.000000 bip_utils-2.7.0/bip_utils/addr/substrate_addr.py
--rw-rw-rw-   0        0        0     4151 2022-09-13 12:39:25.000000 bip_utils-2.7.0/bip_utils/addr/trx_addr.py
--rw-rw-rw-   0        0        0     5891 2022-09-13 12:39:26.000000 bip_utils-2.7.0/bip_utils/addr/xlm_addr.py
--rw-rw-rw-   0        0        0    10588 2022-09-13 12:39:26.000000 bip_utils-2.7.0/bip_utils/addr/xmr_addr.py
--rw-rw-rw-   0        0        0     3454 2022-09-13 12:39:26.000000 bip_utils-2.7.0/bip_utils/addr/xrp_addr.py
--rw-rw-rw-   0        0        0     4629 2022-09-13 12:39:27.000000 bip_utils-2.7.0/bip_utils/addr/xtz_addr.py
--rw-rw-rw-   0        0        0     3828 2022-09-13 12:39:27.000000 bip_utils-2.7.0/bip_utils/addr/zil_addr.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.603231 bip_utils-2.7.0/bip_utils/algorand/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:39:27.000000 bip_utils-2.7.0/bip_utils/algorand/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.657230 bip_utils-2.7.0/bip_utils/algorand/mnemonic/
--rw-rw-rw-   0        0        0      688 2022-09-13 12:39:28.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     3145 2022-09-13 12:39:28.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_entropy_generator.py
--rw-rw-rw-   0        0        0     1994 2022-09-13 12:39:29.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic.py
--rw-rw-rw-   0        0        0     5234 2022-09-13 12:39:29.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     3907 2022-09-13 12:39:30.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     4297 2022-09-13 12:39:30.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py
--rw-rw-rw-   0        0        0     3852 2022-09-13 12:39:31.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py
--rw-rw-rw-   0        0        0     2144 2022-09-13 12:39:31.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py
--rw-rw-rw-   0        0        0     2779 2022-09-13 12:39:32.000000 bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_seed_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.677231 bip_utils-2.7.0/bip_utils/base58/
--rw-rw-rw-   0        0        0      219 2022-09-13 12:39:32.000000 bip_utils-2.7.0/bip_utils/base58/__init__.py
--rw-rw-rw-   0        0        0     7113 2022-09-13 12:39:33.000000 bip_utils-2.7.0/bip_utils/base58/base58.py
--rw-rw-rw-   0        0        0     1247 2022-09-13 12:39:33.000000 bip_utils-2.7.0/bip_utils/base58/base58_ex.py
--rw-rw-rw-   0        0        0     5462 2022-09-25 20:02:30.000000 bip_utils-2.7.0/bip_utils/base58/base58_xmr.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.713229 bip_utils-2.7.0/bip_utils/bech32/
--rw-rw-rw-   0        0        0      287 2022-09-13 12:39:34.000000 bip_utils-2.7.0/bip_utils/bech32/__init__.py
--rw-rw-rw-   0        0        0     6863 2022-09-13 12:39:34.000000 bip_utils-2.7.0/bip_utils/bech32/bch_bech32.py
--rw-rw-rw-   0        0        0     7472 2022-09-13 12:39:34.000000 bip_utils-2.7.0/bip_utils/bech32/bech32.py
--rw-rw-rw-   0        0        0     8249 2022-09-13 12:39:35.000000 bip_utils-2.7.0/bip_utils/bech32/bech32_base.py
--rw-rw-rw-   0        0        0     1247 2022-09-13 12:39:35.000000 bip_utils-2.7.0/bip_utils/bech32/bech32_ex.py
--rw-rw-rw-   0        0        0     6264 2022-09-26 19:44:08.000000 bip_utils-2.7.0/bip_utils/bech32/segwit_bech32.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.717229 bip_utils-2.7.0/bip_utils/bip/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:39:36.000000 bip_utils-2.7.0/bip_utils/bip/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.769229 bip_utils-2.7.0/bip_utils/bip/bip32/
--rw-rw-rw-   0        0        0     1354 2022-09-13 12:39:37.000000 bip_utils-2.7.0/bip_utils/bip/bip32/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.790230 bip_utils-2.7.0/bip_utils/bip/bip32/base/
--rw-rw-rw-   0        0        0      222 2022-09-13 12:39:37.000000 bip_utils-2.7.0/bip_utils/bip/bip32/base/__init__.py
--rw-rw-rw-   0        0        0    21303 2022-09-13 12:39:37.000000 bip_utils-2.7.0/bip_utils/bip/bip32/base/bip32_base.py
--rw-rw-rw-   0        0        0     3130 2022-09-13 12:39:38.000000 bip_utils-2.7.0/bip_utils/bip/bip32/base/ibip32_key_derivator.py
--rw-rw-rw-   0        0        0     1897 2022-09-13 12:39:39.000000 bip_utils-2.7.0/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py
--rw-rw-rw-   0        0        0     1835 2022-09-13 12:39:39.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_const.py
--rw-rw-rw-   0        0        0     1318 2022-09-13 12:39:39.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_ex.py
--rw-rw-rw-   0        0        0    14058 2022-09-13 12:39:40.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_key_data.py
--rw-rw-rw-   0        0        0     2694 2022-09-13 12:39:40.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_key_net_ver.py
--rw-rw-rw-   0        0        0    10535 2022-09-13 12:39:41.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_key_ser.py
--rw-rw-rw-   0        0        0    15183 2022-09-13 12:39:41.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_keys.py
--rw-rw-rw-   0        0        0     7428 2022-09-13 12:39:42.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_path.py
--rw-rw-rw-   0        0        0     2346 2022-09-13 12:39:42.000000 bip_utils-2.7.0/bip_utils/bip/bip32/bip32_utils.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.822235 bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/
--rw-rw-rw-   0        0        0      418 2022-09-13 12:39:43.000000 bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/__init__.py
--rw-rw-rw-   0        0        0     3093 2022-09-13 12:39:43.000000 bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py
--rw-rw-rw-   0        0        0     4850 2022-09-13 12:39:44.000000 bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py
--rw-rw-rw-   0        0        0     8071 2022-09-13 12:39:44.000000 bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py
--rw-rw-rw-   0        0        0     4899 2022-09-13 12:39:45.000000 bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.860229 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/
--rw-rw-rw-   0        0        0      728 2022-09-13 12:39:45.000000 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/__init__.py
--rw-rw-rw-   0        0        0     3058 2022-09-13 12:39:46.000000 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py
--rw-rw-rw-   0        0        0     1905 2022-09-13 12:39:46.000000 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py
--rw-rw-rw-   0        0        0     7389 2022-09-13 12:39:46.000000 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py
--rw-rw-rw-   0        0        0     6708 2022-09-13 12:39:47.000000 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py
--rw-rw-rw-   0        0        0     3070 2022-09-13 12:39:48.000000 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py
--rw-rw-rw-   0        0        0     3066 2022-09-13 12:39:48.000000 bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.882230 bip_utils-2.7.0/bip_utils/bip/bip38/
--rw-rw-rw-   0        0        0      194 2022-09-13 12:39:49.000000 bip_utils-2.7.0/bip_utils/bip/bip38/__init__.py
--rw-rw-rw-   0        0        0     5286 2022-09-13 12:39:49.000000 bip_utils-2.7.0/bip_utils/bip/bip38/bip38.py
--rw-rw-rw-   0        0        0     2665 2022-09-13 12:39:49.000000 bip_utils-2.7.0/bip_utils/bip/bip38/bip38_addr.py
--rw-rw-rw-   0        0        0    21332 2022-09-13 12:39:50.000000 bip_utils-2.7.0/bip_utils/bip/bip38/bip38_ec.py
--rw-rw-rw-   0        0        0    11382 2022-09-13 12:39:50.000000 bip_utils-2.7.0/bip_utils/bip/bip38/bip38_no_ec.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.934232 bip_utils-2.7.0/bip_utils/bip/bip39/
--rw-rw-rw-   0        0        0      656 2022-09-13 12:39:51.000000 bip_utils-2.7.0/bip_utils/bip/bip39/__init__.py
--rw-rw-rw-   0        0        0     3376 2022-09-13 12:39:51.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_entropy_generator.py
--rw-rw-rw-   0        0        0     3559 2022-09-13 12:39:52.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic.py
--rw-rw-rw-   0        0        0     7931 2022-09-13 12:39:52.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     3997 2022-09-13 12:39:53.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     4021 2022-09-13 12:39:54.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_generator.py
--rw-rw-rw-   0        0        0     3809 2022-09-13 12:39:54.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_utils.py
--rw-rw-rw-   0        0        0     1850 2022-09-13 12:39:55.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_validator.py
--rw-rw-rw-   0        0        0     3486 2022-09-13 12:39:55.000000 bip_utils-2.7.0/bip_utils/bip/bip39/bip39_seed_generator.py
--rw-rw-rw-   0        0        0     2228 2022-09-13 12:39:55.000000 bip_utils-2.7.0/bip_utils/bip/bip39/ibip39_seed_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.009232 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/
--rw-rw-rw-   0        0        0    10240 2022-09-13 12:39:56.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/chinese_simplified.txt
--rw-rw-rw-   0        0        0    10240 2022-09-13 12:39:56.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/chinese_traditional.txt
--rw-rw-rw-   0        0        0    16993 2022-09-13 12:39:56.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/czech.txt
--rw-rw-rw-   0        0        0    15164 2022-09-13 12:39:57.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/english.txt
--rw-rw-rw-   0        0        0    18825 2022-09-13 12:39:57.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/french.txt
--rw-rw-rw-   0        0        0    18081 2022-09-13 12:39:58.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/italian.txt
--rw-rw-rw-   0        0        0    39880 2022-09-13 12:39:58.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/korean.txt
--rw-rw-rw-   0        0        0    17719 2022-09-13 12:39:59.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/portuguese.txt
--rw-rw-rw-   0        0        0    16044 2022-09-13 12:39:59.000000 bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/spanish.txt
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.024230 bip_utils-2.7.0/bip_utils/bip/bip44/
--rw-rw-rw-   0        0        0       45 2022-09-13 12:40:00.000000 bip_utils-2.7.0/bip_utils/bip/bip44/__init__.py
--rw-rw-rw-   0        0        0     8919 2022-09-13 12:40:00.000000 bip_utils-2.7.0/bip_utils/bip/bip44/bip44.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.043229 bip_utils-2.7.0/bip_utils/bip/bip44_base/
--rw-rw-rw-   0        0        0      235 2022-09-13 12:40:00.000000 bip_utils-2.7.0/bip_utils/bip/bip44_base/__init__.py
--rw-rw-rw-   0        0        0    21706 2022-09-13 12:40:01.000000 bip_utils-2.7.0/bip_utils/bip/bip44_base/bip44_base.py
--rw-rw-rw-   0        0        0     1255 2022-09-13 12:40:01.000000 bip_utils-2.7.0/bip_utils/bip/bip44_base/bip44_base_ex.py
--rw-rw-rw-   0        0        0     7297 2022-09-13 12:40:02.000000 bip_utils-2.7.0/bip_utils/bip/bip44_base/bip44_keys.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.051229 bip_utils-2.7.0/bip_utils/bip/bip49/
--rw-rw-rw-   0        0        0       45 2022-09-13 12:40:02.000000 bip_utils-2.7.0/bip_utils/bip/bip49/__init__.py
--rw-rw-rw-   0        0        0     8919 2022-09-13 12:40:03.000000 bip_utils-2.7.0/bip_utils/bip/bip49/bip49.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.060229 bip_utils-2.7.0/bip_utils/bip/bip84/
--rw-rw-rw-   0        0        0       45 2022-09-13 12:40:03.000000 bip_utils-2.7.0/bip_utils/bip/bip84/__init__.py
--rw-rw-rw-   0        0        0     8919 2022-09-13 12:40:04.000000 bip_utils-2.7.0/bip_utils/bip/bip84/bip84.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.068230 bip_utils-2.7.0/bip_utils/bip/bip86/
--rw-rw-rw-   0        0        0       45 2022-09-13 12:40:04.000000 bip_utils-2.7.0/bip_utils/bip/bip86/__init__.py
--rw-rw-rw-   0        0        0     8917 2022-09-13 12:40:05.000000 bip_utils-2.7.0/bip_utils/bip/bip86/bip86.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.071231 bip_utils-2.7.0/bip_utils/bip/conf/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:05.000000 bip_utils-2.7.0/bip_utils/bip/conf/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.092230 bip_utils-2.7.0/bip_utils/bip/conf/bip44/
--rw-rw-rw-   0        0        0      192 2022-09-13 12:40:06.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip44/__init__.py
--rw-rw-rw-   0        0        0     3317 2022-09-13 12:40:06.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip44/bip44_coins.py
--rw-rw-rw-   0        0        0    41152 2022-09-13 12:40:06.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip44/bip44_conf.py
--rw-rw-rw-   0        0        0     6464 2022-09-13 12:40:07.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip44/bip44_conf_getter.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.111229 bip_utils-2.7.0/bip_utils/bip/conf/bip49/
--rw-rw-rw-   0        0        0      192 2022-09-13 12:40:07.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip49/__init__.py
--rw-rw-rw-   0        0        0     1879 2022-09-13 12:40:08.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip49/bip49_coins.py
--rw-rw-rw-   0        0        0    15121 2022-09-13 12:40:08.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip49/bip49_conf.py
--rw-rw-rw-   0        0        0     3404 2022-09-13 12:40:09.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip49/bip49_conf_getter.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.130230 bip_utils-2.7.0/bip_utils/bip/conf/bip84/
--rw-rw-rw-   0        0        0      192 2022-09-13 12:40:09.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip84/__init__.py
--rw-rw-rw-   0        0        0     1493 2022-09-13 12:40:10.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip84/bip84_coins.py
--rw-rw-rw-   0        0        0     4193 2022-09-13 12:40:10.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip84/bip84_conf.py
--rw-rw-rw-   0        0        0     2542 2022-09-13 12:40:11.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip84/bip84_conf_getter.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.152230 bip_utils-2.7.0/bip_utils/bip/conf/bip86/
--rw-rw-rw-   0        0        0      192 2022-09-13 12:40:11.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip86/__init__.py
--rw-rw-rw-   0        0        0     1439 2022-09-13 12:40:12.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip86/bip86_coins.py
--rw-rw-rw-   0        0        0     2948 2022-09-13 12:40:12.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip86/bip86_conf.py
--rw-rw-rw-   0        0        0     2420 2022-09-13 12:40:12.000000 bip_utils-2.7.0/bip_utils/bip/conf/bip86/bip86_conf_getter.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.185227 bip_utils-2.7.0/bip_utils/bip/conf/common/
--rw-rw-rw-   0        0        0      392 2022-09-13 12:40:13.000000 bip_utils-2.7.0/bip_utils/bip/conf/common/__init__.py
--rw-rw-rw-   0        0        0     4411 2022-09-13 12:40:13.000000 bip_utils-2.7.0/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py
--rw-rw-rw-   0        0        0     7042 2022-09-13 12:40:14.000000 bip_utils-2.7.0/bip_utils/bip/conf/common/bip_coin_conf.py
--rw-rw-rw-   0        0        0     1260 2022-09-13 12:40:14.000000 bip_utils-2.7.0/bip_utils/bip/conf/common/bip_coins.py
--rw-rw-rw-   0        0        0     1306 2022-09-13 12:40:15.000000 bip_utils-2.7.0/bip_utils/bip/conf/common/bip_conf_const.py
--rw-rw-rw-   0        0        0     5101 2022-09-13 12:40:15.000000 bip_utils-2.7.0/bip_utils/bip/conf/common/bip_litecoin_conf.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.188228 bip_utils-2.7.0/bip_utils/cardano/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:16.000000 bip_utils-2.7.0/bip_utils/cardano/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.213229 bip_utils-2.7.0/bip_utils/cardano/bip32/
--rw-rw-rw-   0        0        0      165 2022-09-13 12:40:16.000000 bip_utils-2.7.0/bip_utils/cardano/bip32/__init__.py
--rw-rw-rw-   0        0        0     3051 2022-09-13 12:40:16.000000 bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py
--rw-rw-rw-   0        0        0     4290 2022-09-13 12:40:17.000000 bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py
--rw-rw-rw-   0        0        0     4426 2022-09-13 12:40:17.000000 bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py
--rw-rw-rw-   0        0        0     1975 2022-09-13 12:40:18.000000 bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_icarus_bip32.py
--rw-rw-rw-   0        0        0     4150 2022-09-13 12:40:18.000000 bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.220229 bip_utils-2.7.0/bip_utils/cardano/byron/
--rw-rw-rw-   0        0        0       77 2022-09-13 12:40:18.000000 bip_utils-2.7.0/bip_utils/cardano/byron/__init__.py
--rw-rw-rw-   0        0        0     9560 2022-09-13 12:40:19.000000 bip_utils-2.7.0/bip_utils/cardano/byron/cardano_byron_legacy.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.228230 bip_utils-2.7.0/bip_utils/cardano/cip1852/
--rw-rw-rw-   0        0        0       55 2022-09-13 12:40:19.000000 bip_utils-2.7.0/bip_utils/cardano/cip1852/__init__.py
--rw-rw-rw-   0        0        0     8713 2022-09-13 12:40:20.000000 bip_utils-2.7.0/bip_utils/cardano/cip1852/cip1852.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.246231 bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/
--rw-rw-rw-   0        0        0      222 2022-09-13 12:40:20.000000 bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/__init__.py
--rw-rw-rw-   0        0        0     1495 2022-09-13 12:40:20.000000 bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/cip1852_coins.py
--rw-rw-rw-   0        0        0     3766 2022-09-13 12:40:21.000000 bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/cip1852_conf.py
--rw-rw-rw-   0        0        0     2652 2022-09-13 12:40:21.000000 bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.260231 bip_utils-2.7.0/bip_utils/cardano/mnemonic/
--rw-rw-rw-   0        0        0      205 2022-09-13 12:40:21.000000 bip_utils-2.7.0/bip_utils/cardano/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     2656 2022-09-13 12:40:22.000000 bip_utils-2.7.0/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py
--rw-rw-rw-   0        0        0     2513 2022-09-13 12:40:22.000000 bip_utils-2.7.0/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.282229 bip_utils-2.7.0/bip_utils/cardano/shelley/
--rw-rw-rw-   0        0        0      182 2022-09-13 12:40:22.000000 bip_utils-2.7.0/bip_utils/cardano/shelley/__init__.py
--rw-rw-rw-   0        0        0     7138 2022-09-13 12:40:23.000000 bip_utils-2.7.0/bip_utils/cardano/shelley/cardano_shelley.py
--rw-rw-rw-   0        0        0     6383 2022-09-13 12:40:24.000000 bip_utils-2.7.0/bip_utils/cardano/shelley/cardano_shelley_keys.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.316230 bip_utils-2.7.0/bip_utils/coin_conf/
--rw-rw-rw-   0        0        0      106 2022-09-13 12:40:24.000000 bip_utils-2.7.0/bip_utils/coin_conf/__init__.py
--rw-rw-rw-   0        0        0     2258 2022-09-13 12:40:24.000000 bip_utils-2.7.0/bip_utils/coin_conf/coin_conf.py
--rw-rw-rw-   0        0        0    22166 2022-09-13 12:40:25.000000 bip_utils-2.7.0/bip_utils/coin_conf/coins_conf.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.327229 bip_utils-2.7.0/bip_utils/ecc/
--rw-rw-rw-   0        0        0     2046 2022-09-15 14:56:47.000000 bip_utils-2.7.0/bip_utils/ecc/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.376229 bip_utils-2.7.0/bip_utils/ecc/common/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:25.000000 bip_utils-2.7.0/bip_utils/ecc/common/__init__.py
--rw-rw-rw-   0        0        0     4994 2022-09-13 12:40:26.000000 bip_utils-2.7.0/bip_utils/ecc/common/dummy_point.py
--rw-rw-rw-   0        0        0     6654 2022-09-13 12:40:26.000000 bip_utils-2.7.0/bip_utils/ecc/common/ikeys.py
--rw-rw-rw-   0        0        0     4620 2022-09-13 12:40:26.000000 bip_utils-2.7.0/bip_utils/ecc/common/ipoint.py
--rw-rw-rw-   0        0        0     1315 2022-10-06 12:26:58.000000 bip_utils-2.7.0/bip_utils/ecc/conf.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.420232 bip_utils-2.7.0/bip_utils/ecc/curve/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:27.000000 bip_utils-2.7.0/bip_utils/ecc/curve/__init__.py
--rw-rw-rw-   0        0        0     3851 2022-09-13 12:40:27.000000 bip_utils-2.7.0/bip_utils/ecc/curve/elliptic_curve.py
--rw-rw-rw-   0        0        0     3135 2022-09-13 12:40:28.000000 bip_utils-2.7.0/bip_utils/ecc/curve/elliptic_curve_getter.py
--rw-rw-rw-   0        0        0     1486 2022-09-13 12:40:28.000000 bip_utils-2.7.0/bip_utils/ecc/curve/elliptic_curve_types.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.434232 bip_utils-2.7.0/bip_utils/ecc/ecdsa/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:28.000000 bip_utils-2.7.0/bip_utils/ecc/ecdsa/__init__.py
--rw-rw-rw-   0        0        0     1659 2022-09-13 12:40:29.000000 bip_utils-2.7.0/bip_utils/ecc/ecdsa/ecdsa_keys.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.478233 bip_utils-2.7.0/bip_utils/ecc/ed25519/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:29.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/__init__.py
--rw-rw-rw-   0        0        0     1828 2022-09-13 12:40:29.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519.py
--rw-rw-rw-   0        0        0     1761 2022-09-13 12:40:30.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_const.py
--rw-rw-rw-   0        0        0     7409 2022-10-06 12:31:30.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_keys.py
--rw-rw-rw-   0        0        0     6467 2022-09-24 21:12:51.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_point.py
--rw-rw-rw-   0        0        0     2307 2022-09-22 18:31:27.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_utils.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.487232 bip_utils-2.7.0/bip_utils/ecc/ed25519/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:32.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/lib/__init__.py
--rw-rw-rw-   0        0        0    10382 2022-09-26 10:52:41.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519/lib/ed25519_lib.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.515230 bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:33.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/__init__.py
--rw-rw-rw-   0        0        0     2003 2022-09-13 12:40:33.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py
--rw-rw-rw-   0        0        0     1573 2022-09-13 12:40:33.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py
--rw-rw-rw-   0        0        0     7358 2022-09-22 18:30:36.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py
--rw-rw-rw-   0        0        0     1646 2022-09-13 12:40:35.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.538230 bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:35.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/__init__.py
--rw-rw-rw-   0        0        0     1980 2022-09-13 12:40:35.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py
--rw-rw-rw-   0        0        0     1576 2022-09-13 12:40:36.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py
--rw-rw-rw-   0        0        0     5303 2022-09-22 18:51:23.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py
--rw-rw-rw-   0        0        0     1642 2022-09-13 12:40:36.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.562232 bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:37.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/__init__.py
--rw-rw-rw-   0        0        0     1980 2022-09-13 12:40:37.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero.py
--rw-rw-rw-   0        0        0     1780 2022-09-13 12:40:37.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py
--rw-rw-rw-   0        0        0     4174 2022-09-26 10:52:41.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py
--rw-rw-rw-   0        0        0     1642 2022-09-15 10:52:38.000000 bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.587229 bip_utils-2.7.0/bip_utils/ecc/nist256p1/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:40.000000 bip_utils-2.7.0/bip_utils/ecc/nist256p1/__init__.py
--rw-rw-rw-   0        0        0     1876 2022-09-13 12:40:40.000000 bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1.py
--rw-rw-rw-   0        0        0     1606 2022-09-13 12:40:40.000000 bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1_const.py
--rw-rw-rw-   0        0        0     7231 2022-09-13 12:40:41.000000 bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1_keys.py
--rw-rw-rw-   0        0        0     6754 2022-09-13 12:40:41.000000 bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1_point.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.626229 bip_utils-2.7.0/bip_utils/ecc/secp256k1/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:42.000000 bip_utils-2.7.0/bip_utils/ecc/secp256k1/__init__.py
--rw-rw-rw-   0        0        0     1783 2022-09-13 12:40:42.000000 bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1.py
--rw-rw-rw-   0        0        0     2974 2022-09-13 12:40:43.000000 bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_const.py
--rw-rw-rw-   0        0        0     7065 2022-09-13 12:40:43.000000 bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py
--rw-rw-rw-   0        0        0     7301 2022-09-13 12:40:44.000000 bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py
--rw-rw-rw-   0        0        0     5960 2022-09-13 12:40:44.000000 bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py
--rw-rw-rw-   0        0        0     6800 2022-09-13 12:40:45.000000 bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.652230 bip_utils-2.7.0/bip_utils/ecc/sr25519/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:40:45.000000 bip_utils-2.7.0/bip_utils/ecc/sr25519/__init__.py
--rw-rw-rw-   0        0        0     1828 2022-09-13 12:40:45.000000 bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519.py
--rw-rw-rw-   0        0        0     1562 2022-09-13 12:40:46.000000 bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519_const.py
--rw-rw-rw-   0        0        0     6498 2022-09-13 12:40:46.000000 bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519_keys.py
--rw-rw-rw-   0        0        0     1321 2022-09-13 12:40:46.000000 bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519_point.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.669229 bip_utils-2.7.0/bip_utils/electrum/
--rw-rw-rw-   0        0        0      136 2022-09-13 12:40:47.000000 bip_utils-2.7.0/bip_utils/electrum/__init__.py
--rw-rw-rw-   0        0        0    10444 2022-09-13 12:40:47.000000 bip_utils-2.7.0/bip_utils/electrum/electrum_v1.py
--rw-rw-rw-   0        0        0    12764 2022-09-13 12:40:48.000000 bip_utils-2.7.0/bip_utils/electrum/electrum_v2.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.725231 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/
--rw-rw-rw-   0        0        0      770 2022-09-13 12:40:48.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/__init__.py
--rw-rw-rw-   0        0        0     3183 2022-09-13 12:40:49.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py
--rw-rw-rw-   0        0        0     2149 2022-09-13 12:40:49.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py
--rw-rw-rw-   0        0        0     3685 2022-09-13 12:40:49.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     3162 2022-09-13 12:40:50.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     4396 2022-09-13 12:40:50.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py
--rw-rw-rw-   0        0        0     3890 2022-09-13 12:40:50.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py
--rw-rw-rw-   0        0        0     2181 2022-09-13 12:40:51.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py
--rw-rw-rw-   0        0        0     3621 2022-09-13 12:40:51.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.729230 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/wordlist/
--rw-rw-rw-   0        0        0    12120 2022-09-13 12:40:52.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/wordlist/english.txt
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.775230 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/
--rw-rw-rw-   0        0        0      795 2022-09-13 12:40:53.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/__init__.py
--rw-rw-rw-   0        0        0     4300 2022-09-13 12:40:53.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py
--rw-rw-rw-   0        0        0     2937 2022-09-13 12:40:54.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py
--rw-rw-rw-   0        0        0     4499 2022-09-13 12:40:54.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     4249 2022-09-13 12:40:54.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     5966 2022-09-13 12:40:55.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py
--rw-rw-rw-   0        0        0     4266 2022-09-13 12:40:55.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py
--rw-rw-rw-   0        0        0     2205 2022-09-13 12:40:55.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py
--rw-rw-rw-   0        0        0     3308 2022-09-13 12:40:56.000000 bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.794229 bip_utils-2.7.0/bip_utils/monero/
--rw-rw-rw-   0        0        0      237 2022-09-13 12:40:56.000000 bip_utils-2.7.0/bip_utils/monero/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.818229 bip_utils-2.7.0/bip_utils/monero/conf/
--rw-rw-rw-   0        0        0      256 2022-09-13 12:40:57.000000 bip_utils-2.7.0/bip_utils/monero/conf/__init__.py
--rw-rw-rw-   0        0        0     3770 2022-09-13 12:40:57.000000 bip_utils-2.7.0/bip_utils/monero/conf/monero_coin_conf.py
--rw-rw-rw-   0        0        0     1386 2022-09-13 12:40:58.000000 bip_utils-2.7.0/bip_utils/monero/conf/monero_coins.py
--rw-rw-rw-   0        0        0     1748 2022-09-13 12:40:58.000000 bip_utils-2.7.0/bip_utils/monero/conf/monero_conf.py
--rw-rw-rw-   0        0        0     2508 2022-09-13 12:40:59.000000 bip_utils-2.7.0/bip_utils/monero/conf/monero_conf_getter.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.859228 bip_utils-2.7.0/bip_utils/monero/mnemonic/
--rw-rw-rw-   0        0        0      718 2022-09-13 12:40:59.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     3191 2022-09-13 12:40:59.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_entropy_generator.py
--rw-rw-rw-   0        0        0     3753 2022-09-13 12:41:00.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic.py
--rw-rw-rw-   0        0        0     4355 2022-09-26 07:56:05.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py
--rw-rw-rw-   0        0        0     6520 2022-09-13 12:41:01.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py
--rw-rw-rw-   0        0        0     5109 2022-09-13 12:41:01.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_generator.py
--rw-rw-rw-   0        0        0     4600 2022-09-26 07:56:07.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_utils.py
--rw-rw-rw-   0        0        0     1872 2022-09-13 12:41:02.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_validator.py
--rw-rw-rw-   0        0        0     2545 2022-09-13 12:41:02.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_seed_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.928229 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/
--rw-rw-rw-   0        0        0     8130 2022-09-13 12:41:03.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt
--rw-rw-rw-   0        0        0    14346 2022-09-13 12:41:03.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/dutch.txt
--rw-rw-rw-   0        0        0    13093 2022-09-13 12:41:04.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/english.txt
--rw-rw-rw-   0        0        0    12524 2022-09-13 12:41:05.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/french.txt
--rw-rw-rw-   0        0        0    13960 2022-09-13 12:41:05.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/german.txt
--rw-rw-rw-   0        0        0    14400 2022-09-13 12:41:05.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/italian.txt
--rw-rw-rw-   0        0        0    21054 2022-09-13 12:41:06.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/japanese.txt
--rw-rw-rw-   0        0        0    14765 2022-09-13 12:41:06.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/portuguese.txt
--rw-rw-rw-   0        0        0    22376 2022-09-13 12:41:07.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/russian.txt
--rw-rw-rw-   0        0        0    12524 2022-09-13 12:41:07.000000 bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/spanish.txt
--rw-rw-rw-   0        0        0    10682 2022-09-23 19:18:29.000000 bip_utils-2.7.0/bip_utils/monero/monero.py
--rw-rw-rw-   0        0        0     1244 2022-09-13 12:41:08.000000 bip_utils-2.7.0/bip_utils/monero/monero_ex.py
--rw-rw-rw-   0        0        0     8202 2022-10-06 12:24:47.000000 bip_utils-2.7.0/bip_utils/monero/monero_keys.py
--rw-rw-rw-   0        0        0     6050 2022-10-06 12:27:50.000000 bip_utils-2.7.0/bip_utils/monero/monero_subaddr.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.934230 bip_utils-2.7.0/bip_utils/slip/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:41:09.000000 bip_utils-2.7.0/bip_utils/slip/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.940229 bip_utils-2.7.0/bip_utils/slip/slip173/
--rw-rw-rw-   0        0        0       52 2022-09-13 12:41:09.000000 bip_utils-2.7.0/bip_utils/slip/slip173/__init__.py
--rw-rw-rw-   0        0        0     2055 2022-09-13 12:41:09.000000 bip_utils-2.7.0/bip_utils/slip/slip173/slip173.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.954228 bip_utils-2.7.0/bip_utils/slip/slip32/
--rw-rw-rw-   0        0        0      227 2022-09-13 12:41:10.000000 bip_utils-2.7.0/bip_utils/slip/slip32/__init__.py
--rw-rw-rw-   0        0        0    11214 2022-09-13 12:41:11.000000 bip_utils-2.7.0/bip_utils/slip/slip32/slip32.py
--rw-rw-rw-   0        0        0     2085 2022-09-13 12:41:11.000000 bip_utils-2.7.0/bip_utils/slip/slip32/slip32_key_net_ver.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.961228 bip_utils-2.7.0/bip_utils/slip/slip44/
--rw-rw-rw-   0        0        0       49 2022-09-13 12:41:12.000000 bip_utils-2.7.0/bip_utils/slip/slip44/__init__.py
--rw-rw-rw-   0        0        0     2485 2022-09-13 12:41:12.000000 bip_utils-2.7.0/bip_utils/slip/slip44/slip44.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.968229 bip_utils-2.7.0/bip_utils/solana/
--rw-rw-rw-   0        0        0       49 2022-09-13 12:41:12.000000 bip_utils-2.7.0/bip_utils/solana/__init__.py
--rw-rw-rw-   0        0        0     6588 2022-09-13 12:41:13.000000 bip_utils-2.7.0/bip_utils/solana/spl_token.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:41.979229 bip_utils-2.7.0/bip_utils/ss58/
--rw-rw-rw-   0        0        0      112 2022-09-13 12:41:13.000000 bip_utils-2.7.0/bip_utils/ss58/__init__.py
--rw-rw-rw-   0        0        0     5967 2022-09-13 12:41:14.000000 bip_utils-2.7.0/bip_utils/ss58/ss58.py
--rw-rw-rw-   0        0        0     1243 2022-09-13 12:41:15.000000 bip_utils-2.7.0/bip_utils/ss58/ss58_ex.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.003229 bip_utils-2.7.0/bip_utils/substrate/
--rw-rw-rw-   0        0        0      343 2022-09-13 12:41:16.000000 bip_utils-2.7.0/bip_utils/substrate/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.025231 bip_utils-2.7.0/bip_utils/substrate/conf/
--rw-rw-rw-   0        0        0      292 2022-09-13 12:41:16.000000 bip_utils-2.7.0/bip_utils/substrate/conf/__init__.py
--rw-rw-rw-   0        0        0     3031 2022-09-13 12:41:16.000000 bip_utils-2.7.0/bip_utils/substrate/conf/substrate_coin_conf.py
--rw-rw-rw-   0        0        0     1606 2022-09-13 12:41:17.000000 bip_utils-2.7.0/bip_utils/substrate/conf/substrate_coins.py
--rw-rw-rw-   0        0        0     3116 2022-09-13 12:41:17.000000 bip_utils-2.7.0/bip_utils/substrate/conf/substrate_conf.py
--rw-rw-rw-   0        0        0     3179 2022-09-13 12:41:18.000000 bip_utils-2.7.0/bip_utils/substrate/conf/substrate_conf_getter.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.032228 bip_utils-2.7.0/bip_utils/substrate/mnemonic/
--rw-rw-rw-   0        0        0      101 2022-09-13 12:41:18.000000 bip_utils-2.7.0/bip_utils/substrate/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     2973 2022-09-13 12:41:18.000000 bip_utils-2.7.0/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.053229 bip_utils-2.7.0/bip_utils/substrate/scale/
--rw-rw-rw-   0        0        0      509 2022-09-13 12:41:19.000000 bip_utils-2.7.0/bip_utils/substrate/scale/__init__.py
--rw-rw-rw-   0        0        0     1628 2022-09-13 12:41:19.000000 bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_base.py
--rw-rw-rw-   0        0        0     1948 2022-09-13 12:41:20.000000 bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_bytes.py
--rw-rw-rw-   0        0        0     3082 2022-09-13 12:41:21.000000 bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_cuint.py
--rw-rw-rw-   0        0        0     4954 2022-09-13 12:41:21.000000 bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_uint.py
--rw-rw-rw-   0        0        0    12628 2022-09-13 12:41:21.000000 bip_utils-2.7.0/bip_utils/substrate/substrate.py
--rw-rw-rw-   0        0        0     1349 2022-09-13 12:41:22.000000 bip_utils-2.7.0/bip_utils/substrate/substrate_ex.py
--rw-rw-rw-   0        0        0     8752 2022-09-13 12:41:22.000000 bip_utils-2.7.0/bip_utils/substrate/substrate_keys.py
--rw-rw-rw-   0        0        0     9228 2022-09-13 12:41:23.000000 bip_utils-2.7.0/bip_utils/substrate/substrate_path.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.056228 bip_utils-2.7.0/bip_utils/utils/
--rw-rw-rw-   0        0        0        0 2022-09-13 12:41:23.000000 bip_utils-2.7.0/bip_utils/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.061228 bip_utils-2.7.0/bip_utils/utils/conf/
--rw-rw-rw-   0        0        0       55 2022-09-13 12:41:24.000000 bip_utils-2.7.0/bip_utils/utils/conf/__init__.py
--rw-rw-rw-   0        0        0     1881 2022-09-13 12:41:25.000000 bip_utils-2.7.0/bip_utils/utils/conf/coin_names.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.115229 bip_utils-2.7.0/bip_utils/utils/crypto/
--rw-rw-rw-   0        0        0      748 2022-09-13 12:41:25.000000 bip_utils-2.7.0/bip_utils/utils/crypto/__init__.py
--rw-rw-rw-   0        0        0     4043 2022-09-13 12:41:25.000000 bip_utils-2.7.0/bip_utils/utils/crypto/aes_ecb.py
--rw-rw-rw-   0        0        0     5189 2022-09-13 12:41:26.000000 bip_utils-2.7.0/bip_utils/utils/crypto/blake2.py
--rw-rw-rw-   0        0        0     3566 2022-09-13 12:41:27.000000 bip_utils-2.7.0/bip_utils/utils/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     3048 2022-09-13 12:41:27.000000 bip_utils-2.7.0/bip_utils/utils/crypto/crc.py
--rw-rw-rw-   0        0        0     1944 2022-09-13 12:41:27.000000 bip_utils-2.7.0/bip_utils/utils/crypto/hash160.py
--rw-rw-rw-   0        0        0     3822 2022-09-13 12:41:28.000000 bip_utils-2.7.0/bip_utils/utils/crypto/hmac.py
--rw-rw-rw-   0        0        0     2602 2022-09-13 12:41:28.000000 bip_utils-2.7.0/bip_utils/utils/crypto/pbkdf2.py
--rw-rw-rw-   0        0        0     1927 2022-09-13 12:41:28.000000 bip_utils-2.7.0/bip_utils/utils/crypto/ripemd.py
--rw-rw-rw-   0        0        0     2525 2022-09-13 12:41:29.000000 bip_utils-2.7.0/bip_utils/utils/crypto/scrypt.py
--rw-rw-rw-   0        0        0     4836 2022-09-13 12:41:29.000000 bip_utils-2.7.0/bip_utils/utils/crypto/sha2.py
--rw-rw-rw-   0        0        0     3097 2022-09-13 12:41:30.000000 bip_utils-2.7.0/bip_utils/utils/crypto/sha3.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.150231 bip_utils-2.7.0/bip_utils/utils/misc/
--rw-rw-rw-   0        0        0      501 2022-09-13 12:41:30.000000 bip_utils-2.7.0/bip_utils/utils/misc/__init__.py
--rw-rw-rw-   0        0        0     3458 2022-09-13 12:41:31.000000 bip_utils-2.7.0/bip_utils/utils/misc/algo.py
--rw-rw-rw-   0        0        0     4870 2022-09-13 12:41:32.000000 bip_utils-2.7.0/bip_utils/utils/misc/base32.py
--rw-rw-rw-   0        0        0     3429 2022-09-13 12:41:33.000000 bip_utils-2.7.0/bip_utils/utils/misc/bit.py
--rw-rw-rw-   0        0        0     6326 2022-09-13 12:41:33.000000 bip_utils-2.7.0/bip_utils/utils/misc/bytes.py
--rw-rw-rw-   0        0        0     4344 2022-09-13 12:41:34.000000 bip_utils-2.7.0/bip_utils/utils/misc/cbor_indefinite_len_array.py
--rw-rw-rw-   0        0        0     4924 2022-09-13 12:41:34.000000 bip_utils-2.7.0/bip_utils/utils/misc/data_bytes.py
--rw-rw-rw-   0        0        0     3192 2022-09-13 12:41:34.000000 bip_utils-2.7.0/bip_utils/utils/misc/integer.py
--rw-rw-rw-   0        0        0     1884 2022-09-13 12:41:35.000000 bip_utils-2.7.0/bip_utils/utils/misc/string.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.181228 bip_utils-2.7.0/bip_utils/utils/mnemonic/
--rw-rw-rw-   0        0        0      643 2022-09-13 12:41:35.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/__init__.py
--rw-rw-rw-   0        0        0     1976 2022-09-13 12:41:35.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/entropy_generator.py
--rw-rw-rw-   0        0        0     3716 2022-09-13 12:41:36.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic.py
--rw-rw-rw-   0        0        0     3895 2022-09-13 12:41:36.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_decoder_base.py
--rw-rw-rw-   0        0        0     2578 2022-09-13 12:41:37.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_encoder_base.py
--rw-rw-rw-   0        0        0     1251 2022-09-13 12:41:37.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_ex.py
--rw-rw-rw-   0        0        0    10988 2022-09-26 07:56:25.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_utils.py
--rw-rw-rw-   0        0        0     2860 2022-09-13 12:41:38.000000 bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_validator.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.188231 bip_utils-2.7.0/bip_utils/utils/typing/
--rw-rw-rw-   0        0        0       52 2022-09-13 12:41:39.000000 bip_utils-2.7.0/bip_utils/utils/typing/__init__.py
--rw-rw-rw-   0        0        0     1372 2022-09-13 12:41:39.000000 bip_utils-2.7.0/bip_utils/utils/typing/literal.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.203229 bip_utils-2.7.0/bip_utils/wif/
--rw-rw-rw-   0        0        0       70 2022-09-13 12:41:39.000000 bip_utils-2.7.0/bip_utils/wif/__init__.py
--rw-rw-rw-   0        0        0     5624 2022-09-13 12:41:40.000000 bip_utils-2.7.0/bip_utils/wif/wif.py
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:40.394229 bip_utils-2.7.0/bip_utils.egg-info/
--rw-rw-rw-   0        0        0    11665 2022-10-06 12:40:39.000000 bip_utils-2.7.0/bip_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14337 2022-10-06 12:40:40.000000 bip_utils-2.7.0/bip_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-06 12:40:39.000000 bip_utils-2.7.0/bip_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      320 2022-10-06 12:40:39.000000 bip_utils-2.7.0/bip_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-10-06 12:40:39.000000 bip_utils-2.7.0/bip_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      978 2022-08-25 20:30:48.000000 bip_utils-2.7.0/keywords.txt
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.291729 bip_utils-2.7.0/readme/
--rw-rw-rw-   0        0        0     5128 2022-08-08 18:27:56.000000 bip_utils-2.7.0/readme/algorand_mnemonic.md
--rw-rw-rw-   0        0        0    17713 2022-08-08 18:27:15.000000 bip_utils-2.7.0/readme/bip32.md
--rw-rw-rw-   0        0        0     3317 2022-06-22 12:42:18.000000 bip_utils-2.7.0/readme/bip38.md
--rw-rw-rw-   0        0        0     7775 2022-08-08 18:29:07.000000 bip_utils-2.7.0/readme/bip39.md
--rw-rw-rw-   0        0        0    20022 2022-08-25 20:31:16.000000 bip_utils-2.7.0/readme/bip44.md
--rw-rw-rw-   0        0        0    17246 2022-08-08 18:36:03.000000 bip_utils-2.7.0/readme/cardano.md
--rw-rw-rw-   0        0        0     4701 2022-08-08 18:36:17.000000 bip_utils-2.7.0/readme/electrum.md
--rw-rw-rw-   0        0        0      767 2022-08-08 18:36:37.000000 bip_utils-2.7.0/readme/electrum_mnemonic.md
--rw-rw-rw-   0        0        0     4827 2022-08-08 18:37:09.000000 bip_utils-2.7.0/readme/electrum_v1_mnemonic.md
--rw-rw-rw-   0        0        0     8675 2022-08-08 18:38:17.000000 bip_utils-2.7.0/readme/electrum_v2_mnemonic.md
--rw-rw-rw-   0        0        0     5035 2022-08-08 18:38:58.000000 bip_utils-2.7.0/readme/monero.md
--rw-rw-rw-   0        0        0     6792 2022-08-08 18:40:03.000000 bip_utils-2.7.0/readme/monero_mnemonic.md
--rw-rw-rw-   0        0        0     8496 2022-08-08 18:41:26.000000 bip_utils-2.7.0/readme/substrate.md
-drwxrwxrwx   0        0        0        0 2022-10-06 12:40:42.326031 bip_utils-2.7.0/readme/utility/
--rw-rw-rw-   0        0        0    15078 2022-08-08 18:42:21.000000 bip_utils-2.7.0/readme/utility/addr.md
--rw-rw-rw-   0        0        0     1500 2022-08-08 18:41:47.000000 bip_utils-2.7.0/readme/utility/base58.md
--rw-rw-rw-   0        0        0      613 2022-06-29 09:24:21.000000 bip_utils-2.7.0/readme/utility/bch_addr_converter.md
--rw-rw-rw-   0        0        0     1242 2022-08-08 18:42:01.000000 bip_utils-2.7.0/readme/utility/bech32.md
--rw-rw-rw-   0        0        0     1433 2022-06-29 07:19:26.000000 bip_utils-2.7.0/readme/utility/slip32.md
--rw-rw-rw-   0        0        0      991 2022-06-29 09:09:58.000000 bip_utils-2.7.0/readme/utility/solana_spl.md
--rw-rw-rw-   0        0        0      441 2022-06-29 08:56:27.000000 bip_utils-2.7.0/readme/utility/ss58.md
--rw-rw-rw-   0        0        0     1940 2022-08-08 18:42:10.000000 bip_utils-2.7.0/readme/utility/wif.md
--rw-rw-rw-   0        0        0      874 2022-06-29 09:25:30.000000 bip_utils-2.7.0/readme/utility_libs.md
--rw-rw-rw-   0        0        0      124 2022-08-11 20:25:09.000000 bip_utils-2.7.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      154 2022-08-07 19:59:17.000000 bip_utils-2.7.0/requirements.txt
--rw-rw-rw-   0        0        0      111 2022-10-06 12:40:42.336032 bip_utils-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0     6004 2022-08-11 20:18:02.000000 bip_utils-2.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:28.083875 bip_utils-2.7.1/
+-rw-rw-rw-   0        0        0     1085 2022-07-29 18:35:18.000000 bip_utils-2.7.1/LICENSE
+-rw-rw-rw-   0        0        0      122 2022-08-23 19:50:06.000000 bip_utils-2.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11916 2023-05-26 12:02:28.083875 bip_utils-2.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9998 2023-02-22 12:16:16.000000 bip_utils-2.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.208494 bip_utils-2.7.1/bip_utils/
+-rw-rw-rw-   0        0        0     8578 2023-02-22 10:04:32.000000 bip_utils-2.7.1/bip_utils/__init__.py
+-rw-rw-rw-   0        0        0       28 2023-05-26 11:41:22.000000 bip_utils-2.7.1/bip_utils/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.379784 bip_utils-2.7.1/bip_utils/addr/
+-rw-rw-rw-   0        0        0     7422 2023-05-25 21:02:58.000000 bip_utils-2.7.1/bip_utils/addr/P2PKH_addr.py
+-rw-rw-rw-   0        0        0     6130 2022-09-13 12:39:23.000000 bip_utils-2.7.1/bip_utils/addr/P2SH_addr.py
+-rw-rw-rw-   0        0        0     7404 2023-05-25 21:03:14.000000 bip_utils-2.7.1/bip_utils/addr/P2TR_addr.py
+-rw-rw-rw-   0        0        0     4171 2023-05-25 21:03:26.000000 bip_utils-2.7.1/bip_utils/addr/P2WPKH_addr.py
+-rw-rw-rw-   0        0        0     3332 2023-02-22 10:04:02.000000 bip_utils-2.7.1/bip_utils/addr/__init__.py
+-rw-rw-rw-   0        0        0    18494 2022-11-16 09:43:25.000000 bip_utils-2.7.1/bip_utils/addr/ada_byron_addr.py
+-rw-rw-rw-   0        0        0    11188 2023-05-25 21:03:52.000000 bip_utils-2.7.1/bip_utils/addr/ada_shelley_addr.py
+-rw-rw-rw-   0        0        0     4791 2022-09-13 12:39:15.000000 bip_utils-2.7.1/bip_utils/addr/addr_dec_utils.py
+-rw-rw-rw-   0        0        0     6010 2022-09-13 12:39:16.000000 bip_utils-2.7.1/bip_utils/addr/addr_key_validator.py
+-rw-rw-rw-   0        0        0     4658 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/addr/algo_addr.py
+-rw-rw-rw-   0        0        0     4036 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/addr/aptos_addr.py
+-rw-rw-rw-   0        0        0     3547 2023-05-25 21:04:08.000000 bip_utils-2.7.1/bip_utils/addr/atom_addr.py
+-rw-rw-rw-   0        0        0     5774 2022-09-13 12:39:18.000000 bip_utils-2.7.1/bip_utils/addr/avax_addr.py
+-rw-rw-rw-   0        0        0     2377 2022-09-13 12:39:18.000000 bip_utils-2.7.1/bip_utils/addr/bch_addr_converter.py
+-rw-rw-rw-   0        0        0     3666 2023-05-25 21:10:00.000000 bip_utils-2.7.1/bip_utils/addr/egld_addr.py
+-rw-rw-rw-   0        0        0     4831 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/addr/eos_addr.py
+-rw-rw-rw-   0        0        0     6397 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/addr/ergo_addr.py
+-rw-rw-rw-   0        0        0     5229 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/addr/eth_addr.py
+-rw-rw-rw-   0        0        0     6871 2022-09-13 12:39:20.000000 bip_utils-2.7.1/bip_utils/addr/fil_addr.py
+-rw-rw-rw-   0        0        0     1881 2022-09-13 12:39:20.000000 bip_utils-2.7.1/bip_utils/addr/iaddr_decoder.py
+-rw-rw-rw-   0        0        0     1982 2022-09-13 12:39:21.000000 bip_utils-2.7.1/bip_utils/addr/iaddr_encoder.py
+-rw-rw-rw-   0        0        0     3824 2022-09-13 12:39:21.000000 bip_utils-2.7.1/bip_utils/addr/icx_addr.py
+-rw-rw-rw-   0        0        0     5459 2022-09-13 12:39:21.000000 bip_utils-2.7.1/bip_utils/addr/nano_addr.py
+-rw-rw-rw-   0        0        0     3416 2022-09-13 12:39:22.000000 bip_utils-2.7.1/bip_utils/addr/near_addr.py
+-rw-rw-rw-   0        0        0     4361 2023-05-25 21:04:18.000000 bip_utils-2.7.1/bip_utils/addr/neo_addr.py
+-rw-rw-rw-   0        0        0     3713 2023-05-25 21:04:29.000000 bip_utils-2.7.1/bip_utils/addr/okex_addr.py
+-rw-rw-rw-   0        0        0     3702 2023-05-25 21:04:38.000000 bip_utils-2.7.1/bip_utils/addr/one_addr.py
+-rw-rw-rw-   0        0        0     3387 2022-09-13 12:39:25.000000 bip_utils-2.7.1/bip_utils/addr/sol_addr.py
+-rw-rw-rw-   0        0        0     6173 2022-09-13 12:39:25.000000 bip_utils-2.7.1/bip_utils/addr/substrate_addr.py
+-rw-rw-rw-   0        0        0     4055 2023-05-25 21:05:04.000000 bip_utils-2.7.1/bip_utils/addr/trx_addr.py
+-rw-rw-rw-   0        0        0     5891 2022-09-13 12:39:26.000000 bip_utils-2.7.1/bip_utils/addr/xlm_addr.py
+-rw-rw-rw-   0        0        0    10588 2022-09-13 12:39:26.000000 bip_utils-2.7.1/bip_utils/addr/xmr_addr.py
+-rw-rw-rw-   0        0        0     3454 2022-09-13 12:39:26.000000 bip_utils-2.7.1/bip_utils/addr/xrp_addr.py
+-rw-rw-rw-   0        0        0     4592 2023-05-25 21:05:37.000000 bip_utils-2.7.1/bip_utils/addr/xtz_addr.py
+-rw-rw-rw-   0        0        0     3807 2023-05-25 21:05:30.000000 bip_utils-2.7.1/bip_utils/addr/zil_addr.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.383787 bip_utils-2.7.1/bip_utils/algorand/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:39:27.000000 bip_utils-2.7.1/bip_utils/algorand/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.426554 bip_utils-2.7.1/bip_utils/algorand/mnemonic/
+-rw-rw-rw-   0        0        0      688 2022-09-13 12:39:28.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     3145 2022-09-13 12:39:28.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_entropy_generator.py
+-rw-rw-rw-   0        0        0     1994 2022-09-13 12:39:29.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic.py
+-rw-rw-rw-   0        0        0     5234 2022-09-13 12:39:29.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     3907 2022-09-13 12:39:30.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     4297 2022-09-13 12:39:30.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     3852 2022-09-13 12:39:31.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2144 2022-09-13 12:39:31.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     2779 2022-09-13 12:39:32.000000 bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_seed_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.448298 bip_utils-2.7.1/bip_utils/base58/
+-rw-rw-rw-   0        0        0      219 2022-09-13 12:39:32.000000 bip_utils-2.7.1/bip_utils/base58/__init__.py
+-rw-rw-rw-   0        0        0     7113 2022-09-13 12:39:33.000000 bip_utils-2.7.1/bip_utils/base58/base58.py
+-rw-rw-rw-   0        0        0     1247 2022-09-13 12:39:33.000000 bip_utils-2.7.1/bip_utils/base58/base58_ex.py
+-rw-rw-rw-   0        0        0     5462 2022-09-25 20:02:30.000000 bip_utils-2.7.1/bip_utils/base58/base58_xmr.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.477534 bip_utils-2.7.1/bip_utils/bech32/
+-rw-rw-rw-   0        0        0      287 2022-09-13 12:39:34.000000 bip_utils-2.7.1/bip_utils/bech32/__init__.py
+-rw-rw-rw-   0        0        0     6863 2022-09-13 12:39:34.000000 bip_utils-2.7.1/bip_utils/bech32/bch_bech32.py
+-rw-rw-rw-   0        0        0     7472 2022-09-13 12:39:34.000000 bip_utils-2.7.1/bip_utils/bech32/bech32.py
+-rw-rw-rw-   0        0        0     8249 2022-09-13 12:39:35.000000 bip_utils-2.7.1/bip_utils/bech32/bech32_base.py
+-rw-rw-rw-   0        0        0     1247 2022-09-13 12:39:35.000000 bip_utils-2.7.1/bip_utils/bech32/bech32_ex.py
+-rw-rw-rw-   0        0        0     6264 2022-09-26 19:44:08.000000 bip_utils-2.7.1/bip_utils/bech32/segwit_bech32.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.481797 bip_utils-2.7.1/bip_utils/bip/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:39:36.000000 bip_utils-2.7.1/bip_utils/bip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.518990 bip_utils-2.7.1/bip_utils/bip/bip32/
+-rw-rw-rw-   0        0        0     1354 2022-09-13 12:39:37.000000 bip_utils-2.7.1/bip_utils/bip/bip32/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.538805 bip_utils-2.7.1/bip_utils/bip/bip32/base/
+-rw-rw-rw-   0        0        0      222 2022-09-13 12:39:37.000000 bip_utils-2.7.1/bip_utils/bip/bip32/base/__init__.py
+-rw-rw-rw-   0        0        0    21303 2022-09-13 12:39:37.000000 bip_utils-2.7.1/bip_utils/bip/bip32/base/bip32_base.py
+-rw-rw-rw-   0        0        0     3130 2022-09-13 12:39:38.000000 bip_utils-2.7.1/bip_utils/bip/bip32/base/ibip32_key_derivator.py
+-rw-rw-rw-   0        0        0     1897 2022-09-13 12:39:39.000000 bip_utils-2.7.1/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py
+-rw-rw-rw-   0        0        0     1835 2022-09-13 12:39:39.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_const.py
+-rw-rw-rw-   0        0        0     1318 2022-09-13 12:39:39.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_ex.py
+-rw-rw-rw-   0        0        0    14058 2022-09-13 12:39:40.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_key_data.py
+-rw-rw-rw-   0        0        0     2694 2022-09-13 12:39:40.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_key_net_ver.py
+-rw-rw-rw-   0        0        0    10535 2022-09-13 12:39:41.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_key_ser.py
+-rw-rw-rw-   0        0        0    15183 2022-09-13 12:39:41.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_keys.py
+-rw-rw-rw-   0        0        0     7428 2022-09-13 12:39:42.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_path.py
+-rw-rw-rw-   0        0        0     2346 2022-09-13 12:39:42.000000 bip_utils-2.7.1/bip_utils/bip/bip32/bip32_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.559666 bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/
+-rw-rw-rw-   0        0        0      418 2022-09-13 12:39:43.000000 bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/__init__.py
+-rw-rw-rw-   0        0        0     3093 2022-09-13 12:39:43.000000 bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py
+-rw-rw-rw-   0        0        0     4850 2022-09-13 12:39:44.000000 bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py
+-rw-rw-rw-   0        0        0     8071 2022-09-13 12:39:44.000000 bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py
+-rw-rw-rw-   0        0        0     4899 2022-09-13 12:39:45.000000 bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.597352 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/
+-rw-rw-rw-   0        0        0      728 2022-09-13 12:39:45.000000 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/__init__.py
+-rw-rw-rw-   0        0        0     3058 2022-09-13 12:39:46.000000 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py
+-rw-rw-rw-   0        0        0     1905 2022-09-13 12:39:46.000000 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py
+-rw-rw-rw-   0        0        0     7389 2023-05-26 11:19:43.000000 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py
+-rw-rw-rw-   0        0        0     6708 2022-09-13 12:39:47.000000 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py
+-rw-rw-rw-   0        0        0     3070 2022-09-13 12:39:48.000000 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py
+-rw-rw-rw-   0        0        0     3066 2022-09-13 12:39:48.000000 bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.621705 bip_utils-2.7.1/bip_utils/bip/bip38/
+-rw-rw-rw-   0        0        0      194 2022-09-13 12:39:49.000000 bip_utils-2.7.1/bip_utils/bip/bip38/__init__.py
+-rw-rw-rw-   0        0        0     5286 2022-09-13 12:39:49.000000 bip_utils-2.7.1/bip_utils/bip/bip38/bip38.py
+-rw-rw-rw-   0        0        0     2665 2022-09-13 12:39:49.000000 bip_utils-2.7.1/bip_utils/bip/bip38/bip38_addr.py
+-rw-rw-rw-   0        0        0    21343 2023-05-25 21:29:13.000000 bip_utils-2.7.1/bip_utils/bip/bip38/bip38_ec.py
+-rw-rw-rw-   0        0        0    11382 2022-09-13 12:39:50.000000 bip_utils-2.7.1/bip_utils/bip/bip38/bip38_no_ec.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.670801 bip_utils-2.7.1/bip_utils/bip/bip39/
+-rw-rw-rw-   0        0        0      656 2022-09-13 12:39:51.000000 bip_utils-2.7.1/bip_utils/bip/bip39/__init__.py
+-rw-rw-rw-   0        0        0     3376 2023-01-03 20:45:03.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_entropy_generator.py
+-rw-rw-rw-   0        0        0     3559 2022-09-13 12:39:52.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic.py
+-rw-rw-rw-   0        0        0     7931 2022-09-13 12:39:52.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     3997 2023-01-03 20:45:05.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     4021 2023-01-03 20:45:06.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     3809 2022-09-13 12:39:54.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     1850 2022-09-13 12:39:55.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     3486 2022-09-13 12:39:55.000000 bip_utils-2.7.1/bip_utils/bip/bip39/bip39_seed_generator.py
+-rw-rw-rw-   0        0        0     2228 2022-09-13 12:39:55.000000 bip_utils-2.7.1/bip_utils/bip/bip39/ibip39_seed_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.826447 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/
+-rw-rw-rw-   0        0        0    10240 2022-09-13 12:39:56.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/chinese_simplified.txt
+-rw-rw-rw-   0        0        0    10240 2022-09-13 12:39:56.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/chinese_traditional.txt
+-rw-rw-rw-   0        0        0    16993 2022-09-13 12:39:56.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/czech.txt
+-rw-rw-rw-   0        0        0    15164 2022-09-13 12:39:57.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/english.txt
+-rw-rw-rw-   0        0        0    18825 2022-09-13 12:39:57.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/french.txt
+-rw-rw-rw-   0        0        0    18081 2022-09-13 12:39:58.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/italian.txt
+-rw-rw-rw-   0        0        0    39880 2022-09-13 12:39:58.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/korean.txt
+-rw-rw-rw-   0        0        0    17719 2022-09-13 12:39:59.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/portuguese.txt
+-rw-rw-rw-   0        0        0    16044 2022-09-13 12:39:59.000000 bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/spanish.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.848275 bip_utils-2.7.1/bip_utils/bip/bip44/
+-rw-rw-rw-   0        0        0       45 2022-09-13 12:40:00.000000 bip_utils-2.7.1/bip_utils/bip/bip44/__init__.py
+-rw-rw-rw-   0        0        0     8919 2022-09-13 12:40:00.000000 bip_utils-2.7.1/bip_utils/bip/bip44/bip44.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.866612 bip_utils-2.7.1/bip_utils/bip/bip44_base/
+-rw-rw-rw-   0        0        0      235 2022-09-13 12:40:00.000000 bip_utils-2.7.1/bip_utils/bip/bip44_base/__init__.py
+-rw-rw-rw-   0        0        0    21706 2022-09-13 12:40:01.000000 bip_utils-2.7.1/bip_utils/bip/bip44_base/bip44_base.py
+-rw-rw-rw-   0        0        0     1255 2022-09-13 12:40:01.000000 bip_utils-2.7.1/bip_utils/bip/bip44_base/bip44_base_ex.py
+-rw-rw-rw-   0        0        0     7297 2022-09-13 12:40:02.000000 bip_utils-2.7.1/bip_utils/bip/bip44_base/bip44_keys.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.874633 bip_utils-2.7.1/bip_utils/bip/bip49/
+-rw-rw-rw-   0        0        0       45 2022-09-13 12:40:02.000000 bip_utils-2.7.1/bip_utils/bip/bip49/__init__.py
+-rw-rw-rw-   0        0        0     8919 2022-09-13 12:40:03.000000 bip_utils-2.7.1/bip_utils/bip/bip49/bip49.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.884597 bip_utils-2.7.1/bip_utils/bip/bip84/
+-rw-rw-rw-   0        0        0       45 2022-09-13 12:40:03.000000 bip_utils-2.7.1/bip_utils/bip/bip84/__init__.py
+-rw-rw-rw-   0        0        0     8919 2022-09-13 12:40:04.000000 bip_utils-2.7.1/bip_utils/bip/bip84/bip84.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.893553 bip_utils-2.7.1/bip_utils/bip/bip86/
+-rw-rw-rw-   0        0        0       45 2022-09-13 12:40:04.000000 bip_utils-2.7.1/bip_utils/bip/bip86/__init__.py
+-rw-rw-rw-   0        0        0     8917 2022-09-13 12:40:05.000000 bip_utils-2.7.1/bip_utils/bip/bip86/bip86.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.898437 bip_utils-2.7.1/bip_utils/bip/conf/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:05.000000 bip_utils-2.7.1/bip_utils/bip/conf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.939945 bip_utils-2.7.1/bip_utils/bip/conf/bip44/
+-rw-rw-rw-   0        0        0      192 2022-09-13 12:40:06.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip44/__init__.py
+-rw-rw-rw-   0        0        0     3362 2023-02-22 12:17:00.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip44/bip44_coins.py
+-rw-rw-rw-   0        0        0    42493 2023-02-22 12:56:40.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip44/bip44_conf.py
+-rw-rw-rw-   0        0        0     6561 2023-02-22 12:19:44.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip44/bip44_conf_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.967709 bip_utils-2.7.1/bip_utils/bip/conf/bip49/
+-rw-rw-rw-   0        0        0      192 2022-09-13 12:40:07.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip49/__init__.py
+-rw-rw-rw-   0        0        0     1879 2022-09-13 12:40:08.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip49/bip49_coins.py
+-rw-rw-rw-   0        0        0    15216 2023-02-22 12:54:50.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip49/bip49_conf.py
+-rw-rw-rw-   0        0        0     3404 2022-09-13 12:40:09.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip49/bip49_conf_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.987609 bip_utils-2.7.1/bip_utils/bip/conf/bip84/
+-rw-rw-rw-   0        0        0      192 2022-09-13 12:40:09.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip84/__init__.py
+-rw-rw-rw-   0        0        0     1493 2022-09-13 12:40:10.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip84/bip84_coins.py
+-rw-rw-rw-   0        0        0     4218 2023-02-22 12:54:50.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip84/bip84_conf.py
+-rw-rw-rw-   0        0        0     2542 2022-09-13 12:40:11.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip84/bip84_conf_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.010739 bip_utils-2.7.1/bip_utils/bip/conf/bip86/
+-rw-rw-rw-   0        0        0      192 2022-09-13 12:40:11.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip86/__init__.py
+-rw-rw-rw-   0        0        0     1439 2022-09-13 12:40:12.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip86/bip86_coins.py
+-rw-rw-rw-   0        0        0     2963 2023-02-22 12:54:50.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip86/bip86_conf.py
+-rw-rw-rw-   0        0        0     2420 2022-09-13 12:40:12.000000 bip_utils-2.7.1/bip_utils/bip/conf/bip86/bip86_conf_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.040598 bip_utils-2.7.1/bip_utils/bip/conf/common/
+-rw-rw-rw-   0        0        0      437 2023-02-22 12:55:17.000000 bip_utils-2.7.1/bip_utils/bip/conf/common/__init__.py
+-rw-rw-rw-   0        0        0     4411 2022-09-13 12:40:13.000000 bip_utils-2.7.1/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py
+-rw-rw-rw-   0        0        0     7042 2022-09-13 12:40:14.000000 bip_utils-2.7.1/bip_utils/bip/conf/common/bip_coin_conf.py
+-rw-rw-rw-   0        0        0     1260 2022-09-13 12:40:14.000000 bip_utils-2.7.1/bip_utils/bip/conf/common/bip_coins.py
+-rw-rw-rw-   0        0        0     1400 2023-02-22 12:54:50.000000 bip_utils-2.7.1/bip_utils/bip/conf/common/bip_conf_const.py
+-rw-rw-rw-   0        0        0     5101 2022-12-05 13:46:33.000000 bip_utils-2.7.1/bip_utils/bip/conf/common/bip_litecoin_conf.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.045045 bip_utils-2.7.1/bip_utils/cardano/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:16.000000 bip_utils-2.7.1/bip_utils/cardano/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.067524 bip_utils-2.7.1/bip_utils/cardano/bip32/
+-rw-rw-rw-   0        0        0      165 2022-09-13 12:40:16.000000 bip_utils-2.7.1/bip_utils/cardano/bip32/__init__.py
+-rw-rw-rw-   0        0        0     3051 2022-09-13 12:40:16.000000 bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py
+-rw-rw-rw-   0        0        0     4290 2022-09-13 12:40:17.000000 bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py
+-rw-rw-rw-   0        0        0     4426 2022-09-13 12:40:17.000000 bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py
+-rw-rw-rw-   0        0        0     1975 2022-09-13 12:40:18.000000 bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_icarus_bip32.py
+-rw-rw-rw-   0        0        0     4150 2022-09-13 12:40:18.000000 bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.076042 bip_utils-2.7.1/bip_utils/cardano/byron/
+-rw-rw-rw-   0        0        0       77 2022-09-13 12:40:18.000000 bip_utils-2.7.1/bip_utils/cardano/byron/__init__.py
+-rw-rw-rw-   0        0        0     9560 2022-09-13 12:40:19.000000 bip_utils-2.7.1/bip_utils/cardano/byron/cardano_byron_legacy.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.084970 bip_utils-2.7.1/bip_utils/cardano/cip1852/
+-rw-rw-rw-   0        0        0       55 2022-09-13 12:40:19.000000 bip_utils-2.7.1/bip_utils/cardano/cip1852/__init__.py
+-rw-rw-rw-   0        0        0     8713 2022-09-13 12:40:20.000000 bip_utils-2.7.1/bip_utils/cardano/cip1852/cip1852.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.101882 bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/
+-rw-rw-rw-   0        0        0      222 2022-09-13 12:40:20.000000 bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/__init__.py
+-rw-rw-rw-   0        0        0     1495 2022-09-13 12:40:20.000000 bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/cip1852_coins.py
+-rw-rw-rw-   0        0        0     3791 2023-02-22 12:54:50.000000 bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/cip1852_conf.py
+-rw-rw-rw-   0        0        0     2652 2022-09-13 12:40:21.000000 bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.112620 bip_utils-2.7.1/bip_utils/cardano/mnemonic/
+-rw-rw-rw-   0        0        0      205 2022-09-13 12:40:21.000000 bip_utils-2.7.1/bip_utils/cardano/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     2656 2022-09-13 12:40:22.000000 bip_utils-2.7.1/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py
+-rw-rw-rw-   0        0        0     2513 2022-09-13 12:40:22.000000 bip_utils-2.7.1/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.124507 bip_utils-2.7.1/bip_utils/cardano/shelley/
+-rw-rw-rw-   0        0        0      182 2022-09-13 12:40:22.000000 bip_utils-2.7.1/bip_utils/cardano/shelley/__init__.py
+-rw-rw-rw-   0        0        0     7138 2022-09-13 12:40:23.000000 bip_utils-2.7.1/bip_utils/cardano/shelley/cardano_shelley.py
+-rw-rw-rw-   0        0        0     6383 2022-09-13 12:40:24.000000 bip_utils-2.7.1/bip_utils/cardano/shelley/cardano_shelley_keys.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.137336 bip_utils-2.7.1/bip_utils/coin_conf/
+-rw-rw-rw-   0        0        0      106 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/coin_conf/__init__.py
+-rw-rw-rw-   0        0        0     2258 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/coin_conf/coin_conf.py
+-rw-rw-rw-   0        0        0    22503 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/coin_conf/coins_conf.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.147286 bip_utils-2.7.1/bip_utils/ecc/
+-rw-rw-rw-   0        0        0     2046 2022-09-15 14:56:47.000000 bip_utils-2.7.1/bip_utils/ecc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.163815 bip_utils-2.7.1/bip_utils/ecc/common/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:25.000000 bip_utils-2.7.1/bip_utils/ecc/common/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-26 11:57:25.000000 bip_utils-2.7.1/bip_utils/ecc/common/dummy_point.py
+-rw-rw-rw-   0        0        0     6654 2022-09-13 12:40:26.000000 bip_utils-2.7.1/bip_utils/ecc/common/ikeys.py
+-rw-rw-rw-   0        0        0     4819 2023-05-25 20:41:55.000000 bip_utils-2.7.1/bip_utils/ecc/common/ipoint.py
+-rw-rw-rw-   0        0        0     1315 2022-11-25 13:55:56.000000 bip_utils-2.7.1/bip_utils/ecc/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.180096 bip_utils-2.7.1/bip_utils/ecc/curve/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:27.000000 bip_utils-2.7.1/bip_utils/ecc/curve/__init__.py
+-rw-rw-rw-   0        0        0     3851 2022-09-13 12:40:27.000000 bip_utils-2.7.1/bip_utils/ecc/curve/elliptic_curve.py
+-rw-rw-rw-   0        0        0     3135 2022-09-13 12:40:28.000000 bip_utils-2.7.1/bip_utils/ecc/curve/elliptic_curve_getter.py
+-rw-rw-rw-   0        0        0     1486 2022-09-13 12:40:28.000000 bip_utils-2.7.1/bip_utils/ecc/curve/elliptic_curve_types.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.186077 bip_utils-2.7.1/bip_utils/ecc/ecdsa/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:28.000000 bip_utils-2.7.1/bip_utils/ecc/ecdsa/__init__.py
+-rw-rw-rw-   0        0        0     1659 2022-09-13 12:40:29.000000 bip_utils-2.7.1/bip_utils/ecc/ecdsa/ecdsa_keys.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.208746 bip_utils-2.7.1/bip_utils/ecc/ed25519/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:29.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/__init__.py
+-rw-rw-rw-   0        0        0     1828 2022-09-13 12:40:29.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519.py
+-rw-rw-rw-   0        0        0     1761 2022-09-13 12:40:30.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_const.py
+-rw-rw-rw-   0        0        0     7409 2022-10-06 12:31:30.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_keys.py
+-rw-rw-rw-   0        0        0     6701 2023-05-25 20:54:04.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_point.py
+-rw-rw-rw-   0        0        0     2307 2022-09-22 18:31:27.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.213997 bip_utils-2.7.1/bip_utils/ecc/ed25519/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:32.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/lib/__init__.py
+-rw-rw-rw-   0        0        0    10382 2022-09-26 10:52:41.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519/lib/ed25519_lib.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.232245 bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:33.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/__init__.py
+-rw-rw-rw-   0        0        0     2003 2022-09-13 12:40:33.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py
+-rw-rw-rw-   0        0        0     1573 2022-09-13 12:40:33.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py
+-rw-rw-rw-   0        0        0     7358 2022-09-22 18:30:36.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py
+-rw-rw-rw-   0        0        0     1646 2022-09-13 12:40:35.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.252532 bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:35.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/__init__.py
+-rw-rw-rw-   0        0        0     1980 2022-09-13 12:40:35.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py
+-rw-rw-rw-   0        0        0     1576 2022-09-13 12:40:36.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py
+-rw-rw-rw-   0        0        0     5303 2022-09-22 18:51:23.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py
+-rw-rw-rw-   0        0        0     1642 2022-09-13 12:40:36.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.273240 bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:37.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/__init__.py
+-rw-rw-rw-   0        0        0     1980 2022-09-13 12:40:37.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero.py
+-rw-rw-rw-   0        0        0     1780 2022-09-13 12:40:37.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py
+-rw-rw-rw-   0        0        0     4174 2022-09-26 10:52:41.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py
+-rw-rw-rw-   0        0        0     1642 2022-09-15 10:52:38.000000 bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.291963 bip_utils-2.7.1/bip_utils/ecc/nist256p1/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:40.000000 bip_utils-2.7.1/bip_utils/ecc/nist256p1/__init__.py
+-rw-rw-rw-   0        0        0     1876 2022-09-13 12:40:40.000000 bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1.py
+-rw-rw-rw-   0        0        0     1606 2022-09-13 12:40:40.000000 bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1_const.py
+-rw-rw-rw-   0        0        0     7231 2022-09-13 12:40:41.000000 bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1_keys.py
+-rw-rw-rw-   0        0        0     6984 2023-05-25 20:43:27.000000 bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1_point.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.321541 bip_utils-2.7.1/bip_utils/ecc/secp256k1/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:42.000000 bip_utils-2.7.1/bip_utils/ecc/secp256k1/__init__.py
+-rw-rw-rw-   0        0        0     1783 2022-09-13 12:40:42.000000 bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1.py
+-rw-rw-rw-   0        0        0     2974 2022-09-13 12:40:43.000000 bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_const.py
+-rw-rw-rw-   0        0        0     7065 2022-09-13 12:40:43.000000 bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py
+-rw-rw-rw-   0        0        0     7301 2022-09-13 12:40:44.000000 bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py
+-rw-rw-rw-   0        0        0     6190 2023-05-25 20:43:43.000000 bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py
+-rw-rw-rw-   0        0        0     7030 2023-05-25 20:43:49.000000 bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.341868 bip_utils-2.7.1/bip_utils/ecc/sr25519/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:40:45.000000 bip_utils-2.7.1/bip_utils/ecc/sr25519/__init__.py
+-rw-rw-rw-   0        0        0     1828 2022-09-13 12:40:45.000000 bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519.py
+-rw-rw-rw-   0        0        0     1562 2022-09-13 12:40:46.000000 bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519_const.py
+-rw-rw-rw-   0        0        0     6498 2023-05-26 11:57:26.000000 bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519_keys.py
+-rw-rw-rw-   0        0        0     1321 2022-09-13 12:40:46.000000 bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519_point.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.352753 bip_utils-2.7.1/bip_utils/electrum/
+-rw-rw-rw-   0        0        0      136 2022-09-13 12:40:47.000000 bip_utils-2.7.1/bip_utils/electrum/__init__.py
+-rw-rw-rw-   0        0        0    10444 2022-09-13 12:40:47.000000 bip_utils-2.7.1/bip_utils/electrum/electrum_v1.py
+-rw-rw-rw-   0        0        0    12764 2022-09-13 12:40:48.000000 bip_utils-2.7.1/bip_utils/electrum/electrum_v2.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.394380 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/
+-rw-rw-rw-   0        0        0      770 2022-09-13 12:40:48.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/__init__.py
+-rw-rw-rw-   0        0        0     3183 2022-09-13 12:40:49.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py
+-rw-rw-rw-   0        0        0     2149 2022-09-13 12:40:49.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py
+-rw-rw-rw-   0        0        0     3685 2022-09-13 12:40:49.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     3162 2022-09-13 12:40:50.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     4396 2022-09-13 12:40:50.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     3890 2022-09-13 12:40:50.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2181 2022-09-13 12:40:51.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     3621 2022-09-13 12:40:51.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.397889 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/wordlist/
+-rw-rw-rw-   0        0        0    12120 2022-09-13 12:40:52.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/wordlist/english.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.438473 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/
+-rw-rw-rw-   0        0        0      795 2022-09-13 12:40:53.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/__init__.py
+-rw-rw-rw-   0        0        0     4300 2022-09-13 12:40:53.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py
+-rw-rw-rw-   0        0        0     2937 2022-09-13 12:40:54.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py
+-rw-rw-rw-   0        0        0     4499 2022-09-13 12:40:54.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     4249 2022-09-13 12:40:54.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     5966 2022-09-13 12:40:55.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     4266 2022-09-13 12:40:55.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2205 2022-09-13 12:40:55.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     3308 2022-09-13 12:40:56.000000 bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.460879 bip_utils-2.7.1/bip_utils/monero/
+-rw-rw-rw-   0        0        0      237 2022-09-13 12:40:56.000000 bip_utils-2.7.1/bip_utils/monero/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.483950 bip_utils-2.7.1/bip_utils/monero/conf/
+-rw-rw-rw-   0        0        0      256 2022-09-13 12:40:57.000000 bip_utils-2.7.1/bip_utils/monero/conf/__init__.py
+-rw-rw-rw-   0        0        0     3770 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/monero/conf/monero_coin_conf.py
+-rw-rw-rw-   0        0        0     1386 2022-09-13 12:40:58.000000 bip_utils-2.7.1/bip_utils/monero/conf/monero_coins.py
+-rw-rw-rw-   0        0        0     1748 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/monero/conf/monero_conf.py
+-rw-rw-rw-   0        0        0     2508 2022-09-13 12:40:59.000000 bip_utils-2.7.1/bip_utils/monero/conf/monero_conf_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.529610 bip_utils-2.7.1/bip_utils/monero/mnemonic/
+-rw-rw-rw-   0        0        0      718 2022-09-13 12:40:59.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     3191 2022-09-13 12:40:59.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_entropy_generator.py
+-rw-rw-rw-   0        0        0     3753 2022-09-13 12:41:00.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic.py
+-rw-rw-rw-   0        0        0     4355 2022-09-26 07:56:05.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py
+-rw-rw-rw-   0        0        0     6520 2022-09-13 12:41:01.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py
+-rw-rw-rw-   0        0        0     5109 2022-09-13 12:41:01.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_generator.py
+-rw-rw-rw-   0        0        0     4600 2022-09-26 07:56:07.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_utils.py
+-rw-rw-rw-   0        0        0     1872 2022-09-13 12:41:02.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_validator.py
+-rw-rw-rw-   0        0        0     2545 2022-09-13 12:41:02.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_seed_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.652596 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/
+-rw-rw-rw-   0        0        0     8130 2022-09-13 12:41:03.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt
+-rw-rw-rw-   0        0        0    14346 2022-09-13 12:41:03.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/dutch.txt
+-rw-rw-rw-   0        0        0    13093 2022-09-13 12:41:04.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/english.txt
+-rw-rw-rw-   0        0        0    12524 2022-09-13 12:41:05.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/french.txt
+-rw-rw-rw-   0        0        0    13960 2022-09-13 12:41:05.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/german.txt
+-rw-rw-rw-   0        0        0    14400 2022-09-13 12:41:05.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/italian.txt
+-rw-rw-rw-   0        0        0    21054 2022-09-13 12:41:06.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/japanese.txt
+-rw-rw-rw-   0        0        0    14765 2022-09-13 12:41:06.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/portuguese.txt
+-rw-rw-rw-   0        0        0    22376 2022-09-13 12:41:07.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/russian.txt
+-rw-rw-rw-   0        0        0    12524 2022-09-13 12:41:07.000000 bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/spanish.txt
+-rw-rw-rw-   0        0        0    10682 2022-09-23 19:18:29.000000 bip_utils-2.7.1/bip_utils/monero/monero.py
+-rw-rw-rw-   0        0        0     1244 2022-09-13 12:41:08.000000 bip_utils-2.7.1/bip_utils/monero/monero_ex.py
+-rw-rw-rw-   0        0        0     8202 2022-10-06 12:24:47.000000 bip_utils-2.7.1/bip_utils/monero/monero_keys.py
+-rw-rw-rw-   0        0        0     6050 2022-10-06 12:27:50.000000 bip_utils-2.7.1/bip_utils/monero/monero_subaddr.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.665449 bip_utils-2.7.1/bip_utils/slip/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:41:09.000000 bip_utils-2.7.1/bip_utils/slip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.670460 bip_utils-2.7.1/bip_utils/slip/slip173/
+-rw-rw-rw-   0        0        0       52 2022-09-13 12:41:09.000000 bip_utils-2.7.1/bip_utils/slip/slip173/__init__.py
+-rw-rw-rw-   0        0        0     2055 2022-09-13 12:41:09.000000 bip_utils-2.7.1/bip_utils/slip/slip173/slip173.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.685349 bip_utils-2.7.1/bip_utils/slip/slip32/
+-rw-rw-rw-   0        0        0      227 2022-09-13 12:41:10.000000 bip_utils-2.7.1/bip_utils/slip/slip32/__init__.py
+-rw-rw-rw-   0        0        0    11214 2022-09-13 12:41:11.000000 bip_utils-2.7.1/bip_utils/slip/slip32/slip32.py
+-rw-rw-rw-   0        0        0     2085 2022-09-13 12:41:11.000000 bip_utils-2.7.1/bip_utils/slip/slip32/slip32_key_net_ver.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.694378 bip_utils-2.7.1/bip_utils/slip/slip44/
+-rw-rw-rw-   0        0        0       49 2022-09-13 12:41:12.000000 bip_utils-2.7.1/bip_utils/slip/slip44/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-02-22 12:15:52.000000 bip_utils-2.7.1/bip_utils/slip/slip44/slip44.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.703800 bip_utils-2.7.1/bip_utils/solana/
+-rw-rw-rw-   0        0        0       49 2022-09-13 12:41:12.000000 bip_utils-2.7.1/bip_utils/solana/__init__.py
+-rw-rw-rw-   0        0        0     6588 2022-09-13 12:41:13.000000 bip_utils-2.7.1/bip_utils/solana/spl_token.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.716628 bip_utils-2.7.1/bip_utils/ss58/
+-rw-rw-rw-   0        0        0      112 2022-09-13 12:41:13.000000 bip_utils-2.7.1/bip_utils/ss58/__init__.py
+-rw-rw-rw-   0        0        0     5967 2022-09-13 12:41:14.000000 bip_utils-2.7.1/bip_utils/ss58/ss58.py
+-rw-rw-rw-   0        0        0     1243 2022-09-13 12:41:15.000000 bip_utils-2.7.1/bip_utils/ss58/ss58_ex.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.746806 bip_utils-2.7.1/bip_utils/substrate/
+-rw-rw-rw-   0        0        0      343 2022-09-13 12:41:16.000000 bip_utils-2.7.1/bip_utils/substrate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.773207 bip_utils-2.7.1/bip_utils/substrate/conf/
+-rw-rw-rw-   0        0        0      292 2022-09-13 12:41:16.000000 bip_utils-2.7.1/bip_utils/substrate/conf/__init__.py
+-rw-rw-rw-   0        0        0     3031 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/substrate/conf/substrate_coin_conf.py
+-rw-rw-rw-   0        0        0     1606 2022-09-13 12:41:17.000000 bip_utils-2.7.1/bip_utils/substrate/conf/substrate_coins.py
+-rw-rw-rw-   0        0        0     3116 2023-03-18 08:59:39.000000 bip_utils-2.7.1/bip_utils/substrate/conf/substrate_conf.py
+-rw-rw-rw-   0        0        0     3179 2022-09-13 12:41:18.000000 bip_utils-2.7.1/bip_utils/substrate/conf/substrate_conf_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.781624 bip_utils-2.7.1/bip_utils/substrate/mnemonic/
+-rw-rw-rw-   0        0        0      101 2022-09-13 12:41:18.000000 bip_utils-2.7.1/bip_utils/substrate/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     2973 2022-09-13 12:41:18.000000 bip_utils-2.7.1/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.803533 bip_utils-2.7.1/bip_utils/substrate/scale/
+-rw-rw-rw-   0        0        0      509 2022-09-13 12:41:19.000000 bip_utils-2.7.1/bip_utils/substrate/scale/__init__.py
+-rw-rw-rw-   0        0        0     1628 2022-09-13 12:41:19.000000 bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_base.py
+-rw-rw-rw-   0        0        0     1948 2022-09-13 12:41:20.000000 bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_bytes.py
+-rw-rw-rw-   0        0        0     3082 2022-09-13 12:41:21.000000 bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_cuint.py
+-rw-rw-rw-   0        0        0     4954 2022-09-13 12:41:21.000000 bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_uint.py
+-rw-rw-rw-   0        0        0    12628 2022-09-13 12:41:21.000000 bip_utils-2.7.1/bip_utils/substrate/substrate.py
+-rw-rw-rw-   0        0        0     1349 2022-09-13 12:41:22.000000 bip_utils-2.7.1/bip_utils/substrate/substrate_ex.py
+-rw-rw-rw-   0        0        0     8752 2022-09-13 12:41:22.000000 bip_utils-2.7.1/bip_utils/substrate/substrate_keys.py
+-rw-rw-rw-   0        0        0     9228 2022-09-13 12:41:23.000000 bip_utils-2.7.1/bip_utils/substrate/substrate_path.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.807446 bip_utils-2.7.1/bip_utils/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-13 12:41:23.000000 bip_utils-2.7.1/bip_utils/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.811463 bip_utils-2.7.1/bip_utils/utils/conf/
+-rw-rw-rw-   0        0        0       55 2022-09-13 12:41:24.000000 bip_utils-2.7.1/bip_utils/utils/conf/__init__.py
+-rw-rw-rw-   0        0        0     1881 2022-09-13 12:41:25.000000 bip_utils-2.7.1/bip_utils/utils/conf/coin_names.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.864431 bip_utils-2.7.1/bip_utils/utils/crypto/
+-rw-rw-rw-   0        0        0      748 2022-09-13 12:41:25.000000 bip_utils-2.7.1/bip_utils/utils/crypto/__init__.py
+-rw-rw-rw-   0        0        0     4043 2022-09-13 12:41:25.000000 bip_utils-2.7.1/bip_utils/utils/crypto/aes_ecb.py
+-rw-rw-rw-   0        0        0     5189 2022-09-13 12:41:26.000000 bip_utils-2.7.1/bip_utils/utils/crypto/blake2.py
+-rw-rw-rw-   0        0        0     3566 2022-09-13 12:41:27.000000 bip_utils-2.7.1/bip_utils/utils/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     3048 2022-09-13 12:41:27.000000 bip_utils-2.7.1/bip_utils/utils/crypto/crc.py
+-rw-rw-rw-   0        0        0     1944 2022-09-13 12:41:27.000000 bip_utils-2.7.1/bip_utils/utils/crypto/hash160.py
+-rw-rw-rw-   0        0        0     3822 2022-09-13 12:41:28.000000 bip_utils-2.7.1/bip_utils/utils/crypto/hmac.py
+-rw-rw-rw-   0        0        0     2613 2023-05-25 21:29:06.000000 bip_utils-2.7.1/bip_utils/utils/crypto/pbkdf2.py
+-rw-rw-rw-   0        0        0     1927 2022-09-13 12:41:28.000000 bip_utils-2.7.1/bip_utils/utils/crypto/ripemd.py
+-rw-rw-rw-   0        0        0     2561 2023-05-25 21:28:43.000000 bip_utils-2.7.1/bip_utils/utils/crypto/scrypt.py
+-rw-rw-rw-   0        0        0     4836 2022-09-13 12:41:29.000000 bip_utils-2.7.1/bip_utils/utils/crypto/sha2.py
+-rw-rw-rw-   0        0        0     3097 2022-09-13 12:41:30.000000 bip_utils-2.7.1/bip_utils/utils/crypto/sha3.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.905611 bip_utils-2.7.1/bip_utils/utils/misc/
+-rw-rw-rw-   0        0        0      501 2022-09-13 12:41:30.000000 bip_utils-2.7.1/bip_utils/utils/misc/__init__.py
+-rw-rw-rw-   0        0        0     3458 2022-09-13 12:41:31.000000 bip_utils-2.7.1/bip_utils/utils/misc/algo.py
+-rw-rw-rw-   0        0        0     4870 2022-09-13 12:41:32.000000 bip_utils-2.7.1/bip_utils/utils/misc/base32.py
+-rw-rw-rw-   0        0        0     3429 2022-09-13 12:41:33.000000 bip_utils-2.7.1/bip_utils/utils/misc/bit.py
+-rw-rw-rw-   0        0        0     6326 2022-09-13 12:41:33.000000 bip_utils-2.7.1/bip_utils/utils/misc/bytes.py
+-rw-rw-rw-   0        0        0     4344 2022-09-13 12:41:34.000000 bip_utils-2.7.1/bip_utils/utils/misc/cbor_indefinite_len_array.py
+-rw-rw-rw-   0        0        0     4924 2022-09-13 12:41:34.000000 bip_utils-2.7.1/bip_utils/utils/misc/data_bytes.py
+-rw-rw-rw-   0        0        0     3192 2022-09-13 12:41:34.000000 bip_utils-2.7.1/bip_utils/utils/misc/integer.py
+-rw-rw-rw-   0        0        0     1884 2022-09-13 12:41:35.000000 bip_utils-2.7.1/bip_utils/utils/misc/string.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.941913 bip_utils-2.7.1/bip_utils/utils/mnemonic/
+-rw-rw-rw-   0        0        0      643 2022-09-13 12:41:35.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/__init__.py
+-rw-rw-rw-   0        0        0     1976 2022-09-13 12:41:35.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/entropy_generator.py
+-rw-rw-rw-   0        0        0     3716 2022-09-13 12:41:36.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic.py
+-rw-rw-rw-   0        0        0     3895 2022-09-13 12:41:36.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_decoder_base.py
+-rw-rw-rw-   0        0        0     2578 2022-09-13 12:41:37.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_encoder_base.py
+-rw-rw-rw-   0        0        0     1251 2022-09-13 12:41:37.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_ex.py
+-rw-rw-rw-   0        0        0    10988 2022-09-26 07:56:25.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_utils.py
+-rw-rw-rw-   0        0        0     2860 2022-09-13 12:41:38.000000 bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.949825 bip_utils-2.7.1/bip_utils/utils/typing/
+-rw-rw-rw-   0        0        0       52 2022-09-13 12:41:39.000000 bip_utils-2.7.1/bip_utils/utils/typing/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-05-25 21:29:39.000000 bip_utils-2.7.1/bip_utils/utils/typing/literal.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:27.962721 bip_utils-2.7.1/bip_utils/wif/
+-rw-rw-rw-   0        0        0       70 2022-09-13 12:41:39.000000 bip_utils-2.7.1/bip_utils/wif/__init__.py
+-rw-rw-rw-   0        0        0     5624 2022-09-13 12:41:40.000000 bip_utils-2.7.1/bip_utils/wif/wif.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:26.225165 bip_utils-2.7.1/bip_utils.egg-info/
+-rw-rw-rw-   0        0        0    11916 2023-05-26 12:02:25.000000 bip_utils-2.7.1/bip_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14366 2023-05-26 12:02:26.000000 bip_utils-2.7.1/bip_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:02:25.000000 bip_utils-2.7.1/bip_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      320 2023-05-26 12:02:25.000000 bip_utils-2.7.1/bip_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 12:02:25.000000 bip_utils-2.7.1/bip_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      997 2023-02-22 12:21:26.000000 bip_utils-2.7.1/keywords.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:28.041707 bip_utils-2.7.1/readme/
+-rw-rw-rw-   0        0        0     5128 2022-08-08 18:27:56.000000 bip_utils-2.7.1/readme/algorand_mnemonic.md
+-rw-rw-rw-   0        0        0    17713 2022-08-08 18:27:15.000000 bip_utils-2.7.1/readme/bip32.md
+-rw-rw-rw-   0        0        0     3317 2022-06-22 12:42:18.000000 bip_utils-2.7.1/readme/bip38.md
+-rw-rw-rw-   0        0        0     7775 2022-08-08 18:29:07.000000 bip_utils-2.7.1/readme/bip39.md
+-rw-rw-rw-   0        0        0    20092 2023-02-22 12:16:44.000000 bip_utils-2.7.1/readme/bip44.md
+-rw-rw-rw-   0        0        0    17246 2022-08-08 18:36:03.000000 bip_utils-2.7.1/readme/cardano.md
+-rw-rw-rw-   0        0        0     4701 2022-08-08 18:36:17.000000 bip_utils-2.7.1/readme/electrum.md
+-rw-rw-rw-   0        0        0      767 2022-08-08 18:36:37.000000 bip_utils-2.7.1/readme/electrum_mnemonic.md
+-rw-rw-rw-   0        0        0     4827 2022-08-08 18:37:09.000000 bip_utils-2.7.1/readme/electrum_v1_mnemonic.md
+-rw-rw-rw-   0        0        0     8675 2022-08-08 18:38:17.000000 bip_utils-2.7.1/readme/electrum_v2_mnemonic.md
+-rw-rw-rw-   0        0        0     5035 2022-08-08 18:38:58.000000 bip_utils-2.7.1/readme/monero.md
+-rw-rw-rw-   0        0        0     6792 2022-08-08 18:40:03.000000 bip_utils-2.7.1/readme/monero_mnemonic.md
+-rw-rw-rw-   0        0        0     8496 2022-08-08 18:41:26.000000 bip_utils-2.7.1/readme/substrate.md
+drwxrwxrwx   0        0        0        0 2023-05-26 12:02:28.075634 bip_utils-2.7.1/readme/utility/
+-rw-rw-rw-   0        0        0    16914 2023-02-22 11:50:35.000000 bip_utils-2.7.1/readme/utility/addr.md
+-rw-rw-rw-   0        0        0     1500 2022-08-08 18:41:47.000000 bip_utils-2.7.1/readme/utility/base58.md
+-rw-rw-rw-   0        0        0      613 2022-06-29 09:24:21.000000 bip_utils-2.7.1/readme/utility/bch_addr_converter.md
+-rw-rw-rw-   0        0        0     1242 2022-08-08 18:42:01.000000 bip_utils-2.7.1/readme/utility/bech32.md
+-rw-rw-rw-   0        0        0     1433 2022-06-29 07:19:26.000000 bip_utils-2.7.1/readme/utility/slip32.md
+-rw-rw-rw-   0        0        0      991 2022-06-29 09:09:58.000000 bip_utils-2.7.1/readme/utility/solana_spl.md
+-rw-rw-rw-   0        0        0      441 2022-06-29 08:56:27.000000 bip_utils-2.7.1/readme/utility/ss58.md
+-rw-rw-rw-   0        0        0     1940 2022-08-08 18:42:10.000000 bip_utils-2.7.1/readme/utility/wif.md
+-rw-rw-rw-   0        0        0      874 2022-06-29 09:25:30.000000 bip_utils-2.7.1/readme/utility_libs.md
+-rw-rw-rw-   0        0        0      124 2022-08-11 20:25:09.000000 bip_utils-2.7.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0      154 2022-08-07 19:59:17.000000 bip_utils-2.7.1/requirements.txt
+-rw-rw-rw-   0        0        0      111 2023-05-26 12:02:28.087837 bip_utils-2.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     6055 2022-10-26 13:18:53.000000 bip_utils-2.7.1/setup.py
```

### Comparing `bip_utils-2.7.0/LICENSE` & `bip_utils-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/PKG-INFO` & `bip_utils-2.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bip_utils
-Version: 2.7.0
+Version: 2.7.1
 Summary: Generation of mnemonics, seeds, private/public keys and addresses for different types of cryptocurrencies
 Home-page: https://github.com/ebellocchia/bip_utils
-Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.7.0.tar.gz
+Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.7.1.tar.gz
 Author: Emanuele Bellocchia
 Author-email: ebellocchia@gmail.com
 Maintainer: Emanuele Bellocchia
 Maintainer-email: ebellocchia@gmail.com
 License: MIT
-Keywords: python,cryptography,ecdsa,ed25519,ed25519-blake2b,nist256p1,secp256k1,sr25519,wallet,hd-wallet,slip10,slip32,bip38,bip39,bip39-substrate,bip32,bip44,bip49,bip84,bip86,bip173,bip350,base58,ss58,bech32,bech32m,segwit,electrum,substrate,taproot,daedalus,byron,shelley,akash,algorand,atom,avalanche,avax,axelar,band protocol,binance chain,binance smart chain,bitcoin,bitcoin cash,bitcoinsv,bnb,cardano,cardano-byron,cardano-shelley,celo,certik,cosmos,dash,dogecoin,ecash,elrond,eos,ethereum,ethereum classic,fantom opera,filecoin,harmony one,huobi chain,icon,iris,irisnet,kava,litecoin,matic,monero,okex chain,ontology,osmosis,nano,near,near protocol,neo,polygon,ripple,secret,solana,stellar,substrate,terra,tezos,theta,tron,vechain,verge,zcash,zilliqa,acala,bifrost,chainx,edgeware,karura,kusama,moonbeam,moonriver,phala,plasm,sora,stafi,polkadot
+Keywords: python,cryptography,ecdsa,ed25519,ed25519-blake2b,nist256p1,secp256k1,sr25519,wallet,hd-wallet,slip10,slip32,bip38,bip39,bip39-substrate,bip32,bip44,bip49,bip84,bip86,bip173,bip350,base58,ss58,bech32,bech32m,segwit,electrum,substrate,taproot,daedalus,byron,shelley,akash,algorand,aptos,atom,avalanche,avax,axelar,band protocol,binance chain,binance smart chain,bitcoin,bitcoin cash,bitcoinsv,bnb,cardano,cardano-byron,cardano-shelley,celo,certik,cosmos,dash,dogecoin,ecash,elrond,eos,ethereum,ethereum classic,fantom opera,filecoin,harmony one,huobi chain,icon,iris,irisnet,kava,litecoin,matic,monero,okex chain,ontology,osmosis,nano,near,near protocol,neo,pi network,polygon,ripple,secret,solana,stellar,substrate,terra,tezos,theta,tron,vechain,verge,zcash,zilliqa,acala,bifrost,chainx,edgeware,karura,kusama,moonbeam,moonriver,phala,plasm,sora,stafi,polkadot
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
@@ -82,14 +83,15 @@
 Please note that, for the py-sr25519-bindings library, Rust is required to be installed.
 
 ## Supported coins
 
 Supported BIP coins:
 - Akash Network
 - Algorand
+- Aptos
 - Avalanche (all the 3 chains)
 - Axelar
 - Band Protocol
 - Binance Chain
 - Binance Smart Chain
 - Bitcoin (and related test net)
 - Bitcoin Cash (and related test net)
@@ -118,14 +120,15 @@
 - Monero (based on BIP44 and secp256k1 or ed25519 SLIP-0010, it won't generate the same addresses of the official wallets, but it supports subaddresses generation)
 - Nano
 - Near Protocol
 - NEO
 - OKEx Chain (Ethereum and Cosmos addresses)
 - Ontology
 - Osmosis
+- Pi Network
 - Polkadot (based on BIP44 and ed25519 SLIP-0010, like TrustWallet, it won't generate the same addresses of Polkadot-JS)
 - Polygon
 - Ripple
 - Secret Network
 - Solana
 - Stellar
 - Terra
@@ -181,15 +184,17 @@
 
             pip install . --install-option="--coincurve=0"
 
     - Using *pip*, from PyPI:
 
             pip install bip_utils --install-option="--coincurve=0"
 
-**NOTE:** if you are using an Apple M1, please make sure to update *coincurve* to version 17.0.0 otherwise it won't work.
+**NOTES:**
+- if you are using an Apple M1, please make sure to update *coincurve* to version 17.0.0
+- in case of problems when building the *ed25519_blake2b* library, you can try one of the prebuilt wheels [here](https://github.com/ebellocchia/bip_utils/tree/master/libs_wheels)
 
 To run tests:
 
     python -m unittest discover
 
 Or you can install *tox*:
```

### Comparing `bip_utils-2.7.0/README.md` & `bip_utils-2.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 Please note that, for the py-sr25519-bindings library, Rust is required to be installed.
 
 ## Supported coins
 
 Supported BIP coins:
 - Akash Network
 - Algorand
+- Aptos
 - Avalanche (all the 3 chains)
 - Axelar
 - Band Protocol
 - Binance Chain
 - Binance Smart Chain
 - Bitcoin (and related test net)
 - Bitcoin Cash (and related test net)
@@ -92,14 +93,15 @@
 - Monero (based on BIP44 and secp256k1 or ed25519 SLIP-0010, it won't generate the same addresses of the official wallets, but it supports subaddresses generation)
 - Nano
 - Near Protocol
 - NEO
 - OKEx Chain (Ethereum and Cosmos addresses)
 - Ontology
 - Osmosis
+- Pi Network
 - Polkadot (based on BIP44 and ed25519 SLIP-0010, like TrustWallet, it won't generate the same addresses of Polkadot-JS)
 - Polygon
 - Ripple
 - Secret Network
 - Solana
 - Stellar
 - Terra
@@ -155,15 +157,17 @@
 
             pip install . --install-option="--coincurve=0"
 
     - Using *pip*, from PyPI:
 
             pip install bip_utils --install-option="--coincurve=0"
 
-**NOTE:** if you are using an Apple M1, please make sure to update *coincurve* to version 17.0.0 otherwise it won't work.
+**NOTES:**
+- if you are using an Apple M1, please make sure to update *coincurve* to version 17.0.0
+- in case of problems when building the *ed25519_blake2b* library, you can try one of the prebuilt wheels [here](https://github.com/ebellocchia/bip_utils/tree/master/libs_wheels)
 
 To run tests:
 
     python -m unittest discover
 
 Or you can install *tox*:
```

### Comparing `bip_utils-2.7.0/bip_utils/__init__.py` & `bip_utils-2.7.1/bip_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from bip_utils._version import __version__
 
 # Address computation
 from bip_utils.addr import (
     AdaByronAddrDecoder, AdaByronAddrTypes, AdaByronIcarusAddr, AdaByronIcarusAddrEncoder, AdaByronLegacyAddr,
     AdaByronLegacyAddrEncoder, AdaShelleyAddr, AdaShelleyAddrDecoder, AdaShelleyAddrEncoder, AdaShelleyAddrNetworkTags,
     AdaShelleyRewardAddr, AdaShelleyRewardAddrDecoder, AdaShelleyRewardAddrEncoder, AdaShelleyStakingAddr,
-    AdaShelleyStakingAddrDecoder, AdaShelleyStakingAddrEncoder, AlgoAddr, AlgoAddrDecoder, AlgoAddrEncoder, AtomAddr,
-    AtomAddrDecoder, AtomAddrEncoder, AvaxPChainAddr, AvaxPChainAddrDecoder, AvaxPChainAddrEncoder, AvaxXChainAddr,
-    AvaxXChainAddrDecoder, AvaxXChainAddrEncoder, BchAddrConverter, BchP2PKHAddr, BchP2PKHAddrDecoder,
-    BchP2PKHAddrEncoder, BchP2SHAddr, BchP2SHAddrDecoder, BchP2SHAddrEncoder, EgldAddr, EgldAddrDecoder,
-    EgldAddrEncoder, EosAddr, EosAddrDecoder, EosAddrEncoder, ErgoNetworkTypes, ErgoP2PKHAddr, ErgoP2PKHAddrDecoder,
-    ErgoP2PKHAddrEncoder, EthAddr, EthAddrDecoder, EthAddrEncoder, FilSecp256k1Addr, FilSecp256k1AddrDecoder,
-    FilSecp256k1AddrEncoder, IcxAddr, IcxAddrDecoder, IcxAddrEncoder, NanoAddr, NanoAddrDecoder, NanoAddrEncoder,
-    NearAddr, NearAddrDecoder, NearAddrEncoder, NeoAddr, NeoAddrDecoder, NeoAddrEncoder, OkexAddr, OkexAddrDecoder,
-    OkexAddrEncoder, OneAddr, OneAddrDecoder, OneAddrEncoder, P2PKHAddr, P2PKHAddrDecoder, P2PKHAddrEncoder,
-    P2PKHPubKeyModes, P2SHAddr, P2SHAddrDecoder, P2SHAddrEncoder, P2TRAddr, P2TRAddrDecoder, P2TRAddrEncoder,
-    P2WPKHAddr, P2WPKHAddrDecoder, P2WPKHAddrEncoder, SolAddr, SolAddrDecoder, SolAddrEncoder, SubstrateEd25519Addr,
-    SubstrateEd25519AddrDecoder, SubstrateEd25519AddrEncoder, SubstrateSr25519Addr, SubstrateSr25519AddrDecoder,
-    SubstrateSr25519AddrEncoder, TrxAddr, TrxAddrDecoder, TrxAddrEncoder, XlmAddr, XlmAddrDecoder, XlmAddrEncoder,
-    XlmAddrTypes, XmrAddr, XmrAddrDecoder, XmrAddrEncoder, XmrIntegratedAddr, XmrIntegratedAddrDecoder,
-    XmrIntegratedAddrEncoder, XrpAddr, XrpAddrDecoder, XrpAddrEncoder, XtzAddr, XtzAddrDecoder, XtzAddrEncoder,
-    XtzAddrPrefixes, ZilAddr, ZilAddrDecoder, ZilAddrEncoder
+    AdaShelleyStakingAddrDecoder, AdaShelleyStakingAddrEncoder, AlgoAddr, AlgoAddrDecoder, AlgoAddrEncoder, AptosAddr,
+    AptosAddrDecoder, AptosAddrEncoder, AtomAddr, AtomAddrDecoder, AtomAddrEncoder, AvaxPChainAddr,
+    AvaxPChainAddrDecoder, AvaxPChainAddrEncoder, AvaxXChainAddr, AvaxXChainAddrDecoder, AvaxXChainAddrEncoder,
+    BchAddrConverter, BchP2PKHAddr, BchP2PKHAddrDecoder, BchP2PKHAddrEncoder, BchP2SHAddr, BchP2SHAddrDecoder,
+    BchP2SHAddrEncoder, EgldAddr, EgldAddrDecoder, EgldAddrEncoder, EosAddr, EosAddrDecoder, EosAddrEncoder,
+    ErgoNetworkTypes, ErgoP2PKHAddr, ErgoP2PKHAddrDecoder, ErgoP2PKHAddrEncoder, EthAddr, EthAddrDecoder,
+    EthAddrEncoder, FilSecp256k1Addr, FilSecp256k1AddrDecoder, FilSecp256k1AddrEncoder, IcxAddr, IcxAddrDecoder,
+    IcxAddrEncoder, NanoAddr, NanoAddrDecoder, NanoAddrEncoder, NearAddr, NearAddrDecoder, NearAddrEncoder, NeoAddr,
+    NeoAddrDecoder, NeoAddrEncoder, OkexAddr, OkexAddrDecoder, OkexAddrEncoder, OneAddr, OneAddrDecoder, OneAddrEncoder,
+    P2PKHAddr, P2PKHAddrDecoder, P2PKHAddrEncoder, P2PKHPubKeyModes, P2SHAddr, P2SHAddrDecoder, P2SHAddrEncoder,
+    P2TRAddr, P2TRAddrDecoder, P2TRAddrEncoder, P2WPKHAddr, P2WPKHAddrDecoder, P2WPKHAddrEncoder, SolAddr,
+    SolAddrDecoder, SolAddrEncoder, SubstrateEd25519Addr, SubstrateEd25519AddrDecoder, SubstrateEd25519AddrEncoder,
+    SubstrateSr25519Addr, SubstrateSr25519AddrDecoder, SubstrateSr25519AddrEncoder, TrxAddr, TrxAddrDecoder,
+    TrxAddrEncoder, XlmAddr, XlmAddrDecoder, XlmAddrEncoder, XlmAddrTypes, XmrAddr, XmrAddrDecoder, XmrAddrEncoder,
+    XmrIntegratedAddr, XmrIntegratedAddrDecoder, XmrIntegratedAddrEncoder, XrpAddr, XrpAddrDecoder, XrpAddrEncoder,
+    XtzAddr, XtzAddrDecoder, XtzAddrEncoder, XtzAddrPrefixes, ZilAddr, ZilAddrDecoder, ZilAddrEncoder
 )
 
 # Algorand mnemonic
 from bip_utils.algorand.mnemonic import (
     AlgorandEntropyBitLen, AlgorandEntropyGenerator, AlgorandLanguages, AlgorandMnemonic, AlgorandMnemonicDecoder,
     AlgorandMnemonicEncoder, AlgorandMnemonicGenerator, AlgorandMnemonicValidator, AlgorandSeedGenerator,
     AlgorandWordsNum
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/P2PKH_addr.py` & `bip_utils-2.7.1/bip_utils/addr/P2PKH_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         net_ver_bytes = kwargs["net_ver"]
         base58_alph = kwargs.get("base58_alph", Base58Alphabets.BITCOIN)
 
         try:
             addr_dec_bytes = Base58Decoder.CheckDecode(addr, base58_alph)
         except Base58ChecksumError as ex:
             raise ValueError("Invalid base58 checksum") from ex
-        else:
-            # Validate length
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        Hash160.DigestSize() + len(net_ver_bytes))
-            # Validate and remove prefix
-            return AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, net_ver_bytes)
+
+        # Validate length
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    Hash160.DigestSize() + len(net_ver_bytes))
+        # Validate and remove prefix
+        return AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, net_ver_bytes)
 
 
 class P2PKHAddrEncoder(IAddrEncoder):
     """
     P2PKH address encoder class.
     It allows the Pay-to-Public-Key-Hash address encoding.
     """
@@ -150,23 +150,23 @@
         hrp = kwargs["hrp"]
         net_ver_bytes = kwargs["net_ver"]
 
         try:
             net_ver_bytes_got, addr_dec_bytes = BchBech32Decoder.Decode(hrp, addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            # Check net version
-            if net_ver_bytes != net_ver_bytes_got:
-                raise ValueError(f"Invalid net version (expected {BytesUtils.ToHexString(net_ver_bytes)}, "
-                                 f"got {BytesUtils.ToHexString(net_ver_bytes_got)})")
-            # Validate length
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        Hash160.DigestSize())
-            return addr_dec_bytes
+
+        # Check net version
+        if net_ver_bytes != net_ver_bytes_got:
+            raise ValueError(f"Invalid net version (expected {BytesUtils.ToHexString(net_ver_bytes)}, "
+                             f"got {BytesUtils.ToHexString(net_ver_bytes_got)})")
+        # Validate length
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    Hash160.DigestSize())
+        return addr_dec_bytes
 
 
 class BchP2PKHAddrEncoder(IAddrEncoder):
     """
     Bitcoin Cash P2PKH address encoder class.
     It allows the Bitcoin Cash P2PKH encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/P2SH_addr.py` & `bip_utils-2.7.1/bip_utils/addr/P2SH_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/P2TR_addr.py` & `bip_utils-2.7.1/bip_utils/addr/P2TR_addr.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,16 +81,19 @@
             pub_key (IPublicKey object): Public key
 
         Returns:
             bytes: Computed hash
         """
 
         # Use the pre-computed SHA256 of "TapTweak" for speeding up
-        return _P2TRUtils.TaggedHash(P2TRConst.TAP_TWEAK_SHA256,
-                                     IntegerUtils.ToBytes(pub_key.Point().X()))
+        return _P2TRUtils.TaggedHash(
+            P2TRConst.TAP_TWEAK_SHA256,
+            IntegerUtils.ToBytes(pub_key.Point().X(),
+                                 bytes_num=Secp256k1Point.CoordinateLength())
+        )
 
     @staticmethod
     def LiftX(pub_key: IPublicKey) -> IPoint:
         """
         Implementation of the lift_x function as defined by BIP-0340.
         It computes the point P for which P.X() = pub_key.X() and has_even_y(P).
 
@@ -123,15 +126,16 @@
             pub_key (IPublicKey object): Public key
 
         Returns:
             bytes: X coordinate of the tweaked public key
         """
         h = _P2TRUtils.HashTapTweak(pub_key)
         out_point = _P2TRUtils.LiftX(pub_key) + (BytesUtils.ToInteger(h) * Secp256k1.Generator())
-        return IntegerUtils.ToBytes(out_point.X())
+        return IntegerUtils.ToBytes(out_point.X(),
+                                    bytes_num=Secp256k1Point.CoordinateLength())
 
 
 class P2TRAddrDecoder(IAddrDecoder):
     """
     P2WPKH address decoder class.
     It allows the Pay-to-Witness-Public-Key-Hash address decoding.
     """
@@ -156,21 +160,21 @@
         """
         hrp = kwargs["hrp"]
 
         try:
             wit_ver_got, addr_dec_bytes = SegwitBech32Decoder.Decode(hrp, addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            # Validate length
-            AddrDecUtils.ValidateLength(addr_dec_bytes, Secp256k1PublicKey.CompressedLength() - 1)
-            # Check witness version
-            if wit_ver_got != P2TRConst.WITNESS_VER:
-                raise ValueError(f"Invalid witness version (expected {P2TRConst.WITNESS_VER}, got {wit_ver_got})")
-            return addr_dec_bytes
+
+        # Validate length
+        AddrDecUtils.ValidateLength(addr_dec_bytes, Secp256k1PublicKey.CompressedLength() - 1)
+        # Check witness version
+        if wit_ver_got != P2TRConst.WITNESS_VER:
+            raise ValueError(f"Invalid witness version (expected {P2TRConst.WITNESS_VER}, got {wit_ver_got})")
+        return addr_dec_bytes
 
 
 class P2TRAddrEncoder(IAddrEncoder):
     """
     P2TR address encoder class.
     It allows the Pay-to-Taproot address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/P2WPKH_addr.py` & `bip_utils-2.7.1/bip_utils/addr/P2WPKH_addr.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,20 +71,20 @@
         hrp = kwargs["hrp"]
 
         try:
             # SegwitBech32Decoder also validates the length
             wit_ver_got, addr_dec_bytes = SegwitBech32Decoder.Decode(hrp, addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            # Check witness version
-            if wit_ver_got != P2WPKHAddrConst.WITNESS_VER:
-                raise ValueError(f"Invalid witness version (expected {P2WPKHAddrConst.WITNESS_VER}, "
-                                 f"got {wit_ver_got})")
-            return addr_dec_bytes
+
+        # Check witness version
+        if wit_ver_got != P2WPKHAddrConst.WITNESS_VER:
+            raise ValueError(f"Invalid witness version (expected {P2WPKHAddrConst.WITNESS_VER}, "
+                             f"got {wit_ver_got})")
+        return addr_dec_bytes
 
 
 class P2WPKHAddrEncoder(IAddrEncoder):
     """
     P2WPKH address encoder class.
     It allows the Pay-to-Witness-Public-Key-Hash address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/__init__.py` & `bip_utils-2.7.1/bip_utils/addr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 )
 from bip_utils.addr.ada_shelley_addr import (
     AdaShelleyAddr, AdaShelleyAddrDecoder, AdaShelleyAddrEncoder, AdaShelleyAddrNetworkTags, AdaShelleyRewardAddr,
     AdaShelleyRewardAddrDecoder, AdaShelleyRewardAddrEncoder, AdaShelleyStakingAddr, AdaShelleyStakingAddrDecoder,
     AdaShelleyStakingAddrEncoder
 )
 from bip_utils.addr.algo_addr import AlgoAddr, AlgoAddrDecoder, AlgoAddrEncoder
+from bip_utils.addr.aptos_addr import AptosAddr, AptosAddrDecoder, AptosAddrEncoder
 from bip_utils.addr.atom_addr import AtomAddr, AtomAddrDecoder, AtomAddrEncoder
 from bip_utils.addr.avax_addr import (
     AvaxPChainAddr, AvaxPChainAddrDecoder, AvaxPChainAddrEncoder, AvaxXChainAddr, AvaxXChainAddrDecoder,
     AvaxXChainAddrEncoder
 )
 from bip_utils.addr.bch_addr_converter import BchAddrConverter
 from bip_utils.addr.egld_addr import EgldAddr, EgldAddrDecoder, EgldAddrEncoder
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/ada_byron_addr.py` & `bip_utils-2.7.1/bip_utils/addr/ada_byron_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/ada_shelley_addr.py` & `bip_utils-2.7.1/bip_utils/addr/ada_shelley_addr.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,21 @@
 
         # Decode bech32
         try:
             addr_dec_bytes = Bech32Decoder.Decode(AdaShelleyAddrConst.NETWORK_TAG_TO_ADDR_HRP[net_tag],
                                                   addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        (Blake2b224.DigestSize() * 2) + 1)
-            # Validate and remove prefix
-            prefix_byte = _AdaShelleyAddrUtils.EncodePrefix(AdaShelleyAddrHeaderTypes.PAYMENT,
-                                                            net_tag)
-            return AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, prefix_byte)
+
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    (Blake2b224.DigestSize() * 2) + 1)
+        # Validate and remove prefix
+        prefix_byte = _AdaShelleyAddrUtils.EncodePrefix(AdaShelleyAddrHeaderTypes.PAYMENT,
+                                                        net_tag)
+        return AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, prefix_byte)
 
 
 class AdaShelleyAddrEncoder(IAddrEncoder):
     """
     Cardano Shelley address encoder class.
     It allows the Cardano Shelley address encoding.
     """
@@ -224,21 +224,21 @@
 
         # Decode bech32
         try:
             addr_dec_bytes = Bech32Decoder.Decode(AdaShelleyAddrConst.NETWORK_TAG_TO_REWARD_ADDR_HRP[net_tag],
                                                   addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        Blake2b224.DigestSize() + 1)
-            # Validate and remove prefix
-            prefix_byte = _AdaShelleyAddrUtils.EncodePrefix(AdaShelleyAddrHeaderTypes.REWARD,
-                                                            net_tag)
-            return AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, prefix_byte)
+
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    Blake2b224.DigestSize() + 1)
+        # Validate and remove prefix
+        prefix_byte = _AdaShelleyAddrUtils.EncodePrefix(AdaShelleyAddrHeaderTypes.REWARD,
+                                                        net_tag)
+        return AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, prefix_byte)
 
 
 class AdaShelleyStakingAddrEncoder(IAddrEncoder):
     """
     Cardano Shelley staking address encoder class.
     It allows the Cardano Shelley staking address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/addr_dec_utils.py` & `bip_utils-2.7.1/bip_utils/addr/addr_dec_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/addr_key_validator.py` & `bip_utils-2.7.1/bip_utils/addr/addr_key_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/algo_addr.py` & `bip_utils-2.7.1/bip_utils/addr/algo_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/atom_addr.py` & `bip_utils-2.7.1/bip_utils/addr/atom_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,18 @@
         """
         hrp = kwargs["hrp"]
 
         try:
             addr_dec_bytes = Bech32Decoder.Decode(hrp, addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        Hash160.DigestSize())
-            return addr_dec_bytes
+
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    Hash160.DigestSize())
+        return addr_dec_bytes
 
 
 class AtomAddrEncoder(IAddrEncoder):
     """
     Atom address encoder class.
     It allows the Atom address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/avax_addr.py` & `bip_utils-2.7.1/bip_utils/addr/avax_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/bch_addr_converter.py` & `bip_utils-2.7.1/bip_utils/addr/bch_addr_converter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/egld_addr.py` & `bip_utils-2.7.1/bip_utils/addr/egld_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,20 +56,20 @@
             ValueError: If the address encoding is not valid
         """
         try:
             addr_dec_bytes = Bech32Decoder.Decode(CoinsConf.Elrond.ParamByKey("addr_hrp"),
                                                   addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        Ed25519PublicKey.CompressedLength() - 1)
-            AddrDecUtils.ValidatePubKey(addr_dec_bytes, Ed25519PublicKey)
 
-            return addr_dec_bytes
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    Ed25519PublicKey.CompressedLength() - 1)
+        AddrDecUtils.ValidatePubKey(addr_dec_bytes, Ed25519PublicKey)
+
+        return addr_dec_bytes
 
 
 class EgldAddrEncoder(IAddrEncoder):
     """
     Elrond address encoder class.
     It allows the Elrond address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/eos_addr.py` & `bip_utils-2.7.1/bip_utils/addr/eos_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/ergo_addr.py` & `bip_utils-2.7.1/bip_utils/addr/ergo_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/eth_addr.py` & `bip_utils-2.7.1/bip_utils/addr/eth_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         # Validate and remove prefix
         addr_no_prefix = AddrDecUtils.ValidateAndRemovePrefix(addr,
                                                               CoinsConf.Ethereum.ParamByKey("addr_prefix"))
         # Validate length
         AddrDecUtils.ValidateLength(addr_no_prefix, EthAddrConst.ADDR_LEN)
         # Check checksum encoding
         if not skip_chksum_enc and addr_no_prefix != _EthAddrUtils.ChecksumEncode(addr_no_prefix):
-            raise ValueError("Invalid checksum encode")
+            raise ValueError("Invalid checksum encoding")
 
         return BytesUtils.FromHexString(addr_no_prefix)
 
 
 class EthAddrEncoder(IAddrEncoder):
     """
     Ethereum address encoder class.
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/fil_addr.py` & `bip_utils-2.7.1/bip_utils/addr/fil_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/iaddr_decoder.py` & `bip_utils-2.7.1/bip_utils/addr/iaddr_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/iaddr_encoder.py` & `bip_utils-2.7.1/bip_utils/addr/iaddr_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/icx_addr.py` & `bip_utils-2.7.1/bip_utils/addr/icx_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/nano_addr.py` & `bip_utils-2.7.1/bip_utils/addr/nano_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/near_addr.py` & `bip_utils-2.7.1/bip_utils/addr/near_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/neo_addr.py` & `bip_utils-2.7.1/bip_utils/addr/neo_addr.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 from bip_utils.utils.crypto import Hash160
 from bip_utils.utils.misc import BytesUtils, IntegerUtils
 
 
 class NeoAddrConst:
     """Class container for NEO address constants."""
 
-    # Address prefix
-    PREFIX: bytes = b"\x21"
-    # Address suffix
-    SUFFIX: bytes = b"\xac"
+    # Address prefix byte
+    PREFIX_BYTE: bytes = b"\x21"
+    # Address suffix byte
+    SUFFIX_BYTE: bytes = b"\xac"
 
 
 class NeoAddrDecoder(IAddrDecoder):
     """
     Neo address decoder class.
     It allows the Neo address decoding.
     """
@@ -69,25 +69,25 @@
         ver_bytes = kwargs["ver"]
 
         try:
             # Decode from base58
             addr_dec_bytes = Base58Decoder.CheckDecode(addr)
         except Base58ChecksumError as ex:
             raise ValueError("Invalid base58 checksum") from ex
-        else:
-            # Validate length
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        Hash160.DigestSize() + len(ver_bytes))
-            # Check version
-            ver_got = IntegerUtils.ToBytes(addr_dec_bytes[0])
-            if ver_bytes != ver_got:
-                raise ValueError(f"Invalid version (expected {BytesUtils.ToHexString(ver_bytes)}, "
-                                 f"got {BytesUtils.ToHexString(ver_got)})")
 
-            return addr_dec_bytes[1:]
+        # Validate length
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    Hash160.DigestSize() + len(ver_bytes))
+        # Check version
+        ver_got = IntegerUtils.ToBytes(addr_dec_bytes[0])
+        if ver_bytes != ver_got:
+            raise ValueError(f"Invalid version (expected {BytesUtils.ToHexString(ver_bytes)}, "
+                             f"got {BytesUtils.ToHexString(ver_got)})")
+
+        return addr_dec_bytes[1:]
 
 
 class NeoAddrEncoder(IAddrEncoder):
     """
     Neo address encoder class.
     It allows the Neo address encoding.
     """
@@ -112,16 +112,16 @@
             TypeError: If the public key is not ed25519
         """
         ver_bytes = kwargs["ver"]
 
         pub_key_obj = AddrKeyValidator.ValidateAndGetNist256p1Key(pub_key)
 
         # Get payload
-        payload_bytes = (NeoAddrConst.PREFIX
+        payload_bytes = (NeoAddrConst.PREFIX_BYTE
                          + pub_key_obj.RawCompressed().ToBytes()
-                         + NeoAddrConst.SUFFIX)
+                         + NeoAddrConst.SUFFIX_BYTE)
         # Encode to base58
         return Base58Encoder.CheckEncode(ver_bytes + Hash160.QuickDigest(payload_bytes))
 
 
 # Deprecated: only for compatibility, Encoder class shall be used instead
 NeoAddr = NeoAddrEncoder
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/okex_addr.py` & `bip_utils-2.7.1/bip_utils/addr/okex_addr.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,19 +55,19 @@
             ValueError: If the address encoding is not valid
         """
         try:
             addr_dec_bytes = Bech32Decoder.Decode(CoinsConf.OkexChain.ParamByKey("addr_hrp"),
                                                   addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            return EthAddrDecoder.DecodeAddr(
-                CoinsConf.Ethereum.ParamByKey("addr_prefix") + BytesUtils.ToHexString(addr_dec_bytes),
-                skip_chksum_enc=True
-            )
+
+        return EthAddrDecoder.DecodeAddr(
+            CoinsConf.Ethereum.ParamByKey("addr_prefix") + BytesUtils.ToHexString(addr_dec_bytes),
+            skip_chksum_enc=True
+        )
 
 
 class OkexAddrEncoder(IAddrEncoder):
     """
     OKEx Chain address encoder class.
     It allows the OKEx Chain address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/one_addr.py` & `bip_utils-2.7.1/bip_utils/addr/one_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,19 +55,19 @@
             ValueError: If the address encoding is not valid
         """
         try:
             addr_dec_bytes = Bech32Decoder.Decode(CoinsConf.HarmonyOne.ParamByKey("addr_hrp"),
                                                   addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            return EthAddrDecoder.DecodeAddr(
-                CoinsConf.Ethereum.ParamByKey("addr_prefix") + BytesUtils.ToHexString(addr_dec_bytes),
-                skip_chksum_enc=True
-            )
+
+        return EthAddrDecoder.DecodeAddr(
+            CoinsConf.Ethereum.ParamByKey("addr_prefix") + BytesUtils.ToHexString(addr_dec_bytes),
+            skip_chksum_enc=True
+        )
 
 
 class OneAddrEncoder(IAddrEncoder):
     """
     Harmony One address encoder class.
     It allows the Harmony One address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/sol_addr.py` & `bip_utils-2.7.1/bip_utils/addr/sol_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/substrate_addr.py` & `bip_utils-2.7.1/bip_utils/addr/substrate_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/trx_addr.py` & `bip_utils-2.7.1/bip_utils/addr/trx_addr.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,25 +57,26 @@
         """
 
         try:
             # Decode from base58
             addr_dec = Base58Decoder.CheckDecode(addr)
         except Base58ChecksumError as ex:
             raise ValueError("Invalid base58 checksum") from ex
-        else:
-            # Validate length
-            AddrDecUtils.ValidateLength(addr_dec,
-                                        (EthAddrConst.ADDR_LEN // 2) + len(CoinsConf.Tron.ParamByKey("addr_prefix")))
-            # Validate and remove prefix
-            addr_no_prefix = AddrDecUtils.ValidateAndRemovePrefix(addr_dec,
-                                                                  CoinsConf.Tron.ParamByKey("addr_prefix"))
 
-            return EthAddrDecoder.DecodeAddr(CoinsConf.Ethereum.ParamByKey("addr_prefix")
-                                             + BytesUtils.ToHexString(addr_no_prefix),
-                                             skip_chksum_enc=True)
+        # Validate length
+        AddrDecUtils.ValidateLength(addr_dec,
+                                    (EthAddrConst.ADDR_LEN // 2) + len(CoinsConf.Tron.ParamByKey("addr_prefix")))
+        # Validate and remove prefix
+        addr_no_prefix = AddrDecUtils.ValidateAndRemovePrefix(addr_dec,
+                                                              CoinsConf.Tron.ParamByKey("addr_prefix"))
+
+        return EthAddrDecoder.DecodeAddr(
+            CoinsConf.Ethereum.ParamByKey("addr_prefix") + BytesUtils.ToHexString(addr_no_prefix),
+            skip_chksum_enc=True
+        )
 
 
 class TrxAddrEncoder(IAddrEncoder):
     """
     Tron address encoder class.
     It allows the Tron address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/xlm_addr.py` & `bip_utils-2.7.1/bip_utils/addr/xlm_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/xmr_addr.py` & `bip_utils-2.7.1/bip_utils/addr/xmr_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/xrp_addr.py` & `bip_utils-2.7.1/bip_utils/addr/xrp_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/addr/xtz_addr.py` & `bip_utils-2.7.1/bip_utils/addr/xtz_addr.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,22 +74,22 @@
             raise TypeError("Address type is not an enumerative of XtzAddrPrefixes")
 
         # Decode from base58
         try:
             addr_dec_bytes = Base58Decoder.CheckDecode(addr)
         except Base58ChecksumError as ex:
             raise ValueError("Invalid base58 checksum") from ex
-        else:
-            # Validate length
-            AddrDecUtils.ValidateLength(addr_dec_bytes,
-                                        len(prefix.value) + Blake2b160.DigestSize())
-            # Validate and remove prefix
-            blake_bytes = AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, prefix.value)
 
-            return blake_bytes
+        # Validate length
+        AddrDecUtils.ValidateLength(addr_dec_bytes,
+                                    len(prefix.value) + Blake2b160.DigestSize())
+        # Validate and remove prefix
+        blake_bytes = AddrDecUtils.ValidateAndRemovePrefix(addr_dec_bytes, prefix.value)
+
+        return blake_bytes
 
 
 class XtzAddrEncoder(IAddrEncoder):
     """
     Tezos address encoder class.
     It allows the Tezos address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/addr/zil_addr.py` & `bip_utils-2.7.1/bip_utils/addr/zil_addr.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,17 +63,17 @@
             ValueError: If the address encoding is not valid
         """
         try:
             addr_dec_bytes = Bech32Decoder.Decode(CoinsConf.Zilliqa.ParamByKey("addr_hrp"),
                                                   addr)
         except Bech32ChecksumError as ex:
             raise ValueError("Invalid bech32 checksum") from ex
-        else:
-            AddrDecUtils.ValidateLength(addr_dec_bytes, ZilAddrConst.SHA256_BYTE_LEN)
-            return addr_dec_bytes
+
+        AddrDecUtils.ValidateLength(addr_dec_bytes, ZilAddrConst.SHA256_BYTE_LEN)
+        return addr_dec_bytes
 
 
 class ZilAddrEncoder(IAddrEncoder):
     """
     Zilliqa address encoder class.
     It allows the Zilliqa address encoding.
     """
```

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/__init__.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_entropy_generator.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/algorand/mnemonic/algorand_seed_generator.py` & `bip_utils-2.7.1/bip_utils/algorand/mnemonic/algorand_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/base58/base58.py` & `bip_utils-2.7.1/bip_utils/base58/base58.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/base58/base58_ex.py` & `bip_utils-2.7.1/bip_utils/base58/base58_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/base58/base58_xmr.py` & `bip_utils-2.7.1/bip_utils/base58/base58_xmr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bech32/bch_bech32.py` & `bip_utils-2.7.1/bip_utils/bech32/bch_bech32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bech32/bech32.py` & `bip_utils-2.7.1/bip_utils/bech32/bech32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bech32/bech32_base.py` & `bip_utils-2.7.1/bip_utils/bech32/bech32_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bech32/bech32_ex.py` & `bip_utils-2.7.1/bip_utils/bech32/bech32_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bech32/segwit_bech32.py` & `bip_utils-2.7.1/bip_utils/bech32/segwit_bech32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/__init__.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/base/bip32_base.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/base/bip32_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/base/ibip32_key_derivator.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/base/ibip32_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/base/ibip32_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_const.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_ex.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_key_data.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_key_data.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_key_net_ver.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_key_net_ver.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_key_ser.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_key_ser.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_keys.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_path.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_path.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/bip32_utils.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/bip32_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_ed25519_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_key_derivator_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/kholaw/bip32_kholaw_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/slip10/__init__.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/slip10/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_ed25519_blake2b.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_nist256p1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py` & `bip_utils-2.7.1/bip_utils/bip/bip32/slip10/bip32_slip10_secp256k1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip38/bip38.py` & `bip_utils-2.7.1/bip_utils/bip/bip38/bip38.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip38/bip38_addr.py` & `bip_utils-2.7.1/bip_utils/bip/bip38/bip38_addr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip38/bip38_ec.py` & `bip_utils-2.7.1/bip_utils/bip/bip38/bip38_ec.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         """
 
         # Get if lot and sequence are used
         has_lot_seq = lot_num is not None and sequence_num is not None
 
         # Compute owner entropy and salt
         # We can ignore the mypy warning because has_lot_seq checks for variables for being not None
-        owner_entropy = (_Bip38EcUtils.OwnerEntropyWithLotSeq(lot_num, sequence_num)    # type: ignore
+        owner_entropy = (_Bip38EcUtils.OwnerEntropyWithLotSeq(lot_num, sequence_num)    # type: ignore [arg-type]
                          if has_lot_seq
                          else _Bip38EcUtils.OwnerEntropyNoLotSeq())
         # Compute passpoint
         passfactor = _Bip38EcUtils.PassFactor(passphrase, owner_entropy, has_lot_seq)
         passpoint = _Bip38EcUtils.PassPoint(passfactor)
 
         # Get magic
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip38/bip38_no_ec.py` & `bip_utils-2.7.1/bip_utils/bip/bip38/bip38_no_ec.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/__init__.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_entropy_generator.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_decoder.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_encoder.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_generator.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_utils.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_mnemonic_validator.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/bip39_seed_generator.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/bip39_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/ibip39_seed_generator.py` & `bip_utils-2.7.1/bip_utils/bip/bip39/ibip39_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/chinese_simplified.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/chinese_traditional.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/chinese_traditional.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/czech.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/czech.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/english.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/french.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/italian.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/korean.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/korean.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/portuguese.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/portuguese.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip39/wordlist/spanish.txt` & `bip_utils-2.7.1/bip_utils/bip/bip39/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip44/bip44.py` & `bip_utils-2.7.1/bip_utils/bip/bip44/bip44.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip44_base/bip44_base.py` & `bip_utils-2.7.1/bip_utils/bip/bip44_base/bip44_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip44_base/bip44_base_ex.py` & `bip_utils-2.7.1/bip_utils/bip/bip44_base/bip44_base_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip44_base/bip44_keys.py` & `bip_utils-2.7.1/bip_utils/bip/bip44_base/bip44_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip49/bip49.py` & `bip_utils-2.7.1/bip_utils/bip/bip49/bip49.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip84/bip84.py` & `bip_utils-2.7.1/bip_utils/bip/bip84/bip84.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/bip86/bip86.py` & `bip_utils-2.7.1/bip_utils/bip/bip86/bip86.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip44/bip44_coins.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip44/bip44_coins.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 @unique
 class Bip44Coins(BipCoins):
     """Enumerative for supported BIP44 coins."""
 
     # Main nets
     AKASH_NETWORK = auto()
     ALGORAND = auto()
+    APTOS = auto()
     AVAX_C_CHAIN = auto()
     AVAX_P_CHAIN = auto()
     AVAX_X_CHAIN = auto()
     AXELAR = auto()
     BAND_PROTOCOL = auto()
     BINANCE_CHAIN = auto()
     BINANCE_SMART_CHAIN = auto()
@@ -76,14 +77,15 @@
     NEO = auto()
     NINE_CHRONICLES_GOLD = auto()
     OKEX_CHAIN_ATOM = auto()
     OKEX_CHAIN_ATOM_OLD = auto()
     OKEX_CHAIN_ETH = auto()
     ONTOLOGY = auto()
     OSMOSIS = auto()
+    PI_NETWORK = auto()
     POLKADOT_ED25519_SLIP = auto()
     POLYGON = auto()
     RIPPLE = auto()
     SECRET_NETWORK_OLD = auto()
     SECRET_NETWORK_NEW = auto()
     SOLANA = auto()
     STELLAR = auto()
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip44/bip44_conf.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip44/bip44_conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,26 +18,27 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 """Module for BIP44 coins configuration."""
 
 # Imports
 from bip_utils.addr import (
-    AdaByronIcarusAddrEncoder, AlgoAddrEncoder, AtomAddrEncoder, AvaxPChainAddrEncoder, AvaxXChainAddrEncoder,
-    BchP2PKHAddrEncoder, EgldAddrEncoder, EosAddrEncoder, ErgoNetworkTypes, ErgoP2PKHAddrEncoder, EthAddrEncoder,
-    FilSecp256k1AddrEncoder, IcxAddrEncoder, NanoAddrEncoder, NearAddrEncoder, NeoAddrEncoder, OkexAddrEncoder,
-    OneAddrEncoder, P2PKHAddrEncoder, SolAddrEncoder, SubstrateEd25519AddrEncoder, TrxAddrEncoder, XlmAddrEncoder,
-    XlmAddrTypes, XmrAddrEncoder, XrpAddrEncoder, XtzAddrEncoder, XtzAddrPrefixes, ZilAddrEncoder
+    AdaByronIcarusAddrEncoder, AlgoAddrEncoder, AptosAddrEncoder, AtomAddrEncoder, AvaxPChainAddrEncoder,
+    AvaxXChainAddrEncoder, BchP2PKHAddrEncoder, EgldAddrEncoder, EosAddrEncoder, ErgoNetworkTypes, ErgoP2PKHAddrEncoder,
+    EthAddrEncoder, FilSecp256k1AddrEncoder, IcxAddrEncoder, NanoAddrEncoder, NearAddrEncoder, NeoAddrEncoder,
+    OkexAddrEncoder, OneAddrEncoder, P2PKHAddrEncoder, SolAddrEncoder, SubstrateEd25519AddrEncoder, TrxAddrEncoder,
+    XlmAddrEncoder, XlmAddrTypes, XmrAddrEncoder, XrpAddrEncoder, XtzAddrEncoder, XtzAddrPrefixes, ZilAddrEncoder
 )
 from bip_utils.bip.bip32 import (
     Bip32Const, Bip32KeyNetVersions, Bip32KholawEd25519, Bip32Slip10Ed25519, Bip32Slip10Ed25519Blake2b,
     Bip32Slip10Nist256p1, Bip32Slip10Secp256k1
 )
 from bip_utils.bip.conf.common import (
-    HARDENED_DEF_PATH, NOT_HARDENED_DEF_PATH, BipBitcoinCashConf, BipCoinConf, BipCoinFctCallsConf, BipLitecoinConf
+    DER_PATH_HARDENED_FULL, DER_PATH_HARDENED_SHORT, DER_PATH_NON_HARDENED_FULL, BipBitcoinCashConf, BipCoinConf,
+    BipCoinFctCallsConf, BipLitecoinConf
 )
 from bip_utils.cardano.bip32.cardano_icarus_bip32 import CardanoIcarusBip32
 from bip_utils.coin_conf import CoinsConf
 from bip_utils.slip.slip44 import Slip44
 
 
 # Bitcoin key net version for main net (same as BIP32)
@@ -50,166 +51,179 @@
     """Class container for BIP44 configuration."""
 
     # Configuration for Akash Network
     AkashNetwork: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.AkashNetwork.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.AkashNetwork.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Algorand
     Algorand: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Algorand.CoinNames(),
         coin_idx=Slip44.ALGORAND,
         is_testnet=False,
-        def_path=HARDENED_DEF_PATH,
+        def_path=DER_PATH_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=AlgoAddrEncoder,
         addr_params={},
     )
 
+    # Configuration for Aptos
+    Aptos: BipCoinConf = BipCoinConf(
+        coin_names=CoinsConf.Aptos.CoinNames(),
+        coin_idx=Slip44.APTOS,
+        is_testnet=False,
+        def_path=DER_PATH_HARDENED_FULL,
+        key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
+        wif_net_ver=None,
+        bip32_cls=Bip32Slip10Ed25519,
+        addr_cls=AptosAddrEncoder,
+        addr_params={},
+    )
+
     # Configuration for Avax C-Chain
     AvaxCChain: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.AvaxCChain.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
     # Configuration for Avax P-Chain
     AvaxPChain: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.AvaxPChain.CoinNames(),
         coin_idx=Slip44.AVALANCHE,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AvaxPChainAddrEncoder,
         addr_params={},
     )
     # Configuration for Avax X-Chain
     AvaxXChain: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.AvaxXChain.CoinNames(),
         coin_idx=Slip44.AVALANCHE,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AvaxXChainAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Axelar
     Axelar: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Axelar.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.Axelar.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Band Protocol
     BandProtocol: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BandProtocol.CoinNames(),
         coin_idx=Slip44.BAND_PROTOCOL,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BandProtocol.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Binance Chain
     BinanceChain: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BinanceChain.CoinNames(),
         coin_idx=Slip44.BINANCE_CHAIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BinanceChain.ParamByKey("addr_hrp"),
         },
     )
     # Configuration for Binance Smart Chain
     BinanceSmartChain: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BinanceSmartChain.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Bitcoin main net
     BitcoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinMainNet.ParamByKey("p2pkh_net_ver"),
         },
     )
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinTestNet.ParamByKey("p2pkh_net_ver"),
         },
     )
 
     # Configuration for Bitcoin Cash main net
     BitcoinCashMainNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_CASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinCashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2PKHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashMainNet.ParamByKey("p2pkh_std_net_ver"),
@@ -222,15 +236,15 @@
         addr_cls_legacy=P2PKHAddrEncoder,
     )
     # Configuration for Bitcoin Cash test net
     BitcoinCashTestNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinCashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2PKHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashTestNet.ParamByKey("p2pkh_std_net_ver"),
@@ -244,15 +258,15 @@
     )
 
     # Configuration for Bitcoin Cash Simple Ledger Protocol main net
     BitcoinCashSlpMainNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashSlpMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_CASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinCashSlpMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2PKHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashSlpMainNet.ParamByKey("p2pkh_std_net_ver"),
@@ -265,15 +279,15 @@
         addr_cls_legacy=P2PKHAddrEncoder,
     )
     # Configuration for Bitcoin Cash Simple Ledger Protocol test net
     BitcoinCashSlpTestNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashSlpTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinCashSlpTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2PKHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashSlpTestNet.ParamByKey("p2pkh_std_net_ver"),
@@ -287,175 +301,175 @@
     )
 
     # Configuration for BitcoinSV main net
     BitcoinSvMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinSvMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_SV,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinSvMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinSvMainNet.ParamByKey("p2pkh_net_ver"),
         },
     )
     # Configuration for BitcoinSV test net
     BitcoinSvTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinSvTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinSvTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinSvTestNet.ParamByKey("p2pkh_net_ver"),
         },
     )
 
     # Configuration for Cardano Byron (Icarus)
     CardanoByronIcarus: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.CardanoMainNet.CoinNames(),
         coin_idx=Slip44.CARDANO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32Const.KHOLAW_KEY_NET_VERSIONS,
         wif_net_ver=None,
         bip32_cls=CardanoIcarusBip32,
         addr_cls=AdaByronIcarusAddrEncoder,
         addr_params={
             "chain_code": BipCoinFctCallsConf("ChainCode"),
         },
     )
     # Configuration for Cardano Byron (Ledger)
     CardanoByronLedger: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.CardanoMainNet.CoinNames(),
         coin_idx=Slip44.CARDANO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32Const.KHOLAW_KEY_NET_VERSIONS,
         wif_net_ver=None,
         bip32_cls=Bip32KholawEd25519,
         addr_cls=AdaByronIcarusAddrEncoder,
         addr_params={
             "chain_code": BipCoinFctCallsConf("ChainCode"),
         },
     )
 
     # Configuration for Celo
     Celo: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Celo.CoinNames(),
         coin_idx=Slip44.CELO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Certik
     Certik: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Certik.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.Certik.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Chihuahua
     Chihuahua: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Chihuahua.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.Chihuahua.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Cosmos
     Cosmos: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Cosmos.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.Cosmos.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Dash main net
     DashMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DashMainNet.CoinNames(),
         coin_idx=Slip44.DASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.DashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DashMainNet.ParamByKey("p2pkh_net_ver"),
         },
     )
     # Configuration for Dash test net
     DashTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.DashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DashTestNet.ParamByKey("p2pkh_net_ver"),
         },
     )
 
     # Configuration for Dogecoin main net
     DogecoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DogecoinMainNet.CoinNames(),
         coin_idx=Slip44.DOGECOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x02\xfa\xca\xfd",
                                         b"\x02\xfa\xc3\x98"),   # dgub / dgpv
         wif_net_ver=CoinsConf.DogecoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DogecoinMainNet.ParamByKey("p2pkh_net_ver"),
         },
     )
     # Configuration for Dogecoin test net
     DogecoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DogecoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x04\x32\xa9\xa8",
                                         b"\x04\x32\xa2\x43"),   # tgub / tgpv
         wif_net_ver=CoinsConf.DogecoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DogecoinTestNet.ParamByKey("p2pkh_net_ver"),
@@ -463,15 +477,15 @@
     )
 
     # Configuration for eCash main net
     EcashMainNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.EcashMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_CASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.EcashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2PKHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.EcashMainNet.ParamByKey("p2pkh_std_net_ver"),
@@ -484,15 +498,15 @@
         addr_cls_legacy=P2PKHAddrEncoder,
     )
     # Configuration for eCash test net
     EcashTestNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.EcashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.EcashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2PKHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.EcashTestNet.ParamByKey("p2pkh_std_net_ver"),
@@ -506,230 +520,230 @@
     )
 
     # Configuration for Elrond
     Elrond: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Elrond.CoinNames(),
         coin_idx=Slip44.ELROND,
         is_testnet=False,
-        def_path=HARDENED_DEF_PATH,
+        def_path=DER_PATH_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=EgldAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Eos
     Eos: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Eos.CoinNames(),
         coin_idx=Slip44.EOS,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EosAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Ergo main net
     ErgoMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.ErgoMainNet.CoinNames(),
         coin_idx=Slip44.ERGO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=ErgoP2PKHAddrEncoder,
         addr_params={
             "net_type": ErgoNetworkTypes.MAINNET,
         },
     )
 
     # Configuration for Ergo test net
     ErgoTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.ErgoTestNet.CoinNames(),
         coin_idx=Slip44.ERGO,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=ErgoP2PKHAddrEncoder,
         addr_params={
             "net_type": ErgoNetworkTypes.TESTNET,
         },
     )
 
     # Configuration for Ethereum
     Ethereum: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Ethereum.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
     # Configuration for Ethereum Classic
     EthereumClassic: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.EthereumClassic.CoinNames(),
         coin_idx=Slip44.ETHEREUM_CLASSIC,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Fantom Opera
     FantomOpera: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.FantomOpera.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Filecoin
     Filecoin: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Filecoin.CoinNames(),
         coin_idx=Slip44.FILECOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=FilSecp256k1AddrEncoder,
         addr_params={},
     )
 
     # Configuration for Harmony One (Metamask address)
     HarmonyOneMetamask: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.HarmonyOne.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
     # Configuration for Harmony One (Ethereum address)
     HarmonyOneEth: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.HarmonyOne.CoinNames(),
         coin_idx=Slip44.HARMONY_ONE,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
     # Configuration for Harmony One (Atom address)
     HarmonyOneAtom: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.HarmonyOne.CoinNames(),
         coin_idx=Slip44.HARMONY_ONE,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=OneAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Huobi Chain
     HuobiChain: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.HuobiChain.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Icon
     Icon: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Icon.CoinNames(),
         coin_idx=Slip44.ICON,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=IcxAddrEncoder,
         addr_params={},
     )
 
     # Configuration for IRISnet
     IrisNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.IrisNet.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.IrisNet.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Kava
     Kava: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Kava.CoinNames(),
         coin_idx=Slip44.KAVA,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.Kava.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Kusama (ed25519 SLIP-0010)
     KusamaEd25519Slip: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Kusama.CoinNames(),
         coin_idx=Slip44.KUSAMA,
         is_testnet=False,
-        def_path=HARDENED_DEF_PATH,
+        def_path=DER_PATH_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=SubstrateEd25519AddrEncoder,
         addr_params={
             "ss58_format": CoinsConf.Kusama.ParamByKey("addr_ss58_format"),
         },
     )
 
     # Configuration for Litecoin main net
     LitecoinMainNet: BipLitecoinConf = BipLitecoinConf(
         coin_names=CoinsConf.LitecoinMainNet.CoinNames(),
         coin_idx=Slip44.LITECOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         alt_key_net_ver=Bip32KeyNetVersions(b"\x01\x9d\xa4\x62",
                                             b"\x01\x9d\x9c\xfe"),   # Ltpv / Ltub
         wif_net_ver=CoinsConf.LitecoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
@@ -738,15 +752,15 @@
         },
     )
     # Configuration for Litecoin test net
     LitecoinTestNet: BipLitecoinConf = BipLitecoinConf(
         coin_names=CoinsConf.LitecoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x04\x36\xf6\xe1",
                                         b"\x04\x36\xef\x7d"),       # ttub / ttpv
         alt_key_net_ver=Bip32KeyNetVersions(b"\x04\x36\xf6\xe1",
                                             b"\x04\x36\xef\x7d"),   # ttub / ttpv
         wif_net_ver=CoinsConf.LitecoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
@@ -757,260 +771,273 @@
     )
 
     # Configuration for Monero (ed25519 SLIP-0010)
     MoneroEd25519Slip: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.MoneroMainNet.CoinNames(),
         coin_idx=Slip44.MONERO,
         is_testnet=False,
-        def_path=HARDENED_DEF_PATH,
+        def_path=DER_PATH_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=XmrAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Monero (secp256k1)
     MoneroSecp256k1: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.MoneroMainNet.CoinNames(),
         coin_idx=Slip44.MONERO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=XmrAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Nano
     Nano: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Nano.CoinNames(),
         coin_idx=Slip44.NANO,
         is_testnet=False,
-        def_path="0'",
+        def_path=DER_PATH_HARDENED_SHORT,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519Blake2b,
         addr_cls=NanoAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Near Protocol
     NearProtocol: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.NearProtocol.CoinNames(),
         coin_idx=Slip44.NEAR_PROTOCOL,
         is_testnet=False,
-        def_path="0'",
+        def_path=DER_PATH_HARDENED_SHORT,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=NearAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Neo
     Neo: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Neo.CoinNames(),
         coin_idx=Slip44.NEO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Nist256p1,
         addr_cls=NeoAddrEncoder,
         addr_params={
             "ver": CoinsConf.Neo.ParamByKey("addr_ver"),
         },
     )
 
     # Configuration for NG
     NineChroniclesGold: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.NineChroniclesGold.CoinNames(),
         coin_idx=Slip44.NINE_CHRONICLES,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for OKEx Chain (Ethereum address)
     OkexChainEth: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.OkexChain.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for OKEx Chain (Atom address)
     OkexChainAtom: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.OkexChain.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=OkexAddrEncoder,
         addr_params={},
     )
 
     # Configuration for OKEx Chain (old Atom address)
     OkexChainAtomOld: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.OkexChain.CoinNames(),
         coin_idx=Slip44.OKEX_CHAIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=OkexAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Ontology
     Ontology: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Ontology.CoinNames(),
         coin_idx=Slip44.ONTOLOGY,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Nist256p1,
         addr_cls=NeoAddrEncoder,
         addr_params={
             "ver": CoinsConf.Ontology.ParamByKey("addr_ver"),
         },
     )
 
     # Configuration for Osmosis
     Osmosis: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Osmosis.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.Osmosis.ParamByKey("addr_hrp"),
         },
     )
 
+    # Configuration for Pi Network
+    PiNetwork: BipCoinConf = BipCoinConf(
+        coin_names=CoinsConf.PiNetwork.CoinNames(),
+        coin_idx=Slip44.PI_NETWORK,
+        is_testnet=False,
+        def_path=DER_PATH_HARDENED_SHORT,
+        key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
+        wif_net_ver=None,
+        bip32_cls=Bip32Slip10Ed25519,
+        addr_cls=XlmAddrEncoder,
+        addr_params={"addr_type": XlmAddrTypes.PUB_KEY},
+    )
+
     # Configuration for Polkadot (ed25519 SLIP-0010)
     PolkadotEd25519Slip: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Polkadot.CoinNames(),
         coin_idx=Slip44.POLKADOT,
         is_testnet=False,
-        def_path=HARDENED_DEF_PATH,
+        def_path=DER_PATH_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=SubstrateEd25519AddrEncoder,
         addr_params={
             "ss58_format": CoinsConf.Polkadot.ParamByKey("addr_ss58_format"),
         },
     )
 
     # Configuration for Polygon
     Polygon: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Polygon.CoinNames(),
         coin_idx=Slip44.ETHEREUM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Ripple
     Ripple: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Ripple.CoinNames(),
         coin_idx=Slip44.RIPPLE,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=XrpAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Secret Network (old path)
     SecretNetworkOld: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.SecretNetwork.CoinNames(),
         coin_idx=Slip44.ATOM,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.SecretNetwork.ParamByKey("addr_hrp"),
         },
     )
     # Configuration for Secret Network (new path)
     SecretNetworkNew: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.SecretNetwork.CoinNames(),
         coin_idx=Slip44.SECRET_NETWORK,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.SecretNetwork.ParamByKey("addr_hrp"),
         },
     )
 
     # Configuration for Solana
     Solana: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Solana.CoinNames(),
         coin_idx=Slip44.SOLANA,
         is_testnet=False,
-        def_path="0'",
+        def_path=DER_PATH_HARDENED_SHORT,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=SolAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Stellar
     Stellar: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Stellar.CoinNames(),
         coin_idx=Slip44.STELLAR,
         is_testnet=False,
-        def_path="0'",
+        def_path=DER_PATH_HARDENED_SHORT,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Ed25519,
         addr_cls=XlmAddrEncoder,
         addr_params={"addr_type": XlmAddrTypes.PUB_KEY},
     )
 
     # Configuration for Terra
     Terra: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Terra.CoinNames(),
         coin_idx=Slip44.TERRA,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=AtomAddrEncoder,
         addr_params={
             "hrp": CoinsConf.Terra.ParamByKey("addr_hrp"),
         },
@@ -1030,97 +1057,97 @@
     )
 
     # Configuration for Theta
     Theta: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Theta.CoinNames(),
         coin_idx=Slip44.THETA,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Tron
     Tron: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Tron.CoinNames(),
         coin_idx=Slip44.TRON,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=TrxAddrEncoder,
         addr_params={},
     )
 
     # Configuration for VeChain
     VeChain: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.VeChain.CoinNames(),
         coin_idx=Slip44.VECHAIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=EthAddrEncoder,
         addr_params={},
     )
 
     # Configuration for Verge
     Verge: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Verge.CoinNames(),
         coin_idx=Slip44.VERGE,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.Verge.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.Verge.ParamByKey("p2pkh_net_ver"),
         },
     )
 
     # Configuration for Zcash main net
     ZcashMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.ZcashMainNet.CoinNames(),
         coin_idx=Slip44.ZCASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.ZcashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.ZcashMainNet.ParamByKey("p2pkh_net_ver"),
         },
     )
     # Configuration for Zcash test net
     ZcashTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.ZcashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.ZcashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2PKHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.ZcashTestNet.ParamByKey("p2pkh_net_ver"),
         },
     )
 
     # Configuration for Zilliqa
     Zilliqa: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.Zilliqa.CoinNames(),
         coin_idx=Slip44.ZILLIQA,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP44_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=None,
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=ZilAddrEncoder,
         addr_params={},
     )
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip44/bip44_conf_getter.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip44/bip44_conf_getter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 class Bip44ConfGetterConst:
     """Class container for BIP44 configuration getter constants."""
 
     # Map from Bip44Coins to configuration classes
     COIN_TO_CONF: Dict[BipCoins, BipCoinConf] = {
         Bip44Coins.AKASH_NETWORK: Bip44Conf.AkashNetwork,
         Bip44Coins.ALGORAND: Bip44Conf.Algorand,
+        Bip44Coins.APTOS: Bip44Conf.Aptos,
         Bip44Coins.AVAX_C_CHAIN: Bip44Conf.AvaxCChain,
         Bip44Coins.AVAX_P_CHAIN: Bip44Conf.AvaxPChain,
         Bip44Coins.AVAX_X_CHAIN: Bip44Conf.AvaxXChain,
         Bip44Coins.AXELAR: Bip44Conf.Axelar,
         Bip44Coins.BAND_PROTOCOL: Bip44Conf.BandProtocol,
         Bip44Coins.BINANCE_CHAIN: Bip44Conf.BinanceChain,
         Bip44Coins.BINANCE_SMART_CHAIN: Bip44Conf.BinanceSmartChain,
@@ -87,14 +88,15 @@
         Bip44Coins.NEO: Bip44Conf.Neo,
         Bip44Coins.NINE_CHRONICLES_GOLD: Bip44Conf.NineChroniclesGold,
         Bip44Coins.OKEX_CHAIN_ATOM: Bip44Conf.OkexChainAtom,
         Bip44Coins.OKEX_CHAIN_ATOM_OLD: Bip44Conf.OkexChainAtomOld,
         Bip44Coins.OKEX_CHAIN_ETH: Bip44Conf.OkexChainEth,
         Bip44Coins.ONTOLOGY: Bip44Conf.Ontology,
         Bip44Coins.OSMOSIS: Bip44Conf.Osmosis,
+        Bip44Coins.PI_NETWORK: Bip44Conf.PiNetwork,
         Bip44Coins.POLKADOT_ED25519_SLIP: Bip44Conf.PolkadotEd25519Slip,
         Bip44Coins.POLYGON: Bip44Conf.Polygon,
         Bip44Coins.RIPPLE: Bip44Conf.Ripple,
         Bip44Coins.SECRET_NETWORK_OLD: Bip44Conf.SecretNetworkOld,
         Bip44Coins.SECRET_NETWORK_NEW: Bip44Conf.SecretNetworkNew,
         Bip44Coins.SOLANA: Bip44Conf.Solana,
         Bip44Coins.STELLAR: Bip44Conf.Stellar,
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip49/bip49_coins.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip49/bip49_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip49/bip49_conf.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip49/bip49_conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # THE SOFTWARE.
 
 """Module for BIP49 coins configuration."""
 
 # Imports
 from bip_utils.addr import BchP2SHAddrEncoder, P2SHAddrEncoder
 from bip_utils.bip.bip32 import Bip32KeyNetVersions, Bip32Slip10Secp256k1
-from bip_utils.bip.conf.common import NOT_HARDENED_DEF_PATH, BipBitcoinCashConf, BipCoinConf, BipLitecoinConf
+from bip_utils.bip.conf.common import DER_PATH_NON_HARDENED_FULL, BipBitcoinCashConf, BipCoinConf, BipLitecoinConf
 from bip_utils.coin_conf import CoinsConf
 from bip_utils.slip.slip44 import Slip44
 
 
 # Bitcoin key net version for main net (ypub / yprv)
 _BIP49_BTC_KEY_NET_VER_MAIN: Bip32KeyNetVersions = Bip32KeyNetVersions(b"\x04\x9d\x7c\xb2",
                                                                        b"\x04\x9d\x78\x78")
@@ -40,44 +40,44 @@
     """Class container for BIP49 configuration."""
 
     # Configuration for Bitcoin main net
     BitcoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinMainNet.ParamByKey("p2sh_net_ver"),
         },
     )
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinTestNet.ParamByKey("p2sh_net_ver"),
         },
     )
 
     # Configuration for Bitcoin Cash main net
     BitcoinCashMainNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_CASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinCashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2SHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashMainNet.ParamByKey("p2sh_std_net_ver"),
@@ -90,15 +90,15 @@
         addr_cls_legacy=P2SHAddrEncoder,
     )
     # Configuration for Bitcoin Cash test net
     BitcoinCashTestNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinCashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2SHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashTestNet.ParamByKey("p2sh_std_net_ver"),
@@ -112,15 +112,15 @@
     )
 
     # Configuration for Bitcoin Cash Simple Ledger Protocol main net
     BitcoinCashSlpMainNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashSlpMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_CASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinCashSlpMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2SHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashSlpMainNet.ParamByKey("p2sh_std_net_ver"),
@@ -133,15 +133,15 @@
         addr_cls_legacy=P2SHAddrEncoder,
     )
     # Configuration for Bitcoin Cash Simple Ledger Protocol test net
     BitcoinCashSlpTestNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.BitcoinCashSlpTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinCashSlpTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2SHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.BitcoinCashSlpTestNet.ParamByKey("p2sh_std_net_ver"),
@@ -155,88 +155,88 @@
     )
 
     # Configuration for BitcoinSV main net
     BitcoinSvMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinSvMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_SV,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.BitcoinSvMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinSvMainNet.ParamByKey("p2sh_net_ver"),
         },
     )
     # Configuration for BitcoinSV test net
     BitcoinSvTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinSvTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinSvTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.BitcoinSvTestNet.ParamByKey("p2sh_net_ver"),
         },
     )
 
     # Configuration for Dash main net
     DashMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DashMainNet.CoinNames(),
         coin_idx=Slip44.DASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.DashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DashMainNet.ParamByKey("p2sh_net_ver"),
         },
     )
     # Configuration for Dash test net
     DashTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.DashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DashTestNet.ParamByKey("p2sh_net_ver"),
         },
     )
 
     # Configuration for Dogecoin main net
     DogecoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DogecoinMainNet.CoinNames(),
         coin_idx=Slip44.DOGECOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x02\xfa\xca\xfd",
                                         b"\x02\xfa\xc3\x98"),   # dgub / dgpv
         wif_net_ver=CoinsConf.DogecoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DogecoinMainNet.ParamByKey("p2sh_net_ver"),
         },
     )
     # Configuration for Dogecoin test net
     DogecoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.DogecoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x04\x32\xa9\xa8",
                                         b"\x04\x32\xa2\x43"),   # tgub / tgpv
         wif_net_ver=CoinsConf.DogecoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.DogecoinTestNet.ParamByKey("p2sh_net_ver"),
@@ -244,15 +244,15 @@
     )
 
     # Configuration for eCash main net
     EcashMainNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.EcashMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN_CASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.EcashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2SHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.EcashMainNet.ParamByKey("p2sh_std_net_ver"),
@@ -265,15 +265,15 @@
         addr_cls_legacy=P2SHAddrEncoder,
     )
     # Configuration for eCash test net
     EcashTestNet: BipBitcoinCashConf = BipBitcoinCashConf(
         coin_names=CoinsConf.EcashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.EcashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=BchP2SHAddrEncoder,
         addr_params={
             "std": {
                 "net_ver": CoinsConf.EcashTestNet.ParamByKey("p2sh_std_net_ver"),
@@ -287,15 +287,15 @@
     )
 
     # Configuration for Litecoin main net
     LitecoinMainNet: BipLitecoinConf = BipLitecoinConf(
         coin_names=CoinsConf.LitecoinMainNet.CoinNames(),
         coin_idx=Slip44.LITECOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         alt_key_net_ver=Bip32KeyNetVersions(b"\x01\xb2\x6e\xf6",
                                             b"\x01\xb2\x67\x92"),   # Mtpv / Mtub
         wif_net_ver=CoinsConf.LitecoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
@@ -304,15 +304,15 @@
         },
     )
     # Configuration for Litecoin test net
     LitecoinTestNet: BipLitecoinConf = BipLitecoinConf(
         coin_names=CoinsConf.LitecoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x04\x36\xf6\xe1",
                                         b"\x04\x36\xef\x7d"),       # ttub / ttpv
         alt_key_net_ver=Bip32KeyNetVersions(b"\x04\x36\xf6\xe1",
                                             b"\x04\x36\xef\x7d"),   # ttub / ttpv
         wif_net_ver=CoinsConf.LitecoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
@@ -323,29 +323,29 @@
     )
 
     # Configuration for Zcash main net
     ZcashMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.ZcashMainNet.CoinNames(),
         coin_idx=Slip44.ZCASH,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_MAIN,
         wif_net_ver=CoinsConf.ZcashMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.ZcashMainNet.ParamByKey("p2sh_net_ver"),
         },
     )
     # Configuration for Zcash test net
     ZcashTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.ZcashTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP49_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.ZcashTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2SHAddrEncoder,
         addr_params={
             "net_ver": CoinsConf.ZcashTestNet.ParamByKey("p2sh_net_ver"),
         },
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip49/bip49_conf_getter.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip49/bip49_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip84/bip84_coins.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip84/bip84_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip84/bip84_conf.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip84/bip84_conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # THE SOFTWARE.
 
 """Module for BIP84 coins configuration."""
 
 # Imports
 from bip_utils.addr import P2WPKHAddrEncoder
 from bip_utils.bip.bip32 import Bip32KeyNetVersions, Bip32Slip10Secp256k1
-from bip_utils.bip.conf.common import NOT_HARDENED_DEF_PATH, BipCoinConf
+from bip_utils.bip.conf.common import DER_PATH_NON_HARDENED_FULL, BipCoinConf
 from bip_utils.coin_conf import CoinsConf
 from bip_utils.slip.slip44 import Slip44
 
 
 # Bitcoin key net version (zpub / zprv)
 _BIP84_BTC_KEY_NET_VER: Bip32KeyNetVersions = Bip32KeyNetVersions(b"\x04\xb2\x47\x46",
                                                                   b"\x04\xb2\x43\x0c")
@@ -37,29 +37,29 @@
     """Class container for BIP84 configuration."""
 
     # Configuration for Bitcoin main net
     BitcoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP84_BTC_KEY_NET_VER,
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2WPKHAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BitcoinMainNet.ParamByKey("p2wpkh_hrp"),
         },
     )
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x04\x5f\x1c\xf6",
                                         b"\x04\x5f\x18\xbc"),   # vpub / vprv
         wif_net_ver=CoinsConf.BitcoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2WPKHAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BitcoinTestNet.ParamByKey("p2wpkh_hrp"),
@@ -67,29 +67,29 @@
     )
 
     # Configuration for Litecoin main net
     LitecoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.LitecoinMainNet.CoinNames(),
         coin_idx=Slip44.LITECOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP84_BTC_KEY_NET_VER,
         wif_net_ver=CoinsConf.LitecoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2WPKHAddrEncoder,
         addr_params={
             "hrp": CoinsConf.LitecoinMainNet.ParamByKey("p2wpkh_hrp"),
         },
     )
     # Configuration for Litecoin test net
     LitecoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.LitecoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32KeyNetVersions(b"\x04\x36\xf6\xe1",
                                         b"\x04\x36\xef\x7d"),   # ttub / ttpv
         wif_net_ver=CoinsConf.LitecoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2WPKHAddrEncoder,
         addr_params={
             "hrp": CoinsConf.LitecoinTestNet.ParamByKey("p2wpkh_hrp"),
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip84/bip84_conf_getter.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip84/bip84_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip86/bip86_coins.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip86/bip86_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip86/bip86_conf.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip86/bip86_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # THE SOFTWARE.
 
 """Module for BIP86 coins configuration."""
 
 # Imports
 from bip_utils.addr import P2TRAddrEncoder
 from bip_utils.bip.bip32 import Bip32Const, Bip32KeyNetVersions, Bip32Slip10Secp256k1
-from bip_utils.bip.conf.common import NOT_HARDENED_DEF_PATH, BipCoinConf
+from bip_utils.bip.conf.common import DER_PATH_NON_HARDENED_FULL, BipCoinConf
 from bip_utils.coin_conf import CoinsConf
 from bip_utils.slip.slip44 import Slip44
 
 
 # Bitcoin key net version for main net (same as BIP32)
 _BIP86_BTC_KEY_NET_VER: Bip32KeyNetVersions = Bip32Const.MAIN_NET_KEY_NET_VERSIONS
 # Bitcoin key net version for test net (same as BIP32)
@@ -38,30 +38,30 @@
     """Class container for BIP86 configuration."""
 
     # Configuration for Bitcoin main net
     BitcoinMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinMainNet.CoinNames(),
         coin_idx=Slip44.BITCOIN,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP86_BTC_KEY_NET_VER,
         wif_net_ver=CoinsConf.BitcoinMainNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2TRAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BitcoinMainNet.ParamByKey("p2tr_hrp"),
         },
     )
 
     # Configuration for Bitcoin test net
     BitcoinTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.BitcoinTestNet.CoinNames(),
         coin_idx=Slip44.TESTNET,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=_BIP86_BTC_KEY_NET_VER_TEST,
         wif_net_ver=CoinsConf.BitcoinTestNet.ParamByKey("wif_net_ver"),
         bip32_cls=Bip32Slip10Secp256k1,
         addr_cls=P2TRAddrEncoder,
         addr_params={
             "hrp": CoinsConf.BitcoinTestNet.ParamByKey("p2tr_hrp"),
         },
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/bip86/bip86_conf_getter.py` & `bip_utils-2.7.1/bip_utils/bip/conf/bip86/bip86_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py` & `bip_utils-2.7.1/bip_utils/bip/conf/common/bip_bitcoin_cash_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/common/bip_coin_conf.py` & `bip_utils-2.7.1/bip_utils/bip/conf/common/bip_coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/common/bip_coins.py` & `bip_utils-2.7.1/bip_utils/bip/conf/common/bip_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/common/bip_conf_const.py` & `bip_utils-2.7.1/bip_utils/bip/conf/common/bip_conf_const.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,11 +16,13 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 """Module for generic BIP configuration constants."""
 
-# Hardened default path
-HARDENED_DEF_PATH: str = "0'/0'/0'"
-# Not hardened default path
-NOT_HARDENED_DEF_PATH: str = "0'/0/0"
+# Hardened default path (full)
+DER_PATH_HARDENED_FULL: str = "0'/0'/0'"
+# Hardened default path (short)
+DER_PATH_HARDENED_SHORT: str = "0'"
+# Non-hardened default path (full)
+DER_PATH_NON_HARDENED_FULL: str = "0'/0/0"
```

### Comparing `bip_utils-2.7.0/bip_utils/bip/conf/common/bip_litecoin_conf.py` & `bip_utils-2.7.1/bip_utils/bip/conf/common/bip_litecoin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py` & `bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_byron_legacy_bip32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py` & `bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_byron_legacy_key_derivator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py` & `bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_byron_legacy_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_icarus_bip32.py` & `bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_icarus_bip32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py` & `bip_utils-2.7.1/bip_utils/cardano/bip32/cardano_icarus_mst_key_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/byron/cardano_byron_legacy.py` & `bip_utils-2.7.1/bip_utils/cardano/byron/cardano_byron_legacy.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/cip1852/cip1852.py` & `bip_utils-2.7.1/bip_utils/cardano/cip1852/cip1852.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/cip1852_coins.py` & `bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/cip1852_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/cip1852_conf.py` & `bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/cip1852_conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,74 +19,74 @@
 # THE SOFTWARE.
 
 """Module for CIP-1852 coins configuration."""
 
 # Imports
 from bip_utils.addr import AdaShelleyAddrEncoder, AdaShelleyAddrNetworkTags
 from bip_utils.bip.bip32 import Bip32Const, Bip32KholawEd25519
-from bip_utils.bip.conf.common import NOT_HARDENED_DEF_PATH, BipCoinConf
+from bip_utils.bip.conf.common import DER_PATH_NON_HARDENED_FULL, BipCoinConf
 from bip_utils.cardano.bip32.cardano_icarus_bip32 import CardanoIcarusBip32
 from bip_utils.coin_conf import CoinsConf
 from bip_utils.slip.slip44 import Slip44
 
 
 class Cip1852Conf:
     """Class container for CIP-1852 configuration."""
 
     # Configuration for Cardano main net (Icarus)
     CardanoIcarusMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.CardanoMainNet.CoinNames(),
         coin_idx=Slip44.CARDANO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32Const.KHOLAW_KEY_NET_VERSIONS,
         wif_net_ver=None,
         bip32_cls=CardanoIcarusBip32,
         addr_cls=AdaShelleyAddrEncoder,
         addr_params={
             "net_tag": AdaShelleyAddrNetworkTags.MAINNET,
         },
     )
 
     # Configuration for Cardano test net (Icarus)
     CardanoIcarusTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.CardanoTestNet.CoinNames(),
         coin_idx=Slip44.CARDANO,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32Const.TEST_NET_KEY_NET_VERSIONS,
         wif_net_ver=None,
         bip32_cls=CardanoIcarusBip32,
         addr_cls=AdaShelleyAddrEncoder,
         addr_params={
             "net_tag": AdaShelleyAddrNetworkTags.TESTNET,
         },
     )
 
     # Configuration for Cardano main net (Ledger)
     CardanoLedgerMainNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.CardanoMainNet.CoinNames(),
         coin_idx=Slip44.CARDANO,
         is_testnet=False,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32Const.KHOLAW_KEY_NET_VERSIONS,
         wif_net_ver=None,
         bip32_cls=Bip32KholawEd25519,
         addr_cls=AdaShelleyAddrEncoder,
         addr_params={
             "net_tag": AdaShelleyAddrNetworkTags.MAINNET,
         },
     )
 
     # Configuration for Cardano test net (Ledger)
     CardanoLedgerTestNet: BipCoinConf = BipCoinConf(
         coin_names=CoinsConf.CardanoTestNet.CoinNames(),
         coin_idx=Slip44.CARDANO,
         is_testnet=True,
-        def_path=NOT_HARDENED_DEF_PATH,
+        def_path=DER_PATH_NON_HARDENED_FULL,
         key_net_ver=Bip32Const.TEST_NET_KEY_NET_VERSIONS,
         wif_net_ver=None,
         bip32_cls=Bip32KholawEd25519,
         addr_cls=AdaShelleyAddrEncoder,
         addr_params={
             "net_tag": AdaShelleyAddrNetworkTags.TESTNET,
         },
```

### Comparing `bip_utils-2.7.0/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py` & `bip_utils-2.7.1/bip_utils/cardano/cip1852/conf/cip1852_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py` & `bip_utils-2.7.1/bip_utils/cardano/mnemonic/cardano_byron_legacy_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py` & `bip_utils-2.7.1/bip_utils/cardano/mnemonic/cardano_icarus_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/shelley/cardano_shelley.py` & `bip_utils-2.7.1/bip_utils/cardano/shelley/cardano_shelley.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/cardano/shelley/cardano_shelley_keys.py` & `bip_utils-2.7.1/bip_utils/cardano/shelley/cardano_shelley_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/coin_conf/coin_conf.py` & `bip_utils-2.7.1/bip_utils/coin_conf/coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/coin_conf/coins_conf.py` & `bip_utils-2.7.1/bip_utils/coin_conf/coins_conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,22 @@
 
     # Configuration for Algorand
     Algorand: CoinConf = CoinConf(
         coin_name=CoinNames("Algorand", "ALGO"),
         params={},
     )
 
+    # Configuration for Aptos
+    Aptos: CoinConf = CoinConf(
+        coin_name=CoinNames("Aptos", "APTOS"),
+        params={
+            "addr_prefix": "0x",
+        },
+    )
+
     # Configuration for Avax C-Chain
     AvaxCChain: CoinConf = CoinConf(
         coin_name=CoinNames("Avax C-Chain", "AVAX"),
         params={},
     )
 
     # Configuration for Avax P-Chain
@@ -616,14 +624,20 @@
     Phala: CoinConf = CoinConf(
         coin_name=CoinNames("Phala Network", "PHA"),
         params={
             "addr_ss58_format": 30,
         },
     )
 
+    # Configuration for Pi Network
+    PiNetwork: CoinConf = CoinConf(
+        coin_name=CoinNames("Pi Network", "PI"),
+        params={},
+    )
+
     # Configuration for Plasm
     Plasm: CoinConf = CoinConf(
         coin_name=CoinNames("Plasm Network", "PLM"),
         params={
             "addr_ss58_format": 5,
         },
     )
```

### Comparing `bip_utils-2.7.0/bip_utils/ecc/__init__.py` & `bip_utils-2.7.1/bip_utils/ecc/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/common/dummy_point.py` & `bip_utils-2.7.1/bip_utils/ecc/common/dummy_point.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 from typing import Any
 
 from bip_utils.ecc.common.ipoint import IPoint
 from bip_utils.ecc.curve.elliptic_curve_types import EllipticCurveTypes
 from bip_utils.utils.misc import DataBytes
 
 
+class DummyPointConst:
+    """Class container for dummy point constants."""
+
+    # Point coordinate length in bytes
+    POINT_COORD_BYTE_LEN: int = 32
+
+
 class DummyPoint(IPoint):
     """Dummy point class."""
 
     m_x: int
     m_y: int
 
     @classmethod
@@ -87,14 +94,24 @@
         """
         Get the elliptic curve type.
 
         Returns:
            EllipticCurveTypes: Elliptic curve type
         """
 
+    @staticmethod
+    def CoordinateLength() -> int:
+        """
+        Get the coordinate length.
+
+        Returns:
+           int: Coordinate key length
+        """
+        return DummyPointConst.POINT_COORD_BYTE_LEN
+
     def UnderlyingObject(self) -> Any:
         """
         Get the underlying object.
 
         Returns:
            Any: Underlying object
         """
```

### Comparing `bip_utils-2.7.0/bip_utils/ecc/common/ikeys.py` & `bip_utils-2.7.1/bip_utils/ecc/common/ikeys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/common/ipoint.py` & `bip_utils-2.7.1/bip_utils/ecc/common/ipoint.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,24 @@
         """
         Get the elliptic curve type.
 
         Returns:
            EllipticCurveTypes: Elliptic curve type
         """
 
+    @staticmethod
+    @abstractmethod
+    def CoordinateLength() -> int:
+        """
+        Get the coordinate length.
+
+        Returns:
+           int: Coordinate key length
+        """
+
     @abstractmethod
     def UnderlyingObject(self) -> Any:
         """
         Get the underlying object.
 
         Returns:
            Any: Underlying object
```

### Comparing `bip_utils-2.7.0/bip_utils/ecc/conf.py` & `bip_utils-2.7.1/bip_utils/ecc/conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/curve/elliptic_curve.py` & `bip_utils-2.7.1/bip_utils/ecc/curve/elliptic_curve.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/curve/elliptic_curve_getter.py` & `bip_utils-2.7.1/bip_utils/ecc/curve/elliptic_curve_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/curve/elliptic_curve_types.py` & `bip_utils-2.7.1/bip_utils/ecc/curve/elliptic_curve_types.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ecdsa/ecdsa_keys.py` & `bip_utils-2.7.1/bip_utils/ecc/ecdsa/ecdsa_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_const.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_keys.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_point.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_point.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from bip_utils.ecc.ed25519.lib import ed25519_lib
 from bip_utils.utils.misc import DataBytes
 
 
 class Ed25519PointConst:
     """Class container for ed25519 point constants."""
 
-    # Point coordinte length in bytes
+    # Point coordinate length in bytes
     POINT_COORD_BYTE_LEN: int = 32
 
 
 class Ed25519Point(IPoint):
     """Ed25519 point class."""
 
     m_is_generator: bool
@@ -103,14 +103,24 @@
         Get the elliptic curve type.
 
         Returns:
            EllipticCurveTypes: Elliptic curve type
         """
         return EllipticCurveTypes.ED25519
 
+    @staticmethod
+    def CoordinateLength() -> int:
+        """
+        Get the coordinate length.
+
+        Returns:
+           int: Coordinate key length
+        """
+        return Ed25519PointConst.POINT_COORD_BYTE_LEN
+
     def UnderlyingObject(self) -> Any:
         """
         Get the underlying object.
 
         Returns:
            Any: Underlying object
         """
```

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519/ed25519_utils.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519/ed25519_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519/lib/ed25519_lib.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519/lib/ed25519_lib.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_blake2b/ed25519_blake2b_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_kholaw/ed25519_kholaw_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py` & `bip_utils-2.7.1/bip_utils/ecc/ed25519_monero/ed25519_monero_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1.py` & `bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1_const.py` & `bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1_keys.py` & `bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/nist256p1/nist256p1_point.py` & `bip_utils-2.7.1/bip_utils/ecc/nist256p1/nist256p1_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,24 @@
         Get the elliptic curve type.
 
         Returns:
            EllipticCurveTypes: Elliptic curve type
         """
         return EllipticCurveTypes.NIST256P1
 
+    @staticmethod
+    def CoordinateLength() -> int:
+        """
+        Get the coordinate length.
+
+        Returns:
+           int: Coordinate key length
+        """
+        return EcdsaKeysConst.POINT_COORD_BYTE_LEN
+
     def UnderlyingObject(self) -> Any:
         """
         Get the underlying object.
 
         Returns:
            Any: Underlying object
         """
```

### Comparing `bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1.py` & `bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_const.py` & `bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py` & `bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_keys_coincurve.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py` & `bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_keys_ecdsa.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py` & `bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_point_coincurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,24 @@
         Get the elliptic curve type.
 
         Returns:
            EllipticCurveTypes: Elliptic curve type
         """
         return EllipticCurveTypes.SECP256K1
 
+    @staticmethod
+    def CoordinateLength() -> int:
+        """
+        Get the coordinate length.
+
+        Returns:
+           int: Coordinate key length
+        """
+        return EcdsaKeysConst.POINT_COORD_BYTE_LEN
+
     def UnderlyingObject(self) -> Any:
         """
         Get the underlying object.
 
         Returns:
            Any: Underlying object
         """
```

### Comparing `bip_utils-2.7.0/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py` & `bip_utils-2.7.1/bip_utils/ecc/secp256k1/secp256k1_point_ecdsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,24 @@
         Get the elliptic curve type.
 
         Returns:
            EllipticCurveTypes: Elliptic curve type
         """
         return EllipticCurveTypes.SECP256K1
 
+    @staticmethod
+    def CoordinateLength() -> int:
+        """
+        Get the coordinate length.
+
+        Returns:
+           int: Coordinate key length
+        """
+        return EcdsaKeysConst.POINT_COORD_BYTE_LEN
+
     def UnderlyingObject(self) -> Any:
         """
         Get the underlying object.
 
         Returns:
            Any: Underlying object
         """
```

### Comparing `bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519.py` & `bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519_const.py` & `bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519_const.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519_keys.py` & `bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ecc/sr25519/sr25519_point.py` & `bip_utils-2.7.1/bip_utils/ecc/sr25519/sr25519_point.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/electrum_v1.py` & `bip_utils-2.7.1/bip_utils/electrum/electrum_v1.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/electrum_v2.py` & `bip_utils-2.7.1/bip_utils/electrum/electrum_v2.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/__init__.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/electrum_v1_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v1/wordlist/english.txt` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v1/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/__init__.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py` & `bip_utils-2.7.1/bip_utils/electrum/mnemonic_v2/electrum_v2_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/conf/monero_coin_conf.py` & `bip_utils-2.7.1/bip_utils/monero/conf/monero_coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/conf/monero_coins.py` & `bip_utils-2.7.1/bip_utils/monero/conf/monero_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/conf/monero_conf.py` & `bip_utils-2.7.1/bip_utils/monero/conf/monero_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/conf/monero_conf_getter.py` & `bip_utils-2.7.1/bip_utils/monero/conf/monero_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/__init__.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_entropy_generator.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_decoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_encoder.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_generator.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_utils.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_mnemonic_validator.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/monero_seed_generator.py` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/monero_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/chinese_simplified.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/dutch.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/dutch.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/english.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/english.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/french.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/french.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/german.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/german.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/italian.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/italian.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/japanese.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/japanese.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/portuguese.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/portuguese.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/russian.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/russian.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/mnemonic/wordlist/spanish.txt` & `bip_utils-2.7.1/bip_utils/monero/mnemonic/wordlist/spanish.txt`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/monero.py` & `bip_utils-2.7.1/bip_utils/monero/monero.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/monero_ex.py` & `bip_utils-2.7.1/bip_utils/monero/monero_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/monero_keys.py` & `bip_utils-2.7.1/bip_utils/monero/monero_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/monero/monero_subaddr.py` & `bip_utils-2.7.1/bip_utils/monero/monero_subaddr.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/slip/slip173/slip173.py` & `bip_utils-2.7.1/bip_utils/slip/slip173/slip173.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/slip/slip32/slip32.py` & `bip_utils-2.7.1/bip_utils/slip/slip32/slip32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/slip/slip32/slip32_key_net_ver.py` & `bip_utils-2.7.1/bip_utils/slip/slip32/slip32_key_net_ver.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/slip/slip44/slip44.py` & `bip_utils-2.7.1/bip_utils/slip/slip44/slip44.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,17 +61,19 @@
     FILECOIN: int = 461
     BAND_PROTOCOL: int = 494
     THETA: int = 500
     SOLANA: int = 501
     ELROND: int = 508
     SECRET_NETWORK: int = 529
     NINE_CHRONICLES: int = 567
+    APTOS: int = 637
     BINANCE_CHAIN: int = 714
     VECHAIN: int = 818
     NEO: int = 888
     OKEX_CHAIN: int = 996
     HARMONY_ONE: int = 1023
     ONTOLOGY: int = 1024
     TEZOS: int = 1729
     CARDANO: int = 1815
     AVALANCHE: int = 9000
     CELO: int = 52752
+    PI_NETWORK: int = 314159
```

### Comparing `bip_utils-2.7.0/bip_utils/solana/spl_token.py` & `bip_utils-2.7.1/bip_utils/solana/spl_token.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ss58/ss58.py` & `bip_utils-2.7.1/bip_utils/ss58/ss58.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/ss58/ss58_ex.py` & `bip_utils-2.7.1/bip_utils/ss58/ss58_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/conf/substrate_coin_conf.py` & `bip_utils-2.7.1/bip_utils/substrate/conf/substrate_coin_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/conf/substrate_coins.py` & `bip_utils-2.7.1/bip_utils/substrate/conf/substrate_coins.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/conf/substrate_conf.py` & `bip_utils-2.7.1/bip_utils/substrate/conf/substrate_conf.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/conf/substrate_conf_getter.py` & `bip_utils-2.7.1/bip_utils/substrate/conf/substrate_conf_getter.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py` & `bip_utils-2.7.1/bip_utils/substrate/mnemonic/substrate_bip39_seed_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_base.py` & `bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_bytes.py` & `bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_bytes.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_cuint.py` & `bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_cuint.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/scale/substrate_scale_enc_uint.py` & `bip_utils-2.7.1/bip_utils/substrate/scale/substrate_scale_enc_uint.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/substrate.py` & `bip_utils-2.7.1/bip_utils/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/substrate_ex.py` & `bip_utils-2.7.1/bip_utils/substrate/substrate_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/substrate_keys.py` & `bip_utils-2.7.1/bip_utils/substrate/substrate_keys.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/substrate/substrate_path.py` & `bip_utils-2.7.1/bip_utils/substrate/substrate_path.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/conf/coin_names.py` & `bip_utils-2.7.1/bip_utils/utils/conf/coin_names.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/__init__.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/aes_ecb.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/aes_ecb.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/blake2.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/blake2.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/chacha20_poly1305.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/crc.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/crc.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/hash160.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/hash160.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/hmac.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/hmac.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/pbkdf2.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/pbkdf2.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,12 +55,12 @@
 
         Returns:
             bytes: Computed result
         """
         if HASHLIB_USE_PBKDF2_SHA512:
             return hashlib.pbkdf2_hmac("sha512", AlgoUtils.Encode(password), AlgoUtils.Encode(salt), itr_num, dklen)
         # Use Cryptodome if not implemented in hashlib
-        return PBKDF2(AlgoUtils.Encode(password),  # type: ignore
+        return PBKDF2(AlgoUtils.Encode(password),  # type: ignore [arg-type]
                       AlgoUtils.Encode(salt),
                       dklen or SHA512.digest_size,
                       count=itr_num,
                       hmac_hash_module=SHA512)
```

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/ripemd.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/ripemd.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/scrypt.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/scrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,13 +54,13 @@
 
         Returns:
             bytes: Computed result
         """
 
         # Type for password and salt should be Union[bytes, str] in pycryptodome, but it's only str
         # So, we ignore the mypy warning
-        return scrypt(AlgoUtils.Encode(password),   # type: ignore
-                      AlgoUtils.Encode(salt),       # type: ignore
+        return scrypt(AlgoUtils.Encode(password),   # type: ignore [arg-type, return-value]
+                      AlgoUtils.Encode(salt),       # type: ignore [arg-type]
                       key_len=key_len,
                       N=n,
                       r=r,
                       p=p)
```

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/sha2.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/sha2.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/crypto/sha3.py` & `bip_utils-2.7.1/bip_utils/utils/crypto/sha3.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/algo.py` & `bip_utils-2.7.1/bip_utils/utils/misc/algo.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/base32.py` & `bip_utils-2.7.1/bip_utils/utils/misc/base32.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/bit.py` & `bip_utils-2.7.1/bip_utils/utils/misc/bit.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/bytes.py` & `bip_utils-2.7.1/bip_utils/utils/misc/bytes.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/cbor_indefinite_len_array.py` & `bip_utils-2.7.1/bip_utils/utils/misc/cbor_indefinite_len_array.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/data_bytes.py` & `bip_utils-2.7.1/bip_utils/utils/misc/data_bytes.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/integer.py` & `bip_utils-2.7.1/bip_utils/utils/misc/integer.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/misc/string.py` & `bip_utils-2.7.1/bip_utils/utils/misc/string.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/__init__.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/__init__.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/entropy_generator.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/entropy_generator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_decoder_base.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_decoder_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_encoder_base.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_encoder_base.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_ex.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_ex.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_utils.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_utils.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/mnemonic/mnemonic_validator.py` & `bip_utils-2.7.1/bip_utils/utils/mnemonic/mnemonic_validator.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils/utils/typing/literal.py` & `bip_utils-2.7.1/bip_utils/utils/typing/literal.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 """Module with Literal type definition."""
 
 try:
     from typing import Literal  # pylint: disable=unused-import
 except ImportError:
     # Literal not supported by Python 3.7
-    from typing_extensions import Literal  # type: ignore # noqa: F401
+    from typing_extensions import Literal  # type: ignore [assignment] # noqa: F401
```

### Comparing `bip_utils-2.7.0/bip_utils/wif/wif.py` & `bip_utils-2.7.1/bip_utils/wif/wif.py`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/bip_utils.egg-info/PKG-INFO` & `bip_utils-2.7.1/bip_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bip-utils
-Version: 2.7.0
+Version: 2.7.1
 Summary: Generation of mnemonics, seeds, private/public keys and addresses for different types of cryptocurrencies
 Home-page: https://github.com/ebellocchia/bip_utils
-Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.7.0.tar.gz
+Download-URL: https://github.com/ebellocchia/bip_utils/archive/v2.7.1.tar.gz
 Author: Emanuele Bellocchia
 Author-email: ebellocchia@gmail.com
 Maintainer: Emanuele Bellocchia
 Maintainer-email: ebellocchia@gmail.com
 License: MIT
-Keywords: python,cryptography,ecdsa,ed25519,ed25519-blake2b,nist256p1,secp256k1,sr25519,wallet,hd-wallet,slip10,slip32,bip38,bip39,bip39-substrate,bip32,bip44,bip49,bip84,bip86,bip173,bip350,base58,ss58,bech32,bech32m,segwit,electrum,substrate,taproot,daedalus,byron,shelley,akash,algorand,atom,avalanche,avax,axelar,band protocol,binance chain,binance smart chain,bitcoin,bitcoin cash,bitcoinsv,bnb,cardano,cardano-byron,cardano-shelley,celo,certik,cosmos,dash,dogecoin,ecash,elrond,eos,ethereum,ethereum classic,fantom opera,filecoin,harmony one,huobi chain,icon,iris,irisnet,kava,litecoin,matic,monero,okex chain,ontology,osmosis,nano,near,near protocol,neo,polygon,ripple,secret,solana,stellar,substrate,terra,tezos,theta,tron,vechain,verge,zcash,zilliqa,acala,bifrost,chainx,edgeware,karura,kusama,moonbeam,moonriver,phala,plasm,sora,stafi,polkadot
+Keywords: python,cryptography,ecdsa,ed25519,ed25519-blake2b,nist256p1,secp256k1,sr25519,wallet,hd-wallet,slip10,slip32,bip38,bip39,bip39-substrate,bip32,bip44,bip49,bip84,bip86,bip173,bip350,base58,ss58,bech32,bech32m,segwit,electrum,substrate,taproot,daedalus,byron,shelley,akash,algorand,aptos,atom,avalanche,avax,axelar,band protocol,binance chain,binance smart chain,bitcoin,bitcoin cash,bitcoinsv,bnb,cardano,cardano-byron,cardano-shelley,celo,certik,cosmos,dash,dogecoin,ecash,elrond,eos,ethereum,ethereum classic,fantom opera,filecoin,harmony one,huobi chain,icon,iris,irisnet,kava,litecoin,matic,monero,okex chain,ontology,osmosis,nano,near,near protocol,neo,pi network,polygon,ripple,secret,solana,stellar,substrate,terra,tezos,theta,tron,vechain,verge,zcash,zilliqa,acala,bifrost,chainx,edgeware,karura,kusama,moonbeam,moonriver,phala,plasm,sora,stafi,polkadot
 Platform: any
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
@@ -82,14 +83,15 @@
 Please note that, for the py-sr25519-bindings library, Rust is required to be installed.
 
 ## Supported coins
 
 Supported BIP coins:
 - Akash Network
 - Algorand
+- Aptos
 - Avalanche (all the 3 chains)
 - Axelar
 - Band Protocol
 - Binance Chain
 - Binance Smart Chain
 - Bitcoin (and related test net)
 - Bitcoin Cash (and related test net)
@@ -118,14 +120,15 @@
 - Monero (based on BIP44 and secp256k1 or ed25519 SLIP-0010, it won't generate the same addresses of the official wallets, but it supports subaddresses generation)
 - Nano
 - Near Protocol
 - NEO
 - OKEx Chain (Ethereum and Cosmos addresses)
 - Ontology
 - Osmosis
+- Pi Network
 - Polkadot (based on BIP44 and ed25519 SLIP-0010, like TrustWallet, it won't generate the same addresses of Polkadot-JS)
 - Polygon
 - Ripple
 - Secret Network
 - Solana
 - Stellar
 - Terra
@@ -181,15 +184,17 @@
 
             pip install . --install-option="--coincurve=0"
 
     - Using *pip*, from PyPI:
 
             pip install bip_utils --install-option="--coincurve=0"
 
-**NOTE:** if you are using an Apple M1, please make sure to update *coincurve* to version 17.0.0 otherwise it won't work.
+**NOTES:**
+- if you are using an Apple M1, please make sure to update *coincurve* to version 17.0.0
+- in case of problems when building the *ed25519_blake2b* library, you can try one of the prebuilt wheels [here](https://github.com/ebellocchia/bip_utils/tree/master/libs_wheels)
 
 To run tests:
 
     python -m unittest discover
 
 Or you can install *tox*:
```

### Comparing `bip_utils-2.7.0/bip_utils.egg-info/SOURCES.txt` & `bip_utils-2.7.1/bip_utils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 bip_utils/addr/P2WPKH_addr.py
 bip_utils/addr/__init__.py
 bip_utils/addr/ada_byron_addr.py
 bip_utils/addr/ada_shelley_addr.py
 bip_utils/addr/addr_dec_utils.py
 bip_utils/addr/addr_key_validator.py
 bip_utils/addr/algo_addr.py
+bip_utils/addr/aptos_addr.py
 bip_utils/addr/atom_addr.py
 bip_utils/addr/avax_addr.py
 bip_utils/addr/bch_addr_converter.py
 bip_utils/addr/egld_addr.py
 bip_utils/addr/eos_addr.py
 bip_utils/addr/ergo_addr.py
 bip_utils/addr/eth_addr.py
```

### Comparing `bip_utils-2.7.0/keywords.txt` & `bip_utils-2.7.1/keywords.txt`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 daedalus
 byron
 shelley
 
 # BIP coins
 akash
 algorand
+aptos
 atom
 avalanche
 avax
 axelar
 band protocol
 binance chain
 binance smart chain
@@ -73,14 +74,15 @@
 okex chain
 ontology
 osmosis
 nano
 near
 near protocol
 neo
+pi network
 polygon
 ripple
 secret
 solana
 stellar
 substrate
 terra
```

### Comparing `bip_utils-2.7.0/readme/algorand_mnemonic.md` & `bip_utils-2.7.1/readme/algorand_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/bip32.md` & `bip_utils-2.7.1/readme/bip32.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/bip38.md` & `bip_utils-2.7.1/readme/bip38.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/bip39.md` & `bip_utils-2.7.1/readme/bip39.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/bip44.md` & `bip_utils-2.7.1/readme/bip44.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 Supported coins enumerative for BIP-0044:
 
 |Coin|Main net enum|Test net enum|
 |---|---|---|
 |Akash Network|`Bip44Coins.AKASH_NETWORK`|-|
 |Algorand|`Bip44Coins.ALGORAND`|-|
+|Aptos|`Bip44Coins.APTOS`|-|
 |Avalanche C-Chain|`Bip44Coins.AVAX_C_CHAIN`|-|
 |Avalanche P-Chain|`Bip44Coins.AVAX_P_CHAIN`|-|
 |Avalanche X-Chain|`Bip44Coins.AVAX_X_CHAIN`|-|
 |Axelar|`Bip44Coins.AXELAR`|-|
 |Band Protocol|`Bip44Coins.BAND_PROTOCOL`|-|
 |Binance Chain|`Bip44Coins.BINANCE_CHAIN`|-|
 |Binance Smart Chain|`Bip44Coins.BINANCE_SMART_CHAIN`|-|
@@ -60,14 +61,15 @@
 |Near Protocol|`Bip44Coins.NEAR_PROTOCOL`|-|
 |NEO|`Bip44Coins.NEO`|-|
 |OKEx Chain (Cosmos address)|`Bip44Coins.OKEX_CHAIN_ATOM`|-|
 |OKEx Chain (Ethereum address)|`Bip44Coins.OKEX_CHAIN_ETH`|-|
 |OKEx Chain (Old Cosmos address before mainnet upgrade)|`Bip44Coins.OKEX_CHAIN_ATOM_OLD`|-|
 |Ontology|`Bip44Coins.ONTOLOGY`|-|
 |Osmosis|`Bip44Coins.OSMOSIS`|-|
+|Pi Network|`Bip44Coins.PI_NETWORK`|-|
 |Polkadot (ed25519 SLIP-0010)|`Bip44Coins.POLKADOT_ED25519_SLIP`|-|
 |Polygon|`Bip44Coins.POLYGON`|-|
 |Ripple|`Bip44Coins.RIPPLE`|-|
 |Secret Network (old path)|`Bip44Coins.SECRET_NETWORK_OLD`|-|
 |Secret Network (new path)|`Bip44Coins.SECRET_NETWORK_NEW`|-|
 |Solana|`Bip44Coins.SOLANA`|-|
 |Stellar|`Bip44Coins.STELLAR`|-|
```

### Comparing `bip_utils-2.7.0/readme/cardano.md` & `bip_utils-2.7.1/readme/cardano.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/electrum.md` & `bip_utils-2.7.1/readme/electrum.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/electrum_mnemonic.md` & `bip_utils-2.7.1/readme/electrum_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/electrum_v1_mnemonic.md` & `bip_utils-2.7.1/readme/electrum_v1_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/electrum_v2_mnemonic.md` & `bip_utils-2.7.1/readme/electrum_v2_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/monero.md` & `bip_utils-2.7.1/readme/monero.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/monero_mnemonic.md` & `bip_utils-2.7.1/readme/monero_mnemonic.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/substrate.md` & `bip_utils-2.7.1/readme/substrate.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/utility/addr.md` & `bip_utils-2.7.1/readme/utility/addr.md`

 * *Files 9% similar despite different names*

```diff
@@ -139,14 +139,17 @@
     pub_key = binascii.unhexlify(b"00dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832")
     pub_key = Ed25519PublicKey.FromBytes(
         binascii.unhexlify(b"00dff41688eadfb8574c8fbfeb8707e07ecf571e96e929c395cc506839cc3ef832"))
     
     # Algorand address
     addr = AlgoAddrEncoder.EncodeKey(pub_key)
     pub_key_bytes = AlgoAddrDecoder.DecodeAddr(addr)
+    # Aptos address
+    addr = AptosAddrEncoder.EncodeKey(pub_key)
+    pub_key_hash = AptosAddrDecoder.DecodeAddr(addr)
     # Elrond address
     addr = EgldAddrEncoder.EncodeKey(pub_key)
     pub_key_bytes = EgldAddrDecoder.DecodeAddr(addr)
     
     # Solana address
     addr = SolAddrEncoder.EncodeKey(pub_key)
     pub_key_bytes = SolAddrDecoder.DecodeAddr(addr)
@@ -240,14 +243,48 @@
                                               net_ver=MoneroConf.MainNet.IntegratedAddrNetVersion(),
                                               payment_id=binascii.unhexlify(b"d7af025ab223b74e"))
     # Decoding
     pub_key_bytes = XmrIntegratedAddrDecoder.DecodeAddr(addr,
                                                         net_ver=CoinsConf.MoneroMainNet.ParamByKey("addr_int_net_ver"),
                                                         payment_id=binascii.unhexlify(b"d7af025ab223b74e"))
 
+**Code example (coins based on the ed25519-kholaw curve)**
+
+    import binascii
+    from bip_utils import *
+    
+    # Public key bytes or a public key object can be used
+    pub_key = binascii.unhexlify(b"01f9256746c79ad5ba163ae677e3e3477471f0c3f8e1b5012c7a09f862e3972d")
+    pub_key = Ed25519KholawPublicKey.FromBytes(
+        binascii.unhexlify(b"0072629d389eabb6a4a6e35c9b0cab50b546b4a49a20d1d831956bd06098ba3370")
+    )
+    
+    # ADA Byron Icarus address (a chain code is also required)
+    chain_code = binascii.unhexlify(b"fa8397359cea983fe2195214e96b4d9f9bc31941d973a77d2d98ac77ea186db8")
+    
+    addr = AdaByronIcarusAddrEncoder.EncodeKey(pub_key, chain_code=chain_code)
+    pub_key_hash = AdaByronAddrDecoder.DecodeAddr(addr)
+    
+    # ADA Byron legacy address (chain code and HD data are also required)
+    hd_path_key = binascii.unhexlify(b"c582f8e7cf7aeb6e5f3e96e939a92ae1642360a51d45150f34e70132a152203f")
+    
+    addr = AdaByronLegacyAddrEncoder.EncodeKey(pub_key,
+                                               chain_code=chain_code,
+                                               hd_path="m/0'/0'",
+                                               hd_path_key=hd_path_key)
+    pub_key_hash = AdaByronAddrDecoder.DecodeAddr(addr)
+    
+    # ADA Shelley address (a staking key is also required)
+    pub_skey = binascii.unhexlify(b"7680c767b8096daa3299dc282068327c79976f346e55b72d0ffd751295a45913")
+    
+    addr = AdaShelleyAddrEncoder.EncodeKey(pub_key,
+                                           pub_skey=pub_skey,
+                                           net_tag=AdaShelleyAddrNetworkTags.MAINNET)
+    pub_key_hash = AdaShelleyAddrDecoder.DecodeAddr(addr)
+
 **Code example (coins based on the nist256p1 curve)**
 
     import binascii
     from bip_utils import *
 
     # Public key bytes or a public key object can be used
     pub_key = binascii.unhexlify(b"038ea003d38b3f2043e681f06f56b3864d28d73b4f243aee90ed04a28dbc058c5b")
```

### Comparing `bip_utils-2.7.0/readme/utility/base58.md` & `bip_utils-2.7.1/readme/utility/base58.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/utility/bch_addr_converter.md` & `bip_utils-2.7.1/readme/utility/bch_addr_converter.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/utility/bech32.md` & `bip_utils-2.7.1/readme/utility/bech32.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/utility/slip32.md` & `bip_utils-2.7.1/readme/utility/slip32.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/utility/solana_spl.md` & `bip_utils-2.7.1/readme/utility/solana_spl.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/utility/wif.md` & `bip_utils-2.7.1/readme/utility/wif.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/readme/utility_libs.md` & `bip_utils-2.7.1/readme/utility_libs.md`

 * *Files identical despite different names*

### Comparing `bip_utils-2.7.0/setup.py` & `bip_utils-2.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
     keywords=load_keywords("keywords.txt"),
     platforms=["any"],
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
     ],
     python_requires=">=3.7",
 )
```

