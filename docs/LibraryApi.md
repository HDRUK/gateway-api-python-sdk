# gateway_api_sdk.LibraryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_077bba41c87bc61e6c290b3fea2a5848**](LibraryApi.md#call_077bba41c87bc61e6c290b3fea2a5848) | **PUT** /api/v1/libraries/{id} | Library@update
[**call_3b22aa4bb101550915e675702f8f3174**](LibraryApi.md#call_3b22aa4bb101550915e675702f8f3174) | **POST** /api/v1/libraries | Library@store
[**call_416921483907d62b39163e3c4188d10c**](LibraryApi.md#call_416921483907d62b39163e3c4188d10c) | **DELETE** /api/v1/libraries/{id} | Library@destroy
[**call_771bea7be0a7f7d2e0056f8c192100ad**](LibraryApi.md#call_771bea7be0a7f7d2e0056f8c192100ad) | **PATCH** /api/v1/libraries/{id} | Library@update
[**d736d637e675097aaf709dfd755864c7**](LibraryApi.md#d736d637e675097aaf709dfd755864c7) | **GET** /api/v1/libraries/{id} | Return a single library
[**list_libraries**](LibraryApi.md#list_libraries) | **GET** /api/v1/libraries | Retrieve a list of libraries


# **call_077bba41c87bc61e6c290b3fea2a5848**
> Model077bba41c87bc61e6c290b3fea2a5848200Response call_077bba41c87bc61e6c290b3fea2a5848(id, model3b22aa4bb101550915e675702f8f3174_request)

Library@update

Update a library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model077bba41c87bc61e6c290b3fea2a5848200_response import Model077bba41c87bc61e6c290b3fea2a5848200Response
from gateway_api_sdk.models.model3b22aa4bb101550915e675702f8f3174_request import Model3b22aa4bb101550915e675702f8f3174Request
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id
    model3b22aa4bb101550915e675702f8f3174_request = gateway_api_sdk.Model3b22aa4bb101550915e675702f8f3174Request() # Model3b22aa4bb101550915e675702f8f3174Request | library definition

    try:
        # Library@update
        api_response = api_instance.call_077bba41c87bc61e6c290b3fea2a5848(id, model3b22aa4bb101550915e675702f8f3174_request)
        print("The response of LibraryApi->call_077bba41c87bc61e6c290b3fea2a5848:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->call_077bba41c87bc61e6c290b3fea2a5848: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 
 **model3b22aa4bb101550915e675702f8f3174_request** | [**Model3b22aa4bb101550915e675702f8f3174Request**](Model3b22aa4bb101550915e675702f8f3174Request.md)| library definition | 

### Return type

[**Model077bba41c87bc61e6c290b3fea2a5848200Response**](Model077bba41c87bc61e6c290b3fea2a5848200Response.md)

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

# **call_3b22aa4bb101550915e675702f8f3174**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_3b22aa4bb101550915e675702f8f3174(model3b22aa4bb101550915e675702f8f3174_request)

Library@store

Creates a new library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model3b22aa4bb101550915e675702f8f3174_request import Model3b22aa4bb101550915e675702f8f3174Request
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    model3b22aa4bb101550915e675702f8f3174_request = gateway_api_sdk.Model3b22aa4bb101550915e675702f8f3174Request() # Model3b22aa4bb101550915e675702f8f3174Request | library definition

    try:
        # Library@store
        api_response = api_instance.call_3b22aa4bb101550915e675702f8f3174(model3b22aa4bb101550915e675702f8f3174_request)
        print("The response of LibraryApi->call_3b22aa4bb101550915e675702f8f3174:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->call_3b22aa4bb101550915e675702f8f3174: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model3b22aa4bb101550915e675702f8f3174_request** | [**Model3b22aa4bb101550915e675702f8f3174Request**](Model3b22aa4bb101550915e675702f8f3174Request.md)| library definition | 

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

# **call_416921483907d62b39163e3c4188d10c**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_416921483907d62b39163e3c4188d10c(id)

Library@destroy

Delete a library

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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id

    try:
        # Library@destroy
        api_response = api_instance.call_416921483907d62b39163e3c4188d10c(id)
        print("The response of LibraryApi->call_416921483907d62b39163e3c4188d10c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->call_416921483907d62b39163e3c4188d10c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 

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

# **call_771bea7be0a7f7d2e0056f8c192100ad**
> Model077bba41c87bc61e6c290b3fea2a5848200Response call_771bea7be0a7f7d2e0056f8c192100ad(id, model3b22aa4bb101550915e675702f8f3174_request)

Library@update

Edit a library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model077bba41c87bc61e6c290b3fea2a5848200_response import Model077bba41c87bc61e6c290b3fea2a5848200Response
from gateway_api_sdk.models.model3b22aa4bb101550915e675702f8f3174_request import Model3b22aa4bb101550915e675702f8f3174Request
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id
    model3b22aa4bb101550915e675702f8f3174_request = gateway_api_sdk.Model3b22aa4bb101550915e675702f8f3174Request() # Model3b22aa4bb101550915e675702f8f3174Request | library definition

    try:
        # Library@update
        api_response = api_instance.call_771bea7be0a7f7d2e0056f8c192100ad(id, model3b22aa4bb101550915e675702f8f3174_request)
        print("The response of LibraryApi->call_771bea7be0a7f7d2e0056f8c192100ad:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->call_771bea7be0a7f7d2e0056f8c192100ad: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 
 **model3b22aa4bb101550915e675702f8f3174_request** | [**Model3b22aa4bb101550915e675702f8f3174Request**](Model3b22aa4bb101550915e675702f8f3174Request.md)| library definition | 

### Return type

[**Model077bba41c87bc61e6c290b3fea2a5848200Response**](Model077bba41c87bc61e6c290b3fea2a5848200Response.md)

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

# **d736d637e675097aaf709dfd755864c7**
> D736d637e675097aaf709dfd755864c7200Response d736d637e675097aaf709dfd755864c7(id)

Return a single library

Return a single library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.d736d637e675097aaf709dfd755864c7200_response import D736d637e675097aaf709dfd755864c7200Response
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id

    try:
        # Return a single library
        api_response = api_instance.d736d637e675097aaf709dfd755864c7(id)
        print("The response of LibraryApi->d736d637e675097aaf709dfd755864c7:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->d736d637e675097aaf709dfd755864c7: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 

### Return type

[**D736d637e675097aaf709dfd755864c7200Response**](D736d637e675097aaf709dfd755864c7200Response.md)

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

# **list_libraries**
> ListLibraries200Response list_libraries(per_page=per_page)

Retrieve a list of libraries

Returns a paginated list of libraries along with associated datasets and teams.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.list_libraries200_response import ListLibraries200Response
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    per_page = 10 # int | Specify the number of libraries per page (optional) (default to 10)

    try:
        # Retrieve a list of libraries
        api_response = api_instance.list_libraries(per_page=per_page)
        print("The response of LibraryApi->list_libraries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->list_libraries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| Specify the number of libraries per page | [optional] [default to 10]

### Return type

[**ListLibraries200Response**](ListLibraries200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

