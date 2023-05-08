# Comparing `tmp/safe-eth-py-suraneti-5.3.2.tar.gz` & `tmp/safe-eth-py-suraneti-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-eth-py-suraneti-5.3.2.tar", last modified: Wed May  3 04:27:46 2023, max compression
+gzip compressed data, was "safe-eth-py-suraneti-5.3.3.tar", last modified: Mon May  8 09:24:41 2023, max compression
```

## Comparing `safe-eth-py-suraneti-5.3.2.tar` & `safe-eth-py-suraneti-5.3.3.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.723920 safe-eth-py-suraneti-5.3.2/
--rw-r--r--   0 suraneti   (501) staff       (20)     1082 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/LICENSE
--rw-r--r--   0 suraneti   (501) staff       (20)       71 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/MANIFEST.in
--rw-r--r--   0 suraneti   (501) staff       (20)     6681 2023-05-03 04:27:46.724067 safe-eth-py-suraneti-5.3.2/PKG-INFO
--rw-r--r--   0 suraneti   (501) staff       (20)     5417 2023-05-03 03:36:31.000000 safe-eth-py-suraneti-5.3.2/README.rst
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.449404 safe-eth-py-suraneti-5.3.2/docs/
--rw-r--r--   0 suraneti   (501) staff       (20)      638 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/Makefile
--rw-r--r--   0 suraneti   (501) staff       (20)      799 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/make.bat
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.492538 safe-eth-py-suraneti-5.3.2/docs/source/
--rw-r--r--   0 suraneti   (501) staff       (20)     1984 2023-02-07 07:15:36.000000 safe-eth-py-suraneti-5.3.2/docs/source/conf.py
--rw-r--r--   0 suraneti   (501) staff       (20)      964 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      183 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      954 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      177 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 suraneti   (501) staff       (20)     1198 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      450 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      936 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      226 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.rst
--rw-r--r--   0 suraneti   (501) staff       (20)     1852 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/gnosis.safe.rst
--rw-r--r--   0 suraneti   (501) staff       (20)      896 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/index.rst
--rw-r--r--   0 suraneti   (501) staff       (20)       55 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/modules.rst
--rw-r--r--   0 suraneti   (501) staff       (20)     8492 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/docs/source/quickstart.rst
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.493461 safe-eth-py-suraneti-5.3.2/gnosis/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.501344 safe-eth-py-suraneti-5.3.2/gnosis/eth/
--rw-r--r--   0 suraneti   (501) staff       (20)     1064 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.503177 safe-eth-py-suraneti-5.3.2/gnosis/eth/abis/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/abis/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    19012 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/abis/multicall.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.506580 safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/
--rw-r--r--   0 suraneti   (501) staff       (20)      657 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4938 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)      194 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6831 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2324 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 suraneti   (501) staff       (20)      625 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/constants.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.553320 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/
--rw-r--r--   0 suraneti   (501) staff       (20)   328664 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 suraneti   (501) staff       (20)    28908 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    26897 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 suraneti   (501) staff       (20)    29068 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 suraneti   (501) staff       (20)    54748 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 suraneti   (501) staff       (20)    89890 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 suraneti   (501) staff       (20)   622260 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 suraneti   (501) staff       (20)   983403 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)  1158944 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)  1347363 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)   119875 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    19886 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 suraneti   (501) staff       (20)    78793 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 suraneti   (501) staff       (20)   136946 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)   288861 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)    18975 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    32495 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)    39032 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 suraneti   (501) staff       (20)     1862 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 suraneti   (501) staff       (20)     6967 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7351 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 suraneti   (501) staff       (20)    17165 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 suraneti   (501) staff       (20)     2480 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 suraneti   (501) staff       (20)     2242 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 suraneti   (501) staff       (20)     8293 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 suraneti   (501) staff       (20)    11889 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.557350 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1501 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/admin.py
--rw-r--r--   0 suraneti   (501) staff       (20)      269 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/filters.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2400 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/forms.py
--rw-r--r--   0 suraneti   (501) staff       (20)     8445 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/models.py
--rw-r--r--   0 suraneti   (501) staff       (20)     5740 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.561445 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)      547 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/models.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3013 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7414 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6203 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 suraneti   (501) staff       (20)      508 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 suraneti   (501) staff       (20)      320 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/django/validators.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.562229 safe-eth-py-suraneti-5.3.2/gnosis/eth/eip712/
--rw-r--r--   0 suraneti   (501) staff       (20)     6538 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    77421 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/ethereum_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)    20913 2023-05-03 04:25:18.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/ethereum_network.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1104 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/exceptions.py
--rw-r--r--   0 suraneti   (501) staff       (20)    13603 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/multicall.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.570758 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/
--rw-r--r--   0 suraneti   (501) staff       (20)     1093 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.578224 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    15986 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    30036 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    29731 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    27567 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    25872 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)      239 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)    45208 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 suraneti   (501) staff       (20)    36257 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1464 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2398 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)      161 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.579152 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/helpers/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     5856 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4194 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 suraneti   (501) staff       (20)    32144 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1677 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1520 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7154 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1064 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.585552 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.590060 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)   107062 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1047 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1246 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1357 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.591099 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/eip712/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    13315 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2725 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.599315 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    31306 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12057 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 suraneti   (501) staff       (20)   793149 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 suraneti   (501) staff       (20)    92795 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 suraneti   (501) staff       (20)   171076 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.622225 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2706 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1820 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1460 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2043 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3461 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 suraneti   (501) staff       (20)    61046 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7087 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 suraneti   (501) staff       (20)    21070 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 suraneti   (501) staff       (20)     7380 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4474 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/utils.py
--rw-r--r--   0 suraneti   (501) staff       (20)      281 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/typing.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6399 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/eth/utils.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.627436 safe-eth-py-suraneti-5.3.2/gnosis/protocol/
--rw-r--r--   0 suraneti   (501) staff       (20)      177 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/protocol/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     8642 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2695 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/protocol/order.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.672183 safe-eth-py-suraneti-5.3.2/gnosis/protocol/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     5926 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/py.typed
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.702666 safe-eth-py-suraneti-5.3.2/gnosis/safe/
--rw-r--r--   0 suraneti   (501) staff       (20)      716 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)    24703 2023-05-03 03:54:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/addresses.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.706614 safe-eth-py-suraneti-5.3.2/gnosis/safe/api/
--rw-r--r--   0 suraneti   (501) staff       (20)      346 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/api/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1917 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/api/base_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3062 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     9262 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1451 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/exceptions.py
--rw-r--r--   0 suraneti   (501) staff       (20)    11385 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/multi_send.py
--rw-r--r--   0 suraneti   (501) staff       (20)     8070 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/proxy_factory.py
--rw-r--r--   0 suraneti   (501) staff       (20)    41997 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/safe.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12116 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12982 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)     9885 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_signature.py
--rw-r--r--   0 suraneti   (501) staff       (20)    16881 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4181 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/serializers.py
--rw-r--r--   0 suraneti   (501) staff       (20)     2039 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/signatures.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.716912 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.718972 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/api/
--rw-r--r--   0 suraneti   (501) staff       (20)        0 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)     4989 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 suraneti   (501) staff       (20)    10808 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 suraneti   (501) staff       (20)    10515 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 suraneti   (501) staff       (20)     6448 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 suraneti   (501) staff       (20)    32608 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 suraneti   (501) staff       (20)    16628 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)    16965 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)    14117 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 suraneti   (501) staff       (20)    12928 2023-05-03 02:51:41.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3762 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 suraneti   (501) staff       (20)     3701 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 suraneti   (501) staff       (20)     1967 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.720242 safe-eth-py-suraneti-5.3.2/gnosis/util/
--rw-r--r--   0 suraneti   (501) staff       (20)       83 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/util/__init__.py
--rw-r--r--   0 suraneti   (501) staff       (20)      442 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/gnosis/util/util.py
-drwxr-xr-x   0 suraneti   (501) staff       (20)        0 2023-05-03 04:27:46.723559 safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/
--rw-r--r--   0 suraneti   (501) staff       (20)     6681 2023-05-03 04:27:46.000000 safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/PKG-INFO
--rw-r--r--   0 suraneti   (501) staff       (20)     5696 2023-05-03 04:27:46.000000 safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/SOURCES.txt
--rw-r--r--   0 suraneti   (501) staff       (20)        1 2023-05-03 04:27:46.000000 safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/dependency_links.txt
--rw-r--r--   0 suraneti   (501) staff       (20)      219 2023-05-03 04:27:46.000000 safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/requires.txt
--rw-r--r--   0 suraneti   (501) staff       (20)        7 2023-05-03 04:27:46.000000 safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/top_level.txt
--rw-r--r--   0 suraneti   (501) staff       (20)     2523 2023-05-03 04:27:46.727220 safe-eth-py-suraneti-5.3.2/setup.cfg
--rw-r--r--   0 suraneti   (501) staff       (20)       69 2023-02-03 11:50:27.000000 safe-eth-py-suraneti-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.901666 safe-eth-py-suraneti-5.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-08 09:24:41.901666 safe-eth-py-suraneti-5.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.873667 safe-eth-py-suraneti-5.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.877667 safe-eth-py-suraneti-5.3.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.877667 safe-eth-py-suraneti-5.3.3/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.877667 safe-eth-py-suraneti-5.3.3/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.877667 safe-eth-py-suraneti-5.3.3/gnosis/eth/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/abis/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.877667 safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.885667 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.885667 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.889667 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.889667 safe-eth-py-suraneti-5.3.3/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77421 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.889667 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.889667 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.889667 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.889667 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.893667 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.893667 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.893667 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.893667 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.893667 safe-eth-py-suraneti-5.3.3/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.893667 safe-eth-py-suraneti-5.3.3/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.897667 safe-eth-py-suraneti-5.3.3/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24703 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.897667 safe-eth-py-suraneti-5.3.3/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41997 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.897667 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.897667 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.897667 safe-eth-py-suraneti-5.3.3/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:24:41.901666 safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-05-08 09:24:41.000000 safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-08 09:24:41.000000 safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:24:41.000000 safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-08 09:24:41.000000 safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 09:24:41.000000 safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-08 09:24:41.901666 safe-eth-py-suraneti-5.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 09:24:27.000000 safe-eth-py-suraneti-5.3.3/setup.py
```

### Comparing `safe-eth-py-suraneti-5.3.2/LICENSE` & `safe-eth-py-suraneti-5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/PKG-INFO` & `safe-eth-py-suraneti-5.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py-suraneti
-Version: 5.3.2
+Version: 5.3.3
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-suraneti-5.3.2/README.rst` & `safe-eth-py-suraneti-5.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/Makefile` & `safe-eth-py-suraneti-5.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/make.bat` & `safe-eth-py-suraneti-5.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/conf.py` & `safe-eth-py-suraneti-5.3.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.clients.rst` & `safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.django.rst` & `safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.oracles.abis.rst` & `safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/gnosis.eth.rst` & `safe-eth-py-suraneti-5.3.3/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/gnosis.safe.rst` & `safe-eth-py-suraneti-5.3.3/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/index.rst` & `safe-eth-py-suraneti-5.3.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/docs/source/quickstart.rst` & `safe-eth-py-suraneti-5.3.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/__init__.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/abis/multicall.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/__init__.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/blockscout_client.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/etherscan_client.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/clients/sourcify.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/clients/sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/constants.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/CPKFactory.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/DelegateConstructorProxy.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC1155.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC20.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC20TestToken.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ERC721.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/MultiSend.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/PayingProxy.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/Proxy_V1_0_0.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/Proxy_V1_1_1.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/Proxy_V1_3_0.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/__init__.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/kyber_network_proxy.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_exchange.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_factory.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_v2_factory.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_v2_pair.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/contracts/uniswap_v2_router.json` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/admin.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/forms.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/models.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/serializers.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/models.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/test_forms.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/test_models.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/django/tests/test_serializers.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/eip712/__init__.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/ethereum_client.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/ethereum_network.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/exceptions.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/multicall.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/__init__.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/aave_abis.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/balancer_abis.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/cream_abis.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/curve_abis.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/mooniswap_abis.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/uniswap_v3.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/yearn_abis.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/abis/zerion_abis.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/cowswap.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/kyber.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/oracles.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/superfluid.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/sushiswap.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/uniswap_v3.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/oracles/utils.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/mocks.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/test_blockscout_client.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/test_etherscan_client.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/clients/test_sourcify.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/eip712/test_eip712.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/ethereum_test_case.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_internal_txs.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_log_receipts.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_trace_block.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_trace_filter.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_cowswap.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_kyber.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_superfluid.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_sushiswap.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_ethereum_client.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_multicall.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_oracles.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/test_utils.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/tests/utils.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/eth/utils.py` & `safe-eth-py-suraneti-5.3.3/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/protocol/gnosis_protocol_api.py` & `safe-eth-py-suraneti-5.3.3/gnosis/protocol/gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/protocol/order.py` & `safe-eth-py-suraneti-5.3.3/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `safe-eth-py-suraneti-5.3.3/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/__init__.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/addresses.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/addresses.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/api/base_api.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/api/relay_service_api.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/api/relay_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/api/transaction_service_api.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/exceptions.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/multi_send.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/proxy_factory.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/safe.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_create2_tx.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_creation_tx.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_signature.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/safe_tx.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/serializers.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/signatures.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/api/test_transaction_service_api.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/safe_test_case.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_multi_send.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_proxy_factory.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_create2_tx.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_creation_tx.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_signature.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_safe_tx.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_serializers.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/test_signatures.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/gnosis/safe/tests/utils.py` & `safe-eth-py-suraneti-5.3.3/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/PKG-INFO` & `safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py-suraneti
-Version: 5.3.2
+Version: 5.3.3
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-suraneti-5.3.2/safe_eth_py_suraneti.egg-info/SOURCES.txt` & `safe-eth-py-suraneti-5.3.3/safe_eth_py_suraneti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe-eth-py-suraneti-5.3.2/setup.cfg` & `safe-eth-py-suraneti-5.3.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = safe-eth-py-suraneti
-version = 5.3.2
+version = 5.3.3
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

