# gateway_api_sdk.DataProviderCollApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_data_provider_coll**](DataProviderCollApi.md#create_data_provider_coll) | **POST** /api/v1/data_provider_colls | DataProviderColl@store
[**delete_data_provider_coll**](DataProviderCollApi.md#delete_data_provider_coll) | **DELETE** /api/v1/data_provider_colls/{id} | DataProviderColl@destroy
[**edit_data_provider_coll**](DataProviderCollApi.md#edit_data_provider_coll) | **PATCH** /api/v1/data_provider_colls/{id} | DataProviderColl@edit
[**fetch_data_provider_coll**](DataProviderCollApi.md#fetch_data_provider_coll) | **GET** /api/v1/data_provider_colls/{id} | DataProviderColl@show
[**fetch_data_provider_coll_summary**](DataProviderCollApi.md#fetch_data_provider_coll_summary) | **GET** /api/v1/data_provider_colls/{id}/summary | DataProviderColl@showSummary
[**fetch_data_provider_colls**](DataProviderCollApi.md#fetch_data_provider_colls) | **GET** /api/v1/data_provider_colls | DataProviderColl@index
[**update_data_provider_coll**](DataProviderCollApi.md#update_data_provider_coll) | **PUT** /api/v1/data_provider_colls/{id} | DataProviderColl@update


# **create_data_provider_coll**
> CreateCategories200Response create_data_provider_coll(create_data_provider_coll_request)

DataProviderColl@store

Creates a new DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_data_provider_coll_request import CreateDataProviderCollRequest
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
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    create_data_provider_coll_request = gateway_api_sdk.CreateDataProviderCollRequest() # CreateDataProviderCollRequest | DataProviderColl definition

    try:
        # DataProviderColl@store
        api_response = api_instance.create_data_provider_coll(create_data_provider_coll_request)
        print("The response of DataProviderCollApi->create_data_provider_coll:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->create_data_provider_coll: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_data_provider_coll_request** | [**CreateDataProviderCollRequest**](CreateDataProviderCollRequest.md)| DataProviderColl definition | 

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

# **delete_data_provider_coll**
> DeleteAliases200Response delete_data_provider_coll(id)

DataProviderColl@destroy

Delete a DataProviderColl

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
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID

    try:
        # DataProviderColl@destroy
        api_response = api_instance.delete_data_provider_coll(id)
        print("The response of DataProviderCollApi->delete_data_provider_coll:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->delete_data_provider_coll: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 

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

# **edit_data_provider_coll**
> UpdateDataProviderColl200Response edit_data_provider_coll(id, edit_data_provider_coll_request)

DataProviderColl@edit

Edit a DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_data_provider_coll_request import EditDataProviderCollRequest
from gateway_api_sdk.models.update_data_provider_coll200_response import UpdateDataProviderColl200Response
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
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID
    edit_data_provider_coll_request = gateway_api_sdk.EditDataProviderCollRequest() # EditDataProviderCollRequest | DataProviderColl definition

    try:
        # DataProviderColl@edit
        api_response = api_instance.edit_data_provider_coll(id, edit_data_provider_coll_request)
        print("The response of DataProviderCollApi->edit_data_provider_coll:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->edit_data_provider_coll: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 
 **edit_data_provider_coll_request** | [**EditDataProviderCollRequest**](EditDataProviderCollRequest.md)| DataProviderColl definition | 

### Return type

[**UpdateDataProviderColl200Response**](UpdateDataProviderColl200Response.md)

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

# **fetch_data_provider_coll**
> FetchDataProviderColl200Response fetch_data_provider_coll(id)

DataProviderColl@show

Return a single DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_provider_coll200_response import FetchDataProviderColl200Response
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
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID

    try:
        # DataProviderColl@show
        api_response = api_instance.fetch_data_provider_coll(id)
        print("The response of DataProviderCollApi->fetch_data_provider_coll:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->fetch_data_provider_coll: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 

### Return type

[**FetchDataProviderColl200Response**](FetchDataProviderColl200Response.md)

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

# **fetch_data_provider_coll_summary**
> FetchDataProviderCollSummary200Response fetch_data_provider_coll_summary(id)

DataProviderColl@showSummary

Return a single DataProviderColl - summary

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_provider_coll_summary200_response import FetchDataProviderCollSummary200Response
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
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID - summary

    try:
        # DataProviderColl@showSummary
        api_response = api_instance.fetch_data_provider_coll_summary(id)
        print("The response of DataProviderCollApi->fetch_data_provider_coll_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->fetch_data_provider_coll_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID - summary | 

### Return type

[**FetchDataProviderCollSummary200Response**](FetchDataProviderCollSummary200Response.md)

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

# **fetch_data_provider_colls**
> FetchDataProviderColls200Response fetch_data_provider_colls(per_page=per_page)

DataProviderColl@index

Returns a list of DataProviderColls enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_provider_colls200_response import FetchDataProviderColls200Response
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
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # DataProviderColl@index
        api_response = api_instance.fetch_data_provider_colls(per_page=per_page)
        print("The response of DataProviderCollApi->fetch_data_provider_colls:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->fetch_data_provider_colls: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchDataProviderColls200Response**](FetchDataProviderColls200Response.md)

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

# **update_data_provider_coll**
> UpdateDataProviderColl200Response update_data_provider_coll(id, update_data_provider_coll_request)

DataProviderColl@update

Update a DataProviderColl

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_data_provider_coll200_response import UpdateDataProviderColl200Response
from gateway_api_sdk.models.update_data_provider_coll_request import UpdateDataProviderCollRequest
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
    api_instance = gateway_api_sdk.DataProviderCollApi(api_client)
    id = 1 # int | DataProviderColl ID
    update_data_provider_coll_request = gateway_api_sdk.UpdateDataProviderCollRequest() # UpdateDataProviderCollRequest | DataProviderColl definition

    try:
        # DataProviderColl@update
        api_response = api_instance.update_data_provider_coll(id, update_data_provider_coll_request)
        print("The response of DataProviderCollApi->update_data_provider_coll:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataProviderCollApi->update_data_provider_coll: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataProviderColl ID | 
 **update_data_provider_coll_request** | [**UpdateDataProviderCollRequest**](UpdateDataProviderCollRequest.md)| DataProviderColl definition | 

### Return type

[**UpdateDataProviderColl200Response**](UpdateDataProviderColl200Response.md)

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

