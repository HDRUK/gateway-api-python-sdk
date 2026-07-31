# gateway_api_sdk.SearchCollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_collections**](SearchCollectionsApi.md#search_collections) | **POST** /api/v1/search/collections | Search@collections


# **search_collections**
> SearchCollections200Response search_collections(search_collections_request, sort=sort, direction=direction)

Search@collections

Returns gateway collections related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.search_collections200_response import SearchCollections200Response
from gateway_api_sdk.models.search_collections_request import SearchCollectionsRequest
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
    api_instance = gateway_api_sdk.SearchCollectionsApi(api_client)
    search_collections_request = gateway_api_sdk.SearchCollectionsRequest() # SearchCollectionsRequest | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)

    try:
        # Search@collections
        api_response = api_instance.search_collections(search_collections_request, sort=sort, direction=direction)
        print("The response of SearchCollectionsApi->search_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchCollectionsApi->search_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_collections_request** | [**SearchCollectionsRequest**](SearchCollectionsRequest.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 

### Return type

[**SearchCollections200Response**](SearchCollections200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

