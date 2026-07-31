# gateway_api_sdk.SearchSimilarDatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_similar_datasets**](SearchSimilarDatasetsApi.md#search_similar_datasets) | **POST** /api/v1/search/similar/datasets | Search@similarDatasets


# **search_similar_datasets**
> SearchSimilarDatasets200Response search_similar_datasets(search_similar_datasets_request)

Search@similarDatasets

Returns top three gateway datasets most similar to the provided dataset

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.search_similar_datasets200_response import SearchSimilarDatasets200Response
from gateway_api_sdk.models.search_similar_datasets_request import SearchSimilarDatasetsRequest
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
    search_similar_datasets_request = gateway_api_sdk.SearchSimilarDatasetsRequest() # SearchSimilarDatasetsRequest | Submit dataset id

    try:
        # Search@similarDatasets
        api_response = api_instance.search_similar_datasets(search_similar_datasets_request)
        print("The response of SearchSimilarDatasetsApi->search_similar_datasets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchSimilarDatasetsApi->search_similar_datasets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_similar_datasets_request** | [**SearchSimilarDatasetsRequest**](SearchSimilarDatasetsRequest.md)| Submit dataset id | 

### Return type

[**SearchSimilarDatasets200Response**](SearchSimilarDatasets200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

