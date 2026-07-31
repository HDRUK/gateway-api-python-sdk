# gateway_api_sdk.DataProviderCollApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**c5bb5300d6a46cc5b1b6a3bb1c3fa869**](DataProviderCollApi.md#c5bb5300d6a46cc5b1b6a3bb1c3fa869) | **PUT** /api/v1/data_provider_colls/{id} | DataProviderColl@update
[**call_02ada355a680c816624e98ae028dc8b6**](DataProviderCollApi.md#call_02ada355a680c816624e98ae028dc8b6) | **POST** /api/v1/data_provider_colls | DataProviderColl@store
[**call_08f75648c437bdf2ba9f66d0c1371d0c**](DataProviderCollApi.md#call_08f75648c437bdf2ba9f66d0c1371d0c) | **GET** /api/v1/data_provider_colls/{id} | DataProviderColl@show
[**call_3351120ae1ae550ab36ee958b1feaf48**](DataProviderCollApi.md#call_3351120ae1ae550ab36ee958b1feaf48) | **DELETE** /api/v1/data_provider_colls/{id} | DataProviderColl@destroy
[**call_81b552b8803870790579d840279ce8a3**](DataProviderCollApi.md#call_81b552b8803870790579d840279ce8a3) | **PATCH** /api/v1/data_provider_colls/{id} | DataProviderColl@edit
[**d0fe0e1c60dd979135440e3e0b440b75**](DataProviderCollApi.md#d0fe0e1c60dd979135440e3e0b440b75) | **GET** /api/v1/data_provider_colls | DataProviderColl@index
[**ed769d8210100bbcd0e3a11660d25dc0**](DataProviderCollApi.md#ed769d8210100bbcd0e3a11660d25dc0) | **GET** /api/v1/data_provider_colls/{id}/summary | DataProviderColl@showSummary


# **c5bb5300d6a46cc5b1b6a3bb1c3fa869**
> C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response c5bb5300d6a46cc5b1b6a3bb1c3fa869(id, c5bb5300d6a46cc5b1b6a3bb1c3fa869_request)

DataProviderColl@update

Update a DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c5bb5300d6a46cc5b1b6a3bb1c3fa869200_response import C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response
from gateway_api_sdk.models.c5bb5300d6a46cc5b1b6a3bb1c3fa869_request import C5bb5300d6a46cc5b1b6a3bb1c3fa869Request
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID
    c5bb5300d6a46cc5b1b6a3bb1c3fa869_request = gateway_api_sdk.C5bb5300d6a46cc5b1b6a3bb1c3fa869Request() # C5bb5300d6a46cc5b1b6a3bb1c3fa869Request | DataProviderColl definition

    try:
        # DataProviderColl@update
        api_response = api_instance.c5bb5300d6a46cc5b1b6a3bb1c3fa869(id, c5bb5300d6a46cc5b1b6a3bb1c3fa869_request)
        print("The response of DataProviderCollApi->c5bb5300d6a46cc5b1b6a3bb1c3fa869:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->c5bb5300d6a46cc5b1b6a3bb1c3fa869: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 
 **c5bb5300d6a46cc5b1b6a3bb1c3fa869_request** | [**C5bb5300d6a46cc5b1b6a3bb1c3fa869Request**](C5bb5300d6a46cc5b1b6a3bb1c3fa869Request.md)| DataProviderColl definition | 

### Return type

[**C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response**](C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_02ada355a680c816624e98ae028dc8b6**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_02ada355a680c816624e98ae028dc8b6(model02ada355a680c816624e98ae028dc8b6_request)

DataProviderColl@store

Creates a new DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model02ada355a680c816624e98ae028dc8b6_request import Model02ada355a680c816624e98ae028dc8b6Request
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    model02ada355a680c816624e98ae028dc8b6_request = gateway_api_sdk.Model02ada355a680c816624e98ae028dc8b6Request() # Model02ada355a680c816624e98ae028dc8b6Request | DataProviderColl definition

    try:
        # DataProviderColl@store
        api_response = api_instance.call_02ada355a680c816624e98ae028dc8b6(model02ada355a680c816624e98ae028dc8b6_request)
        print("The response of DataProviderCollApi->call_02ada355a680c816624e98ae028dc8b6:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->call_02ada355a680c816624e98ae028dc8b6: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model02ada355a680c816624e98ae028dc8b6_request** | [**Model02ada355a680c816624e98ae028dc8b6Request**](Model02ada355a680c816624e98ae028dc8b6Request.md)| DataProviderColl definition | 

### Return type

[**Dd76b8d73b7ea8b4951f03d7c0904c92200Response**](Dd76b8d73b7ea8b4951f03d7c0904c92200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_08f75648c437bdf2ba9f66d0c1371d0c**
> Model08f75648c437bdf2ba9f66d0c1371d0c200Response call_08f75648c437bdf2ba9f66d0c1371d0c(id)

DataProviderColl@show

Return a single DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model08f75648c437bdf2ba9f66d0c1371d0c200_response import Model08f75648c437bdf2ba9f66d0c1371d0c200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID

    try:
        # DataProviderColl@show
        api_response = api_instance.call_08f75648c437bdf2ba9f66d0c1371d0c(id)
        print("The response of DataProviderCollApi->call_08f75648c437bdf2ba9f66d0c1371d0c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->call_08f75648c437bdf2ba9f66d0c1371d0c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 

### Return type

[**Model08f75648c437bdf2ba9f66d0c1371d0c200Response**](Model08f75648c437bdf2ba9f66d0c1371d0c200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_3351120ae1ae550ab36ee958b1feaf48**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_3351120ae1ae550ab36ee958b1feaf48(id)

DataProviderColl@destroy

Delete a DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID

    try:
        # DataProviderColl@destroy
        api_response = api_instance.call_3351120ae1ae550ab36ee958b1feaf48(id)
        print("The response of DataProviderCollApi->call_3351120ae1ae550ab36ee958b1feaf48:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->call_3351120ae1ae550ab36ee958b1feaf48: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_81b552b8803870790579d840279ce8a3**
> C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response call_81b552b8803870790579d840279ce8a3(id, model81b552b8803870790579d840279ce8a3_request)

DataProviderColl@edit

Edit a DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c5bb5300d6a46cc5b1b6a3bb1c3fa869200_response import C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response
from gateway_api_sdk.models.model81b552b8803870790579d840279ce8a3_request import Model81b552b8803870790579d840279ce8a3Request
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID
    model81b552b8803870790579d840279ce8a3_request = gateway_api_sdk.Model81b552b8803870790579d840279ce8a3Request() # Model81b552b8803870790579d840279ce8a3Request | DataProviderColl definition

    try:
        # DataProviderColl@edit
        api_response = api_instance.call_81b552b8803870790579d840279ce8a3(id, model81b552b8803870790579d840279ce8a3_request)
        print("The response of DataProviderCollApi->call_81b552b8803870790579d840279ce8a3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->call_81b552b8803870790579d840279ce8a3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 
 **model81b552b8803870790579d840279ce8a3_request** | [**Model81b552b8803870790579d840279ce8a3Request**](Model81b552b8803870790579d840279ce8a3Request.md)| DataProviderColl definition | 

### Return type

[**C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response**](C5bb5300d6a46cc5b1b6a3bb1c3fa869200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **d0fe0e1c60dd979135440e3e0b440b75**
> D0fe0e1c60dd979135440e3e0b440b75200Response d0fe0e1c60dd979135440e3e0b440b75(per_page=per_page)

DataProviderColl@index

Returns a list of DataProviderColls enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.d0fe0e1c60dd979135440e3e0b440b75200_response import D0fe0e1c60dd979135440e3e0b440b75200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # DataProviderColl@index
        api_response = api_instance.d0fe0e1c60dd979135440e3e0b440b75(per_page=per_page)
        print("The response of DataProviderCollApi->d0fe0e1c60dd979135440e3e0b440b75:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->d0fe0e1c60dd979135440e3e0b440b75: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**D0fe0e1c60dd979135440e3e0b440b75200Response**](D0fe0e1c60dd979135440e3e0b440b75200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **ed769d8210100bbcd0e3a11660d25dc0**
> Ed769d8210100bbcd0e3a11660d25dc0200Response ed769d8210100bbcd0e3a11660d25dc0(id)

DataProviderColl@showSummary

Return a single DataProviderColl - summary

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.ed769d8210100bbcd0e3a11660d25dc0200_response import Ed769d8210100bbcd0e3a11660d25dc0200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = gateway_api_sdk.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID - summary

    try:
        # DataProviderColl@showSummary
        api_response = api_instance.ed769d8210100bbcd0e3a11660d25dc0(id)
        print("The response of DataProviderCollApi->ed769d8210100bbcd0e3a11660d25dc0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->ed769d8210100bbcd0e3a11660d25dc0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID - summary | 

### Return type

[**Ed769d8210100bbcd0e3a11660d25dc0200Response**](Ed769d8210100bbcd0e3a11660d25dc0200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

