# gateway_api_sdk.KeywordApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_keywords**](KeywordApi.md#create_keywords) | **POST** /api/v1/keywords | KeywordController@store
[**delete_keywords**](KeywordApi.md#delete_keywords) | **DELETE** /api/v1/keywords/{id} | KeywordController@destroy
[**edit_keywords**](KeywordApi.md#edit_keywords) | **PATCH** /api/v1/keywords/{id} | KeywordController@update
[**fetch_all_keywords**](KeywordApi.md#fetch_all_keywords) | **GET** /api/v1/keywords | KeywordController@index
[**fetch_keywords**](KeywordApi.md#fetch_keywords) | **GET** /api/v1/keywords/{id} | KeywordController@show
[**update_keywords**](KeywordApi.md#update_keywords) | **PUT** /api/v1/keywords/{id} | KeywordController@update


# **create_keywords**
> CreateCategories200Response create_keywords(create_categories_request)

KeywordController@store

Creates a new keyword

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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    create_categories_request = gateway_api_sdk.CreateCategoriesRequest() # CreateCategoriesRequest | Keyword definition

    try:
        # KeywordController@store
        api_response = api_instance.create_keywords(create_categories_request)
        print("The response of KeywordApi->create_keywords:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->create_keywords: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_categories_request** | [**CreateCategoriesRequest**](CreateCategoriesRequest.md)| Keyword definition | 

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
**409** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_keywords**
> DeleteAliases200Response delete_keywords(id)

KeywordController@destroy

Delete a keyword by id

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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id

    try:
        # KeywordController@destroy
        api_response = api_instance.delete_keywords(id)
        print("The response of KeywordApi->delete_keywords:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->delete_keywords: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 

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

# **edit_keywords**
> UpdateKeywords200Response edit_keywords(id, edit_categories_request)

KeywordController@update

Edit a keyword by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_categories_request import EditCategoriesRequest
from gateway_api_sdk.models.update_keywords200_response import UpdateKeywords200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id
    edit_categories_request = gateway_api_sdk.EditCategoriesRequest() # EditCategoriesRequest | Category definition

    try:
        # KeywordController@update
        api_response = api_instance.edit_keywords(id, edit_categories_request)
        print("The response of KeywordApi->edit_keywords:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->edit_keywords: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 
 **edit_categories_request** | [**EditCategoriesRequest**](EditCategoriesRequest.md)| Category definition | 

### Return type

[**UpdateKeywords200Response**](UpdateKeywords200Response.md)

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

# **fetch_all_keywords**
> FetchAllKeywords200Response fetch_all_keywords(per_page=per_page)

KeywordController@index

Returns a list of keywords

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_keywords200_response import FetchAllKeywords200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    per_page = 56 # int | Alternative output schema version. (optional)

    try:
        # KeywordController@index
        api_response = api_instance.fetch_all_keywords(per_page=per_page)
        print("The response of KeywordApi->fetch_all_keywords:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->fetch_all_keywords: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| Alternative output schema version. | [optional] 

### Return type

[**FetchAllKeywords200Response**](FetchAllKeywords200Response.md)

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

# **fetch_keywords**
> FetchKeywords200Response fetch_keywords(id)

KeywordController@show

Return a single keyword

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_keywords200_response import FetchKeywords200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id

    try:
        # KeywordController@show
        api_response = api_instance.fetch_keywords(id)
        print("The response of KeywordApi->fetch_keywords:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->fetch_keywords: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 

### Return type

[**FetchKeywords200Response**](FetchKeywords200Response.md)

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

# **update_keywords**
> UpdateKeywords200Response update_keywords(id, update_categories_request)

KeywordController@update

Update a keyword by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_categories_request import UpdateCategoriesRequest
from gateway_api_sdk.models.update_keywords200_response import UpdateKeywords200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id
    update_categories_request = gateway_api_sdk.UpdateCategoriesRequest() # UpdateCategoriesRequest | Keyword definition

    try:
        # KeywordController@update
        api_response = api_instance.update_keywords(id, update_categories_request)
        print("The response of KeywordApi->update_keywords:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->update_keywords: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 
 **update_categories_request** | [**UpdateCategoriesRequest**](UpdateCategoriesRequest.md)| Keyword definition | 

### Return type

[**UpdateKeywords200Response**](UpdateKeywords200Response.md)

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

