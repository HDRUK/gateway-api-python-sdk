# gateway_api_sdk.ProgrammingLanguageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_programming_languages**](ProgrammingLanguageApi.md#create_programming_languages) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store
[**delete_programming_languages**](ProgrammingLanguageApi.md#delete_programming_languages) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy
[**edit_programming_languages**](ProgrammingLanguageApi.md#edit_programming_languages) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update
[**update_programming_languages**](ProgrammingLanguageApi.md#update_programming_languages) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update


# **create_programming_languages**
> CreateDarIntegration201Response create_programming_languages(create_programming_languages_request)

ProgrammingLanguage@store

Creates a new system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
from gateway_api_sdk.models.create_programming_languages_request import CreateProgrammingLanguagesRequest
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
    create_programming_languages_request = gateway_api_sdk.CreateProgrammingLanguagesRequest() # CreateProgrammingLanguagesRequest | Programming language definition

    try:
        # ProgrammingLanguage@store
        api_response = api_instance.create_programming_languages(create_programming_languages_request)
        print("The response of ProgrammingLanguageApi->create_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->create_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_programming_languages_request** | [**CreateProgrammingLanguagesRequest**](CreateProgrammingLanguagesRequest.md)| Programming language definition | 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_programming_languages**
> DeleteApplications200Response delete_programming_languages(id)

ProgrammingLanguage@destroy

Delete a system programming language

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

# **edit_programming_languages**
> UpdateProgrammingLanguages200Response edit_programming_languages(id, edit_programming_languages_request)

ProgrammingLanguage@update

Edit a system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_programming_languages_request import EditProgrammingLanguagesRequest
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
    edit_programming_languages_request = gateway_api_sdk.EditProgrammingLanguagesRequest() # EditProgrammingLanguagesRequest | ProgrammingLanguage definition

    try:
        # ProgrammingLanguage@update
        api_response = api_instance.edit_programming_languages(id, edit_programming_languages_request)
        print("The response of ProgrammingLanguageApi->edit_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->edit_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 
 **edit_programming_languages_request** | [**EditProgrammingLanguagesRequest**](EditProgrammingLanguagesRequest.md)| ProgrammingLanguage definition | 

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

# **update_programming_languages**
> UpdateProgrammingLanguages200Response update_programming_languages(id, update_programming_languages_request)

ProgrammingLanguage@update

Update a system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_programming_languages200_response import UpdateProgrammingLanguages200Response
from gateway_api_sdk.models.update_programming_languages_request import UpdateProgrammingLanguagesRequest
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
    update_programming_languages_request = gateway_api_sdk.UpdateProgrammingLanguagesRequest() # UpdateProgrammingLanguagesRequest | ProgrammingLanguage definition

    try:
        # ProgrammingLanguage@update
        api_response = api_instance.update_programming_languages(id, update_programming_languages_request)
        print("The response of ProgrammingLanguageApi->update_programming_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->update_programming_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 
 **update_programming_languages_request** | [**UpdateProgrammingLanguagesRequest**](UpdateProgrammingLanguagesRequest.md)| ProgrammingLanguage definition | 

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

