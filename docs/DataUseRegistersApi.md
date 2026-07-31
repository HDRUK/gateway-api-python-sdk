# gateway_api_sdk.DataUseRegistersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_220a00f946309dea9f126baed550c9cd**](DataUseRegistersApi.md#call_220a00f946309dea9f126baed550c9cd) | **GET** /api/v2/dur/template | DurController@exportTemplate
[**call_2c16b33b0f6636db91657b64f4a7bbda**](DataUseRegistersApi.md#call_2c16b33b0f6636db91657b64f4a7bbda) | **PUT** /api/v1/dur/{id} | Update a dur by id
[**call_3d9acaab46169ca5e55cf017e9659f8e**](DataUseRegistersApi.md#call_3d9acaab46169ca5e55cf017e9659f8e) | **PATCH** /api/v1/dur/{id} | Edit a dur
[**call_491cd8b54449d3269b5d69d4d5732523**](DataUseRegistersApi.md#call_491cd8b54449d3269b5d69d4d5732523) | **GET** /api/v1/dur/template | DurController@exportTemplate
[**count_team_unique_fields_dur_v2**](DataUseRegistersApi.md#count_team_unique_fields_dur_v2) | **GET** /api/v2/teams/{teamId}/dur/count/{field} | TeamDurController@count
[**create_dur**](DataUseRegistersApi.md#create_dur) | **POST** /api/v1/dur | DurController@store
[**create_dur_by_team_v2**](DataUseRegistersApi.md#create_dur_by_team_v2) | **POST** /api/v2/teams/{teamId}/dur | TeamDurController@store
[**delete_durs_v2_by_team_id**](DataUseRegistersApi.md#delete_durs_v2_by_team_id) | **DELETE** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@destroy
[**e78bbbfec43b70397fd580225bb968ce**](DataUseRegistersApi.md#e78bbbfec43b70397fd580225bb968ce) | **DELETE** /api/v1/dur/{id} | Delete a dur
[**edit_durs_v2_by_team_id**](DataUseRegistersApi.md#edit_durs_v2_by_team_id) | **PATCH** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@edit
[**export_dur_v2**](DataUseRegistersApi.md#export_dur_v2) | **GET** /api/v2/dur/export | DurController@export
[**fetch_all_dur**](DataUseRegistersApi.md#fetch_all_dur) | **GET** /api/v1/dur | DurController@index
[**fetch_all_dur_v2**](DataUseRegistersApi.md#fetch_all_dur_v2) | **GET** /api/v2/dur | DurController@indexActive
[**fetch_all_team_dur_status**](DataUseRegistersApi.md#fetch_all_team_dur_status) | **GET** /api/v2/teams/{teamId}/dur/status/{status} | TeamDurController@indexStatus
[**fetch_dur_by_id**](DataUseRegistersApi.md#fetch_dur_by_id) | **GET** /api/v1/dur/{id} | DurController@show
[**fetch_dur_by_id_v2**](DataUseRegistersApi.md#fetch_dur_by_id_v2) | **GET** /api/v2/dur/{id} | DurController@showActive
[**fetch_dur_by_team_and_by_id_v2**](DataUseRegistersApi.md#fetch_dur_by_team_and_by_id_v2) | **GET** /api/v1/teams/{teamId}/dur/{id} | TeamDurController@show
[**update_dur_v2_by_team_id**](DataUseRegistersApi.md#update_dur_v2_by_team_id) | **PUT** /api/v2/teams/{teamId}/dur/{id} | TeamDurController@update
[**upload_dur**](DataUseRegistersApi.md#upload_dur) | **POST** /api/v1/dur/upload | DurController@upload


# **call_220a00f946309dea9f126baed550c9cd**
> object call_220a00f946309dea9f126baed550c9cd()

DurController@exportTemplate

Export Dur upload template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)

    try:
        # DurController@exportTemplate
        api_response = api_instance.call_220a00f946309dea9f126baed550c9cd()
        print("The response of DataUseRegistersApi->call_220a00f946309dea9f126baed550c9cd:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->call_220a00f946309dea9f126baed550c9cd: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | File download |  -  |
**401** | Unauthorized |  -  |
**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_2c16b33b0f6636db91657b64f4a7bbda**
> Model2c16b33b0f6636db91657b64f4a7bbda200Response call_2c16b33b0f6636db91657b64f4a7bbda(id, create_dur_request)

Update a dur by id

Update a dur

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_request import CreateDurRequest
from gateway_api_sdk.models.model2c16b33b0f6636db91657b64f4a7bbda200_response import Model2c16b33b0f6636db91657b64f4a7bbda200Response
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    id = 1 # int | dur id
    create_dur_request = gateway_api_sdk.CreateDurRequest() # CreateDurRequest | Pass user credentials

    try:
        # Update a dur by id
        api_response = api_instance.call_2c16b33b0f6636db91657b64f4a7bbda(id, create_dur_request)
        print("The response of DataUseRegistersApi->call_2c16b33b0f6636db91657b64f4a7bbda:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->call_2c16b33b0f6636db91657b64f4a7bbda: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dur id | 
 **create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md)| Pass user credentials | 

### Return type

[**Model2c16b33b0f6636db91657b64f4a7bbda200Response**](Model2c16b33b0f6636db91657b64f4a7bbda200Response.md)

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

# **call_3d9acaab46169ca5e55cf017e9659f8e**
> Model2c16b33b0f6636db91657b64f4a7bbda200Response call_3d9acaab46169ca5e55cf017e9659f8e(id, create_dur_request, unarchive=unarchive)

Edit a dur

Edit a dur

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_request import CreateDurRequest
from gateway_api_sdk.models.model2c16b33b0f6636db91657b64f4a7bbda200_response import Model2c16b33b0f6636db91657b64f4a7bbda200Response
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    id = 1 # int | dur id
    create_dur_request = gateway_api_sdk.CreateDurRequest() # CreateDurRequest | Pass user credentials
    unarchive = 'unarchive_example' # str | Unarchive a dur (optional)

    try:
        # Edit a dur
        api_response = api_instance.call_3d9acaab46169ca5e55cf017e9659f8e(id, create_dur_request, unarchive=unarchive)
        print("The response of DataUseRegistersApi->call_3d9acaab46169ca5e55cf017e9659f8e:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->call_3d9acaab46169ca5e55cf017e9659f8e: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dur id | 
 **create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md)| Pass user credentials | 
 **unarchive** | **str**| Unarchive a dur | [optional] 

### Return type

[**Model2c16b33b0f6636db91657b64f4a7bbda200Response**](Model2c16b33b0f6636db91657b64f4a7bbda200Response.md)

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

# **call_491cd8b54449d3269b5d69d4d5732523**
> object call_491cd8b54449d3269b5d69d4d5732523()

DurController@exportTemplate

Export Dur upload template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)

    try:
        # DurController@exportTemplate
        api_response = api_instance.call_491cd8b54449d3269b5d69d4d5732523()
        print("The response of DataUseRegistersApi->call_491cd8b54449d3269b5d69d4d5732523:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->call_491cd8b54449d3269b5d69d4d5732523: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | File download |  -  |
**401** | Unauthorized |  -  |
**404** | File Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **count_team_unique_fields_dur_v2**
> CountUniqueFieldsCollections200Response count_team_unique_fields_dur_v2(team_id, var_field)

TeamDurController@count

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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    team_id = 1 # int | team id
    var_field = 'status' # str | name of the field to perform a count on

    try:
        # TeamDurController@count
        api_response = api_instance.count_team_unique_fields_dur_v2(team_id, var_field)
        print("The response of DataUseRegistersApi->count_team_unique_fields_dur_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->count_team_unique_fields_dur_v2: %s\n" % e)
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

# **create_dur**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_dur(create_dur_request)

DurController@store

Create a new dur

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_request import CreateDurRequest
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    create_dur_request = gateway_api_sdk.CreateDurRequest() # CreateDurRequest | Pass user credentials

    try:
        # DurController@store
        api_response = api_instance.create_dur(create_dur_request)
        print("The response of DataUseRegistersApi->create_dur:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->create_dur: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md)| Pass user credentials | 

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

# **create_dur_by_team_v2**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_dur_by_team_v2(team_id, create_dur_request)

TeamDurController@store

Create a new dur by team v2

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_request import CreateDurRequest
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    team_id = 1 # int | team id
    create_dur_request = gateway_api_sdk.CreateDurRequest() # CreateDurRequest | Pass user credentials

    try:
        # TeamDurController@store
        api_response = api_instance.create_dur_by_team_v2(team_id, create_dur_request)
        print("The response of DataUseRegistersApi->create_dur_by_team_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->create_dur_by_team_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md)| Pass user credentials | 

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

# **delete_durs_v2_by_team_id**
> C29b5b3424f7317b69b4bda048ccfafb200Response delete_durs_v2_by_team_id(team_id, id)

TeamDurController@destroy

Delete a dur by team and id v2

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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | dur id

    try:
        # TeamDurController@destroy
        api_response = api_instance.delete_durs_v2_by_team_id(team_id, id)
        print("The response of DataUseRegistersApi->delete_durs_v2_by_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->delete_durs_v2_by_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| dur id | 

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

# **e78bbbfec43b70397fd580225bb968ce**
> C29b5b3424f7317b69b4bda048ccfafb200Response e78bbbfec43b70397fd580225bb968ce(id)

Delete a dur

Delete a dur

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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    id = 1 # int | dur id

    try:
        # Delete a dur
        api_response = api_instance.e78bbbfec43b70397fd580225bb968ce(id)
        print("The response of DataUseRegistersApi->e78bbbfec43b70397fd580225bb968ce:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->e78bbbfec43b70397fd580225bb968ce: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dur id | 

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

# **edit_durs_v2_by_team_id**
> Model2c16b33b0f6636db91657b64f4a7bbda200Response edit_durs_v2_by_team_id(team_id, id, create_dur_request)

TeamDurController@edit

Edit a dur by team v2

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_request import CreateDurRequest
from gateway_api_sdk.models.model2c16b33b0f6636db91657b64f4a7bbda200_response import Model2c16b33b0f6636db91657b64f4a7bbda200Response
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | dur id
    create_dur_request = gateway_api_sdk.CreateDurRequest() # CreateDurRequest | Pass user credentials

    try:
        # TeamDurController@edit
        api_response = api_instance.edit_durs_v2_by_team_id(team_id, id, create_dur_request)
        print("The response of DataUseRegistersApi->edit_durs_v2_by_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->edit_durs_v2_by_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| dur id | 
 **create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md)| Pass user credentials | 

### Return type

[**Model2c16b33b0f6636db91657b64f4a7bbda200Response**](Model2c16b33b0f6636db91657b64f4a7bbda200Response.md)

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

# **export_dur_v2**
> str export_dur_v2(id=id)

DurController@export

Export CSV of one or more DURs

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    id = 1 # int | dur id (optional)

    try:
        # DurController@export
        api_response = api_instance.export_dur_v2(id=id)
        print("The response of DataUseRegistersApi->export_dur_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->export_dur_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| dur id | [optional] 

### Return type

**str**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/csv, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | CSV file |  -  |
**401** | Unauthorized |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_dur**
> FetchAllDur200Response fetch_all_dur(sort=sort, project_title=project_title, per_page=per_page)

DurController@index

Returns a list of dur

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_dur200_response import FetchAllDur200Response
from gateway_api_sdk.models.project_title_ascupdated_at_asc import ProjectTitleAscupdatedAtAsc
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    sort = gateway_api_sdk.ProjectTitleAscupdatedAtAsc() # ProjectTitleAscupdatedAtAsc | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc (optional)
    project_title = 'project_title_example' # str | Filter tools by project title (optional)
    per_page = 1 # int | per page (optional)

    try:
        # DurController@index
        api_response = api_instance.fetch_all_dur(sort=sort, project_title=project_title, per_page=per_page)
        print("The response of DataUseRegistersApi->fetch_all_dur:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->fetch_all_dur: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sort** | [**ProjectTitleAscupdatedAtAsc**](.md)| Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc | [optional] 
 **project_title** | **str**| Filter tools by project title | [optional] 
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchAllDur200Response**](FetchAllDur200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_dur_v2**
> FetchAllDurV2200Response fetch_all_dur_v2(sort=sort, project_title=project_title, per_page=per_page, with_related=with_related)

DurController@indexActive

Returns a list of active dur

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_dur_v2200_response import FetchAllDurV2200Response
from gateway_api_sdk.models.project_title_ascupdated_at_asc import ProjectTitleAscupdatedAtAsc
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    sort = gateway_api_sdk.ProjectTitleAscupdatedAtAsc() # ProjectTitleAscupdatedAtAsc | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc (optional)
    project_title = 'project_title_example' # str | Filter tools by project title (optional)
    per_page = 1 # int | per page (optional)
    with_related = True # bool | Show related entities (optional)

    try:
        # DurController@indexActive
        api_response = api_instance.fetch_all_dur_v2(sort=sort, project_title=project_title, per_page=per_page, with_related=with_related)
        print("The response of DataUseRegistersApi->fetch_all_dur_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->fetch_all_dur_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sort** | [**ProjectTitleAscupdatedAtAsc**](.md)| Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc | [optional] 
 **project_title** | **str**| Filter tools by project title | [optional] 
 **per_page** | **int**| per page | [optional] 
 **with_related** | **bool**| Show related entities | [optional] 

### Return type

[**FetchAllDurV2200Response**](FetchAllDurV2200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_team_dur_status**
> FetchAllDur200Response fetch_all_team_dur_status(team_id, status, sort=sort, project_title=project_title, per_page=per_page, with_related=with_related)

TeamDurController@indexStatus

Returns a list of dur owned by this team with given status

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_dur200_response import FetchAllDur200Response
from gateway_api_sdk.models.project_title_ascupdated_at_asc import ProjectTitleAscupdatedAtAsc
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    team_id = 1 # int | team id
    status = 'active' # str | Status of the DUR (active, draft, or archived). Defaults to active if not provided. (default to 'active')
    sort = gateway_api_sdk.ProjectTitleAscupdatedAtAsc() # ProjectTitleAscupdatedAtAsc | Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc (optional)
    project_title = 'project_title_example' # str | Filter dur by project title (optional)
    per_page = 1 # int | per page (optional)
    with_related = True # bool | Show related entities (optional)

    try:
        # TeamDurController@indexStatus
        api_response = api_instance.fetch_all_team_dur_status(team_id, status, sort=sort, project_title=project_title, per_page=per_page, with_related=with_related)
        print("The response of DataUseRegistersApi->fetch_all_team_dur_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->fetch_all_team_dur_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **status** | **str**| Status of the DUR (active, draft, or archived). Defaults to active if not provided. | [default to &#39;active&#39;]
 **sort** | [**ProjectTitleAscupdatedAtAsc**](.md)| Sort fields in the format field:direction, e.g., project_title:asc,updated_at:asc | [optional] 
 **project_title** | **str**| Filter dur by project title | [optional] 
 **per_page** | **int**| per page | [optional] 
 **with_related** | **bool**| Show related entities | [optional] 

### Return type

[**FetchAllDur200Response**](FetchAllDur200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dur_by_id**
> FetchDurById200Response fetch_dur_by_id(id)

DurController@show

Get dur by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dur_by_id200_response import FetchDurById200Response
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    id = 1 # int | data use register id

    try:
        # DurController@show
        api_response = api_instance.fetch_dur_by_id(id)
        print("The response of DataUseRegistersApi->fetch_dur_by_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->fetch_dur_by_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| data use register id | 

### Return type

[**FetchDurById200Response**](FetchDurById200Response.md)

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

# **fetch_dur_by_id_v2**
> Model2c16b33b0f6636db91657b64f4a7bbda200Response fetch_dur_by_id_v2(id)

DurController@showActive

Get dur by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model2c16b33b0f6636db91657b64f4a7bbda200_response import Model2c16b33b0f6636db91657b64f4a7bbda200Response
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    id = 1 # int | data use register id

    try:
        # DurController@showActive
        api_response = api_instance.fetch_dur_by_id_v2(id)
        print("The response of DataUseRegistersApi->fetch_dur_by_id_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->fetch_dur_by_id_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| data use register id | 

### Return type

[**Model2c16b33b0f6636db91657b64f4a7bbda200Response**](Model2c16b33b0f6636db91657b64f4a7bbda200Response.md)

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

# **fetch_dur_by_team_and_by_id_v2**
> Model2c16b33b0f6636db91657b64f4a7bbda200Response fetch_dur_by_team_and_by_id_v2(team_id, id)

TeamDurController@show

Get dur by team id and by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model2c16b33b0f6636db91657b64f4a7bbda200_response import Model2c16b33b0f6636db91657b64f4a7bbda200Response
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | data use register id

    try:
        # TeamDurController@show
        api_response = api_instance.fetch_dur_by_team_and_by_id_v2(team_id, id)
        print("The response of DataUseRegistersApi->fetch_dur_by_team_and_by_id_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->fetch_dur_by_team_and_by_id_v2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| data use register id | 

### Return type

[**Model2c16b33b0f6636db91657b64f4a7bbda200Response**](Model2c16b33b0f6636db91657b64f4a7bbda200Response.md)

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

# **update_dur_v2_by_team_id**
> Model2c16b33b0f6636db91657b64f4a7bbda200Response update_dur_v2_by_team_id(team_id, id, create_dur_request)

TeamDurController@update

Update a dur by team and id v2

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dur_request import CreateDurRequest
from gateway_api_sdk.models.model2c16b33b0f6636db91657b64f4a7bbda200_response import Model2c16b33b0f6636db91657b64f4a7bbda200Response
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    team_id = 1 # int | team id
    id = 1 # int | dur id
    create_dur_request = gateway_api_sdk.CreateDurRequest() # CreateDurRequest | Pass user credentials

    try:
        # TeamDurController@update
        api_response = api_instance.update_dur_v2_by_team_id(team_id, id, create_dur_request)
        print("The response of DataUseRegistersApi->update_dur_v2_by_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->update_dur_v2_by_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **id** | **int**| dur id | 
 **create_dur_request** | [**CreateDurRequest**](CreateDurRequest.md)| Pass user credentials | 

### Return type

[**Model2c16b33b0f6636db91657b64f4a7bbda200Response**](Model2c16b33b0f6636db91657b64f4a7bbda200Response.md)

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

# **upload_dur**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response upload_dur(upload_dur_request)

DurController@upload

Create a new dur with upload data

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.upload_dur_request import UploadDurRequest
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
    api_instance = gateway_api_sdk.DataUseRegistersApi(api_client)
    upload_dur_request = gateway_api_sdk.UploadDurRequest() # UploadDurRequest | Pass user credentials

    try:
        # DurController@upload
        api_response = api_instance.upload_dur(upload_dur_request)
        print("The response of DataUseRegistersApi->upload_dur:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataUseRegistersApi->upload_dur: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **upload_dur_request** | [**UploadDurRequest**](UploadDurRequest.md)| Pass user credentials | 

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

