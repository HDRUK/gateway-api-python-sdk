# gateway_api_sdk.SearchDataUsesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_data_uses**](SearchDataUsesApi.md#search_data_uses) | **POST** /api/v1/search/dur | Search@data_uses


# **search_data_uses**
> SearchDataUses200Response search_data_uses(search_data_uses_request, sort=sort, direction=direction, download=download)

Search@data_uses

Returns gateway data uses related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.search_data_uses200_response import SearchDataUses200Response
from gateway_api_sdk.models.search_data_uses_request import SearchDataUsesRequest
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
    api_instance = gateway_api_sdk.SearchDataUsesApi(api_client)
    search_data_uses_request = gateway_api_sdk.SearchDataUsesRequest() # SearchDataUsesRequest | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)
    download = true # bool | Download a csv of the results (default: false) (optional)

    try:
        # Search@data_uses
        api_response = api_instance.search_data_uses(search_data_uses_request, sort=sort, direction=direction, download=download)
        print("The response of SearchDataUsesApi->search_data_uses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchDataUsesApi->search_data_uses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_data_uses_request** | [**SearchDataUsesRequest**](SearchDataUsesRequest.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 
 **download** | **bool**| Download a csv of the results (default: false) | [optional] 

### Return type

[**SearchDataUses200Response**](SearchDataUses200Response.md)

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

