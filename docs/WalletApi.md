# openapi_client.WalletApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_gas_market**](WalletApi.md#get_gas_market) | **GET** /v1/wallet/gas_market | 
[**post_balance_change**](WalletApi.md#post_balance_change) | **POST** /v1/wallet/token_balance_change | 
[**post_check_tx**](WalletApi.md#post_check_tx) | **POST** /v1/wallet/check_tx | 
[**post_estimate_gas**](WalletApi.md#post_estimate_gas) | **POST** /v1/wallet/estimate_gas | 

# **get_gas_market**
> get_gas_market(chain_id, custom_price=custom_price)



gas market

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.WalletApi()
chain_id = 'chain_id_example' # str | ChainId
custom_price = '0' # str | CustomPrice (optional) (default to 0)

try:
    api_instance.get_gas_market(chain_id, custom_price=custom_price)
except ApiException as e:
    print("Exception when calling WalletApi->get_gas_market: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **chain_id** | **str**| ChainId | 
 **custom_price** | **str**| CustomPrice | [optional] [default to 0]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_balance_change**
> post_balance_change()



token balance change

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.WalletApi()

try:
    api_instance.post_balance_change()
except ApiException as e:
    print("Exception when calling WalletApi->post_balance_change: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_check_tx**
> post_check_tx()



check tx

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.WalletApi()

try:
    api_instance.post_check_tx()
except ApiException as e:
    print("Exception when calling WalletApi->post_check_tx: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_estimate_gas**
> post_estimate_gas()



### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.WalletApi()

try:
    api_instance.post_estimate_gas()
except ApiException as e:
    print("Exception when calling WalletApi->post_estimate_gas: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

