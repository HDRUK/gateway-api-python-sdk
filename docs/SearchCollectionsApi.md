# gateway_api_sdk.SearchCollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**aa33edfdace17b70600d964e0db4d44b**](SearchCollectionsApi.md#aa33edfdace17b70600d964e0db4d44b) | **POST** /api/v1/search/collections | Search@collections


# **aa33edfdace17b70600d964e0db4d44b**
> Aa33edfdace17b70600d964e0db4d44b200Response aa33edfdace17b70600d964e0db4d44b(aa33edfdace17b70600d964e0db4d44b_request, sort=sort, direction=direction)

Search@collections

Returns gateway collections related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.aa33edfdace17b70600d964e0db4d44b200_response import Aa33edfdace17b70600d964e0db4d44b200Response
from gateway_api_sdk.models.aa33edfdace17b70600d964e0db4d44b_request import Aa33edfdace17b70600d964e0db4d44bRequest
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
    aa33edfdace17b70600d964e0db4d44b_request = gateway_api_sdk.Aa33edfdace17b70600d964e0db4d44bRequest() # Aa33edfdace17b70600d964e0db4d44bRequest | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)

    try:
        # Search@collections
        api_response = api_instance.aa33edfdace17b70600d964e0db4d44b(aa33edfdace17b70600d964e0db4d44b_request, sort=sort, direction=direction)
        print("The response of SearchCollectionsApi->aa33edfdace17b70600d964e0db4d44b:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchCollectionsApi->aa33edfdace17b70600d964e0db4d44b: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **aa33edfdace17b70600d964e0db4d44b_request** | [**Aa33edfdace17b70600d964e0db4d44bRequest**](Aa33edfdace17b70600d964e0db4d44bRequest.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 

### Return type

[**Aa33edfdace17b70600d964e0db4d44b200Response**](Aa33edfdace17b70600d964e0db4d44b200Response.md)

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

