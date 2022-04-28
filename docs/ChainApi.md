# openapi_client.ChainApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_chain_list**](ChainApi.md#get_chain_list) | **GET** /v1/chain/list | 
[**get_chain_r**](ChainApi.md#get_chain_r) | **GET** /v1/chain | 

# **get_chain_list**
> list[Chain] get_chain_list()



Get supported chain list

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.ChainApi()

try:
    api_response = api_instance.get_chain_list()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ChainApi->get_chain_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Chain]**](Chain.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_chain_r**
> Chain get_chain_r(id)



Get chain info by id

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.ChainApi()
id = 'id_example' # str | ChainID

try:
    api_response = api_instance.get_chain_r(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ChainApi->get_chain_r: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| ChainID | 

### Return type

[**Chain**](Chain.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

