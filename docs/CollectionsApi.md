# gateway_api_sdk.CollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**a18eed83ffe8ac895df3e1efa5ffb421**](CollectionsApi.md#a18eed83ffe8ac895df3e1efa5ffb421) | **PUT** /api/v1/teams/{teamId}/collections/{id} | Update a collection
[**b2e32406fe513dd0c0747a0864b5ed28**](CollectionsApi.md#b2e32406fe513dd0c0747a0864b5ed28) | **DELETE** /api/v2/collections/{id} | Delete a collection
[**call_22bf9932e93726b8338c13e489c7d96e**](CollectionsApi.md#call_22bf9932e93726b8338c13e489c7d96e) | **PUT** /api/v2/users/{userId}/collections/{id} | Update a collection
[**call_2e589ea17282e3818437328b1a6d2c45**](CollectionsApi.md#call_2e589ea17282e3818437328b1a6d2c45) | **PATCH** /api/v2/teams/{teamId}/collections/{id} | Edit a collection
[**call_63175dd3a255646e0428a630af683e21**](CollectionsApi.md#call_63175dd3a255646e0428a630af683e21) | **PATCH** /api/v2/users/{userId}/collections/{id} | Edit a collection
[**call_6907582348e596c660cc65263dc3a4fc**](CollectionsApi.md#call_6907582348e596c660cc65263dc3a4fc) | **DELETE** /api/v1/teams/{teamId}/collections/{id} | Delete a collection
[**call_75c378b5764d9d73e14fe2d65c654910**](CollectionsApi.md#call_75c378b5764d9d73e14fe2d65c654910) | **PATCH** /api/v1/teams/{teamId}/collections/{id} | Edit a collection
[**call_78c554f5fb0f01c8d788a5789fd0c35b**](CollectionsApi.md#call_78c554f5fb0f01c8d788a5789fd0c35b) | **DELETE** /api/v2/users/{userId}/collections/{id} | Delete a collection
[**call_8abb5928cecc676521f3e3d8eea0c49c**](CollectionsApi.md#call_8abb5928cecc676521f3e3d8eea0c49c) | **PUT** /api/v2/collections/{id} | Update a collection
[**call_94ae4ab159160f6240a4bc00d2e6fe5f**](CollectionsApi.md#call_94ae4ab159160f6240a4bc00d2e6fe5f) | **PUT** /api/v2/teams/{teamId}/collections/{id} | Update a collection
[**call_9c525a2aaf8e8a81cbcdf1a3033bb1bb**](CollectionsApi.md#call_9c525a2aaf8e8a81cbcdf1a3033bb1bb) | **DELETE** /api/v2/teams/{teamId}/collections/{id} | Delete a collection
[**count_team_unique_fields_collection_v2**](CollectionsApi.md#count_team_unique_fields_collection_v2) | **GET** /api/v2/teams/{teamId}/collections/count/{field} | TeamCollectionController@count
[**count_unique_fields_collections**](CollectionsApi.md#count_unique_fields_collections) | **GET** /api/v1/collections/count/{field} | CollectionController@count
[**count_unique_fields_collections_v2**](CollectionsApi.md#count_unique_fields_collections_v2) | **GET** /api/v2/collections/count/{field} | CollectionController@count
[**count_user_unique_fields_collection_v2**](CollectionsApi.md#count_user_unique_fields_collection_v2) | **GET** /api/v2/users/{userId}/collections/count/{field} | UserCollectionController@count
[**create_collections**](CollectionsApi.md#create_collections) | **POST** /api/v2/collections | CollectionController@store
[**create_team_collections**](CollectionsApi.md#create_team_collections) | **POST** /api/v1/teams/{teamId}/collections | CollectionController@store
[**create_team_collections_v2**](CollectionsApi.md#create_team_collections_v2) | **POST** /api/v2/teams/{teamId}/collections | TeamCollectionController@store
[**create_user_collections**](CollectionsApi.md#create_user_collections) | **POST** /api/v2/users/collections | UserCollectionController@store
[**d183a285f65bdc0e6341ed79b3a63670**](CollectionsApi.md#d183a285f65bdc0e6341ed79b3a63670) | **PATCH** /api/v2/collections/{id} | Edit a collection
[**fetch_all_collections**](CollectionsApi.md#fetch_all_collections) | **GET** /api/v1/collections | CollectionController@index
[**fetch_all_collections_v2**](CollectionsApi.md#fetch_all_collections_v2) | **GET** /api/v2/collections | CollectionController@index
[**fetch_collections**](CollectionsApi.md#fetch_collections) | **GET** /api/v1/collections/{id} | CollectionController@show
[**fetch_collections_v2**](CollectionsApi.md#fetch_collections_v2) | **GET** /api/v2/collections/{id} | CollectionController@show
[**fetch_team_active_collections_v2**](CollectionsApi.md#fetch_team_active_collections_v2) | **GET** /api/v2/teams/{teamId}/collections/status/active | TeamCollectionController@indexActive
[**fetch_team_archived_collections_v2**](CollectionsApi.md#fetch_team_archived_collections_v2) | **GET** /api/v2/teams/{teamId}/collections/status/archived | TeamCollectionController@indexArchived
[**fetch_team_collection_v2**](CollectionsApi.md#fetch_team_collection_v2) | **GET** /api/v2/teams/{teamId}/collections/{id} | TeamCollectionController@show
[**fetch_team_draft_collections_v2**](CollectionsApi.md#fetch_team_draft_collections_v2) | **GET** /api/v2/teams/{teamId}/collections/status/draft | TeamCollectionController@indexDraft
[**fetch_user_archived_collections_v2**](CollectionsApi.md#fetch_user_archived_collections_v2) | **GET** /api/v2/users/{userId}/collections/status/archived | UserCollectionController@indexArchived
[**fetch_user_collection_v2**](CollectionsApi.md#fetch_user_collection_v2) | **GET** /api/v2/users/{userId}/collections/{id} | CollectionController@show
[**fetch_user_collections_v2**](CollectionsApi.md#fetch_user_collections_v2) | **GET** /api/v2/users/{userId}/collections/status/active | UserCollectionController@indexActive
[**fetch_user_draft_collections_v2**](CollectionsApi.md#fetch_user_draft_collections_v2) | **GET** /api/v2/users/{userId}/collections/status/draft | UserCollectionController@indexDraft


# **a18eed83ffe8ac895df3e1efa5ffb421**
> FetchCollections200Response a18eed83ffe8ac895df3e1efa5ffb421(team_id, id, a18eed83ffe8ac895df3e1efa5ffb421_request)

Update a collection

Update a collection owned by a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a18eed83ffe8ac895df3e1efa5ffb421_request import A18eed83ffe8ac895df3e1efa5ffb421Request
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
    team_id = 1 # int | team id
    id = 1 # int | collection id
    a18eed83ffe8ac895df3e1efa5ffb421_request = gateway_api_sdk.A18eed83ffe8ac895df3e1efa5ffb421Request() # A18eed83ffe8ac895df3e1efa5ffb421Request | Pass user credentials

    try:
        # Update a collection
        api_response = api_instance.a18eed83ffe8ac895df3e1efa5ffb421(team_id, id, a18eed83ffe8ac895df3e1efa5ffb421_request)
        print("The response of CollectionsApi->a18eed83ffe8ac895df3e1efa5ffb421:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->a18eed83ffe8ac895df3e1efa5ffb421: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| collection id | 
 **a18eed83ffe8ac895df3e1efa5ffb421_request** | [**A18eed83ffe8ac895df3e1efa5ffb421Request**](A18eed83ffe8ac895df3e1efa5ffb421Request.md)| Pass user credentials | 

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

# **b2e32406fe513dd0c0747a0864b5ed28**
> C29b5b3424f7317b69b4bda048ccfafb200Response b2e32406fe513dd0c0747a0864b5ed28(id)

Delete a collection

Delete a collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
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
        api_response = api_instance.b2e32406fe513dd0c0747a0864b5ed28(id)
        print("The response of CollectionsApi->b2e32406fe513dd0c0747a0864b5ed28:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->b2e32406fe513dd0c0747a0864b5ed28: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

# **call_22bf9932e93726b8338c13e489c7d96e**
> FetchCollections200Response call_22bf9932e93726b8338c13e489c7d96e(user_id, id, model8abb5928cecc676521f3e3d8eea0c49c_request)

Update a collection

Update a collection owned by an individual

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
from gateway_api_sdk.models.model8abb5928cecc676521f3e3d8eea0c49c_request import Model8abb5928cecc676521f3e3d8eea0c49cRequest
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
    user_id = 1 # int | user id
    id = 1 # int | collection id
    model8abb5928cecc676521f3e3d8eea0c49c_request = gateway_api_sdk.Model8abb5928cecc676521f3e3d8eea0c49cRequest() # Model8abb5928cecc676521f3e3d8eea0c49cRequest | Pass user credentials

    try:
        # Update a collection
        api_response = api_instance.call_22bf9932e93726b8338c13e489c7d96e(user_id, id, model8abb5928cecc676521f3e3d8eea0c49c_request)
        print("The response of CollectionsApi->call_22bf9932e93726b8338c13e489c7d96e:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_22bf9932e93726b8338c13e489c7d96e: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 
 **id** | **int**| collection id | 
 **model8abb5928cecc676521f3e3d8eea0c49c_request** | [**Model8abb5928cecc676521f3e3d8eea0c49cRequest**](Model8abb5928cecc676521f3e3d8eea0c49cRequest.md)| Pass user credentials | 

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

# **call_2e589ea17282e3818437328b1a6d2c45**
> FetchCollections200Response call_2e589ea17282e3818437328b1a6d2c45(team_id, id, model75c378b5764d9d73e14fe2d65c654910_request)

Edit a collection

Edit a collection owned by a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
from gateway_api_sdk.models.model75c378b5764d9d73e14fe2d65c654910_request import Model75c378b5764d9d73e14fe2d65c654910Request
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
    team_id = 1 # int | team id
    id = 1 # int | collection id
    model75c378b5764d9d73e14fe2d65c654910_request = gateway_api_sdk.Model75c378b5764d9d73e14fe2d65c654910Request() # Model75c378b5764d9d73e14fe2d65c654910Request | Pass user credentials

    try:
        # Edit a collection
        api_response = api_instance.call_2e589ea17282e3818437328b1a6d2c45(team_id, id, model75c378b5764d9d73e14fe2d65c654910_request)
        print("The response of CollectionsApi->call_2e589ea17282e3818437328b1a6d2c45:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_2e589ea17282e3818437328b1a6d2c45: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| collection id | 
 **model75c378b5764d9d73e14fe2d65c654910_request** | [**Model75c378b5764d9d73e14fe2d65c654910Request**](Model75c378b5764d9d73e14fe2d65c654910Request.md)| Pass user credentials | 

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

# **call_63175dd3a255646e0428a630af683e21**
> FetchCollections200Response call_63175dd3a255646e0428a630af683e21(user_id, id, d183a285f65bdc0e6341ed79b3a63670_request)

Edit a collection

Edit a collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.d183a285f65bdc0e6341ed79b3a63670_request import D183a285f65bdc0e6341ed79b3a63670Request
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
    user_id = 1 # int | user id
    id = 1 # int | collection id
    d183a285f65bdc0e6341ed79b3a63670_request = gateway_api_sdk.D183a285f65bdc0e6341ed79b3a63670Request() # D183a285f65bdc0e6341ed79b3a63670Request | Pass user credentials

    try:
        # Edit a collection
        api_response = api_instance.call_63175dd3a255646e0428a630af683e21(user_id, id, d183a285f65bdc0e6341ed79b3a63670_request)
        print("The response of CollectionsApi->call_63175dd3a255646e0428a630af683e21:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_63175dd3a255646e0428a630af683e21: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 
 **id** | **int**| collection id | 
 **d183a285f65bdc0e6341ed79b3a63670_request** | [**D183a285f65bdc0e6341ed79b3a63670Request**](D183a285f65bdc0e6341ed79b3a63670Request.md)| Pass user credentials | 

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

# **call_6907582348e596c660cc65263dc3a4fc**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_6907582348e596c660cc65263dc3a4fc(team_id, id)

Delete a collection

Delete a collection owned by a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
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
    team_id = 1 # int | team id
    id = 1 # int | collection id

    try:
        # Delete a collection
        api_response = api_instance.call_6907582348e596c660cc65263dc3a4fc(team_id, id)
        print("The response of CollectionsApi->call_6907582348e596c660cc65263dc3a4fc:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_6907582348e596c660cc65263dc3a4fc: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| collection id | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

# **call_75c378b5764d9d73e14fe2d65c654910**
> FetchCollections200Response call_75c378b5764d9d73e14fe2d65c654910(team_id, id, model75c378b5764d9d73e14fe2d65c654910_request, unarchive=unarchive)

Edit a collection

Edit a collection owned by a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
from gateway_api_sdk.models.model75c378b5764d9d73e14fe2d65c654910_request import Model75c378b5764d9d73e14fe2d65c654910Request
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
    team_id = 1 # int | team id
    id = 1 # int | collection id
    model75c378b5764d9d73e14fe2d65c654910_request = gateway_api_sdk.Model75c378b5764d9d73e14fe2d65c654910Request() # Model75c378b5764d9d73e14fe2d65c654910Request | Pass user credentials
    unarchive = 'unarchive_example' # str | Unarchive a collection (optional)

    try:
        # Edit a collection
        api_response = api_instance.call_75c378b5764d9d73e14fe2d65c654910(team_id, id, model75c378b5764d9d73e14fe2d65c654910_request, unarchive=unarchive)
        print("The response of CollectionsApi->call_75c378b5764d9d73e14fe2d65c654910:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_75c378b5764d9d73e14fe2d65c654910: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| collection id | 
 **model75c378b5764d9d73e14fe2d65c654910_request** | [**Model75c378b5764d9d73e14fe2d65c654910Request**](Model75c378b5764d9d73e14fe2d65c654910Request.md)| Pass user credentials | 
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

# **call_78c554f5fb0f01c8d788a5789fd0c35b**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_78c554f5fb0f01c8d788a5789fd0c35b(user_id, id)

Delete a collection

Delete a collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
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
    user_id = 1 # int | user id
    id = 1 # int | collection id

    try:
        # Delete a collection
        api_response = api_instance.call_78c554f5fb0f01c8d788a5789fd0c35b(user_id, id)
        print("The response of CollectionsApi->call_78c554f5fb0f01c8d788a5789fd0c35b:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_78c554f5fb0f01c8d788a5789fd0c35b: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 
 **id** | **int**| collection id | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

# **call_8abb5928cecc676521f3e3d8eea0c49c**
> FetchCollections200Response call_8abb5928cecc676521f3e3d8eea0c49c(id, model8abb5928cecc676521f3e3d8eea0c49c_request)

Update a collection

Update a collection owned by an individual

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_collections200_response import FetchCollections200Response
from gateway_api_sdk.models.model8abb5928cecc676521f3e3d8eea0c49c_request import Model8abb5928cecc676521f3e3d8eea0c49cRequest
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
    model8abb5928cecc676521f3e3d8eea0c49c_request = gateway_api_sdk.Model8abb5928cecc676521f3e3d8eea0c49cRequest() # Model8abb5928cecc676521f3e3d8eea0c49cRequest | Pass user credentials

    try:
        # Update a collection
        api_response = api_instance.call_8abb5928cecc676521f3e3d8eea0c49c(id, model8abb5928cecc676521f3e3d8eea0c49c_request)
        print("The response of CollectionsApi->call_8abb5928cecc676521f3e3d8eea0c49c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_8abb5928cecc676521f3e3d8eea0c49c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **model8abb5928cecc676521f3e3d8eea0c49c_request** | [**Model8abb5928cecc676521f3e3d8eea0c49cRequest**](Model8abb5928cecc676521f3e3d8eea0c49cRequest.md)| Pass user credentials | 

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

# **call_94ae4ab159160f6240a4bc00d2e6fe5f**
> FetchCollections200Response call_94ae4ab159160f6240a4bc00d2e6fe5f(team_id, id, a18eed83ffe8ac895df3e1efa5ffb421_request)

Update a collection

Update a collection owned by a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a18eed83ffe8ac895df3e1efa5ffb421_request import A18eed83ffe8ac895df3e1efa5ffb421Request
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
    team_id = 1 # int | team id
    id = 1 # int | collection id
    a18eed83ffe8ac895df3e1efa5ffb421_request = gateway_api_sdk.A18eed83ffe8ac895df3e1efa5ffb421Request() # A18eed83ffe8ac895df3e1efa5ffb421Request | Pass user credentials

    try:
        # Update a collection
        api_response = api_instance.call_94ae4ab159160f6240a4bc00d2e6fe5f(team_id, id, a18eed83ffe8ac895df3e1efa5ffb421_request)
        print("The response of CollectionsApi->call_94ae4ab159160f6240a4bc00d2e6fe5f:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_94ae4ab159160f6240a4bc00d2e6fe5f: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| collection id | 
 **a18eed83ffe8ac895df3e1efa5ffb421_request** | [**A18eed83ffe8ac895df3e1efa5ffb421Request**](A18eed83ffe8ac895df3e1efa5ffb421Request.md)| Pass user credentials | 

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

# **call_9c525a2aaf8e8a81cbcdf1a3033bb1bb**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_9c525a2aaf8e8a81cbcdf1a3033bb1bb(team_id, id)

Delete a collection

Delete a collection owned by a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
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
    team_id = 1 # int | team id
    id = 1 # int | collection id

    try:
        # Delete a collection
        api_response = api_instance.call_9c525a2aaf8e8a81cbcdf1a3033bb1bb(team_id, id)
        print("The response of CollectionsApi->call_9c525a2aaf8e8a81cbcdf1a3033bb1bb:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->call_9c525a2aaf8e8a81cbcdf1a3033bb1bb: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| collection id | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

# **count_team_unique_fields_collection_v2**
> CountUniqueFieldsCollections200Response count_team_unique_fields_collection_v2(team_id, var_field)

TeamCollectionController@count

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    team_id = 1 # int | team id
    var_field = 'status' # str | name of the field to perform a count on

    try:
        # TeamCollectionController@count
        api_response = api_instance.count_team_unique_fields_collection_v2(team_id, var_field)
        print("The response of CollectionsApi->count_team_unique_fields_collection_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->count_team_unique_fields_collection_v2: %s\n" % e)
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

# **count_user_unique_fields_collection_v2**
> CountUniqueFieldsCollections200Response count_user_unique_fields_collection_v2(user_id, var_field)

UserCollectionController@count

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
    api_instance = gateway_api_sdk.CollectionsApi(api_client)
    user_id = 1 # int | user id
    var_field = 'status' # str | name of the field to perform a count on

    try:
        # UserCollectionController@count
        api_response = api_instance.count_user_unique_fields_collection_v2(user_id, var_field)
        print("The response of CollectionsApi->count_user_unique_fields_collection_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->count_user_unique_fields_collection_v2: %s\n" % e)
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

# **create_collections**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_collections(create_collections_request)

CollectionController@store

Create a new collection owned by an individual

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_collections_request import CreateCollectionsRequest
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
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

[**Dd76b8d73b7ea8b4951f03d7c0904c92200Response**](Dd76b8d73b7ea8b4951f03d7c0904c92200Response.md)

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

# **create_team_collections**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_team_collections(team_id, create_team_collections_request)

CollectionController@store

Create a new collection for a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_team_collections_request import CreateTeamCollectionsRequest
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
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
    team_id = 1 # int | team id
    create_team_collections_request = gateway_api_sdk.CreateTeamCollectionsRequest() # CreateTeamCollectionsRequest | Pass user credentials

    try:
        # CollectionController@store
        api_response = api_instance.create_team_collections(team_id, create_team_collections_request)
        print("The response of CollectionsApi->create_team_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->create_team_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **create_team_collections_request** | [**CreateTeamCollectionsRequest**](CreateTeamCollectionsRequest.md)| Pass user credentials | 

### Return type

[**Dd76b8d73b7ea8b4951f03d7c0904c92200Response**](Dd76b8d73b7ea8b4951f03d7c0904c92200Response.md)

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

# **create_team_collections_v2**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_team_collections_v2(team_id, create_team_collections_request)

TeamCollectionController@store

Create a new collection for a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_team_collections_request import CreateTeamCollectionsRequest
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
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
    team_id = 1 # int | team id
    create_team_collections_request = gateway_api_sdk.CreateTeamCollectionsRequest() # CreateTeamCollectionsRequest | Pass user credentials

    try:
        # TeamCollectionController@store
        api_response = api_instance.create_team_collections_v2(team_id, create_team_collections_request)
        print("The response of CollectionsApi->create_team_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->create_team_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **create_team_collections_request** | [**CreateTeamCollectionsRequest**](CreateTeamCollectionsRequest.md)| Pass user credentials | 

### Return type

[**Dd76b8d73b7ea8b4951f03d7c0904c92200Response**](Dd76b8d73b7ea8b4951f03d7c0904c92200Response.md)

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

# **create_user_collections**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_user_collections(create_collections_request)

UserCollectionController@store

Create a new collection owned by an individual

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_collections_request import CreateCollectionsRequest
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
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
        # UserCollectionController@store
        api_response = api_instance.create_user_collections(create_collections_request)
        print("The response of CollectionsApi->create_user_collections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->create_user_collections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_collections_request** | [**CreateCollectionsRequest**](CreateCollectionsRequest.md)| Pass user credentials | 

### Return type

[**Dd76b8d73b7ea8b4951f03d7c0904c92200Response**](Dd76b8d73b7ea8b4951f03d7c0904c92200Response.md)

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

# **d183a285f65bdc0e6341ed79b3a63670**
> FetchCollections200Response d183a285f65bdc0e6341ed79b3a63670(id, d183a285f65bdc0e6341ed79b3a63670_request, unarchive=unarchive)

Edit a collection

Edit a collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.d183a285f65bdc0e6341ed79b3a63670_request import D183a285f65bdc0e6341ed79b3a63670Request
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
    d183a285f65bdc0e6341ed79b3a63670_request = gateway_api_sdk.D183a285f65bdc0e6341ed79b3a63670Request() # D183a285f65bdc0e6341ed79b3a63670Request | Pass user credentials
    unarchive = 'unarchive_example' # str | Unarchive a collection (optional)

    try:
        # Edit a collection
        api_response = api_instance.d183a285f65bdc0e6341ed79b3a63670(id, d183a285f65bdc0e6341ed79b3a63670_request, unarchive=unarchive)
        print("The response of CollectionsApi->d183a285f65bdc0e6341ed79b3a63670:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->d183a285f65bdc0e6341ed79b3a63670: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| collection id | 
 **d183a285f65bdc0e6341ed79b3a63670_request** | [**D183a285f65bdc0e6341ed79b3a63670Request**](D183a285f65bdc0e6341ed79b3a63670Request.md)| Pass user credentials | 
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

# **fetch_team_active_collections_v2**
> FetchAllCollections200Response fetch_team_active_collections_v2(team_id)

TeamCollectionController@indexActive

Returns a list of a teams collections

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
    team_id = 1 # int | team id

    try:
        # TeamCollectionController@indexActive
        api_response = api_instance.fetch_team_active_collections_v2(team_id)
        print("The response of CollectionsApi->fetch_team_active_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_team_active_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 

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

# **fetch_team_archived_collections_v2**
> FetchAllCollections200Response fetch_team_archived_collections_v2(team_id)

TeamCollectionController@indexArchived

Returns a list of a teams archived collections

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
    team_id = 1 # int | team id

    try:
        # TeamCollectionController@indexArchived
        api_response = api_instance.fetch_team_archived_collections_v2(team_id)
        print("The response of CollectionsApi->fetch_team_archived_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_team_archived_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 

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

# **fetch_team_collection_v2**
> FetchCollections200Response fetch_team_collection_v2(team_id, id)

TeamCollectionController@show

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
    team_id = 1 # int | team id
    id = 1 # int | collection id

    try:
        # TeamCollectionController@show
        api_response = api_instance.fetch_team_collection_v2(team_id, id)
        print("The response of CollectionsApi->fetch_team_collection_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_team_collection_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| collection id | 

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

# **fetch_team_draft_collections_v2**
> FetchAllCollections200Response fetch_team_draft_collections_v2(team_id)

TeamCollectionController@indexDraft

Returns a list of a teams draft collections

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
    team_id = 1 # int | team id

    try:
        # TeamCollectionController@indexDraft
        api_response = api_instance.fetch_team_draft_collections_v2(team_id)
        print("The response of CollectionsApi->fetch_team_draft_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_team_draft_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 

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

# **fetch_user_archived_collections_v2**
> FetchAllCollections200Response fetch_user_archived_collections_v2(user_id)

UserCollectionController@indexArchived

Returns a list of a users archived collections

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
    user_id = 1 # int | user id

    try:
        # UserCollectionController@indexArchived
        api_response = api_instance.fetch_user_archived_collections_v2(user_id)
        print("The response of CollectionsApi->fetch_user_archived_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_user_archived_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 

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

# **fetch_user_collection_v2**
> FetchCollections200Response fetch_user_collection_v2(user_id, id)

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
    user_id = 1 # int | user id
    id = 1 # int | collection id

    try:
        # CollectionController@show
        api_response = api_instance.fetch_user_collection_v2(user_id, id)
        print("The response of CollectionsApi->fetch_user_collection_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_user_collection_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 
 **id** | **int**| collection id | 

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

# **fetch_user_collections_v2**
> FetchAllCollections200Response fetch_user_collections_v2(user_id)

UserCollectionController@indexActive

Returns a list of a users collections

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
    user_id = 1 # int | user id

    try:
        # UserCollectionController@indexActive
        api_response = api_instance.fetch_user_collections_v2(user_id)
        print("The response of CollectionsApi->fetch_user_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_user_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 

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

# **fetch_user_draft_collections_v2**
> FetchAllCollections200Response fetch_user_draft_collections_v2(user_id)

UserCollectionController@indexDraft

Returns a list of a users draft collections

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
    user_id = 1 # int | user id

    try:
        # UserCollectionController@indexDraft
        api_response = api_instance.fetch_user_draft_collections_v2(user_id)
        print("The response of CollectionsApi->fetch_user_draft_collections_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CollectionsApi->fetch_user_draft_collections_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 

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

