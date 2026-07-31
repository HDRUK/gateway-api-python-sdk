# gateway_api_sdk.CustomerSatisfactionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_csat**](CustomerSatisfactionApi.md#create_csat) | **POST** /api/v1/csat | Create Customer Satisfaction Score
[**edit_csat**](CustomerSatisfactionApi.md#edit_csat) | **PATCH** /api/v1/csat/{id} | Update Customer Satisfaction Description


# **create_csat**
> DeleteAliases200Response create_csat(create_csat_request)

Create Customer Satisfaction Score

Creates a customer satisfaction score between 0 and 5

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_csat_request import CreateCsatRequest
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
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
    create_csat_request = gateway_api_sdk.CreateCsatRequest() # CreateCsatRequest | Customer Satisfaction score

    try:
        # Create Customer Satisfaction Score
        api_response = api_instance.create_csat(create_csat_request)
        print("The response of CustomerSatisfactionApi->create_csat:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerSatisfactionApi->create_csat: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_csat_request** | [**CreateCsatRequest**](CreateCsatRequest.md)| Customer Satisfaction score | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **edit_csat**
> EditCsat200Response edit_csat(id, edit_csat_request)

Update Customer Satisfaction Description

Update a description for a satisfaction score entry

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_csat200_response import EditCsat200Response
from gateway_api_sdk.models.edit_csat_request import EditCsatRequest
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
    edit_csat_request = gateway_api_sdk.EditCsatRequest() # EditCsatRequest | Reason to update

    try:
        # Update Customer Satisfaction Description
        api_response = api_instance.edit_csat(id, edit_csat_request)
        print("The response of CustomerSatisfactionApi->edit_csat:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustomerSatisfactionApi->edit_csat: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the CSAT entry | 
 **edit_csat_request** | [**EditCsatRequest**](EditCsatRequest.md)| Reason to update | 

### Return type

[**EditCsat200Response**](EditCsat200Response.md)

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

