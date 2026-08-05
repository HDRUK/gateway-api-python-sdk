# gateway_api_sdk.UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**verify_secondary_email**](UsersApi.md#verify_secondary_email) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user&#39;s secondary email using a UUID


# **verify_secondary_email**
> VerifySecondaryEmail200Response verify_secondary_email(uuid)

Verify user's secondary email using a UUID

This endpoint verifies the secondary email for a user if the UUID is valid and not expired.

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.verify_secondary_email200_response import VerifySecondaryEmail200Response
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    uuid = '03af1f5e-5cd2-4c41-ae23-56dd2c9efc67' # str | Verification UUID

    try:
        # Verify user's secondary email using a UUID
        api_response = api_instance.verify_secondary_email(uuid)
        print("The response of UsersApi->verify_secondary_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->verify_secondary_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **str**| Verification UUID | 

### Return type

[**VerifySecondaryEmail200Response**](VerifySecondaryEmail200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Email verified successfully |  -  |
**400** | Invalid or expired token |  -  |
**404** | UUID not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

