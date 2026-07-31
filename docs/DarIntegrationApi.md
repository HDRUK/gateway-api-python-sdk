# gateway_api_sdk.DarIntegrationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**c663ccf8b1926d7678370d095b9b358f**](DarIntegrationApi.md#c663ccf8b1926d7678370d095b9b358f) | **PATCH** /api/v1/dar-integration/{id} | DarIntegration@edit
[**call_09c033f0336380c3d8bb6801e96378bc**](DarIntegrationApi.md#call_09c033f0336380c3d8bb6801e96378bc) | **PUT** /api/v1/dar-integration/{id} | DarIntegration@update
[**call_17fa1074b71d9cefd3e65f2757117b57**](DarIntegrationApi.md#call_17fa1074b71d9cefd3e65f2757117b57) | **DELETE** /api/v1/dar-integrations/{id} | DarIntegration@destroy
[**call_406144045c21a19659ee66f6d4a78235**](DarIntegrationApi.md#call_406144045c21a19659ee66f6d4a78235) | **GET** /api/v1/dar-integration/{id} | DarIntegration@show
[**call_757fd0f4616caa763b0789d7ad7b3053**](DarIntegrationApi.md#call_757fd0f4616caa763b0789d7ad7b3053) | **POST** /api/v1/dar-integration/{id} | DarIntegration@store
[**call_7ab50add4fe0a4b7cff7eab0f4b8df18**](DarIntegrationApi.md#call_7ab50add4fe0a4b7cff7eab0f4b8df18) | **GET** /api/v1/dar-integration | DarIntegration@index


# **c663ccf8b1926d7678370d095b9b358f**
> Model09c033f0336380c3d8bb6801e96378bc200Response c663ccf8b1926d7678370d095b9b358f(id, c663ccf8b1926d7678370d095b9b358f_request)

DarIntegration@edit

Edit a DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c663ccf8b1926d7678370d095b9b358f_request import C663ccf8b1926d7678370d095b9b358fRequest
from gateway_api_sdk.models.model09c033f0336380c3d8bb6801e96378bc200_response import Model09c033f0336380c3d8bb6801e96378bc200Response
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id
    c663ccf8b1926d7678370d095b9b358f_request = gateway_api_sdk.C663ccf8b1926d7678370d095b9b358fRequest() # C663ccf8b1926d7678370d095b9b358fRequest | DarIntegration definition

    try:
        # DarIntegration@edit
        api_response = api_instance.c663ccf8b1926d7678370d095b9b358f(id, c663ccf8b1926d7678370d095b9b358f_request)
        print("The response of DarIntegrationApi->c663ccf8b1926d7678370d095b9b358f:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->c663ccf8b1926d7678370d095b9b358f: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 
 **c663ccf8b1926d7678370d095b9b358f_request** | [**C663ccf8b1926d7678370d095b9b358fRequest**](C663ccf8b1926d7678370d095b9b358fRequest.md)| DarIntegration definition | 

### Return type

[**Model09c033f0336380c3d8bb6801e96378bc200Response**](Model09c033f0336380c3d8bb6801e96378bc200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_09c033f0336380c3d8bb6801e96378bc**
> Model09c033f0336380c3d8bb6801e96378bc200Response call_09c033f0336380c3d8bb6801e96378bc(id, model09c033f0336380c3d8bb6801e96378bc_request)

DarIntegration@update

Updates a DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model09c033f0336380c3d8bb6801e96378bc200_response import Model09c033f0336380c3d8bb6801e96378bc200Response
from gateway_api_sdk.models.model09c033f0336380c3d8bb6801e96378bc_request import Model09c033f0336380c3d8bb6801e96378bcRequest
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id
    model09c033f0336380c3d8bb6801e96378bc_request = gateway_api_sdk.Model09c033f0336380c3d8bb6801e96378bcRequest() # Model09c033f0336380c3d8bb6801e96378bcRequest | DarIntegration definition

    try:
        # DarIntegration@update
        api_response = api_instance.call_09c033f0336380c3d8bb6801e96378bc(id, model09c033f0336380c3d8bb6801e96378bc_request)
        print("The response of DarIntegrationApi->call_09c033f0336380c3d8bb6801e96378bc:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->call_09c033f0336380c3d8bb6801e96378bc: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 
 **model09c033f0336380c3d8bb6801e96378bc_request** | [**Model09c033f0336380c3d8bb6801e96378bcRequest**](Model09c033f0336380c3d8bb6801e96378bcRequest.md)| DarIntegration definition | 

### Return type

[**Model09c033f0336380c3d8bb6801e96378bc200Response**](Model09c033f0336380c3d8bb6801e96378bc200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_17fa1074b71d9cefd3e65f2757117b57**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_17fa1074b71d9cefd3e65f2757117b57(id)

DarIntegration@destroy

Delete a system Dar Integration

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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id

    try:
        # DarIntegration@destroy
        api_response = api_instance.call_17fa1074b71d9cefd3e65f2757117b57(id)
        print("The response of DarIntegrationApi->call_17fa1074b71d9cefd3e65f2757117b57:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->call_17fa1074b71d9cefd3e65f2757117b57: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 

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

# **call_406144045c21a19659ee66f6d4a78235**
> Model7ab50add4fe0a4b7cff7eab0f4b8df18200ResponseDataInner call_406144045c21a19659ee66f6d4a78235(id)

DarIntegration@show

Returns a single DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model7ab50add4fe0a4b7cff7eab0f4b8df18200_response_data_inner import Model7ab50add4fe0a4b7cff7eab0f4b8df18200ResponseDataInner
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id

    try:
        # DarIntegration@show
        api_response = api_instance.call_406144045c21a19659ee66f6d4a78235(id)
        print("The response of DarIntegrationApi->call_406144045c21a19659ee66f6d4a78235:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->call_406144045c21a19659ee66f6d4a78235: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 

### Return type

[**Model7ab50add4fe0a4b7cff7eab0f4b8df18200ResponseDataInner**](Model7ab50add4fe0a4b7cff7eab0f4b8df18200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_757fd0f4616caa763b0789d7ad7b3053**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_757fd0f4616caa763b0789d7ad7b3053(id, model09c033f0336380c3d8bb6801e96378bc_request)

DarIntegration@store

Creates a new DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model09c033f0336380c3d8bb6801e96378bc_request import Model09c033f0336380c3d8bb6801e96378bcRequest
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id
    model09c033f0336380c3d8bb6801e96378bc_request = gateway_api_sdk.Model09c033f0336380c3d8bb6801e96378bcRequest() # Model09c033f0336380c3d8bb6801e96378bcRequest | DarIntegration definition

    try:
        # DarIntegration@store
        api_response = api_instance.call_757fd0f4616caa763b0789d7ad7b3053(id, model09c033f0336380c3d8bb6801e96378bc_request)
        print("The response of DarIntegrationApi->call_757fd0f4616caa763b0789d7ad7b3053:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->call_757fd0f4616caa763b0789d7ad7b3053: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 
 **model09c033f0336380c3d8bb6801e96378bc_request** | [**Model09c033f0336380c3d8bb6801e96378bcRequest**](Model09c033f0336380c3d8bb6801e96378bcRequest.md)| DarIntegration definition | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_7ab50add4fe0a4b7cff7eab0f4b8df18**
> Model7ab50add4fe0a4b7cff7eab0f4b8df18200Response call_7ab50add4fe0a4b7cff7eab0f4b8df18()

DarIntegration@index

Returns a list of DAR integrations enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model7ab50add4fe0a4b7cff7eab0f4b8df18200_response import Model7ab50add4fe0a4b7cff7eab0f4b8df18200Response
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)

    try:
        # DarIntegration@index
        api_response = api_instance.call_7ab50add4fe0a4b7cff7eab0f4b8df18()
        print("The response of DarIntegrationApi->call_7ab50add4fe0a4b7cff7eab0f4b8df18:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->call_7ab50add4fe0a4b7cff7eab0f4b8df18: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Model7ab50add4fe0a4b7cff7eab0f4b8df18200Response**](Model7ab50add4fe0a4b7cff7eab0f4b8df18200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

