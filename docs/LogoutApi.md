# gateway_api_sdk.LogoutApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**logout**](LogoutApi.md#logout) | **POST** /api/v1/logout | LogoutController@logout


# **logout**
> DeleteAliases200Response logout()

LogoutController@logout

logout

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
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
    api_instance = gateway_api_sdk.LogoutApi(api_client)

    try:
        # LogoutController@logout
        api_response = api_instance.logout()
        print("The response of LogoutApi->logout:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LogoutApi->logout: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

