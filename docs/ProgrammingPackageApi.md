# gateway_api_sdk.ProgrammingPackageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_programming_packages**](ProgrammingPackageApi.md#create_programming_packages) | **POST** /api/v1/programming_packages | ProgrammingPackage@store
[**delete_programming_packages**](ProgrammingPackageApi.md#delete_programming_packages) | **DELETE** /api/v1/programming_packages/{id} | ProgrammingPackage@destroy
[**edit_programming_packages**](ProgrammingPackageApi.md#edit_programming_packages) | **PATCH** /api/v1/programming_packages/{id} | ProgrammingPackage@update
[**fetch_all_programming_packages**](ProgrammingPackageApi.md#fetch_all_programming_packages) | **GET** /api/v1/programming_packages | ProgrammingPackage@index
[**fetch_programming_packages**](ProgrammingPackageApi.md#fetch_programming_packages) | **GET** /api/v1/programming_packages/{id} | ProgrammingPackage@show
[**update_programming_packages**](ProgrammingPackageApi.md#update_programming_packages) | **PUT** /api/v1/programming_packages/{id} | ProgrammingPackage@update


# **create_programming_packages**
> CreateCategories200Response create_programming_packages(create_categories_request)

ProgrammingPackage@store

Creates a new system programming package

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_categories_request import CreateCategoriesRequest
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    create_categories_request = gateway_api_sdk.CreateCategoriesRequest() # CreateCategoriesRequest | Programming package definition

    try:
        # ProgrammingPackage@store
        api_response = api_instance.create_programming_packages(create_categories_request)
        print("The response of ProgrammingPackageApi->create_programming_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->create_programming_packages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md)| Programming package definition | 

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

# **delete_programming_packages**
> DeleteAliases200Response delete_programming_packages(id)

ProgrammingPackage@destroy

Delete a system programming package

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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id

    try:
        # ProgrammingPackage@destroy
        api_response = api_instance.delete_programming_packages(id)
        print("The response of ProgrammingPackageApi->delete_programming_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->delete_programming_packages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 

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

# **edit_programming_packages**
> UpdateProgrammingPackages200Response edit_programming_packages(id, edit_categories_request)

ProgrammingPackage@update

Edit a system programming package

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_categories_request import EditCategoriesRequest
from gateway_api_sdk.models.update_programming_packages200_response import UpdateProgrammingPackages200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id
    edit_categories_request = gateway_api_sdk.EditCategoriesRequest() # EditCategoriesRequest | ProgrammingPackage definition

    try:
        # ProgrammingPackage@update
        api_response = api_instance.edit_programming_packages(id, edit_categories_request)
        print("The response of ProgrammingPackageApi->edit_programming_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->edit_programming_packages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 
 **edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md)| ProgrammingPackage definition | 

### Return type

[**UpdateProgrammingPackages200Response**](UpdateProgrammingPackages200Response.md)

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

# **fetch_all_programming_packages**
> FetchAllProgrammingPackages200Response fetch_all_programming_packages()

ProgrammingPackage@index

Returns a list of programming packages enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_programming_packages200_response import FetchAllProgrammingPackages200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)

    try:
        # ProgrammingPackage@index
        api_response = api_instance.fetch_all_programming_packages()
        print("The response of ProgrammingPackageApi->fetch_all_programming_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->fetch_all_programming_packages: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllProgrammingPackages200Response**](FetchAllProgrammingPackages200Response.md)

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

# **fetch_programming_packages**
> FetchProgrammingPackages200Response fetch_programming_packages(id)

ProgrammingPackage@show

Return a single system programming package

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_programming_packages200_response import FetchProgrammingPackages200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id

    try:
        # ProgrammingPackage@show
        api_response = api_instance.fetch_programming_packages(id)
        print("The response of ProgrammingPackageApi->fetch_programming_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->fetch_programming_packages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 

### Return type

[**FetchProgrammingPackages200Response**](FetchProgrammingPackages200Response.md)

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

# **update_programming_packages**
> UpdateProgrammingPackages200Response update_programming_packages(id, update_categories_request)

ProgrammingPackage@update

Update a system programming package

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_categories_request import UpdateCategoriesRequest
from gateway_api_sdk.models.update_programming_packages200_response import UpdateProgrammingPackages200Response
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
    api_instance = gateway_api_sdk.ProgrammingPackageApi(api_client)
    id = 1 # int | programming package id
    update_categories_request = gateway_api_sdk.UpdateCategoriesRequest() # UpdateCategoriesRequest | ProgrammingPackage definition

    try:
        # ProgrammingPackage@update
        api_response = api_instance.update_programming_packages(id, update_categories_request)
        print("The response of ProgrammingPackageApi->update_programming_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingPackageApi->update_programming_packages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming package id | 
 **update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md)| ProgrammingPackage definition | 

### Return type

[**UpdateProgrammingPackages200Response**](UpdateProgrammingPackages200Response.md)

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

