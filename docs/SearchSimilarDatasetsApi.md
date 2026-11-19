# gateway_api_sdk.SearchSimilarDatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_similar_datasets**](SearchSimilarDatasetsApi.md#search_similar_datasets) | **POST** /api/v1/search/similar/datasets | Search for similar datasets (deprecated)
[**search_similar_datasets_v2**](SearchSimilarDatasetsApi.md#search_similar_datasets_v2) | **POST** /api/v2/search/similar/datasets | Search for similar datasets


# **search_similar_datasets**
> search_similar_datasets(search_similar_datasets_v2_request)

Search for similar datasets (deprecated)

Deprecated: use /api/v2/search/similar/datasets, which this endpoint now serves. Responses carry Deprecation, Sunset and Link headers; it stops working after the Sunset date (17 May 2027).

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.search_similar_datasets_v2_request import SearchSimilarDatasetsV2Request
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
    api_instance = gateway_api_sdk.SearchSimilarDatasetsApi(api_client)
    search_similar_datasets_v2_request = gateway_api_sdk.SearchSimilarDatasetsV2Request() # SearchSimilarDatasetsV2Request | 

    try:
        # Search for similar datasets (deprecated)
        api_instance.search_similar_datasets(search_similar_datasets_v2_request)
    except Exception as e:
        print("Exception when calling SearchSimilarDatasetsApi->search_similar_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_similar_datasets_v2_request** | [**SearchSimilarDatasetsV2Request**](SearchSimilarDatasetsV2Request.md)|  | 

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
**200** | Same as /api/v2/search/similar/datasets |  -  |
**400** | Missing or invalid dataset id |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **search_similar_datasets_v2**
> SearchSimilarDatasetsV2200Response search_similar_datasets_v2(search_similar_datasets_v2_request)

Search for similar datasets

Returns up to three gateway datasets sharing the most terms with the provided dataset's keywords and title. The provided dataset is never included.

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.search_similar_datasets_v2200_response import SearchSimilarDatasetsV2200Response
from gateway_api_sdk.models.search_similar_datasets_v2_request import SearchSimilarDatasetsV2Request
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
    api_instance = gateway_api_sdk.SearchSimilarDatasetsApi(api_client)
    search_similar_datasets_v2_request = gateway_api_sdk.SearchSimilarDatasetsV2Request() # SearchSimilarDatasetsV2Request | 

    try:
        # Search for similar datasets
        api_response = api_instance.search_similar_datasets_v2(search_similar_datasets_v2_request)
        print("The response of SearchSimilarDatasetsApi->search_similar_datasets_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchSimilarDatasetsApi->search_similar_datasets_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_similar_datasets_v2_request** | [**SearchSimilarDatasetsV2Request**](SearchSimilarDatasetsV2Request.md)|  | 

### Return type

[**SearchSimilarDatasetsV2200Response**](SearchSimilarDatasetsV2200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success; empty data when the dataset is not indexed |  -  |
**400** | Missing or invalid dataset id |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

