# gateway_api_sdk.CustomerSatisfactionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_2e155418e5f0de41829414447919439e**](CustomerSatisfactionApi.md#call_2e155418e5f0de41829414447919439e) | **PATCH** /api/v1/csat/{id} | Update Customer Satisfaction Description
[**call_3604171bd1ea2588906fe1cf65353366**](CustomerSatisfactionApi.md#call_3604171bd1ea2588906fe1cf65353366) | **POST** /api/v1/csat | Create Customer Satisfaction Score


# **call_2e155418e5f0de41829414447919439e**
> Model2e155418e5f0de41829414447919439e200Response call_2e155418e5f0de41829414447919439e(id, model2e155418e5f0de41829414447919439e_request)

Update Customer Satisfaction Description

Update a description for a satisfaction score entry

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model2e155418e5f0de41829414447919439e200_response import Model2e155418e5f0de41829414447919439e200Response
from gateway_api_sdk.models.model2e155418e5f0de41829414447919439e_request import Model2e155418e5f0de41829414447919439eRequest
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
    api_instance = gateway_api_sdk.CustomerSatisfactionApi(api_client)
    id = 56 # int | ID of the CSAT entry
    model2e155418e5f0de41829414447919439e_request = gateway_api_sdk.Model2e155418e5f0de41829414447919439eRequest() # Model2e155418e5f0de41829414447919439eRequest | Reason to update

    try:
        # Update Customer Satisfaction Description
        api_response = api_instance.call_2e155418e5f0de41829414447919439e(id, model2e155418e5f0de41829414447919439e_request)
        print("The response of CustomerSatisfactionApi->call_2e155418e5f0de41829414447919439e:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerSatisfactionApi->call_2e155418e5f0de41829414447919439e: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the CSAT entry | 
 **model2e155418e5f0de41829414447919439e_request** | [**Model2e155418e5f0de41829414447919439eRequest**](Model2e155418e5f0de41829414447919439eRequest.md)| Reason to update | 

### Return type

[**Model2e155418e5f0de41829414447919439e200Response**](Model2e155418e5f0de41829414447919439e200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Update successful |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_3604171bd1ea2588906fe1cf65353366**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_3604171bd1ea2588906fe1cf65353366(model3604171bd1ea2588906fe1cf65353366_request)

Create Customer Satisfaction Score

Creates a customer satisfaction score between 0 and 5

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
from gateway_api_sdk.models.model3604171bd1ea2588906fe1cf65353366_request import Model3604171bd1ea2588906fe1cf65353366Request
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
    api_instance = gateway_api_sdk.CustomerSatisfactionApi(api_client)
    model3604171bd1ea2588906fe1cf65353366_request = gateway_api_sdk.Model3604171bd1ea2588906fe1cf65353366Request() # Model3604171bd1ea2588906fe1cf65353366Request | Customer Satisfaction score

    try:
        # Create Customer Satisfaction Score
        api_response = api_instance.call_3604171bd1ea2588906fe1cf65353366(model3604171bd1ea2588906fe1cf65353366_request)
        print("The response of CustomerSatisfactionApi->call_3604171bd1ea2588906fe1cf65353366:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerSatisfactionApi->call_3604171bd1ea2588906fe1cf65353366: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model3604171bd1ea2588906fe1cf65353366_request** | [**Model3604171bd1ea2588906fe1cf65353366Request**](Model3604171bd1ea2588906fe1cf65353366Request.md)| Customer Satisfaction score | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Resource Created |  -  |
**422** | Validation Error |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

