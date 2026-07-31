# gateway_api_sdk.EnquiryThreadApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_enquiry_threads**](EnquiryThreadApi.md#create_enquiry_threads) | **POST** /api/v1/enquiry_threads | EnquiryThread@store
[**fetch_all_enquiry_threads**](EnquiryThreadApi.md#fetch_all_enquiry_threads) | **GET** /api/v1/enquiry_threads | EnquiryThread@index
[**fetch_enquiry_threads**](EnquiryThreadApi.md#fetch_enquiry_threads) | **GET** /api/v1/enquiry_threads/{id} | EnquiryThread@show


# **create_enquiry_threads**
> CreateCategories200Response create_enquiry_threads(create_enquiry_threads_request)

EnquiryThread@store

Creates one or more new EnquiryThreads

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_enquiry_threads_request import CreateEnquiryThreadsRequest
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
    create_enquiry_threads_request = gateway_api_sdk.CreateEnquiryThreadsRequest() # CreateEnquiryThreadsRequest | EnquiryThread definition

    try:
        # EnquiryThread@store
        api_response = api_instance.create_enquiry_threads(create_enquiry_threads_request)
        print("The response of EnquiryThreadApi->create_enquiry_threads:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnquiryThreadApi->create_enquiry_threads: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_enquiry_threads_request** | [**CreateEnquiryThreadsRequest**](CreateEnquiryThreadsRequest.md)| EnquiryThread definition | 

### Return type

[**CreateCategories200Response**](CreateCategories200Response.md)

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

# **fetch_all_enquiry_threads**
> FetchAllEnquiryThreads200Response fetch_all_enquiry_threads(per_page=per_page)

EnquiryThread@index

Returns a list of EnquiryThreads from the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_enquiry_threads200_response import FetchAllEnquiryThreads200Response
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
        api_response = api_instance.fetch_all_enquiry_threads(per_page=per_page)
        print("The response of EnquiryThreadApi->fetch_all_enquiry_threads:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnquiryThreadApi->fetch_all_enquiry_threads: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchAllEnquiryThreads200Response**](FetchAllEnquiryThreads200Response.md)

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

# **fetch_enquiry_threads**
> FetchAllEnquiryThreads200Response fetch_enquiry_threads(id)

EnquiryThread@show

Return a single EnquiryThread

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_enquiry_threads200_response import FetchAllEnquiryThreads200Response
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
        api_response = api_instance.fetch_enquiry_threads(id)
        print("The response of EnquiryThreadApi->fetch_enquiry_threads:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnquiryThreadApi->fetch_enquiry_threads: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| EnquiryThread id | 

### Return type

[**FetchAllEnquiryThreads200Response**](FetchAllEnquiryThreads200Response.md)

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

