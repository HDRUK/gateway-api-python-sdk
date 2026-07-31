# gateway_api_sdk.SearchDataCustodianNetworksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_9b95892cc29cee3ccd11e3f92223224c**](SearchDataCustodianNetworksApi.md#call_9b95892cc29cee3ccd11e3f92223224c) | **POST** /api/v1/search/data_custodian_networks | Search@data_custodian_networks


# **call_9b95892cc29cee3ccd11e3f92223224c**
> Model9b95892cc29cee3ccd11e3f92223224c200Response call_9b95892cc29cee3ccd11e3f92223224c(model9b95892cc29cee3ccd11e3f92223224c_request, sort=sort, direction=direction)

Search@data_custodian_networks

Returns gateway data custodian networks related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model9b95892cc29cee3ccd11e3f92223224c200_response import Model9b95892cc29cee3ccd11e3f92223224c200Response
from gateway_api_sdk.models.model9b95892cc29cee3ccd11e3f92223224c_request import Model9b95892cc29cee3ccd11e3f92223224cRequest
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
    api_instance = gateway_api_sdk.SearchDataCustodianNetworksApi(api_client)
    model9b95892cc29cee3ccd11e3f92223224c_request = gateway_api_sdk.Model9b95892cc29cee3ccd11e3f92223224cRequest() # Model9b95892cc29cee3ccd11e3f92223224cRequest | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)

    try:
        # Search@data_custodian_networks
        api_response = api_instance.call_9b95892cc29cee3ccd11e3f92223224c(model9b95892cc29cee3ccd11e3f92223224c_request, sort=sort, direction=direction)
        print("The response of SearchDataCustodianNetworksApi->call_9b95892cc29cee3ccd11e3f92223224c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchDataCustodianNetworksApi->call_9b95892cc29cee3ccd11e3f92223224c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model9b95892cc29cee3ccd11e3f92223224c_request** | [**Model9b95892cc29cee3ccd11e3f92223224cRequest**](Model9b95892cc29cee3ccd11e3f92223224cRequest.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 

### Return type

[**Model9b95892cc29cee3ccd11e3f92223224c200Response**](Model9b95892cc29cee3ccd11e3f92223224c200Response.md)

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

