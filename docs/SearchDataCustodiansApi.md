# gateway_api_sdk.SearchDataCustodiansApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ada26698c9cdc86c01aaf53b0677a48d**](SearchDataCustodiansApi.md#ada26698c9cdc86c01aaf53b0677a48d) | **POST** /api/v1/search/data_custodians | Search@data_custodians


# **ada26698c9cdc86c01aaf53b0677a48d**
> Ada26698c9cdc86c01aaf53b0677a48d200Response ada26698c9cdc86c01aaf53b0677a48d(ada26698c9cdc86c01aaf53b0677a48d_request, sort=sort, direction=direction, per_page=per_page)

Search@data_custodians

Returns gateway data custodians related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.ada26698c9cdc86c01aaf53b0677a48d200_response import Ada26698c9cdc86c01aaf53b0677a48d200Response
from gateway_api_sdk.models.ada26698c9cdc86c01aaf53b0677a48d_request import Ada26698c9cdc86c01aaf53b0677a48dRequest
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
    api_instance = gateway_api_sdk.SearchDataCustodiansApi(api_client)
    ada26698c9cdc86c01aaf53b0677a48d_request = gateway_api_sdk.Ada26698c9cdc86c01aaf53b0677a48dRequest() # Ada26698c9cdc86c01aaf53b0677a48dRequest | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)
    per_page = 25 # int | Number of results to return per page (optional)

    try:
        # Search@data_custodians
        api_response = api_instance.ada26698c9cdc86c01aaf53b0677a48d(ada26698c9cdc86c01aaf53b0677a48d_request, sort=sort, direction=direction, per_page=per_page)
        print("The response of SearchDataCustodiansApi->ada26698c9cdc86c01aaf53b0677a48d:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchDataCustodiansApi->ada26698c9cdc86c01aaf53b0677a48d: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ada26698c9cdc86c01aaf53b0677a48d_request** | [**Ada26698c9cdc86c01aaf53b0677a48dRequest**](Ada26698c9cdc86c01aaf53b0677a48dRequest.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 
 **per_page** | **int**| Number of results to return per page | [optional] 

### Return type

[**Ada26698c9cdc86c01aaf53b0677a48d200Response**](Ada26698c9cdc86c01aaf53b0677a48d200Response.md)

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

