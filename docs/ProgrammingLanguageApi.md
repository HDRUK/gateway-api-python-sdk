# gateway_api_sdk.ProgrammingLanguageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_programming_languages**](ProgrammingLanguageApi.md#create_programming_languages) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store
[**delete_programming_languages**](ProgrammingLanguageApi.md#delete_programming_languages) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy
[**edit_programming_languages**](ProgrammingLanguageApi.md#edit_programming_languages) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update
[**fetch_all_programming_languages**](ProgrammingLanguageApi.md#fetch_all_programming_languages) | **GET** /api/v1/programming_languages | ProgrammingLanguage@index
[**fetch_programming_languages**](ProgrammingLanguageApi.md#fetch_programming_languages) | **GET** /api/v1/programming_languages/{id} | ProgrammingLanguage@show
[**update_programming_languages**](ProgrammingLanguageApi.md#update_programming_languages) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update


# **create_programming_languages**
> CreateCategories200Response create_programming_languages(create_categories_request)

ProgrammingLanguage@store

Creates a new system programming language

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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    create_categories_request = gateway_api_sdk.CreateCategoriesRequest() # CreateCategoriesRequest | Programming language definition

    try:
        # ProgrammingLanguage@store
        api_response = api_instance.create_programming_languages(create_categories_request)
        print("The response of ProgrammingLanguageApi->create_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->create_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md)| Programming language definition | 

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

# **delete_programming_languages**
> DeleteAliases200Response delete_programming_languages(id)

ProgrammingLanguage@destroy

Delete a system programming language

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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id

    try:
        # ProgrammingLanguage@destroy
        api_response = api_instance.delete_programming_languages(id)
        print("The response of ProgrammingLanguageApi->delete_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->delete_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 

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

# **edit_programming_languages**
> UpdateProgrammingLanguages200Response edit_programming_languages(id, edit_categories_request)

ProgrammingLanguage@update

Edit a system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_categories_request import EditCategoriesRequest
from gateway_api_sdk.models.update_programming_languages200_response import UpdateProgrammingLanguages200Response
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id
    edit_categories_request = gateway_api_sdk.EditCategoriesRequest() # EditCategoriesRequest | ProgrammingLanguage definition

    try:
        # ProgrammingLanguage@update
        api_response = api_instance.edit_programming_languages(id, edit_categories_request)
        print("The response of ProgrammingLanguageApi->edit_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->edit_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 
 **edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md)| ProgrammingLanguage definition | 

### Return type

[**UpdateProgrammingLanguages200Response**](UpdateProgrammingLanguages200Response.md)

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

# **fetch_all_programming_languages**
> FetchAllProgrammingLanguages200Response fetch_all_programming_languages()

ProgrammingLanguage@index

Returns a list of programming languages enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_programming_languages200_response import FetchAllProgrammingLanguages200Response
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)

    try:
        # ProgrammingLanguage@index
        api_response = api_instance.fetch_all_programming_languages()
        print("The response of ProgrammingLanguageApi->fetch_all_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->fetch_all_programming_languages: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllProgrammingLanguages200Response**](FetchAllProgrammingLanguages200Response.md)

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

# **fetch_programming_languages**
> FetchProgrammingLanguages200Response fetch_programming_languages(id)

ProgrammingLanguage@show

Return a single system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_programming_languages200_response import FetchProgrammingLanguages200Response
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id

    try:
        # ProgrammingLanguage@show
        api_response = api_instance.fetch_programming_languages(id)
        print("The response of ProgrammingLanguageApi->fetch_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->fetch_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 

### Return type

[**FetchProgrammingLanguages200Response**](FetchProgrammingLanguages200Response.md)

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

# **update_programming_languages**
> UpdateProgrammingLanguages200Response update_programming_languages(id, update_categories_request)

ProgrammingLanguage@update

Update a system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_categories_request import UpdateCategoriesRequest
from gateway_api_sdk.models.update_programming_languages200_response import UpdateProgrammingLanguages200Response
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id
    update_categories_request = gateway_api_sdk.UpdateCategoriesRequest() # UpdateCategoriesRequest | ProgrammingLanguage definition

    try:
        # ProgrammingLanguage@update
        api_response = api_instance.update_programming_languages(id, update_categories_request)
        print("The response of ProgrammingLanguageApi->update_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->update_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 
 **update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md)| ProgrammingLanguage definition | 

### Return type

[**UpdateProgrammingLanguages200Response**](UpdateProgrammingLanguages200Response.md)

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

