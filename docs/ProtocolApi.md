# openapi_client.ProtocolApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_protocol_all_list_r**](ProtocolApi.md#get_protocol_all_list_r) | **GET** /v1/protocol/all_list | 
[**get_protocol_list_r**](ProtocolApi.md#get_protocol_list_r) | **GET** /v1/protocol/contract_addr_list | 
[**get_protocol_list_r_0**](ProtocolApi.md#get_protocol_list_r_0) | **GET** /v1/protocol/list | 
[**get_protocol_r**](ProtocolApi.md#get_protocol_r) | **GET** /v1/protocol | 

# **get_protocol_all_list_r**
> list[Protocol] get_protocol_all_list_r()



### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.ProtocolApi()

try:
    api_response = api_instance.get_protocol_all_list_r()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ProtocolApi->get_protocol_all_list_r: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Protocol]**](Protocol.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_protocol_list_r**
> get_protocol_list_r()



### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.ProtocolApi()

try:
    api_instance.get_protocol_list_r()
except ApiException as e:
    print("Exception when calling ProtocolApi->get_protocol_list_r: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_protocol_list_r_0**
> list[Protocol] get_protocol_list_r_0()



### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.ProtocolApi()

try:
    api_response = api_instance.get_protocol_list_r_0()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ProtocolApi->get_protocol_list_r_0: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Protocol]**](Protocol.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_protocol_r**
> Protocol get_protocol_r(id)



### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.ProtocolApi()
id = 'id_example' # str | protocol id

try:
    api_response = api_instance.get_protocol_r(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ProtocolApi->get_protocol_r: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| protocol id | 

### Return type

[**Protocol**](Protocol.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

