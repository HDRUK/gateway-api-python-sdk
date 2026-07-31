# gateway_api_sdk.SearchDataUsesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_8db417727e7fe7c2e99206b060a3b882**](SearchDataUsesApi.md#call_8db417727e7fe7c2e99206b060a3b882) | **POST** /api/v1/search/dur | Search@data_uses


# **call_8db417727e7fe7c2e99206b060a3b882**
> Model8db417727e7fe7c2e99206b060a3b882200Response call_8db417727e7fe7c2e99206b060a3b882(model8db417727e7fe7c2e99206b060a3b882_request, sort=sort, direction=direction, download=download)

Search@data_uses

Returns gateway data uses related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model8db417727e7fe7c2e99206b060a3b882200_response import Model8db417727e7fe7c2e99206b060a3b882200Response
from gateway_api_sdk.models.model8db417727e7fe7c2e99206b060a3b882_request import Model8db417727e7fe7c2e99206b060a3b882Request
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
    model8db417727e7fe7c2e99206b060a3b882_request = gateway_api_sdk.Model8db417727e7fe7c2e99206b060a3b882Request() # Model8db417727e7fe7c2e99206b060a3b882Request | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)
    download = true # bool | Download a csv of the results (default: false) (optional)

    try:
        # Search@data_uses
        api_response = api_instance.call_8db417727e7fe7c2e99206b060a3b882(model8db417727e7fe7c2e99206b060a3b882_request, sort=sort, direction=direction, download=download)
        print("The response of SearchDataUsesApi->call_8db417727e7fe7c2e99206b060a3b882:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchDataUsesApi->call_8db417727e7fe7c2e99206b060a3b882: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model8db417727e7fe7c2e99206b060a3b882_request** | [**Model8db417727e7fe7c2e99206b060a3b882Request**](Model8db417727e7fe7c2e99206b060a3b882Request.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 
 **download** | **bool**| Download a csv of the results (default: false) | [optional] 

### Return type

[**Model8db417727e7fe7c2e99206b060a3b882200Response**](Model8db417727e7fe7c2e99206b060a3b882200Response.md)

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

