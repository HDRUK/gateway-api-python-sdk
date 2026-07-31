# gateway_api_sdk.PublicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_team_unique_fields_publication_v2**](PublicationApi.md#count_team_unique_fields_publication_v2) | **GET** /api/v2/teams/{teamId}/publications/count/{field} | TeamPublicationController@count
[**count_unique_fields_publications**](PublicationApi.md#count_unique_fields_publications) | **GET** /api/v1/publication/count/{field} | PublicationController@count
[**count_user_unique_fields_publication_v2**](PublicationApi.md#count_user_unique_fields_publication_v2) | **GET** /api/v2/users/{userId}/publications/count/{field} | UserPublicationController@count
[**create_publications**](PublicationApi.md#create_publications) | **POST** /api/v1/publications | PublicationController@store
[**create_publications_v2_by_team_id**](PublicationApi.md#create_publications_v2_by_team_id) | **POST** /api/v2/teams/{teamId}/publications | TeamPublicationController@store
[**create_publications_v2_by_user_id**](PublicationApi.md#create_publications_v2_by_user_id) | **POST** /api/v2/users/{userId}/publications | UserPublicationController@store
[**delete_publications**](PublicationApi.md#delete_publications) | **DELETE** /api/v1/publications/{id} | PublicationController@destroy
[**delete_publications_v2_by_team_id**](PublicationApi.md#delete_publications_v2_by_team_id) | **DELETE** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@destroy
[**delete_publications_v2_by_user_id**](PublicationApi.md#delete_publications_v2_by_user_id) | **DELETE** /api/v2/users/{userId}/publications/{id} | UserPublicationController@destroy
[**edit_publications**](PublicationApi.md#edit_publications) | **PATCH** /api/v1/publications/{id} | PublicationController@edit
[**edit_publications_v2_by_team_id**](PublicationApi.md#edit_publications_v2_by_team_id) | **PATCH** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@edit
[**edit_publications_v2_by_user_id**](PublicationApi.md#edit_publications_v2_by_user_id) | **PATCH** /api/v2/users/{userId}/publications/{id} | UserPublicationController@edit
[**fetch_all_publications**](PublicationApi.md#fetch_all_publications) | **GET** /api/v1/publications | PublicationController@index
[**fetch_all_publications_by_team_and_status_v2**](PublicationApi.md#fetch_all_publications_by_team_and_status_v2) | **GET** /api/v2/teams/{teamId}/publications/status/{status} | TeamPublicationController@indexStatus
[**fetch_all_publications_by_user_and_status_v2**](PublicationApi.md#fetch_all_publications_by_user_and_status_v2) | **GET** /api/v2/users/{userId}/publications/{status} | UserPublicationController@indexStatus
[**fetch_all_publications_v2**](PublicationApi.md#fetch_all_publications_v2) | **GET** /api/v2/publications | PublicationController@indexActive
[**fetch_publications**](PublicationApi.md#fetch_publications) | **GET** /api/v1/publications/{id} | PublicationController@show
[**fetch_publications_by_team_and_by_id_v2**](PublicationApi.md#fetch_publications_by_team_and_by_id_v2) | **GET** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@show
[**fetch_publications_by_user_and_by_id_v2**](PublicationApi.md#fetch_publications_by_user_and_by_id_v2) | **GET** /api/v2/users/{userId}/publications/{id} | UserPublicationController@show
[**fetch_publications_v2**](PublicationApi.md#fetch_publications_v2) | **GET** /api/v2/publications/{id} | PublicationController@showActive
[**update_publications**](PublicationApi.md#update_publications) | **PUT** /api/v1/publications/{id} | PublicationController@update
[**update_publications_v2_by_team_id**](PublicationApi.md#update_publications_v2_by_team_id) | **PUT** /api/v2/teams/{teamId}/publications/{id} | TeamPublicationController@update
[**update_publications_v2_by_user_id**](PublicationApi.md#update_publications_v2_by_user_id) | **PUT** /api/v2/users/{userId}/publications/{id} | UserPublicationController@update


# **count_team_unique_fields_publication_v2**
> CountUniqueFieldsCollections200Response count_team_unique_fields_publication_v2(team_id, var_field)

TeamPublicationController@count

Get team counts for distinct entries of a field in the model

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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    team_id = 1 # int | team id
    var_field = 'status' # str | name of the field to perform a count on

    try:
        # TeamPublicationController@count
        api_response = api_instance.count_team_unique_fields_publication_v2(team_id, var_field)
        print("The response of PublicationApi->count_team_unique_fields_publication_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->count_team_unique_fields_publication_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
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

# **count_unique_fields_publications**
> CountUniqueFieldsCollections200Response count_unique_fields_publications(var_field, owner_id, team_id=team_id)

PublicationController@count

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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    var_field = 'status' # str | name of the field to perform a count on
    owner_id = 1 # int | owner id
    team_id = 1 # int |  (optional)

    try:
        # PublicationController@count
        api_response = api_instance.count_unique_fields_publications(var_field, owner_id, team_id=team_id)
        print("The response of PublicationApi->count_unique_fields_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->count_unique_fields_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **var_field** | **str**| name of the field to perform a count on | 
 **owner_id** | **int**| owner id | 
 **team_id** | **int**|  | [optional] 

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

# **count_user_unique_fields_publication_v2**
> CountUniqueFieldsCollections200Response count_user_unique_fields_publication_v2(user_id, var_field)

UserPublicationController@count

Get user counts for distinct entries of a field in the model

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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    user_id = 1 # int | user id
    var_field = 'status' # str | name of the field to perform a count on

    try:
        # UserPublicationController@count
        api_response = api_instance.count_user_unique_fields_publication_v2(user_id, var_field)
        print("The response of PublicationApi->count_user_unique_fields_publication_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->count_user_unique_fields_publication_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 
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

# **create_publications**
> CreateCategories200Response create_publications(create_publications_request)

PublicationController@store

Create a new publication

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_publications_request import CreatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    create_publications_request = gateway_api_sdk.CreatePublicationsRequest() # CreatePublicationsRequest | Pass user credentials

    try:
        # PublicationController@store
        api_response = api_instance.create_publications(create_publications_request)
        print("The response of PublicationApi->create_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->create_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_publications_request** | [**CreatePublicationsRequest**](CreatePublicationsRequest.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_publications_v2_by_team_id**
> CreateCategories200Response create_publications_v2_by_team_id(team_id, create_publications_request)

TeamPublicationController@store

Create a new publication by team id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_publications_request import CreatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    team_id = 1 # int | team id
    create_publications_request = gateway_api_sdk.CreatePublicationsRequest() # CreatePublicationsRequest | Pass user credentials

    try:
        # TeamPublicationController@store
        api_response = api_instance.create_publications_v2_by_team_id(team_id, create_publications_request)
        print("The response of PublicationApi->create_publications_v2_by_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->create_publications_v2_by_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **create_publications_request** | [**CreatePublicationsRequest**](CreatePublicationsRequest.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_publications_v2_by_user_id**
> CreateCategories200Response create_publications_v2_by_user_id(user_id, create_publications_request)

UserPublicationController@store

Create a new publication by user id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_publications_request import CreatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    user_id = 56 # int | ID of the user
    create_publications_request = gateway_api_sdk.CreatePublicationsRequest() # CreatePublicationsRequest | Pass user credentials

    try:
        # UserPublicationController@store
        api_response = api_instance.create_publications_v2_by_user_id(user_id, create_publications_request)
        print("The response of PublicationApi->create_publications_v2_by_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->create_publications_v2_by_user_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **create_publications_request** | [**CreatePublicationsRequest**](CreatePublicationsRequest.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_publications**
> DeleteFederation200Response delete_publications(id)

PublicationController@destroy

Delete publication by id

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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    id = 1 # int | publication id

    try:
        # PublicationController@destroy
        api_response = api_instance.delete_publications(id)
        print("The response of PublicationApi->delete_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->delete_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| publication id | 

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
**401** | Unauthorized |  -  |
**404** | Error response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_publications_v2_by_team_id**
> DeleteFederation200Response delete_publications_v2_by_team_id(team_id, id)

TeamPublicationController@destroy

Delete publication by team id and id

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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | publication id

    try:
        # TeamPublicationController@destroy
        api_response = api_instance.delete_publications_v2_by_team_id(team_id, id)
        print("The response of PublicationApi->delete_publications_v2_by_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->delete_publications_v2_by_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| publication id | 

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
**401** | Unauthorized |  -  |
**404** | Error response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_publications_v2_by_user_id**
> DeleteFederation200Response delete_publications_v2_by_user_id(user_id, id)

UserPublicationController@destroy

Delete publication by user id and id

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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    user_id = 56 # int | ID of the user
    id = 1 # int | publication id

    try:
        # UserPublicationController@destroy
        api_response = api_instance.delete_publications_v2_by_user_id(user_id, id)
        print("The response of PublicationApi->delete_publications_v2_by_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->delete_publications_v2_by_user_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **id** | **int**| publication id | 

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
**401** | Unauthorized |  -  |
**404** | Error response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_publications**
> FetchPublications200Response edit_publications(id, update_publications_request, unarchive=unarchive)

PublicationController@edit

Edit publications

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
from gateway_api_sdk.models.update_publications_request import UpdatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    id = 1 # int | publications id
    update_publications_request = gateway_api_sdk.UpdatePublicationsRequest() # UpdatePublicationsRequest | Pass user credentials
    unarchive = 'unarchive_example' # str | Unarchive a publication (optional)

    try:
        # PublicationController@edit
        api_response = api_instance.edit_publications(id, update_publications_request, unarchive=unarchive)
        print("The response of PublicationApi->edit_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->edit_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| publications id | 
 **update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md)| Pass user credentials | 
 **unarchive** | **str**| Unarchive a publication | [optional] 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_publications_v2_by_team_id**
> FetchPublications200Response edit_publications_v2_by_team_id(team_id, id, update_publications_request)

TeamPublicationController@edit

Edit publications by team id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
from gateway_api_sdk.models.update_publications_request import UpdatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | publications id
    update_publications_request = gateway_api_sdk.UpdatePublicationsRequest() # UpdatePublicationsRequest | Pass user credentials

    try:
        # TeamPublicationController@edit
        api_response = api_instance.edit_publications_v2_by_team_id(team_id, id, update_publications_request)
        print("The response of PublicationApi->edit_publications_v2_by_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->edit_publications_v2_by_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| publications id | 
 **update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md)| Pass user credentials | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_publications_v2_by_user_id**
> FetchPublications200Response edit_publications_v2_by_user_id(user_id, id, update_publications_request)

UserPublicationController@edit

Edit publications by user id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
from gateway_api_sdk.models.update_publications_request import UpdatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    user_id = 56 # int | ID of the user
    id = 1 # int | publications id
    update_publications_request = gateway_api_sdk.UpdatePublicationsRequest() # UpdatePublicationsRequest | Pass user credentials

    try:
        # UserPublicationController@edit
        api_response = api_instance.edit_publications_v2_by_user_id(user_id, id, update_publications_request)
        print("The response of PublicationApi->edit_publications_v2_by_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->edit_publications_v2_by_user_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **id** | **int**| publications id | 
 **update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md)| Pass user credentials | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_publications**
> FetchAllPublications200Response fetch_all_publications(paper_title=paper_title, owner_id=owner_id, team_id=team_id, status=status)

PublicationController@index

Get All Publications

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_publications200_response import FetchAllPublications200Response
from gateway_api_sdk.models.int import int
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    paper_title = 'paper_title_example' # str | Filter tools by paper title (optional)
    owner_id = 56 # int | Filter tools by owner id (optional)
    team_id = 56 # int | Filter tools by team id (optional)
    status = 'ACTIVE' # str | Publication status to filter by ('ACTIVE', 'DRAFT', 'ARCHIVED') (optional)

    try:
        # PublicationController@index
        api_response = api_instance.fetch_all_publications(paper_title=paper_title, owner_id=owner_id, team_id=team_id, status=status)
        print("The response of PublicationApi->fetch_all_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_all_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **paper_title** | **str**| Filter tools by paper title | [optional] 
 **owner_id** | [**int**](.md)| Filter tools by owner id | [optional] 
 **team_id** | [**int**](.md)| Filter tools by team id | [optional] 
 **status** | **str**| Publication status to filter by (&#39;ACTIVE&#39;, &#39;DRAFT&#39;, &#39;ARCHIVED&#39;) | [optional] 

### Return type

[**FetchAllPublications200Response**](FetchAllPublications200Response.md)

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

# **fetch_all_publications_by_team_and_status_v2**
> FetchAllPublications200Response fetch_all_publications_by_team_and_status_v2(team_id, status, paper_title=paper_title)

TeamPublicationController@indexStatus

Returns a list of a teams publications

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_publications200_response import FetchAllPublications200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    team_id = 56 # int | ID of the team
    status = 'active' # str | Status of the team (active, draft, or archived). Defaults to active if not provided. (default to 'active')
    paper_title = 'paper_title_example' # str | Filter Publication by title (optional)

    try:
        # TeamPublicationController@indexStatus
        api_response = api_instance.fetch_all_publications_by_team_and_status_v2(team_id, status, paper_title=paper_title)
        print("The response of PublicationApi->fetch_all_publications_by_team_and_status_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_all_publications_by_team_and_status_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| ID of the team | 
 **status** | **str**| Status of the team (active, draft, or archived). Defaults to active if not provided. | [default to &#39;active&#39;]
 **paper_title** | **str**| Filter Publication by title | [optional] 

### Return type

[**FetchAllPublications200Response**](FetchAllPublications200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_publications_by_user_and_status_v2**
> FetchAllPublications200Response fetch_all_publications_by_user_and_status_v2(user_id, status, paper_title=paper_title)

UserPublicationController@indexStatus

Returns a list of a users publications

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_publications200_response import FetchAllPublications200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    user_id = 56 # int | ID of the user
    status = 'active' # str | Status of the team (active, draft, or archived). Defaults to active if not provided. (default to 'active')
    paper_title = 'paper_title_example' # str | Filter Publication by title (optional)

    try:
        # UserPublicationController@indexStatus
        api_response = api_instance.fetch_all_publications_by_user_and_status_v2(user_id, status, paper_title=paper_title)
        print("The response of PublicationApi->fetch_all_publications_by_user_and_status_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_all_publications_by_user_and_status_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **status** | **str**| Status of the team (active, draft, or archived). Defaults to active if not provided. | [default to &#39;active&#39;]
 **paper_title** | **str**| Filter Publication by title | [optional] 

### Return type

[**FetchAllPublications200Response**](FetchAllPublications200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_publications_v2**
> FetchAllPublications200Response fetch_all_publications_v2(paper_title=paper_title, with_related=with_related, per_page=per_page)

PublicationController@indexActive

Get All Publications

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_publications200_response import FetchAllPublications200Response
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    paper_title = 'paper_title_example' # str | Filter tools by paper title (optional)
    with_related = True # bool | Return related datasets (optional)
    per_page = 1 # int | per page (optional)

    try:
        # PublicationController@indexActive
        api_response = api_instance.fetch_all_publications_v2(paper_title=paper_title, with_related=with_related, per_page=per_page)
        print("The response of PublicationApi->fetch_all_publications_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_all_publications_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **paper_title** | **str**| Filter tools by paper title | [optional] 
 **with_related** | **bool**| Return related datasets | [optional] 
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchAllPublications200Response**](FetchAllPublications200Response.md)

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

# **fetch_publications**
> FetchPublications200Response fetch_publications(id)

PublicationController@show

Get publication by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    id = 1 # int | publication id

    try:
        # PublicationController@show
        api_response = api_instance.fetch_publications(id)
        print("The response of PublicationApi->fetch_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| publication id | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

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

# **fetch_publications_by_team_and_by_id_v2**
> FetchPublications200Response fetch_publications_by_team_and_by_id_v2(team_id, id)

TeamPublicationController@show

Get publication by team id and by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | publication id

    try:
        # TeamPublicationController@show
        api_response = api_instance.fetch_publications_by_team_and_by_id_v2(team_id, id)
        print("The response of PublicationApi->fetch_publications_by_team_and_by_id_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_publications_by_team_and_by_id_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| publication id | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

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

# **fetch_publications_by_user_and_by_id_v2**
> FetchPublications200Response fetch_publications_by_user_and_by_id_v2(user_id, id)

UserPublicationController@show

Get publication by user id and by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    user_id = 56 # int | ID of the user
    id = 1 # int | publication id

    try:
        # UserPublicationController@show
        api_response = api_instance.fetch_publications_by_user_and_by_id_v2(user_id, id)
        print("The response of PublicationApi->fetch_publications_by_user_and_by_id_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_publications_by_user_and_by_id_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **id** | **int**| publication id | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

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

# **fetch_publications_v2**
> FetchPublications200Response fetch_publications_v2(id)

PublicationController@showActive

Get publication by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    id = 1 # int | publication id

    try:
        # PublicationController@showActive
        api_response = api_instance.fetch_publications_v2(id)
        print("The response of PublicationApi->fetch_publications_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->fetch_publications_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| publication id | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

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

# **update_publications**
> FetchPublications200Response update_publications(id, update_publications_request)

PublicationController@update

Update publications

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
from gateway_api_sdk.models.update_publications_request import UpdatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    id = 1 # int | publication id
    update_publications_request = gateway_api_sdk.UpdatePublicationsRequest() # UpdatePublicationsRequest | Pass user credentials

    try:
        # PublicationController@update
        api_response = api_instance.update_publications(id, update_publications_request)
        print("The response of PublicationApi->update_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->update_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| publication id | 
 **update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md)| Pass user credentials | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_publications_v2_by_team_id**
> FetchPublications200Response update_publications_v2_by_team_id(team_id, id, update_publications_request)

TeamPublicationController@update

Update publications by team id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
from gateway_api_sdk.models.update_publications_request import UpdatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | publication id
    update_publications_request = gateway_api_sdk.UpdatePublicationsRequest() # UpdatePublicationsRequest | Pass user credentials

    try:
        # TeamPublicationController@update
        api_response = api_instance.update_publications_v2_by_team_id(team_id, id, update_publications_request)
        print("The response of PublicationApi->update_publications_v2_by_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->update_publications_v2_by_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| publication id | 
 **update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md)| Pass user credentials | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_publications_v2_by_user_id**
> FetchPublications200Response update_publications_v2_by_user_id(user_id, id, update_publications_request)

UserPublicationController@update

Update publications by user id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_publications200_response import FetchPublications200Response
from gateway_api_sdk.models.update_publications_request import UpdatePublicationsRequest
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
    api_instance = gateway_api_sdk.PublicationApi(api_client)
    user_id = 56 # int | ID of the user
    id = 1 # int | publication id
    update_publications_request = gateway_api_sdk.UpdatePublicationsRequest() # UpdatePublicationsRequest | Pass user credentials

    try:
        # UserPublicationController@update
        api_response = api_instance.update_publications_v2_by_user_id(user_id, id, update_publications_request)
        print("The response of PublicationApi->update_publications_v2_by_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicationApi->update_publications_v2_by_user_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **id** | **int**| publication id | 
 **update_publications_request** | [**UpdatePublicationsRequest**](UpdatePublicationsRequest.md)| Pass user credentials | 

### Return type

[**FetchPublications200Response**](FetchPublications200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

