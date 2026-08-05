# gateway_api_sdk.ToolsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_unique_fields_tools**](ToolsApi.md#count_unique_fields_tools) | **GET** /api/v1/tools/count/{field} | ToolController@count
[**create_tools**](ToolsApi.md#create_tools) | **POST** /api/v1/tools | ToolController@store
[**create_tools_by_team_v2**](ToolsApi.md#create_tools_by_team_v2) | **POST** /api/v2/teams/{teamId}/tools | ToolController@store
[**create_tools_integrations**](ToolsApi.md#create_tools_integrations) | **POST** /api/v1/integrations/tools | IntegrationToolController@store
[**delete_tools**](ToolsApi.md#delete_tools) | **DELETE** /api/v1/tools/{id} | ToolController@destroy
[**delete_tools_by_teamid_v2**](ToolsApi.md#delete_tools_by_teamid_v2) | **DELETE** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@destroy
[**delete_tools_integrations**](ToolsApi.md#delete_tools_integrations) | **DELETE** /api/v1/integrations/tools/{id} | IntegrationToolController@destroy
[**edit_tools**](ToolsApi.md#edit_tools) | **PATCH** /api/v1/tools/{id} | ToolController@edit
[**edit_tools_by_teamid_v2**](ToolsApi.md#edit_tools_by_teamid_v2) | **PATCH** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@edit
[**edit_tools_integrations**](ToolsApi.md#edit_tools_integrations) | **PATCH** /api/v1/integrations/tools/{id} | IntegrationToolController@edit
[**fetch_all_tools**](ToolsApi.md#fetch_all_tools) | **GET** /api/v1/tools | Fetch all tools
[**fetch_all_tools_integrations**](ToolsApi.md#fetch_all_tools_integrations) | **GET** /api/v1/integrations/tools | IntegrationToolController@index
[**fetch_all_tools_v2**](ToolsApi.md#fetch_all_tools_v2) | **GET** /api/v2/tools | ToolController@indexActive
[**fetch_tools**](ToolsApi.md#fetch_tools) | **GET** /api/v1/tools/{id} | ToolController@show
[**fetch_tools_integrations**](ToolsApi.md#fetch_tools_integrations) | **GET** /api/v1/integrations/tools/{id} | IntegrationToolController@show
[**fetch_tools_v2**](ToolsApi.md#fetch_tools_v2) | **GET** /api/v2/tools/{id} | ToolController@showActive
[**update_tools**](ToolsApi.md#update_tools) | **PUT** /api/v1/tools/{id} | ToolController@update
[**update_tools_by_teamid_v2**](ToolsApi.md#update_tools_by_teamid_v2) | **PUT** /api/v2/teams/{teamId}/tools/{id} | TeamToolController@update
[**update_tools_integrations**](ToolsApi.md#update_tools_integrations) | **PUT** /api/v1/integrations/tools/{id} | IntegrationToolController@update


# **count_unique_fields_tools**
> CountUniqueFieldsCollections200Response count_unique_fields_tools(var_field, team_id)

ToolController@count

Get Counts for distinct entries of a field in the model

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.count_unique_fields_collections200_response import CountUniqueFieldsCollections200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    var_field = 'status' # str | name of the field to perform a count on
    team_id = 1 # int | team id

    try:
        # ToolController@count
        api_response = api_instance.count_unique_fields_tools(var_field, team_id)
        print("The response of ToolsApi->count_unique_fields_tools:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->count_unique_fields_tools: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_field** | **str**| name of the field to perform a count on | 
 **team_id** | **int**| team id | 

### Return type

[**CountUniqueFieldsCollections200Response**](CountUniqueFieldsCollections200Response.md)

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

# **create_tools**
> CreateDarIntegration201Response create_tools(create_tools_request)

ToolController@store

Create a new tool

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
from gateway_api_sdk.models.create_tools_request import CreateToolsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    create_tools_request = gateway_api_sdk.CreateToolsRequest() # CreateToolsRequest | Pass user credentials

    try:
        # ToolController@store
        api_response = api_instance.create_tools(create_tools_request)
        print("The response of ToolsApi->create_tools:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->create_tools: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_tools_request** | [**CreateToolsRequest**](CreateToolsRequest.md)| Pass user credentials | 

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
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_tools_by_team_v2**
> CreateDarIntegration201Response create_tools_by_team_v2(team_id, create_tools_request)

ToolController@store

Create a new tool by team v2

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
from gateway_api_sdk.models.create_tools_request import CreateToolsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    team_id = 1 # int | team id
    create_tools_request = gateway_api_sdk.CreateToolsRequest() # CreateToolsRequest | Pass user credentials

    try:
        # ToolController@store
        api_response = api_instance.create_tools_by_team_v2(team_id, create_tools_request)
        print("The response of ToolsApi->create_tools_by_team_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->create_tools_by_team_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **create_tools_request** | [**CreateToolsRequest**](CreateToolsRequest.md)| Pass user credentials | 

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
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_tools_integrations**
> CreateDarIntegration201Response create_tools_integrations(create_tools_integrations_request)

IntegrationToolController@store

Create a new tool

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
from gateway_api_sdk.models.create_tools_integrations_request import CreateToolsIntegrationsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    create_tools_integrations_request = gateway_api_sdk.CreateToolsIntegrationsRequest() # CreateToolsIntegrationsRequest | Pass user credentials

    try:
        # IntegrationToolController@store
        api_response = api_instance.create_tools_integrations(create_tools_integrations_request)
        print("The response of ToolsApi->create_tools_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->create_tools_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_tools_integrations_request** | [**CreateToolsIntegrationsRequest**](CreateToolsIntegrationsRequest.md)| Pass user credentials | 

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
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_tools**
> DeleteFederation200Response delete_tools(id)

ToolController@destroy

Delete tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_federation200_response import DeleteFederation200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id

    try:
        # ToolController@destroy
        api_response = api_instance.delete_tools(id)
        print("The response of ToolsApi->delete_tools:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->delete_tools: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 

### Return type

[**DeleteFederation200Response**](DeleteFederation200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Error response |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_tools_by_teamid_v2**
> DeleteFederation200Response delete_tools_by_teamid_v2(team_id, id)

TeamToolController@destroy

Delete tool by id and by team_id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_federation200_response import DeleteFederation200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | tool id

    try:
        # TeamToolController@destroy
        api_response = api_instance.delete_tools_by_teamid_v2(team_id, id)
        print("The response of ToolsApi->delete_tools_by_teamid_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->delete_tools_by_teamid_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| tool id | 

### Return type

[**DeleteFederation200Response**](DeleteFederation200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Error response |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_tools_integrations**
> DeleteFederation200Response delete_tools_integrations(id)

IntegrationToolController@destroy

Delete tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_federation200_response import DeleteFederation200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id

    try:
        # IntegrationToolController@destroy
        api_response = api_instance.delete_tools_integrations(id)
        print("The response of ToolsApi->delete_tools_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->delete_tools_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 

### Return type

[**DeleteFederation200Response**](DeleteFederation200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Error response |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_tools**
> FetchToolsIntegrations200Response edit_tools(id, update_tools_request, unarchive=unarchive)

ToolController@edit

Edit tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
from gateway_api_sdk.models.update_tools_request import UpdateToolsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id
    update_tools_request = gateway_api_sdk.UpdateToolsRequest() # UpdateToolsRequest | Pass user credentials
    unarchive = 'unarchive_example' # str | Unarchive a tool (optional)

    try:
        # ToolController@edit
        api_response = api_instance.edit_tools(id, update_tools_request, unarchive=unarchive)
        print("The response of ToolsApi->edit_tools:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->edit_tools: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 
 **update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md)| Pass user credentials | 
 **unarchive** | **str**| Unarchive a tool | [optional] 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_tools_by_teamid_v2**
> FetchToolsIntegrations200Response edit_tools_by_teamid_v2(team_id, id, update_tools_request)

TeamToolController@edit

Edit tool by id and by teamid

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
from gateway_api_sdk.models.update_tools_request import UpdateToolsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | tool id
    update_tools_request = gateway_api_sdk.UpdateToolsRequest() # UpdateToolsRequest | Pass user credentials

    try:
        # TeamToolController@edit
        api_response = api_instance.edit_tools_by_teamid_v2(team_id, id, update_tools_request)
        print("The response of ToolsApi->edit_tools_by_teamid_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->edit_tools_by_teamid_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| tool id | 
 **update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md)| Pass user credentials | 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_tools_integrations**
> FetchToolsIntegrations200Response edit_tools_integrations(id, update_tools_integrations_request)

IntegrationToolController@edit

Edit tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
from gateway_api_sdk.models.update_tools_integrations_request import UpdateToolsIntegrationsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id
    update_tools_integrations_request = gateway_api_sdk.UpdateToolsIntegrationsRequest() # UpdateToolsIntegrationsRequest | Pass user credentials

    try:
        # IntegrationToolController@edit
        api_response = api_instance.edit_tools_integrations(id, update_tools_integrations_request)
        print("The response of ToolsApi->edit_tools_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->edit_tools_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 
 **update_tools_integrations_request** | [**UpdateToolsIntegrationsRequest**](UpdateToolsIntegrationsRequest.md)| Pass user credentials | 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_tools**
> FetchAllTools200Response fetch_all_tools(mongo_id=mongo_id, team_id=team_id, user_id=user_id, title=title, sort=sort)

Fetch all tools

Get all tools with optional filters and sorting

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_tools200_response import FetchAllTools200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    mongo_id = 'mongo_id_example' # str | Filter tools by mongo ID (optional)
    team_id = 56 # int | Filter tools by team ID (optional)
    user_id = 56 # int | Filter tools by user ID (optional)
    title = 'title_example' # str | Filter tools by title (optional)
    sort = 'name:asc' # str | Sort tools by a specific field and direction, e.g., 'name:asc' or 'created_at:desc' (optional)

    try:
        # Fetch all tools
        api_response = api_instance.fetch_all_tools(mongo_id=mongo_id, team_id=team_id, user_id=user_id, title=title, sort=sort)
        print("The response of ToolsApi->fetch_all_tools:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->fetch_all_tools: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mongo_id** | **str**| Filter tools by mongo ID | [optional] 
 **team_id** | **int**| Filter tools by team ID | [optional] 
 **user_id** | **int**| Filter tools by user ID | [optional] 
 **title** | **str**| Filter tools by title | [optional] 
 **sort** | **str**| Sort tools by a specific field and direction, e.g., &#39;name:asc&#39; or &#39;created_at:desc&#39; | [optional] 

### Return type

[**FetchAllTools200Response**](FetchAllTools200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Bad request response |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_tools_integrations**
> FetchAllToolsIntegrations200Response fetch_all_tools_integrations()

IntegrationToolController@index

Get All Tools

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_tools_integrations200_response import FetchAllToolsIntegrations200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)

    try:
        # IntegrationToolController@index
        api_response = api_instance.fetch_all_tools_integrations()
        print("The response of ToolsApi->fetch_all_tools_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->fetch_all_tools_integrations: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllToolsIntegrations200Response**](FetchAllToolsIntegrations200Response.md)

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

# **fetch_all_tools_v2**
> FetchAllTools200Response fetch_all_tools_v2(name=name, sort=sort)

ToolController@indexActive

Get all tools with optional filters and sorting

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_tools200_response import FetchAllTools200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    name = 'name_example' # str | Filter tools by name (optional)
    sort = 'name:asc' # str | Sort tools by a specific field and direction, e.g., 'name:asc' or 'created_at:desc' (optional)

    try:
        # ToolController@indexActive
        api_response = api_instance.fetch_all_tools_v2(name=name, sort=sort)
        print("The response of ToolsApi->fetch_all_tools_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->fetch_all_tools_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Filter tools by name | [optional] 
 **sort** | **str**| Sort tools by a specific field and direction, e.g., &#39;name:asc&#39; or &#39;created_at:desc&#39; | [optional] 

### Return type

[**FetchAllTools200Response**](FetchAllTools200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Bad request response |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_tools**
> FetchToolsIntegrations200Response fetch_tools(id, view_type=view_type)

ToolController@show

Get tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id
    view_type = 'full' # str | Query flag to show full tool data or a trimmed version (defaults to full). (optional) (default to 'full')

    try:
        # ToolController@show
        api_response = api_instance.fetch_tools(id, view_type=view_type)
        print("The response of ToolsApi->fetch_tools:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->fetch_tools: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 
 **view_type** | **str**| Query flag to show full tool data or a trimmed version (defaults to full). | [optional] [default to &#39;full&#39;]

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**401** | Unauthorized |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_tools_integrations**
> FetchToolsIntegrations200Response fetch_tools_integrations(id)

IntegrationToolController@show

Get tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id

    try:
        # IntegrationToolController@show
        api_response = api_instance.fetch_tools_integrations(id)
        print("The response of ToolsApi->fetch_tools_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->fetch_tools_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**401** | Unauthorized |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_tools_v2**
> FetchToolsIntegrations200Response fetch_tools_v2(id)

ToolController@showActive

Get tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id

    try:
        # ToolController@showActive
        api_response = api_instance.fetch_tools_v2(id)
        print("The response of ToolsApi->fetch_tools_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->fetch_tools_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**401** | Unauthorized |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tools**
> FetchToolsIntegrations200Response update_tools(id, update_tools_request)

ToolController@update

Update tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
from gateway_api_sdk.models.update_tools_request import UpdateToolsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id
    update_tools_request = gateway_api_sdk.UpdateToolsRequest() # UpdateToolsRequest | Pass user credentials

    try:
        # ToolController@update
        api_response = api_instance.update_tools(id, update_tools_request)
        print("The response of ToolsApi->update_tools:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->update_tools: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 
 **update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md)| Pass user credentials | 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tools_by_teamid_v2**
> FetchToolsIntegrations200Response update_tools_by_teamid_v2(team_id, id, update_tools_request)

TeamToolController@update

Update tools by team id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
from gateway_api_sdk.models.update_tools_request import UpdateToolsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | tool id
    update_tools_request = gateway_api_sdk.UpdateToolsRequest() # UpdateToolsRequest | Pass user credentials

    try:
        # TeamToolController@update
        api_response = api_instance.update_tools_by_teamid_v2(team_id, id, update_tools_request)
        print("The response of ToolsApi->update_tools_by_teamid_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->update_tools_by_teamid_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| tool id | 
 **update_tools_request** | [**UpdateToolsRequest**](UpdateToolsRequest.md)| Pass user credentials | 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_tools_integrations**
> FetchToolsIntegrations200Response update_tools_integrations(id, update_tools_integrations_request)

IntegrationToolController@update

Update tool by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_tools_integrations200_response import FetchToolsIntegrations200Response
from gateway_api_sdk.models.update_tools_integrations_request import UpdateToolsIntegrationsRequest
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
    api_instance = gateway_api_sdk.ToolsApi(api_client)
    id = 1 # int | tool id
    update_tools_integrations_request = gateway_api_sdk.UpdateToolsIntegrationsRequest() # UpdateToolsIntegrationsRequest | Pass user credentials

    try:
        # IntegrationToolController@update
        api_response = api_instance.update_tools_integrations(id, update_tools_integrations_request)
        print("The response of ToolsApi->update_tools_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ToolsApi->update_tools_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| tool id | 
 **update_tools_integrations_request** | [**UpdateToolsIntegrationsRequest**](UpdateToolsIntegrationsRequest.md)| Pass user credentials | 

### Return type

[**FetchToolsIntegrations200Response**](FetchToolsIntegrations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | bad request |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

