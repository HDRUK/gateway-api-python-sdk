# gateway_api_sdk.AdminSearchApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_admin_search_reindex**](AdminSearchApi.md#create_admin_search_reindex) | **POST** /api/v1/admin/search/reindex | Queue a drop+recreate+import of a search entity&#39;s Typesense collection
[**fetch_admin_search_status**](AdminSearchApi.md#fetch_admin_search_status) | **GET** /api/v1/admin/search/status | Get Typesense collection status for every onboarded search entity
[**update_admin_search_feature**](AdminSearchApi.md#update_admin_search_feature) | **POST** /api/v1/admin/search/feature | Activate or deactivate a search-related Pennant feature flag


# **create_admin_search_reindex**
> create_admin_search_reindex(create_admin_search_reindex_request)

Queue a drop+recreate+import of a search entity's Typesense collection

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_admin_search_reindex_request import CreateAdminSearchReindexRequest
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
    create_admin_search_reindex_request = gateway_api_sdk.CreateAdminSearchReindexRequest() # CreateAdminSearchReindexRequest | 

    try:
        # Queue a drop+recreate+import of a search entity's Typesense collection
        api_instance.create_admin_search_reindex(create_admin_search_reindex_request)
    except Exception as e:
        print("Exception when calling AdminSearchApi->create_admin_search_reindex: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_admin_search_reindex_request** | [**CreateAdminSearchReindexRequest**](CreateAdminSearchReindexRequest.md)|  | 

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

# **fetch_admin_search_status**
> fetch_admin_search_status()

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
        api_instance.fetch_admin_search_status()
    except Exception as e:
        print("Exception when calling AdminSearchApi->fetch_admin_search_status: %s\n" % e)
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

# **update_admin_search_feature**
> update_admin_search_feature(update_admin_search_feature_request)

Activate or deactivate a search-related Pennant feature flag

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.update_admin_search_feature_request import UpdateAdminSearchFeatureRequest
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
    update_admin_search_feature_request = gateway_api_sdk.UpdateAdminSearchFeatureRequest() # UpdateAdminSearchFeatureRequest | 

    try:
        # Activate or deactivate a search-related Pennant feature flag
        api_instance.update_admin_search_feature(update_admin_search_feature_request)
    except Exception as e:
        print("Exception when calling AdminSearchApi->update_admin_search_feature: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **update_admin_search_feature_request** | [**UpdateAdminSearchFeatureRequest**](UpdateAdminSearchFeatureRequest.md)|  | 

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

