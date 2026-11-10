# gateway_api_sdk.AdminApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**revoke_all_tokens_v2**](AdminApi.md#revoke_all_tokens_v2) | **POST** /api/v2/admin/tokens/revoke_all | TokenRevocationController@revokeAll


# **revoke_all_tokens_v2**
> RevokeAllTokensV2200Response revoke_all_tokens_v2()

TokenRevocationController@revokeAll

Revoke every Gateway JWT issued up to now, including the caller's own. All users must sign in again.

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.revoke_all_tokens_v2200_response import RevokeAllTokensV2200Response
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
    api_instance = gateway_api_sdk.AdminApi(api_client)

    try:
        # TokenRevocationController@revokeAll
        api_response = api_instance.revoke_all_tokens_v2()
        print("The response of AdminApi->revoke_all_tokens_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminApi->revoke_all_tokens_v2: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**RevokeAllTokensV2200Response**](RevokeAllTokensV2200Response.md)

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

