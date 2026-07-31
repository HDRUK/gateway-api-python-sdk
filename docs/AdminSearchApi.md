# gateway_api_sdk.AdminSearchApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_4ff0fc5e7c66284608ce55dc6cb7d846**](AdminSearchApi.md#call_4ff0fc5e7c66284608ce55dc6cb7d846) | **POST** /api/v1/admin/search/feature | Activate or deactivate a search-related Pennant feature flag
[**call_8918bd9dfb8e055a335f3c0695428e73**](AdminSearchApi.md#call_8918bd9dfb8e055a335f3c0695428e73) | **GET** /api/v1/admin/search/status | Get Typesense collection status for every onboarded search entity
[**call_92a06ea019f5560b5c9e76e02fe38e31**](AdminSearchApi.md#call_92a06ea019f5560b5c9e76e02fe38e31) | **POST** /api/v1/admin/search/reindex | Queue a drop+recreate+import of a search entity&#39;s Typesense collection


# **call_4ff0fc5e7c66284608ce55dc6cb7d846**
> call_4ff0fc5e7c66284608ce55dc6cb7d846(model4ff0fc5e7c66284608ce55dc6cb7d846_request)

Activate or deactivate a search-related Pennant feature flag

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.model4ff0fc5e7c66284608ce55dc6cb7d846_request import Model4ff0fc5e7c66284608ce55dc6cb7d846Request
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.AdminSearchApi(api_client)
    model4ff0fc5e7c66284608ce55dc6cb7d846_request = gateway_api_sdk.Model4ff0fc5e7c66284608ce55dc6cb7d846Request() # Model4ff0fc5e7c66284608ce55dc6cb7d846Request | 

    try:
        # Activate or deactivate a search-related Pennant feature flag
        api_instance.call_4ff0fc5e7c66284608ce55dc6cb7d846(model4ff0fc5e7c66284608ce55dc6cb7d846_request)
    except Exception as e:
        print("Exception when calling AdminSearchApi->call_4ff0fc5e7c66284608ce55dc6cb7d846: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model4ff0fc5e7c66284608ce55dc6cb7d846_request** | [**Model4ff0fc5e7c66284608ce55dc6cb7d846Request**](Model4ff0fc5e7c66284608ce55dc6cb7d846Request.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**422** | Unknown feature |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_8918bd9dfb8e055a335f3c0695428e73**
> call_8918bd9dfb8e055a335f3c0695428e73()

Get Typesense collection status for every onboarded search entity

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.AdminSearchApi(api_client)

    try:
        # Get Typesense collection status for every onboarded search entity
        api_instance.call_8918bd9dfb8e055a335f3c0695428e73()
    except Exception as e:
        print("Exception when calling AdminSearchApi->call_8918bd9dfb8e055a335f3c0695428e73: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_92a06ea019f5560b5c9e76e02fe38e31**
> call_92a06ea019f5560b5c9e76e02fe38e31(model92a06ea019f5560b5c9e76e02fe38e31_request)

Queue a drop+recreate+import of a search entity's Typesense collection

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.model92a06ea019f5560b5c9e76e02fe38e31_request import Model92a06ea019f5560b5c9e76e02fe38e31Request
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.AdminSearchApi(api_client)
    model92a06ea019f5560b5c9e76e02fe38e31_request = gateway_api_sdk.Model92a06ea019f5560b5c9e76e02fe38e31Request() # Model92a06ea019f5560b5c9e76e02fe38e31Request | 

    try:
        # Queue a drop+recreate+import of a search entity's Typesense collection
        api_instance.call_92a06ea019f5560b5c9e76e02fe38e31(model92a06ea019f5560b5c9e76e02fe38e31_request)
    except Exception as e:
        print("Exception when calling AdminSearchApi->call_92a06ea019f5560b5c9e76e02fe38e31: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model92a06ea019f5560b5c9e76e02fe38e31_request** | [**Model92a06ea019f5560b5c9e76e02fe38e31Request**](Model92a06ea019f5560b5c9e76e02fe38e31Request.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**202** | Reindex queued |  -  |
**422** | Unknown entity |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

