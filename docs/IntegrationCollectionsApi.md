# gateway_api_sdk.IntegrationCollectionsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_03c4b87e83a5e290cee5b9bfd43f9b0d**](IntegrationCollectionsApi.md#call_03c4b87e83a5e290cee5b9bfd43f9b0d) | **PUT** /api/v1/integrations/collections/{id} | Update a collection
[**call_9909f9e058a98d63144b44938dbb0939**](IntegrationCollectionsApi.md#call_9909f9e058a98d63144b44938dbb0939) | **DELETE** /api/v1/integrations/collections/{id} | Delete a collection
[**create_collections_integrations**](IntegrationCollectionsApi.md#create_collections_integrations) | **POST** /api/v1/integrations/collections | IntegrationCollectionController@store
[**e935d442a0adfe7fa4fffabbfd45512c**](IntegrationCollectionsApi.md#e935d442a0adfe7fa4fffabbfd45512c) | **PATCH** /api/v1/integrations/collections/{id} | Edit a collection
[**fetch_all_collections_integrations**](IntegrationCollectionsApi.md#fetch_all_collections_integrations) | **GET** /api/v1/integrations/collections | IntegrationCollectionController@index
[**fetch_collections_integrations**](IntegrationCollectionsApi.md#fetch_collections_integrations) | **GET** /api/v1/integrations/collections/{id} | IntegrationCollectionController@show


# **call_03c4b87e83a5e290cee5b9bfd43f9b0d**
> FetchCollections200Response call_03c4b87e83a5e290cee5b9bfd43f9b0d(id, a18eed83ffe8ac895df3e1efa5ffb421_request)

Update a collection

Update a collection

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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id
    a18eed83ffe8ac895df3e1efa5ffb421_request = gateway_api_sdk.A18eed83ffe8ac895df3e1efa5ffb421Request() # A18eed83ffe8ac895df3e1efa5ffb421Request | Pass user credentials

    try:
        # Update a collection
        api_response = api_instance.call_03c4b87e83a5e290cee5b9bfd43f9b0d(id, a18eed83ffe8ac895df3e1efa5ffb421_request)
        print("The response of IntegrationCollectionsApi->call_03c4b87e83a5e290cee5b9bfd43f9b0d:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->call_03c4b87e83a5e290cee5b9bfd43f9b0d: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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

# **call_9909f9e058a98d63144b44938dbb0939**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_9909f9e058a98d63144b44938dbb0939(id)

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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id

    try:
        # Delete a collection
        api_response = api_instance.call_9909f9e058a98d63144b44938dbb0939(id)
        print("The response of IntegrationCollectionsApi->call_9909f9e058a98d63144b44938dbb0939:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->call_9909f9e058a98d63144b44938dbb0939: %s\n" % e)
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

# **create_collections_integrations**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_collections_integrations(a18eed83ffe8ac895df3e1efa5ffb421_request)

IntegrationCollectionController@store

Create a new collection

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a18eed83ffe8ac895df3e1efa5ffb421_request import A18eed83ffe8ac895df3e1efa5ffb421Request
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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    a18eed83ffe8ac895df3e1efa5ffb421_request = gateway_api_sdk.A18eed83ffe8ac895df3e1efa5ffb421Request() # A18eed83ffe8ac895df3e1efa5ffb421Request | Pass user credentials

    try:
        # IntegrationCollectionController@store
        api_response = api_instance.create_collections_integrations(a18eed83ffe8ac895df3e1efa5ffb421_request)
        print("The response of IntegrationCollectionsApi->create_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->create_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **a18eed83ffe8ac895df3e1efa5ffb421_request** | [**A18eed83ffe8ac895df3e1efa5ffb421Request**](A18eed83ffe8ac895df3e1efa5ffb421Request.md)| Pass user credentials | 

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

# **e935d442a0adfe7fa4fffabbfd45512c**
> FetchCollections200Response e935d442a0adfe7fa4fffabbfd45512c(id, a18eed83ffe8ac895df3e1efa5ffb421_request)

Edit a collection

Edit a collection

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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id
    a18eed83ffe8ac895df3e1efa5ffb421_request = gateway_api_sdk.A18eed83ffe8ac895df3e1efa5ffb421Request() # A18eed83ffe8ac895df3e1efa5ffb421Request | Pass user credentials

    try:
        # Edit a collection
        api_response = api_instance.e935d442a0adfe7fa4fffabbfd45512c(id, a18eed83ffe8ac895df3e1efa5ffb421_request)
        print("The response of IntegrationCollectionsApi->e935d442a0adfe7fa4fffabbfd45512c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->e935d442a0adfe7fa4fffabbfd45512c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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

# **fetch_all_collections_integrations**
> FetchAllCollections200Response fetch_all_collections_integrations(name=name, per_page=per_page)

IntegrationCollectionController@index

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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    name = 'name_example' # str | Filter collections by name (optional)
    per_page = 1 # int | per page (optional)

    try:
        # IntegrationCollectionController@index
        api_response = api_instance.fetch_all_collections_integrations(name=name, per_page=per_page)
        print("The response of IntegrationCollectionsApi->fetch_all_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->fetch_all_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| Filter collections by name | [optional] 
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

# **fetch_collections_integrations**
> FetchCollections200Response fetch_collections_integrations(id)

IntegrationCollectionController@show

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
    api_instance = gateway_api_sdk.IntegrationCollectionsApi(api_client)
    id = 1 # int | collection id

    try:
        # IntegrationCollectionController@show
        api_response = api_instance.fetch_collections_integrations(id)
        print("The response of IntegrationCollectionsApi->fetch_collections_integrations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationCollectionsApi->fetch_collections_integrations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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

