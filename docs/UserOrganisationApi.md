# gateway_api_sdk.UserOrganisationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_58e41162a49b5b1bf92231b359ea70cb**](UserOrganisationApi.md#call_58e41162a49b5b1bf92231b359ea70cb) | **GET** /api/v1/users/organisations | UserOrganisation@index


# **call_58e41162a49b5b1bf92231b359ea70cb**
> Model58e41162a49b5b1bf92231b359ea70cb200Response call_58e41162a49b5b1bf92231b359ea70cb()

UserOrganisation@index

Return a distinct list of all organisations which users belong to

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model58e41162a49b5b1bf92231b359ea70cb200_response import Model58e41162a49b5b1bf92231b359ea70cb200Response
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
    api_instance = gateway_api_sdk.UserOrganisationApi(api_client)

    try:
        # UserOrganisation@index
        api_response = api_instance.call_58e41162a49b5b1bf92231b359ea70cb()
        print("The response of UserOrganisationApi->call_58e41162a49b5b1bf92231b359ea70cb:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserOrganisationApi->call_58e41162a49b5b1bf92231b359ea70cb: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Model58e41162a49b5b1bf92231b359ea70cb200Response**](Model58e41162a49b5b1bf92231b359ea70cb200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

