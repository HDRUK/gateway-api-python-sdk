# gateway_api_sdk.EnquiryThreadApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**a961db529080eb3a29e4b7cc13dabaaa**](EnquiryThreadApi.md#a961db529080eb3a29e4b7cc13dabaaa) | **POST** /api/v1/enquiry_threads | EnquiryThread@store
[**call_4321ab5e45636e3e917c94fd21edac28**](EnquiryThreadApi.md#call_4321ab5e45636e3e917c94fd21edac28) | **GET** /api/v1/enquiry_threads | EnquiryThread@index
[**fd828cd8df74859b18600bb6b36edf83**](EnquiryThreadApi.md#fd828cd8df74859b18600bb6b36edf83) | **GET** /api/v1/enquiry_threads/{id} | EnquiryThread@show


# **a961db529080eb3a29e4b7cc13dabaaa**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response a961db529080eb3a29e4b7cc13dabaaa(a961db529080eb3a29e4b7cc13dabaaa_request)

EnquiryThread@store

Creates one or more new EnquiryThreads

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a961db529080eb3a29e4b7cc13dabaaa_request import A961db529080eb3a29e4b7cc13dabaaaRequest
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
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
    api_instance = gateway_api_sdk.EnquiryThreadApi(api_client)
    a961db529080eb3a29e4b7cc13dabaaa_request = gateway_api_sdk.A961db529080eb3a29e4b7cc13dabaaaRequest() # A961db529080eb3a29e4b7cc13dabaaaRequest | EnquiryThread definition

    try:
        # EnquiryThread@store
        api_response = api_instance.a961db529080eb3a29e4b7cc13dabaaa(a961db529080eb3a29e4b7cc13dabaaa_request)
        print("The response of EnquiryThreadApi->a961db529080eb3a29e4b7cc13dabaaa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnquiryThreadApi->a961db529080eb3a29e4b7cc13dabaaa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **a961db529080eb3a29e4b7cc13dabaaa_request** | [**A961db529080eb3a29e4b7cc13dabaaaRequest**](A961db529080eb3a29e4b7cc13dabaaaRequest.md)| EnquiryThread definition | 

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

# **call_4321ab5e45636e3e917c94fd21edac28**
> Model4321ab5e45636e3e917c94fd21edac28200Response call_4321ab5e45636e3e917c94fd21edac28(per_page=per_page)

EnquiryThread@index

Returns a list of EnquiryThreads from the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model4321ab5e45636e3e917c94fd21edac28200_response import Model4321ab5e45636e3e917c94fd21edac28200Response
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
    api_instance = gateway_api_sdk.EnquiryThreadApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # EnquiryThread@index
        api_response = api_instance.call_4321ab5e45636e3e917c94fd21edac28(per_page=per_page)
        print("The response of EnquiryThreadApi->call_4321ab5e45636e3e917c94fd21edac28:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnquiryThreadApi->call_4321ab5e45636e3e917c94fd21edac28: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**Model4321ab5e45636e3e917c94fd21edac28200Response**](Model4321ab5e45636e3e917c94fd21edac28200Response.md)

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

# **fd828cd8df74859b18600bb6b36edf83**
> Model4321ab5e45636e3e917c94fd21edac28200Response fd828cd8df74859b18600bb6b36edf83(id)

EnquiryThread@show

Return a single EnquiryThread

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model4321ab5e45636e3e917c94fd21edac28200_response import Model4321ab5e45636e3e917c94fd21edac28200Response
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
    api_instance = gateway_api_sdk.EnquiryThreadApi(api_client)
    id = 1 # int | EnquiryThread id

    try:
        # EnquiryThread@show
        api_response = api_instance.fd828cd8df74859b18600bb6b36edf83(id)
        print("The response of EnquiryThreadApi->fd828cd8df74859b18600bb6b36edf83:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnquiryThreadApi->fd828cd8df74859b18600bb6b36edf83: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| EnquiryThread id | 

### Return type

[**Model4321ab5e45636e3e917c94fd21edac28200Response**](Model4321ab5e45636e3e917c94fd21edac28200Response.md)

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

