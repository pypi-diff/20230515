# Comparing `tmp/web3-6.3.0.tar.gz` & `tmp/web3-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3-6.3.0.tar", last modified: Wed May  3 16:27:24 2023, max compression
+gzip compressed data, was "web3-6.4.0.tar", last modified: Mon May 15 20:38:14 2023, max compression
```

## Comparing `web3-6.3.0.tar` & `web3-6.4.0.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.421461 web3-6.3.0/
--rw-r--r--   0 fselmo     (501) staff       (20)     1080 2021-06-07 18:31:00.000000 web3-6.3.0/LICENSE
--rw-r--r--   0 fselmo     (501) staff       (20)      260 2022-10-19 16:28:38.000000 web3-6.3.0/MANIFEST.in
--rw-r--r--   0 fselmo     (501) staff       (20)     2184 2023-05-03 16:27:24.421154 web3-6.3.0/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     1294 2023-03-13 21:36:03.000000 web3-6.3.0/README.md
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.291262 web3-6.3.0/ens/
--rw-r--r--   0 fselmo     (501) staff       (20)      285 2023-03-13 21:36:03.000000 web3-6.3.0/ens/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    23773 2023-03-13 21:36:03.000000 web3-6.3.0/ens/abis.py
--rw-r--r--   0 fselmo     (501) staff       (20)    20886 2023-03-13 21:36:03.000000 web3-6.3.0/ens/async_ens.py
--rw-r--r--   0 fselmo     (501) staff       (20)       41 2023-03-13 21:36:03.000000 web3-6.3.0/ens/auto.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3287 2023-03-13 21:36:03.000000 web3-6.3.0/ens/base_ens.py
--rw-r--r--   0 fselmo     (501) staff       (20)      601 2023-03-13 21:36:03.000000 web3-6.3.0/ens/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)   199089 2023-03-13 21:36:03.000000 web3-6.3.0/ens/contract_data.py
--rw-r--r--   0 fselmo     (501) staff       (20)    20044 2023-03-13 21:36:03.000000 web3-6.3.0/ens/ens.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2390 2023-03-13 21:36:03.000000 web3-6.3.0/ens/exceptions.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8978 2023-03-13 21:36:03.000000 web3-6.3.0/ens/utils.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.294037 web3-6.3.0/ethpm/
--rw-r--r--   0 fselmo     (501) staff       (20)      580 2023-02-01 21:57:10.000000 web3-6.3.0/ethpm/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.296769 web3-6.3.0/ethpm/_utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/_utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2511 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/_utils/backend.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1477 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/_utils/cache.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2848 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/_utils/chains.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1030 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/_utils/contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5263 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/_utils/deployments.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2717 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/_utils/ipfs.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.297345 web3-6.3.0/ethpm/_utils/protobuf/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-11-22 17:31:20.000000 web3-6.3.0/ethpm/_utils/protobuf/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1938 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/_utils/protobuf/ipfs_file_pb2.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1488 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/_utils/registry.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.298074 web3-6.3.0/ethpm/assets/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.298798 web3-6.3.0/ethpm/assets/ens/
--rw-r--r--   0 fselmo     (501) staff       (20)    74682 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/ens/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.300313 web3-6.3.0/ethpm/assets/escrow/
--rw-r--r--   0 fselmo     (501) staff       (20)     8007 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/escrow/with_bytecode_v3.json
--rw-r--r--   0 fselmo     (501) staff       (20)      760 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/assets/ipfs_file.proto
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.300998 web3-6.3.0/ethpm/assets/owned/
--rw-r--r--   0 fselmo     (501) staff       (20)     2655 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/owned/output_v3.json
--rw-r--r--   0 fselmo     (501) staff       (20)      746 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/owned/with_contract_type_v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.306175 web3-6.3.0/ethpm/assets/registry/
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.313176 web3-6.3.0/ethpm/assets/registry/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)     3129 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/contracts/Authority.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     2876 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     6380 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/contracts/PackageDB.sol
--rw-r--r--   0 fselmo     (501) staff       (20)    10553 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/contracts/PackageRegistry.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     2966 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     9041 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/contracts/ReleaseDB.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     4980 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/contracts/ReleaseValidator.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     1046 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/solc_input.json
--rw-r--r--   0 fselmo     (501) staff       (20)   727775 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/registry/solc_output.json
--rw-r--r--   0 fselmo     (501) staff       (20)   270218 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/registry/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.313751 web3-6.3.0/ethpm/assets/safe-math-lib/
--rw-r--r--   0 fselmo     (501) staff       (20)     2845 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.317381 web3-6.3.0/ethpm/assets/simple-registry/
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.319872 web3-6.3.0/ethpm/assets/simple-registry/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)     1841 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/simple-registry/contracts/Ownable.sol
--rw-r--r--   0 fselmo     (501) staff       (20)    12350 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     3278 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
--rw-r--r--   0 fselmo     (501) staff       (20)      950 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/simple-registry/solc_input.json
--rw-r--r--   0 fselmo     (501) staff       (20)   199338 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/simple-registry/solc_output.json
--rw-r--r--   0 fselmo     (501) staff       (20)    75677 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/simple-registry/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.321328 web3-6.3.0/ethpm/assets/standard-token/
--rw-r--r--   0 fselmo     (501) staff       (20)    22292 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/standard-token/output_v3.json
--rw-r--r--   0 fselmo     (501) staff       (20)     8765 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/assets/standard-token/with_bytecode_v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.324673 web3-6.3.0/ethpm/assets/vyper_registry/
--rw-r--r--   0 fselmo     (501) staff       (20)    81363 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/vyper_registry/0.1.0.json
--rw-r--r--   0 fselmo     (501) staff       (20)     6339 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/vyper_registry/registry.vy
--rw-r--r--   0 fselmo     (501) staff       (20)     7596 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/assets/vyper_registry/registry_with_delete.vy
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.326500 web3-6.3.0/ethpm/backends/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/backends/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      956 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/backends/base.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3006 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/backends/http.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6551 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/backends/ipfs.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4174 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/backends/registry.py
--rw-r--r--   0 fselmo     (501) staff       (20)      405 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/constants.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6256 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1890 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/dependencies.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2134 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/deployments.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.279095 web3-6.3.0/ethpm/ethpm-spec/
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.278512 web3-6.3.0/ethpm/ethpm-spec/examples/
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.329006 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/
--rw-r--r--   0 fselmo     (501) staff       (20)     6810 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     5361 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.330279 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)      888 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
--rw-r--r--   0 fselmo     (501) staff       (20)      644 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
--rw-r--r--   0 fselmo     (501) staff       (20)    11598 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     8669 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/escrow/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.332508 web3-6.3.0/ethpm/ethpm-spec/examples/owned/
--rw-r--r--   0 fselmo     (501) staff       (20)      544 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)      443 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/owned/1.0.0.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.332847 web3-6.3.0/ethpm/ethpm-spec/examples/owned/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)      222 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
--rw-r--r--   0 fselmo     (501) staff       (20)      728 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)      478 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/owned/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.334945 web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/
--rw-r--r--   0 fselmo     (501) staff       (20)     5272 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     5030 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
--rw-r--r--   0 fselmo     (501) staff       (20)     5220 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     4993 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.337338 web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/
--rw-r--r--   0 fselmo     (501) staff       (20)     3976 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     3143 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.337928 web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)      802 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     5517 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     3289 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.340463 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/
--rw-r--r--   0 fselmo     (501) staff       (20)     3794 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     3238 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.341487 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)     1155 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     2949 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
--rw-r--r--   0 fselmo     (501) staff       (20)    17129 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     6100 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.343691 web3-6.3.0/ethpm/ethpm-spec/examples/transferable/
--rw-r--r--   0 fselmo     (501) staff       (20)      590 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)      507 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/transferable/1.0.0.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.344207 web3-6.3.0/ethpm/ethpm-spec/examples/transferable/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)      396 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
--rw-r--r--   0 fselmo     (501) staff       (20)      786 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)      548 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/transferable/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.346249 web3-6.3.0/ethpm/ethpm-spec/examples/wallet/
--rw-r--r--   0 fselmo     (501) staff       (20)     6669 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     5456 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.349131 web3-6.3.0/ethpm/ethpm-spec/examples/wallet/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)     1454 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
--rw-r--r--   0 fselmo     (501) staff       (20)     9710 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     7326 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.348209 web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/
--rw-r--r--   0 fselmo     (501) staff       (20)     8052 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     6657 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.348668 web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
--rw-r--r--   0 fselmo     (501) staff       (20)      621 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
--rw-r--r--   0 fselmo     (501) staff       (20)    12191 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
--rw-r--r--   0 fselmo     (501) staff       (20)     9503 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.350278 web3-6.3.0/ethpm/ethpm-spec/spec/
--rw-r--r--   0 fselmo     (501) staff       (20)    10302 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/spec/package.spec.json
--rw-r--r--   0 fselmo     (501) staff       (20)    12879 2023-01-03 18:30:11.000000 web3-6.3.0/ethpm/ethpm-spec/spec/v3.spec.json
--rw-r--r--   0 fselmo     (501) staff       (20)     1194 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/exceptions.py
--rw-r--r--   0 fselmo     (501) staff       (20)    14493 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/package.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.351509 web3-6.3.0/ethpm/tools/
--rw-r--r--   0 fselmo     (501) staff       (20)      103 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/tools/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    27045 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/tools/builder.py
--rw-r--r--   0 fselmo     (501) staff       (20)    10373 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/tools/checker.py
--rw-r--r--   0 fselmo     (501) staff       (20)      475 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/tools/get_manifest.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4368 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/uri.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.352875 web3-6.3.0/ethpm/validation/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.3.0/ethpm/validation/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4716 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/validation/manifest.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1072 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/validation/misc.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2317 2022-08-03 17:01:33.000000 web3-6.3.0/ethpm/validation/package.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4873 2023-03-13 21:36:03.000000 web3-6.3.0/ethpm/validation/uri.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1046 2023-03-09 20:41:55.000000 web3-6.3.0/pyproject.toml
--rw-r--r--   0 fselmo     (501) staff       (20)       38 2023-05-03 16:27:24.421550 web3-6.3.0/setup.cfg
--rw-r--r--   0 fselmo     (501) staff       (20)     3168 2023-05-03 16:27:07.000000 web3-6.3.0/setup.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.358018 web3-6.3.0/web3/
--rw-r--r--   0 fselmo     (501) staff       (20)      752 2023-03-13 21:36:03.000000 web3-6.3.0/web3/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.370671 web3-6.3.0/web3/_utils/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.3.0/web3/_utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    28771 2023-03-24 19:41:43.000000 web3-6.3.0/web3/_utils/abi.py
--rw-r--r--   0 fselmo     (501) staff       (20)      456 2023-03-17 20:50:50.000000 web3-6.3.0/web3/_utils/async_caching.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7693 2023-04-18 15:26:41.000000 web3-6.3.0/web3/_utils/async_transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2059 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/blocks.py
--rw-r--r--   0 fselmo     (501) staff       (20)      992 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/caching.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.371891 web3-6.3.0/web3/_utils/compat/
--rw-r--r--   0 fselmo     (501) staff       (20)      319 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/compat/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.3.0/web3/_utils/compat/compat_py2.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.3.0/web3/_utils/compat/compat_py3.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.372445 web3-6.3.0/web3/_utils/contract_sources/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/contract_sources/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6406 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/contract_sources/compile_contracts.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.386291 web3-6.3.0/web3/_utils/contract_sources/contract_data/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      517 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5344 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/address_reflector.py
--rw-r--r--   0 fselmo     (501) staff       (20)    19324 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/arrays_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)    15157 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6219 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6492 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
--rw-r--r--   0 fselmo     (501) staff       (20)    38375 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/emitter_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5673 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/event_contracts.py
--rw-r--r--   0 fselmo     (501) staff       (20)    16216 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/extended_resolver.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1685 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7829 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/math_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)    17122 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
--rw-r--r--   0 fselmo     (501) staff       (20)    33495 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1863 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/payable_tester.py
--rw-r--r--   0 fselmo     (501) staff       (20)    17734 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5410 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4338 2023-04-18 15:26:41.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/revert_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3653 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/simple_resolver.py
--rw-r--r--   0 fselmo     (501) staff       (20)    11900 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/string_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)    23756 2023-04-10 19:45:10.000000 web3-6.3.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
--rw-r--r--   0 fselmo     (501) staff       (20)    14980 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/contracts.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1640 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/datatypes.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1738 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/decorators.py
--rw-r--r--   0 fselmo     (501) staff       (20)      144 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/empty.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9065 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/encoding.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2120 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/ens.py
--rw-r--r--   0 fselmo     (501) staff       (20)    17134 2023-05-01 19:20:37.000000 web3-6.3.0/web3/_utils/events.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2113 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/fee_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)    11886 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/filters.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3071 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/formatters.py
--rw-r--r--   0 fselmo     (501) staff       (20)       55 2022-01-11 17:23:55.000000 web3-6.3.0/web3/_utils/function_identifiers.py
--rw-r--r--   0 fselmo     (501) staff       (20)      195 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/http.py
--rw-r--r--   0 fselmo     (501) staff       (20)      209 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/hypothesis.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1047 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/math.py
--rw-r--r--   0 fselmo     (501) staff       (20)    32977 2023-05-01 21:51:26.000000 web3-6.3.0/web3/_utils/method_formatters.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1146 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/miner.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3147 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.392346 web3-6.3.0/web3/_utils/module_testing/
--rw-r--r--   0 fselmo     (501) staff       (20)      539 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module_testing/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)   166576 2023-05-03 16:16:36.000000 web3-6.3.0/web3/_utils/module_testing/eth_module.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3406 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module_testing/go_ethereum_admin_module.py
--rw-r--r--   0 fselmo     (501) staff       (20)    10338 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module_testing/go_ethereum_personal_module.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1176 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module_testing/go_ethereum_txpool_module.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4825 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module_testing/module_testing_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1272 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module_testing/net_module.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9335 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/module_testing/web3_module.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6493 2023-03-28 22:38:40.000000 web3-6.3.0/web3/_utils/normalizers.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8833 2023-03-30 17:28:09.000000 web3-6.3.0/web3/_utils/request.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9449 2023-04-03 19:23:10.000000 web3-6.3.0/web3/_utils/rpc_abi.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4207 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/threads.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8737 2023-04-18 15:26:41.000000 web3-6.3.0/web3/_utils/transactions.py
--rw-r--r--   0 fselmo     (501) staff       (20)      816 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/type_conversion.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1669 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/utility_methods.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6291 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/validation.py
--rw-r--r--   0 fselmo     (501) staff       (20)      994 2023-03-13 21:36:03.000000 web3-6.3.0/web3/_utils/windows.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.393255 web3-6.3.0/web3/auto/
--rw-r--r--   0 fselmo     (501) staff       (20)       44 2023-03-13 21:36:03.000000 web3-6.3.0/web3/auto/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      263 2023-02-18 04:25:14.000000 web3-6.3.0/web3/auto/gethdev.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.395618 web3-6.3.0/web3/beacon/
--rw-r--r--   0 fselmo     (501) staff       (20)       91 2023-03-13 21:36:03.000000 web3-6.3.0/web3/beacon/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1516 2023-03-13 21:36:03.000000 web3-6.3.0/web3/beacon/api_endpoints.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5421 2023-03-13 21:36:03.000000 web3-6.3.0/web3/beacon/async_beacon.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4772 2023-03-13 21:36:03.000000 web3-6.3.0/web3/beacon/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)      396 2023-03-13 21:36:03.000000 web3-6.3.0/web3/constants.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.397642 web3-6.3.0/web3/contract/
--rw-r--r--   0 fselmo     (501) staff       (20)      215 2023-03-13 21:36:03.000000 web3-6.3.0/web3/contract/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    19756 2023-03-13 21:36:03.000000 web3-6.3.0/web3/contract/async_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)    35710 2023-03-13 21:36:03.000000 web3-6.3.0/web3/contract/base_contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)    18804 2023-03-13 21:36:03.000000 web3-6.3.0/web3/contract/contract.py
--rw-r--r--   0 fselmo     (501) staff       (20)    12338 2023-04-26 20:55:37.000000 web3-6.3.0/web3/contract/utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8271 2023-03-13 21:36:03.000000 web3-6.3.0/web3/datastructures.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.398773 web3-6.3.0/web3/eth/
--rw-r--r--   0 fselmo     (501) staff       (20)      166 2023-03-13 21:36:03.000000 web3-6.3.0/web3/eth/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    20181 2023-05-03 16:16:36.000000 web3-6.3.0/web3/eth/async_eth.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5943 2023-03-13 21:36:03.000000 web3-6.3.0/web3/eth/base_eth.py
--rw-r--r--   0 fselmo     (501) staff       (20)    19295 2023-03-30 18:14:04.000000 web3-6.3.0/web3/eth/eth.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6238 2023-05-01 19:20:38.000000 web3-6.3.0/web3/exceptions.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.400100 web3-6.3.0/web3/gas_strategies/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-06-07 18:31:01.000000 web3-6.3.0/web3/gas_strategies/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      430 2023-03-13 21:36:03.000000 web3-6.3.0/web3/gas_strategies/rpc.py
--rw-r--r--   0 fselmo     (501) staff       (20)     9010 2023-03-13 21:36:03.000000 web3-6.3.0/web3/gas_strategies/time_based.py
--rw-r--r--   0 fselmo     (501) staff       (20)    11826 2023-03-13 21:36:03.000000 web3-6.3.0/web3/geth.py
--rw-r--r--   0 fselmo     (501) staff       (20)      198 2022-09-26 17:05:32.000000 web3-6.3.0/web3/logs.py
--rw-r--r--   0 fselmo     (501) staff       (20)    12774 2023-05-01 19:20:37.000000 web3-6.3.0/web3/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     7875 2023-04-03 19:23:10.000000 web3-6.3.0/web3/manager.py
--rw-r--r--   0 fselmo     (501) staff       (20)     8430 2023-04-03 18:07:44.000000 web3-6.3.0/web3/method.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.406983 web3-6.3.0/web3/middleware/
--rw-r--r--   0 fselmo     (501) staff       (20)     3724 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      239 2023-01-31 22:25:40.000000 web3-6.3.0/web3/middleware/abi.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2755 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/async_cache.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1779 2023-04-03 19:23:10.000000 web3-6.3.0/web3/middleware/attrdict.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1785 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/buffered_gas_estimate.py
--rw-r--r--   0 fselmo     (501) staff       (20)    12617 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/cache.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1167 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/exception_handling.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3119 2023-03-28 22:38:40.000000 web3-6.3.0/web3/middleware/exception_retry_request.py
--rw-r--r--   0 fselmo     (501) staff       (20)    21131 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/filter.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4596 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/fixture.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4762 2023-04-03 19:23:10.000000 web3-6.3.0/web3/middleware/formatting.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4212 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/gas_price_strategy.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1657 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/geth_poa.py
--rw-r--r--   0 fselmo     (501) staff       (20)      590 2023-01-27 23:21:48.000000 web3-6.3.0/web3/middleware/names.py
--rw-r--r--   0 fselmo     (501) staff       (20)      246 2022-12-08 21:12:34.000000 web3-6.3.0/web3/middleware/normalize_request_parameters.py
--rw-r--r--   0 fselmo     (501) staff       (20)      351 2023-02-03 21:22:38.000000 web3-6.3.0/web3/middleware/pythonic.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4450 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/signing.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1014 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/simulate_unmined_transaction.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3739 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/stalecheck.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4573 2023-03-13 21:36:03.000000 web3-6.3.0/web3/middleware/validation.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3615 2023-04-03 19:23:10.000000 web3-6.3.0/web3/module.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1562 2023-03-13 21:36:03.000000 web3-6.3.0/web3/net.py
--rw-r--r--   0 fselmo     (501) staff       (20)    21609 2023-03-13 21:36:03.000000 web3-6.3.0/web3/pm.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.409118 web3-6.3.0/web3/providers/
--rw-r--r--   0 fselmo     (501) staff       (20)      368 2023-04-03 19:23:10.000000 web3-6.3.0/web3/providers/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4178 2023-05-01 19:20:37.000000 web3-6.3.0/web3/providers/async_base.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2469 2023-03-13 21:36:03.000000 web3-6.3.0/web3/providers/async_rpc.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3447 2023-05-01 19:20:37.000000 web3-6.3.0/web3/providers/auto.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4111 2023-05-01 19:20:37.000000 web3-6.3.0/web3/providers/base.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.410224 web3-6.3.0/web3/providers/eth_tester/
--rw-r--r--   0 fselmo     (501) staff       (20)       97 2023-03-13 21:36:03.000000 web3-6.3.0/web3/providers/eth_tester/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)    14397 2023-05-01 19:20:38.000000 web3-6.3.0/web3/providers/eth_tester/defaults.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5512 2023-05-01 19:20:37.000000 web3-6.3.0/web3/providers/eth_tester/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)    12665 2023-05-03 16:16:32.000000 web3-6.3.0/web3/providers/eth_tester/middleware.py
--rw-r--r--   0 fselmo     (501) staff       (20)     6533 2023-05-01 19:20:37.000000 web3-6.3.0/web3/providers/ipc.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2686 2023-03-13 21:36:03.000000 web3-6.3.0/web3/providers/rpc.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3919 2023-03-29 17:00:22.000000 web3-6.3.0/web3/providers/websocket.py
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.3.0/web3/py.typed
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.410489 web3-6.3.0/web3/scripts/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.3.0/web3/scripts/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.410922 web3-6.3.0/web3/scripts/release/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-01-11 17:23:55.000000 web3-6.3.0/web3/scripts/release/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1534 2023-03-13 21:36:03.000000 web3-6.3.0/web3/scripts/release/test_package.py
--rw-r--r--   0 fselmo     (501) staff       (20)      951 2023-03-13 21:36:03.000000 web3-6.3.0/web3/testing.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.411756 web3-6.3.0/web3/tools/
--rw-r--r--   0 fselmo     (501) staff       (20)       73 2022-09-26 17:05:32.000000 web3-6.3.0/web3/tools/__init__.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.414548 web3-6.3.0/web3/tools/benchmark/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2022-08-03 17:01:33.000000 web3-6.3.0/web3/tools/benchmark/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     5886 2023-03-13 21:36:03.000000 web3-6.3.0/web3/tools/benchmark/main.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3435 2023-03-28 22:38:40.000000 web3-6.3.0/web3/tools/benchmark/node.py
--rw-r--r--   0 fselmo     (501) staff       (20)      912 2023-03-13 21:36:03.000000 web3-6.3.0/web3/tools/benchmark/reporting.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1722 2023-02-13 20:41:33.000000 web3-6.3.0/web3/tools/benchmark/utils.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.417948 web3-6.3.0/web3/tools/pytest_ethereum/
--rw-r--r--   0 fselmo     (501) staff       (20)        0 2021-11-01 21:09:29.000000 web3-6.3.0/web3/tools/pytest_ethereum/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)     4158 2023-03-13 21:36:03.000000 web3-6.3.0/web3/tools/pytest_ethereum/_utils.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1423 2023-03-13 21:36:03.000000 web3-6.3.0/web3/tools/pytest_ethereum/deployer.py
--rw-r--r--   0 fselmo     (501) staff       (20)      380 2021-11-01 21:09:29.000000 web3-6.3.0/web3/tools/pytest_ethereum/exceptions.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3927 2023-03-13 21:36:03.000000 web3-6.3.0/web3/tools/pytest_ethereum/linker.py
--rw-r--r--   0 fselmo     (501) staff       (20)      645 2023-03-13 21:36:03.000000 web3-6.3.0/web3/tools/pytest_ethereum/plugins.py
--rw-r--r--   0 fselmo     (501) staff       (20)     2968 2023-04-18 15:26:41.000000 web3-6.3.0/web3/tracing.py
--rw-r--r--   0 fselmo     (501) staff       (20)    10665 2023-04-18 15:26:41.000000 web3-6.3.0/web3/types.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.420559 web3-6.3.0/web3/utils/
--rw-r--r--   0 fselmo     (501) staff       (20)      454 2023-03-13 21:36:03.000000 web3-6.3.0/web3/utils/__init__.py
--rw-r--r--   0 fselmo     (501) staff       (20)      498 2023-03-13 21:36:03.000000 web3-6.3.0/web3/utils/abi.py
--rw-r--r--   0 fselmo     (501) staff       (20)      967 2023-03-13 21:36:03.000000 web3-6.3.0/web3/utils/address.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3096 2023-03-13 21:36:03.000000 web3-6.3.0/web3/utils/async_exception_handling.py
--rw-r--r--   0 fselmo     (501) staff       (20)     1521 2023-03-13 21:36:03.000000 web3-6.3.0/web3/utils/caching.py
--rw-r--r--   0 fselmo     (501) staff       (20)     3052 2023-03-13 21:36:03.000000 web3-6.3.0/web3/utils/exception_handling.py
-drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2023-05-03 16:27:24.360153 web3-6.3.0/web3.egg-info/
--rw-r--r--   0 fselmo     (501) staff       (20)     2184 2023-05-03 16:27:24.000000 web3-6.3.0/web3.egg-info/PKG-INFO
--rw-r--r--   0 fselmo     (501) staff       (20)     9743 2023-05-03 16:27:24.000000 web3-6.3.0/web3.egg-info/SOURCES.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-05-03 16:27:24.000000 web3-6.3.0/web3.egg-info/dependency_links.txt
--rw-r--r--   0 fselmo     (501) staff       (20)       64 2023-05-03 16:27:24.000000 web3-6.3.0/web3.egg-info/entry_points.txt
--rw-r--r--   0 fselmo     (501) staff       (20)        1 2023-05-03 16:27:24.000000 web3-6.3.0/web3.egg-info/not-zip-safe
--rw-r--r--   0 fselmo     (501) staff       (20)     1165 2023-05-03 16:27:24.000000 web3-6.3.0/web3.egg-info/requires.txt
--rw-r--r--   0 fselmo     (501) staff       (20)       15 2023-05-03 16:27:24.000000 web3-6.3.0/web3.egg-info/top_level.txt
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.720725 web3-6.4.0/
+-rw-r--r--   0 eve        (501) staff       (20)     1080 2023-04-06 21:34:13.000000 web3-6.4.0/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      260 2023-04-06 21:34:13.000000 web3-6.4.0/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     2184 2023-05-15 20:38:14.720576 web3-6.4.0/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     1294 2023-04-10 20:16:28.000000 web3-6.4.0/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.663650 web3-6.4.0/ens/
+-rw-r--r--   0 eve        (501) staff       (20)      285 2023-04-10 20:16:28.000000 web3-6.4.0/ens/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    23773 2023-04-06 21:34:13.000000 web3-6.4.0/ens/abis.py
+-rw-r--r--   0 eve        (501) staff       (20)    20886 2023-04-10 20:16:28.000000 web3-6.4.0/ens/async_ens.py
+-rw-r--r--   0 eve        (501) staff       (20)       41 2023-04-10 20:16:28.000000 web3-6.4.0/ens/auto.py
+-rw-r--r--   0 eve        (501) staff       (20)     3287 2023-04-10 20:16:28.000000 web3-6.4.0/ens/base_ens.py
+-rw-r--r--   0 eve        (501) staff       (20)      601 2023-04-06 21:34:13.000000 web3-6.4.0/ens/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)   199089 2023-04-06 21:34:13.000000 web3-6.4.0/ens/contract_data.py
+-rw-r--r--   0 eve        (501) staff       (20)    20044 2023-04-10 20:16:28.000000 web3-6.4.0/ens/ens.py
+-rw-r--r--   0 eve        (501) staff       (20)     2390 2023-04-06 21:34:13.000000 web3-6.4.0/ens/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)     8978 2023-04-10 20:16:28.000000 web3-6.4.0/ens/utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.665095 web3-6.4.0/ethpm/
+-rw-r--r--   0 eve        (501) staff       (20)      746 2023-05-15 20:27:41.000000 web3-6.4.0/ethpm/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.666454 web3-6.4.0/ethpm/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     2511 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/_utils/backend.py
+-rw-r--r--   0 eve        (501) staff       (20)     1477 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)     2848 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/chains.py
+-rw-r--r--   0 eve        (501) staff       (20)     1030 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     5263 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/deployments.py
+-rw-r--r--   0 eve        (501) staff       (20)     2717 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/ipfs.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.666759 web3-6.4.0/ethpm/_utils/protobuf/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/protobuf/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1938 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/protobuf/ipfs_file_pb2.py
+-rw-r--r--   0 eve        (501) staff       (20)     1488 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/_utils/registry.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.666971 web3-6.4.0/ethpm/assets/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.667199 web3-6.4.0/ethpm/assets/ens/
+-rw-r--r--   0 eve        (501) staff       (20)    74682 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/ens/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.667504 web3-6.4.0/ethpm/assets/escrow/
+-rw-r--r--   0 eve        (501) staff       (20)     8007 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/escrow/with_bytecode_v3.json
+-rw-r--r--   0 eve        (501) staff       (20)      760 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/ipfs_file.proto
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.667762 web3-6.4.0/ethpm/assets/owned/
+-rw-r--r--   0 eve        (501) staff       (20)     2655 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/owned/output_v3.json
+-rw-r--r--   0 eve        (501) staff       (20)      746 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/owned/with_contract_type_v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.669876 web3-6.4.0/ethpm/assets/registry/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.672226 web3-6.4.0/ethpm/assets/registry/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     3129 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/contracts/Authority.sol
+-rw-r--r--   0 eve        (501) staff       (20)     2876 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol
+-rw-r--r--   0 eve        (501) staff       (20)     6380 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/contracts/PackageDB.sol
+-rw-r--r--   0 eve        (501) staff       (20)    10553 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 eve        (501) staff       (20)     2966 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 eve        (501) staff       (20)     9041 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/contracts/ReleaseDB.sol
+-rw-r--r--   0 eve        (501) staff       (20)     4980 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/contracts/ReleaseValidator.sol
+-rw-r--r--   0 eve        (501) staff       (20)     1046 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/solc_input.json
+-rw-r--r--   0 eve        (501) staff       (20)   727775 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/solc_output.json
+-rw-r--r--   0 eve        (501) staff       (20)   270218 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/registry/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.672373 web3-6.4.0/ethpm/assets/safe-math-lib/
+-rw-r--r--   0 eve        (501) staff       (20)     2845 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.673720 web3-6.4.0/ethpm/assets/simple-registry/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.674785 web3-6.4.0/ethpm/assets/simple-registry/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     1841 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/simple-registry/contracts/Ownable.sol
+-rw-r--r--   0 eve        (501) staff       (20)    12350 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol
+-rw-r--r--   0 eve        (501) staff       (20)     3278 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol
+-rw-r--r--   0 eve        (501) staff       (20)      950 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/simple-registry/solc_input.json
+-rw-r--r--   0 eve        (501) staff       (20)   199338 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/simple-registry/solc_output.json
+-rw-r--r--   0 eve        (501) staff       (20)    75677 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/simple-registry/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.675421 web3-6.4.0/ethpm/assets/standard-token/
+-rw-r--r--   0 eve        (501) staff       (20)    22292 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/standard-token/output_v3.json
+-rw-r--r--   0 eve        (501) staff       (20)     8765 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/standard-token/with_bytecode_v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.675938 web3-6.4.0/ethpm/assets/vyper_registry/
+-rw-r--r--   0 eve        (501) staff       (20)    81363 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/vyper_registry/0.1.0.json
+-rw-r--r--   0 eve        (501) staff       (20)     6339 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/vyper_registry/registry.vy
+-rw-r--r--   0 eve        (501) staff       (20)     7596 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/assets/vyper_registry/registry_with_delete.vy
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.676555 web3-6.4.0/ethpm/backends/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/backends/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      956 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/backends/base.py
+-rw-r--r--   0 eve        (501) staff       (20)     3006 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/backends/http.py
+-rw-r--r--   0 eve        (501) staff       (20)     6551 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/backends/ipfs.py
+-rw-r--r--   0 eve        (501) staff       (20)     4174 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/backends/registry.py
+-rw-r--r--   0 eve        (501) staff       (20)      405 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/constants.py
+-rw-r--r--   0 eve        (501) staff       (20)     6256 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     1890 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/dependencies.py
+-rw-r--r--   0 eve        (501) staff       (20)     2134 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/deployments.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.658754 web3-6.4.0/ethpm/ethpm-spec/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.658568 web3-6.4.0/ethpm/ethpm-spec/examples/
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.677344 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/
+-rw-r--r--   0 eve        (501) staff       (20)     6810 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     5361 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.677656 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      888 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol
+-rw-r--r--   0 eve        (501) staff       (20)      644 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol
+-rw-r--r--   0 eve        (501) staff       (20)    11598 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     8669 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/escrow/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.678369 web3-6.4.0/ethpm/ethpm-spec/examples/owned/
+-rw-r--r--   0 eve        (501) staff       (20)      544 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      443 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/owned/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.678514 web3-6.4.0/ethpm/ethpm-spec/examples/owned/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      222 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/owned/contracts/Owned.sol
+-rw-r--r--   0 eve        (501) staff       (20)      728 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      478 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/owned/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.679097 web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/
+-rw-r--r--   0 eve        (501) staff       (20)     5272 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     5030 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json
+-rw-r--r--   0 eve        (501) staff       (20)     5220 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     4993 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.679781 web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/
+-rw-r--r--   0 eve        (501) staff       (20)     3976 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     3143 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.680021 web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      802 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol
+-rw-r--r--   0 eve        (501) staff       (20)     5517 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     3289 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.680663 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/
+-rw-r--r--   0 eve        (501) staff       (20)     3794 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     3238 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.680955 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     1155 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol
+-rw-r--r--   0 eve        (501) staff       (20)     2949 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol
+-rw-r--r--   0 eve        (501) staff       (20)    17129 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     6100 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.681821 web3-6.4.0/ethpm/ethpm-spec/examples/transferable/
+-rw-r--r--   0 eve        (501) staff       (20)      590 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      507 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/transferable/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.682076 web3-6.4.0/ethpm/ethpm-spec/examples/transferable/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      396 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/transferable/contracts/Transferable.sol
+-rw-r--r--   0 eve        (501) staff       (20)      786 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)      548 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/transferable/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.682889 web3-6.4.0/ethpm/ethpm-spec/examples/wallet/
+-rw-r--r--   0 eve        (501) staff       (20)     6669 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     5456 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.683794 web3-6.4.0/ethpm/ethpm-spec/examples/wallet/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)     1454 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol
+-rw-r--r--   0 eve        (501) staff       (20)     9710 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     7326 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.683534 web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/
+-rw-r--r--   0 eve        (501) staff       (20)     8052 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     6657 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.683667 web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/
+-rw-r--r--   0 eve        (501) staff       (20)      621 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol
+-rw-r--r--   0 eve        (501) staff       (20)    12191 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json
+-rw-r--r--   0 eve        (501) staff       (20)     9503 2022-04-27 21:13:00.000000 web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.684207 web3-6.4.0/ethpm/ethpm-spec/spec/
+-rw-r--r--   0 eve        (501) staff       (20)    10302 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/spec/package.spec.json
+-rw-r--r--   0 eve        (501) staff       (20)    12879 2021-02-11 20:53:14.000000 web3-6.4.0/ethpm/ethpm-spec/spec/v3.spec.json
+-rw-r--r--   0 eve        (501) staff       (20)     1194 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)    14493 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/package.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.684750 web3-6.4.0/ethpm/tools/
+-rw-r--r--   0 eve        (501) staff       (20)      103 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/tools/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    27045 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/tools/builder.py
+-rw-r--r--   0 eve        (501) staff       (20)    10373 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/tools/checker.py
+-rw-r--r--   0 eve        (501) staff       (20)      475 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/tools/get_manifest.py
+-rw-r--r--   0 eve        (501) staff       (20)     4368 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/uri.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.685594 web3-6.4.0/ethpm/validation/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/validation/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4716 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/validation/manifest.py
+-rw-r--r--   0 eve        (501) staff       (20)     1072 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/validation/misc.py
+-rw-r--r--   0 eve        (501) staff       (20)     2317 2023-04-06 21:34:13.000000 web3-6.4.0/ethpm/validation/package.py
+-rw-r--r--   0 eve        (501) staff       (20)     4873 2023-04-10 20:16:28.000000 web3-6.4.0/ethpm/validation/uri.py
+-rw-r--r--   0 eve        (501) staff       (20)     1202 2023-05-15 20:27:41.000000 web3-6.4.0/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-05-15 20:38:14.720762 web3-6.4.0/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     3168 2023-05-15 20:38:09.000000 web3-6.4.0/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.689267 web3-6.4.0/web3/
+-rw-r--r--   0 eve        (501) staff       (20)      752 2023-04-10 20:16:28.000000 web3-6.4.0/web3/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.696795 web3-6.4.0/web3/_utils/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    28771 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)      456 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/async_caching.py
+-rw-r--r--   0 eve        (501) staff       (20)     7693 2023-05-01 22:27:52.000000 web3-6.4.0/web3/_utils/async_transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)     2059 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/blocks.py
+-rw-r--r--   0 eve        (501) staff       (20)      992 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/caching.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.697333 web3-6.4.0/web3/_utils/compat/
+-rw-r--r--   0 eve        (501) staff       (20)      319 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/compat/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/compat/compat_py2.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/compat/compat_py3.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.697538 web3-6.4.0/web3/_utils/contract_sources/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/contract_sources/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     6406 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/contract_sources/compile_contracts.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.701533 web3-6.4.0/web3/_utils/contract_sources/contract_data/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      517 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py
+-rw-r--r--   0 eve        (501) staff       (20)     5344 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/address_reflector.py
+-rw-r--r--   0 eve        (501) staff       (20)    18852 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/arrays_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    14783 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     6089 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     6334 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py
+-rw-r--r--   0 eve        (501) staff       (20)    37881 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/emitter_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     5573 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/event_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)    15824 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/extended_resolver.py
+-rw-r--r--   0 eve        (501) staff       (20)     1651 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     7637 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/math_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    16716 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py
+-rw-r--r--   0 eve        (501) staff       (20)    32645 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/offchain_resolver.py
+-rw-r--r--   0 eve        (501) staff       (20)     1825 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/payable_tester.py
+-rw-r--r--   0 eve        (501) staff       (20)    17290 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/receive_function_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     5264 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     4264 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/revert_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)     3555 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/simple_resolver.py
+-rw-r--r--   0 eve        (501) staff       (20)    11586 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/string_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    23180 2023-05-15 20:27:41.000000 web3-6.4.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)    14980 2023-04-14 16:25:46.000000 web3-6.4.0/web3/_utils/contracts.py
+-rw-r--r--   0 eve        (501) staff       (20)     1640 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/datatypes.py
+-rw-r--r--   0 eve        (501) staff       (20)     1738 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/decorators.py
+-rw-r--r--   0 eve        (501) staff       (20)      144 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/empty.py
+-rw-r--r--   0 eve        (501) staff       (20)     9065 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)     2120 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/ens.py
+-rw-r--r--   0 eve        (501) staff       (20)    17134 2023-04-27 17:00:05.000000 web3-6.4.0/web3/_utils/events.py
+-rw-r--r--   0 eve        (501) staff       (20)     2113 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/fee_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)    11886 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/filters.py
+-rw-r--r--   0 eve        (501) staff       (20)     3071 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/formatters.py
+-rw-r--r--   0 eve        (501) staff       (20)       55 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/function_identifiers.py
+-rw-r--r--   0 eve        (501) staff       (20)      195 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/http.py
+-rw-r--r--   0 eve        (501) staff       (20)      209 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/hypothesis.py
+-rw-r--r--   0 eve        (501) staff       (20)     1047 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/math.py
+-rw-r--r--   0 eve        (501) staff       (20)    32977 2023-05-10 19:26:40.000000 web3-6.4.0/web3/_utils/method_formatters.py
+-rw-r--r--   0 eve        (501) staff       (20)     1146 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/miner.py
+-rw-r--r--   0 eve        (501) staff       (20)     3147 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.703134 web3-6.4.0/web3/_utils/module_testing/
+-rw-r--r--   0 eve        (501) staff       (20)      539 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module_testing/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)   166576 2023-05-10 19:26:40.000000 web3-6.4.0/web3/_utils/module_testing/eth_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     3406 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module_testing/go_ethereum_admin_module.py
+-rw-r--r--   0 eve        (501) staff       (20)    10338 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module_testing/go_ethereum_personal_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     1176 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module_testing/go_ethereum_txpool_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     4825 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module_testing/module_testing_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1272 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module_testing/net_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     9335 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/module_testing/web3_module.py
+-rw-r--r--   0 eve        (501) staff       (20)     6493 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/normalizers.py
+-rw-r--r--   0 eve        (501) staff       (20)     8833 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/request.py
+-rw-r--r--   0 eve        (501) staff       (20)     9449 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/rpc_abi.py
+-rw-r--r--   0 eve        (501) staff       (20)     4207 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/threads.py
+-rw-r--r--   0 eve        (501) staff       (20)     8737 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/transactions.py
+-rw-r--r--   0 eve        (501) staff       (20)      816 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/type_conversion.py
+-rw-r--r--   0 eve        (501) staff       (20)     1669 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/utility_methods.py
+-rw-r--r--   0 eve        (501) staff       (20)     6291 2023-04-10 20:16:28.000000 web3-6.4.0/web3/_utils/validation.py
+-rw-r--r--   0 eve        (501) staff       (20)      994 2023-04-06 21:34:13.000000 web3-6.4.0/web3/_utils/windows.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.703396 web3-6.4.0/web3/auto/
+-rw-r--r--   0 eve        (501) staff       (20)       44 2023-04-10 20:16:28.000000 web3-6.4.0/web3/auto/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      263 2023-04-06 21:34:13.000000 web3-6.4.0/web3/auto/gethdev.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.703904 web3-6.4.0/web3/beacon/
+-rw-r--r--   0 eve        (501) staff       (20)       91 2023-04-10 20:16:28.000000 web3-6.4.0/web3/beacon/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1516 2023-04-06 21:34:13.000000 web3-6.4.0/web3/beacon/api_endpoints.py
+-rw-r--r--   0 eve        (501) staff       (20)     5421 2023-04-06 21:34:13.000000 web3-6.4.0/web3/beacon/async_beacon.py
+-rw-r--r--   0 eve        (501) staff       (20)     4772 2023-04-06 21:34:13.000000 web3-6.4.0/web3/beacon/main.py
+-rw-r--r--   0 eve        (501) staff       (20)      396 2023-04-06 21:34:13.000000 web3-6.4.0/web3/constants.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.708614 web3-6.4.0/web3/contract/
+-rw-r--r--   0 eve        (501) staff       (20)      215 2023-04-10 20:16:28.000000 web3-6.4.0/web3/contract/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    19756 2023-04-10 20:16:28.000000 web3-6.4.0/web3/contract/async_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    35710 2023-04-10 20:16:28.000000 web3-6.4.0/web3/contract/base_contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    18804 2023-04-10 20:16:28.000000 web3-6.4.0/web3/contract/contract.py
+-rw-r--r--   0 eve        (501) staff       (20)    12338 2023-04-20 16:31:09.000000 web3-6.4.0/web3/contract/utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     9104 2023-05-15 20:27:41.000000 web3-6.4.0/web3/datastructures.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.710993 web3-6.4.0/web3/eth/
+-rw-r--r--   0 eve        (501) staff       (20)      166 2023-04-10 20:16:28.000000 web3-6.4.0/web3/eth/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    20181 2023-05-10 19:26:40.000000 web3-6.4.0/web3/eth/async_eth.py
+-rw-r--r--   0 eve        (501) staff       (20)     5943 2023-04-10 20:16:28.000000 web3-6.4.0/web3/eth/base_eth.py
+-rw-r--r--   0 eve        (501) staff       (20)    19295 2023-05-01 22:35:55.000000 web3-6.4.0/web3/eth/eth.py
+-rw-r--r--   0 eve        (501) staff       (20)     6238 2023-05-01 18:21:29.000000 web3-6.4.0/web3/exceptions.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.711717 web3-6.4.0/web3/gas_strategies/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/gas_strategies/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      430 2023-04-10 20:16:28.000000 web3-6.4.0/web3/gas_strategies/rpc.py
+-rw-r--r--   0 eve        (501) staff       (20)     9010 2023-04-10 20:16:28.000000 web3-6.4.0/web3/gas_strategies/time_based.py
+-rw-r--r--   0 eve        (501) staff       (20)    11826 2023-04-10 20:16:28.000000 web3-6.4.0/web3/geth.py
+-rw-r--r--   0 eve        (501) staff       (20)      198 2023-04-06 21:34:13.000000 web3-6.4.0/web3/logs.py
+-rw-r--r--   0 eve        (501) staff       (20)    12774 2023-04-27 17:00:05.000000 web3-6.4.0/web3/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     7875 2023-04-10 20:16:28.000000 web3-6.4.0/web3/manager.py
+-rw-r--r--   0 eve        (501) staff       (20)     8430 2023-04-06 21:34:13.000000 web3-6.4.0/web3/method.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.714909 web3-6.4.0/web3/middleware/
+-rw-r--r--   0 eve        (501) staff       (20)     3724 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      239 2023-04-06 21:34:13.000000 web3-6.4.0/web3/middleware/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)     2755 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/async_cache.py
+-rw-r--r--   0 eve        (501) staff       (20)     1779 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/attrdict.py
+-rw-r--r--   0 eve        (501) staff       (20)     1785 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/buffered_gas_estimate.py
+-rw-r--r--   0 eve        (501) staff       (20)    12617 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/cache.py
+-rw-r--r--   0 eve        (501) staff       (20)     1167 2023-04-06 21:34:13.000000 web3-6.4.0/web3/middleware/exception_handling.py
+-rw-r--r--   0 eve        (501) staff       (20)     3119 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/exception_retry_request.py
+-rw-r--r--   0 eve        (501) staff       (20)    21131 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/filter.py
+-rw-r--r--   0 eve        (501) staff       (20)     4596 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/fixture.py
+-rw-r--r--   0 eve        (501) staff       (20)     4762 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/formatting.py
+-rw-r--r--   0 eve        (501) staff       (20)     4212 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/gas_price_strategy.py
+-rw-r--r--   0 eve        (501) staff       (20)     1657 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/geth_poa.py
+-rw-r--r--   0 eve        (501) staff       (20)      590 2023-04-06 21:34:13.000000 web3-6.4.0/web3/middleware/names.py
+-rw-r--r--   0 eve        (501) staff       (20)      246 2023-04-06 21:34:13.000000 web3-6.4.0/web3/middleware/normalize_request_parameters.py
+-rw-r--r--   0 eve        (501) staff       (20)      351 2023-04-06 21:34:13.000000 web3-6.4.0/web3/middleware/pythonic.py
+-rw-r--r--   0 eve        (501) staff       (20)     4450 2023-04-06 21:34:13.000000 web3-6.4.0/web3/middleware/signing.py
+-rw-r--r--   0 eve        (501) staff       (20)     1014 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/simulate_unmined_transaction.py
+-rw-r--r--   0 eve        (501) staff       (20)     3739 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/stalecheck.py
+-rw-r--r--   0 eve        (501) staff       (20)     4573 2023-04-10 20:16:28.000000 web3-6.4.0/web3/middleware/validation.py
+-rw-r--r--   0 eve        (501) staff       (20)     3615 2023-04-10 20:16:28.000000 web3-6.4.0/web3/module.py
+-rw-r--r--   0 eve        (501) staff       (20)     1562 2023-04-06 21:34:13.000000 web3-6.4.0/web3/net.py
+-rw-r--r--   0 eve        (501) staff       (20)    21609 2023-04-10 20:16:28.000000 web3-6.4.0/web3/pm.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.716586 web3-6.4.0/web3/providers/
+-rw-r--r--   0 eve        (501) staff       (20)      368 2023-04-06 21:34:13.000000 web3-6.4.0/web3/providers/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4178 2023-04-27 17:00:05.000000 web3-6.4.0/web3/providers/async_base.py
+-rw-r--r--   0 eve        (501) staff       (20)     2469 2023-04-06 21:34:13.000000 web3-6.4.0/web3/providers/async_rpc.py
+-rw-r--r--   0 eve        (501) staff       (20)     3447 2023-04-27 17:00:05.000000 web3-6.4.0/web3/providers/auto.py
+-rw-r--r--   0 eve        (501) staff       (20)     4111 2023-04-27 17:00:05.000000 web3-6.4.0/web3/providers/base.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.717356 web3-6.4.0/web3/providers/eth_tester/
+-rw-r--r--   0 eve        (501) staff       (20)       97 2023-04-10 20:16:28.000000 web3-6.4.0/web3/providers/eth_tester/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)    14397 2023-05-01 18:21:29.000000 web3-6.4.0/web3/providers/eth_tester/defaults.py
+-rw-r--r--   0 eve        (501) staff       (20)     5512 2023-04-27 17:00:05.000000 web3-6.4.0/web3/providers/eth_tester/main.py
+-rw-r--r--   0 eve        (501) staff       (20)    12861 2023-05-15 20:27:41.000000 web3-6.4.0/web3/providers/eth_tester/middleware.py
+-rw-r--r--   0 eve        (501) staff       (20)     6533 2023-04-27 17:00:05.000000 web3-6.4.0/web3/providers/ipc.py
+-rw-r--r--   0 eve        (501) staff       (20)     2686 2023-04-06 21:34:13.000000 web3-6.4.0/web3/providers/rpc.py
+-rw-r--r--   0 eve        (501) staff       (20)     3919 2023-04-06 21:34:13.000000 web3-6.4.0/web3/providers/websocket.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.717484 web3-6.4.0/web3/scripts/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/scripts/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.717652 web3-6.4.0/web3/scripts/release/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/scripts/release/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     1534 2023-04-06 21:34:13.000000 web3-6.4.0/web3/scripts/release/test_package.py
+-rw-r--r--   0 eve        (501) staff       (20)      951 2023-04-06 21:34:13.000000 web3-6.4.0/web3/testing.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.717791 web3-6.4.0/web3/tools/
+-rw-r--r--   0 eve        (501) staff       (20)       73 2023-04-06 21:34:13.000000 web3-6.4.0/web3/tools/__init__.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.718655 web3-6.4.0/web3/tools/benchmark/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/tools/benchmark/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     5886 2023-04-10 20:16:28.000000 web3-6.4.0/web3/tools/benchmark/main.py
+-rw-r--r--   0 eve        (501) staff       (20)     3435 2023-04-10 20:16:28.000000 web3-6.4.0/web3/tools/benchmark/node.py
+-rw-r--r--   0 eve        (501) staff       (20)      912 2023-04-06 21:34:13.000000 web3-6.4.0/web3/tools/benchmark/reporting.py
+-rw-r--r--   0 eve        (501) staff       (20)     1722 2023-04-06 21:34:13.000000 web3-6.4.0/web3/tools/benchmark/utils.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.719608 web3-6.4.0/web3/tools/pytest_ethereum/
+-rw-r--r--   0 eve        (501) staff       (20)        0 2023-04-06 21:34:13.000000 web3-6.4.0/web3/tools/pytest_ethereum/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)     4158 2023-04-10 20:16:28.000000 web3-6.4.0/web3/tools/pytest_ethereum/_utils.py
+-rw-r--r--   0 eve        (501) staff       (20)     1423 2023-04-10 20:16:28.000000 web3-6.4.0/web3/tools/pytest_ethereum/deployer.py
+-rw-r--r--   0 eve        (501) staff       (20)      380 2023-04-06 21:34:13.000000 web3-6.4.0/web3/tools/pytest_ethereum/exceptions.py
+-rw-r--r--   0 eve        (501) staff       (20)     3927 2023-04-06 21:34:13.000000 web3-6.4.0/web3/tools/pytest_ethereum/linker.py
+-rw-r--r--   0 eve        (501) staff       (20)      645 2023-04-10 20:16:28.000000 web3-6.4.0/web3/tools/pytest_ethereum/plugins.py
+-rw-r--r--   0 eve        (501) staff       (20)     2968 2023-04-14 17:20:25.000000 web3-6.4.0/web3/tracing.py
+-rw-r--r--   0 eve        (501) staff       (20)    10909 2023-05-15 20:27:41.000000 web3-6.4.0/web3/types.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.720379 web3-6.4.0/web3/utils/
+-rw-r--r--   0 eve        (501) staff       (20)      454 2023-04-06 21:34:13.000000 web3-6.4.0/web3/utils/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)      498 2023-04-06 21:34:13.000000 web3-6.4.0/web3/utils/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)      967 2023-04-06 21:34:13.000000 web3-6.4.0/web3/utils/address.py
+-rw-r--r--   0 eve        (501) staff       (20)     3096 2023-04-06 21:34:13.000000 web3-6.4.0/web3/utils/async_exception_handling.py
+-rw-r--r--   0 eve        (501) staff       (20)     1521 2023-04-06 21:34:13.000000 web3-6.4.0/web3/utils/caching.py
+-rw-r--r--   0 eve        (501) staff       (20)     3052 2023-04-06 21:34:13.000000 web3-6.4.0/web3/utils/exception_handling.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-05-15 20:38:14.690098 web3-6.4.0/web3.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     2184 2023-05-15 20:38:14.000000 web3-6.4.0/web3.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     9743 2023-05-15 20:38:14.000000 web3-6.4.0/web3.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-05-15 20:38:14.000000 web3-6.4.0/web3.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)       64 2023-05-15 20:38:14.000000 web3-6.4.0/web3.egg-info/entry_points.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-05-15 20:38:14.000000 web3-6.4.0/web3.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)     1165 2023-05-15 20:38:14.000000 web3-6.4.0/web3.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)       15 2023-05-15 20:38:14.000000 web3-6.4.0/web3.egg-info/top_level.txt
```

### Comparing `web3-6.3.0/LICENSE` & `web3-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/PKG-INFO` & `web3-6.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.3.0
+Version: 6.4.0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.3.0/README.md` & `web3-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/abis.py` & `web3-6.4.0/ens/abis.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/async_ens.py` & `web3-6.4.0/ens/async_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/base_ens.py` & `web3-6.4.0/ens/base_ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/constants.py` & `web3-6.4.0/ens/constants.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/contract_data.py` & `web3-6.4.0/ens/contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/ens.py` & `web3-6.4.0/ens/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/exceptions.py` & `web3-6.4.0/ens/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ens/utils.py` & `web3-6.4.0/ens/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/__init__.py` & `web3-6.4.0/ethpm/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,17 @@
+import warnings
 from pathlib import Path
 
 
+warnings.warn(
+    "The ``ethPM`` module is no longer being maintained and will be "
+    "deprecated with ``web3.py`` version 7",
+    UserWarning,
+)
+
 ETHPM_DIR = Path(__file__).parent
 ASSETS_DIR = ETHPM_DIR / "assets"
 
 
 def get_ethpm_spec_dir() -> Path:
     ethpm_spec_dir = ETHPM_DIR / "ethpm-spec"
     v3_spec = ethpm_spec_dir / "spec" / "v3.spec.json"
```

### Comparing `web3-6.3.0/ethpm/_utils/backend.py` & `web3-6.4.0/ethpm/_utils/backend.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/_utils/cache.py` & `web3-6.4.0/ethpm/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/_utils/chains.py` & `web3-6.4.0/ethpm/_utils/chains.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/_utils/contract.py` & `web3-6.4.0/ethpm/_utils/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/_utils/deployments.py` & `web3-6.4.0/ethpm/_utils/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/_utils/ipfs.py` & `web3-6.4.0/ethpm/_utils/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/_utils/protobuf/ipfs_file_pb2.py` & `web3-6.4.0/ethpm/_utils/protobuf/ipfs_file_pb2.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/_utils/registry.py` & `web3-6.4.0/ethpm/_utils/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/ens/v3.json` & `web3-6.4.0/ethpm/assets/ens/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/escrow/with_bytecode_v3.json` & `web3-6.4.0/ethpm/assets/escrow/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/ipfs_file.proto` & `web3-6.4.0/ethpm/assets/ipfs_file.proto`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/owned/output_v3.json` & `web3-6.4.0/ethpm/assets/owned/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/owned/with_contract_type_v3.json` & `web3-6.4.0/ethpm/assets/owned/with_contract_type_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/contracts/Authority.sol` & `web3-6.4.0/ethpm/assets/registry/contracts/Authority.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol` & `web3-6.4.0/ethpm/assets/registry/contracts/IndexedOrderedSetLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/contracts/PackageDB.sol` & `web3-6.4.0/ethpm/assets/registry/contracts/PackageDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/contracts/PackageRegistry.sol` & `web3-6.4.0/ethpm/assets/registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol` & `web3-6.4.0/ethpm/assets/registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/contracts/ReleaseDB.sol` & `web3-6.4.0/ethpm/assets/registry/contracts/ReleaseDB.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/contracts/ReleaseValidator.sol` & `web3-6.4.0/ethpm/assets/registry/contracts/ReleaseValidator.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/solc_input.json` & `web3-6.4.0/ethpm/assets/registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/solc_output.json` & `web3-6.4.0/ethpm/assets/registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/registry/v3.json` & `web3-6.4.0/ethpm/assets/registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json` & `web3-6.4.0/ethpm/assets/safe-math-lib/v3-strict-no-deployments.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/simple-registry/contracts/Ownable.sol` & `web3-6.4.0/ethpm/assets/simple-registry/contracts/Ownable.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol` & `web3-6.4.0/ethpm/assets/simple-registry/contracts/PackageRegistry.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol` & `web3-6.4.0/ethpm/assets/simple-registry/contracts/PackageRegistryInterface.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/simple-registry/solc_input.json` & `web3-6.4.0/ethpm/assets/simple-registry/solc_input.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/simple-registry/solc_output.json` & `web3-6.4.0/ethpm/assets/simple-registry/solc_output.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/simple-registry/v3.json` & `web3-6.4.0/ethpm/assets/simple-registry/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/standard-token/output_v3.json` & `web3-6.4.0/ethpm/assets/standard-token/output_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/standard-token/with_bytecode_v3.json` & `web3-6.4.0/ethpm/assets/standard-token/with_bytecode_v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/vyper_registry/0.1.0.json` & `web3-6.4.0/ethpm/assets/vyper_registry/0.1.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/vyper_registry/registry.vy` & `web3-6.4.0/ethpm/assets/vyper_registry/registry.vy`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/assets/vyper_registry/registry_with_delete.vy` & `web3-6.4.0/ethpm/assets/vyper_registry/registry_with_delete.vy`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/backends/base.py` & `web3-6.4.0/ethpm/backends/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/backends/http.py` & `web3-6.4.0/ethpm/backends/http.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/backends/ipfs.py` & `web3-6.4.0/ethpm/backends/ipfs.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/backends/registry.py` & `web3-6.4.0/ethpm/backends/registry.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/contract.py` & `web3-6.4.0/ethpm/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/dependencies.py` & `web3-6.4.0/ethpm/dependencies.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/deployments.py` & `web3-6.4.0/ethpm/deployments.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/escrow/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/escrow/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol` & `web3-6.4.0/ethpm/ethpm-spec/examples/escrow/contracts/Escrow.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol` & `web3-6.4.0/ethpm/ethpm-spec/examples/escrow/contracts/SafeSendLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/escrow/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/escrow/v3.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/escrow/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/owned/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/owned/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/piper-coin/v3.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/piper-coin/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol` & `web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/contracts/SafeMathLib.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/safe-math-lib/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol` & `web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/contracts/AbstractToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol` & `web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/contracts/StandardToken.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/standard-token/v3.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/standard-token/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/transferable/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/transferable/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/transferable/v3.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/transferable/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet/contracts/Wallet.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet/v3.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/1.0.0.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/contracts/WalletWithSend.sol`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/v3-pretty.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json` & `web3-6.4.0/ethpm/ethpm-spec/examples/wallet-with-send/v3.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/spec/package.spec.json` & `web3-6.4.0/ethpm/ethpm-spec/spec/package.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/ethpm-spec/spec/v3.spec.json` & `web3-6.4.0/ethpm/ethpm-spec/spec/v3.spec.json`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/exceptions.py` & `web3-6.4.0/ethpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/package.py` & `web3-6.4.0/ethpm/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/tools/builder.py` & `web3-6.4.0/ethpm/tools/builder.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/tools/checker.py` & `web3-6.4.0/ethpm/tools/checker.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/uri.py` & `web3-6.4.0/ethpm/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/validation/manifest.py` & `web3-6.4.0/ethpm/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/validation/misc.py` & `web3-6.4.0/ethpm/validation/misc.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/validation/package.py` & `web3-6.4.0/ethpm/validation/package.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/ethpm/validation/uri.py` & `web3-6.4.0/ethpm/validation/uri.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/setup.py` & `web3-6.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from setuptools import (
     find_packages,
     setup,
 )
 
 extras_require = {
     "tester": [
-        "eth-tester[py-evm]==v0.8.0-b.3",
+        "eth-tester[py-evm]==v0.9.0-b.1",
         "py-geth>=3.11.0",
     ],
     "linter": [
         "black>=22.1.0",
         "flake8==3.8.3",
         "isort>=5.11.0",
         "mypy==0.910",
         "types-setuptools>=57.4.4",
         "types-requests>=2.26.1",
         "types-protobuf==3.19.13",
     ],
     "docs": [
-        "sphinx>=5.0.0",
+        "sphinx>=5.3.0",
         "sphinx_rtd_theme>=1.0.0",
         "towncrier>=21,<22",
     ],
     "dev": [
         "bumpversion",
         "flaky>=3.7.0",
         "hypothesis>=3.31.2",
@@ -56,15 +56,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="web3",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="6.3.0",
+    version="6.4.0",
     description="""web3.py""",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Piper Merriam",
     author_email="pipermerriam@gmail.com",
     url="https://github.com/ethereum/web3.py",
     include_package_data=True,
```

### Comparing `web3-6.3.0/web3/__init__.py` & `web3-6.4.0/web3/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/abi.py` & `web3-6.4.0/web3/_utils/abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/async_transactions.py` & `web3-6.4.0/web3/_utils/async_transactions.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/blocks.py` & `web3-6.4.0/web3/_utils/blocks.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/caching.py` & `web3-6.4.0/web3/_utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/contract_sources/compile_contracts.py` & `web3-6.4.0/web3/_utils/contract_sources/compile_contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/_custom_contract_data.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/address_reflector.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/address_reflector.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/bytes_contracts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/BytesContracts.sol:BytesContract
-BYTES_CONTRACT_BYTECODE = "0x60806040526040518060400160405280600281526020017f0123000000000000000000000000000000000000000000000000000000000000815250600090816200004a919062000311565b503480156200005857600080fd5b5060405162000de638038062000de683398181016040528101906200007e91906200055c565b80600190816200008f9190620005b8565b50506200069f565b600081519050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602260045260246000fd5b600060028204905060018216806200011957607f821691505b6020821081036200012f576200012e620000d1565b5b50919050565b60008190508160005260206000209050919050565b60006020601f8301049050919050565b600082821b905092915050565b600060088302620001997fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff826200015a565b620001a586836200015a565b95508019841693508086168417925050509392505050565b6000819050919050565b6000819050919050565b6000620001f2620001ec620001e684620001bd565b620001c7565b620001bd565b9050919050565b6000819050919050565b6200020e83620001d1565b620002266200021d82620001f9565b84845462000167565b825550505050565b600090565b6200023d6200022e565b6200024a81848462000203565b505050565b5b8181101562000272576200026660008262000233565b60018101905062000250565b5050565b601f821115620002c1576200028b8162000135565b62000296846200014a565b81016020851015620002a6578190505b620002be620002b5856200014a565b8301826200024f565b50505b505050565b600082821c905092915050565b6000620002e660001984600802620002c6565b1980831691505092915050565b6000620003018383620002d3565b9150826002028217905092915050565b6200031c8262000097565b67ffffffffffffffff811115620003385762000337620000a2565b5b62000344825462000100565b6200035182828562000276565b600060209050601f83116001811462000389576000841562000374578287015190505b620003808582620002f3565b865550620003f0565b601f198416620003998662000135565b60005b82811015620003c3578489015182556001820191506020850194506020810190506200039c565b86831015620003e35784890151620003df601f891682620002d3565b8355505b6001600288020188555050505b505050505050565b6000604051905090565b600080fd5b600080fd5b600080fd5b600080fd5b6000601f19601f8301169050919050565b620004328262000416565b810181811067ffffffffffffffff82111715620004545762000453620000a2565b5b80604052505050565b600062000469620003f8565b905062000477828262000427565b919050565b600067ffffffffffffffff8211156200049a5762000499620000a2565b5b620004a58262000416565b9050602081019050919050565b60005b83811015620004d2578082015181840152602081019050620004b5565b60008484015250505050565b6000620004f5620004ef846200047c565b6200045d565b90508281526020810184848401111562000514576200051362000411565b5b62000521848285620004b2565b509392505050565b600082601f8301126200054157620005406200040c565b5b815162000553848260208601620004de565b91505092915050565b60006020828403121562000575576200057462000402565b5b600082015167ffffffffffffffff81111562000596576200059562000407565b5b620005a48482850162000529565b91505092915050565b600081519050919050565b620005c382620005ad565b67ffffffffffffffff811115620005df57620005de620000a2565b5b620005eb825462000100565b620005f882828562000276565b600060209050601f8311600181146200063057600084156200061b578287015190505b620006278582620002f3565b86555062000697565b601f198416620006408662000135565b60005b828110156200066a5784890151825560018201915060208501945060208101905062000643565b868310156200068a578489015162000686601f891682620002d3565b8355505b6001600288020188555050505b505050505050565b61073780620006af6000396000f3fe608060405234801561001057600080fd5b50600436106100415760003560e01c8063209652551461004657806330de3cee14610064578063439970aa14610082575b600080fd5b61004e61009e565b60405161005b9190610265565b60405180910390f35b61006c610130565b6040516100799190610265565b60405180910390f35b61009c600480360381019061009791906103d0565b6101c2565b005b6060600180546100ad90610448565b80601f01602080910402602001604051908101604052809291908181526020018280546100d990610448565b80156101265780601f106100fb57610100808354040283529160200191610126565b820191906000526020600020905b81548152906001019060200180831161010957829003601f168201915b5050505050905090565b60606000805461013f90610448565b80601f016020809104026020016040519081016040528092919081815260200182805461016b90610448565b80156101b85780601f1061018d576101008083540402835291602001916101b8565b820191906000526020600020905b81548152906001019060200180831161019b57829003601f168201915b5050505050905090565b80600190816101d1919061062f565b5050565b600081519050919050565b600082825260208201905092915050565b60005b8381101561020f5780820151818401526020810190506101f4565b60008484015250505050565b6000601f19601f8301169050919050565b6000610237826101d5565b61024181856101e0565b93506102518185602086016101f1565b61025a8161021b565b840191505092915050565b6000602082019050818103600083015261027f818461022c565b905092915050565b6000604051905090565b600080fd5b600080fd5b600080fd5b600080fd5b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b6102dd8261021b565b810181811067ffffffffffffffff821117156102fc576102fb6102a5565b5b80604052505050565b600061030f610287565b905061031b82826102d4565b919050565b600067ffffffffffffffff82111561033b5761033a6102a5565b5b6103448261021b565b9050602081019050919050565b82818337600083830152505050565b600061037361036e84610320565b610305565b90508281526020810184848401111561038f5761038e6102a0565b5b61039a848285610351565b509392505050565b600082601f8301126103b7576103b661029b565b5b81356103c7848260208601610360565b91505092915050565b6000602082840312156103e6576103e5610291565b5b600082013567ffffffffffffffff81111561040457610403610296565b5b610410848285016103a2565b91505092915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602260045260246000fd5b6000600282049050600182168061046057607f821691505b60208210810361047357610472610419565b5b50919050565b60008190508160005260206000209050919050565b60006020601f8301049050919050565b600082821b905092915050565b6000600883026104db7fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff8261049e565b6104e5868361049e565b95508019841693508086168417925050509392505050565b6000819050919050565b6000819050919050565b600061052c610527610522846104fd565b610507565b6104fd565b9050919050565b6000819050919050565b61054683610511565b61055a61055282610533565b8484546104ab565b825550505050565b600090565b61056f610562565b61057a81848461053d565b505050565b5b8181101561059e57610593600082610567565b600181019050610580565b5050565b601f8211156105e3576105b481610479565b6105bd8461048e565b810160208510156105cc578190505b6105e06105d88561048e565b83018261057f565b50505b505050565b600082821c905092915050565b6000610606600019846008026105e8565b1980831691505092915050565b600061061f83836105f5565b9150826002028217905092915050565b610638826101d5565b67ffffffffffffffff811115610651576106506102a5565b5b61065b8254610448565b6106668282856105a2565b600060209050601f8311600181146106995760008415610687578287015190505b6106918582610613565b8655506106f9565b601f1984166106a786610479565b60005b828110156106cf578489015182556001820191506020850194506020810190506106aa565b868310156106ec57848901516106e8601f8916826105f5565b8355505b6001600288020188555050505b50505050505056fea2646970667358221220c5a150a475addd26c4cd9d9204d977fc0c35b4469324383a14761aee10349fc264736f6c63430008130033"  # noqa: E501
-BYTES_CONTRACT_RUNTIME = "0x608060405234801561001057600080fd5b50600436106100415760003560e01c8063209652551461004657806330de3cee14610064578063439970aa14610082575b600080fd5b61004e61009e565b60405161005b9190610265565b60405180910390f35b61006c610130565b6040516100799190610265565b60405180910390f35b61009c600480360381019061009791906103d0565b6101c2565b005b6060600180546100ad90610448565b80601f01602080910402602001604051908101604052809291908181526020018280546100d990610448565b80156101265780601f106100fb57610100808354040283529160200191610126565b820191906000526020600020905b81548152906001019060200180831161010957829003601f168201915b5050505050905090565b60606000805461013f90610448565b80601f016020809104026020016040519081016040528092919081815260200182805461016b90610448565b80156101b85780601f1061018d576101008083540402835291602001916101b8565b820191906000526020600020905b81548152906001019060200180831161019b57829003601f168201915b5050505050905090565b80600190816101d1919061062f565b5050565b600081519050919050565b600082825260208201905092915050565b60005b8381101561020f5780820151818401526020810190506101f4565b60008484015250505050565b6000601f19601f8301169050919050565b6000610237826101d5565b61024181856101e0565b93506102518185602086016101f1565b61025a8161021b565b840191505092915050565b6000602082019050818103600083015261027f818461022c565b905092915050565b6000604051905090565b600080fd5b600080fd5b600080fd5b600080fd5b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b6102dd8261021b565b810181811067ffffffffffffffff821117156102fc576102fb6102a5565b5b80604052505050565b600061030f610287565b905061031b82826102d4565b919050565b600067ffffffffffffffff82111561033b5761033a6102a5565b5b6103448261021b565b9050602081019050919050565b82818337600083830152505050565b600061037361036e84610320565b610305565b90508281526020810184848401111561038f5761038e6102a0565b5b61039a848285610351565b509392505050565b600082601f8301126103b7576103b661029b565b5b81356103c7848260208601610360565b91505092915050565b6000602082840312156103e6576103e5610291565b5b600082013567ffffffffffffffff81111561040457610403610296565b5b610410848285016103a2565b91505092915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602260045260246000fd5b6000600282049050600182168061046057607f821691505b60208210810361047357610472610419565b5b50919050565b60008190508160005260206000209050919050565b60006020601f8301049050919050565b600082821b905092915050565b6000600883026104db7fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff8261049e565b6104e5868361049e565b95508019841693508086168417925050509392505050565b6000819050919050565b6000819050919050565b600061052c610527610522846104fd565b610507565b6104fd565b9050919050565b6000819050919050565b61054683610511565b61055a61055282610533565b8484546104ab565b825550505050565b600090565b61056f610562565b61057a81848461053d565b505050565b5b8181101561059e57610593600082610567565b600181019050610580565b5050565b601f8211156105e3576105b481610479565b6105bd8461048e565b810160208510156105cc578190505b6105e06105d88561048e565b83018261057f565b50505b505050565b600082821c905092915050565b6000610606600019846008026105e8565b1980831691505092915050565b600061061f83836105f5565b9150826002028217905092915050565b610638826101d5565b67ffffffffffffffff811115610651576106506102a5565b5b61065b8254610448565b6106668282856105a2565b600060209050601f8311600181146106995760008415610687578287015190505b6106918582610613565b8655506106f9565b601f1984166106a786610479565b60005b828110156106cf578489015182556001820191506020850194506020810190506106aa565b868310156106ec57848901516106e8601f8916826105f5565b8355505b6001600288020188555050505b50505050505056fea2646970667358221220c5a150a475addd26c4cd9d9204d977fc0c35b4469324383a14761aee10349fc264736f6c63430008130033"  # noqa: E501
+BYTES_CONTRACT_BYTECODE = "0x60806040526040518060400160405280600281526020017f01230000000000000000000000000000000000000000000000000000000000008152505f9081620000499190620002f9565b5034801562000056575f80fd5b5060405162000d8338038062000d8383398181016040528101906200007c919062000535565b80600190816200008d91906200058e565b505062000672565b5f81519050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602260045260245ffd5b5f60028204905060018216806200011157607f821691505b602082108103620001275762000126620000cc565b5b50919050565b5f819050815f5260205f209050919050565b5f6020601f8301049050919050565b5f82821b905092915050565b5f600883026200018b7fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff826200014e565b6200019786836200014e565b95508019841693508086168417925050509392505050565b5f819050919050565b5f819050919050565b5f620001e1620001db620001d584620001af565b620001b8565b620001af565b9050919050565b5f819050919050565b620001fc83620001c1565b620002146200020b82620001e8565b8484546200015a565b825550505050565b5f90565b6200022a6200021c565b62000237818484620001f1565b505050565b5b818110156200025e57620002525f8262000220565b6001810190506200023d565b5050565b601f821115620002ad5762000277816200012d565b62000282846200013f565b8101602085101562000292578190505b620002aa620002a1856200013f565b8301826200023c565b50505b505050565b5f82821c905092915050565b5f620002cf5f1984600802620002b2565b1980831691505092915050565b5f620002e98383620002be565b9150826002028217905092915050565b620003048262000095565b67ffffffffffffffff81111562000320576200031f6200009f565b5b6200032c8254620000f9565b6200033982828562000262565b5f60209050601f8311600181146200036f575f84156200035a578287015190505b620003668582620002dc565b865550620003d5565b601f1984166200037f866200012d565b5f5b82811015620003a85784890151825560018201915060208501945060208101905062000381565b86831015620003c85784890151620003c4601f891682620002be565b8355505b6001600288020188555050505b505050505050565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f80fd5b5f601f19601f8301169050919050565b6200041182620003f6565b810181811067ffffffffffffffff821117156200043357620004326200009f565b5b80604052505050565b5f62000447620003dd565b905062000455828262000406565b919050565b5f67ffffffffffffffff8211156200047757620004766200009f565b5b6200048282620003f6565b9050602081019050919050565b5f5b83811015620004ae57808201518184015260208101905062000491565b5f8484015250505050565b5f620004cf620004c9846200045a565b6200043c565b905082815260208101848484011115620004ee57620004ed620003f2565b5b620004fb8482856200048f565b509392505050565b5f82601f8301126200051a5762000519620003ee565b5b81516200052c848260208601620004b9565b91505092915050565b5f602082840312156200054d576200054c620003e6565b5b5f82015167ffffffffffffffff8111156200056d576200056c620003ea565b5b6200057b8482850162000503565b91505092915050565b5f81519050919050565b620005998262000584565b67ffffffffffffffff811115620005b557620005b46200009f565b5b620005c18254620000f9565b620005ce82828562000262565b5f60209050601f83116001811462000604575f8415620005ef578287015190505b620005fb8582620002dc565b8655506200066a565b601f19841662000614866200012d565b5f5b828110156200063d5784890151825560018201915060208501945060208101905062000616565b868310156200065d578489015162000659601f891682620002be565b8355505b6001600288020188555050505b505050505050565b61070380620006805f395ff3fe608060405234801561000f575f80fd5b506004361061003f575f3560e01c8063209652551461004357806330de3cee14610061578063439970aa1461007f575b5f80fd5b61004b61009b565b6040516100589190610257565b60405180910390f35b61006961012b565b6040516100769190610257565b60405180910390f35b610099600480360381019061009491906103b4565b6101ba565b005b6060600180546100aa90610428565b80601f01602080910402602001604051908101604052809291908181526020018280546100d690610428565b80156101215780601f106100f857610100808354040283529160200191610121565b820191905f5260205f20905b81548152906001019060200180831161010457829003601f168201915b5050505050905090565b60605f805461013990610428565b80601f016020809104026020016040519081016040528092919081815260200182805461016590610428565b80156101b05780601f10610187576101008083540402835291602001916101b0565b820191905f5260205f20905b81548152906001019060200180831161019357829003601f168201915b5050505050905090565b80600190816101c991906105fe565b5050565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156102045780820151818401526020810190506101e9565b5f8484015250505050565b5f601f19601f8301169050919050565b5f610229826101cd565b61023381856101d7565b93506102438185602086016101e7565b61024c8161020f565b840191505092915050565b5f6020820190508181035f83015261026f818461021f565b905092915050565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f80fd5b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6102c68261020f565b810181811067ffffffffffffffff821117156102e5576102e4610290565b5b80604052505050565b5f6102f7610277565b905061030382826102bd565b919050565b5f67ffffffffffffffff82111561032257610321610290565b5b61032b8261020f565b9050602081019050919050565b828183375f83830152505050565b5f61035861035384610308565b6102ee565b9050828152602081018484840111156103745761037361028c565b5b61037f848285610338565b509392505050565b5f82601f83011261039b5761039a610288565b5b81356103ab848260208601610346565b91505092915050565b5f602082840312156103c9576103c8610280565b5b5f82013567ffffffffffffffff8111156103e6576103e5610284565b5b6103f284828501610387565b91505092915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602260045260245ffd5b5f600282049050600182168061043f57607f821691505b602082108103610452576104516103fb565b5b50919050565b5f819050815f5260205f209050919050565b5f6020601f8301049050919050565b5f82821b905092915050565b5f600883026104b47fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff82610479565b6104be8683610479565b95508019841693508086168417925050509392505050565b5f819050919050565b5f819050919050565b5f6105026104fd6104f8846104d6565b6104df565b6104d6565b9050919050565b5f819050919050565b61051b836104e8565b61052f61052782610509565b848454610485565b825550505050565b5f90565b610543610537565b61054e818484610512565b505050565b5b81811015610571576105665f8261053b565b600181019050610554565b5050565b601f8211156105b65761058781610458565b6105908461046a565b8101602085101561059f578190505b6105b36105ab8561046a565b830182610553565b50505b505050565b5f82821c905092915050565b5f6105d65f19846008026105bb565b1980831691505092915050565b5f6105ee83836105c7565b9150826002028217905092915050565b610607826101cd565b67ffffffffffffffff8111156106205761061f610290565b5b61062a8254610428565b610635828285610575565b5f60209050601f831160018114610666575f8415610654578287015190505b61065e85826105e3565b8655506106c5565b601f19841661067486610458565b5f5b8281101561069b57848901518255600182019150602085019450602081019050610676565b868310156106b857848901516106b4601f8916826105c7565b8355505b6001600288020188555050505b50505050505056fea26469706673582212200c951fefe65356cb6c3ea1f46ccf81fd82719a235a484bd7bab2cc19c484e7ad64736f6c63430008140033"  # noqa: E501
+BYTES_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b506004361061003f575f3560e01c8063209652551461004357806330de3cee14610061578063439970aa1461007f575b5f80fd5b61004b61009b565b6040516100589190610257565b60405180910390f35b61006961012b565b6040516100769190610257565b60405180910390f35b610099600480360381019061009491906103b4565b6101ba565b005b6060600180546100aa90610428565b80601f01602080910402602001604051908101604052809291908181526020018280546100d690610428565b80156101215780601f106100f857610100808354040283529160200191610121565b820191905f5260205f20905b81548152906001019060200180831161010457829003601f168201915b5050505050905090565b60605f805461013990610428565b80601f016020809104026020016040519081016040528092919081815260200182805461016590610428565b80156101b05780601f10610187576101008083540402835291602001916101b0565b820191905f5260205f20905b81548152906001019060200180831161019357829003601f168201915b5050505050905090565b80600190816101c991906105fe565b5050565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156102045780820151818401526020810190506101e9565b5f8484015250505050565b5f601f19601f8301169050919050565b5f610229826101cd565b61023381856101d7565b93506102438185602086016101e7565b61024c8161020f565b840191505092915050565b5f6020820190508181035f83015261026f818461021f565b905092915050565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f80fd5b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6102c68261020f565b810181811067ffffffffffffffff821117156102e5576102e4610290565b5b80604052505050565b5f6102f7610277565b905061030382826102bd565b919050565b5f67ffffffffffffffff82111561032257610321610290565b5b61032b8261020f565b9050602081019050919050565b828183375f83830152505050565b5f61035861035384610308565b6102ee565b9050828152602081018484840111156103745761037361028c565b5b61037f848285610338565b509392505050565b5f82601f83011261039b5761039a610288565b5b81356103ab848260208601610346565b91505092915050565b5f602082840312156103c9576103c8610280565b5b5f82013567ffffffffffffffff8111156103e6576103e5610284565b5b6103f284828501610387565b91505092915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602260045260245ffd5b5f600282049050600182168061043f57607f821691505b602082108103610452576104516103fb565b5b50919050565b5f819050815f5260205f209050919050565b5f6020601f8301049050919050565b5f82821b905092915050565b5f600883026104b47fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff82610479565b6104be8683610479565b95508019841693508086168417925050509392505050565b5f819050919050565b5f819050919050565b5f6105026104fd6104f8846104d6565b6104df565b6104d6565b9050919050565b5f819050919050565b61051b836104e8565b61052f61052782610509565b848454610485565b825550505050565b5f90565b610543610537565b61054e818484610512565b505050565b5b81811015610571576105665f8261053b565b600181019050610554565b5050565b601f8211156105b65761058781610458565b6105908461046a565b8101602085101561059f578190505b6105b36105ab8561046a565b830182610553565b50505b505050565b5f82821c905092915050565b5f6105d65f19846008026105bb565b1980831691505092915050565b5f6105ee83836105c7565b9150826002028217905092915050565b610607826101cd565b67ffffffffffffffff8111156106205761061f610290565b5b61062a8254610428565b610635828285610575565b5f60209050601f831160018114610666575f8415610654578287015190505b61065e85826105e3565b8655506106c5565b601f19841661067486610458565b5f5b8281101561069b57848901518255600182019150602085019450602081019050610676565b868310156106b857848901516106b4601f8916826105c7565b8355505b6001600288020188555050505b50505050505056fea26469706673582212200c951fefe65356cb6c3ea1f46ccf81fd82719a235a484bd7bab2cc19c484e7ad64736f6c63430008140033"  # noqa: E501
 BYTES_CONTRACT_ABI = [
     {
         "inputs": [{"internalType": "bytes", "name": "_value", "type": "bytes"}],
         "stateMutability": "nonpayable",
         "type": "constructor",
     },
     {
@@ -38,16 +38,16 @@
     "bytecode": BYTES_CONTRACT_BYTECODE,
     "bytecode_runtime": BYTES_CONTRACT_RUNTIME,
     "abi": BYTES_CONTRACT_ABI,
 }
 
 
 # source: web3/_utils/contract_sources/BytesContracts.sol:Bytes32Contract
-BYTES32_CONTRACT_BYTECODE = "0x60806040527f012301230123012301230123012301230123012301230123012301230123012360005534801561003457600080fd5b5060405161025d38038061025d8339818101604052810190610056919061009e565b80600181905550506100cb565b600080fd5b6000819050919050565b61007b81610068565b811461008657600080fd5b50565b60008151905061009881610072565b92915050565b6000602082840312156100b4576100b3610063565b5b60006100c284828501610089565b91505092915050565b610183806100da6000396000f3fe608060405234801561001057600080fd5b50600436106100415760003560e01c8063209652551461004657806330de3cee1461006457806358825b1014610082575b600080fd5b61004e61009e565b60405161005b91906100d4565b60405180910390f35b61006c6100a8565b60405161007991906100d4565b60405180910390f35b61009c60048036038101906100979190610120565b6100b1565b005b6000600154905090565b60008054905090565b8060018190555050565b6000819050919050565b6100ce816100bb565b82525050565b60006020820190506100e960008301846100c5565b92915050565b600080fd5b6100fd816100bb565b811461010857600080fd5b50565b60008135905061011a816100f4565b92915050565b600060208284031215610136576101356100ef565b5b60006101448482850161010b565b9150509291505056fea2646970667358221220967501f16e2398d7682cc7112f089eeb3c3153bebb94e7a01a943c7c89a57f3a64736f6c63430008130033"  # noqa: E501
-BYTES32_CONTRACT_RUNTIME = "0x608060405234801561001057600080fd5b50600436106100415760003560e01c8063209652551461004657806330de3cee1461006457806358825b1014610082575b600080fd5b61004e61009e565b60405161005b91906100d4565b60405180910390f35b61006c6100a8565b60405161007991906100d4565b60405180910390f35b61009c60048036038101906100979190610120565b6100b1565b005b6000600154905090565b60008054905090565b8060018190555050565b6000819050919050565b6100ce816100bb565b82525050565b60006020820190506100e960008301846100c5565b92915050565b600080fd5b6100fd816100bb565b811461010857600080fd5b50565b60008135905061011a816100f4565b92915050565b600060208284031215610136576101356100ef565b5b60006101448482850161010b565b9150509291505056fea2646970667358221220967501f16e2398d7682cc7112f089eeb3c3153bebb94e7a01a943c7c89a57f3a64736f6c63430008130033"  # noqa: E501
+BYTES32_CONTRACT_BYTECODE = "0x60806040527f01230123012301230123012301230123012301230123012301230123012301235f55348015610032575f80fd5b5060405161024638038061024683398181016040528101906100549190610098565b80600181905550506100c3565b5f80fd5b5f819050919050565b61007781610065565b8114610081575f80fd5b50565b5f815190506100928161006e565b92915050565b5f602082840312156100ad576100ac610061565b5b5f6100ba84828501610084565b91505092915050565b610176806100d05f395ff3fe608060405234801561000f575f80fd5b506004361061003f575f3560e01c8063209652551461004357806330de3cee1461006157806358825b101461007f575b5f80fd5b61004b61009b565b60405161005891906100ce565b60405180910390f35b6100696100a4565b60405161007691906100ce565b60405180910390f35b61009960048036038101906100949190610115565b6100ac565b005b5f600154905090565b5f8054905090565b8060018190555050565b5f819050919050565b6100c8816100b6565b82525050565b5f6020820190506100e15f8301846100bf565b92915050565b5f80fd5b6100f4816100b6565b81146100fe575f80fd5b50565b5f8135905061010f816100eb565b92915050565b5f6020828403121561012a576101296100e7565b5b5f61013784828501610101565b9150509291505056fea2646970667358221220c503016919f2342748db08a70857cb709d81da9201dccb4ff281d22fdedbc83f64736f6c63430008140033"  # noqa: E501
+BYTES32_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b506004361061003f575f3560e01c8063209652551461004357806330de3cee1461006157806358825b101461007f575b5f80fd5b61004b61009b565b60405161005891906100ce565b60405180910390f35b6100696100a4565b60405161007691906100ce565b60405180910390f35b61009960048036038101906100949190610115565b6100ac565b005b5f600154905090565b5f8054905090565b8060018190555050565b5f819050919050565b6100c8816100b6565b82525050565b5f6020820190506100e15f8301846100bf565b92915050565b5f80fd5b6100f4816100b6565b81146100fe575f80fd5b50565b5f8135905061010f816100eb565b92915050565b5f6020828403121561012a576101296100e7565b5b5f61013784828501610101565b9150509291505056fea2646970667358221220c503016919f2342748db08a70857cb709d81da9201dccb4ff281d22fdedbc83f64736f6c63430008140033"  # noqa: E501
 BYTES32_CONTRACT_ABI = [
     {
         "inputs": [{"internalType": "bytes32", "name": "_value", "type": "bytes32"}],
         "stateMutability": "nonpayable",
         "type": "constructor",
     },
     {
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/constructor_contracts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/ConstructorContracts.sol:SimpleConstructorContract  # noqa: E501
-SIMPLE_CONSTRUCTOR_CONTRACT_BYTECODE = "0x6080604052348015600f57600080fd5b50603f80601d6000396000f3fe6080604052600080fdfea264697066735822122059abb498a58b8a64c7139393e325cb4efbf87e2ad05e76a9bb1554f94c57f38764736f6c63430008130033"  # noqa: E501
-SIMPLE_CONSTRUCTOR_CONTRACT_RUNTIME = "0x6080604052600080fdfea264697066735822122059abb498a58b8a64c7139393e325cb4efbf87e2ad05e76a9bb1554f94c57f38764736f6c63430008130033"  # noqa: E501
+SIMPLE_CONSTRUCTOR_CONTRACT_BYTECODE = "0x6080604052348015600e575f80fd5b50603e80601a5f395ff3fe60806040525f80fdfea264697066735822122012ecdbcdd6cc4f577900d4a31f5a9598df06995235dae4ae1e2a391bf80a6ad264736f6c63430008140033"  # noqa: E501
+SIMPLE_CONSTRUCTOR_CONTRACT_RUNTIME = "0x60806040525f80fdfea264697066735822122012ecdbcdd6cc4f577900d4a31f5a9598df06995235dae4ae1e2a391bf80a6ad264736f6c63430008140033"  # noqa: E501
 SIMPLE_CONSTRUCTOR_CONTRACT_ABI = [
     {"inputs": [], "stateMutability": "nonpayable", "type": "constructor"}
 ]
 SIMPLE_CONSTRUCTOR_CONTRACT_DATA = {
     "bytecode": SIMPLE_CONSTRUCTOR_CONTRACT_BYTECODE,
     "bytecode_runtime": SIMPLE_CONSTRUCTOR_CONTRACT_RUNTIME,
     "abi": SIMPLE_CONSTRUCTOR_CONTRACT_ABI,
 }
 
 
 # source: web3/_utils/contract_sources/ConstructorContracts.sol:ConstructorWithArgumentsContract  # noqa: E501
-CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_BYTECODE = "0x608060405234801561001057600080fd5b50604051610214380380610214833981810160405281019061003291906100b8565b816000819055508060018190555050506100f8565b600080fd5b6000819050919050565b61005f8161004c565b811461006a57600080fd5b50565b60008151905061007c81610056565b92915050565b6000819050919050565b61009581610082565b81146100a057600080fd5b50565b6000815190506100b28161008c565b92915050565b600080604083850312156100cf576100ce610047565b5b60006100dd8582860161006d565b92505060206100ee858286016100a3565b9150509250929050565b61010d806101076000396000f3fe6080604052348015600f57600080fd5b506004361060325760003560e01c806388ec1346146037578063d4c46c76146051575b600080fd5b603d606b565b60405160489190608e565b60405180910390f35b60576071565b6040516062919060be565b60405180910390f35b60005481565b60015481565b6000819050919050565b6088816077565b82525050565b600060208201905060a160008301846081565b92915050565b6000819050919050565b60b88160a7565b82525050565b600060208201905060d1600083018460b1565b9291505056fea2646970667358221220d59463714be22b6ef7ac4ea1c9a2649286c98430ecda1b5ad84e64f73fbf97bb64736f6c63430008130033"  # noqa: E501
-CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_RUNTIME = "0x6080604052348015600f57600080fd5b506004361060325760003560e01c806388ec1346146037578063d4c46c76146051575b600080fd5b603d606b565b60405160489190608e565b60405180910390f35b60576071565b6040516062919060be565b60405180910390f35b60005481565b60015481565b6000819050919050565b6088816077565b82525050565b600060208201905060a160008301846081565b92915050565b6000819050919050565b60b88160a7565b82525050565b600060208201905060d1600083018460b1565b9291505056fea2646970667358221220d59463714be22b6ef7ac4ea1c9a2649286c98430ecda1b5ad84e64f73fbf97bb64736f6c63430008130033"  # noqa: E501
+CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b506040516101fd3803806101fd833981810160405281019061003191906100af565b815f819055508060018190555050506100ed565b5f80fd5b5f819050919050565b61005b81610049565b8114610065575f80fd5b50565b5f8151905061007681610052565b92915050565b5f819050919050565b61008e8161007c565b8114610098575f80fd5b50565b5f815190506100a981610085565b92915050565b5f80604083850312156100c5576100c4610045565b5b5f6100d285828601610068565b92505060206100e38582860161009b565b9150509250929050565b610103806100fa5f395ff3fe6080604052348015600e575f80fd5b50600436106030575f3560e01c806388ec1346146034578063d4c46c7614604e575b5f80fd5b603a6068565b604051604591906089565b60405180910390f35b6054606d565b604051605f919060b6565b60405180910390f35b5f5481565b60015481565b5f819050919050565b6083816073565b82525050565b5f602082019050609a5f830184607c565b92915050565b5f819050919050565b60b08160a0565b82525050565b5f60208201905060c75f83018460a9565b9291505056fea2646970667358221220605cf878f0fbb3ee5e94e8de43849d105ac50df572f1b07980500c444e3f6e9b64736f6c63430008140033"  # noqa: E501
+CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_RUNTIME = "0x6080604052348015600e575f80fd5b50600436106030575f3560e01c806388ec1346146034578063d4c46c7614604e575b5f80fd5b603a6068565b604051604591906089565b60405180910390f35b6054606d565b604051605f919060b6565b60405180910390f35b5f5481565b60015481565b5f819050919050565b6083816073565b82525050565b5f602082019050609a5f830184607c565b92915050565b5f819050919050565b60b08160a0565b82525050565b5f60208201905060c75f83018460a9565b9291505056fea2646970667358221220605cf878f0fbb3ee5e94e8de43849d105ac50df572f1b07980500c444e3f6e9b64736f6c63430008140033"  # noqa: E501
 CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_ABI = [
     {
         "inputs": [
             {"internalType": "uint256", "name": "a", "type": "uint256"},
             {"internalType": "bytes32", "name": "b", "type": "bytes32"},
         ],
         "stateMutability": "nonpayable",
@@ -47,16 +47,16 @@
     "bytecode": CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_BYTECODE,
     "bytecode_runtime": CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_RUNTIME,
     "abi": CONSTRUCTOR_WITH_ARGUMENTS_CONTRACT_ABI,
 }
 
 
 # source: web3/_utils/contract_sources/ConstructorContracts.sol:ConstructorWithAddressArgumentContract  # noqa: E501
-CONSTRUCTOR_WITH_ADDRESS_ARGUMENT_CONTRACT_BYTECODE = "0x608060405234801561001057600080fd5b5060405161020d38038061020d833981810160405281019061003291906100db565b806000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555050610108565b600080fd5b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006100a88261007d565b9050919050565b6100b88161009d565b81146100c357600080fd5b50565b6000815190506100d5816100af565b92915050565b6000602082840312156100f1576100f0610078565b5b60006100ff848285016100c6565b91505092915050565b60f7806101166000396000f3fe6080604052348015600f57600080fd5b506004361060285760003560e01c806334664e3a14602d575b600080fd5b60336047565b604051603e919060a8565b60405180910390f35b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b6000609482606b565b9050919050565b60a281608b565b82525050565b600060208201905060bb6000830184609b565b9291505056fea26469706673582212202163673b7255f6a02361134ec5f1ddfb92101c44d12922f841e949ebd2787e8864736f6c63430008130033"  # noqa: E501
-CONSTRUCTOR_WITH_ADDRESS_ARGUMENT_CONTRACT_RUNTIME = "0x6080604052348015600f57600080fd5b506004361060285760003560e01c806334664e3a14602d575b600080fd5b60336047565b604051603e919060a8565b60405180910390f35b60008054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b6000609482606b565b9050919050565b60a281608b565b82525050565b600060208201905060bb6000830184609b565b9291505056fea26469706673582212202163673b7255f6a02361134ec5f1ddfb92101c44d12922f841e949ebd2787e8864736f6c63430008130033"  # noqa: E501
+CONSTRUCTOR_WITH_ADDRESS_ARGUMENT_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b506040516101fa3803806101fa833981810160405281019061003191906100d4565b805f806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff160217905550506100ff565b5f80fd5b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6100a38261007a565b9050919050565b6100b381610099565b81146100bd575f80fd5b50565b5f815190506100ce816100aa565b92915050565b5f602082840312156100e9576100e8610076565b5b5f6100f6848285016100c0565b91505092915050565b60ef8061010b5f395ff3fe6080604052348015600e575f80fd5b50600436106026575f3560e01c806334664e3a14602a575b5f80fd5b60306044565b604051603b919060a2565b60405180910390f35b5f8054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f608e826067565b9050919050565b609c816086565b82525050565b5f60208201905060b35f8301846095565b9291505056fea26469706673582212202250337f0c250bf5cf3fa7a5db19244d27f964450a536f014297602192efa03364736f6c63430008140033"  # noqa: E501
+CONSTRUCTOR_WITH_ADDRESS_ARGUMENT_CONTRACT_RUNTIME = "0x6080604052348015600e575f80fd5b50600436106026575f3560e01c806334664e3a14602a575b5f80fd5b60306044565b604051603b919060a2565b60405180910390f35b5f8054906101000a900473ffffffffffffffffffffffffffffffffffffffff1681565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f608e826067565b9050919050565b609c816086565b82525050565b5f60208201905060b35f8301846095565b9291505056fea26469706673582212202250337f0c250bf5cf3fa7a5db19244d27f964450a536f014297602192efa03364736f6c63430008140033"  # noqa: E501
 CONSTRUCTOR_WITH_ADDRESS_ARGUMENT_CONTRACT_ABI = [
     {
         "inputs": [{"internalType": "address", "name": "_testAddr", "type": "address"}],
         "stateMutability": "nonpayable",
         "type": "constructor",
     },
     {
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/contract_caller_tester.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/reflector_contracts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,29 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
-# source: web3/_utils/contract_sources/ContractCallerTester.sol:ContractCallerTester
-CONTRACT_CALLER_TESTER_BYTECODE = "0x608060405234801561001057600080fd5b50610458806100206000396000f3fe60806040526004361061004a5760003560e01c806306661abd1461004f57806361bc221a1461007a578063a5f3c23b14610098578063c7fa7d66146100c8578063d09de08a146100ea575b600080fd5b34801561005b57600080fd5b50610064610115565b60405161007191906101df565b60405180910390f35b61008261011b565b60405161008f91906101df565b60405180910390f35b6100b260048036038101906100ad919061022b565b610124565b6040516100bf91906101df565b60405180910390f35b6100d061013a565b6040516100e1959493929190610355565b60405180910390f35b3480156100f657600080fd5b506100ff6101a7565b60405161010c91906101df565b60405180910390f35b60005481565b60008054905090565b6000818361013291906103de565b905092915050565b600060606000806000336000365a344384848080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505093509091929350945094509450945094509091929394565b600060016000808282546101bb91906103de565b925050819055905090565b6000819050919050565b6101d9816101c6565b82525050565b60006020820190506101f460008301846101d0565b92915050565b600080fd5b610208816101c6565b811461021357600080fd5b50565b600081359050610225816101ff565b92915050565b60008060408385031215610242576102416101fa565b5b600061025085828601610216565b925050602061026185828601610216565b9150509250929050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006102968261026b565b9050919050565b6102a68161028b565b82525050565b600081519050919050565b600082825260208201905092915050565b60005b838110156102e65780820151818401526020810190506102cb565b60008484015250505050565b6000601f19601f8301169050919050565b600061030e826102ac565b61031881856102b7565b93506103288185602086016102c8565b610331816102f2565b840191505092915050565b6000819050919050565b61034f8161033c565b82525050565b600060a08201905061036a600083018861029d565b818103602083015261037c8187610303565b905061038b6040830186610346565b6103986060830185610346565b6103a56080830184610346565b9695505050505050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006103e9826101c6565b91506103f4836101c6565b92508282019050828112156000831216838212600084121516171561041c5761041b6103af565b5b9291505056fea26469706673582212200d898dac1fb4d379c02eb5a80e3cd572f005544ef7e2d010b3f8ba59e83df88364736f6c63430008130033"  # noqa: E501
-CONTRACT_CALLER_TESTER_RUNTIME = "0x60806040526004361061004a5760003560e01c806306661abd1461004f57806361bc221a1461007a578063a5f3c23b14610098578063c7fa7d66146100c8578063d09de08a146100ea575b600080fd5b34801561005b57600080fd5b50610064610115565b60405161007191906101df565b60405180910390f35b61008261011b565b60405161008f91906101df565b60405180910390f35b6100b260048036038101906100ad919061022b565b610124565b6040516100bf91906101df565b60405180910390f35b6100d061013a565b6040516100e1959493929190610355565b60405180910390f35b3480156100f657600080fd5b506100ff6101a7565b60405161010c91906101df565b60405180910390f35b60005481565b60008054905090565b6000818361013291906103de565b905092915050565b600060606000806000336000365a344384848080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505093509091929350945094509450945094509091929394565b600060016000808282546101bb91906103de565b925050819055905090565b6000819050919050565b6101d9816101c6565b82525050565b60006020820190506101f460008301846101d0565b92915050565b600080fd5b610208816101c6565b811461021357600080fd5b50565b600081359050610225816101ff565b92915050565b60008060408385031215610242576102416101fa565b5b600061025085828601610216565b925050602061026185828601610216565b9150509250929050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006102968261026b565b9050919050565b6102a68161028b565b82525050565b600081519050919050565b600082825260208201905092915050565b60005b838110156102e65780820151818401526020810190506102cb565b60008484015250505050565b6000601f19601f8301169050919050565b600061030e826102ac565b61031881856102b7565b93506103288185602086016102c8565b610331816102f2565b840191505092915050565b6000819050919050565b61034f8161033c565b82525050565b600060a08201905061036a600083018861029d565b818103602083015261037c8187610303565b905061038b6040830186610346565b6103986060830185610346565b6103a56080830184610346565b9695505050505050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006103e9826101c6565b91506103f4836101c6565b92508282019050828112156000831216838212600084121516171561041c5761041b6103af565b5b9291505056fea26469706673582212200d898dac1fb4d379c02eb5a80e3cd572f005544ef7e2d010b3f8ba59e83df88364736f6c63430008130033"  # noqa: E501
-CONTRACT_CALLER_TESTER_ABI = [
+# source: web3/_utils/contract_sources/ReflectorContracts.sol:AddressReflectorContract
+ADDRESS_REFLECTOR_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b5061040d8061001d5f395ff3fe608060405234801561000f575f80fd5b5060043610610034575f3560e01c80630b816c1614610038578063c04d11fc14610068575b5f80fd5b610052600480360381019061004d9190610116565b610098565b60405161005f9190610150565b60405180910390f35b610082600480360381019061007d91906102b9565b6100a1565b60405161008f91906103b7565b60405180910390f35b5f819050919050565b6060819050919050565b5f604051905090565b5f80fd5b5f80fd5b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6100e5826100bc565b9050919050565b6100f5816100db565b81146100ff575f80fd5b50565b5f81359050610110816100ec565b92915050565b5f6020828403121561012b5761012a6100b4565b5b5f61013884828501610102565b91505092915050565b61014a816100db565b82525050565b5f6020820190506101635f830184610141565b92915050565b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6101b38261016d565b810181811067ffffffffffffffff821117156101d2576101d161017d565b5b80604052505050565b5f6101e46100ab565b90506101f082826101aa565b919050565b5f67ffffffffffffffff82111561020f5761020e61017d565b5b602082029050602081019050919050565b5f80fd5b5f610236610231846101f5565b6101db565b9050808382526020820190506020840283018581111561025957610258610220565b5b835b81811015610282578061026e8882610102565b84526020840193505060208101905061025b565b5050509392505050565b5f82601f8301126102a05761029f610169565b5b81356102b0848260208601610224565b91505092915050565b5f602082840312156102ce576102cd6100b4565b5b5f82013567ffffffffffffffff8111156102eb576102ea6100b8565b5b6102f78482850161028c565b91505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b610332816100db565b82525050565b5f6103438383610329565b60208301905092915050565b5f602082019050919050565b5f61036582610300565b61036f818561030a565b935061037a8361031a565b805f5b838110156103aa5781516103918882610338565b975061039c8361034f565b92505060018101905061037d565b5085935050505092915050565b5f6020820190508181035f8301526103cf818461035b565b90509291505056fea26469706673582212205b599d97c355322f734f2dba099c5c76992707633929ddbd950c073a461a2eae64736f6c63430008140033"  # noqa: E501
+ADDRESS_REFLECTOR_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b5060043610610034575f3560e01c80630b816c1614610038578063c04d11fc14610068575b5f80fd5b610052600480360381019061004d9190610116565b610098565b60405161005f9190610150565b60405180910390f35b610082600480360381019061007d91906102b9565b6100a1565b60405161008f91906103b7565b60405180910390f35b5f819050919050565b6060819050919050565b5f604051905090565b5f80fd5b5f80fd5b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6100e5826100bc565b9050919050565b6100f5816100db565b81146100ff575f80fd5b50565b5f81359050610110816100ec565b92915050565b5f6020828403121561012b5761012a6100b4565b5b5f61013884828501610102565b91505092915050565b61014a816100db565b82525050565b5f6020820190506101635f830184610141565b92915050565b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6101b38261016d565b810181811067ffffffffffffffff821117156101d2576101d161017d565b5b80604052505050565b5f6101e46100ab565b90506101f082826101aa565b919050565b5f67ffffffffffffffff82111561020f5761020e61017d565b5b602082029050602081019050919050565b5f80fd5b5f610236610231846101f5565b6101db565b9050808382526020820190506020840283018581111561025957610258610220565b5b835b81811015610282578061026e8882610102565b84526020840193505060208101905061025b565b5050509392505050565b5f82601f8301126102a05761029f610169565b5b81356102b0848260208601610224565b91505092915050565b5f602082840312156102ce576102cd6100b4565b5b5f82013567ffffffffffffffff8111156102eb576102ea6100b8565b5b6102f78482850161028c565b91505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b610332816100db565b82525050565b5f6103438383610329565b60208301905092915050565b5f602082019050919050565b5f61036582610300565b61036f818561030a565b935061037a8361031a565b805f5b838110156103aa5781516103918882610338565b975061039c8361034f565b92505060018101905061037d565b5085935050505092915050565b5f6020820190508181035f8301526103cf818461035b565b90509291505056fea26469706673582212205b599d97c355322f734f2dba099c5c76992707633929ddbd950c073a461a2eae64736f6c63430008140033"  # noqa: E501
+ADDRESS_REFLECTOR_CONTRACT_ABI = [
     {
-        "inputs": [
-            {"internalType": "int256", "name": "a", "type": "int256"},
-            {"internalType": "int256", "name": "b", "type": "int256"},
-        ],
-        "name": "add",
-        "outputs": [{"internalType": "int256", "name": "", "type": "int256"}],
-        "stateMutability": "payable",
+        "inputs": [{"internalType": "address", "name": "arg", "type": "address"}],
+        "name": "reflect",
+        "outputs": [{"internalType": "address", "name": "", "type": "address"}],
+        "stateMutability": "pure",
         "type": "function",
     },
     {
-        "inputs": [],
-        "name": "count",
-        "outputs": [{"internalType": "int256", "name": "", "type": "int256"}],
-        "stateMutability": "view",
-        "type": "function",
-    },
-    {
-        "inputs": [],
-        "name": "counter",
-        "outputs": [{"internalType": "int256", "name": "", "type": "int256"}],
-        "stateMutability": "payable",
-        "type": "function",
-    },
-    {
-        "inputs": [],
-        "name": "increment",
-        "outputs": [{"internalType": "int256", "name": "", "type": "int256"}],
-        "stateMutability": "nonpayable",
-        "type": "function",
-    },
-    {
-        "inputs": [],
-        "name": "returnMeta",
-        "outputs": [
-            {"internalType": "address", "name": "", "type": "address"},
-            {"internalType": "bytes", "name": "", "type": "bytes"},
-            {"internalType": "uint256", "name": "", "type": "uint256"},
-            {"internalType": "uint256", "name": "", "type": "uint256"},
-            {"internalType": "uint256", "name": "", "type": "uint256"},
-        ],
-        "stateMutability": "payable",
+        "inputs": [{"internalType": "address[]", "name": "arg", "type": "address[]"}],
+        "name": "reflect",
+        "outputs": [{"internalType": "address[]", "name": "", "type": "address[]"}],
+        "stateMutability": "pure",
         "type": "function",
     },
 ]
-CONTRACT_CALLER_TESTER_DATA = {
-    "bytecode": CONTRACT_CALLER_TESTER_BYTECODE,
-    "bytecode_runtime": CONTRACT_CALLER_TESTER_RUNTIME,
-    "abi": CONTRACT_CALLER_TESTER_ABI,
+ADDRESS_REFLECTOR_CONTRACT_DATA = {
+    "bytecode": ADDRESS_REFLECTOR_CONTRACT_BYTECODE,
+    "bytecode_runtime": ADDRESS_REFLECTOR_CONTRACT_RUNTIME,
+    "abi": ADDRESS_REFLECTOR_CONTRACT_ABI,
 }
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/emitter_contract.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/emitter_contract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/EmitterContract.sol:EmitterContract
-EMITTER_CONTRACT_BYTECODE = "0x608060405234801561001057600080fd5b50611757806100206000396000f3fe608060405234801561001057600080fd5b50600436106100b45760003560e01c80639c377053116100715780639c37705314610161578063aa6fd8221461017d578063acabb9ed14610199578063b2ddc449146101b5578063e17bf956146101d1578063f82ef69e146101ed576100b4565b80630bb563d6146100b957806317c0c180146100d557806320f0256e146100f15780635da86c171461010d57806390b41d8b14610129578063966b50e014610145575b600080fd5b6100d360048036038101906100ce9190610af3565b610209565b005b6100ef60048036038101906100ea9190610b61565b610243565b005b61010b60048036038101906101069190610bc4565b61031b565b005b61012760048036038101906101229190610ce4565b610438565b005b610143600480360381019061013e9190610d24565b610475565b005b61015f600480360381019061015a9190610e97565b6105d2565b005b61017b60048036038101906101769190610f0f565b610623565b005b61019760048036038101906101929190610f76565b61073b565b005b6101b360048036038101906101ae9190610fb6565b61087f565b005b6101cf60048036038101906101ca919061108c565b6108d0565b005b6101eb60048036038101906101e6919061116d565b610922565b005b6102076004803603810190610202919061108c565b61095c565b005b7fa95e6e2a182411e7a6f9ed114a85c3761d87f9b8f453d842c71235aa64fff99f816040516102389190611235565b60405180910390a150565b6001601281111561025757610256611257565b5b81601281111561026a57610269611257565b5b036102a0577f1e86022f78f8d04f8e3dfd13a2bdb280403e6632877c0dbee5e4eeb259908a5c60405160405180910390a1610318565b600060128111156102b4576102b3611257565b5b8160128111156102c7576102c6611257565b5b036102dc5760405160405180910390a0610317565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161030e906112f8565b60405180910390fd5b5b50565b6005601281111561032f5761032e611257565b5b85601281111561034257610341611257565b5b03610389577ff039d147f23fe975a4254bdf6b1502b8c79132ae1833986b7ccef2638e73fdf98484848460405161037c9493929190611327565b60405180910390a1610431565b600b601281111561039d5761039c611257565b5b8560128111156103b0576103af611257565b5b036103f55780827fa30ece802b64cd2b7e57dabf4010aabf5df26d1556977affb07b98a77ad955b586866040516103e892919061136c565b60405180910390a3610430565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610427906112f8565b60405180910390fd5b5b5050505050565b7f8ccce2523cca5f3851d20df50b5a59509bc4ac7d9ddba344f5e331969d09b8e78282604051610469929190611402565b60405180910390a15050565b6003601281111561048957610488611257565b5b83601281111561049c5761049b611257565b5b036104df577fdf0cb1dea99afceb3ea698d62e705b736f1345a7eee9eb07e63d1f8f556c1bc582826040516104d292919061136c565b60405180910390a16105cd565b600960128111156104f3576104f2611257565b5b83601281111561050657610505611257565b5b0361054857807f057bc32826fbe161da1c110afcdcae7c109a8b69149f727fc37a603c60ef94ca8360405161053b919061142b565b60405180910390a26105cc565b6008601281111561055c5761055b611257565b5b83601281111561056f5761056e611257565b5b03610590578082604051610583919061142b565b60405180910390a16105cb565b6040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016105c2906112f8565b60405180910390fd5b5b5b505050565b816040516105e091906114fe565b60405180910390207fdbc4c1d1d2f0d84e58d36ca767ec9ba2ec2f933c055e50e5ccdd57697f7b58b08260405161061791906115ab565b60405180910390a25050565b6004601281111561063757610636611257565b5b84601281111561064a57610649611257565b5b0361068f577f4a25b279c7c585f25eda9788ac9420ebadae78ca6b206a0e6ab488fd81f55062838383604051610682939291906115cd565b60405180910390a1610735565b600a60128111156106a3576106a2611257565b5b8460128111156106b6576106b5611257565b5b036106f95780827ff16c999b533366ca5138d78e85da51611089cd05749f098d6c225d4cd42ee6ec856040516106ec919061142b565b60405180910390a3610734565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161072b906112f8565b60405180910390fd5b5b50505050565b6002601281111561074f5761074e611257565b5b82601281111561076257610761611257565b5b036107a3577f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d481604051610796919061142b565b60405180910390a161087b565b600760128111156107b7576107b6611257565b5b8260128111156107ca576107c9611257565b5b0361080157807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a261087a565b6006601281111561081557610814611257565b5b82601281111561082857610827611257565b5b0361083e578060405160405180910390a1610879565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610870906112f8565b60405180910390fd5b5b5b5050565b8160405161088d9190611640565b60405180910390207fe77cf33df73da7bc2e253a2dae617e6f15e4e337eaa462a108903af4643d1b75826040516108c49190611235565b60405180910390a25050565b8173ffffffffffffffffffffffffffffffffffffffff167ff922c215689548d72c3d2fe4ea8dafb2a30c43312c9b43fe5d10f713181f991c826040516109169190611666565b60405180910390a25050565b7f532fd6ea96cfb78bb46e09279a26828b8b493de1a2b8b1ee1face527978a15a58160405161095191906116d6565b60405180910390a150565b7f06029e18f16caae06a69281f35b00ed3fcf47950e6c99dafa1bdd8c4b93479a0828260405161098d9291906116f8565b60405180910390a15050565b6000604051905090565b600080fd5b600080fd5b600080fd5b600080fd5b6000601f19601f8301169050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b610a00826109b7565b810181811067ffffffffffffffff82111715610a1f57610a1e6109c8565b5b80604052505050565b6000610a32610999565b9050610a3e82826109f7565b919050565b600067ffffffffffffffff821115610a5e57610a5d6109c8565b5b610a67826109b7565b9050602081019050919050565b82818337600083830152505050565b6000610a96610a9184610a43565b610a28565b905082815260208101848484011115610ab257610ab16109b2565b5b610abd848285610a74565b509392505050565b600082601f830112610ada57610ad96109ad565b5b8135610aea848260208601610a83565b91505092915050565b600060208284031215610b0957610b086109a3565b5b600082013567ffffffffffffffff811115610b2757610b266109a8565b5b610b3384828501610ac5565b91505092915050565b60138110610b4957600080fd5b50565b600081359050610b5b81610b3c565b92915050565b600060208284031215610b7757610b766109a3565b5b6000610b8584828501610b4c565b91505092915050565b6000819050919050565b610ba181610b8e565b8114610bac57600080fd5b50565b600081359050610bbe81610b98565b92915050565b600080600080600060a08688031215610be057610bdf6109a3565b5b6000610bee88828901610b4c565b9550506020610bff88828901610baf565b9450506040610c1088828901610baf565b9350506060610c2188828901610baf565b9250506080610c3288828901610baf565b9150509295509295909350565b600080fd5b600060208284031215610c5a57610c59610c3f565b5b610c646020610a28565b90506000610c7484828501610baf565b60008301525092915050565b600060608284031215610c9657610c95610c3f565b5b610ca06060610a28565b90506000610cb084828501610baf565b6000830152506020610cc484828501610baf565b6020830152506040610cd884828501610c44565b60408301525092915050565b60008060808385031215610cfb57610cfa6109a3565b5b6000610d0985828601610baf565b9250506020610d1a85828601610c80565b9150509250929050565b600080600060608486031215610d3d57610d3c6109a3565b5b6000610d4b86828701610b4c565b9350506020610d5c86828701610baf565b9250506040610d6d86828701610baf565b9150509250925092565b600067ffffffffffffffff821115610d9257610d916109c8565b5b602082029050602081019050919050565b600080fd5b60007fffff00000000000000000000000000000000000000000000000000000000000082169050919050565b610ddd81610da8565b8114610de857600080fd5b50565b600081359050610dfa81610dd4565b92915050565b6000610e13610e0e84610d77565b610a28565b90508083825260208201905060208402830185811115610e3657610e35610da3565b5b835b81811015610e5f5780610e4b8882610deb565b845260208401935050602081019050610e38565b5050509392505050565b600082601f830112610e7e57610e7d6109ad565b5b8135610e8e848260208601610e00565b91505092915050565b60008060408385031215610eae57610ead6109a3565b5b600083013567ffffffffffffffff811115610ecc57610ecb6109a8565b5b610ed885828601610e69565b925050602083013567ffffffffffffffff811115610ef957610ef86109a8565b5b610f0585828601610e69565b9150509250929050565b60008060008060808587031215610f2957610f286109a3565b5b6000610f3787828801610b4c565b9450506020610f4887828801610baf565b9350506040610f5987828801610baf565b9250506060610f6a87828801610baf565b91505092959194509250565b60008060408385031215610f8d57610f8c6109a3565b5b6000610f9b85828601610b4c565b9250506020610fac85828601610baf565b9150509250929050565b60008060408385031215610fcd57610fcc6109a3565b5b600083013567ffffffffffffffff811115610feb57610fea6109a8565b5b610ff785828601610ac5565b925050602083013567ffffffffffffffff811115611018576110176109a8565b5b61102485828601610ac5565b9150509250929050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006110598261102e565b9050919050565b6110698161104e565b811461107457600080fd5b50565b60008135905061108681611060565b92915050565b600080604083850312156110a3576110a26109a3565b5b60006110b185828601611077565b92505060206110c285828601611077565b9150509250929050565b600067ffffffffffffffff8211156110e7576110e66109c8565b5b6110f0826109b7565b9050602081019050919050565b600061111061110b846110cc565b610a28565b90508281526020810184848401111561112c5761112b6109b2565b5b611137848285610a74565b509392505050565b600082601f830112611154576111536109ad565b5b81356111648482602086016110fd565b91505092915050565b600060208284031215611183576111826109a3565b5b600082013567ffffffffffffffff8111156111a1576111a06109a8565b5b6111ad8482850161113f565b91505092915050565b600081519050919050565b600082825260208201905092915050565b60005b838110156111f05780820151818401526020810190506111d5565b60008484015250505050565b6000611207826111b6565b61121181856111c1565b93506112218185602086016111d2565b61122a816109b7565b840191505092915050565b6000602082019050818103600083015261124f81846111fc565b905092915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602160045260246000fd5b7f4469646e2774206d6174636820616e7920616c6c6f7761626c65206576656e7460008201527f20696e6465780000000000000000000000000000000000000000000000000000602082015250565b60006112e26026836111c1565b91506112ed82611286565b604082019050919050565b60006020820190508181036000830152611311816112d5565b9050919050565b61132181610b8e565b82525050565b600060808201905061133c6000830187611318565b6113496020830186611318565b6113566040830185611318565b6113636060830184611318565b95945050505050565b60006040820190506113816000830185611318565b61138e6020830184611318565b9392505050565b61139e81610b8e565b82525050565b6020820160008201516113ba6000850182611395565b50505050565b6060820160008201516113d66000850182611395565b5060208201516113e96020850182611395565b5060408201516113fc60408501826113a4565b50505050565b60006080820190506114176000830185611318565b61142460208301846113c0565b9392505050565b60006020820190506114406000830184611318565b92915050565b600081519050919050565b600081905092915050565b6000819050602082019050919050565b61147581610da8565b82525050565b6000611487838361146c565b60208301905092915050565b6000602082019050919050565b60006114ab82611446565b6114b58185611451565b93506114c08361145c565b8060005b838110156114f15781516114d8888261147b565b97506114e383611493565b9250506001810190506114c4565b5085935050505092915050565b600061150a82846114a0565b915081905092915050565b600082825260208201905092915050565b61152f81610da8565b82525050565b60006115418383611526565b60208301905092915050565b600061155882611446565b6115628185611515565b935061156d8361145c565b8060005b8381101561159e5781516115858882611535565b975061159083611493565b925050600181019050611571565b5085935050505092915050565b600060208201905081810360008301526115c5818461154d565b905092915050565b60006060820190506115e26000830186611318565b6115ef6020830185611318565b6115fc6040830184611318565b949350505050565b600081905092915050565b600061161a826111b6565b6116248185611604565b93506116348185602086016111d2565b80840191505092915050565b600061164c828461160f565b915081905092915050565b6116608161104e565b82525050565b600060208201905061167b6000830184611657565b92915050565b600081519050919050565b600082825260208201905092915050565b60006116a882611681565b6116b2818561168c565b93506116c28185602086016111d2565b6116cb816109b7565b840191505092915050565b600060208201905081810360008301526116f0818461169d565b905092915050565b600060408201905061170d6000830185611657565b61171a6020830184611657565b939250505056fea264697066735822122032046b888f6fa110fcef57e075d1d0dc39c921c65480e9c796549089971aa01b64736f6c63430008130033"  # noqa: E501
-EMITTER_CONTRACT_RUNTIME = "0x608060405234801561001057600080fd5b50600436106100b45760003560e01c80639c377053116100715780639c37705314610161578063aa6fd8221461017d578063acabb9ed14610199578063b2ddc449146101b5578063e17bf956146101d1578063f82ef69e146101ed576100b4565b80630bb563d6146100b957806317c0c180146100d557806320f0256e146100f15780635da86c171461010d57806390b41d8b14610129578063966b50e014610145575b600080fd5b6100d360048036038101906100ce9190610af3565b610209565b005b6100ef60048036038101906100ea9190610b61565b610243565b005b61010b60048036038101906101069190610bc4565b61031b565b005b61012760048036038101906101229190610ce4565b610438565b005b610143600480360381019061013e9190610d24565b610475565b005b61015f600480360381019061015a9190610e97565b6105d2565b005b61017b60048036038101906101769190610f0f565b610623565b005b61019760048036038101906101929190610f76565b61073b565b005b6101b360048036038101906101ae9190610fb6565b61087f565b005b6101cf60048036038101906101ca919061108c565b6108d0565b005b6101eb60048036038101906101e6919061116d565b610922565b005b6102076004803603810190610202919061108c565b61095c565b005b7fa95e6e2a182411e7a6f9ed114a85c3761d87f9b8f453d842c71235aa64fff99f816040516102389190611235565b60405180910390a150565b6001601281111561025757610256611257565b5b81601281111561026a57610269611257565b5b036102a0577f1e86022f78f8d04f8e3dfd13a2bdb280403e6632877c0dbee5e4eeb259908a5c60405160405180910390a1610318565b600060128111156102b4576102b3611257565b5b8160128111156102c7576102c6611257565b5b036102dc5760405160405180910390a0610317565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161030e906112f8565b60405180910390fd5b5b50565b6005601281111561032f5761032e611257565b5b85601281111561034257610341611257565b5b03610389577ff039d147f23fe975a4254bdf6b1502b8c79132ae1833986b7ccef2638e73fdf98484848460405161037c9493929190611327565b60405180910390a1610431565b600b601281111561039d5761039c611257565b5b8560128111156103b0576103af611257565b5b036103f55780827fa30ece802b64cd2b7e57dabf4010aabf5df26d1556977affb07b98a77ad955b586866040516103e892919061136c565b60405180910390a3610430565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610427906112f8565b60405180910390fd5b5b5050505050565b7f8ccce2523cca5f3851d20df50b5a59509bc4ac7d9ddba344f5e331969d09b8e78282604051610469929190611402565b60405180910390a15050565b6003601281111561048957610488611257565b5b83601281111561049c5761049b611257565b5b036104df577fdf0cb1dea99afceb3ea698d62e705b736f1345a7eee9eb07e63d1f8f556c1bc582826040516104d292919061136c565b60405180910390a16105cd565b600960128111156104f3576104f2611257565b5b83601281111561050657610505611257565b5b0361054857807f057bc32826fbe161da1c110afcdcae7c109a8b69149f727fc37a603c60ef94ca8360405161053b919061142b565b60405180910390a26105cc565b6008601281111561055c5761055b611257565b5b83601281111561056f5761056e611257565b5b03610590578082604051610583919061142b565b60405180910390a16105cb565b6040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016105c2906112f8565b60405180910390fd5b5b5b505050565b816040516105e091906114fe565b60405180910390207fdbc4c1d1d2f0d84e58d36ca767ec9ba2ec2f933c055e50e5ccdd57697f7b58b08260405161061791906115ab565b60405180910390a25050565b6004601281111561063757610636611257565b5b84601281111561064a57610649611257565b5b0361068f577f4a25b279c7c585f25eda9788ac9420ebadae78ca6b206a0e6ab488fd81f55062838383604051610682939291906115cd565b60405180910390a1610735565b600a60128111156106a3576106a2611257565b5b8460128111156106b6576106b5611257565b5b036106f95780827ff16c999b533366ca5138d78e85da51611089cd05749f098d6c225d4cd42ee6ec856040516106ec919061142b565b60405180910390a3610734565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161072b906112f8565b60405180910390fd5b5b50505050565b6002601281111561074f5761074e611257565b5b82601281111561076257610761611257565b5b036107a3577f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d481604051610796919061142b565b60405180910390a161087b565b600760128111156107b7576107b6611257565b5b8260128111156107ca576107c9611257565b5b0361080157807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a261087a565b6006601281111561081557610814611257565b5b82601281111561082857610827611257565b5b0361083e578060405160405180910390a1610879565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610870906112f8565b60405180910390fd5b5b5b5050565b8160405161088d9190611640565b60405180910390207fe77cf33df73da7bc2e253a2dae617e6f15e4e337eaa462a108903af4643d1b75826040516108c49190611235565b60405180910390a25050565b8173ffffffffffffffffffffffffffffffffffffffff167ff922c215689548d72c3d2fe4ea8dafb2a30c43312c9b43fe5d10f713181f991c826040516109169190611666565b60405180910390a25050565b7f532fd6ea96cfb78bb46e09279a26828b8b493de1a2b8b1ee1face527978a15a58160405161095191906116d6565b60405180910390a150565b7f06029e18f16caae06a69281f35b00ed3fcf47950e6c99dafa1bdd8c4b93479a0828260405161098d9291906116f8565b60405180910390a15050565b6000604051905090565b600080fd5b600080fd5b600080fd5b600080fd5b6000601f19601f8301169050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b610a00826109b7565b810181811067ffffffffffffffff82111715610a1f57610a1e6109c8565b5b80604052505050565b6000610a32610999565b9050610a3e82826109f7565b919050565b600067ffffffffffffffff821115610a5e57610a5d6109c8565b5b610a67826109b7565b9050602081019050919050565b82818337600083830152505050565b6000610a96610a9184610a43565b610a28565b905082815260208101848484011115610ab257610ab16109b2565b5b610abd848285610a74565b509392505050565b600082601f830112610ada57610ad96109ad565b5b8135610aea848260208601610a83565b91505092915050565b600060208284031215610b0957610b086109a3565b5b600082013567ffffffffffffffff811115610b2757610b266109a8565b5b610b3384828501610ac5565b91505092915050565b60138110610b4957600080fd5b50565b600081359050610b5b81610b3c565b92915050565b600060208284031215610b7757610b766109a3565b5b6000610b8584828501610b4c565b91505092915050565b6000819050919050565b610ba181610b8e565b8114610bac57600080fd5b50565b600081359050610bbe81610b98565b92915050565b600080600080600060a08688031215610be057610bdf6109a3565b5b6000610bee88828901610b4c565b9550506020610bff88828901610baf565b9450506040610c1088828901610baf565b9350506060610c2188828901610baf565b9250506080610c3288828901610baf565b9150509295509295909350565b600080fd5b600060208284031215610c5a57610c59610c3f565b5b610c646020610a28565b90506000610c7484828501610baf565b60008301525092915050565b600060608284031215610c9657610c95610c3f565b5b610ca06060610a28565b90506000610cb084828501610baf565b6000830152506020610cc484828501610baf565b6020830152506040610cd884828501610c44565b60408301525092915050565b60008060808385031215610cfb57610cfa6109a3565b5b6000610d0985828601610baf565b9250506020610d1a85828601610c80565b9150509250929050565b600080600060608486031215610d3d57610d3c6109a3565b5b6000610d4b86828701610b4c565b9350506020610d5c86828701610baf565b9250506040610d6d86828701610baf565b9150509250925092565b600067ffffffffffffffff821115610d9257610d916109c8565b5b602082029050602081019050919050565b600080fd5b60007fffff00000000000000000000000000000000000000000000000000000000000082169050919050565b610ddd81610da8565b8114610de857600080fd5b50565b600081359050610dfa81610dd4565b92915050565b6000610e13610e0e84610d77565b610a28565b90508083825260208201905060208402830185811115610e3657610e35610da3565b5b835b81811015610e5f5780610e4b8882610deb565b845260208401935050602081019050610e38565b5050509392505050565b600082601f830112610e7e57610e7d6109ad565b5b8135610e8e848260208601610e00565b91505092915050565b60008060408385031215610eae57610ead6109a3565b5b600083013567ffffffffffffffff811115610ecc57610ecb6109a8565b5b610ed885828601610e69565b925050602083013567ffffffffffffffff811115610ef957610ef86109a8565b5b610f0585828601610e69565b9150509250929050565b60008060008060808587031215610f2957610f286109a3565b5b6000610f3787828801610b4c565b9450506020610f4887828801610baf565b9350506040610f5987828801610baf565b9250506060610f6a87828801610baf565b91505092959194509250565b60008060408385031215610f8d57610f8c6109a3565b5b6000610f9b85828601610b4c565b9250506020610fac85828601610baf565b9150509250929050565b60008060408385031215610fcd57610fcc6109a3565b5b600083013567ffffffffffffffff811115610feb57610fea6109a8565b5b610ff785828601610ac5565b925050602083013567ffffffffffffffff811115611018576110176109a8565b5b61102485828601610ac5565b9150509250929050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006110598261102e565b9050919050565b6110698161104e565b811461107457600080fd5b50565b60008135905061108681611060565b92915050565b600080604083850312156110a3576110a26109a3565b5b60006110b185828601611077565b92505060206110c285828601611077565b9150509250929050565b600067ffffffffffffffff8211156110e7576110e66109c8565b5b6110f0826109b7565b9050602081019050919050565b600061111061110b846110cc565b610a28565b90508281526020810184848401111561112c5761112b6109b2565b5b611137848285610a74565b509392505050565b600082601f830112611154576111536109ad565b5b81356111648482602086016110fd565b91505092915050565b600060208284031215611183576111826109a3565b5b600082013567ffffffffffffffff8111156111a1576111a06109a8565b5b6111ad8482850161113f565b91505092915050565b600081519050919050565b600082825260208201905092915050565b60005b838110156111f05780820151818401526020810190506111d5565b60008484015250505050565b6000611207826111b6565b61121181856111c1565b93506112218185602086016111d2565b61122a816109b7565b840191505092915050565b6000602082019050818103600083015261124f81846111fc565b905092915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602160045260246000fd5b7f4469646e2774206d6174636820616e7920616c6c6f7761626c65206576656e7460008201527f20696e6465780000000000000000000000000000000000000000000000000000602082015250565b60006112e26026836111c1565b91506112ed82611286565b604082019050919050565b60006020820190508181036000830152611311816112d5565b9050919050565b61132181610b8e565b82525050565b600060808201905061133c6000830187611318565b6113496020830186611318565b6113566040830185611318565b6113636060830184611318565b95945050505050565b60006040820190506113816000830185611318565b61138e6020830184611318565b9392505050565b61139e81610b8e565b82525050565b6020820160008201516113ba6000850182611395565b50505050565b6060820160008201516113d66000850182611395565b5060208201516113e96020850182611395565b5060408201516113fc60408501826113a4565b50505050565b60006080820190506114176000830185611318565b61142460208301846113c0565b9392505050565b60006020820190506114406000830184611318565b92915050565b600081519050919050565b600081905092915050565b6000819050602082019050919050565b61147581610da8565b82525050565b6000611487838361146c565b60208301905092915050565b6000602082019050919050565b60006114ab82611446565b6114b58185611451565b93506114c08361145c565b8060005b838110156114f15781516114d8888261147b565b97506114e383611493565b9250506001810190506114c4565b5085935050505092915050565b600061150a82846114a0565b915081905092915050565b600082825260208201905092915050565b61152f81610da8565b82525050565b60006115418383611526565b60208301905092915050565b600061155882611446565b6115628185611515565b935061156d8361145c565b8060005b8381101561159e5781516115858882611535565b975061159083611493565b925050600181019050611571565b5085935050505092915050565b600060208201905081810360008301526115c5818461154d565b905092915050565b60006060820190506115e26000830186611318565b6115ef6020830185611318565b6115fc6040830184611318565b949350505050565b600081905092915050565b600061161a826111b6565b6116248185611604565b93506116348185602086016111d2565b80840191505092915050565b600061164c828461160f565b915081905092915050565b6116608161104e565b82525050565b600060208201905061167b6000830184611657565b92915050565b600081519050919050565b600082825260208201905092915050565b60006116a882611681565b6116b2818561168c565b93506116c28185602086016111d2565b6116cb816109b7565b840191505092915050565b600060208201905081810360008301526116f0818461169d565b905092915050565b600060408201905061170d6000830185611657565b61171a6020830184611657565b939250505056fea264697066735822122032046b888f6fa110fcef57e075d1d0dc39c921c65480e9c796549089971aa01b64736f6c63430008130033"  # noqa: E501
+EMITTER_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b506116dd8061001d5f395ff3fe608060405234801561000f575f80fd5b50600436106100b2575f3560e01c80639c3770531161006f5780639c3770531461015e578063aa6fd8221461017a578063acabb9ed14610196578063b2ddc449146101b2578063e17bf956146101ce578063f82ef69e146101ea576100b2565b80630bb563d6146100b657806317c0c180146100d257806320f0256e146100ee5780635da86c171461010a57806390b41d8b14610126578063966b50e014610142575b5f80fd5b6100d060048036038101906100cb9190610ae2565b610206565b005b6100ec60048036038101906100e79190610b4c565b610240565b005b61010860048036038101906101039190610baa565b610317565b005b610124600480360381019061011f9190610cbf565b610434565b005b610140600480360381019061013b9190610cfd565b610471565b005b61015c60048036038101906101579190610e66565b6105ce565b005b61017860048036038101906101739190610edc565b61061f565b005b610194600480360381019061018f9190610f40565b610737565b005b6101b060048036038101906101ab9190610f7e565b61087b565b005b6101cc60048036038101906101c7919061104e565b6108cc565b005b6101e860048036038101906101e3919061112a565b61091e565b005b61020460048036038101906101ff919061104e565b610958565b005b7fa95e6e2a182411e7a6f9ed114a85c3761d87f9b8f453d842c71235aa64fff99f8160405161023591906111eb565b60405180910390a150565b600160128111156102545761025361120b565b5b8160128111156102675761026661120b565b5b0361029d577f1e86022f78f8d04f8e3dfd13a2bdb280403e6632877c0dbee5e4eeb259908a5c60405160405180910390a1610314565b5f60128111156102b0576102af61120b565b5b8160128111156102c3576102c261120b565b5b036102d85760405160405180910390a0610313565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161030a906112a8565b60405180910390fd5b5b50565b6005601281111561032b5761032a61120b565b5b85601281111561033e5761033d61120b565b5b03610385577ff039d147f23fe975a4254bdf6b1502b8c79132ae1833986b7ccef2638e73fdf98484848460405161037894939291906112d5565b60405180910390a161042d565b600b60128111156103995761039861120b565b5b8560128111156103ac576103ab61120b565b5b036103f15780827fa30ece802b64cd2b7e57dabf4010aabf5df26d1556977affb07b98a77ad955b586866040516103e4929190611318565b60405180910390a361042c565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610423906112a8565b60405180910390fd5b5b5050505050565b7f8ccce2523cca5f3851d20df50b5a59509bc4ac7d9ddba344f5e331969d09b8e782826040516104659291906113a8565b60405180910390a15050565b600360128111156104855761048461120b565b5b8360128111156104985761049761120b565b5b036104db577fdf0cb1dea99afceb3ea698d62e705b736f1345a7eee9eb07e63d1f8f556c1bc582826040516104ce929190611318565b60405180910390a16105c9565b600960128111156104ef576104ee61120b565b5b8360128111156105025761050161120b565b5b0361054457807f057bc32826fbe161da1c110afcdcae7c109a8b69149f727fc37a603c60ef94ca8360405161053791906113cf565b60405180910390a26105c8565b600860128111156105585761055761120b565b5b83601281111561056b5761056a61120b565b5b0361058c57808260405161057f91906113cf565b60405180910390a16105c7565b6040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016105be906112a8565b60405180910390fd5b5b5b505050565b816040516105dc9190611499565b60405180910390207fdbc4c1d1d2f0d84e58d36ca767ec9ba2ec2f933c055e50e5ccdd57697f7b58b0826040516106139190611541565b60405180910390a25050565b600460128111156106335761063261120b565b5b8460128111156106465761064561120b565b5b0361068b577f4a25b279c7c585f25eda9788ac9420ebadae78ca6b206a0e6ab488fd81f5506283838360405161067e93929190611561565b60405180910390a1610731565b600a601281111561069f5761069e61120b565b5b8460128111156106b2576106b161120b565b5b036106f55780827ff16c999b533366ca5138d78e85da51611089cd05749f098d6c225d4cd42ee6ec856040516106e891906113cf565b60405180910390a3610730565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610727906112a8565b60405180910390fd5b5b50505050565b6002601281111561074b5761074a61120b565b5b82601281111561075e5761075d61120b565b5b0361079f577f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d48160405161079291906113cf565b60405180910390a1610877565b600760128111156107b3576107b261120b565b5b8260128111156107c6576107c561120b565b5b036107fd57807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a2610876565b600660128111156108115761081061120b565b5b8260128111156108245761082361120b565b5b0361083a578060405160405180910390a1610875565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161086c906112a8565b60405180910390fd5b5b5b5050565b8160405161088991906115d0565b60405180910390207fe77cf33df73da7bc2e253a2dae617e6f15e4e337eaa462a108903af4643d1b75826040516108c091906111eb565b60405180910390a25050565b8173ffffffffffffffffffffffffffffffffffffffff167ff922c215689548d72c3d2fe4ea8dafb2a30c43312c9b43fe5d10f713181f991c8260405161091291906115f5565b60405180910390a25050565b7f532fd6ea96cfb78bb46e09279a26828b8b493de1a2b8b1ee1face527978a15a58160405161094d9190611660565b60405180910390a150565b7f06029e18f16caae06a69281f35b00ed3fcf47950e6c99dafa1bdd8c4b93479a08282604051610989929190611680565b60405180910390a15050565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6109f4826109ae565b810181811067ffffffffffffffff82111715610a1357610a126109be565b5b80604052505050565b5f610a25610995565b9050610a3182826109eb565b919050565b5f67ffffffffffffffff821115610a5057610a4f6109be565b5b610a59826109ae565b9050602081019050919050565b828183375f83830152505050565b5f610a86610a8184610a36565b610a1c565b905082815260208101848484011115610aa257610aa16109aa565b5b610aad848285610a66565b509392505050565b5f82601f830112610ac957610ac86109a6565b5b8135610ad9848260208601610a74565b91505092915050565b5f60208284031215610af757610af661099e565b5b5f82013567ffffffffffffffff811115610b1457610b136109a2565b5b610b2084828501610ab5565b91505092915050565b60138110610b35575f80fd5b50565b5f81359050610b4681610b29565b92915050565b5f60208284031215610b6157610b6061099e565b5b5f610b6e84828501610b38565b91505092915050565b5f819050919050565b610b8981610b77565b8114610b93575f80fd5b50565b5f81359050610ba481610b80565b92915050565b5f805f805f60a08688031215610bc357610bc261099e565b5b5f610bd088828901610b38565b9550506020610be188828901610b96565b9450506040610bf288828901610b96565b9350506060610c0388828901610b96565b9250506080610c1488828901610b96565b9150509295509295909350565b5f80fd5b5f60208284031215610c3a57610c39610c21565b5b610c446020610a1c565b90505f610c5384828501610b96565b5f8301525092915050565b5f60608284031215610c7357610c72610c21565b5b610c7d6060610a1c565b90505f610c8c84828501610b96565b5f830152506020610c9f84828501610b96565b6020830152506040610cb384828501610c25565b60408301525092915050565b5f8060808385031215610cd557610cd461099e565b5b5f610ce285828601610b96565b9250506020610cf385828601610c5e565b9150509250929050565b5f805f60608486031215610d1457610d1361099e565b5b5f610d2186828701610b38565b9350506020610d3286828701610b96565b9250506040610d4386828701610b96565b9150509250925092565b5f67ffffffffffffffff821115610d6757610d666109be565b5b602082029050602081019050919050565b5f80fd5b5f7fffff00000000000000000000000000000000000000000000000000000000000082169050919050565b610db081610d7c565b8114610dba575f80fd5b50565b5f81359050610dcb81610da7565b92915050565b5f610de3610dde84610d4d565b610a1c565b90508083825260208201905060208402830185811115610e0657610e05610d78565b5b835b81811015610e2f5780610e1b8882610dbd565b845260208401935050602081019050610e08565b5050509392505050565b5f82601f830112610e4d57610e4c6109a6565b5b8135610e5d848260208601610dd1565b91505092915050565b5f8060408385031215610e7c57610e7b61099e565b5b5f83013567ffffffffffffffff811115610e9957610e986109a2565b5b610ea585828601610e39565b925050602083013567ffffffffffffffff811115610ec657610ec56109a2565b5b610ed285828601610e39565b9150509250929050565b5f805f8060808587031215610ef457610ef361099e565b5b5f610f0187828801610b38565b9450506020610f1287828801610b96565b9350506040610f2387828801610b96565b9250506060610f3487828801610b96565b91505092959194509250565b5f8060408385031215610f5657610f5561099e565b5b5f610f6385828601610b38565b9250506020610f7485828601610b96565b9150509250929050565b5f8060408385031215610f9457610f9361099e565b5b5f83013567ffffffffffffffff811115610fb157610fb06109a2565b5b610fbd85828601610ab5565b925050602083013567ffffffffffffffff811115610fde57610fdd6109a2565b5b610fea85828601610ab5565b9150509250929050565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f61101d82610ff4565b9050919050565b61102d81611013565b8114611037575f80fd5b50565b5f8135905061104881611024565b92915050565b5f80604083850312156110645761106361099e565b5b5f6110718582860161103a565b92505060206110828582860161103a565b9150509250929050565b5f67ffffffffffffffff8211156110a6576110a56109be565b5b6110af826109ae565b9050602081019050919050565b5f6110ce6110c98461108c565b610a1c565b9050828152602081018484840111156110ea576110e96109aa565b5b6110f5848285610a66565b509392505050565b5f82601f830112611111576111106109a6565b5b81356111218482602086016110bc565b91505092915050565b5f6020828403121561113f5761113e61099e565b5b5f82013567ffffffffffffffff81111561115c5761115b6109a2565b5b611168848285016110fd565b91505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156111a857808201518184015260208101905061118d565b5f8484015250505050565b5f6111bd82611171565b6111c7818561117b565b93506111d781856020860161118b565b6111e0816109ae565b840191505092915050565b5f6020820190508181035f83015261120381846111b3565b905092915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602160045260245ffd5b7f4469646e2774206d6174636820616e7920616c6c6f7761626c65206576656e745f8201527f20696e6465780000000000000000000000000000000000000000000000000000602082015250565b5f61129260268361117b565b915061129d82611238565b604082019050919050565b5f6020820190508181035f8301526112bf81611286565b9050919050565b6112cf81610b77565b82525050565b5f6080820190506112e85f8301876112c6565b6112f560208301866112c6565b61130260408301856112c6565b61130f60608301846112c6565b95945050505050565b5f60408201905061132b5f8301856112c6565b61133860208301846112c6565b9392505050565b61134881610b77565b82525050565b602082015f8201516113625f85018261133f565b50505050565b606082015f82015161137c5f85018261133f565b50602082015161138f602085018261133f565b5060408201516113a2604085018261134e565b50505050565b5f6080820190506113bb5f8301856112c6565b6113c86020830184611368565b9392505050565b5f6020820190506113e25f8301846112c6565b92915050565b5f81519050919050565b5f81905092915050565b5f819050602082019050919050565b61141481610d7c565b82525050565b5f611425838361140b565b60208301905092915050565b5f602082019050919050565b5f611447826113e8565b61145181856113f2565b935061145c836113fc565b805f5b8381101561148c578151611473888261141a565b975061147e83611431565b92505060018101905061145f565b5085935050505092915050565b5f6114a4828461143d565b915081905092915050565b5f82825260208201905092915050565b6114c881610d7c565b82525050565b5f6114d983836114bf565b60208301905092915050565b5f6114ef826113e8565b6114f981856114af565b9350611504836113fc565b805f5b8381101561153457815161151b88826114ce565b975061152683611431565b925050600181019050611507565b5085935050505092915050565b5f6020820190508181035f83015261155981846114e5565b905092915050565b5f6060820190506115745f8301866112c6565b61158160208301856112c6565b61158e60408301846112c6565b949350505050565b5f81905092915050565b5f6115aa82611171565b6115b48185611596565b93506115c481856020860161118b565b80840191505092915050565b5f6115db82846115a0565b915081905092915050565b6115ef81611013565b82525050565b5f6020820190506116085f8301846115e6565b92915050565b5f81519050919050565b5f82825260208201905092915050565b5f6116328261160e565b61163c8185611618565b935061164c81856020860161118b565b611655816109ae565b840191505092915050565b5f6020820190508181035f8301526116788184611628565b905092915050565b5f6040820190506116935f8301856115e6565b6116a060208301846115e6565b939250505056fea26469706673582212203a9f8d99e43e7a7100fe2b0b2a9096d37ef438b62e771f2ec364ba6fdfa499fa64736f6c63430008140033"  # noqa: E501
+EMITTER_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b50600436106100b2575f3560e01c80639c3770531161006f5780639c3770531461015e578063aa6fd8221461017a578063acabb9ed14610196578063b2ddc449146101b2578063e17bf956146101ce578063f82ef69e146101ea576100b2565b80630bb563d6146100b657806317c0c180146100d257806320f0256e146100ee5780635da86c171461010a57806390b41d8b14610126578063966b50e014610142575b5f80fd5b6100d060048036038101906100cb9190610ae2565b610206565b005b6100ec60048036038101906100e79190610b4c565b610240565b005b61010860048036038101906101039190610baa565b610317565b005b610124600480360381019061011f9190610cbf565b610434565b005b610140600480360381019061013b9190610cfd565b610471565b005b61015c60048036038101906101579190610e66565b6105ce565b005b61017860048036038101906101739190610edc565b61061f565b005b610194600480360381019061018f9190610f40565b610737565b005b6101b060048036038101906101ab9190610f7e565b61087b565b005b6101cc60048036038101906101c7919061104e565b6108cc565b005b6101e860048036038101906101e3919061112a565b61091e565b005b61020460048036038101906101ff919061104e565b610958565b005b7fa95e6e2a182411e7a6f9ed114a85c3761d87f9b8f453d842c71235aa64fff99f8160405161023591906111eb565b60405180910390a150565b600160128111156102545761025361120b565b5b8160128111156102675761026661120b565b5b0361029d577f1e86022f78f8d04f8e3dfd13a2bdb280403e6632877c0dbee5e4eeb259908a5c60405160405180910390a1610314565b5f60128111156102b0576102af61120b565b5b8160128111156102c3576102c261120b565b5b036102d85760405160405180910390a0610313565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161030a906112a8565b60405180910390fd5b5b50565b6005601281111561032b5761032a61120b565b5b85601281111561033e5761033d61120b565b5b03610385577ff039d147f23fe975a4254bdf6b1502b8c79132ae1833986b7ccef2638e73fdf98484848460405161037894939291906112d5565b60405180910390a161042d565b600b60128111156103995761039861120b565b5b8560128111156103ac576103ab61120b565b5b036103f15780827fa30ece802b64cd2b7e57dabf4010aabf5df26d1556977affb07b98a77ad955b586866040516103e4929190611318565b60405180910390a361042c565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610423906112a8565b60405180910390fd5b5b5050505050565b7f8ccce2523cca5f3851d20df50b5a59509bc4ac7d9ddba344f5e331969d09b8e782826040516104659291906113a8565b60405180910390a15050565b600360128111156104855761048461120b565b5b8360128111156104985761049761120b565b5b036104db577fdf0cb1dea99afceb3ea698d62e705b736f1345a7eee9eb07e63d1f8f556c1bc582826040516104ce929190611318565b60405180910390a16105c9565b600960128111156104ef576104ee61120b565b5b8360128111156105025761050161120b565b5b0361054457807f057bc32826fbe161da1c110afcdcae7c109a8b69149f727fc37a603c60ef94ca8360405161053791906113cf565b60405180910390a26105c8565b600860128111156105585761055761120b565b5b83601281111561056b5761056a61120b565b5b0361058c57808260405161057f91906113cf565b60405180910390a16105c7565b6040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016105be906112a8565b60405180910390fd5b5b5b505050565b816040516105dc9190611499565b60405180910390207fdbc4c1d1d2f0d84e58d36ca767ec9ba2ec2f933c055e50e5ccdd57697f7b58b0826040516106139190611541565b60405180910390a25050565b600460128111156106335761063261120b565b5b8460128111156106465761064561120b565b5b0361068b577f4a25b279c7c585f25eda9788ac9420ebadae78ca6b206a0e6ab488fd81f5506283838360405161067e93929190611561565b60405180910390a1610731565b600a601281111561069f5761069e61120b565b5b8460128111156106b2576106b161120b565b5b036106f55780827ff16c999b533366ca5138d78e85da51611089cd05749f098d6c225d4cd42ee6ec856040516106e891906113cf565b60405180910390a3610730565b6040517f08c379a0000000000000000000000000000000000000000000000000000000008152600401610727906112a8565b60405180910390fd5b5b50505050565b6002601281111561074b5761074a61120b565b5b82601281111561075e5761075d61120b565b5b0361079f577f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d48160405161079291906113cf565b60405180910390a1610877565b600760128111156107b3576107b261120b565b5b8260128111156107c6576107c561120b565b5b036107fd57807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a2610876565b600660128111156108115761081061120b565b5b8260128111156108245761082361120b565b5b0361083a578060405160405180910390a1610875565b6040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161086c906112a8565b60405180910390fd5b5b5b5050565b8160405161088991906115d0565b60405180910390207fe77cf33df73da7bc2e253a2dae617e6f15e4e337eaa462a108903af4643d1b75826040516108c091906111eb565b60405180910390a25050565b8173ffffffffffffffffffffffffffffffffffffffff167ff922c215689548d72c3d2fe4ea8dafb2a30c43312c9b43fe5d10f713181f991c8260405161091291906115f5565b60405180910390a25050565b7f532fd6ea96cfb78bb46e09279a26828b8b493de1a2b8b1ee1face527978a15a58160405161094d9190611660565b60405180910390a150565b7f06029e18f16caae06a69281f35b00ed3fcf47950e6c99dafa1bdd8c4b93479a08282604051610989929190611680565b60405180910390a15050565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6109f4826109ae565b810181811067ffffffffffffffff82111715610a1357610a126109be565b5b80604052505050565b5f610a25610995565b9050610a3182826109eb565b919050565b5f67ffffffffffffffff821115610a5057610a4f6109be565b5b610a59826109ae565b9050602081019050919050565b828183375f83830152505050565b5f610a86610a8184610a36565b610a1c565b905082815260208101848484011115610aa257610aa16109aa565b5b610aad848285610a66565b509392505050565b5f82601f830112610ac957610ac86109a6565b5b8135610ad9848260208601610a74565b91505092915050565b5f60208284031215610af757610af661099e565b5b5f82013567ffffffffffffffff811115610b1457610b136109a2565b5b610b2084828501610ab5565b91505092915050565b60138110610b35575f80fd5b50565b5f81359050610b4681610b29565b92915050565b5f60208284031215610b6157610b6061099e565b5b5f610b6e84828501610b38565b91505092915050565b5f819050919050565b610b8981610b77565b8114610b93575f80fd5b50565b5f81359050610ba481610b80565b92915050565b5f805f805f60a08688031215610bc357610bc261099e565b5b5f610bd088828901610b38565b9550506020610be188828901610b96565b9450506040610bf288828901610b96565b9350506060610c0388828901610b96565b9250506080610c1488828901610b96565b9150509295509295909350565b5f80fd5b5f60208284031215610c3a57610c39610c21565b5b610c446020610a1c565b90505f610c5384828501610b96565b5f8301525092915050565b5f60608284031215610c7357610c72610c21565b5b610c7d6060610a1c565b90505f610c8c84828501610b96565b5f830152506020610c9f84828501610b96565b6020830152506040610cb384828501610c25565b60408301525092915050565b5f8060808385031215610cd557610cd461099e565b5b5f610ce285828601610b96565b9250506020610cf385828601610c5e565b9150509250929050565b5f805f60608486031215610d1457610d1361099e565b5b5f610d2186828701610b38565b9350506020610d3286828701610b96565b9250506040610d4386828701610b96565b9150509250925092565b5f67ffffffffffffffff821115610d6757610d666109be565b5b602082029050602081019050919050565b5f80fd5b5f7fffff00000000000000000000000000000000000000000000000000000000000082169050919050565b610db081610d7c565b8114610dba575f80fd5b50565b5f81359050610dcb81610da7565b92915050565b5f610de3610dde84610d4d565b610a1c565b90508083825260208201905060208402830185811115610e0657610e05610d78565b5b835b81811015610e2f5780610e1b8882610dbd565b845260208401935050602081019050610e08565b5050509392505050565b5f82601f830112610e4d57610e4c6109a6565b5b8135610e5d848260208601610dd1565b91505092915050565b5f8060408385031215610e7c57610e7b61099e565b5b5f83013567ffffffffffffffff811115610e9957610e986109a2565b5b610ea585828601610e39565b925050602083013567ffffffffffffffff811115610ec657610ec56109a2565b5b610ed285828601610e39565b9150509250929050565b5f805f8060808587031215610ef457610ef361099e565b5b5f610f0187828801610b38565b9450506020610f1287828801610b96565b9350506040610f2387828801610b96565b9250506060610f3487828801610b96565b91505092959194509250565b5f8060408385031215610f5657610f5561099e565b5b5f610f6385828601610b38565b9250506020610f7485828601610b96565b9150509250929050565b5f8060408385031215610f9457610f9361099e565b5b5f83013567ffffffffffffffff811115610fb157610fb06109a2565b5b610fbd85828601610ab5565b925050602083013567ffffffffffffffff811115610fde57610fdd6109a2565b5b610fea85828601610ab5565b9150509250929050565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f61101d82610ff4565b9050919050565b61102d81611013565b8114611037575f80fd5b50565b5f8135905061104881611024565b92915050565b5f80604083850312156110645761106361099e565b5b5f6110718582860161103a565b92505060206110828582860161103a565b9150509250929050565b5f67ffffffffffffffff8211156110a6576110a56109be565b5b6110af826109ae565b9050602081019050919050565b5f6110ce6110c98461108c565b610a1c565b9050828152602081018484840111156110ea576110e96109aa565b5b6110f5848285610a66565b509392505050565b5f82601f830112611111576111106109a6565b5b81356111218482602086016110bc565b91505092915050565b5f6020828403121561113f5761113e61099e565b5b5f82013567ffffffffffffffff81111561115c5761115b6109a2565b5b611168848285016110fd565b91505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156111a857808201518184015260208101905061118d565b5f8484015250505050565b5f6111bd82611171565b6111c7818561117b565b93506111d781856020860161118b565b6111e0816109ae565b840191505092915050565b5f6020820190508181035f83015261120381846111b3565b905092915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602160045260245ffd5b7f4469646e2774206d6174636820616e7920616c6c6f7761626c65206576656e745f8201527f20696e6465780000000000000000000000000000000000000000000000000000602082015250565b5f61129260268361117b565b915061129d82611238565b604082019050919050565b5f6020820190508181035f8301526112bf81611286565b9050919050565b6112cf81610b77565b82525050565b5f6080820190506112e85f8301876112c6565b6112f560208301866112c6565b61130260408301856112c6565b61130f60608301846112c6565b95945050505050565b5f60408201905061132b5f8301856112c6565b61133860208301846112c6565b9392505050565b61134881610b77565b82525050565b602082015f8201516113625f85018261133f565b50505050565b606082015f82015161137c5f85018261133f565b50602082015161138f602085018261133f565b5060408201516113a2604085018261134e565b50505050565b5f6080820190506113bb5f8301856112c6565b6113c86020830184611368565b9392505050565b5f6020820190506113e25f8301846112c6565b92915050565b5f81519050919050565b5f81905092915050565b5f819050602082019050919050565b61141481610d7c565b82525050565b5f611425838361140b565b60208301905092915050565b5f602082019050919050565b5f611447826113e8565b61145181856113f2565b935061145c836113fc565b805f5b8381101561148c578151611473888261141a565b975061147e83611431565b92505060018101905061145f565b5085935050505092915050565b5f6114a4828461143d565b915081905092915050565b5f82825260208201905092915050565b6114c881610d7c565b82525050565b5f6114d983836114bf565b60208301905092915050565b5f6114ef826113e8565b6114f981856114af565b9350611504836113fc565b805f5b8381101561153457815161151b88826114ce565b975061152683611431565b925050600181019050611507565b5085935050505092915050565b5f6020820190508181035f83015261155981846114e5565b905092915050565b5f6060820190506115745f8301866112c6565b61158160208301856112c6565b61158e60408301846112c6565b949350505050565b5f81905092915050565b5f6115aa82611171565b6115b48185611596565b93506115c481856020860161118b565b80840191505092915050565b5f6115db82846115a0565b915081905092915050565b6115ef81611013565b82525050565b5f6020820190506116085f8301846115e6565b92915050565b5f81519050919050565b5f82825260208201905092915050565b5f6116328261160e565b61163c8185611618565b935061164c81856020860161118b565b611655816109ae565b840191505092915050565b5f6020820190508181035f8301526116788184611628565b905092915050565b5f6040820190506116935f8301856115e6565b6116a060208301846115e6565b939250505056fea26469706673582212203a9f8d99e43e7a7100fe2b0b2a9096d37ef438b62e771f2ec364ba6fdfa499fa64736f6c63430008140033"  # noqa: E501
 EMITTER_CONTRACT_ABI = [
     {
         "anonymous": False,
         "inputs": [
             {
                 "indexed": True,
                 "internalType": "address",
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/event_contracts.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/event_contracts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/EventContracts.sol:EventContract
-EVENT_CONTRACT_BYTECODE = "0x608060405234801561001057600080fd5b50610185806100206000396000f3fe608060405234801561001057600080fd5b506004361061002b5760003560e01c80635818fad714610030575b600080fd5b61004a600480360381019061004591906100f8565b61004c565b005b7ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb158160405161007b9190610134565b60405180910390a17f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100b29190610134565b60405180910390a150565b600080fd5b6000819050919050565b6100d5816100c2565b81146100e057600080fd5b50565b6000813590506100f2816100cc565b92915050565b60006020828403121561010e5761010d6100bd565b5b600061011c848285016100e3565b91505092915050565b61012e816100c2565b82525050565b60006020820190506101496000830184610125565b9291505056fea2646970667358221220722d2c8e718484643ec6e2a231cf7652e5dc0660ce16ca85abd3e52518abd80164736f6c63430008130033"  # noqa: E501
-EVENT_CONTRACT_RUNTIME = "0x608060405234801561001057600080fd5b506004361061002b5760003560e01c80635818fad714610030575b600080fd5b61004a600480360381019061004591906100f8565b61004c565b005b7ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb158160405161007b9190610134565b60405180910390a17f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100b29190610134565b60405180910390a150565b600080fd5b6000819050919050565b6100d5816100c2565b81146100e057600080fd5b50565b6000813590506100f2816100cc565b92915050565b60006020828403121561010e5761010d6100bd565b5b600061011c848285016100e3565b91505092915050565b61012e816100c2565b82525050565b60006020820190506101496000830184610125565b9291505056fea2646970667358221220722d2c8e718484643ec6e2a231cf7652e5dc0660ce16ca85abd3e52518abd80164736f6c63430008130033"  # noqa: E501
+EVENT_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b5061017a8061001d5f395ff3fe608060405234801561000f575f80fd5b5060043610610029575f3560e01c80635818fad71461002d575b5f80fd5b610047600480360381019061004291906100f1565b610049565b005b7ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1581604051610078919061012b565b60405180910390a17f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100af919061012b565b60405180910390a150565b5f80fd5b5f819050919050565b6100d0816100be565b81146100da575f80fd5b50565b5f813590506100eb816100c7565b92915050565b5f60208284031215610106576101056100ba565b5b5f610113848285016100dd565b91505092915050565b610125816100be565b82525050565b5f60208201905061013e5f83018461011c565b9291505056fea2646970667358221220a74d657dddf878b6ea41057e71e2057e1eca051c8b54ba30237d6df5a4e8857964736f6c63430008140033"  # noqa: E501
+EVENT_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b5060043610610029575f3560e01c80635818fad71461002d575b5f80fd5b610047600480360381019061004291906100f1565b610049565b005b7ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1581604051610078919061012b565b60405180910390a17f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100af919061012b565b60405180910390a150565b5f80fd5b5f819050919050565b6100d0816100be565b81146100da575f80fd5b50565b5f813590506100eb816100c7565b92915050565b5f60208284031215610106576101056100ba565b5b5f610113848285016100dd565b91505092915050565b610125816100be565b82525050565b5f60208201905061013e5f83018461011c565b9291505056fea2646970667358221220a74d657dddf878b6ea41057e71e2057e1eca051c8b54ba30237d6df5a4e8857964736f6c63430008140033"  # noqa: E501
 EVENT_CONTRACT_ABI = [
     {
         "anonymous": False,
         "inputs": [
             {
                 "indexed": False,
                 "internalType": "uint256",
@@ -45,16 +45,16 @@
     "bytecode": EVENT_CONTRACT_BYTECODE,
     "bytecode_runtime": EVENT_CONTRACT_RUNTIME,
     "abi": EVENT_CONTRACT_ABI,
 }
 
 
 # source: web3/_utils/contract_sources/EventContracts.sol:IndexedEventContract
-INDEXED_EVENT_CONTRACT_BYTECODE = "0x608060405234801561001057600080fd5b5061017b806100206000396000f3fe608060405234801561001057600080fd5b506004361061002b5760003560e01c80635818fad714610030575b600080fd5b61004a600480360381019061004591906100ee565b61004c565b005b807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a27f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100a8919061012a565b60405180910390a150565b600080fd5b6000819050919050565b6100cb816100b8565b81146100d657600080fd5b50565b6000813590506100e8816100c2565b92915050565b600060208284031215610104576101036100b3565b5b6000610112848285016100d9565b91505092915050565b610124816100b8565b82525050565b600060208201905061013f600083018461011b565b9291505056fea2646970667358221220e3ae4f34b41d4603e54206e0c06c86c3b16bdd5d8fcbb6876dd3205457c7b2eb64736f6c63430008130033"  # noqa: E501
-INDEXED_EVENT_CONTRACT_RUNTIME = "0x608060405234801561001057600080fd5b506004361061002b5760003560e01c80635818fad714610030575b600080fd5b61004a600480360381019061004591906100ee565b61004c565b005b807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a27f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100a8919061012a565b60405180910390a150565b600080fd5b6000819050919050565b6100cb816100b8565b81146100d657600080fd5b50565b6000813590506100e8816100c2565b92915050565b600060208284031215610104576101036100b3565b5b6000610112848285016100d9565b91505092915050565b610124816100b8565b82525050565b600060208201905061013f600083018461011b565b9291505056fea2646970667358221220e3ae4f34b41d4603e54206e0c06c86c3b16bdd5d8fcbb6876dd3205457c7b2eb64736f6c63430008130033"  # noqa: E501
+INDEXED_EVENT_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b506101708061001d5f395ff3fe608060405234801561000f575f80fd5b5060043610610029575f3560e01c80635818fad71461002d575b5f80fd5b610047600480360381019061004291906100e7565b610049565b005b807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a27f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100a59190610121565b60405180910390a150565b5f80fd5b5f819050919050565b6100c6816100b4565b81146100d0575f80fd5b50565b5f813590506100e1816100bd565b92915050565b5f602082840312156100fc576100fb6100b0565b5b5f610109848285016100d3565b91505092915050565b61011b816100b4565b82525050565b5f6020820190506101345f830184610112565b9291505056fea2646970667358221220e7ebe2ab727aab62c9912b25cb11a2482e49f8ac679173379069bc303ae61ad164736f6c63430008140033"  # noqa: E501
+INDEXED_EVENT_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b5060043610610029575f3560e01c80635818fad71461002d575b5f80fd5b610047600480360381019061004291906100e7565b610049565b005b807ff70fe689e290d8ce2b2a388ac28db36fbb0e16a6d89c6804c461f65a1b40bb1560405160405180910390a27f56d2ef3c5228bf5d88573621e325a4672ab50e033749a601e4f4a5e1dce905d4816040516100a59190610121565b60405180910390a150565b5f80fd5b5f819050919050565b6100c6816100b4565b81146100d0575f80fd5b50565b5f813590506100e1816100bd565b92915050565b5f602082840312156100fc576100fb6100b0565b5b5f610109848285016100d3565b91505092915050565b61011b816100b4565b82525050565b5f6020820190506101345f830184610112565b9291505056fea2646970667358221220e7ebe2ab727aab62c9912b25cb11a2482e49f8ac679173379069bc303ae61ad164736f6c63430008140033"  # noqa: E501
 INDEXED_EVENT_CONTRACT_ABI = [
     {
         "anonymous": False,
         "inputs": [
             {
                 "indexed": False,
                 "internalType": "uint256",
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/extended_resolver.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/extended_resolver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/ExtendedResolver.sol:ExtendedResolver
-EXTENDED_RESOLVER_BYTECODE = "0x608060405234801561001057600080fd5b50604051610d90380380610d90833981810160405281019061003291906100ed565b806000806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff1602179055505061011a565b600080fd5b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006100a88261007d565b9050919050565b60006100ba8261009d565b9050919050565b6100ca816100af565b81146100d557600080fd5b50565b6000815190506100e7816100c1565b92915050565b60006020828403121561010357610102610078565b5b6000610111848285016100d8565b91505092915050565b610c67806101296000396000f3fe608060405234801561001057600080fd5b506004361061004c5760003560e01c806301ffc9a7146100515780633e9ce794146100815780639061b9231461009d578063f86bc879146100cd575b600080fd5b61006b60048036038101906100669190610554565b6100fd565b604051610078919061059c565b60405180910390f35b61009b60048036038101906100969190610677565b61015e565b005b6100b760048036038101906100b2919061072f565b610245565b6040516100c49190610840565b60405180910390f35b6100e760048036038101906100e29190610862565b610465565b6040516100f4919061059c565b60405180910390f35b6000639061b92360e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191614806101575750610156826104a1565b5b9050919050565b806001600085815260200190815260200160002060003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548160ff0219169083151502179055507fe1c5610a6e0cbe10764ecd182adcef1ec338dc4e199c99c32ce98f38e12791df8333848460405161023894939291906108d3565b60405180910390a1505050565b60606040518060400160405280601781526020017f11657874656e6465642d7265736f6c7665720365746800000000000000000000815250805190602001208585604051610294929190610957565b60405180910390201480156102ad575060248383905010155b1561035e577ff0a378cc2afe91730d0105e67d6bb037cc5b8b6bfec5b5962d9b637ff6497e5560001b83836004906024926102ea9392919061097a565b906102f591906109cd565b14610335576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161032c90610aaf565b60405180910390fd5b61beef6040516020016103489190610acf565b604051602081830303815290604052905061045d565b60008585600081811061037457610373610aea565b5b9050013560f81c60f81b60f81c60ff1690506040518060400160405280601781526020017f11657874656e6465642d7265736f6c76657203657468000000000000000000008152508051906020012086868360016103d29190610b52565b9080926103e19392919061097a565b6040516103ef929190610b86565b604051809103902014610437576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161042e90610c11565b60405180910390fd5b61dead60405160200161044a9190610acf565b6040516020818303038152906040529150505b949350505050565b6001602052826000526040600020602052816000526040600020602052806000526040600020600092509250509054906101000a900460ff1681565b60006301ffc9a760e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916149050919050565b600080fd5b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610531816104fc565b811461053c57600080fd5b50565b60008135905061054e81610528565b92915050565b60006020828403121561056a576105696104f2565b5b60006105788482850161053f565b91505092915050565b60008115159050919050565b61059681610581565b82525050565b60006020820190506105b1600083018461058d565b92915050565b6000819050919050565b6105ca816105b7565b81146105d557600080fd5b50565b6000813590506105e7816105c1565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b6000610618826105ed565b9050919050565b6106288161060d565b811461063357600080fd5b50565b6000813590506106458161061f565b92915050565b61065481610581565b811461065f57600080fd5b50565b6000813590506106718161064b565b92915050565b6000806000606084860312156106905761068f6104f2565b5b600061069e868287016105d8565b93505060206106af86828701610636565b92505060406106c086828701610662565b9150509250925092565b600080fd5b600080fd5b600080fd5b60008083601f8401126106ef576106ee6106ca565b5b8235905067ffffffffffffffff81111561070c5761070b6106cf565b5b602083019150836001820283011115610728576107276106d4565b5b9250929050565b60008060008060408587031215610749576107486104f2565b5b600085013567ffffffffffffffff811115610767576107666104f7565b5b610773878288016106d9565b9450945050602085013567ffffffffffffffff811115610796576107956104f7565b5b6107a2878288016106d9565b925092505092959194509250565b600081519050919050565b600082825260208201905092915050565b60005b838110156107ea5780820151818401526020810190506107cf565b60008484015250505050565b6000601f19601f8301169050919050565b6000610812826107b0565b61081c81856107bb565b935061082c8185602086016107cc565b610835816107f6565b840191505092915050565b6000602082019050818103600083015261085a8184610807565b905092915050565b60008060006060848603121561087b5761087a6104f2565b5b6000610889868287016105d8565b935050602061089a86828701610636565b92505060406108ab86828701610636565b9150509250925092565b6108be816105b7565b82525050565b6108cd8161060d565b82525050565b60006080820190506108e860008301876108b5565b6108f560208301866108c4565b61090260408301856108c4565b61090f606083018461058d565b95945050505050565b600081905092915050565b82818337600083830152505050565b600061093e8385610918565b935061094b838584610923565b82840190509392505050565b6000610964828486610932565b91508190509392505050565b600080fd5b600080fd5b6000808585111561098e5761098d610970565b5b8386111561099f5761099e610975565b5b6001850283019150848603905094509492505050565b600082905092915050565b600082821b905092915050565b60006109d983836109b5565b826109e481356105b7565b92506020821015610a2457610a1f7fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff836020036008026109c0565b831692505b505092915050565b600082825260208201905092915050565b7f706172656e7420646f6d61696e206e6f742076616c696461746564206170707260008201527f6f7072696174656c790000000000000000000000000000000000000000000000602082015250565b6000610a99602983610a2c565b9150610aa482610a3d565b604082019050919050565b60006020820190508181036000830152610ac881610a8c565b9050919050565b6000602082019050610ae460008301846108c4565b92915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052603260045260246000fd5b6000819050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b6000610b5d82610b19565b9150610b6883610b19565b9250828201905080821115610b8057610b7f610b23565b5b92915050565b6000610b93828486610932565b91508190509392505050565b7f737562646f6d61696e206e6f742076616c69646174656420617070726f70726960008201527f6174656c79000000000000000000000000000000000000000000000000000000602082015250565b6000610bfb602583610a2c565b9150610c0682610b9f565b604082019050919050565b60006020820190508181036000830152610c2a81610bee565b905091905056fea2646970667358221220b4a07e5c49c4c40acfce45f221d05911195626c497b39e3584fe123647de236464736f6c63430008130033"  # noqa: E501
-EXTENDED_RESOLVER_RUNTIME = "0x608060405234801561001057600080fd5b506004361061004c5760003560e01c806301ffc9a7146100515780633e9ce794146100815780639061b9231461009d578063f86bc879146100cd575b600080fd5b61006b60048036038101906100669190610554565b6100fd565b604051610078919061059c565b60405180910390f35b61009b60048036038101906100969190610677565b61015e565b005b6100b760048036038101906100b2919061072f565b610245565b6040516100c49190610840565b60405180910390f35b6100e760048036038101906100e29190610862565b610465565b6040516100f4919061059c565b60405180910390f35b6000639061b92360e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff191614806101575750610156826104a1565b5b9050919050565b806001600085815260200190815260200160002060003373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060008473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff16815260200190815260200160002060006101000a81548160ff0219169083151502179055507fe1c5610a6e0cbe10764ecd182adcef1ec338dc4e199c99c32ce98f38e12791df8333848460405161023894939291906108d3565b60405180910390a1505050565b60606040518060400160405280601781526020017f11657874656e6465642d7265736f6c7665720365746800000000000000000000815250805190602001208585604051610294929190610957565b60405180910390201480156102ad575060248383905010155b1561035e577ff0a378cc2afe91730d0105e67d6bb037cc5b8b6bfec5b5962d9b637ff6497e5560001b83836004906024926102ea9392919061097a565b906102f591906109cd565b14610335576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161032c90610aaf565b60405180910390fd5b61beef6040516020016103489190610acf565b604051602081830303815290604052905061045d565b60008585600081811061037457610373610aea565b5b9050013560f81c60f81b60f81c60ff1690506040518060400160405280601781526020017f11657874656e6465642d7265736f6c76657203657468000000000000000000008152508051906020012086868360016103d29190610b52565b9080926103e19392919061097a565b6040516103ef929190610b86565b604051809103902014610437576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161042e90610c11565b60405180910390fd5b61dead60405160200161044a9190610acf565b6040516020818303038152906040529150505b949350505050565b6001602052826000526040600020602052816000526040600020602052806000526040600020600092509250509054906101000a900460ff1681565b60006301ffc9a760e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916149050919050565b600080fd5b600080fd5b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610531816104fc565b811461053c57600080fd5b50565b60008135905061054e81610528565b92915050565b60006020828403121561056a576105696104f2565b5b60006105788482850161053f565b91505092915050565b60008115159050919050565b61059681610581565b82525050565b60006020820190506105b1600083018461058d565b92915050565b6000819050919050565b6105ca816105b7565b81146105d557600080fd5b50565b6000813590506105e7816105c1565b92915050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b6000610618826105ed565b9050919050565b6106288161060d565b811461063357600080fd5b50565b6000813590506106458161061f565b92915050565b61065481610581565b811461065f57600080fd5b50565b6000813590506106718161064b565b92915050565b6000806000606084860312156106905761068f6104f2565b5b600061069e868287016105d8565b93505060206106af86828701610636565b92505060406106c086828701610662565b9150509250925092565b600080fd5b600080fd5b600080fd5b60008083601f8401126106ef576106ee6106ca565b5b8235905067ffffffffffffffff81111561070c5761070b6106cf565b5b602083019150836001820283011115610728576107276106d4565b5b9250929050565b60008060008060408587031215610749576107486104f2565b5b600085013567ffffffffffffffff811115610767576107666104f7565b5b610773878288016106d9565b9450945050602085013567ffffffffffffffff811115610796576107956104f7565b5b6107a2878288016106d9565b925092505092959194509250565b600081519050919050565b600082825260208201905092915050565b60005b838110156107ea5780820151818401526020810190506107cf565b60008484015250505050565b6000601f19601f8301169050919050565b6000610812826107b0565b61081c81856107bb565b935061082c8185602086016107cc565b610835816107f6565b840191505092915050565b6000602082019050818103600083015261085a8184610807565b905092915050565b60008060006060848603121561087b5761087a6104f2565b5b6000610889868287016105d8565b935050602061089a86828701610636565b92505060406108ab86828701610636565b9150509250925092565b6108be816105b7565b82525050565b6108cd8161060d565b82525050565b60006080820190506108e860008301876108b5565b6108f560208301866108c4565b61090260408301856108c4565b61090f606083018461058d565b95945050505050565b600081905092915050565b82818337600083830152505050565b600061093e8385610918565b935061094b838584610923565b82840190509392505050565b6000610964828486610932565b91508190509392505050565b600080fd5b600080fd5b6000808585111561098e5761098d610970565b5b8386111561099f5761099e610975565b5b6001850283019150848603905094509492505050565b600082905092915050565b600082821b905092915050565b60006109d983836109b5565b826109e481356105b7565b92506020821015610a2457610a1f7fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff836020036008026109c0565b831692505b505092915050565b600082825260208201905092915050565b7f706172656e7420646f6d61696e206e6f742076616c696461746564206170707260008201527f6f7072696174656c790000000000000000000000000000000000000000000000602082015250565b6000610a99602983610a2c565b9150610aa482610a3d565b604082019050919050565b60006020820190508181036000830152610ac881610a8c565b9050919050565b6000602082019050610ae460008301846108c4565b92915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052603260045260246000fd5b6000819050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b6000610b5d82610b19565b9150610b6883610b19565b9250828201905080821115610b8057610b7f610b23565b5b92915050565b6000610b93828486610932565b91508190509392505050565b7f737562646f6d61696e206e6f742076616c69646174656420617070726f70726960008201527f6174656c79000000000000000000000000000000000000000000000000000000602082015250565b6000610bfb602583610a2c565b9150610c0682610b9f565b604082019050919050565b60006020820190508181036000830152610c2a81610bee565b905091905056fea2646970667358221220b4a07e5c49c4c40acfce45f221d05911195626c497b39e3584fe123647de236464736f6c63430008130033"  # noqa: E501
+EXTENDED_RESOLVER_BYTECODE = "0x608060405234801561000f575f80fd5b50604051610d28380380610d28833981810160405281019061003191906100e5565b805f806101000a81548173ffffffffffffffffffffffffffffffffffffffff021916908373ffffffffffffffffffffffffffffffffffffffff16021790555050610110565b5f80fd5b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6100a38261007a565b9050919050565b5f6100b482610099565b9050919050565b6100c4816100aa565b81146100ce575f80fd5b50565b5f815190506100df816100bb565b92915050565b5f602082840312156100fa576100f9610076565b5b5f610107848285016100d1565b91505092915050565b610c0b8061011d5f395ff3fe608060405234801561000f575f80fd5b506004361061004a575f3560e01c806301ffc9a71461004e5780633e9ce7941461007e5780639061b9231461009a578063f86bc879146100ca575b5f80fd5b61006860048036038101906100639190610539565b6100fa565b604051610075919061057e565b60405180910390f35b6100986004803603810190610093919061064e565b61015a565b005b6100b460048036038101906100af91906106ff565b61023a565b6040516100c19190610807565b60405180910390f35b6100e460048036038101906100df9190610827565b610457565b6040516100f1919061057e565b60405180910390f35b5f639061b92360e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916148061015357506101528261048c565b5b9050919050565b8060015f8581526020019081526020015f205f3373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020015f205f8473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020015f205f6101000a81548160ff0219169083151502179055507fe1c5610a6e0cbe10764ecd182adcef1ec338dc4e199c99c32ce98f38e12791df8333848460405161022d9493929190610895565b60405180910390a1505050565b60606040518060400160405280601781526020017f11657874656e6465642d7265736f6c7665720365746800000000000000000000815250805190602001208585604051610289929190610914565b60405180910390201480156102a2575060248383905010155b15610352577ff0a378cc2afe91730d0105e67d6bb037cc5b8b6bfec5b5962d9b637ff6497e555f1b83836004906024926102de93929190610934565b906102e99190610984565b14610329576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161032090610a62565b60405180910390fd5b61beef60405160200161033c9190610a80565b604051602081830303815290604052905061044f565b5f85855f81811061036657610365610a99565b5b9050013560f81c60f81b60f81c60ff1690506040518060400160405280601781526020017f11657874656e6465642d7265736f6c76657203657468000000000000000000008152508051906020012086868360016103c49190610afc565b9080926103d393929190610934565b6040516103e1929190610b2f565b604051809103902014610429576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161042090610bb7565b60405180910390fd5b61dead60405160200161043c9190610a80565b6040516020818303038152906040529150505b949350505050565b6001602052825f5260405f20602052815f5260405f20602052805f5260405f205f92509250509054906101000a900460ff1681565b5f6301ffc9a760e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916149050919050565b5f80fd5b5f80fd5b5f7fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610518816104e4565b8114610522575f80fd5b50565b5f813590506105338161050f565b92915050565b5f6020828403121561054e5761054d6104dc565b5b5f61055b84828501610525565b91505092915050565b5f8115159050919050565b61057881610564565b82525050565b5f6020820190506105915f83018461056f565b92915050565b5f819050919050565b6105a981610597565b81146105b3575f80fd5b50565b5f813590506105c4816105a0565b92915050565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6105f3826105ca565b9050919050565b610603816105e9565b811461060d575f80fd5b50565b5f8135905061061e816105fa565b92915050565b61062d81610564565b8114610637575f80fd5b50565b5f8135905061064881610624565b92915050565b5f805f60608486031215610665576106646104dc565b5b5f610672868287016105b6565b935050602061068386828701610610565b92505060406106948682870161063a565b9150509250925092565b5f80fd5b5f80fd5b5f80fd5b5f8083601f8401126106bf576106be61069e565b5b8235905067ffffffffffffffff8111156106dc576106db6106a2565b5b6020830191508360018202830111156106f8576106f76106a6565b5b9250929050565b5f805f8060408587031215610717576107166104dc565b5b5f85013567ffffffffffffffff811115610734576107336104e0565b5b610740878288016106aa565b9450945050602085013567ffffffffffffffff811115610763576107626104e0565b5b61076f878288016106aa565b925092505092959194509250565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156107b4578082015181840152602081019050610799565b5f8484015250505050565b5f601f19601f8301169050919050565b5f6107d98261077d565b6107e38185610787565b93506107f3818560208601610797565b6107fc816107bf565b840191505092915050565b5f6020820190508181035f83015261081f81846107cf565b905092915050565b5f805f6060848603121561083e5761083d6104dc565b5b5f61084b868287016105b6565b935050602061085c86828701610610565b925050604061086d86828701610610565b9150509250925092565b61088081610597565b82525050565b61088f816105e9565b82525050565b5f6080820190506108a85f830187610877565b6108b56020830186610886565b6108c26040830185610886565b6108cf606083018461056f565b95945050505050565b5f81905092915050565b828183375f83830152505050565b5f6108fb83856108d8565b93506109088385846108e2565b82840190509392505050565b5f6109208284866108f0565b91508190509392505050565b5f80fd5b5f80fd5b5f80858511156109475761094661092c565b5b8386111561095857610957610930565b5b6001850283019150848603905094509492505050565b5f82905092915050565b5f82821b905092915050565b5f61098f838361096e565b8261099a8135610597565b925060208210156109da576109d57fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff83602003600802610978565b831692505b505092915050565b5f82825260208201905092915050565b7f706172656e7420646f6d61696e206e6f742076616c69646174656420617070725f8201527f6f7072696174656c790000000000000000000000000000000000000000000000602082015250565b5f610a4c6029836109e2565b9150610a57826109f2565b604082019050919050565b5f6020820190508181035f830152610a7981610a40565b9050919050565b5f602082019050610a935f830184610886565b92915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52603260045260245ffd5b5f819050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52601160045260245ffd5b5f610b0682610ac6565b9150610b1183610ac6565b9250828201905080821115610b2957610b28610acf565b5b92915050565b5f610b3b8284866108f0565b91508190509392505050565b7f737562646f6d61696e206e6f742076616c69646174656420617070726f7072695f8201527f6174656c79000000000000000000000000000000000000000000000000000000602082015250565b5f610ba16025836109e2565b9150610bac82610b47565b604082019050919050565b5f6020820190508181035f830152610bce81610b95565b905091905056fea264697066735822122069cd8e8bbd4aef4d134d88d34bd84e9b9e73b22f71ef5ce68972f91bae7d7a2364736f6c63430008140033"  # noqa: E501
+EXTENDED_RESOLVER_RUNTIME = "0x608060405234801561000f575f80fd5b506004361061004a575f3560e01c806301ffc9a71461004e5780633e9ce7941461007e5780639061b9231461009a578063f86bc879146100ca575b5f80fd5b61006860048036038101906100639190610539565b6100fa565b604051610075919061057e565b60405180910390f35b6100986004803603810190610093919061064e565b61015a565b005b6100b460048036038101906100af91906106ff565b61023a565b6040516100c19190610807565b60405180910390f35b6100e460048036038101906100df9190610827565b610457565b6040516100f1919061057e565b60405180910390f35b5f639061b92360e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916148061015357506101528261048c565b5b9050919050565b8060015f8581526020019081526020015f205f3373ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020015f205f8473ffffffffffffffffffffffffffffffffffffffff1673ffffffffffffffffffffffffffffffffffffffff1681526020019081526020015f205f6101000a81548160ff0219169083151502179055507fe1c5610a6e0cbe10764ecd182adcef1ec338dc4e199c99c32ce98f38e12791df8333848460405161022d9493929190610895565b60405180910390a1505050565b60606040518060400160405280601781526020017f11657874656e6465642d7265736f6c7665720365746800000000000000000000815250805190602001208585604051610289929190610914565b60405180910390201480156102a2575060248383905010155b15610352577ff0a378cc2afe91730d0105e67d6bb037cc5b8b6bfec5b5962d9b637ff6497e555f1b83836004906024926102de93929190610934565b906102e99190610984565b14610329576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161032090610a62565b60405180910390fd5b61beef60405160200161033c9190610a80565b604051602081830303815290604052905061044f565b5f85855f81811061036657610365610a99565b5b9050013560f81c60f81b60f81c60ff1690506040518060400160405280601781526020017f11657874656e6465642d7265736f6c76657203657468000000000000000000008152508051906020012086868360016103c49190610afc565b9080926103d393929190610934565b6040516103e1929190610b2f565b604051809103902014610429576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161042090610bb7565b60405180910390fd5b61dead60405160200161043c9190610a80565b6040516020818303038152906040529150505b949350505050565b6001602052825f5260405f20602052815f5260405f20602052805f5260405f205f92509250509054906101000a900460ff1681565b5f6301ffc9a760e01b7bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916827bffffffffffffffffffffffffffffffffffffffffffffffffffffffff1916149050919050565b5f80fd5b5f80fd5b5f7fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b610518816104e4565b8114610522575f80fd5b50565b5f813590506105338161050f565b92915050565b5f6020828403121561054e5761054d6104dc565b5b5f61055b84828501610525565b91505092915050565b5f8115159050919050565b61057881610564565b82525050565b5f6020820190506105915f83018461056f565b92915050565b5f819050919050565b6105a981610597565b81146105b3575f80fd5b50565b5f813590506105c4816105a0565b92915050565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6105f3826105ca565b9050919050565b610603816105e9565b811461060d575f80fd5b50565b5f8135905061061e816105fa565b92915050565b61062d81610564565b8114610637575f80fd5b50565b5f8135905061064881610624565b92915050565b5f805f60608486031215610665576106646104dc565b5b5f610672868287016105b6565b935050602061068386828701610610565b92505060406106948682870161063a565b9150509250925092565b5f80fd5b5f80fd5b5f80fd5b5f8083601f8401126106bf576106be61069e565b5b8235905067ffffffffffffffff8111156106dc576106db6106a2565b5b6020830191508360018202830111156106f8576106f76106a6565b5b9250929050565b5f805f8060408587031215610717576107166104dc565b5b5f85013567ffffffffffffffff811115610734576107336104e0565b5b610740878288016106aa565b9450945050602085013567ffffffffffffffff811115610763576107626104e0565b5b61076f878288016106aa565b925092505092959194509250565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156107b4578082015181840152602081019050610799565b5f8484015250505050565b5f601f19601f8301169050919050565b5f6107d98261077d565b6107e38185610787565b93506107f3818560208601610797565b6107fc816107bf565b840191505092915050565b5f6020820190508181035f83015261081f81846107cf565b905092915050565b5f805f6060848603121561083e5761083d6104dc565b5b5f61084b868287016105b6565b935050602061085c86828701610610565b925050604061086d86828701610610565b9150509250925092565b61088081610597565b82525050565b61088f816105e9565b82525050565b5f6080820190506108a85f830187610877565b6108b56020830186610886565b6108c26040830185610886565b6108cf606083018461056f565b95945050505050565b5f81905092915050565b828183375f83830152505050565b5f6108fb83856108d8565b93506109088385846108e2565b82840190509392505050565b5f6109208284866108f0565b91508190509392505050565b5f80fd5b5f80fd5b5f80858511156109475761094661092c565b5b8386111561095857610957610930565b5b6001850283019150848603905094509492505050565b5f82905092915050565b5f82821b905092915050565b5f61098f838361096e565b8261099a8135610597565b925060208210156109da576109d57fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff83602003600802610978565b831692505b505092915050565b5f82825260208201905092915050565b7f706172656e7420646f6d61696e206e6f742076616c69646174656420617070725f8201527f6f7072696174656c790000000000000000000000000000000000000000000000602082015250565b5f610a4c6029836109e2565b9150610a57826109f2565b604082019050919050565b5f6020820190508181035f830152610a7981610a40565b9050919050565b5f602082019050610a935f830184610886565b92915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52603260045260245ffd5b5f819050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52601160045260245ffd5b5f610b0682610ac6565b9150610b1183610ac6565b9250828201905080821115610b2957610b28610acf565b5b92915050565b5f610b3b8284866108f0565b91508190509392505050565b7f737562646f6d61696e206e6f742076616c69646174656420617070726f7072695f8201527f6174656c79000000000000000000000000000000000000000000000000000000602082015250565b5f610ba16025836109e2565b9150610bac82610b47565b604082019050919050565b5f6020820190508181035f830152610bce81610b95565b905091905056fea264697066735822122069cd8e8bbd4aef4d134d88d34bd84e9b9e73b22f71ef5ce68972f91bae7d7a2364736f6c63430008140033"  # noqa: E501
 EXTENDED_RESOLVER_ABI = [
     {
         "inputs": [{"internalType": "contract ENS", "name": "_ens", "type": "address"}],
         "stateMutability": "nonpayable",
         "type": "constructor",
     },
     {
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/fallback_function_contract.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/FallbackFunctionContract.sol:FallbackFunctionContract  # noqa: E501
-FALLBACK_FUNCTION_CONTRACT_BYTECODE = "0x60806040526000808190555060be806100196000396000f3fe6080604052348015600f57600080fd5b5060043610602b5760003560e01c80633bc5de3014603557602c565b5b60016000819055005b603b604f565b60405160469190606f565b60405180910390f35b60008054905090565b6000819050919050565b6069816058565b82525050565b6000602082019050608260008301846062565b9291505056fea2646970667358221220d95c3cd5a0ca6d47e2f21437ca1df40d72b5db8af0fa1be2b496bee3a29c45d464736f6c63430008130033"  # noqa: E501
-FALLBACK_FUNCTION_CONTRACT_RUNTIME = "0x6080604052348015600f57600080fd5b5060043610602b5760003560e01c80633bc5de3014603557602c565b5b60016000819055005b603b604f565b60405160469190606f565b60405180910390f35b60008054905090565b6000819050919050565b6069816058565b82525050565b6000602082019050608260008301846062565b9291505056fea2646970667358221220d95c3cd5a0ca6d47e2f21437ca1df40d72b5db8af0fa1be2b496bee3a29c45d464736f6c63430008130033"  # noqa: E501
+FALLBACK_FUNCTION_CONTRACT_BYTECODE = "0x60806040525f808190555060b7806100165f395ff3fe6080604052348015600e575f80fd5b50600436106029575f3560e01c80633bc5de3014603257602a565b5b60015f819055005b6038604c565b60405160439190606a565b60405180910390f35b5f8054905090565b5f819050919050565b6064816054565b82525050565b5f602082019050607b5f830184605d565b9291505056fea264697066735822122091dda03dc9a450d5acd30e36f45faa3c8eae615b354fcb1b5650fcd13206d40f64736f6c63430008140033"  # noqa: E501
+FALLBACK_FUNCTION_CONTRACT_RUNTIME = "0x6080604052348015600e575f80fd5b50600436106029575f3560e01c80633bc5de3014603257602a565b5b60015f819055005b6038604c565b60405160439190606a565b60405180910390f35b5f8054905090565b5f819050919050565b6064816054565b82525050565b5f602082019050607b5f830184605d565b9291505056fea264697066735822122091dda03dc9a450d5acd30e36f45faa3c8eae615b354fcb1b5650fcd13206d40f64736f6c63430008140033"  # noqa: E501
 FALLBACK_FUNCTION_CONTRACT_ABI = [
     {"inputs": [], "stateMutability": "payable", "type": "constructor"},
     {"stateMutability": "nonpayable", "type": "fallback"},
     {
         "inputs": [],
         "name": "getData",
         "outputs": [{"internalType": "uint256", "name": "r", "type": "uint256"}],
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/math_contract.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/math_contract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/MathContract.sol:MathContract
-MATH_CONTRACT_BYTECODE = "0x60806040526000805534801561001457600080fd5b5061055b806100246000396000f3fe6080604052600436106100555760003560e01c806316216f391461005a5780635b34b9661461008557806361bc221a146100a35780636abbb3b4146100ce578063a5f3c23b146100fe578063dcf537b11461012e575b600080fd5b34801561006657600080fd5b5061006f61015e565b60405161007c9190610260565b60405180910390f35b61008d610167565b60405161009a9190610294565b60405180910390f35b3480156100af57600080fd5b506100b86101be565b6040516100c59190610294565b60405180910390f35b6100e860048036038101906100e391906102e0565b6101c4565b6040516100f59190610294565b60405180910390f35b61011860048036038101906101139190610339565b61021b565b6040516101259190610260565b60405180910390f35b61014860048036038101906101439190610379565b610231565b6040516101559190610260565b60405180910390f35b6000600d905090565b6000600160005461017891906103d5565b6000819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c560016040516101ae919061044e565b60405180910390a1600054905090565b60005481565b6000816000546101d491906103d5565b6000819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c5826040516102099190610294565b60405180910390a16000549050919050565b600081836102299190610469565b905092915050565b600060078261024091906104ad565b9050919050565b6000819050919050565b61025a81610247565b82525050565b60006020820190506102756000830184610251565b92915050565b6000819050919050565b61028e8161027b565b82525050565b60006020820190506102a96000830184610285565b92915050565b600080fd5b6102bd8161027b565b81146102c857600080fd5b50565b6000813590506102da816102b4565b92915050565b6000602082840312156102f6576102f56102af565b5b6000610304848285016102cb565b91505092915050565b61031681610247565b811461032157600080fd5b50565b6000813590506103338161030d565b92915050565b600080604083850312156103505761034f6102af565b5b600061035e85828601610324565b925050602061036f85828601610324565b9150509250929050565b60006020828403121561038f5761038e6102af565b5b600061039d84828501610324565b91505092915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006103e08261027b565b91506103eb8361027b565b9250828201905080821115610403576104026103a6565b5b92915050565b6000819050919050565b6000819050919050565b600061043861043361042e84610409565b610413565b61027b565b9050919050565b6104488161041d565b82525050565b6000602082019050610463600083018461043f565b92915050565b600061047482610247565b915061047f83610247565b9250828201905082811215600083121683821260008412151617156104a7576104a66103a6565b5b92915050565b60006104b882610247565b91506104c383610247565b92508282026104d181610247565b91507f80000000000000000000000000000000000000000000000000000000000000008414600084121615610509576105086103a6565b5b828205841483151761051e5761051d6103a6565b5b509291505056fea2646970667358221220c048b14ed3f40c1a02806ce098b93b0850411f910e3ed7e262bc92fea1e0abc864736f6c63430008130033"  # noqa: E501
-MATH_CONTRACT_RUNTIME = "0x6080604052600436106100555760003560e01c806316216f391461005a5780635b34b9661461008557806361bc221a146100a35780636abbb3b4146100ce578063a5f3c23b146100fe578063dcf537b11461012e575b600080fd5b34801561006657600080fd5b5061006f61015e565b60405161007c9190610260565b60405180910390f35b61008d610167565b60405161009a9190610294565b60405180910390f35b3480156100af57600080fd5b506100b86101be565b6040516100c59190610294565b60405180910390f35b6100e860048036038101906100e391906102e0565b6101c4565b6040516100f59190610294565b60405180910390f35b61011860048036038101906101139190610339565b61021b565b6040516101259190610260565b60405180910390f35b61014860048036038101906101439190610379565b610231565b6040516101559190610260565b60405180910390f35b6000600d905090565b6000600160005461017891906103d5565b6000819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c560016040516101ae919061044e565b60405180910390a1600054905090565b60005481565b6000816000546101d491906103d5565b6000819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c5826040516102099190610294565b60405180910390a16000549050919050565b600081836102299190610469565b905092915050565b600060078261024091906104ad565b9050919050565b6000819050919050565b61025a81610247565b82525050565b60006020820190506102756000830184610251565b92915050565b6000819050919050565b61028e8161027b565b82525050565b60006020820190506102a96000830184610285565b92915050565b600080fd5b6102bd8161027b565b81146102c857600080fd5b50565b6000813590506102da816102b4565b92915050565b6000602082840312156102f6576102f56102af565b5b6000610304848285016102cb565b91505092915050565b61031681610247565b811461032157600080fd5b50565b6000813590506103338161030d565b92915050565b600080604083850312156103505761034f6102af565b5b600061035e85828601610324565b925050602061036f85828601610324565b9150509250929050565b60006020828403121561038f5761038e6102af565b5b600061039d84828501610324565b91505092915050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052601160045260246000fd5b60006103e08261027b565b91506103eb8361027b565b9250828201905080821115610403576104026103a6565b5b92915050565b6000819050919050565b6000819050919050565b600061043861043361042e84610409565b610413565b61027b565b9050919050565b6104488161041d565b82525050565b6000602082019050610463600083018461043f565b92915050565b600061047482610247565b915061047f83610247565b9250828201905082811215600083121683821260008412151617156104a7576104a66103a6565b5b92915050565b60006104b882610247565b91506104c383610247565b92508282026104d181610247565b91507f80000000000000000000000000000000000000000000000000000000000000008414600084121615610509576105086103a6565b5b828205841483151761051e5761051d6103a6565b5b509291505056fea2646970667358221220c048b14ed3f40c1a02806ce098b93b0850411f910e3ed7e262bc92fea1e0abc864736f6c63430008130033"  # noqa: E501
+MATH_CONTRACT_BYTECODE = "0x60806040525f8055348015610012575f80fd5b5061052d806100205f395ff3fe608060405260043610610054575f3560e01c806316216f39146100585780635b34b9661461008257806361bc221a146100a05780636abbb3b4146100ca578063a5f3c23b146100fa578063dcf537b11461012a575b5f80fd5b348015610063575f80fd5b5061006c61015a565b604051610079919061024f565b60405180910390f35b61008a610162565b6040516100979190610280565b60405180910390f35b3480156100ab575f80fd5b506100b46101b5565b6040516100c19190610280565b60405180910390f35b6100e460048036038101906100df91906102c7565b6101ba565b6040516100f19190610280565b60405180910390f35b610114600480360381019061010f919061031c565b61020d565b604051610121919061024f565b60405180910390f35b610144600480360381019061013f919061035a565b610222565b604051610151919061024f565b60405180910390f35b5f600d905090565b5f60015f5461017191906103b2565b5f819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c560016040516101a69190610427565b60405180910390a15f54905090565b5f5481565b5f815f546101c891906103b2565b5f819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c5826040516101fc9190610280565b60405180910390a15f549050919050565b5f818361021a9190610440565b905092915050565b5f6007826102309190610481565b9050919050565b5f819050919050565b61024981610237565b82525050565b5f6020820190506102625f830184610240565b92915050565b5f819050919050565b61027a81610268565b82525050565b5f6020820190506102935f830184610271565b92915050565b5f80fd5b6102a681610268565b81146102b0575f80fd5b50565b5f813590506102c18161029d565b92915050565b5f602082840312156102dc576102db610299565b5b5f6102e9848285016102b3565b91505092915050565b6102fb81610237565b8114610305575f80fd5b50565b5f81359050610316816102f2565b92915050565b5f806040838503121561033257610331610299565b5b5f61033f85828601610308565b925050602061035085828601610308565b9150509250929050565b5f6020828403121561036f5761036e610299565b5b5f61037c84828501610308565b91505092915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52601160045260245ffd5b5f6103bc82610268565b91506103c783610268565b92508282019050808211156103df576103de610385565b5b92915050565b5f819050919050565b5f819050919050565b5f61041161040c610407846103e5565b6103ee565b610268565b9050919050565b610421816103f7565b82525050565b5f60208201905061043a5f830184610418565b92915050565b5f61044a82610237565b915061045583610237565b92508282019050828112155f8312168382125f84121516171561047b5761047a610385565b5b92915050565b5f61048b82610237565b915061049683610237565b92508282026104a481610237565b91507f800000000000000000000000000000000000000000000000000000000000000084145f841216156104db576104da610385565b5b82820584148315176104f0576104ef610385565b5b509291505056fea264697066735822122004c925325fc831d9edc52c8187dc974b64c5d37f907e3400a503f1af4bd4ef9364736f6c63430008140033"  # noqa: E501
+MATH_CONTRACT_RUNTIME = "0x608060405260043610610054575f3560e01c806316216f39146100585780635b34b9661461008257806361bc221a146100a05780636abbb3b4146100ca578063a5f3c23b146100fa578063dcf537b11461012a575b5f80fd5b348015610063575f80fd5b5061006c61015a565b604051610079919061024f565b60405180910390f35b61008a610162565b6040516100979190610280565b60405180910390f35b3480156100ab575f80fd5b506100b46101b5565b6040516100c19190610280565b60405180910390f35b6100e460048036038101906100df91906102c7565b6101ba565b6040516100f19190610280565b60405180910390f35b610114600480360381019061010f919061031c565b61020d565b604051610121919061024f565b60405180910390f35b610144600480360381019061013f919061035a565b610222565b604051610151919061024f565b60405180910390f35b5f600d905090565b5f60015f5461017191906103b2565b5f819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c560016040516101a69190610427565b60405180910390a15f54905090565b5f5481565b5f815f546101c891906103b2565b5f819055507f3496c3ede4ec3ab3686712aa1c238593ea6a42df83f98a5ec7df9834cfa577c5826040516101fc9190610280565b60405180910390a15f549050919050565b5f818361021a9190610440565b905092915050565b5f6007826102309190610481565b9050919050565b5f819050919050565b61024981610237565b82525050565b5f6020820190506102625f830184610240565b92915050565b5f819050919050565b61027a81610268565b82525050565b5f6020820190506102935f830184610271565b92915050565b5f80fd5b6102a681610268565b81146102b0575f80fd5b50565b5f813590506102c18161029d565b92915050565b5f602082840312156102dc576102db610299565b5b5f6102e9848285016102b3565b91505092915050565b6102fb81610237565b8114610305575f80fd5b50565b5f81359050610316816102f2565b92915050565b5f806040838503121561033257610331610299565b5b5f61033f85828601610308565b925050602061035085828601610308565b9150509250929050565b5f6020828403121561036f5761036e610299565b5b5f61037c84828501610308565b91505092915050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52601160045260245ffd5b5f6103bc82610268565b91506103c783610268565b92508282019050808211156103df576103de610385565b5b92915050565b5f819050919050565b5f819050919050565b5f61041161040c610407846103e5565b6103ee565b610268565b9050919050565b610421816103f7565b82525050565b5f60208201905061043a5f830184610418565b92915050565b5f61044a82610237565b915061045583610237565b92508282019050828112155f8312168382125f84121516171561047b5761047a610385565b5b92915050565b5f61048b82610237565b915061049683610237565b92508282026104a481610237565b91507f800000000000000000000000000000000000000000000000000000000000000084145f841216156104db576104da610385565b5b82820584148315176104f0576104ef610385565b5b509291505056fea264697066735822122004c925325fc831d9edc52c8187dc974b64c5d37f907e3400a503f1af4bd4ef9364736f6c63430008140033"  # noqa: E501
 MATH_CONTRACT_ABI = [
     {
         "anonymous": False,
         "inputs": [
             {
                 "indexed": False,
                 "internalType": "uint256",
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/offchain_lookup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/OffchainLookup.sol:OffchainLookup
-OFFCHAIN_LOOKUP_BYTECODE = "0x608060405260405180604001604052806040518060600160405280602c815260200162001129602c91398152602001604051806060016040528060258152602001620011556025913981525060009060026200005d92919062000072565b503480156200006b57600080fd5b50620004c0565b828054828255906000526020600020908101928215620000bf579160200282015b82811115620000be578251829081620000ad9190620003d9565b509160200191906001019062000093565b5b509050620000ce9190620000d2565b5090565b5b80821115620000f65760008181620000ec9190620000fa565b50600101620000d3565b5090565b5080546200010890620001c8565b6000825580601f106200011c57506200013d565b601f0160209004906000526020600020908101906200013c919062000140565b5b50565b5b808211156200015b57600081600090555060010162000141565b5090565b600081519050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602260045260246000fd5b60006002820490506001821680620001e157607f821691505b602082108103620001f757620001f662000199565b5b50919050565b60008190508160005260206000209050919050565b60006020601f8301049050919050565b600082821b905092915050565b600060088302620002617fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff8262000222565b6200026d868362000222565b95508019841693508086168417925050509392505050565b6000819050919050565b6000819050919050565b6000620002ba620002b4620002ae8462000285565b6200028f565b62000285565b9050919050565b6000819050919050565b620002d68362000299565b620002ee620002e582620002c1565b8484546200022f565b825550505050565b600090565b62000305620002f6565b62000312818484620002cb565b505050565b5b818110156200033a576200032e600082620002fb565b60018101905062000318565b5050565b601f82111562000389576200035381620001fd565b6200035e8462000212565b810160208510156200036e578190505b620003866200037d8562000212565b83018262000317565b50505b505050565b600082821c905092915050565b6000620003ae600019846008026200038e565b1980831691505092915050565b6000620003c983836200039b565b9150826002028217905092915050565b620003e4826200015f565b67ffffffffffffffff8111156200040057620003ff6200016a565b5b6200040c8254620001c8565b620004198282856200033e565b600060209050601f8311600181146200045157600084156200043c578287015190505b620004488582620003bb565b865550620004b8565b601f1984166200046186620001fd565b60005b828110156200048b5784890151825560018201915060208501945060208101905062000464565b86831015620004ab5784890151620004a7601f8916826200039b565b8355505b6001600288020188555050505b505050505050565b610c5980620004d06000396000f3fe608060405234801561001057600080fd5b50600436106100415760003560e01c806309a3c01b146100465780636337ed5814610064578063da96d05a14610094575b600080fd5b61004e6100c4565b60405161005b919061041b565b60405180910390f35b61007e600480360381019061007991906104b6565b610114565b60405161008b919061041b565b60405180910390f35b6100ae60048036038101906100a99190610503565b610202565b6040516100bb919061041b565b60405180910390f35b606080306000826309a3c01b60e01b846040517f556f183000000000000000000000000000000000000000000000000000000000815260040161010b9594939291906107d0565b60405180910390fd5b6060600083838101906101279190610968565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af0758160405160200161015b91906109f8565b60405160208183030381529060405280519060200120146101b1576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016101a890610a6c565b60405180910390fd5b306000858563da96d05a60e01b88886040517f556f18300000000000000000000000000000000000000000000000000000000081526004016101f99796959493929190610ab9565b60405180910390fd5b6060600085858101906102159190610968565b90507faed76f463930323372899e36460e078e5292aac45f645bbe567be6fca83ede108160405160200161024991906109f8565b604051602081830303815290604052805190602001201461029f576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161029690610b97565b60405180910390fd5b600084848101906102b09190610968565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af075816040516020016102e491906109f8565b604051602081830303815290604052805190602001201461033a576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161033190610c03565b60405180910390fd5b86868080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505092505050949350505050565b600081519050919050565b600082825260208201905092915050565b60005b838110156103c55780820151818401526020810190506103aa565b60008484015250505050565b6000601f19601f8301169050919050565b60006103ed8261038b565b6103f78185610396565b93506104078185602086016103a7565b610410816103d1565b840191505092915050565b6000602082019050818103600083015261043581846103e2565b905092915050565b6000604051905090565b600080fd5b600080fd5b600080fd5b600080fd5b600080fd5b60008083601f84011261047657610475610451565b5b8235905067ffffffffffffffff81111561049357610492610456565b5b6020830191508360018202830111156104af576104ae61045b565b5b9250929050565b600080602083850312156104cd576104cc610447565b5b600083013567ffffffffffffffff8111156104eb576104ea61044c565b5b6104f785828601610460565b92509250509250929050565b6000806000806040858703121561051d5761051c610447565b5b600085013567ffffffffffffffff81111561053b5761053a61044c565b5b61054787828801610460565b9450945050602085013567ffffffffffffffff81111561056a5761056961044c565b5b61057687828801610460565b925092505092959194509250565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006105af82610584565b9050919050565b6105bf816105a4565b82525050565b600081549050919050565b600082825260208201905092915050565b60008190508160005260206000209050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602260045260246000fd5b6000600282049050600182168061063d57607f821691505b6020821081036106505761064f6105f6565b5b50919050565b600082825260208201905092915050565b60008190508160005260206000209050919050565b6000815461068981610625565b6106938186610656565b945060018216600081146106ae57600181146106c4576106f7565b60ff1983168652811515602002860193506106f7565b6106cd85610667565b60005b838110156106ef578154818901526001820191506020810190506106d0565b808801955050505b50505092915050565b600061070c838361067c565b905092915050565b6000600182019050919050565b600061072c826105c5565b61073681856105d0565b935083602082028501610748856105e1565b8060005b85811015610783578484038952816107648582610700565b945061076f83610714565b925060208a0199505060018101905061074c565b50829750879550505050505092915050565b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b6107ca81610795565b82525050565b600060a0820190506107e560008301886105b6565b81810360208301526107f78187610721565b9050818103604083015261080b81866103e2565b905061081a60608301856107c1565b818103608083015261082c81846103e2565b90509695505050505050565b600080fd5b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b610875826103d1565b810181811067ffffffffffffffff821117156108945761089361083d565b5b80604052505050565b60006108a761043d565b90506108b3828261086c565b919050565b600067ffffffffffffffff8211156108d3576108d261083d565b5b6108dc826103d1565b9050602081019050919050565b82818337600083830152505050565b600061090b610906846108b8565b61089d565b90508281526020810184848401111561092757610926610838565b5b6109328482856108e9565b509392505050565b600082601f83011261094f5761094e610451565b5b813561095f8482602086016108f8565b91505092915050565b60006020828403121561097e5761097d610447565b5b600082013567ffffffffffffffff81111561099c5761099b61044c565b5b6109a88482850161093a565b91505092915050565b600081519050919050565b600081905092915050565b60006109d2826109b1565b6109dc81856109bc565b93506109ec8185602086016103a7565b80840191505092915050565b6000610a0482846109c7565b915081905092915050565b600082825260208201905092915050565b7f7465737420646174612076616c69646174696f6e206661696c65642e00000000600082015250565b6000610a56601c83610a0f565b9150610a6182610a20565b602082019050919050565b60006020820190508181036000830152610a8581610a49565b9050919050565b6000610a988385610396565b9350610aa58385846108e9565b610aae836103d1565b840190509392505050565b600060a082019050610ace600083018a6105b6565b8181036020830152610ae08189610721565b90508181036040830152610af5818789610a8c565b9050610b0460608301866107c1565b8181036080830152610b17818486610a8c565b905098975050505050505050565b7f68747470207265717565737420726573756c742076616c69646174696f6e206660008201527f61696c65642e0000000000000000000000000000000000000000000000000000602082015250565b6000610b81602683610a0f565b9150610b8c82610b25565b604082019050919050565b60006020820190508181036000830152610bb081610b74565b9050919050565b7f6578747261446174612076616c69646174696f6e206661696c65642e00000000600082015250565b6000610bed601c83610a0f565b9150610bf882610bb7565b602082019050919050565b60006020820190508181036000830152610c1c81610be0565b905091905056fea26469706673582212207d45ce0c131520a39dcebc7261dd61227c25059a661ba1fb25e1acbd0061870164736f6c6343000813003368747470733a2f2f776562332e70792f676174657761792f7b73656e6465727d2f7b646174617d2e6a736f6e68747470733a2f2f776562332e70792f676174657761792f7b73656e6465727d2e6a736f6e"  # noqa: E501
-OFFCHAIN_LOOKUP_RUNTIME = "0x608060405234801561001057600080fd5b50600436106100415760003560e01c806309a3c01b146100465780636337ed5814610064578063da96d05a14610094575b600080fd5b61004e6100c4565b60405161005b919061041b565b60405180910390f35b61007e600480360381019061007991906104b6565b610114565b60405161008b919061041b565b60405180910390f35b6100ae60048036038101906100a99190610503565b610202565b6040516100bb919061041b565b60405180910390f35b606080306000826309a3c01b60e01b846040517f556f183000000000000000000000000000000000000000000000000000000000815260040161010b9594939291906107d0565b60405180910390fd5b6060600083838101906101279190610968565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af0758160405160200161015b91906109f8565b60405160208183030381529060405280519060200120146101b1576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016101a890610a6c565b60405180910390fd5b306000858563da96d05a60e01b88886040517f556f18300000000000000000000000000000000000000000000000000000000081526004016101f99796959493929190610ab9565b60405180910390fd5b6060600085858101906102159190610968565b90507faed76f463930323372899e36460e078e5292aac45f645bbe567be6fca83ede108160405160200161024991906109f8565b604051602081830303815290604052805190602001201461029f576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161029690610b97565b60405180910390fd5b600084848101906102b09190610968565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af075816040516020016102e491906109f8565b604051602081830303815290604052805190602001201461033a576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161033190610c03565b60405180910390fd5b86868080601f016020809104026020016040519081016040528093929190818152602001838380828437600081840152601f19601f8201169050808301925050505050505092505050949350505050565b600081519050919050565b600082825260208201905092915050565b60005b838110156103c55780820151818401526020810190506103aa565b60008484015250505050565b6000601f19601f8301169050919050565b60006103ed8261038b565b6103f78185610396565b93506104078185602086016103a7565b610410816103d1565b840191505092915050565b6000602082019050818103600083015261043581846103e2565b905092915050565b6000604051905090565b600080fd5b600080fd5b600080fd5b600080fd5b600080fd5b60008083601f84011261047657610475610451565b5b8235905067ffffffffffffffff81111561049357610492610456565b5b6020830191508360018202830111156104af576104ae61045b565b5b9250929050565b600080602083850312156104cd576104cc610447565b5b600083013567ffffffffffffffff8111156104eb576104ea61044c565b5b6104f785828601610460565b92509250509250929050565b6000806000806040858703121561051d5761051c610447565b5b600085013567ffffffffffffffff81111561053b5761053a61044c565b5b61054787828801610460565b9450945050602085013567ffffffffffffffff81111561056a5761056961044c565b5b61057687828801610460565b925092505092959194509250565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006105af82610584565b9050919050565b6105bf816105a4565b82525050565b600081549050919050565b600082825260208201905092915050565b60008190508160005260206000209050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052602260045260246000fd5b6000600282049050600182168061063d57607f821691505b6020821081036106505761064f6105f6565b5b50919050565b600082825260208201905092915050565b60008190508160005260206000209050919050565b6000815461068981610625565b6106938186610656565b945060018216600081146106ae57600181146106c4576106f7565b60ff1983168652811515602002860193506106f7565b6106cd85610667565b60005b838110156106ef578154818901526001820191506020810190506106d0565b808801955050505b50505092915050565b600061070c838361067c565b905092915050565b6000600182019050919050565b600061072c826105c5565b61073681856105d0565b935083602082028501610748856105e1565b8060005b85811015610783578484038952816107648582610700565b945061076f83610714565b925060208a0199505060018101905061074c565b50829750879550505050505092915050565b60007fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b6107ca81610795565b82525050565b600060a0820190506107e560008301886105b6565b81810360208301526107f78187610721565b9050818103604083015261080b81866103e2565b905061081a60608301856107c1565b818103608083015261082c81846103e2565b90509695505050505050565b600080fd5b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b610875826103d1565b810181811067ffffffffffffffff821117156108945761089361083d565b5b80604052505050565b60006108a761043d565b90506108b3828261086c565b919050565b600067ffffffffffffffff8211156108d3576108d261083d565b5b6108dc826103d1565b9050602081019050919050565b82818337600083830152505050565b600061090b610906846108b8565b61089d565b90508281526020810184848401111561092757610926610838565b5b6109328482856108e9565b509392505050565b600082601f83011261094f5761094e610451565b5b813561095f8482602086016108f8565b91505092915050565b60006020828403121561097e5761097d610447565b5b600082013567ffffffffffffffff81111561099c5761099b61044c565b5b6109a88482850161093a565b91505092915050565b600081519050919050565b600081905092915050565b60006109d2826109b1565b6109dc81856109bc565b93506109ec8185602086016103a7565b80840191505092915050565b6000610a0482846109c7565b915081905092915050565b600082825260208201905092915050565b7f7465737420646174612076616c69646174696f6e206661696c65642e00000000600082015250565b6000610a56601c83610a0f565b9150610a6182610a20565b602082019050919050565b60006020820190508181036000830152610a8581610a49565b9050919050565b6000610a988385610396565b9350610aa58385846108e9565b610aae836103d1565b840190509392505050565b600060a082019050610ace600083018a6105b6565b8181036020830152610ae08189610721565b90508181036040830152610af5818789610a8c565b9050610b0460608301866107c1565b8181036080830152610b17818486610a8c565b905098975050505050505050565b7f68747470207265717565737420726573756c742076616c69646174696f6e206660008201527f61696c65642e0000000000000000000000000000000000000000000000000000602082015250565b6000610b81602683610a0f565b9150610b8c82610b25565b604082019050919050565b60006020820190508181036000830152610bb081610b74565b9050919050565b7f6578747261446174612076616c69646174696f6e206661696c65642e00000000600082015250565b6000610bed601c83610a0f565b9150610bf882610bb7565b602082019050919050565b60006020820190508181036000830152610c1c81610be0565b905091905056fea26469706673582212207d45ce0c131520a39dcebc7261dd61227c25059a661ba1fb25e1acbd0061870164736f6c63430008130033"  # noqa: E501
+OFFCHAIN_LOOKUP_BYTECODE = "0x608060405260405180604001604052806040518060600160405280602c8152602001620010b1602c91398152602001604051806060016040528060258152602001620010dd602591398152505f9060026200005c92919062000070565b5034801562000069575f80fd5b506200049d565b828054828255905f5260205f20908101928215620000bb579160200282015b82811115620000ba578251829081620000a99190620003b9565b50916020019190600101906200008f565b5b509050620000ca9190620000ce565b5090565b5b80821115620000f1575f8181620000e79190620000f5565b50600101620000cf565b5090565b5080546200010390620001b9565b5f825580601f1062000116575062000135565b601f0160209004905f5260205f209081019062000134919062000138565b5b50565b5b8082111562000151575f815f90555060010162000139565b5090565b5f81519050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602260045260245ffd5b5f6002820490506001821680620001d157607f821691505b602082108103620001e757620001e66200018c565b5b50919050565b5f819050815f5260205f209050919050565b5f6020601f8301049050919050565b5f82821b905092915050565b5f600883026200024b7fffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff826200020e565b6200025786836200020e565b95508019841693508086168417925050509392505050565b5f819050919050565b5f819050919050565b5f620002a16200029b62000295846200026f565b62000278565b6200026f565b9050919050565b5f819050919050565b620002bc8362000281565b620002d4620002cb82620002a8565b8484546200021a565b825550505050565b5f90565b620002ea620002dc565b620002f7818484620002b1565b505050565b5b818110156200031e57620003125f82620002e0565b600181019050620002fd565b5050565b601f8211156200036d576200033781620001ed565b6200034284620001ff565b8101602085101562000352578190505b6200036a6200036185620001ff565b830182620002fc565b50505b505050565b5f82821c905092915050565b5f6200038f5f198460080262000372565b1980831691505092915050565b5f620003a983836200037e565b9150826002028217905092915050565b620003c48262000155565b67ffffffffffffffff811115620003e057620003df6200015f565b5b620003ec8254620001b9565b620003f982828562000322565b5f60209050601f8311600181146200042f575f84156200041a578287015190505b6200042685826200039c565b86555062000495565b601f1984166200043f86620001ed565b5f5b82811015620004685784890151825560018201915060208501945060208101905062000441565b8683101562000488578489015162000484601f8916826200037e565b8355505b6001600288020188555050505b505050505050565b610c0680620004ab5f395ff3fe608060405234801561000f575f80fd5b506004361061003f575f3560e01c806309a3c01b146100435780636337ed5814610061578063da96d05a14610091575b5f80fd5b61004b6100c1565b604051610058919061040c565b60405180910390f35b61007b6004803603810190610076919061049e565b610110565b604051610088919061040c565b60405180910390f35b6100ab60048036038101906100a691906104e9565b6101fc565b6040516100b8919061040c565b60405180910390f35b606080305f826309a3c01b60e01b846040517f556f183000000000000000000000000000000000000000000000000000000000815260040161010795949392919061079d565b60405180910390fd5b60605f8383810190610122919061092b565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af0758160405160200161015691906109b6565b60405160208183030381529060405280519060200120146101ac576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016101a390610a26565b60405180910390fd5b305f858563da96d05a60e01b88886040517f556f18300000000000000000000000000000000000000000000000000000000081526004016101f39796959493929190610a70565b60405180910390fd5b60605f858581019061020e919061092b565b90507faed76f463930323372899e36460e078e5292aac45f645bbe567be6fca83ede108160405160200161024291906109b6565b6040516020818303038152906040528051906020012014610298576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161028f90610b4a565b60405180910390fd5b5f84848101906102a8919061092b565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af075816040516020016102dc91906109b6565b6040516020818303038152906040528051906020012014610332576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161032990610bb2565b60405180910390fd5b86868080601f0160208091040260200160405190810160405280939291908181526020018383808284375f81840152601f19601f8201169050808301925050505050505092505050949350505050565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156103b957808201518184015260208101905061039e565b5f8484015250505050565b5f601f19601f8301169050919050565b5f6103de82610382565b6103e8818561038c565b93506103f881856020860161039c565b610401816103c4565b840191505092915050565b5f6020820190508181035f83015261042481846103d4565b905092915050565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f80fd5b5f80fd5b5f8083601f84011261045e5761045d61043d565b5b8235905067ffffffffffffffff81111561047b5761047a610441565b5b60208301915083600182028301111561049757610496610445565b5b9250929050565b5f80602083850312156104b4576104b3610435565b5b5f83013567ffffffffffffffff8111156104d1576104d0610439565b5b6104dd85828601610449565b92509250509250929050565b5f805f806040858703121561050157610500610435565b5b5f85013567ffffffffffffffff81111561051e5761051d610439565b5b61052a87828801610449565b9450945050602085013567ffffffffffffffff81111561054d5761054c610439565b5b61055987828801610449565b925092505092959194509250565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f61059082610567565b9050919050565b6105a081610586565b82525050565b5f81549050919050565b5f82825260208201905092915050565b5f819050815f5260205f209050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602260045260245ffd5b5f600282049050600182168061061657607f821691505b602082108103610629576106286105d2565b5b50919050565b5f82825260208201905092915050565b5f819050815f5260205f209050919050565b5f815461065d816105ff565b610667818661062f565b9450600182165f81146106815760018114610697576106c9565b60ff1983168652811515602002860193506106c9565b6106a08561063f565b5f5b838110156106c1578154818901526001820191506020810190506106a2565b808801955050505b50505092915050565b5f6106dd8383610651565b905092915050565b5f600182019050919050565b5f6106fb826105a6565b61070581856105b0565b935083602082028501610717856105c0565b805f5b858110156107515784840389528161073285826106d2565b945061073d836106e5565b925060208a0199505060018101905061071a565b50829750879550505050505092915050565b5f7fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b61079781610763565b82525050565b5f60a0820190506107b05f830188610597565b81810360208301526107c281876106f1565b905081810360408301526107d681866103d4565b90506107e5606083018561078e565b81810360808301526107f781846103d4565b90509695505050505050565b5f80fd5b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b61083d826103c4565b810181811067ffffffffffffffff8211171561085c5761085b610807565b5b80604052505050565b5f61086e61042c565b905061087a8282610834565b919050565b5f67ffffffffffffffff82111561089957610898610807565b5b6108a2826103c4565b9050602081019050919050565b828183375f83830152505050565b5f6108cf6108ca8461087f565b610865565b9050828152602081018484840111156108eb576108ea610803565b5b6108f68482856108af565b509392505050565b5f82601f8301126109125761091161043d565b5b81356109228482602086016108bd565b91505092915050565b5f602082840312156109405761093f610435565b5b5f82013567ffffffffffffffff81111561095d5761095c610439565b5b610969848285016108fe565b91505092915050565b5f81519050919050565b5f81905092915050565b5f61099082610972565b61099a818561097c565b93506109aa81856020860161039c565b80840191505092915050565b5f6109c18284610986565b915081905092915050565b5f82825260208201905092915050565b7f7465737420646174612076616c69646174696f6e206661696c65642e000000005f82015250565b5f610a10601c836109cc565b9150610a1b826109dc565b602082019050919050565b5f6020820190508181035f830152610a3d81610a04565b9050919050565b5f610a4f838561038c565b9350610a5c8385846108af565b610a65836103c4565b840190509392505050565b5f60a082019050610a835f83018a610597565b8181036020830152610a9581896106f1565b90508181036040830152610aaa818789610a44565b9050610ab9606083018661078e565b8181036080830152610acc818486610a44565b905098975050505050505050565b7f68747470207265717565737420726573756c742076616c69646174696f6e20665f8201527f61696c65642e0000000000000000000000000000000000000000000000000000602082015250565b5f610b346026836109cc565b9150610b3f82610ada565b604082019050919050565b5f6020820190508181035f830152610b6181610b28565b9050919050565b7f6578747261446174612076616c69646174696f6e206661696c65642e000000005f82015250565b5f610b9c601c836109cc565b9150610ba782610b68565b602082019050919050565b5f6020820190508181035f830152610bc981610b90565b905091905056fea2646970667358221220bd330fe0ab45b92249f619f1ea882a9968f3ecdb87bad932a45810389165729864736f6c6343000814003368747470733a2f2f776562332e70792f676174657761792f7b73656e6465727d2f7b646174617d2e6a736f6e68747470733a2f2f776562332e70792f676174657761792f7b73656e6465727d2e6a736f6e"  # noqa: E501
+OFFCHAIN_LOOKUP_RUNTIME = "0x608060405234801561000f575f80fd5b506004361061003f575f3560e01c806309a3c01b146100435780636337ed5814610061578063da96d05a14610091575b5f80fd5b61004b6100c1565b604051610058919061040c565b60405180910390f35b61007b6004803603810190610076919061049e565b610110565b604051610088919061040c565b60405180910390f35b6100ab60048036038101906100a691906104e9565b6101fc565b6040516100b8919061040c565b60405180910390f35b606080305f826309a3c01b60e01b846040517f556f183000000000000000000000000000000000000000000000000000000000815260040161010795949392919061079d565b60405180910390fd5b60605f8383810190610122919061092b565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af0758160405160200161015691906109b6565b60405160208183030381529060405280519060200120146101ac576040517f08c379a00000000000000000000000000000000000000000000000000000000081526004016101a390610a26565b60405180910390fd5b305f858563da96d05a60e01b88886040517f556f18300000000000000000000000000000000000000000000000000000000081526004016101f39796959493929190610a70565b60405180910390fd5b60605f858581019061020e919061092b565b90507faed76f463930323372899e36460e078e5292aac45f645bbe567be6fca83ede108160405160200161024291906109b6565b6040516020818303038152906040528051906020012014610298576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161028f90610b4a565b60405180910390fd5b5f84848101906102a8919061092b565b90507fd9bdd1345ca2a00d0c1413137c1b2b1d0a35e5b0e11508f3b3eff856286af075816040516020016102dc91906109b6565b6040516020818303038152906040528051906020012014610332576040517f08c379a000000000000000000000000000000000000000000000000000000000815260040161032990610bb2565b60405180910390fd5b86868080601f0160208091040260200160405190810160405280939291908181526020018383808284375f81840152601f19601f8201169050808301925050505050505092505050949350505050565b5f81519050919050565b5f82825260208201905092915050565b5f5b838110156103b957808201518184015260208101905061039e565b5f8484015250505050565b5f601f19601f8301169050919050565b5f6103de82610382565b6103e8818561038c565b93506103f881856020860161039c565b610401816103c4565b840191505092915050565b5f6020820190508181035f83015261042481846103d4565b905092915050565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f80fd5b5f80fd5b5f8083601f84011261045e5761045d61043d565b5b8235905067ffffffffffffffff81111561047b5761047a610441565b5b60208301915083600182028301111561049757610496610445565b5b9250929050565b5f80602083850312156104b4576104b3610435565b5b5f83013567ffffffffffffffff8111156104d1576104d0610439565b5b6104dd85828601610449565b92509250509250929050565b5f805f806040858703121561050157610500610435565b5b5f85013567ffffffffffffffff81111561051e5761051d610439565b5b61052a87828801610449565b9450945050602085013567ffffffffffffffff81111561054d5761054c610439565b5b61055987828801610449565b925092505092959194509250565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f61059082610567565b9050919050565b6105a081610586565b82525050565b5f81549050919050565b5f82825260208201905092915050565b5f819050815f5260205f209050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52602260045260245ffd5b5f600282049050600182168061061657607f821691505b602082108103610629576106286105d2565b5b50919050565b5f82825260208201905092915050565b5f819050815f5260205f209050919050565b5f815461065d816105ff565b610667818661062f565b9450600182165f81146106815760018114610697576106c9565b60ff1983168652811515602002860193506106c9565b6106a08561063f565b5f5b838110156106c1578154818901526001820191506020810190506106a2565b808801955050505b50505092915050565b5f6106dd8383610651565b905092915050565b5f600182019050919050565b5f6106fb826105a6565b61070581856105b0565b935083602082028501610717856105c0565b805f5b858110156107515784840389528161073285826106d2565b945061073d836106e5565b925060208a0199505060018101905061071a565b50829750879550505050505092915050565b5f7fffffffff0000000000000000000000000000000000000000000000000000000082169050919050565b61079781610763565b82525050565b5f60a0820190506107b05f830188610597565b81810360208301526107c281876106f1565b905081810360408301526107d681866103d4565b90506107e5606083018561078e565b81810360808301526107f781846103d4565b90509695505050505050565b5f80fd5b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b61083d826103c4565b810181811067ffffffffffffffff8211171561085c5761085b610807565b5b80604052505050565b5f61086e61042c565b905061087a8282610834565b919050565b5f67ffffffffffffffff82111561089957610898610807565b5b6108a2826103c4565b9050602081019050919050565b828183375f83830152505050565b5f6108cf6108ca8461087f565b610865565b9050828152602081018484840111156108eb576108ea610803565b5b6108f68482856108af565b509392505050565b5f82601f8301126109125761091161043d565b5b81356109228482602086016108bd565b91505092915050565b5f602082840312156109405761093f610435565b5b5f82013567ffffffffffffffff81111561095d5761095c610439565b5b610969848285016108fe565b91505092915050565b5f81519050919050565b5f81905092915050565b5f61099082610972565b61099a818561097c565b93506109aa81856020860161039c565b80840191505092915050565b5f6109c18284610986565b915081905092915050565b5f82825260208201905092915050565b7f7465737420646174612076616c69646174696f6e206661696c65642e000000005f82015250565b5f610a10601c836109cc565b9150610a1b826109dc565b602082019050919050565b5f6020820190508181035f830152610a3d81610a04565b9050919050565b5f610a4f838561038c565b9350610a5c8385846108af565b610a65836103c4565b840190509392505050565b5f60a082019050610a835f83018a610597565b8181036020830152610a9581896106f1565b90508181036040830152610aaa818789610a44565b9050610ab9606083018661078e565b8181036080830152610acc818486610a44565b905098975050505050505050565b7f68747470207265717565737420726573756c742076616c69646174696f6e20665f8201527f61696c65642e0000000000000000000000000000000000000000000000000000602082015250565b5f610b346026836109cc565b9150610b3f82610ada565b604082019050919050565b5f6020820190508181035f830152610b6181610b28565b9050919050565b7f6578747261446174612076616c69646174696f6e206661696c65642e000000005f82015250565b5f610b9c601c836109cc565b9150610ba782610b68565b602082019050919050565b5f6020820190508181035f830152610bc981610b90565b905091905056fea2646970667358221220bd330fe0ab45b92249f619f1ea882a9968f3ecdb87bad932a45810389165729864736f6c63430008140033"  # noqa: E501
 OFFCHAIN_LOOKUP_ABI = [
     {
         "inputs": [
             {"internalType": "address", "name": "sender", "type": "address"},
             {"internalType": "string[]", "name": "urls", "type": "string[]"},
             {"internalType": "bytes", "name": "callData", "type": "bytes"},
             {"internalType": "bytes4", "name": "callbackFunction", "type": "bytes4"},
```

### Comparing `web3-6.3.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py` & `web3-6.4.0/web3/_utils/contract_sources/contract_data/tuple_contracts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Generated by `compile_contracts.py` script.
-Compiled with Solidity v0.8.19.
+Compiled with Solidity v0.8.20.
 """
 
 # source: web3/_utils/contract_sources/TupleContracts.sol:TupleContract
-TUPLE_CONTRACT_BYTECODE = "0x608060405234801561001057600080fd5b50610abb806100206000396000f3fe608060405234801561001057600080fd5b506004361061002b5760003560e01c80638e1ae3c714610030575b600080fd5b61004a6004803603810190610045919061067b565b610060565b6040516100579190610a63565b60405180910390f35b610068610070565b819050919050565b60405180606001604052806000815260200160608152602001606081525090565b6000604051905090565b600080fd5b600080fd5b600080fd5b6000601f19601f8301169050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b6100f3826100aa565b810181811067ffffffffffffffff82111715610112576101116100bb565b5b80604052505050565b6000610125610091565b905061013182826100ea565b919050565b600080fd5b6000819050919050565b61014e8161013b565b811461015957600080fd5b50565b60008135905061016b81610145565b92915050565b600080fd5b600067ffffffffffffffff821115610191576101906100bb565b5b602082029050602081019050919050565b600080fd5b60006101ba6101b584610176565b61011b565b905080838252602082019050602084028301858111156101dd576101dc6101a2565b5b835b8181101561020657806101f2888261015c565b8452602084019350506020810190506101df565b5050509392505050565b600082601f83011261022557610224610171565b5b81356102358482602086016101a7565b91505092915050565b600067ffffffffffffffff821115610259576102586100bb565b5b602082029050602081019050919050565b6000819050919050565b61027d8161026a565b811461028857600080fd5b50565b60008135905061029a81610274565b92915050565b600067ffffffffffffffff8211156102bb576102ba6100bb565b5b602082029050919050565b60008115159050919050565b6102db816102c6565b81146102e657600080fd5b50565b6000813590506102f8816102d2565b92915050565b600061031161030c846102a0565b61011b565b9050806020840283018581111561032b5761032a6101a2565b5b835b81811015610354578061034088826102e9565b84526020840193505060208101905061032d565b5050509392505050565b600082601f83011261037357610372610171565b5b60026103808482856102fe565b91505092915050565b600067ffffffffffffffff8211156103a4576103a36100bb565b5b602082029050602081019050919050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006103e0826103b5565b9050919050565b6103f0816103d5565b81146103fb57600080fd5b50565b60008135905061040d816103e7565b92915050565b600061042661042184610389565b61011b565b90508083825260208201905060208402830185811115610449576104486101a2565b5b835b81811015610472578061045e88826103fe565b84526020840193505060208101905061044b565b5050509392505050565b600082601f83011261049157610490610171565b5b81356104a1848260208601610413565b91505092915050565b6000608082840312156104c0576104bf6100a5565b5b6104ca606061011b565b905060006104da8482850161028b565b60008301525060206104ee8482850161035e565b602083015250606082013567ffffffffffffffff81111561051257610511610136565b5b61051e8482850161047c565b60408301525092915050565b600061053d6105388461023e565b61011b565b905080838252602082019050602084028301858111156105605761055f6101a2565b5b835b818110156105a757803567ffffffffffffffff81111561058557610584610171565b5b80860161059289826104aa565b85526020850194505050602081019050610562565b5050509392505050565b600082601f8301126105c6576105c5610171565b5b81356105d684826020860161052a565b91505092915050565b6000606082840312156105f5576105f46100a5565b5b6105ff606061011b565b9050600061060f8482850161015c565b600083015250602082013567ffffffffffffffff81111561063357610632610136565b5b61063f84828501610210565b602083015250604082013567ffffffffffffffff81111561066357610662610136565b5b61066f848285016105b1565b60408301525092915050565b6000602082840312156106915761069061009b565b5b600082013567ffffffffffffffff8111156106af576106ae6100a0565b5b6106bb848285016105df565b91505092915050565b6106cd8161013b565b82525050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b600061070b83836106c4565b60208301905092915050565b6000602082019050919050565b600061072f826106d3565b61073981856106de565b9350610744836106ef565b8060005b8381101561077557815161075c88826106ff565b975061076783610717565b925050600181019050610748565b5085935050505092915050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b6107b78161026a565b82525050565b600060029050919050565b600081905092915050565b6000819050919050565b6107e6816102c6565b82525050565b60006107f883836107dd565b60208301905092915050565b6000602082019050919050565b61081a816107bd565b61082481846107c8565b925061082f826107d3565b8060005b8381101561086057815161084787826107ec565b965061085283610804565b925050600181019050610833565b505050505050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b61089d816103d5565b82525050565b60006108af8383610894565b60208301905092915050565b6000602082019050919050565b60006108d382610868565b6108dd8185610873565b93506108e883610884565b8060005b8381101561091957815161090088826108a3565b975061090b836108bb565b9250506001810190506108ec565b5085935050505092915050565b600060808301600083015161093e60008601826107ae565b5060208301516109516020860182610811565b506040830151848203606086015261096982826108c8565b9150508091505092915050565b60006109828383610926565b905092915050565b6000602082019050919050565b60006109a282610782565b6109ac818561078d565b9350836020820285016109be8561079e565b8060005b858110156109fa57848403895281516109db8582610976565b94506109e68361098a565b925060208a019950506001810190506109c2565b50829750879550505050505092915050565b6000606083016000830151610a2460008601826106c4565b5060208301518482036020860152610a3c8282610724565b91505060408301518482036040860152610a568282610997565b9150508091505092915050565b60006020820190508181036000830152610a7d8184610a0c565b90509291505056fea2646970667358221220dea5e33843b81f2de0d4fc732506054d77f009d84e7ee6273aef6ac06f72ce7464736f6c63430008130033"  # noqa: E501
-TUPLE_CONTRACT_RUNTIME = "0x608060405234801561001057600080fd5b506004361061002b5760003560e01c80638e1ae3c714610030575b600080fd5b61004a6004803603810190610045919061067b565b610060565b6040516100579190610a63565b60405180910390f35b610068610070565b819050919050565b60405180606001604052806000815260200160608152602001606081525090565b6000604051905090565b600080fd5b600080fd5b600080fd5b6000601f19601f8301169050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b6100f3826100aa565b810181811067ffffffffffffffff82111715610112576101116100bb565b5b80604052505050565b6000610125610091565b905061013182826100ea565b919050565b600080fd5b6000819050919050565b61014e8161013b565b811461015957600080fd5b50565b60008135905061016b81610145565b92915050565b600080fd5b600067ffffffffffffffff821115610191576101906100bb565b5b602082029050602081019050919050565b600080fd5b60006101ba6101b584610176565b61011b565b905080838252602082019050602084028301858111156101dd576101dc6101a2565b5b835b8181101561020657806101f2888261015c565b8452602084019350506020810190506101df565b5050509392505050565b600082601f83011261022557610224610171565b5b81356102358482602086016101a7565b91505092915050565b600067ffffffffffffffff821115610259576102586100bb565b5b602082029050602081019050919050565b6000819050919050565b61027d8161026a565b811461028857600080fd5b50565b60008135905061029a81610274565b92915050565b600067ffffffffffffffff8211156102bb576102ba6100bb565b5b602082029050919050565b60008115159050919050565b6102db816102c6565b81146102e657600080fd5b50565b6000813590506102f8816102d2565b92915050565b600061031161030c846102a0565b61011b565b9050806020840283018581111561032b5761032a6101a2565b5b835b81811015610354578061034088826102e9565b84526020840193505060208101905061032d565b5050509392505050565b600082601f83011261037357610372610171565b5b60026103808482856102fe565b91505092915050565b600067ffffffffffffffff8211156103a4576103a36100bb565b5b602082029050602081019050919050565b600073ffffffffffffffffffffffffffffffffffffffff82169050919050565b60006103e0826103b5565b9050919050565b6103f0816103d5565b81146103fb57600080fd5b50565b60008135905061040d816103e7565b92915050565b600061042661042184610389565b61011b565b90508083825260208201905060208402830185811115610449576104486101a2565b5b835b81811015610472578061045e88826103fe565b84526020840193505060208101905061044b565b5050509392505050565b600082601f83011261049157610490610171565b5b81356104a1848260208601610413565b91505092915050565b6000608082840312156104c0576104bf6100a5565b5b6104ca606061011b565b905060006104da8482850161028b565b60008301525060206104ee8482850161035e565b602083015250606082013567ffffffffffffffff81111561051257610511610136565b5b61051e8482850161047c565b60408301525092915050565b600061053d6105388461023e565b61011b565b905080838252602082019050602084028301858111156105605761055f6101a2565b5b835b818110156105a757803567ffffffffffffffff81111561058557610584610171565b5b80860161059289826104aa565b85526020850194505050602081019050610562565b5050509392505050565b600082601f8301126105c6576105c5610171565b5b81356105d684826020860161052a565b91505092915050565b6000606082840312156105f5576105f46100a5565b5b6105ff606061011b565b9050600061060f8482850161015c565b600083015250602082013567ffffffffffffffff81111561063357610632610136565b5b61063f84828501610210565b602083015250604082013567ffffffffffffffff81111561066357610662610136565b5b61066f848285016105b1565b60408301525092915050565b6000602082840312156106915761069061009b565b5b600082013567ffffffffffffffff8111156106af576106ae6100a0565b5b6106bb848285016105df565b91505092915050565b6106cd8161013b565b82525050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b600061070b83836106c4565b60208301905092915050565b6000602082019050919050565b600061072f826106d3565b61073981856106de565b9350610744836106ef565b8060005b8381101561077557815161075c88826106ff565b975061076783610717565b925050600181019050610748565b5085935050505092915050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b6107b78161026a565b82525050565b600060029050919050565b600081905092915050565b6000819050919050565b6107e6816102c6565b82525050565b60006107f883836107dd565b60208301905092915050565b6000602082019050919050565b61081a816107bd565b61082481846107c8565b925061082f826107d3565b8060005b8381101561086057815161084787826107ec565b965061085283610804565b925050600181019050610833565b505050505050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b61089d816103d5565b82525050565b60006108af8383610894565b60208301905092915050565b6000602082019050919050565b60006108d382610868565b6108dd8185610873565b93506108e883610884565b8060005b8381101561091957815161090088826108a3565b975061090b836108bb565b9250506001810190506108ec565b5085935050505092915050565b600060808301600083015161093e60008601826107ae565b5060208301516109516020860182610811565b506040830151848203606086015261096982826108c8565b9150508091505092915050565b60006109828383610926565b905092915050565b6000602082019050919050565b60006109a282610782565b6109ac818561078d565b9350836020820285016109be8561079e565b8060005b858110156109fa57848403895281516109db8582610976565b94506109e68361098a565b925060208a019950506001810190506109c2565b50829750879550505050505092915050565b6000606083016000830151610a2460008601826106c4565b5060208301518482036020860152610a3c8282610724565b91505060408301518482036040860152610a568282610997565b9150508091505092915050565b60006020820190508181036000830152610a7d8184610a0c565b90509291505056fea2646970667358221220dea5e33843b81f2de0d4fc732506054d77f009d84e7ee6273aef6ac06f72ce7464736f6c63430008130033"  # noqa: E501
+TUPLE_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b50610a688061001d5f395ff3fe608060405234801561000f575f80fd5b5060043610610029575f3560e01c80638e1ae3c71461002d575b5f80fd5b6100476004803603810190610042919061064d565b61005d565b6040516100549190610a12565b60405180910390f35b61006561006d565b819050919050565b60405180606001604052805f815260200160608152602001606081525090565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6100e8826100a2565b810181811067ffffffffffffffff82111715610107576101066100b2565b5b80604052505050565b5f61011961008d565b905061012582826100df565b919050565b5f80fd5b5f819050919050565b6101408161012e565b811461014a575f80fd5b50565b5f8135905061015b81610137565b92915050565b5f80fd5b5f67ffffffffffffffff82111561017f5761017e6100b2565b5b602082029050602081019050919050565b5f80fd5b5f6101a66101a184610165565b610110565b905080838252602082019050602084028301858111156101c9576101c8610190565b5b835b818110156101f257806101de888261014d565b8452602084019350506020810190506101cb565b5050509392505050565b5f82601f8301126102105761020f610161565b5b8135610220848260208601610194565b91505092915050565b5f67ffffffffffffffff821115610243576102426100b2565b5b602082029050602081019050919050565b5f819050919050565b61026681610254565b8114610270575f80fd5b50565b5f813590506102818161025d565b92915050565b5f67ffffffffffffffff8211156102a1576102a06100b2565b5b602082029050919050565b5f8115159050919050565b6102c0816102ac565b81146102ca575f80fd5b50565b5f813590506102db816102b7565b92915050565b5f6102f36102ee84610287565b610110565b9050806020840283018581111561030d5761030c610190565b5b835b81811015610336578061032288826102cd565b84526020840193505060208101905061030f565b5050509392505050565b5f82601f83011261035457610353610161565b5b60026103618482856102e1565b91505092915050565b5f67ffffffffffffffff821115610384576103836100b2565b5b602082029050602081019050919050565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6103be82610395565b9050919050565b6103ce816103b4565b81146103d8575f80fd5b50565b5f813590506103e9816103c5565b92915050565b5f6104016103fc8461036a565b610110565b9050808382526020820190506020840283018581111561042457610423610190565b5b835b8181101561044d578061043988826103db565b845260208401935050602081019050610426565b5050509392505050565b5f82601f83011261046b5761046a610161565b5b813561047b8482602086016103ef565b91505092915050565b5f608082840312156104995761049861009e565b5b6104a36060610110565b90505f6104b284828501610273565b5f8301525060206104c584828501610340565b602083015250606082013567ffffffffffffffff8111156104e9576104e861012a565b5b6104f584828501610457565b60408301525092915050565b5f61051361050e84610229565b610110565b9050808382526020820190506020840283018581111561053657610535610190565b5b835b8181101561057d57803567ffffffffffffffff81111561055b5761055a610161565b5b8086016105688982610484565b85526020850194505050602081019050610538565b5050509392505050565b5f82601f83011261059b5761059a610161565b5b81356105ab848260208601610501565b91505092915050565b5f606082840312156105c9576105c861009e565b5b6105d36060610110565b90505f6105e28482850161014d565b5f83015250602082013567ffffffffffffffff8111156106055761060461012a565b5b610611848285016101fc565b602083015250604082013567ffffffffffffffff8111156106355761063461012a565b5b61064184828501610587565b60408301525092915050565b5f6020828403121561066257610661610096565b5b5f82013567ffffffffffffffff81111561067f5761067e61009a565b5b61068b848285016105b4565b91505092915050565b61069d8161012e565b82525050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b5f6106d78383610694565b60208301905092915050565b5f602082019050919050565b5f6106f9826106a3565b61070381856106ad565b935061070e836106bd565b805f5b8381101561073e57815161072588826106cc565b9750610730836106e3565b925050600181019050610711565b5085935050505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b61077d81610254565b82525050565b5f60029050919050565b5f81905092915050565b5f819050919050565b6107a9816102ac565b82525050565b5f6107ba83836107a0565b60208301905092915050565b5f602082019050919050565b6107db81610783565b6107e5818461078d565b92506107f082610797565b805f5b8381101561082057815161080787826107af565b9650610812836107c6565b9250506001810190506107f3565b505050505050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b61085a816103b4565b82525050565b5f61086b8383610851565b60208301905092915050565b5f602082019050919050565b5f61088d82610828565b6108978185610832565b93506108a283610842565b805f5b838110156108d25781516108b98882610860565b97506108c483610877565b9250506001810190506108a5565b5085935050505092915050565b5f608083015f8301516108f45f860182610774565b50602083015161090760208601826107d2565b506040830151848203606086015261091f8282610883565b9150508091505092915050565b5f61093783836108df565b905092915050565b5f602082019050919050565b5f6109558261074b565b61095f8185610755565b93508360208202850161097185610765565b805f5b858110156109ac578484038952815161098d858261092c565b94506109988361093f565b925060208a01995050600181019050610974565b50829750879550505050505092915050565b5f606083015f8301516109d35f860182610694565b50602083015184820360208601526109eb82826106ef565b91505060408301518482036040860152610a05828261094b565b9150508091505092915050565b5f6020820190508181035f830152610a2a81846109be565b90509291505056fea2646970667358221220b662d127aaa31db3b40e31d9a4d477f05b8643f2195ec8a957108cdbe8a79be364736f6c63430008140033"  # noqa: E501
+TUPLE_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b5060043610610029575f3560e01c80638e1ae3c71461002d575b5f80fd5b6100476004803603810190610042919061064d565b61005d565b6040516100549190610a12565b60405180910390f35b61006561006d565b819050919050565b60405180606001604052805f815260200160608152602001606081525090565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6100e8826100a2565b810181811067ffffffffffffffff82111715610107576101066100b2565b5b80604052505050565b5f61011961008d565b905061012582826100df565b919050565b5f80fd5b5f819050919050565b6101408161012e565b811461014a575f80fd5b50565b5f8135905061015b81610137565b92915050565b5f80fd5b5f67ffffffffffffffff82111561017f5761017e6100b2565b5b602082029050602081019050919050565b5f80fd5b5f6101a66101a184610165565b610110565b905080838252602082019050602084028301858111156101c9576101c8610190565b5b835b818110156101f257806101de888261014d565b8452602084019350506020810190506101cb565b5050509392505050565b5f82601f8301126102105761020f610161565b5b8135610220848260208601610194565b91505092915050565b5f67ffffffffffffffff821115610243576102426100b2565b5b602082029050602081019050919050565b5f819050919050565b61026681610254565b8114610270575f80fd5b50565b5f813590506102818161025d565b92915050565b5f67ffffffffffffffff8211156102a1576102a06100b2565b5b602082029050919050565b5f8115159050919050565b6102c0816102ac565b81146102ca575f80fd5b50565b5f813590506102db816102b7565b92915050565b5f6102f36102ee84610287565b610110565b9050806020840283018581111561030d5761030c610190565b5b835b81811015610336578061032288826102cd565b84526020840193505060208101905061030f565b5050509392505050565b5f82601f83011261035457610353610161565b5b60026103618482856102e1565b91505092915050565b5f67ffffffffffffffff821115610384576103836100b2565b5b602082029050602081019050919050565b5f73ffffffffffffffffffffffffffffffffffffffff82169050919050565b5f6103be82610395565b9050919050565b6103ce816103b4565b81146103d8575f80fd5b50565b5f813590506103e9816103c5565b92915050565b5f6104016103fc8461036a565b610110565b9050808382526020820190506020840283018581111561042457610423610190565b5b835b8181101561044d578061043988826103db565b845260208401935050602081019050610426565b5050509392505050565b5f82601f83011261046b5761046a610161565b5b813561047b8482602086016103ef565b91505092915050565b5f608082840312156104995761049861009e565b5b6104a36060610110565b90505f6104b284828501610273565b5f8301525060206104c584828501610340565b602083015250606082013567ffffffffffffffff8111156104e9576104e861012a565b5b6104f584828501610457565b60408301525092915050565b5f61051361050e84610229565b610110565b9050808382526020820190506020840283018581111561053657610535610190565b5b835b8181101561057d57803567ffffffffffffffff81111561055b5761055a610161565b5b8086016105688982610484565b85526020850194505050602081019050610538565b5050509392505050565b5f82601f83011261059b5761059a610161565b5b81356105ab848260208601610501565b91505092915050565b5f606082840312156105c9576105c861009e565b5b6105d36060610110565b90505f6105e28482850161014d565b5f83015250602082013567ffffffffffffffff8111156106055761060461012a565b5b610611848285016101fc565b602083015250604082013567ffffffffffffffff8111156106355761063461012a565b5b61064184828501610587565b60408301525092915050565b5f6020828403121561066257610661610096565b5b5f82013567ffffffffffffffff81111561067f5761067e61009a565b5b61068b848285016105b4565b91505092915050565b61069d8161012e565b82525050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b5f6106d78383610694565b60208301905092915050565b5f602082019050919050565b5f6106f9826106a3565b61070381856106ad565b935061070e836106bd565b805f5b8381101561073e57815161072588826106cc565b9750610730836106e3565b925050600181019050610711565b5085935050505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b61077d81610254565b82525050565b5f60029050919050565b5f81905092915050565b5f819050919050565b6107a9816102ac565b82525050565b5f6107ba83836107a0565b60208301905092915050565b5f602082019050919050565b6107db81610783565b6107e5818461078d565b92506107f082610797565b805f5b8381101561082057815161080787826107af565b9650610812836107c6565b9250506001810190506107f3565b505050505050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b61085a816103b4565b82525050565b5f61086b8383610851565b60208301905092915050565b5f602082019050919050565b5f61088d82610828565b6108978185610832565b93506108a283610842565b805f5b838110156108d25781516108b98882610860565b97506108c483610877565b9250506001810190506108a5565b5085935050505092915050565b5f608083015f8301516108f45f860182610774565b50602083015161090760208601826107d2565b506040830151848203606086015261091f8282610883565b9150508091505092915050565b5f61093783836108df565b905092915050565b5f602082019050919050565b5f6109558261074b565b61095f8185610755565b93508360208202850161097185610765565b805f5b858110156109ac578484038952815161098d858261092c565b94506109988361093f565b925060208a01995050600181019050610974565b50829750879550505050505092915050565b5f606083015f8301516109d35f860182610694565b50602083015184820360208601526109eb82826106ef565b91505060408301518482036040860152610a05828261094b565b9150508091505092915050565b5f6020820190508181035f830152610a2a81846109be565b90509291505056fea2646970667358221220b662d127aaa31db3b40e31d9a4d477f05b8643f2195ec8a957108cdbe8a79be364736f6c63430008140033"  # noqa: E501
 TUPLE_CONTRACT_ABI = [
     {
         "inputs": [
             {
                 "components": [
                     {"internalType": "uint256", "name": "a", "type": "uint256"},
                     {"internalType": "uint256[]", "name": "b", "type": "uint256[]"},
@@ -67,16 +67,16 @@
     "bytecode": TUPLE_CONTRACT_BYTECODE,
     "bytecode_runtime": TUPLE_CONTRACT_RUNTIME,
     "abi": TUPLE_CONTRACT_ABI,
 }
 
 
 # source: web3/_utils/contract_sources/TupleContracts.sol:NestedTupleContract
-NESTED_TUPLE_CONTRACT_BYTECODE = "0x608060405234801561001057600080fd5b506106b5806100206000396000f3fe608060405234801561001057600080fd5b506004361061002b5760003560e01c80632655aef114610030575b600080fd5b61004a60048036038101906100459190610411565b610060565b604051610057919061065d565b60405180910390f35b610068610070565b819050919050565b6040518060200160405280606081525090565b6000604051905090565b600080fd5b600080fd5b600080fd5b6000601f19601f8301169050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b6100e58261009c565b810181811067ffffffffffffffff82111715610104576101036100ad565b5b80604052505050565b6000610117610083565b905061012382826100dc565b919050565b600080fd5b600080fd5b600067ffffffffffffffff82111561014d5761014c6100ad565b5b602082029050602081019050919050565b600080fd5b600067ffffffffffffffff82111561017e5761017d6100ad565b5b602082029050602081019050919050565b6000819050919050565b6101a28161018f565b81146101ad57600080fd5b50565b6000813590506101bf81610199565b92915050565b6000604082840312156101db576101da610097565b5b6101e5604061010d565b905060006101f5848285016101b0565b6000830152506020610209848285016101b0565b60208301525092915050565b600061022861022384610163565b61010d565b9050808382526020820190506040840283018581111561024b5761024a61015e565b5b835b81811015610274578061026088826101c5565b84526020840193505060408101905061024d565b5050509392505050565b600082601f8301126102935761029261012d565b5b81356102a3848260208601610215565b91505092915050565b6000602082840312156102c2576102c1610097565b5b6102cc602061010d565b9050600082013567ffffffffffffffff8111156102ec576102eb610128565b5b6102f88482850161027e565b60008301525092915050565b600061031761031284610132565b61010d565b9050808382526020820190506020840283018581111561033a5761033961015e565b5b835b8181101561038157803567ffffffffffffffff81111561035f5761035e61012d565b5b80860161036c89826102ac565b8552602085019450505060208101905061033c565b5050509392505050565b600082601f8301126103a05761039f61012d565b5b81356103b0848260208601610304565b91505092915050565b6000602082840312156103cf576103ce610097565b5b6103d9602061010d565b9050600082013567ffffffffffffffff8111156103f9576103f8610128565b5b6104058482850161038b565b60008301525092915050565b6000602082840312156104275761042661008d565b5b600082013567ffffffffffffffff81111561044557610444610092565b5b610451848285016103b9565b91505092915050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b6104bb8161018f565b82525050565b6040820160008201516104d760008501826104b2565b5060208201516104ea60208501826104b2565b50505050565b60006104fc83836104c1565b60408301905092915050565b6000602082019050919050565b600061052082610486565b61052a8185610491565b9350610535836104a2565b8060005b8381101561056657815161054d88826104f0565b975061055883610508565b925050600181019050610539565b5085935050505092915050565b600060208301600083015184820360008601526105908282610515565b9150508091505092915050565b60006105a98383610573565b905092915050565b6000602082019050919050565b60006105c98261045a565b6105d38185610465565b9350836020820285016105e585610476565b8060005b858110156106215784840389528151610602858261059d565b945061060d836105b1565b925060208a019950506001810190506105e9565b50829750879550505050505092915050565b6000602083016000830151848203600086015261065082826105be565b9150508091505092915050565b600060208201905081810360008301526106778184610633565b90509291505056fea2646970667358221220376ab34c60e2c0b20b9d41029acf2e00addc4091efcfc60e8b61baaf2a25136764736f6c63430008130033"  # noqa: E501
-NESTED_TUPLE_CONTRACT_RUNTIME = "0x608060405234801561001057600080fd5b506004361061002b5760003560e01c80632655aef114610030575b600080fd5b61004a60048036038101906100459190610411565b610060565b604051610057919061065d565b60405180910390f35b610068610070565b819050919050565b6040518060200160405280606081525090565b6000604051905090565b600080fd5b600080fd5b600080fd5b6000601f19601f8301169050919050565b7f4e487b7100000000000000000000000000000000000000000000000000000000600052604160045260246000fd5b6100e58261009c565b810181811067ffffffffffffffff82111715610104576101036100ad565b5b80604052505050565b6000610117610083565b905061012382826100dc565b919050565b600080fd5b600080fd5b600067ffffffffffffffff82111561014d5761014c6100ad565b5b602082029050602081019050919050565b600080fd5b600067ffffffffffffffff82111561017e5761017d6100ad565b5b602082029050602081019050919050565b6000819050919050565b6101a28161018f565b81146101ad57600080fd5b50565b6000813590506101bf81610199565b92915050565b6000604082840312156101db576101da610097565b5b6101e5604061010d565b905060006101f5848285016101b0565b6000830152506020610209848285016101b0565b60208301525092915050565b600061022861022384610163565b61010d565b9050808382526020820190506040840283018581111561024b5761024a61015e565b5b835b81811015610274578061026088826101c5565b84526020840193505060408101905061024d565b5050509392505050565b600082601f8301126102935761029261012d565b5b81356102a3848260208601610215565b91505092915050565b6000602082840312156102c2576102c1610097565b5b6102cc602061010d565b9050600082013567ffffffffffffffff8111156102ec576102eb610128565b5b6102f88482850161027e565b60008301525092915050565b600061031761031284610132565b61010d565b9050808382526020820190506020840283018581111561033a5761033961015e565b5b835b8181101561038157803567ffffffffffffffff81111561035f5761035e61012d565b5b80860161036c89826102ac565b8552602085019450505060208101905061033c565b5050509392505050565b600082601f8301126103a05761039f61012d565b5b81356103b0848260208601610304565b91505092915050565b6000602082840312156103cf576103ce610097565b5b6103d9602061010d565b9050600082013567ffffffffffffffff8111156103f9576103f8610128565b5b6104058482850161038b565b60008301525092915050565b6000602082840312156104275761042661008d565b5b600082013567ffffffffffffffff81111561044557610444610092565b5b610451848285016103b9565b91505092915050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b600081519050919050565b600082825260208201905092915050565b6000819050602082019050919050565b6104bb8161018f565b82525050565b6040820160008201516104d760008501826104b2565b5060208201516104ea60208501826104b2565b50505050565b60006104fc83836104c1565b60408301905092915050565b6000602082019050919050565b600061052082610486565b61052a8185610491565b9350610535836104a2565b8060005b8381101561056657815161054d88826104f0565b975061055883610508565b925050600181019050610539565b5085935050505092915050565b600060208301600083015184820360008601526105908282610515565b9150508091505092915050565b60006105a98383610573565b905092915050565b6000602082019050919050565b60006105c98261045a565b6105d38185610465565b9350836020820285016105e585610476565b8060005b858110156106215784840389528151610602858261059d565b945061060d836105b1565b925060208a019950506001810190506105e9565b50829750879550505050505092915050565b6000602083016000830151848203600086015261065082826105be565b9150508091505092915050565b600060208201905081810360008301526106778184610633565b90509291505056fea2646970667358221220376ab34c60e2c0b20b9d41029acf2e00addc4091efcfc60e8b61baaf2a25136764736f6c63430008130033"  # noqa: E501
+NESTED_TUPLE_CONTRACT_BYTECODE = "0x608060405234801561000f575f80fd5b5061067b8061001d5f395ff3fe608060405234801561000f575f80fd5b5060043610610029575f3560e01c80632655aef11461002d575b5f80fd5b610047600480360381019061004291906103f1565b61005d565b6040516100549190610625565b60405180910390f35b61006561006d565b819050919050565b6040518060200160405280606081525090565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6100db82610095565b810181811067ffffffffffffffff821117156100fa576100f96100a5565b5b80604052505050565b5f61010c610080565b905061011882826100d2565b919050565b5f80fd5b5f80fd5b5f67ffffffffffffffff82111561013f5761013e6100a5565b5b602082029050602081019050919050565b5f80fd5b5f67ffffffffffffffff82111561016e5761016d6100a5565b5b602082029050602081019050919050565b5f819050919050565b6101918161017f565b811461019b575f80fd5b50565b5f813590506101ac81610188565b92915050565b5f604082840312156101c7576101c6610091565b5b6101d16040610103565b90505f6101e08482850161019e565b5f8301525060206101f38482850161019e565b60208301525092915050565b5f61021161020c84610154565b610103565b9050808382526020820190506040840283018581111561023457610233610150565b5b835b8181101561025d578061024988826101b2565b845260208401935050604081019050610236565b5050509392505050565b5f82601f83011261027b5761027a610121565b5b813561028b8482602086016101ff565b91505092915050565b5f602082840312156102a9576102a8610091565b5b6102b36020610103565b90505f82013567ffffffffffffffff8111156102d2576102d161011d565b5b6102de84828501610267565b5f8301525092915050565b5f6102fb6102f684610125565b610103565b9050808382526020820190506020840283018581111561031e5761031d610150565b5b835b8181101561036557803567ffffffffffffffff81111561034357610342610121565b5b8086016103508982610294565b85526020850194505050602081019050610320565b5050509392505050565b5f82601f83011261038357610382610121565b5b81356103938482602086016102e9565b91505092915050565b5f602082840312156103b1576103b0610091565b5b6103bb6020610103565b90505f82013567ffffffffffffffff8111156103da576103d961011d565b5b6103e68482850161036f565b5f8301525092915050565b5f6020828403121561040657610405610089565b5b5f82013567ffffffffffffffff8111156104235761042261008d565b5b61042f8482850161039c565b91505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b6104938161017f565b82525050565b604082015f8201516104ad5f85018261048a565b5060208201516104c0602085018261048a565b50505050565b5f6104d18383610499565b60408301905092915050565b5f602082019050919050565b5f6104f382610461565b6104fd818561046b565b93506105088361047b565b805f5b8381101561053857815161051f88826104c6565b975061052a836104dd565b92505060018101905061050b565b5085935050505092915050565b5f602083015f8301518482035f86015261055f82826104e9565b9150508091505092915050565b5f6105778383610545565b905092915050565b5f602082019050919050565b5f61059582610438565b61059f8185610442565b9350836020820285016105b185610452565b805f5b858110156105ec57848403895281516105cd858261056c565b94506105d88361057f565b925060208a019950506001810190506105b4565b50829750879550505050505092915050565b5f602083015f8301518482035f860152610618828261058b565b9150508091505092915050565b5f6020820190508181035f83015261063d81846105fe565b90509291505056fea2646970667358221220e7fa69be8e34ef63f83a99439ab93276b8a4153d844fcad43ce448b247e32b7064736f6c63430008140033"  # noqa: E501
+NESTED_TUPLE_CONTRACT_RUNTIME = "0x608060405234801561000f575f80fd5b5060043610610029575f3560e01c80632655aef11461002d575b5f80fd5b610047600480360381019061004291906103f1565b61005d565b6040516100549190610625565b60405180910390f35b61006561006d565b819050919050565b6040518060200160405280606081525090565b5f604051905090565b5f80fd5b5f80fd5b5f80fd5b5f601f19601f8301169050919050565b7f4e487b71000000000000000000000000000000000000000000000000000000005f52604160045260245ffd5b6100db82610095565b810181811067ffffffffffffffff821117156100fa576100f96100a5565b5b80604052505050565b5f61010c610080565b905061011882826100d2565b919050565b5f80fd5b5f80fd5b5f67ffffffffffffffff82111561013f5761013e6100a5565b5b602082029050602081019050919050565b5f80fd5b5f67ffffffffffffffff82111561016e5761016d6100a5565b5b602082029050602081019050919050565b5f819050919050565b6101918161017f565b811461019b575f80fd5b50565b5f813590506101ac81610188565b92915050565b5f604082840312156101c7576101c6610091565b5b6101d16040610103565b90505f6101e08482850161019e565b5f8301525060206101f38482850161019e565b60208301525092915050565b5f61021161020c84610154565b610103565b9050808382526020820190506040840283018581111561023457610233610150565b5b835b8181101561025d578061024988826101b2565b845260208401935050604081019050610236565b5050509392505050565b5f82601f83011261027b5761027a610121565b5b813561028b8482602086016101ff565b91505092915050565b5f602082840312156102a9576102a8610091565b5b6102b36020610103565b90505f82013567ffffffffffffffff8111156102d2576102d161011d565b5b6102de84828501610267565b5f8301525092915050565b5f6102fb6102f684610125565b610103565b9050808382526020820190506020840283018581111561031e5761031d610150565b5b835b8181101561036557803567ffffffffffffffff81111561034357610342610121565b5b8086016103508982610294565b85526020850194505050602081019050610320565b5050509392505050565b5f82601f83011261038357610382610121565b5b81356103938482602086016102e9565b91505092915050565b5f602082840312156103b1576103b0610091565b5b6103bb6020610103565b90505f82013567ffffffffffffffff8111156103da576103d961011d565b5b6103e68482850161036f565b5f8301525092915050565b5f6020828403121561040657610405610089565b5b5f82013567ffffffffffffffff8111156104235761042261008d565b5b61042f8482850161039c565b91505092915050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b5f81519050919050565b5f82825260208201905092915050565b5f819050602082019050919050565b6104938161017f565b82525050565b604082015f8201516104ad5f85018261048a565b5060208201516104c0602085018261048a565b50505050565b5f6104d18383610499565b60408301905092915050565b5f602082019050919050565b5f6104f382610461565b6104fd818561046b565b93506105088361047b565b805f5b8381101561053857815161051f88826104c6565b975061052a836104dd565b92505060018101905061050b565b5085935050505092915050565b5f602083015f8301518482035f86015261055f82826104e9565b9150508091505092915050565b5f6105778383610545565b905092915050565b5f602082019050919050565b5f61059582610438565b61059f8185610442565b9350836020820285016105b185610452565b805f5b858110156105ec57848403895281516105cd858261056c565b94506105d88361057f565b925060208a019950506001810190506105b4565b50829750879550505050505092915050565b5f602083015f8301518482035f860152610618828261058b565b9150508091505092915050565b5f6020820190508181035f83015261063d81846105fe565b90509291505056fea2646970667358221220e7fa69be8e34ef63f83a99439ab93276b8a4153d844fcad43ce448b247e32b7064736f6c63430008140033"  # noqa: E501
 NESTED_TUPLE_CONTRACT_ABI = [
     {
         "inputs": [
             {
                 "components": [
                     {
                         "components": [
```

### Comparing `web3-6.3.0/web3/_utils/contracts.py` & `web3-6.4.0/web3/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/datatypes.py` & `web3-6.4.0/web3/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/decorators.py` & `web3-6.4.0/web3/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/encoding.py` & `web3-6.4.0/web3/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/ens.py` & `web3-6.4.0/web3/_utils/ens.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/events.py` & `web3-6.4.0/web3/_utils/events.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/fee_utils.py` & `web3-6.4.0/web3/_utils/fee_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/filters.py` & `web3-6.4.0/web3/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/formatters.py` & `web3-6.4.0/web3/_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/math.py` & `web3-6.4.0/web3/_utils/math.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/method_formatters.py` & `web3-6.4.0/web3/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/miner.py` & `web3-6.4.0/web3/_utils/miner.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module.py` & `web3-6.4.0/web3/_utils/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/__init__.py` & `web3-6.4.0/web3/_utils/module_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/eth_module.py` & `web3-6.4.0/web3/_utils/module_testing/eth_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/go_ethereum_admin_module.py` & `web3-6.4.0/web3/_utils/module_testing/go_ethereum_admin_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/go_ethereum_personal_module.py` & `web3-6.4.0/web3/_utils/module_testing/go_ethereum_personal_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/go_ethereum_txpool_module.py` & `web3-6.4.0/web3/_utils/module_testing/go_ethereum_txpool_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/module_testing_utils.py` & `web3-6.4.0/web3/_utils/module_testing/module_testing_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/net_module.py` & `web3-6.4.0/web3/_utils/module_testing/net_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/module_testing/web3_module.py` & `web3-6.4.0/web3/_utils/module_testing/web3_module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/normalizers.py` & `web3-6.4.0/web3/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/request.py` & `web3-6.4.0/web3/_utils/request.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/rpc_abi.py` & `web3-6.4.0/web3/_utils/rpc_abi.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/threads.py` & `web3-6.4.0/web3/_utils/threads.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/transactions.py` & `web3-6.4.0/web3/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/type_conversion.py` & `web3-6.4.0/web3/_utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/utility_methods.py` & `web3-6.4.0/web3/_utils/utility_methods.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/validation.py` & `web3-6.4.0/web3/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/_utils/windows.py` & `web3-6.4.0/web3/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/beacon/api_endpoints.py` & `web3-6.4.0/web3/beacon/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/beacon/async_beacon.py` & `web3-6.4.0/web3/beacon/async_beacon.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/beacon/main.py` & `web3-6.4.0/web3/beacon/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/contract/async_contract.py` & `web3-6.4.0/web3/contract/async_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/contract/base_contract.py` & `web3-6.4.0/web3/contract/base_contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/contract/contract.py` & `web3-6.4.0/web3/contract/contract.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/contract/utils.py` & `web3-6.4.0/web3/contract/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/datastructures.py` & `web3-6.4.0/web3/datastructures.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,23 +110,46 @@
                 "This data is immutable -- create a copy instead of modifying"
             )
 
     def __delattr__(self, key: str) -> None:
         raise TypeError("This data is immutable -- create a copy instead of modifying")
 
     def __hash__(self) -> int:
-        return hash(tuple(sorted(self.items())))
+        return hash(tuple(sorted(tupleize_lists_nested(self).items())))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Mapping):
             return self.__dict__ == dict(other)
         else:
             return False
 
 
+def tupleize_lists_nested(d: Mapping[TKey, TValue]) -> AttributeDict[TKey, TValue]:
+    """
+    Unhashable types inside dicts will throw an error if attempted to be hashed.
+    This method converts lists to tuples, rendering them hashable.
+    Other unhashable types found will raise a TypeError
+    """
+
+    def _to_tuple(lst: List[Any]) -> Any:
+        return tuple(_to_tuple(i) if isinstance(i, list) else i for i in lst)
+
+    ret = dict()
+    for k, v in d.items():
+        if isinstance(v, List):
+            ret[k] = _to_tuple(v)
+        elif isinstance(v, Mapping):
+            ret[k] = tupleize_lists_nested(v)
+        elif not isinstance(v, Hashable):
+            raise TypeError(f"Found unhashable type '{type(v).__name__}': {v}")
+        else:
+            ret[k] = v
+    return AttributeDict(ret)
+
+
 class NamedElementOnion(Mapping[TKey, TValue]):
     """
     Add layers to an onion-shaped structure. Optionally, inject to a specific layer.
     This structure is iterable, where the outermost layer is first, and innermost
     is last.
     """
```

### Comparing `web3-6.3.0/web3/eth/async_eth.py` & `web3-6.4.0/web3/eth/async_eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/eth/base_eth.py` & `web3-6.4.0/web3/eth/base_eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/eth/eth.py` & `web3-6.4.0/web3/eth/eth.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/exceptions.py` & `web3-6.4.0/web3/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/gas_strategies/time_based.py` & `web3-6.4.0/web3/gas_strategies/time_based.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/geth.py` & `web3-6.4.0/web3/geth.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/main.py` & `web3-6.4.0/web3/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/manager.py` & `web3-6.4.0/web3/manager.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/method.py` & `web3-6.4.0/web3/method.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/__init__.py` & `web3-6.4.0/web3/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/async_cache.py` & `web3-6.4.0/web3/middleware/async_cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/attrdict.py` & `web3-6.4.0/web3/middleware/attrdict.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/buffered_gas_estimate.py` & `web3-6.4.0/web3/middleware/buffered_gas_estimate.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/cache.py` & `web3-6.4.0/web3/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/exception_handling.py` & `web3-6.4.0/web3/middleware/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/exception_retry_request.py` & `web3-6.4.0/web3/middleware/exception_retry_request.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/filter.py` & `web3-6.4.0/web3/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/fixture.py` & `web3-6.4.0/web3/middleware/fixture.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/formatting.py` & `web3-6.4.0/web3/middleware/formatting.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/gas_price_strategy.py` & `web3-6.4.0/web3/middleware/gas_price_strategy.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/geth_poa.py` & `web3-6.4.0/web3/middleware/geth_poa.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/names.py` & `web3-6.4.0/web3/middleware/names.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/signing.py` & `web3-6.4.0/web3/middleware/signing.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/simulate_unmined_transaction.py` & `web3-6.4.0/web3/middleware/simulate_unmined_transaction.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/stalecheck.py` & `web3-6.4.0/web3/middleware/stalecheck.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/middleware/validation.py` & `web3-6.4.0/web3/middleware/validation.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/module.py` & `web3-6.4.0/web3/module.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/net.py` & `web3-6.4.0/web3/net.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/pm.py` & `web3-6.4.0/web3/pm.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/async_base.py` & `web3-6.4.0/web3/providers/async_base.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/async_rpc.py` & `web3-6.4.0/web3/providers/async_rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/auto.py` & `web3-6.4.0/web3/providers/auto.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/base.py` & `web3-6.4.0/web3/providers/base.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/eth_tester/defaults.py` & `web3-6.4.0/web3/providers/eth_tester/defaults.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/eth_tester/main.py` & `web3-6.4.0/web3/providers/eth_tester/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/eth_tester/middleware.py` & `web3-6.4.0/web3/providers/eth_tester/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,20 +99,14 @@
 transaction_request_formatter = apply_formatters_to_dict(TRANSACTION_REQUEST_FORMATTERS)
 
 transaction_request_transformer = compose(
     transaction_request_remapper,
     transaction_request_formatter,
 )
 
-BLOCK_FORMATTERS = {
-    "logsBloom": integer_to_hex,
-}
-block_formatter = apply_formatters_to_dict(BLOCK_FORMATTERS)
-
-
 FILTER_REQUEST_KEY_MAPPING = {
     "fromBlock": "from_block",
     "toBlock": "to_block",
 }
 filter_request_remapper = apply_key_map(FILTER_REQUEST_KEY_MAPPING)
 
 
@@ -189,17 +183,26 @@
     "gas_used": "gasUsed",
     "base_fee_per_gas": "baseFeePerGas",
     "mix_hash": "mixHash",
     # eth-tester changed the miner key to coinbase since
     # there is no longer any mining happening, but the current
     # JSON-RPC spec still says miner
     "coinbase": "miner",
+    "withdrawals_root": "withdrawalsRoot",
 }
 block_result_remapper = apply_key_map(BLOCK_RESULT_KEY_MAPPING)
 
+BLOCK_RESULT_FORMATTERS = {
+    "logsBloom": integer_to_hex,
+    "withdrawals": apply_list_to_array_formatter(
+        apply_key_map({"validator_index": "validatorIndex"}),
+    ),
+}
+block_result_formatter = apply_formatters_to_dict(BLOCK_RESULT_FORMATTERS)
+
 
 RECEIPT_RESULT_FORMATTERS = {
     "logs": apply_list_to_array_formatter(log_result_remapper),
 }
 receipt_result_formatter = apply_formatters_to_dict(RECEIPT_RESULT_FORMATTERS)
 
 request_formatters = {
@@ -263,19 +266,19 @@
         transaction_request_transformer,
         identity,
     ),
 }
 result_formatters: Optional[Dict[RPCEndpoint, Callable[..., Any]]] = {
     RPCEndpoint("eth_getBlockByHash"): apply_formatter_if(
         is_dict,
-        compose(block_result_remapper, block_formatter),
+        compose(block_result_remapper, block_result_formatter),
     ),
     RPCEndpoint("eth_getBlockByNumber"): apply_formatter_if(
         is_dict,
-        compose(block_result_remapper, block_formatter),
+        compose(block_result_remapper, block_result_formatter),
     ),
     RPCEndpoint("eth_getBlockTransactionCountByHash"): apply_formatter_if(
         is_dict,
         transaction_result_remapper,
     ),
     RPCEndpoint("eth_getBlockTransactionCountByNumber"): apply_formatter_if(
         is_dict,
```

### Comparing `web3-6.3.0/web3/providers/ipc.py` & `web3-6.4.0/web3/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/rpc.py` & `web3-6.4.0/web3/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/providers/websocket.py` & `web3-6.4.0/web3/providers/websocket.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/scripts/release/test_package.py` & `web3-6.4.0/web3/scripts/release/test_package.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/testing.py` & `web3-6.4.0/web3/testing.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/benchmark/main.py` & `web3-6.4.0/web3/tools/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/benchmark/node.py` & `web3-6.4.0/web3/tools/benchmark/node.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/benchmark/reporting.py` & `web3-6.4.0/web3/tools/benchmark/reporting.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/benchmark/utils.py` & `web3-6.4.0/web3/tools/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/pytest_ethereum/_utils.py` & `web3-6.4.0/web3/tools/pytest_ethereum/_utils.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/pytest_ethereum/deployer.py` & `web3-6.4.0/web3/tools/pytest_ethereum/deployer.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/pytest_ethereum/linker.py` & `web3-6.4.0/web3/tools/pytest_ethereum/linker.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tools/pytest_ethereum/plugins.py` & `web3-6.4.0/web3/tools/pytest_ethereum/plugins.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/tracing.py` & `web3-6.4.0/web3/tracing.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/types.py` & `web3-6.4.0/web3/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 _Hash32 = Union[Hash32, HexBytes, HexStr]
 EnodeURI = NewType("EnodeURI", str)
 ENS = NewType("ENS", str)
 Nonce = NewType("Nonce", int)
 RPCEndpoint = NewType("RPCEndpoint", str)
 Timestamp = NewType("Timestamp", int)
 Wei = NewType("Wei", int)
+Gwei = NewType("Gwei", int)
 Formatters = Dict[RPCEndpoint, Callable[..., Any]]
 
 
 class AccessListEntry(TypedDict):
     address: HexStr
     storageKeys: Sequence[HexStr]
 
@@ -235,14 +236,25 @@
         "type": Union[int, HexStr],
         "value": Wei,
     },
     total=False,
 )
 
 
+WithdrawalData = TypedDict(
+    "WithdrawalData",
+    {
+        "index": int,
+        "validator_index": int,
+        "address": ChecksumAddress,
+        "amount": Gwei,
+    },
+)
+
+
 CallOverrideParams = TypedDict(
     "CallOverrideParams",
     {
         "balance": Optional[Wei],
         "nonce": Optional[int],
         "code": Optional[Union[bytes, HexStr]],
         "state": Optional[Dict[HexStr, HexStr]],
@@ -351,18 +363,20 @@
     parentHash: HexBytes
     receiptsRoot: HexBytes
     sha3Uncles: HexBytes
     size: int
     stateRoot: HexBytes
     timestamp: Timestamp
     totalDifficulty: int
-    # list of tx hashes or of txdatas
     transactions: Union[Sequence[HexBytes], Sequence[TxData]]
     transactionsRoot: HexBytes
     uncles: Sequence[HexBytes]
+    withdrawals: Sequence[WithdrawalData]
+    withdrawalsRoot: HexBytes
+
     # geth_poa_middleware replaces extraData w/ proofOfAuthorityData
     proofOfAuthorityData: HexBytes
 
 
 class Uncle(TypedDict):
     author: ChecksumAddress
     difficulty: HexStr
```

### Comparing `web3-6.3.0/web3/utils/address.py` & `web3-6.4.0/web3/utils/address.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/utils/async_exception_handling.py` & `web3-6.4.0/web3/utils/async_exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/utils/caching.py` & `web3-6.4.0/web3/utils/caching.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3/utils/exception_handling.py` & `web3-6.4.0/web3/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3.egg-info/PKG-INFO` & `web3-6.4.0/web3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3
-Version: 6.3.0
+Version: 6.4.0
 Summary: web3.py
 Home-page: https://github.com/ethereum/web3.py
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `web3-6.3.0/web3.egg-info/SOURCES.txt` & `web3-6.4.0/web3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `web3-6.3.0/web3.egg-info/requires.txt` & `web3-6.4.0/web3.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 [:platform_system == "Windows"]
 pywin32>=223
 
 [:python_version < "3.8"]
 typing-extensions<5,>=3.7.4.1
 
 [dev]
-eth-tester[py-evm]==v0.8.0-b.3
+eth-tester[py-evm]==v0.9.0-b.1
 py-geth>=3.11.0
 black>=22.1.0
 flake8==3.8.3
 isort>=5.11.0
 mypy==0.910
 types-setuptools>=57.4.4
 types-requests>=2.26.1
 types-protobuf==3.19.13
-sphinx>=5.0.0
+sphinx>=5.3.0
 sphinx_rtd_theme>=1.0.0
 towncrier<22,>=21
 ipfshttpclient==0.8.0a2
 bumpversion
 flaky>=3.7.0
 hypothesis>=3.31.2
 pytest>=7.0.0
@@ -47,15 +47,15 @@
 when-changed>=0.3.0
 build>=0.9.0
 
 [dev:python_version < "3.8"]
 importlib-metadata<5.0
 
 [docs]
-sphinx>=5.0.0
+sphinx>=5.3.0
 sphinx_rtd_theme>=1.0.0
 towncrier<22,>=21
 
 [ipfs]
 ipfshttpclient==0.8.0a2
 
 [linter]
@@ -64,9 +64,9 @@
 isort>=5.11.0
 mypy==0.910
 types-setuptools>=57.4.4
 types-requests>=2.26.1
 types-protobuf==3.19.13
 
 [tester]
-eth-tester[py-evm]==v0.8.0-b.3
+eth-tester[py-evm]==v0.9.0-b.1
 py-geth>=3.11.0
```

