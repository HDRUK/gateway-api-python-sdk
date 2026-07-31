# gateway_api_sdk.CategoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**a5f6e0a9550d3c58c50dda55412cd051**](CategoryApi.md#a5f6e0a9550d3c58c50dda55412cd051) | **PATCH** /api/v1/categories/{id} | Category@update
[**call_37196d259228d2274dd9dbef8b00e547**](CategoryApi.md#call_37196d259228d2274dd9dbef8b00e547) | **DELETE** /api/v1/categories/{id} | Category@destroy
[**call_988e8695bc991d7f8e40131db5ba7a76**](CategoryApi.md#call_988e8695bc991d7f8e40131db5ba7a76) | **PUT** /api/v1/categories/{id} | Category@update
[**call_9c4934d1b68a6d4440ec72cfc8ae7074**](CategoryApi.md#call_9c4934d1b68a6d4440ec72cfc8ae7074) | **GET** /api/v1/categories/{id} | Category@show
[**dd76b8d73b7ea8b4951f03d7c0904c92**](CategoryApi.md#dd76b8d73b7ea8b4951f03d7c0904c92) | **POST** /api/v1/categories | Category@store
[**e225c2b7eb5daf7fb16e00f4f07ff030**](CategoryApi.md#e225c2b7eb5daf7fb16e00f4f07ff030) | **GET** /api/v1/categories | Category@index


# **a5f6e0a9550d3c58c50dda55412cd051**
> Model988e8695bc991d7f8e40131db5ba7a76200Response a5f6e0a9550d3c58c50dda55412cd051(id, a5f6e0a9550d3c58c50dda55412cd051_request)

Category@update

Edit a tool category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a5f6e0a9550d3c58c50dda55412cd051_request import A5f6e0a9550d3c58c50dda55412cd051Request
from gateway_api_sdk.models.model988e8695bc991d7f8e40131db5ba7a76200_response import Model988e8695bc991d7f8e40131db5ba7a76200Response
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id
    a5f6e0a9550d3c58c50dda55412cd051_request = gateway_api_sdk.A5f6e0a9550d3c58c50dda55412cd051Request() # A5f6e0a9550d3c58c50dda55412cd051Request | Category definition

    try:
        # Category@update
        api_response = api_instance.a5f6e0a9550d3c58c50dda55412cd051(id, a5f6e0a9550d3c58c50dda55412cd051_request)
        print("The response of CategoryApi->a5f6e0a9550d3c58c50dda55412cd051:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->a5f6e0a9550d3c58c50dda55412cd051: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 
 **a5f6e0a9550d3c58c50dda55412cd051_request** | [**A5f6e0a9550d3c58c50dda55412cd051Request**](A5f6e0a9550d3c58c50dda55412cd051Request.md)| Category definition | 

### Return type

[**Model988e8695bc991d7f8e40131db5ba7a76200Response**](Model988e8695bc991d7f8e40131db5ba7a76200Response.md)

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

# **call_37196d259228d2274dd9dbef8b00e547**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_37196d259228d2274dd9dbef8b00e547(id)

Category@destroy

Delete a tool category

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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id

    try:
        # Category@destroy
        api_response = api_instance.call_37196d259228d2274dd9dbef8b00e547(id)
        print("The response of CategoryApi->call_37196d259228d2274dd9dbef8b00e547:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->call_37196d259228d2274dd9dbef8b00e547: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 

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

# **call_988e8695bc991d7f8e40131db5ba7a76**
> Model988e8695bc991d7f8e40131db5ba7a76200Response call_988e8695bc991d7f8e40131db5ba7a76(id, model988e8695bc991d7f8e40131db5ba7a76_request)

Category@update

Update a tool category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model988e8695bc991d7f8e40131db5ba7a76200_response import Model988e8695bc991d7f8e40131db5ba7a76200Response
from gateway_api_sdk.models.model988e8695bc991d7f8e40131db5ba7a76_request import Model988e8695bc991d7f8e40131db5ba7a76Request
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id
    model988e8695bc991d7f8e40131db5ba7a76_request = gateway_api_sdk.Model988e8695bc991d7f8e40131db5ba7a76Request() # Model988e8695bc991d7f8e40131db5ba7a76Request | Category definition

    try:
        # Category@update
        api_response = api_instance.call_988e8695bc991d7f8e40131db5ba7a76(id, model988e8695bc991d7f8e40131db5ba7a76_request)
        print("The response of CategoryApi->call_988e8695bc991d7f8e40131db5ba7a76:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->call_988e8695bc991d7f8e40131db5ba7a76: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 
 **model988e8695bc991d7f8e40131db5ba7a76_request** | [**Model988e8695bc991d7f8e40131db5ba7a76Request**](Model988e8695bc991d7f8e40131db5ba7a76Request.md)| Category definition | 

### Return type

[**Model988e8695bc991d7f8e40131db5ba7a76200Response**](Model988e8695bc991d7f8e40131db5ba7a76200Response.md)

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

# **call_9c4934d1b68a6d4440ec72cfc8ae7074**
> E225c2b7eb5daf7fb16e00f4f07ff030200Response call_9c4934d1b68a6d4440ec72cfc8ae7074(id)

Category@show

Return a single tool category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.e225c2b7eb5daf7fb16e00f4f07ff030200_response import E225c2b7eb5daf7fb16e00f4f07ff030200Response
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id

    try:
        # Category@show
        api_response = api_instance.call_9c4934d1b68a6d4440ec72cfc8ae7074(id)
        print("The response of CategoryApi->call_9c4934d1b68a6d4440ec72cfc8ae7074:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->call_9c4934d1b68a6d4440ec72cfc8ae7074: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 

### Return type

[**E225c2b7eb5daf7fb16e00f4f07ff030200Response**](E225c2b7eb5daf7fb16e00f4f07ff030200Response.md)

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

# **dd76b8d73b7ea8b4951f03d7c0904c92**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response dd76b8d73b7ea8b4951f03d7c0904c92(dd76b8d73b7ea8b4951f03d7c0904c92_request)

Category@store

Creates a new tool category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92_request import Dd76b8d73b7ea8b4951f03d7c0904c92Request
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    dd76b8d73b7ea8b4951f03d7c0904c92_request = gateway_api_sdk.Dd76b8d73b7ea8b4951f03d7c0904c92Request() # Dd76b8d73b7ea8b4951f03d7c0904c92Request | Category definition

    try:
        # Category@store
        api_response = api_instance.dd76b8d73b7ea8b4951f03d7c0904c92(dd76b8d73b7ea8b4951f03d7c0904c92_request)
        print("The response of CategoryApi->dd76b8d73b7ea8b4951f03d7c0904c92:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->dd76b8d73b7ea8b4951f03d7c0904c92: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dd76b8d73b7ea8b4951f03d7c0904c92_request** | [**Dd76b8d73b7ea8b4951f03d7c0904c92Request**](Dd76b8d73b7ea8b4951f03d7c0904c92Request.md)| Category definition | 

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

# **e225c2b7eb5daf7fb16e00f4f07ff030**
> E225c2b7eb5daf7fb16e00f4f07ff030200Response e225c2b7eb5daf7fb16e00f4f07ff030(per_page=per_page)

Category@index

Returns a list of categories enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.e225c2b7eb5daf7fb16e00f4f07ff030200_response import E225c2b7eb5daf7fb16e00f4f07ff030200Response
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # Category@index
        api_response = api_instance.e225c2b7eb5daf7fb16e00f4f07ff030(per_page=per_page)
        print("The response of CategoryApi->e225c2b7eb5daf7fb16e00f4f07ff030:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->e225c2b7eb5daf7fb16e00f4f07ff030: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**E225c2b7eb5daf7fb16e00f4f07ff030200Response**](E225c2b7eb5daf7fb16e00f4f07ff030200Response.md)

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

