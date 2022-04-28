# debank-openapi-client
Build for DeFi Developers.

- API version: 1.0
- Package version: 1.0.0

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on Github, you can install directly from Github

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import openapi_client 
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import openapi_client
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.ChainApi(openapi_client.ApiClient(configuration))

try:
    api_response = api_instance.get_chain_list()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ChainApi->get_chain_list: %s\n" % e)

# create an instance of the API class
api_instance = openapi_client.ChainApi(openapi_client.ApiClient(configuration))
id = 'eth' # str | ChainID

try:
    api_response = api_instance.get_chain_r(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ChainApi->get_chain_r: %s\n" % e)
```

## Documentation for API Endpoints

All URIs are relative to */*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*ChainApi* | [**get_chain_list**](docs/ChainApi.md#get_chain_list) | **GET** /v1/chain/list | 
*ChainApi* | [**get_chain_r**](docs/ChainApi.md#get_chain_r) | **GET** /v1/chain | 
*ProtocolApi* | [**get_protocol_all_list_r**](docs/ProtocolApi.md#get_protocol_all_list_r) | **GET** /v1/protocol/all_list | 
*ProtocolApi* | [**get_protocol_list_r**](docs/ProtocolApi.md#get_protocol_list_r) | **GET** /v1/protocol/contract_addr_list | 
*ProtocolApi* | [**get_protocol_list_r_0**](docs/ProtocolApi.md#get_protocol_list_r_0) | **GET** /v1/protocol/list | 
*ProtocolApi* | [**get_protocol_r**](docs/ProtocolApi.md#get_protocol_r) | **GET** /v1/protocol | 
*TokenApi* | [**get_token_list_by_ids_r**](docs/TokenApi.md#get_token_list_by_ids_r) | **GET** /v1/token/list_by_ids | 
*TokenApi* | [**get_token_r**](docs/TokenApi.md#get_token_r) | **GET** /v1/token | 
*UserApi* | [**get_user_complex_protocol_list**](docs/UserApi.md#get_user_complex_protocol_list) | **GET** /v1/user/all_complex_protocol_list | 
*UserApi* | [**get_user_complex_protocol_list_0**](docs/UserApi.md#get_user_complex_protocol_list_0) | **GET** /v1/user/complex_protocol_list | 
*UserApi* | [**get_user_nft_all_list**](docs/UserApi.md#get_user_nft_all_list) | **GET** /v1/user/all_nft_list | 
*UserApi* | [**get_user_nft_list**](docs/UserApi.md#get_user_nft_list) | **GET** /v1/user/nft_list | 
*UserApi* | [**get_user_protocol**](docs/UserApi.md#get_user_protocol) | **GET** /v1/user/protocol | 
*UserApi* | [**get_user_simple_protocol_list**](docs/UserApi.md#get_user_simple_protocol_list) | **GET** /v1/user/all_simple_protocol_list | 
*UserApi* | [**get_user_simple_protocol_list_0**](docs/UserApi.md#get_user_simple_protocol_list_0) | **GET** /v1/user/simple_protocol_list | 
*UserApi* | [**get_user_token**](docs/UserApi.md#get_user_token) | **GET** /v1/user/token | 
*UserApi* | [**get_user_token_all_list**](docs/UserApi.md#get_user_token_all_list) | **GET** /v1/user/all_token_list | 
*UserApi* | [**get_user_token_authorized_list**](docs/UserApi.md#get_user_token_authorized_list) | **GET** /v1/user/token_authorized_list | 
*UserApi* | [**get_user_token_list**](docs/UserApi.md#get_user_token_list) | **GET** /v1/user/token_list | 
*UserApi* | [**get_user_token_list_0**](docs/UserApi.md#get_user_token_list_0) | **GET** /v1/user/used_chain_list | 
*UserApi* | [**get_user_total_balance**](docs/UserApi.md#get_user_total_balance) | **GET** /v1/user/chain_balance | 
*UserApi* | [**get_user_total_balance_0**](docs/UserApi.md#get_user_total_balance_0) | **GET** /v1/user/total_balance | 
*WalletApi* | [**get_gas_market**](docs/WalletApi.md#get_gas_market) | **GET** /v1/wallet/gas_market | 
*WalletApi* | [**post_balance_change**](docs/WalletApi.md#post_balance_change) | **POST** /v1/wallet/token_balance_change | 
*WalletApi* | [**post_check_tx**](docs/WalletApi.md#post_check_tx) | **POST** /v1/wallet/check_tx | 
*WalletApi* | [**post_estimate_gas**](docs/WalletApi.md#post_estimate_gas) | **POST** /v1/wallet/estimate_gas | 


## Documentation For Models

 - [Chain](docs/Chain.md)
 - [Protocol](docs/Protocol.md)
 - [Token](docs/Token.md)

## Documentation For Authorization

 All endpoints do not require authorization.


## Author


