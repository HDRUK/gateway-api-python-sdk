# gateway_api_sdk.DarIntegrationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dar_integration**](DarIntegrationApi.md#create_dar_integration) | **POST** /api/v1/dar-integration/{id} | DarIntegration@store
[**delete_dar_integration**](DarIntegrationApi.md#delete_dar_integration) | **DELETE** /api/v1/dar-integrations/{id} | DarIntegration@destroy
[**edit_dar_integration**](DarIntegrationApi.md#edit_dar_integration) | **PATCH** /api/v1/dar-integration/{id} | DarIntegration@edit
[**fetch_all_dar_integrations**](DarIntegrationApi.md#fetch_all_dar_integrations) | **GET** /api/v1/dar-integration | DarIntegration@index
[**fetch_dar_integration**](DarIntegrationApi.md#fetch_dar_integration) | **GET** /api/v1/dar-integration/{id} | DarIntegration@show
[**update_dar_integration**](DarIntegrationApi.md#update_dar_integration) | **PUT** /api/v1/dar-integration/{id} | DarIntegration@update


# **create_dar_integration**
> CreateCategories200Response create_dar_integration(id, update_dar_integration_request)

DarIntegration@store

Creates a new DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.update_dar_integration_request import UpdateDarIntegrationRequest
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id
    update_dar_integration_request = gateway_api_sdk.UpdateDarIntegrationRequest() # UpdateDarIntegrationRequest | DarIntegration definition

    try:
        # DarIntegration@store
        api_response = api_instance.create_dar_integration(id, update_dar_integration_request)
        print("The response of DarIntegrationApi->create_dar_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->create_dar_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 
 **update_dar_integration_request** | [**UpdateDarIntegrationRequest**](UpdateDarIntegrationRequest.md)| DarIntegration definition | 

### Return type

[**CreateCategories200Response**](CreateCategories200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_dar_integration**
> DeleteAliases200Response delete_dar_integration(id)

DarIntegration@destroy

Delete a system Dar Integration

### Example

* Bearer (JWT) Authentication (bearerAuth):

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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id

    try:
        # DarIntegration@destroy
        api_response = api_instance.delete_dar_integration(id)
        print("The response of DarIntegrationApi->delete_dar_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->delete_dar_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **edit_dar_integration**
> UpdateDarIntegration200Response edit_dar_integration(id, edit_dar_integration_request)

DarIntegration@edit

Edit a DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_dar_integration_request import EditDarIntegrationRequest
from gateway_api_sdk.models.update_dar_integration200_response import UpdateDarIntegration200Response
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id
    edit_dar_integration_request = gateway_api_sdk.EditDarIntegrationRequest() # EditDarIntegrationRequest | DarIntegration definition

    try:
        # DarIntegration@edit
        api_response = api_instance.edit_dar_integration(id, edit_dar_integration_request)
        print("The response of DarIntegrationApi->edit_dar_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->edit_dar_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 
 **edit_dar_integration_request** | [**EditDarIntegrationRequest**](EditDarIntegrationRequest.md)| DarIntegration definition | 

### Return type

[**UpdateDarIntegration200Response**](UpdateDarIntegration200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_dar_integrations**
> FetchAllDarIntegrations200Response fetch_all_dar_integrations()

DarIntegration@index

Returns a list of DAR integrations enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_dar_integrations200_response import FetchAllDarIntegrations200Response
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)

    try:
        # DarIntegration@index
        api_response = api_instance.fetch_all_dar_integrations()
        print("The response of DarIntegrationApi->fetch_all_dar_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->fetch_all_dar_integrations: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllDarIntegrations200Response**](FetchAllDarIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_integration**
> FetchAllDarIntegrations200ResponseDataInner fetch_dar_integration(id)

DarIntegration@show

Returns a single DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_dar_integrations200_response_data_inner import FetchAllDarIntegrations200ResponseDataInner
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id

    try:
        # DarIntegration@show
        api_response = api_instance.fetch_dar_integration(id)
        print("The response of DarIntegrationApi->fetch_dar_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->fetch_dar_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 

### Return type

[**FetchAllDarIntegrations200ResponseDataInner**](FetchAllDarIntegrations200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**401** | Unauthorized |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_dar_integration**
> UpdateDarIntegration200Response update_dar_integration(id, update_dar_integration_request)

DarIntegration@update

Updates a DAR integration enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_dar_integration200_response import UpdateDarIntegration200Response
from gateway_api_sdk.models.update_dar_integration_request import UpdateDarIntegrationRequest
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
    api_instance = gateway_api_sdk.DarIntegrationApi(api_client)
    id = 1 # int | dar integration id
    update_dar_integration_request = gateway_api_sdk.UpdateDarIntegrationRequest() # UpdateDarIntegrationRequest | DarIntegration definition

    try:
        # DarIntegration@update
        api_response = api_instance.update_dar_integration(id, update_dar_integration_request)
        print("The response of DarIntegrationApi->update_dar_integration:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DarIntegrationApi->update_dar_integration: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dar integration id | 
 **update_dar_integration_request** | [**UpdateDarIntegrationRequest**](UpdateDarIntegrationRequest.md)| DarIntegration definition | 

### Return type

[**UpdateDarIntegration200Response**](UpdateDarIntegration200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

