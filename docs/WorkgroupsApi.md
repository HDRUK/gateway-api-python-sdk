# gateway_api_sdk.WorkgroupsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_all_workgroups**](WorkgroupsApi.md#fetch_all_workgroups) | **GET** /api/v1/workgroups | WorkgroupController@index


# **fetch_all_workgroups**
> FetchAllWorkgroups200Response fetch_all_workgroups()

WorkgroupController@index

Get All Workgroups

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_workgroups200_response import FetchAllWorkgroups200Response
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
    api_instance = gateway_api_sdk.WorkgroupsApi(api_client)

    try:
        # WorkgroupController@index
        api_response = api_instance.fetch_all_workgroups()
        print("The response of WorkgroupsApi->fetch_all_workgroups:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WorkgroupsApi->fetch_all_workgroups: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllWorkgroups200Response**](FetchAllWorkgroups200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

