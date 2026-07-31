# gateway_api_sdk.AliasApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_aliases**](AliasApi.md#create_aliases) | **POST** /api/v1/aliases | AliasController@store
[**delete_aliases**](AliasApi.md#delete_aliases) | **DELETE** /api/v1/aliases/{id} | AliasController@destroy
[**edit_aliases**](AliasApi.md#edit_aliases) | **PATCH** /api/v1/aliases/{id} | AliasController@edit
[**fetch_aliases**](AliasApi.md#fetch_aliases) | **GET** /api/v1/aliases/{id} | Return a single alias
[**fetch_all_aliases**](AliasApi.md#fetch_all_aliases) | **GET** /api/v1/aliases | List of aliases
[**update_aliases**](AliasApi.md#update_aliases) | **PUT** /api/v1/aliases/{id} | AliasController@update


# **create_aliases**
> CreateAliases200Response create_aliases(create_aliases_request)

AliasController@store

Creates a new alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_aliases200_response import CreateAliases200Response
from gateway_api_sdk.models.create_aliases_request import CreateAliasesRequest
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
    api_instance = gateway_api_sdk.AliasApi(api_client)
    create_aliases_request = gateway_api_sdk.CreateAliasesRequest() # CreateAliasesRequest | Alias definition

    try:
        # AliasController@store
        api_response = api_instance.create_aliases(create_aliases_request)
        print("The response of AliasApi->create_aliases:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->create_aliases: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_aliases_request** | [**CreateAliasesRequest**](CreateAliasesRequest.md)| Alias definition | 

### Return type

[**CreateAliases200Response**](CreateAliases200Response.md)

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

# **delete_aliases**
> DeleteAliases200Response delete_aliases(id)

AliasController@destroy

Delete an alias

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
    api_instance = gateway_api_sdk.AliasApi(api_client)
    id = 1 # int | alias id

    try:
        # AliasController@destroy
        api_response = api_instance.delete_aliases(id)
        print("The response of AliasApi->delete_aliases:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->delete_aliases: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 

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

# **edit_aliases**
> UpdateAliases200Response edit_aliases(id, edit_aliases_request)

AliasController@edit

Edit a alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_aliases_request import EditAliasesRequest
from gateway_api_sdk.models.update_aliases200_response import UpdateAliases200Response
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
    api_instance = gateway_api_sdk.AliasApi(api_client)
    id = 1 # int | alias id
    edit_aliases_request = gateway_api_sdk.EditAliasesRequest() # EditAliasesRequest | Alias definition

    try:
        # AliasController@edit
        api_response = api_instance.edit_aliases(id, edit_aliases_request)
        print("The response of AliasApi->edit_aliases:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->edit_aliases: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 
 **edit_aliases_request** | [**EditAliasesRequest**](EditAliasesRequest.md)| Alias definition | 

### Return type

[**UpdateAliases200Response**](UpdateAliases200Response.md)

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

# **fetch_aliases**
> FetchAliases200Response fetch_aliases(id)

Return a single alias

Return a single alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_aliases200_response import FetchAliases200Response
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
    api_instance = gateway_api_sdk.AliasApi(api_client)
    id = 1 # int | alias id

    try:
        # Return a single alias
        api_response = api_instance.fetch_aliases(id)
        print("The response of AliasApi->fetch_aliases:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->fetch_aliases: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 

### Return type

[**FetchAliases200Response**](FetchAliases200Response.md)

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

# **fetch_all_aliases**
> FetchAllAliases200Response fetch_all_aliases()

List of aliases

Returns a list of aliases

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_aliases200_response import FetchAllAliases200Response
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
    api_instance = gateway_api_sdk.AliasApi(api_client)

    try:
        # List of aliases
        api_response = api_instance.fetch_all_aliases()
        print("The response of AliasApi->fetch_all_aliases:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->fetch_all_aliases: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllAliases200Response**](FetchAllAliases200Response.md)

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

# **update_aliases**
> UpdateAliases200Response update_aliases(id, create_aliases_request)

AliasController@update

Update a alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_aliases_request import CreateAliasesRequest
from gateway_api_sdk.models.update_aliases200_response import UpdateAliases200Response
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
    api_instance = gateway_api_sdk.AliasApi(api_client)
    id = 1 # int | alias id
    create_aliases_request = gateway_api_sdk.CreateAliasesRequest() # CreateAliasesRequest | Alias definition

    try:
        # AliasController@update
        api_response = api_instance.update_aliases(id, create_aliases_request)
        print("The response of AliasApi->update_aliases:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->update_aliases: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 
 **create_aliases_request** | [**CreateAliasesRequest**](CreateAliasesRequest.md)| Alias definition | 

### Return type

[**UpdateAliases200Response**](UpdateAliases200Response.md)

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

