# gateway_api_sdk.IntegrationDataUseRegistersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dur_integrations**](IntegrationDataUseRegistersApi.md#create_dur_integrations) | **POST** /api/v1/integrations/dur | IntegrationDurController@store
[**delete_dur_integrations**](IntegrationDataUseRegistersApi.md#delete_dur_integrations) | **DELETE** /api/v1/integrations/dur/{id} | Delete a dur
[**edit_dur_integrations**](IntegrationDataUseRegistersApi.md#edit_dur_integrations) | **PATCH** /api/v1/integrations/dur/{id} | Edit a dur
[**fetch_all_dur_integrations**](IntegrationDataUseRegistersApi.md#fetch_all_dur_integrations) | **GET** /api/v1/integrations/dur | IntegrationDurController@index
[**fetch_dur_by_id_integrations**](IntegrationDataUseRegistersApi.md#fetch_dur_by_id_integrations) | **GET** /api/v1/integrations/dur/{id} | IntegrationDurController@show
[**update_dur_integrations**](IntegrationDataUseRegistersApi.md#update_dur_integrations) | **PUT** /api/v1/integrations/dur/{id} | Update a dur by id


# **create_dur_integrations**
> CreateCategories200Response create_dur_integrations(create_dur_integrations_request)

IntegrationDurController@store

Create a new dur

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_dur_integrations_request import CreateDurIntegrationsRequest
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
    api_instance = gateway_api_sdk.IntegrationDataUseRegistersApi(api_client)
    create_dur_integrations_request = gateway_api_sdk.CreateDurIntegrationsRequest() # CreateDurIntegrationsRequest | Pass user credentials

    try:
        # IntegrationDurController@store
        api_response = api_instance.create_dur_integrations(create_dur_integrations_request)
        print("The response of IntegrationDataUseRegistersApi->create_dur_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationDataUseRegistersApi->create_dur_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_dur_integrations_request** | [**CreateDurIntegrationsRequest**](CreateDurIntegrationsRequest.md)| Pass user credentials | 

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

# **delete_dur_integrations**
> DeleteAliases200Response delete_dur_integrations(id)

Delete a dur

Delete a dur

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
    api_instance = gateway_api_sdk.IntegrationDataUseRegistersApi(api_client)
    id = 1 # int | dur id

    try:
        # Delete a dur
        api_response = api_instance.delete_dur_integrations(id)
        print("The response of IntegrationDataUseRegistersApi->delete_dur_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationDataUseRegistersApi->delete_dur_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dur id | 

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

# **edit_dur_integrations**
> UpdateDurIntegrations200Response edit_dur_integrations(id, create_dur_integrations_request)

Edit a dur

Edit a dur

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_integrations_request import CreateDurIntegrationsRequest
from gateway_api_sdk.models.update_dur_integrations200_response import UpdateDurIntegrations200Response
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
    api_instance = gateway_api_sdk.IntegrationDataUseRegistersApi(api_client)
    id = 1 # int | dur id
    create_dur_integrations_request = gateway_api_sdk.CreateDurIntegrationsRequest() # CreateDurIntegrationsRequest | Pass user credentials

    try:
        # Edit a dur
        api_response = api_instance.edit_dur_integrations(id, create_dur_integrations_request)
        print("The response of IntegrationDataUseRegistersApi->edit_dur_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationDataUseRegistersApi->edit_dur_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dur id | 
 **create_dur_integrations_request** | [**CreateDurIntegrationsRequest**](CreateDurIntegrationsRequest.md)| Pass user credentials | 

### Return type

[**UpdateDurIntegrations200Response**](UpdateDurIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_dur_integrations**
> FetchAllDurIntegrations200Response fetch_all_dur_integrations(sort=sort, per_page=per_page)

IntegrationDurController@index

Returns a list of dur

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_dur_integrations200_response import FetchAllDurIntegrations200Response
from gateway_api_sdk.models.project_title_ascupdated_at_asc import ProjectTitleAscupdatedAtAsc
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
    api_instance = gateway_api_sdk.IntegrationDataUseRegistersApi(api_client)
    sort = gateway_api_sdk.ProjectTitleAscupdatedAtAsc() # ProjectTitleAscupdatedAtAsc | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc (optional)
    per_page = 1 # int | per page (optional)

    try:
        # IntegrationDurController@index
        api_response = api_instance.fetch_all_dur_integrations(sort=sort, per_page=per_page)
        print("The response of IntegrationDataUseRegistersApi->fetch_all_dur_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationDataUseRegistersApi->fetch_all_dur_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sort** | [**ProjectTitleAscupdatedAtAsc**](.md)| Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc | [optional] 
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchAllDurIntegrations200Response**](FetchAllDurIntegrations200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dur_by_id_integrations**
> FetchDurByIdIntegrations200Response fetch_dur_by_id_integrations(id)

IntegrationDurController@show

Get dur by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dur_by_id_integrations200_response import FetchDurByIdIntegrations200Response
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
    api_instance = gateway_api_sdk.IntegrationDataUseRegistersApi(api_client)
    id = 1 # int | data use register id

    try:
        # IntegrationDurController@show
        api_response = api_instance.fetch_dur_by_id_integrations(id)
        print("The response of IntegrationDataUseRegistersApi->fetch_dur_by_id_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationDataUseRegistersApi->fetch_dur_by_id_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| data use register id | 

### Return type

[**FetchDurByIdIntegrations200Response**](FetchDurByIdIntegrations200Response.md)

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

# **update_dur_integrations**
> UpdateDurIntegrations200Response update_dur_integrations(id, create_dur_integrations_request)

Update a dur by id

Update a dur

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_integrations_request import CreateDurIntegrationsRequest
from gateway_api_sdk.models.update_dur_integrations200_response import UpdateDurIntegrations200Response
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
    api_instance = gateway_api_sdk.IntegrationDataUseRegistersApi(api_client)
    id = 1 # int | dur id
    create_dur_integrations_request = gateway_api_sdk.CreateDurIntegrationsRequest() # CreateDurIntegrationsRequest | Pass user credentials

    try:
        # Update a dur by id
        api_response = api_instance.update_dur_integrations(id, create_dur_integrations_request)
        print("The response of IntegrationDataUseRegistersApi->update_dur_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationDataUseRegistersApi->update_dur_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dur id | 
 **create_dur_integrations_request** | [**CreateDurIntegrationsRequest**](CreateDurIntegrationsRequest.md)| Pass user credentials | 

### Return type

[**UpdateDurIntegrations200Response**](UpdateDurIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

