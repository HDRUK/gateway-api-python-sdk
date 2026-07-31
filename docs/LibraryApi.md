# gateway_api_sdk.LibraryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_libraries**](LibraryApi.md#create_libraries) | **POST** /api/v1/libraries | Library@store
[**delete_libraries**](LibraryApi.md#delete_libraries) | **DELETE** /api/v1/libraries/{id} | Library@destroy
[**edit_libraries**](LibraryApi.md#edit_libraries) | **PATCH** /api/v1/libraries/{id} | Library@update
[**fetch_libraries**](LibraryApi.md#fetch_libraries) | **GET** /api/v1/libraries/{id} | Return a single library
[**list_libraries**](LibraryApi.md#list_libraries) | **GET** /api/v1/libraries | Retrieve a list of libraries
[**update_libraries**](LibraryApi.md#update_libraries) | **PUT** /api/v1/libraries/{id} | Library@update


# **create_libraries**
> CreateCategories200Response create_libraries(create_libraries_request)

Library@store

Creates a new library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_libraries_request import CreateLibrariesRequest
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    create_libraries_request = gateway_api_sdk.CreateLibrariesRequest() # CreateLibrariesRequest | library definition

    try:
        # Library@store
        api_response = api_instance.create_libraries(create_libraries_request)
        print("The response of LibraryApi->create_libraries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->create_libraries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_libraries_request** | [**CreateLibrariesRequest**](CreateLibrariesRequest.md)| library definition | 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_libraries**
> DeleteAliases200Response delete_libraries(id)

Library@destroy

Delete a library

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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id

    try:
        # Library@destroy
        api_response = api_instance.delete_libraries(id)
        print("The response of LibraryApi->delete_libraries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->delete_libraries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 

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

# **edit_libraries**
> UpdateLibraries200Response edit_libraries(id, create_libraries_request)

Library@update

Edit a library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_libraries_request import CreateLibrariesRequest
from gateway_api_sdk.models.update_libraries200_response import UpdateLibraries200Response
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id
    create_libraries_request = gateway_api_sdk.CreateLibrariesRequest() # CreateLibrariesRequest | library definition

    try:
        # Library@update
        api_response = api_instance.edit_libraries(id, create_libraries_request)
        print("The response of LibraryApi->edit_libraries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->edit_libraries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 
 **create_libraries_request** | [**CreateLibrariesRequest**](CreateLibrariesRequest.md)| library definition | 

### Return type

[**UpdateLibraries200Response**](UpdateLibraries200Response.md)

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

# **fetch_libraries**
> FetchLibraries200Response fetch_libraries(id)

Return a single library

Return a single library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_libraries200_response import FetchLibraries200Response
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id

    try:
        # Return a single library
        api_response = api_instance.fetch_libraries(id)
        print("The response of LibraryApi->fetch_libraries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->fetch_libraries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 

### Return type

[**FetchLibraries200Response**](FetchLibraries200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_libraries**
> ListLibraries200Response list_libraries(per_page=per_page)

Retrieve a list of libraries

Returns a paginated list of libraries along with associated datasets and teams.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.list_libraries200_response import ListLibraries200Response
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    per_page = 10 # int | Specify the number of libraries per page (optional) (default to 10)

    try:
        # Retrieve a list of libraries
        api_response = api_instance.list_libraries(per_page=per_page)
        print("The response of LibraryApi->list_libraries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->list_libraries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| Specify the number of libraries per page | [optional] [default to 10]

### Return type

[**ListLibraries200Response**](ListLibraries200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_libraries**
> UpdateLibraries200Response update_libraries(id, create_libraries_request)

Library@update

Update a library

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_libraries_request import CreateLibrariesRequest
from gateway_api_sdk.models.update_libraries200_response import UpdateLibraries200Response
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
    api_instance = gateway_api_sdk.LibraryApi(api_client)
    id = 1 # int | library id
    create_libraries_request = gateway_api_sdk.CreateLibrariesRequest() # CreateLibrariesRequest | library definition

    try:
        # Library@update
        api_response = api_instance.update_libraries(id, create_libraries_request)
        print("The response of LibraryApi->update_libraries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LibraryApi->update_libraries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| library id | 
 **create_libraries_request** | [**CreateLibrariesRequest**](CreateLibrariesRequest.md)| library definition | 

### Return type

[**UpdateLibraries200Response**](UpdateLibraries200Response.md)

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

