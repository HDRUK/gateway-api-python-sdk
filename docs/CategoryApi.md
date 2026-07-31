# gateway_api_sdk.CategoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_categories**](CategoryApi.md#create_categories) | **POST** /api/v1/categories | Category@store
[**delete_categories**](CategoryApi.md#delete_categories) | **DELETE** /api/v1/categories/{id} | Category@destroy
[**edit_categories**](CategoryApi.md#edit_categories) | **PATCH** /api/v1/categories/{id} | Category@update
[**fetch_all_categories**](CategoryApi.md#fetch_all_categories) | **GET** /api/v1/categories | Category@index
[**fetch_categories**](CategoryApi.md#fetch_categories) | **GET** /api/v1/categories/{id} | Category@show
[**update_categories**](CategoryApi.md#update_categories) | **PUT** /api/v1/categories/{id} | Category@update


# **create_categories**
> CreateCategories200Response create_categories(create_categories_request)

Category@store

Creates a new tool category

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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    create_categories_request = gateway_api_sdk.CreateCategoriesRequest() # CreateCategoriesRequest | Category definition

    try:
        # Category@store
        api_response = api_instance.create_categories(create_categories_request)
        print("The response of CategoryApi->create_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->create_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md)| Category definition | 

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

# **delete_categories**
> DeleteAliases200Response delete_categories(id)

Category@destroy

Delete a tool category

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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id

    try:
        # Category@destroy
        api_response = api_instance.delete_categories(id)
        print("The response of CategoryApi->delete_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->delete_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 

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

# **edit_categories**
> UpdateCategories200Response edit_categories(id, edit_categories_request)

Category@update

Edit a tool category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_categories_request import EditCategoriesRequest
from gateway_api_sdk.models.update_categories200_response import UpdateCategories200Response
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id
    edit_categories_request = gateway_api_sdk.EditCategoriesRequest() # EditCategoriesRequest | Category definition

    try:
        # Category@update
        api_response = api_instance.edit_categories(id, edit_categories_request)
        print("The response of CategoryApi->edit_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->edit_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 
 **edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md)| Category definition | 

### Return type

[**UpdateCategories200Response**](UpdateCategories200Response.md)

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

# **fetch_all_categories**
> FetchAllCategories200Response fetch_all_categories(per_page=per_page)

Category@index

Returns a list of categories enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_categories200_response import FetchAllCategories200Response
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # Category@index
        api_response = api_instance.fetch_all_categories(per_page=per_page)
        print("The response of CategoryApi->fetch_all_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->fetch_all_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchAllCategories200Response**](FetchAllCategories200Response.md)

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

# **fetch_categories**
> FetchAllCategories200Response fetch_categories(id)

Category@show

Return a single tool category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_categories200_response import FetchAllCategories200Response
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id

    try:
        # Category@show
        api_response = api_instance.fetch_categories(id)
        print("The response of CategoryApi->fetch_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->fetch_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 

### Return type

[**FetchAllCategories200Response**](FetchAllCategories200Response.md)

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

# **update_categories**
> UpdateCategories200Response update_categories(id, update_categories_request)

Category@update

Update a tool category

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_categories200_response import UpdateCategories200Response
from gateway_api_sdk.models.update_categories_request import UpdateCategoriesRequest
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
    api_instance = gateway_api_sdk.CategoryApi(api_client)
    id = 1 # int | category id
    update_categories_request = gateway_api_sdk.UpdateCategoriesRequest() # UpdateCategoriesRequest | Category definition

    try:
        # Category@update
        api_response = api_instance.update_categories(id, update_categories_request)
        print("The response of CategoryApi->update_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CategoryApi->update_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| category id | 
 **update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md)| Category definition | 

### Return type

[**UpdateCategories200Response**](UpdateCategories200Response.md)

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

