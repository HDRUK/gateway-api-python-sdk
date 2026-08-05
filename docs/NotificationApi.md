# gateway_api_sdk.NotificationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_notifications**](NotificationApi.md#delete_notifications) | **DELETE** /api/v1/notifications/{id} | Notification@destroy


# **delete_notifications**
> DeleteApplications200Response delete_notifications(id)

Notification@destroy

Delete a notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_applications200_response import DeleteApplications200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id

    try:
        # Notification@destroy
        api_response = api_instance.delete_notifications(id)
        print("The response of NotificationApi->delete_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->delete_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 

### Return type

[**DeleteApplications200Response**](DeleteApplications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

