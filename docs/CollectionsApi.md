# gateway_api_sdk.CollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_unique_fields_collections**](CollectionsApi.md#count_unique_fields_collections) | **GET** /api/v1/collections/count/{field} | CollectionController@count
[**count_unique_fields_collections_v2**](CollectionsApi.md#count_unique_fields_collections_v2) | **GET** /api/v2/collections/count/{field} | CollectionController@count
[**create_collections**](CollectionsApi.md#create_collections) | **POST** /api/v2/collections | CollectionController@store
[**delete_collections_v2**](CollectionsApi.md#delete_collections_v2) | **DELETE** /api/v2/collections/{id} | Delete a collection
[**edit_collections_v2**](CollectionsApi.md#edit_collections_v2) | **PATCH** /api/v2/collections/{id} | Edit a collection
[**fetch_all_collections**](CollectionsApi.md#fetch_all_collections) | **GET** /api/v1/collections | CollectionController@index
[**fetch_all_collections_v2**](CollectionsApi.md#fetch_all_collections_v2) | **GET** /api/v2/collections | CollectionController@index
[**fetch_collections**](CollectionsApi.md#fetch_collections) | **GET** /api/v1/collections/{id} | CollectionController@show
[**fetch_collections_v2**](CollectionsApi.md#fetch_collections_v2) | **GET** /api/v2/collections/{id} | CollectionController@show
[**update_collections_v2**](CollectionsApi.md#update_collections_v2) | **PUT** /api/v2/collections/{id} | Update a collection


# **count_unique_fields_collections**
> CountUniqueFieldsCollections200Response count_unique_fields_collections(var_field, team_id, user_id)

CollectionController@count

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    var_field = 'status' # str | name of the field to perform a count on
    team_id = 1 # int | team id
    user_id = 1 # int | user id

    try:
        # CollectionController@count
        api_response = api_instance.count_unique_fields_collections(var_field, team_id, user_id)
        print("The response of CollectionsApi->count_unique_fields_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->count_unique_fields_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_field** | **str**| name of the field to perform a count on | 
 **team_id** | **int**| team id | 
 **user_id** | **int**| user id | 

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

# **count_unique_fields_collections_v2**
> CountUniqueFieldsCollections200Response count_unique_fields_collections_v2(var_field)

CollectionController@count

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    var_field = 'status' # str | name of the field to perform a count on

    try:
        # CollectionController@count
        api_response = api_instance.count_unique_fields_collections_v2(var_field)
        print("The response of CollectionsApi->count_unique_fields_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->count_unique_fields_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_field** | **str**| name of the field to perform a count on | 

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

# **create_collections**
> CreateDarIntegration201Response create_collections(create_collections_request)

CollectionController@store

Create a new collection owned by an individual

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_collections_request import CreateCollectionsRequest
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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    create_collections_request = gateway_api_sdk.CreateCollectionsRequest() # CreateCollectionsRequest | Pass user credentials

    try:
        # CollectionController@store
        api_response = api_instance.create_collections(create_collections_request)
        print("The response of CollectionsApi->create_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->create_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_collections_request** | [**CreateCollectionsRequest**](CreateCollectionsRequest.md)| Pass user credentials | 

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

# **delete_collections_v2**
> DeleteApplications200Response delete_collections_v2(id)

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    id = 1 # int | collection id

    try:
        # Delete a collection
        api_response = api_instance.delete_collections_v2(id)
        print("The response of CollectionsApi->delete_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->delete_collections_v2: %s\n" % e)
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

# **edit_collections_v2**
> FetchCollections200Response edit_collections_v2(id, edit_collections_v2_request, unarchive=unarchive)

Edit a collection

Edit a collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_collections_v2_request import EditCollectionsV2Request
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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    id = 1 # int | collection id
    edit_collections_v2_request = gateway_api_sdk.EditCollectionsV2Request() # EditCollectionsV2Request | Pass user credentials
    unarchive = 'unarchive_example' # str | Unarchive a collection (optional)

    try:
        # Edit a collection
        api_response = api_instance.edit_collections_v2(id, edit_collections_v2_request, unarchive=unarchive)
        print("The response of CollectionsApi->edit_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->edit_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **edit_collections_v2_request** | [**EditCollectionsV2Request**](EditCollectionsV2Request.md)| Pass user credentials | 
 **unarchive** | **str**| Unarchive a collection | [optional] 

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

# **fetch_all_collections**
> FetchAllCollections200Response fetch_all_collections(name=name, team_id=team_id, user_id=user_id, title=title, status=status, per_page=per_page)

CollectionController@index

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    name = 'name_example' # str | Filter collections by name (optional)
    team_id = 56 # int | Filter collections by team ID (optional)
    user_id = 56 # int | Filter collections by user ID (optional)
    title = 'title_example' # str | Filter collections by title (optional)
    status = 'status_example' # str | Filter collections by status (DRAFT, ACTIVE, ARCHIVED) (optional)
    per_page = 1 # int | per page (optional)

    try:
        # CollectionController@index
        api_response = api_instance.fetch_all_collections(name=name, team_id=team_id, user_id=user_id, title=title, status=status, per_page=per_page)
        print("The response of CollectionsApi->fetch_all_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_all_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Filter collections by name | [optional] 
 **team_id** | **int**| Filter collections by team ID | [optional] 
 **user_id** | **int**| Filter collections by user ID | [optional] 
 **title** | **str**| Filter collections by title | [optional] 
 **status** | **str**| Filter collections by status (DRAFT, ACTIVE, ARCHIVED) | [optional] 
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

# **fetch_all_collections_v2**
> FetchAllCollections200Response fetch_all_collections_v2()

CollectionController@index

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)

    try:
        # CollectionController@index
        api_response = api_instance.fetch_all_collections_v2()
        print("The response of CollectionsApi->fetch_all_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_all_collections_v2: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

# **fetch_collections**
> FetchCollections200Response fetch_collections(id, view_type=view_type)

CollectionController@show

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    id = 1 # int | collection id
    view_type = 'full' # str | Query flag to show full collection data or a trimmed version (defaults to full). (optional) (default to 'full')

    try:
        # CollectionController@show
        api_response = api_instance.fetch_collections(id, view_type=view_type)
        print("The response of CollectionsApi->fetch_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **view_type** | **str**| Query flag to show full collection data or a trimmed version (defaults to full). | [optional] [default to &#39;full&#39;]

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

# **fetch_collections_v2**
> FetchCollections200Response fetch_collections_v2(id, view_type=view_type)

CollectionController@show

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    id = 1 # int | collection id
    view_type = 'full' # str | Query flag to show full collection data or a trimmed version (defaults to full). (optional) (default to 'full')

    try:
        # CollectionController@show
        api_response = api_instance.fetch_collections_v2(id, view_type=view_type)
        print("The response of CollectionsApi->fetch_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **view_type** | **str**| Query flag to show full collection data or a trimmed version (defaults to full). | [optional] [default to &#39;full&#39;]

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

# **update_collections_v2**
> FetchCollections200Response update_collections_v2(id, update_collections_v2_request)

Update a collection

Update a collection owned by an individual

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
from gateway_api_sdk.models.update_collections_v2_request import UpdateCollectionsV2Request
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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    id = 1 # int | collection id
    update_collections_v2_request = gateway_api_sdk.UpdateCollectionsV2Request() # UpdateCollectionsV2Request | Pass user credentials

    try:
        # Update a collection
        api_response = api_instance.update_collections_v2(id, update_collections_v2_request)
        print("The response of CollectionsApi->update_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->update_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **update_collections_v2_request** | [**UpdateCollectionsV2Request**](UpdateCollectionsV2Request.md)| Pass user credentials | 

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

