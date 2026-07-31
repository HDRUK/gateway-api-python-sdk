# gateway_api_sdk.FormHydrationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_form_schema**](FormHydrationApi.md#get_form_schema) | **GET** /api/v1/form_hydration/schema | Retrieve form schema data
[**onboarding_form_hydration**](FormHydrationApi.md#onboarding_form_hydration) | **GET** /api/v1/form_hydration | Retrieve form schema data


# **get_form_schema**
> object get_form_schema(model=model, version=version)

Retrieve form schema data

Retrieves form schema data based on the provided model and version.

### Example


```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.FormHydrationApi(api_client)
    model = 'model_example' # str | The model for which form schema is requested. (optional)
    version = 'version_example' # str | The version of the model for which form schema is requested. (optional)

    try:
        # Retrieve form schema data
        api_response = api_instance.get_form_schema(model=model, version=version)
        print("The response of FormHydrationApi->get_form_schema:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormHydrationApi->get_form_schema: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model** | **str**| The model for which form schema is requested. | [optional] 
 **version** | **str**| The version of the model for which form schema is requested. | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Bad request. Missing required parameters or invalid parameters. |  -  |
**500** | Internal server error. Failed to retrieve form schema data. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **onboarding_form_hydration**
> object onboarding_form_hydration(name=name, version=version, data_types=data_types)

Retrieve form schema data

Retrieves form schema data based on the provided model and version.

### Example


```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.FormHydrationApi(api_client)
    name = 'name_example' # str | The model name for which form schema is requested. (optional)
    version = 'version_example' # str | The version of the model for which form schema is requested. (optional)
    data_types = 'data_types_example' # str | The data types of the dataset about to be onboarded. (optional)

    try:
        # Retrieve form schema data
        api_response = api_instance.onboarding_form_hydration(name=name, version=version, data_types=data_types)
        print("The response of FormHydrationApi->onboarding_form_hydration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FormHydrationApi->onboarding_form_hydration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| The model name for which form schema is requested. | [optional] 
 **version** | **str**| The version of the model for which form schema is requested. | [optional] 
 **data_types** | **str**| The data types of the dataset about to be onboarded. | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Bad request. Missing required parameters or invalid parameters. |  -  |
**500** | Internal server error. Failed to retrieve form schema data. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

