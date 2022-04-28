# openapi_client.TokenApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_token_list_by_ids_r**](TokenApi.md#get_token_list_by_ids_r) | **GET** /v1/token/list_by_ids | 
[**get_token_r**](TokenApi.md#get_token_r) | **GET** /v1/token | 

# **get_token_list_by_ids_r**
> list[Token] get_token_list_by_ids_r(chain_id, ids)



Bulk token fetching by address

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.TokenApi()
chain_id = 'chain_id_example' # str | ChainID
ids = ['ids_example'] # list[str] | List of token addresses, up to 100

try:
    api_response = api_instance.get_token_list_by_ids_r(chain_id, ids)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TokenApi->get_token_list_by_ids_r: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **chain_id** | **str**| ChainID | 
 **ids** | [**list[str]**](str.md)| List of token addresses, up to 100 | 

### Return type

[**list[Token]**](Token.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_token_r**
> Token get_token_r(chain_id, id)



Get token by address

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.TokenApi()
chain_id = 'chain_id_example' # str | ChainID
id = 'id_example' # str | Ethereum Address or native token id

try:
    api_response = api_instance.get_token_r(chain_id, id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling TokenApi->get_token_r: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **chain_id** | **str**| ChainID | 
 **id** | **str**| Ethereum Address or native token id | 

### Return type

[**Token**](Token.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

