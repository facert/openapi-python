# openapi_client.UserApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_user_complex_protocol_list**](UserApi.md#get_user_complex_protocol_list) | **GET** /v1/user/all_complex_protocol_list | 
[**get_user_complex_protocol_list_0**](UserApi.md#get_user_complex_protocol_list_0) | **GET** /v1/user/complex_protocol_list | 
[**get_user_nft_all_list**](UserApi.md#get_user_nft_all_list) | **GET** /v1/user/all_nft_list | 
[**get_user_nft_list**](UserApi.md#get_user_nft_list) | **GET** /v1/user/nft_list | 
[**get_user_protocol**](UserApi.md#get_user_protocol) | **GET** /v1/user/protocol | 
[**get_user_simple_protocol_list**](UserApi.md#get_user_simple_protocol_list) | **GET** /v1/user/all_simple_protocol_list | 
[**get_user_simple_protocol_list_0**](UserApi.md#get_user_simple_protocol_list_0) | **GET** /v1/user/simple_protocol_list | 
[**get_user_token**](UserApi.md#get_user_token) | **GET** /v1/user/token | 
[**get_user_token_all_list**](UserApi.md#get_user_token_all_list) | **GET** /v1/user/all_token_list | 
[**get_user_token_authorized_list**](UserApi.md#get_user_token_authorized_list) | **GET** /v1/user/token_authorized_list | 
[**get_user_token_list**](UserApi.md#get_user_token_list) | **GET** /v1/user/token_list | 
[**get_user_token_list_0**](UserApi.md#get_user_token_list_0) | **GET** /v1/user/used_chain_list | 
[**get_user_total_balance**](UserApi.md#get_user_total_balance) | **GET** /v1/user/chain_balance | 
[**get_user_total_balance_0**](UserApi.md#get_user_total_balance_0) | **GET** /v1/user/total_balance | 

# **get_user_complex_protocol_list**
> get_user_complex_protocol_list(id)



Get list of protocols with user portfolio details on all supported chains

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address

try:
    api_instance.get_user_complex_protocol_list(id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_complex_protocol_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_complex_protocol_list_0**
> get_user_complex_protocol_list_0(id, chain_id=chain_id)



Get list of protocols with user portfolio details on a chain

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address
chain_id = 'chain_id_example' # str | ChainID (optional)

try:
    api_instance.get_user_complex_protocol_list_0(id, chain_id=chain_id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_complex_protocol_list_0: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 
 **chain_id** | **str**| ChainID | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_nft_all_list**
> get_user_nft_all_list(id, is_all=is_all)



Get user nft list on all supported chains

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | Address
is_all = true # bool | If true, all tokens are returned (optional) (default to true)

try:
    api_instance.get_user_nft_all_list(id, is_all=is_all)
except ApiException as e:
    print("Exception when calling UserApi->get_user_nft_all_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Address | 
 **is_all** | **bool**| If true, all tokens are returned | [optional] [default to true]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_nft_list**
> get_user_nft_list(id, chain_id, is_all=is_all)



Get user nft list

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | Address
chain_id = 'chain_id_example' # str | ChainID
is_all = true # bool | If true, all tokens are returned (optional) (default to true)

try:
    api_instance.get_user_nft_list(id, chain_id, is_all=is_all)
except ApiException as e:
    print("Exception when calling UserApi->get_user_nft_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Address | 
 **chain_id** | **str**| ChainID | 
 **is_all** | **bool**| If true, all tokens are returned | [optional] [default to true]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_protocol**
> get_user_protocol(id, protocol_id)



Get the user's portfolio in the protocol

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address
protocol_id = 'protocol_id_example' # str | protocol id

try:
    api_instance.get_user_protocol(id, protocol_id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_protocol: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 
 **protocol_id** | **str**| protocol id | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_simple_protocol_list**
> get_user_simple_protocol_list(id)



Stats the user's protocol assets on all supported chains

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address

try:
    api_instance.get_user_simple_protocol_list(id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_simple_protocol_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_simple_protocol_list_0**
> get_user_simple_protocol_list_0(id, chain_id)



Stats the user's protocol assets on a chain

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address
chain_id = 'chain_id_example' # str | ChainID

try:
    api_instance.get_user_simple_protocol_list_0(id, chain_id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_simple_protocol_list_0: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 
 **chain_id** | **str**| ChainID | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_token**
> get_user_token(id, chain_id, token_id)



Get user token balance

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | Address
chain_id = 'chain_id_example' # str | ChainID
token_id = 'token_id_example' # str | token id

try:
    api_instance.get_user_token(id, chain_id, token_id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_token: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Address | 
 **chain_id** | **str**| ChainID | 
 **token_id** | **str**| token id | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_token_all_list**
> get_user_token_all_list(id, is_all=is_all)



Get user token balance

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | Address
is_all = true # bool | If true, all tokens are returned, including protocol-derived tokens (optional) (default to true)

try:
    api_instance.get_user_token_all_list(id, is_all=is_all)
except ApiException as e:
    print("Exception when calling UserApi->get_user_token_all_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Address | 
 **is_all** | **bool**| If true, all tokens are returned, including protocol-derived tokens | [optional] [default to true]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_token_authorized_list**
> get_user_token_authorized_list(id, chain_id)



Show the user's risk exposure of approved token on a chain

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address
chain_id = 'chain_id_example' # str | ChainID

try:
    api_instance.get_user_token_authorized_list(id, chain_id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_token_authorized_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 
 **chain_id** | **str**| ChainID | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_token_list**
> get_user_token_list(id, chain_id, is_all=is_all)



Get user token balance

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | Address
chain_id = 'chain_id_example' # str | ChainID
is_all = true # bool | If true, all tokens are returned, including protocol-derived tokens (optional) (default to true)

try:
    api_instance.get_user_token_list(id, chain_id, is_all=is_all)
except ApiException as e:
    print("Exception when calling UserApi->get_user_token_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Address | 
 **chain_id** | **str**| ChainID | 
 **is_all** | **bool**| If true, all tokens are returned, including protocol-derived tokens | [optional] [default to true]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_token_list_0**
> get_user_token_list_0(id)



Get user chain list

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | Address

try:
    api_instance.get_user_token_list_0(id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_token_list_0: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Address | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_total_balance**
> get_user_total_balance(id, chain_id)



Get the net assets of a chain

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address
chain_id = 'chain_id_example' # str | ChainID

try:
    api_instance.get_user_total_balance(id, chain_id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_total_balance: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 
 **chain_id** | **str**| ChainID | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_total_balance_0**
> get_user_total_balance_0(id)



Get net assets on multiple chains, including tokens and protocols

### Example
```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openapi_client.UserApi()
id = 'id_example' # str | User Address

try:
    api_instance.get_user_total_balance_0(id)
except ApiException as e:
    print("Exception when calling UserApi->get_user_total_balance_0: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| User Address | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

