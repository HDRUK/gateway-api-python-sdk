# gateway_api_sdk.CancerTypeFilterApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_cancer_type_filter**](CancerTypeFilterApi.md#get_cancer_type_filter) | **GET** /api/v1/cancer-type-filters/{filter_id} | Get a single cancer type filter
[**get_cancer_type_filters**](CancerTypeFilterApi.md#get_cancer_type_filters) | **GET** /api/v1/cancer-type-filters | Get all cancer type filters


# **get_cancer_type_filter**
> GetCancerTypeFilter200Response get_cancer_type_filter(filter_id)

Get a single cancer type filter

Returns a single cancer type filter with its children by filter_id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.get_cancer_type_filter200_response import GetCancerTypeFilter200Response
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
    api_instance = gateway_api_sdk.CancerTypeFilterApi(api_client)
    filter_id = '0_0_2_59' # str | Filter ID (e.g., 0_0, 0_0_2_59)

    try:
        # Get a single cancer type filter
        api_response = api_instance.get_cancer_type_filter(filter_id)
        print("The response of CancerTypeFilterApi->get_cancer_type_filter:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CancerTypeFilterApi->get_cancer_type_filter: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_id** | **str**| Filter ID (e.g., 0_0, 0_0_2_59) | 

### Return type

[**GetCancerTypeFilter200Response**](GetCancerTypeFilter200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_cancer_type_filters**
> GetCancerTypeFilters200Response get_cancer_type_filters(parent_id=parent_id, level=level)

Get all cancer type filters

Returns a hierarchical tree of cancer type filters

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.get_cancer_type_filters200_response import GetCancerTypeFilters200Response
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
    api_instance = gateway_api_sdk.CancerTypeFilterApi(api_client)
    parent_id = 56 # int | Filter by parent ID (optional)
    level = 56 # int | Filter by hierarchy level (optional)

    try:
        # Get all cancer type filters
        api_response = api_instance.get_cancer_type_filters(parent_id=parent_id, level=level)
        print("The response of CancerTypeFilterApi->get_cancer_type_filters:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CancerTypeFilterApi->get_cancer_type_filters: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parent_id** | **int**| Filter by parent ID | [optional] 
 **level** | **int**| Filter by hierarchy level | [optional] 

### Return type

[**GetCancerTypeFilters200Response**](GetCancerTypeFilters200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

