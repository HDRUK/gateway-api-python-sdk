# gateway_api_sdk.IntegrationCollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_collections_integrations**](IntegrationCollectionsApi.md#create_collections_integrations) | **POST** /api/v1/integrations/collections | IntegrationCollectionController@store
[**delete_collections_integrations**](IntegrationCollectionsApi.md#delete_collections_integrations) | **DELETE** /api/v1/integrations/collections/{id} | Delete a collection
[**edit_collections_integrations**](IntegrationCollectionsApi.md#edit_collections_integrations) | **PATCH** /api/v1/integrations/collections/{id} | Edit a collection
[**fetch_all_collections_integrations**](IntegrationCollectionsApi.md#fetch_all_collections_integrations) | **GET** /api/v1/integrations/collections | IntegrationCollectionController@index
[**fetch_collections_integrations**](IntegrationCollectionsApi.md#fetch_collections_integrations) | **GET** /api/v1/integrations/collections/{id} | IntegrationCollectionController@show
[**update_collections_integrations**](IntegrationCollectionsApi.md#update_collections_integrations) | **PUT** /api/v1/integrations/collections/{id} | Update a collection


# **create_collections_integrations**
> CreateDarIntegration201Response create_collections_integrations(create_collections_integrations_request)

IntegrationCollectionController@store

Create a new collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_collections_integrations_request import CreateCollectionsIntegrationsRequest
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    create_collections_integrations_request = gateway_api_sdk.CreateCollectionsIntegrationsRequest() # CreateCollectionsIntegrationsRequest | Pass user credentials

    try:
        # IntegrationCollectionController@store
        api_response = api_instance.create_collections_integrations(create_collections_integrations_request)
        print("The response of IntegrationCollectionsApi->create_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->create_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_collections_integrations_request** | [**CreateCollectionsIntegrationsRequest**](CreateCollectionsIntegrationsRequest.md)| Pass user credentials | 

### Return type

[**CreateDarIntegration201Response**](CreateDarIntegration201Response.md)

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

# **delete_collections_integrations**
> DeleteApplications200Response delete_collections_integrations(id)

Delete a collection

Delete a collection

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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id

    try:
        # Delete a collection
        api_response = api_instance.delete_collections_integrations(id)
        print("The response of IntegrationCollectionsApi->delete_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->delete_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 

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

# **edit_collections_integrations**
> FetchCollections200Response edit_collections_integrations(id, create_collections_integrations_request)

Edit a collection

Edit a collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_collections_integrations_request import CreateCollectionsIntegrationsRequest
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id
    create_collections_integrations_request = gateway_api_sdk.CreateCollectionsIntegrationsRequest() # CreateCollectionsIntegrationsRequest | Pass user credentials

    try:
        # Edit a collection
        api_response = api_instance.edit_collections_integrations(id, create_collections_integrations_request)
        print("The response of IntegrationCollectionsApi->edit_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->edit_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **create_collections_integrations_request** | [**CreateCollectionsIntegrationsRequest**](CreateCollectionsIntegrationsRequest.md)| Pass user credentials | 

### Return type

[**FetchCollections200Response**](FetchCollections200Response.md)

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

# **fetch_all_collections_integrations**
> FetchAllCollections200Response fetch_all_collections_integrations(name=name, per_page=per_page)

IntegrationCollectionController@index

Returns a list of collections

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_collections200_response import FetchAllCollections200Response
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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    name = 'name_example' # str | Filter collections by name (optional)
    per_page = 1 # int | per page (optional)

    try:
        # IntegrationCollectionController@index
        api_response = api_instance.fetch_all_collections_integrations(name=name, per_page=per_page)
        print("The response of IntegrationCollectionsApi->fetch_all_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->fetch_all_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Filter collections by name | [optional] 
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchAllCollections200Response**](FetchAllCollections200Response.md)

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

# **fetch_collections_integrations**
> FetchCollections200Response fetch_collections_integrations(id)

IntegrationCollectionController@show

Get collection by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id

    try:
        # IntegrationCollectionController@show
        api_response = api_instance.fetch_collections_integrations(id)
        print("The response of IntegrationCollectionsApi->fetch_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->fetch_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 

### Return type

[**FetchCollections200Response**](FetchCollections200Response.md)

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

# **update_collections_integrations**
> FetchCollections200Response update_collections_integrations(id, create_collections_integrations_request)

Update a collection

Update a collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_collections_integrations_request import CreateCollectionsIntegrationsRequest
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id
    create_collections_integrations_request = gateway_api_sdk.CreateCollectionsIntegrationsRequest() # CreateCollectionsIntegrationsRequest | Pass user credentials

    try:
        # Update a collection
        api_response = api_instance.update_collections_integrations(id, create_collections_integrations_request)
        print("The response of IntegrationCollectionsApi->update_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->update_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **create_collections_integrations_request** | [**CreateCollectionsIntegrationsRequest**](CreateCollectionsIntegrationsRequest.md)| Pass user credentials | 

### Return type

[**FetchCollections200Response**](FetchCollections200Response.md)

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

