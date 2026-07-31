# gateway_api_sdk.SearchDatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**b60e5c6bd58001740003449e91216454**](SearchDatasetsApi.md#b60e5c6bd58001740003449e91216454) | **POST** /api/v1/search/datasets | Search@datasets


# **b60e5c6bd58001740003449e91216454**
> B60e5c6bd58001740003449e91216454200Response b60e5c6bd58001740003449e91216454(b60e5c6bd58001740003449e91216454_request)

Search@datasets

Returns gateway datasets related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.b60e5c6bd58001740003449e91216454200_response import B60e5c6bd58001740003449e91216454200Response
from gateway_api_sdk.models.b60e5c6bd58001740003449e91216454_request import B60e5c6bd58001740003449e91216454Request
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
    api_instance = gateway_api_sdk.SearchDatasetsApi(api_client)
    b60e5c6bd58001740003449e91216454_request = gateway_api_sdk.B60e5c6bd58001740003449e91216454Request() # B60e5c6bd58001740003449e91216454Request | Submit search query

    try:
        # Search@datasets
        api_response = api_instance.b60e5c6bd58001740003449e91216454(b60e5c6bd58001740003449e91216454_request)
        print("The response of SearchDatasetsApi->b60e5c6bd58001740003449e91216454:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchDatasetsApi->b60e5c6bd58001740003449e91216454: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **b60e5c6bd58001740003449e91216454_request** | [**B60e5c6bd58001740003449e91216454Request**](B60e5c6bd58001740003449e91216454Request.md)| Submit search query | 

### Return type

[**B60e5c6bd58001740003449e91216454200Response**](B60e5c6bd58001740003449e91216454200Response.md)

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

