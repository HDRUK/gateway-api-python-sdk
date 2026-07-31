# gateway_api_sdk.ProgrammingPackageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ad25f9129aefd55435b425747d5a706c**](ProgrammingPackageApi.md#ad25f9129aefd55435b425747d5a706c) | **POST** /api/v1/programming_packages | ProgrammingPackage@store
[**call_1aeebba947bfb42f364a2d5dd2ad8ef9**](ProgrammingPackageApi.md#call_1aeebba947bfb42f364a2d5dd2ad8ef9) | **PUT** /api/v1/programming_packages/{id} | ProgrammingPackage@update
[**call_47ebee1d2e096dcb033d29f4ff244ad4**](ProgrammingPackageApi.md#call_47ebee1d2e096dcb033d29f4ff244ad4) | **GET** /api/v1/programming_packages/{id} | ProgrammingPackage@show
[**call_6ac98caeb87a37c9286f592834b9c803**](ProgrammingPackageApi.md#call_6ac98caeb87a37c9286f592834b9c803) | **GET** /api/v1/programming_packages | ProgrammingPackage@index
[**call_879046026ce3997dea0d9bf768f2f8e6**](ProgrammingPackageApi.md#call_879046026ce3997dea0d9bf768f2f8e6) | **PATCH** /api/v1/programming_packages/{id} | ProgrammingPackage@update
[**fdbe7e1aad9b02084b06c6d647766efd**](ProgrammingPackageApi.md#fdbe7e1aad9b02084b06c6d647766efd) | **DELETE** /api/v1/programming_packages/{id} | ProgrammingPackage@destroy


# **ad25f9129aefd55435b425747d5a706c**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response ad25f9129aefd55435b425747d5a706c(dd76b8d73b7ea8b4951f03d7c0904c92_request)

ProgrammingPackage@store

Creates a new system programming package

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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    dd76b8d73b7ea8b4951f03d7c0904c92_request = gateway_api_sdk.Dd76b8d73b7ea8b4951f03d7c0904c92Request() # Dd76b8d73b7ea8b4951f03d7c0904c92Request | Programming package definition

    try:
        # ProgrammingPackage@store
        api_response = api_instance.ad25f9129aefd55435b425747d5a706c(dd76b8d73b7ea8b4951f03d7c0904c92_request)
        print("The response of ProgrammingPackageApi->ad25f9129aefd55435b425747d5a706c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->ad25f9129aefd55435b425747d5a706c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dd76b8d73b7ea8b4951f03d7c0904c92_request** | [**Dd76b8d73b7ea8b4951f03d7c0904c92Request**](Dd76b8d73b7ea8b4951f03d7c0904c92Request.md)| Programming package definition | 

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

# **call_1aeebba947bfb42f364a2d5dd2ad8ef9**
> Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response call_1aeebba947bfb42f364a2d5dd2ad8ef9(id, model988e8695bc991d7f8e40131db5ba7a76_request)

ProgrammingPackage@update

Update a system programming package

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model1aeebba947bfb42f364a2d5dd2ad8ef9200_response import Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id
    model988e8695bc991d7f8e40131db5ba7a76_request = gateway_api_sdk.Model988e8695bc991d7f8e40131db5ba7a76Request() # Model988e8695bc991d7f8e40131db5ba7a76Request | ProgrammingPackage definition

    try:
        # ProgrammingPackage@update
        api_response = api_instance.call_1aeebba947bfb42f364a2d5dd2ad8ef9(id, model988e8695bc991d7f8e40131db5ba7a76_request)
        print("The response of ProgrammingPackageApi->call_1aeebba947bfb42f364a2d5dd2ad8ef9:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->call_1aeebba947bfb42f364a2d5dd2ad8ef9: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 
 **model988e8695bc991d7f8e40131db5ba7a76_request** | [**Model988e8695bc991d7f8e40131db5ba7a76Request**](Model988e8695bc991d7f8e40131db5ba7a76Request.md)| ProgrammingPackage definition | 

### Return type

[**Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response**](Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response.md)

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

# **call_47ebee1d2e096dcb033d29f4ff244ad4**
> Model47ebee1d2e096dcb033d29f4ff244ad4200Response call_47ebee1d2e096dcb033d29f4ff244ad4(id)

ProgrammingPackage@show

Return a single system programming package

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model47ebee1d2e096dcb033d29f4ff244ad4200_response import Model47ebee1d2e096dcb033d29f4ff244ad4200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id

    try:
        # ProgrammingPackage@show
        api_response = api_instance.call_47ebee1d2e096dcb033d29f4ff244ad4(id)
        print("The response of ProgrammingPackageApi->call_47ebee1d2e096dcb033d29f4ff244ad4:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->call_47ebee1d2e096dcb033d29f4ff244ad4: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 

### Return type

[**Model47ebee1d2e096dcb033d29f4ff244ad4200Response**](Model47ebee1d2e096dcb033d29f4ff244ad4200Response.md)

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

# **call_6ac98caeb87a37c9286f592834b9c803**
> Model6ac98caeb87a37c9286f592834b9c803200Response call_6ac98caeb87a37c9286f592834b9c803()

ProgrammingPackage@index

Returns a list of programming packages enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model6ac98caeb87a37c9286f592834b9c803200_response import Model6ac98caeb87a37c9286f592834b9c803200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)

    try:
        # ProgrammingPackage@index
        api_response = api_instance.call_6ac98caeb87a37c9286f592834b9c803()
        print("The response of ProgrammingPackageApi->call_6ac98caeb87a37c9286f592834b9c803:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->call_6ac98caeb87a37c9286f592834b9c803: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Model6ac98caeb87a37c9286f592834b9c803200Response**](Model6ac98caeb87a37c9286f592834b9c803200Response.md)

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

# **call_879046026ce3997dea0d9bf768f2f8e6**
> Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response call_879046026ce3997dea0d9bf768f2f8e6(id, a5f6e0a9550d3c58c50dda55412cd051_request)

ProgrammingPackage@update

Edit a system programming package

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a5f6e0a9550d3c58c50dda55412cd051_request import A5f6e0a9550d3c58c50dda55412cd051Request
from gateway_api_sdk.models.model1aeebba947bfb42f364a2d5dd2ad8ef9200_response import Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id
    a5f6e0a9550d3c58c50dda55412cd051_request = gateway_api_sdk.A5f6e0a9550d3c58c50dda55412cd051Request() # A5f6e0a9550d3c58c50dda55412cd051Request | ProgrammingPackage definition

    try:
        # ProgrammingPackage@update
        api_response = api_instance.call_879046026ce3997dea0d9bf768f2f8e6(id, a5f6e0a9550d3c58c50dda55412cd051_request)
        print("The response of ProgrammingPackageApi->call_879046026ce3997dea0d9bf768f2f8e6:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->call_879046026ce3997dea0d9bf768f2f8e6: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 
 **a5f6e0a9550d3c58c50dda55412cd051_request** | [**A5f6e0a9550d3c58c50dda55412cd051Request**](A5f6e0a9550d3c58c50dda55412cd051Request.md)| ProgrammingPackage definition | 

### Return type

[**Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response**](Model1aeebba947bfb42f364a2d5dd2ad8ef9200Response.md)

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

# **fdbe7e1aad9b02084b06c6d647766efd**
> C29b5b3424f7317b69b4bda048ccfafb200Response fdbe7e1aad9b02084b06c6d647766efd(id)

ProgrammingPackage@destroy

Delete a system programming package

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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id

    try:
        # ProgrammingPackage@destroy
        api_response = api_instance.fdbe7e1aad9b02084b06c6d647766efd(id)
        print("The response of ProgrammingPackageApi->fdbe7e1aad9b02084b06c6d647766efd:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->fdbe7e1aad9b02084b06c6d647766efd: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 

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

