# gateway_api_sdk.SavedSearchApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_saved_searches**](SavedSearchApi.md#create_saved_searches) | **POST** /api/v1/saved_searches | SavedSearch@store
[**delete_saved_searches**](SavedSearchApi.md#delete_saved_searches) | **DELETE** /api/v1/saved_searches/{id} | SavedSearch@destroy
[**edit_saved_searches**](SavedSearchApi.md#edit_saved_searches) | **PATCH** /api/v1/saved_searches/{id} | SavedSearch@update
[**fetch_all_saved_searches**](SavedSearchApi.md#fetch_all_saved_searches) | **GET** /api/v1/saved_searches | SavedSearch@index
[**fetch_saved_searches**](SavedSearchApi.md#fetch_saved_searches) | **GET** /api/v1/saved_searches/{id} | SavedSearch@show
[**update_saved_searches**](SavedSearchApi.md#update_saved_searches) | **PUT** /api/v1/saved_searches/{id} | SavedSearch@update


# **create_saved_searches**
> CreateCategories200Response create_saved_searches(create_saved_searches_request)

SavedSearch@store

Creates a new saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_saved_searches_request import CreateSavedSearchesRequest
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    create_saved_searches_request = gateway_api_sdk.CreateSavedSearchesRequest() # CreateSavedSearchesRequest | Saved search definition

    try:
        # SavedSearch@store
        api_response = api_instance.create_saved_searches(create_saved_searches_request)
        print("The response of SavedSearchApi->create_saved_searches:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->create_saved_searches: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_saved_searches_request** | [**CreateSavedSearchesRequest**](CreateSavedSearchesRequest.md)| Saved search definition | 

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

# **delete_saved_searches**
> DeleteAliases200Response delete_saved_searches(id)

SavedSearch@destroy

Delete a saved search

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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id

    try:
        # SavedSearch@destroy
        api_response = api_instance.delete_saved_searches(id)
        print("The response of SavedSearchApi->delete_saved_searches:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->delete_saved_searches: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 

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

# **edit_saved_searches**
> UpdateSavedSearches200Response edit_saved_searches(id, edit_saved_searches_request)

SavedSearch@update

Edit a saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_saved_searches_request import EditSavedSearchesRequest
from gateway_api_sdk.models.update_saved_searches200_response import UpdateSavedSearches200Response
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id
    edit_saved_searches_request = gateway_api_sdk.EditSavedSearchesRequest() # EditSavedSearchesRequest | Saved search definition

    try:
        # SavedSearch@update
        api_response = api_instance.edit_saved_searches(id, edit_saved_searches_request)
        print("The response of SavedSearchApi->edit_saved_searches:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->edit_saved_searches: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 
 **edit_saved_searches_request** | [**EditSavedSearchesRequest**](EditSavedSearchesRequest.md)| Saved search definition | 

### Return type

[**UpdateSavedSearches200Response**](UpdateSavedSearches200Response.md)

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

# **fetch_all_saved_searches**
> FetchAllSavedSearches200Response fetch_all_saved_searches(per_page=per_page)

SavedSearch@index

Returns a list of saved searches enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_saved_searches200_response import FetchAllSavedSearches200Response
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    per_page = 56 # int | Specify number of results per page (optional)

    try:
        # SavedSearch@index
        api_response = api_instance.fetch_all_saved_searches(per_page=per_page)
        print("The response of SavedSearchApi->fetch_all_saved_searches:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->fetch_all_saved_searches: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| Specify number of results per page | [optional] 

### Return type

[**FetchAllSavedSearches200Response**](FetchAllSavedSearches200Response.md)

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

# **fetch_saved_searches**
> FetchAllSavedSearches200Response fetch_saved_searches(id)

SavedSearch@show

Return a single saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_saved_searches200_response import FetchAllSavedSearches200Response
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id

    try:
        # SavedSearch@show
        api_response = api_instance.fetch_saved_searches(id)
        print("The response of SavedSearchApi->fetch_saved_searches:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->fetch_saved_searches: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 

### Return type

[**FetchAllSavedSearches200Response**](FetchAllSavedSearches200Response.md)

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

# **update_saved_searches**
> UpdateSavedSearches200Response update_saved_searches(id, update_saved_searches_request)

SavedSearch@update

Update a saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_saved_searches200_response import UpdateSavedSearches200Response
from gateway_api_sdk.models.update_saved_searches_request import UpdateSavedSearchesRequest
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id
    update_saved_searches_request = gateway_api_sdk.UpdateSavedSearchesRequest() # UpdateSavedSearchesRequest | Saved search definition

    try:
        # SavedSearch@update
        api_response = api_instance.update_saved_searches(id, update_saved_searches_request)
        print("The response of SavedSearchApi->update_saved_searches:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->update_saved_searches: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 
 **update_saved_searches_request** | [**UpdateSavedSearchesRequest**](UpdateSavedSearchesRequest.md)| Saved search definition | 

### Return type

[**UpdateSavedSearches200Response**](UpdateSavedSearches200Response.md)

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

