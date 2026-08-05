# gateway_api_sdk.DataCustodianNetworksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_data_custodian_network**](DataCustodianNetworksApi.md#create_data_custodian_network) | **POST** /api/v2/data_custodian_networks | DataCustodianNetworks@store
[**delete_data_custodian_network**](DataCustodianNetworksApi.md#delete_data_custodian_network) | **DELETE** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@destroy
[**edit_data_custodian_network**](DataCustodianNetworksApi.md#edit_data_custodian_network) | **PATCH** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@edit
[**fetch_data_custodian_network**](DataCustodianNetworksApi.md#fetch_data_custodian_network) | **GET** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@show
[**fetch_data_custodian_network_custodians_summary**](DataCustodianNetworksApi.md#fetch_data_custodian_network_custodians_summary) | **GET** /api/v2/data_custodian_networks/{id}/custodians_summary | DataCustodianNetworks@showCustodiansSummary
[**fetch_data_custodian_network_datasets_summary**](DataCustodianNetworksApi.md#fetch_data_custodian_network_datasets_summary) | **GET** /api/v2/data_custodian_networks/{id}/datasets_summary | DataCustodianNetworks@showDatasetsSummary
[**fetch_data_custodian_network_entities_summary**](DataCustodianNetworksApi.md#fetch_data_custodian_network_entities_summary) | **GET** /api/v2/data_custodian_networks/{id}/entities_summary | DataCustodianNetworks@showSummary
[**fetch_data_custodian_network_info**](DataCustodianNetworksApi.md#fetch_data_custodian_network_info) | **GET** /api/v2/data_custodian_networks/{id}/info | DataCustodianNetworks@showInfoSummary
[**fetch_data_custodian_networks**](DataCustodianNetworksApi.md#fetch_data_custodian_networks) | **GET** /api/v2/data_custodian_networks | DataCustodianNetworks@index
[**update_data_custodian_network**](DataCustodianNetworksApi.md#update_data_custodian_network) | **PUT** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@update


# **create_data_custodian_network**
> CreateDarIntegration201Response create_data_custodian_network(create_data_provider_coll_request)

DataCustodianNetworks@store

Creates a new DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    create_data_provider_coll_request = gateway_api_sdk.CreateDataProviderCollRequest() # CreateDataProviderCollRequest | DataCustodianNetwork definition

    try:
        # DataCustodianNetworks@store
        api_response = api_instance.create_data_custodian_network(create_data_provider_coll_request)
        print("The response of DataCustodianNetworksApi->create_data_custodian_network:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->create_data_custodian_network: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_data_provider_coll_request** | [**CreateDataProviderCollRequest**](CreateDataProviderCollRequest.md)| DataCustodianNetwork definition | 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_data_custodian_network**
> DeleteApplications200Response delete_data_custodian_network(id)

DataCustodianNetworks@destroy

Delete a DataCustodianNetwork

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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID

    try:
        # DataCustodianNetworks@destroy
        api_response = api_instance.delete_data_custodian_network(id)
        print("The response of DataCustodianNetworksApi->delete_data_custodian_network:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->delete_data_custodian_network: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID | 

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

# **edit_data_custodian_network**
> UpdateDataCustodianNetwork200Response edit_data_custodian_network(id, edit_data_provider_coll_request)

DataCustodianNetworks@edit

Edit a DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_data_provider_coll_request import EditDataProviderCollRequest
from gateway_api_sdk.models.update_data_custodian_network200_response import UpdateDataCustodianNetwork200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID
    edit_data_provider_coll_request = gateway_api_sdk.EditDataProviderCollRequest() # EditDataProviderCollRequest | DataCustodianNetwork definition

    try:
        # DataCustodianNetworks@edit
        api_response = api_instance.edit_data_custodian_network(id, edit_data_provider_coll_request)
        print("The response of DataCustodianNetworksApi->edit_data_custodian_network:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->edit_data_custodian_network: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID | 
 **edit_data_provider_coll_request** | [**EditDataProviderCollRequest**](EditDataProviderCollRequest.md)| DataCustodianNetwork definition | 

### Return type

[**UpdateDataCustodianNetwork200Response**](UpdateDataCustodianNetwork200Response.md)

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

# **fetch_data_custodian_network**
> FetchDataCustodianNetwork200Response fetch_data_custodian_network(id)

DataCustodianNetworks@show

Return a single DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_custodian_network200_response import FetchDataCustodianNetwork200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID

    try:
        # DataCustodianNetworks@show
        api_response = api_instance.fetch_data_custodian_network(id)
        print("The response of DataCustodianNetworksApi->fetch_data_custodian_network:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->fetch_data_custodian_network: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID | 

### Return type

[**FetchDataCustodianNetwork200Response**](FetchDataCustodianNetwork200Response.md)

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

# **fetch_data_custodian_network_custodians_summary**
> FetchDataCustodianNetworkCustodiansSummary200Response fetch_data_custodian_network_custodians_summary(id)

DataCustodianNetworks@showCustodiansSummary

Return a single DataCustodianNetwork - custodians summary

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_custodian_network_custodians_summary200_response import FetchDataCustodianNetworkCustodiansSummary200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID - summary

    try:
        # DataCustodianNetworks@showCustodiansSummary
        api_response = api_instance.fetch_data_custodian_network_custodians_summary(id)
        print("The response of DataCustodianNetworksApi->fetch_data_custodian_network_custodians_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->fetch_data_custodian_network_custodians_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**FetchDataCustodianNetworkCustodiansSummary200Response**](FetchDataCustodianNetworkCustodiansSummary200Response.md)

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

# **fetch_data_custodian_network_datasets_summary**
> FetchDataCustodianNetworkDatasetsSummary200Response fetch_data_custodian_network_datasets_summary(id)

DataCustodianNetworks@showDatasetsSummary

Return a single DataCustodianNetwork - summary of datasets

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_custodian_network_datasets_summary200_response import FetchDataCustodianNetworkDatasetsSummary200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID - summary

    try:
        # DataCustodianNetworks@showDatasetsSummary
        api_response = api_instance.fetch_data_custodian_network_datasets_summary(id)
        print("The response of DataCustodianNetworksApi->fetch_data_custodian_network_datasets_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->fetch_data_custodian_network_datasets_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**FetchDataCustodianNetworkDatasetsSummary200Response**](FetchDataCustodianNetworkDatasetsSummary200Response.md)

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

# **fetch_data_custodian_network_entities_summary**
> FetchDataCustodianNetworkEntitiesSummary200Response fetch_data_custodian_network_entities_summary(id)

DataCustodianNetworks@showSummary

Return a single DataCustodianNetwork - summary of entities

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_custodian_network_entities_summary200_response import FetchDataCustodianNetworkEntitiesSummary200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID - summary

    try:
        # DataCustodianNetworks@showSummary
        api_response = api_instance.fetch_data_custodian_network_entities_summary(id)
        print("The response of DataCustodianNetworksApi->fetch_data_custodian_network_entities_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->fetch_data_custodian_network_entities_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**FetchDataCustodianNetworkEntitiesSummary200Response**](FetchDataCustodianNetworkEntitiesSummary200Response.md)

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

# **fetch_data_custodian_network_info**
> FetchDataCustodianNetworkInfo200Response fetch_data_custodian_network_info(id)

DataCustodianNetworks@showInfoSummary

Return a single DataCustodianNetwork - basic information

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_custodian_network_info200_response import FetchDataCustodianNetworkInfo200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID - summary

    try:
        # DataCustodianNetworks@showInfoSummary
        api_response = api_instance.fetch_data_custodian_network_info(id)
        print("The response of DataCustodianNetworksApi->fetch_data_custodian_network_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->fetch_data_custodian_network_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**FetchDataCustodianNetworkInfo200Response**](FetchDataCustodianNetworkInfo200Response.md)

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

# **fetch_data_custodian_networks**
> FetchDataCustodianNetworks200Response fetch_data_custodian_networks(per_page=per_page)

DataCustodianNetworks@index

Returns a list of DataCustodianNetworks enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_data_custodian_networks200_response import FetchDataCustodianNetworks200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # DataCustodianNetworks@index
        api_response = api_instance.fetch_data_custodian_networks(per_page=per_page)
        print("The response of DataCustodianNetworksApi->fetch_data_custodian_networks:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->fetch_data_custodian_networks: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchDataCustodianNetworks200Response**](FetchDataCustodianNetworks200Response.md)

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

# **update_data_custodian_network**
> UpdateDataCustodianNetwork200Response update_data_custodian_network(id, update_data_provider_coll_request)

DataCustodianNetworks@update

Update a DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_data_custodian_network200_response import UpdateDataCustodianNetwork200Response
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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetworks ID
    update_data_provider_coll_request = gateway_api_sdk.UpdateDataProviderCollRequest() # UpdateDataProviderCollRequest | DataCustodianNetwork definition

    try:
        # DataCustodianNetworks@update
        api_response = api_instance.update_data_custodian_network(id, update_data_provider_coll_request)
        print("The response of DataCustodianNetworksApi->update_data_custodian_network:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->update_data_custodian_network: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetworks ID | 
 **update_data_provider_coll_request** | [**UpdateDataProviderCollRequest**](UpdateDataProviderCollRequest.md)| DataCustodianNetwork definition | 

### Return type

[**UpdateDataCustodianNetwork200Response**](UpdateDataCustodianNetwork200Response.md)

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

