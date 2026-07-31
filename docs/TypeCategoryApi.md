# gateway_api_sdk.TypeCategoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_016393e03d3b197d2172abf0d7ce08f5**](TypeCategoryApi.md#call_016393e03d3b197d2172abf0d7ce08f5) | **PUT** /api/v1/type_categories/{id} | TypeCategory@update
[**call_4864cc161acae07c9aaf81414fa6bebd**](TypeCategoryApi.md#call_4864cc161acae07c9aaf81414fa6bebd) | **DELETE** /api/v1/type_categories/{id} | TypeCategory@destroy
[**call_83ae406abb0fb38fa792b4cfcbbbebbf**](TypeCategoryApi.md#call_83ae406abb0fb38fa792b4cfcbbbebbf) | **POST** /api/v1/type_categories | TypeCategory@store
[**cd1f252c1f5296d0e6007eb543ef9099**](TypeCategoryApi.md#cd1f252c1f5296d0e6007eb543ef9099) | **GET** /api/v1/type_categories/{id} | TypeCategory@show
[**f5f0b860854ee5a33ee3d4b5f8a6d2fc**](TypeCategoryApi.md#f5f0b860854ee5a33ee3d4b5f8a6d2fc) | **GET** /api/v1/type_categories | TypeCategory@index
[**faae0a9813b380e92fba8a26820717ee**](TypeCategoryApi.md#faae0a9813b380e92fba8a26820717ee) | **PATCH** /api/v1/type_categories/{id} | TypeCategory@update


# **call_016393e03d3b197d2172abf0d7ce08f5**
> Model016393e03d3b197d2172abf0d7ce08f5200Response call_016393e03d3b197d2172abf0d7ce08f5(id, model016393e03d3b197d2172abf0d7ce08f5_request)

TypeCategory@update

Update a system type category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model016393e03d3b197d2172abf0d7ce08f5200_response import Model016393e03d3b197d2172abf0d7ce08f5200Response
from gateway_api_sdk.models.model016393e03d3b197d2172abf0d7ce08f5_request import Model016393e03d3b197d2172abf0d7ce08f5Request
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    id = 1 # int | type category id
    model016393e03d3b197d2172abf0d7ce08f5_request = gateway_api_sdk.Model016393e03d3b197d2172abf0d7ce08f5Request() # Model016393e03d3b197d2172abf0d7ce08f5Request | TypeCategory definition

    try:
        # TypeCategory@update
        api_response = api_instance.call_016393e03d3b197d2172abf0d7ce08f5(id, model016393e03d3b197d2172abf0d7ce08f5_request)
        print("The response of TypeCategoryApi->call_016393e03d3b197d2172abf0d7ce08f5:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->call_016393e03d3b197d2172abf0d7ce08f5: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| type category id | 
 **model016393e03d3b197d2172abf0d7ce08f5_request** | [**Model016393e03d3b197d2172abf0d7ce08f5Request**](Model016393e03d3b197d2172abf0d7ce08f5Request.md)| TypeCategory definition | 

### Return type

[**Model016393e03d3b197d2172abf0d7ce08f5200Response**](Model016393e03d3b197d2172abf0d7ce08f5200Response.md)

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

# **call_4864cc161acae07c9aaf81414fa6bebd**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_4864cc161acae07c9aaf81414fa6bebd(id)

TypeCategory@destroy

Delete a system type category

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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    id = 1 # int | type category id

    try:
        # TypeCategory@destroy
        api_response = api_instance.call_4864cc161acae07c9aaf81414fa6bebd(id)
        print("The response of TypeCategoryApi->call_4864cc161acae07c9aaf81414fa6bebd:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->call_4864cc161acae07c9aaf81414fa6bebd: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| type category id | 

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

# **call_83ae406abb0fb38fa792b4cfcbbbebbf**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_83ae406abb0fb38fa792b4cfcbbbebbf(model83ae406abb0fb38fa792b4cfcbbbebbf_request)

TypeCategory@store

Creates a new system type category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model83ae406abb0fb38fa792b4cfcbbbebbf_request import Model83ae406abb0fb38fa792b4cfcbbbebbfRequest
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    model83ae406abb0fb38fa792b4cfcbbbebbf_request = gateway_api_sdk.Model83ae406abb0fb38fa792b4cfcbbbebbfRequest() # Model83ae406abb0fb38fa792b4cfcbbbebbfRequest | Programming language definition

    try:
        # TypeCategory@store
        api_response = api_instance.call_83ae406abb0fb38fa792b4cfcbbbebbf(model83ae406abb0fb38fa792b4cfcbbbebbf_request)
        print("The response of TypeCategoryApi->call_83ae406abb0fb38fa792b4cfcbbbebbf:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->call_83ae406abb0fb38fa792b4cfcbbbebbf: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model83ae406abb0fb38fa792b4cfcbbbebbf_request** | [**Model83ae406abb0fb38fa792b4cfcbbbebbfRequest**](Model83ae406abb0fb38fa792b4cfcbbbebbfRequest.md)| Programming language definition | 

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

# **cd1f252c1f5296d0e6007eb543ef9099**
> Cd1f252c1f5296d0e6007eb543ef9099200Response cd1f252c1f5296d0e6007eb543ef9099(id)

TypeCategory@show

Return a single system type category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.cd1f252c1f5296d0e6007eb543ef9099200_response import Cd1f252c1f5296d0e6007eb543ef9099200Response
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    id = 1 # int | type category id

    try:
        # TypeCategory@show
        api_response = api_instance.cd1f252c1f5296d0e6007eb543ef9099(id)
        print("The response of TypeCategoryApi->cd1f252c1f5296d0e6007eb543ef9099:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->cd1f252c1f5296d0e6007eb543ef9099: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| type category id | 

### Return type

[**Cd1f252c1f5296d0e6007eb543ef9099200Response**](Cd1f252c1f5296d0e6007eb543ef9099200Response.md)

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

# **f5f0b860854ee5a33ee3d4b5f8a6d2fc**
> F5f0b860854ee5a33ee3d4b5f8a6d2fc200Response f5f0b860854ee5a33ee3d4b5f8a6d2fc()

TypeCategory@index

Returns a list of type categories enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.f5f0b860854ee5a33ee3d4b5f8a6d2fc200_response import F5f0b860854ee5a33ee3d4b5f8a6d2fc200Response
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)

    try:
        # TypeCategory@index
        api_response = api_instance.f5f0b860854ee5a33ee3d4b5f8a6d2fc()
        print("The response of TypeCategoryApi->f5f0b860854ee5a33ee3d4b5f8a6d2fc:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->f5f0b860854ee5a33ee3d4b5f8a6d2fc: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**F5f0b860854ee5a33ee3d4b5f8a6d2fc200Response**](F5f0b860854ee5a33ee3d4b5f8a6d2fc200Response.md)

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

# **faae0a9813b380e92fba8a26820717ee**
> Model016393e03d3b197d2172abf0d7ce08f5200Response faae0a9813b380e92fba8a26820717ee(id, a5f6e0a9550d3c58c50dda55412cd051_request)

TypeCategory@update

Edit a system type category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a5f6e0a9550d3c58c50dda55412cd051_request import A5f6e0a9550d3c58c50dda55412cd051Request
from gateway_api_sdk.models.model016393e03d3b197d2172abf0d7ce08f5200_response import Model016393e03d3b197d2172abf0d7ce08f5200Response
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    id = 1 # int | type category id
    a5f6e0a9550d3c58c50dda55412cd051_request = gateway_api_sdk.A5f6e0a9550d3c58c50dda55412cd051Request() # A5f6e0a9550d3c58c50dda55412cd051Request | TypeCategory definition

    try:
        # TypeCategory@update
        api_response = api_instance.faae0a9813b380e92fba8a26820717ee(id, a5f6e0a9550d3c58c50dda55412cd051_request)
        print("The response of TypeCategoryApi->faae0a9813b380e92fba8a26820717ee:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->faae0a9813b380e92fba8a26820717ee: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| type category id | 
 **a5f6e0a9550d3c58c50dda55412cd051_request** | [**A5f6e0a9550d3c58c50dda55412cd051Request**](A5f6e0a9550d3c58c50dda55412cd051Request.md)| TypeCategory definition | 

### Return type

[**Model016393e03d3b197d2172abf0d7ce08f5200Response**](Model016393e03d3b197d2172abf0d7ce08f5200Response.md)

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

