# gateway_api_sdk.TypeCategoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_type_categories**](TypeCategoryApi.md#create_type_categories) | **POST** /api/v1/type_categories | TypeCategory@store
[**delete_type_categories**](TypeCategoryApi.md#delete_type_categories) | **DELETE** /api/v1/type_categories/{id} | TypeCategory@destroy
[**edit_type_categories**](TypeCategoryApi.md#edit_type_categories) | **PATCH** /api/v1/type_categories/{id} | TypeCategory@update
[**update_type_categories**](TypeCategoryApi.md#update_type_categories) | **PUT** /api/v1/type_categories/{id} | TypeCategory@update


# **create_type_categories**
> CreateDarIntegration201Response create_type_categories(create_type_categories_request)

TypeCategory@store

Creates a new system type category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
from gateway_api_sdk.models.create_type_categories_request import CreateTypeCategoriesRequest
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    create_type_categories_request = gateway_api_sdk.CreateTypeCategoriesRequest() # CreateTypeCategoriesRequest | Programming language definition

    try:
        # TypeCategory@store
        api_response = api_instance.create_type_categories(create_type_categories_request)
        print("The response of TypeCategoryApi->create_type_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->create_type_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_type_categories_request** | [**CreateTypeCategoriesRequest**](CreateTypeCategoriesRequest.md)| Programming language definition | 

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

# **delete_type_categories**
> DeleteApplications200Response delete_type_categories(id)

TypeCategory@destroy

Delete a system type category

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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    id = 1 # int | type category id

    try:
        # TypeCategory@destroy
        api_response = api_instance.delete_type_categories(id)
        print("The response of TypeCategoryApi->delete_type_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->delete_type_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| type category id | 

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

# **edit_type_categories**
> UpdateTypeCategories200Response edit_type_categories(id, edit_programming_languages_request)

TypeCategory@update

Edit a system type category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_programming_languages_request import EditProgrammingLanguagesRequest
from gateway_api_sdk.models.update_type_categories200_response import UpdateTypeCategories200Response
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    id = 1 # int | type category id
    edit_programming_languages_request = gateway_api_sdk.EditProgrammingLanguagesRequest() # EditProgrammingLanguagesRequest | TypeCategory definition

    try:
        # TypeCategory@update
        api_response = api_instance.edit_type_categories(id, edit_programming_languages_request)
        print("The response of TypeCategoryApi->edit_type_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->edit_type_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| type category id | 
 **edit_programming_languages_request** | [**EditProgrammingLanguagesRequest**](EditProgrammingLanguagesRequest.md)| TypeCategory definition | 

### Return type

[**UpdateTypeCategories200Response**](UpdateTypeCategories200Response.md)

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

# **update_type_categories**
> UpdateTypeCategories200Response update_type_categories(id, update_type_categories_request)

TypeCategory@update

Update a system type category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_type_categories200_response import UpdateTypeCategories200Response
from gateway_api_sdk.models.update_type_categories_request import UpdateTypeCategoriesRequest
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
    api_instance = gateway_api_sdk.TypeCategoryApi(api_client)
    id = 1 # int | type category id
    update_type_categories_request = gateway_api_sdk.UpdateTypeCategoriesRequest() # UpdateTypeCategoriesRequest | TypeCategory definition

    try:
        # TypeCategory@update
        api_response = api_instance.update_type_categories(id, update_type_categories_request)
        print("The response of TypeCategoryApi->update_type_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TypeCategoryApi->update_type_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| type category id | 
 **update_type_categories_request** | [**UpdateTypeCategoriesRequest**](UpdateTypeCategoriesRequest.md)| TypeCategory definition | 

### Return type

[**UpdateTypeCategories200Response**](UpdateTypeCategories200Response.md)

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

