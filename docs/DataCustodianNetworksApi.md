# gateway_api_sdk.DataCustodianNetworksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**abbd5469b6946b3822b4d156b522b03b**](DataCustodianNetworksApi.md#abbd5469b6946b3822b4d156b522b03b) | **POST** /api/v2/data_custodian_networks | DataCustodianNetworks@store
[**b42015102cb75735f63c91ed0c89aadc**](DataCustodianNetworksApi.md#b42015102cb75735f63c91ed0c89aadc) | **GET** /api/v2/data_custodian_networks/{id}/entities_summary | DataCustodianNetworks@showSummary
[**c7827b344f35440af530383c74573c6f**](DataCustodianNetworksApi.md#c7827b344f35440af530383c74573c6f) | **GET** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@show
[**call_0a51cc2388e3015851122c32c548b07e**](DataCustodianNetworksApi.md#call_0a51cc2388e3015851122c32c548b07e) | **PATCH** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@edit
[**call_3b69b09a466561df872e104a19a2ad65**](DataCustodianNetworksApi.md#call_3b69b09a466561df872e104a19a2ad65) | **GET** /api/v2/data_custodian_networks/{id}/datasets_summary | DataCustodianNetworks@showDatasetsSummary
[**call_5e9eca031c07d46c2fa4007e916bc5e1**](DataCustodianNetworksApi.md#call_5e9eca031c07d46c2fa4007e916bc5e1) | **DELETE** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@destroy
[**call_71e5fbca2b5aa8a0160d621feb662ecb**](DataCustodianNetworksApi.md#call_71e5fbca2b5aa8a0160d621feb662ecb) | **GET** /api/v2/data_custodian_networks | DataCustodianNetworks@index
[**call_9ce0c491d34067e8cf15eb9e9b5ec147**](DataCustodianNetworksApi.md#call_9ce0c491d34067e8cf15eb9e9b5ec147) | **GET** /api/v2/data_custodian_networks/{id}/info | DataCustodianNetworks@showInfoSummary
[**ced8add57941554cde6a5fc53f6555e5**](DataCustodianNetworksApi.md#ced8add57941554cde6a5fc53f6555e5) | **GET** /api/v2/data_custodian_networks/{id}/custodians_summary | DataCustodianNetworks@showCustodiansSummary
[**ddc2f5ebf51037175006c6017e20d358**](DataCustodianNetworksApi.md#ddc2f5ebf51037175006c6017e20d358) | **PUT** /api/v2/data_custodian_networks/{id} | DataCustodianNetworks@update


# **abbd5469b6946b3822b4d156b522b03b**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response abbd5469b6946b3822b4d156b522b03b(model02ada355a680c816624e98ae028dc8b6_request)

DataCustodianNetworks@store

Creates a new DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model02ada355a680c816624e98ae028dc8b6_request import Model02ada355a680c816624e98ae028dc8b6Request
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
    model02ada355a680c816624e98ae028dc8b6_request = gateway_api_sdk.Model02ada355a680c816624e98ae028dc8b6Request() # Model02ada355a680c816624e98ae028dc8b6Request | DataCustodianNetwork definition

    try:
        # DataCustodianNetworks@store
        api_response = api_instance.abbd5469b6946b3822b4d156b522b03b(model02ada355a680c816624e98ae028dc8b6_request)
        print("The response of DataCustodianNetworksApi->abbd5469b6946b3822b4d156b522b03b:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->abbd5469b6946b3822b4d156b522b03b: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model02ada355a680c816624e98ae028dc8b6_request** | [**Model02ada355a680c816624e98ae028dc8b6Request**](Model02ada355a680c816624e98ae028dc8b6Request.md)| DataCustodianNetwork definition | 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **b42015102cb75735f63c91ed0c89aadc**
> B42015102cb75735f63c91ed0c89aadc200Response b42015102cb75735f63c91ed0c89aadc(id)

DataCustodianNetworks@showSummary

Return a single DataCustodianNetwork - summary of entities

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.b42015102cb75735f63c91ed0c89aadc200_response import B42015102cb75735f63c91ed0c89aadc200Response
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
        api_response = api_instance.b42015102cb75735f63c91ed0c89aadc(id)
        print("The response of DataCustodianNetworksApi->b42015102cb75735f63c91ed0c89aadc:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->b42015102cb75735f63c91ed0c89aadc: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**B42015102cb75735f63c91ed0c89aadc200Response**](B42015102cb75735f63c91ed0c89aadc200Response.md)

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

# **c7827b344f35440af530383c74573c6f**
> C7827b344f35440af530383c74573c6f200Response c7827b344f35440af530383c74573c6f(id)

DataCustodianNetworks@show

Return a single DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c7827b344f35440af530383c74573c6f200_response import C7827b344f35440af530383c74573c6f200Response
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
        api_response = api_instance.c7827b344f35440af530383c74573c6f(id)
        print("The response of DataCustodianNetworksApi->c7827b344f35440af530383c74573c6f:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->c7827b344f35440af530383c74573c6f: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID | 

### Return type

[**C7827b344f35440af530383c74573c6f200Response**](C7827b344f35440af530383c74573c6f200Response.md)

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

# **call_0a51cc2388e3015851122c32c548b07e**
> Ddc2f5ebf51037175006c6017e20d358200Response call_0a51cc2388e3015851122c32c548b07e(id, model81b552b8803870790579d840279ce8a3_request)

DataCustodianNetworks@edit

Edit a DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.ddc2f5ebf51037175006c6017e20d358200_response import Ddc2f5ebf51037175006c6017e20d358200Response
from gateway_api_sdk.models.model81b552b8803870790579d840279ce8a3_request import Model81b552b8803870790579d840279ce8a3Request
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
    model81b552b8803870790579d840279ce8a3_request = gateway_api_sdk.Model81b552b8803870790579d840279ce8a3Request() # Model81b552b8803870790579d840279ce8a3Request | DataCustodianNetwork definition

    try:
        # DataCustodianNetworks@edit
        api_response = api_instance.call_0a51cc2388e3015851122c32c548b07e(id, model81b552b8803870790579d840279ce8a3_request)
        print("The response of DataCustodianNetworksApi->call_0a51cc2388e3015851122c32c548b07e:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->call_0a51cc2388e3015851122c32c548b07e: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID | 
 **model81b552b8803870790579d840279ce8a3_request** | [**Model81b552b8803870790579d840279ce8a3Request**](Model81b552b8803870790579d840279ce8a3Request.md)| DataCustodianNetwork definition | 

### Return type

[**Ddc2f5ebf51037175006c6017e20d358200Response**](Ddc2f5ebf51037175006c6017e20d358200Response.md)

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

# **call_3b69b09a466561df872e104a19a2ad65**
> Model3b69b09a466561df872e104a19a2ad65200Response call_3b69b09a466561df872e104a19a2ad65(id)

DataCustodianNetworks@showDatasetsSummary

Return a single DataCustodianNetwork - summary of datasets

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model3b69b09a466561df872e104a19a2ad65200_response import Model3b69b09a466561df872e104a19a2ad65200Response
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
        api_response = api_instance.call_3b69b09a466561df872e104a19a2ad65(id)
        print("The response of DataCustodianNetworksApi->call_3b69b09a466561df872e104a19a2ad65:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->call_3b69b09a466561df872e104a19a2ad65: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**Model3b69b09a466561df872e104a19a2ad65200Response**](Model3b69b09a466561df872e104a19a2ad65200Response.md)

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

# **call_5e9eca031c07d46c2fa4007e916bc5e1**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_5e9eca031c07d46c2fa4007e916bc5e1(id)

DataCustodianNetworks@destroy

Delete a DataCustodianNetwork

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
    api_instance = gateway_api_sdk.DataCustodianNetworksApi(api_client)
    id = 1 # int | DataCustodianNetwork ID

    try:
        # DataCustodianNetworks@destroy
        api_response = api_instance.call_5e9eca031c07d46c2fa4007e916bc5e1(id)
        print("The response of DataCustodianNetworksApi->call_5e9eca031c07d46c2fa4007e916bc5e1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->call_5e9eca031c07d46c2fa4007e916bc5e1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID | 

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

# **call_71e5fbca2b5aa8a0160d621feb662ecb**
> Model71e5fbca2b5aa8a0160d621feb662ecb200Response call_71e5fbca2b5aa8a0160d621feb662ecb(per_page=per_page)

DataCustodianNetworks@index

Returns a list of DataCustodianNetworks enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model71e5fbca2b5aa8a0160d621feb662ecb200_response import Model71e5fbca2b5aa8a0160d621feb662ecb200Response
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
        api_response = api_instance.call_71e5fbca2b5aa8a0160d621feb662ecb(per_page=per_page)
        print("The response of DataCustodianNetworksApi->call_71e5fbca2b5aa8a0160d621feb662ecb:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->call_71e5fbca2b5aa8a0160d621feb662ecb: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**Model71e5fbca2b5aa8a0160d621feb662ecb200Response**](Model71e5fbca2b5aa8a0160d621feb662ecb200Response.md)

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

# **call_9ce0c491d34067e8cf15eb9e9b5ec147**
> Model9ce0c491d34067e8cf15eb9e9b5ec147200Response call_9ce0c491d34067e8cf15eb9e9b5ec147(id)

DataCustodianNetworks@showInfoSummary

Return a single DataCustodianNetwork - basic information

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model9ce0c491d34067e8cf15eb9e9b5ec147200_response import Model9ce0c491d34067e8cf15eb9e9b5ec147200Response
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
        api_response = api_instance.call_9ce0c491d34067e8cf15eb9e9b5ec147(id)
        print("The response of DataCustodianNetworksApi->call_9ce0c491d34067e8cf15eb9e9b5ec147:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->call_9ce0c491d34067e8cf15eb9e9b5ec147: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**Model9ce0c491d34067e8cf15eb9e9b5ec147200Response**](Model9ce0c491d34067e8cf15eb9e9b5ec147200Response.md)

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

# **ced8add57941554cde6a5fc53f6555e5**
> Ced8add57941554cde6a5fc53f6555e5200Response ced8add57941554cde6a5fc53f6555e5(id)

DataCustodianNetworks@showCustodiansSummary

Return a single DataCustodianNetwork - custodians summary

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.ced8add57941554cde6a5fc53f6555e5200_response import Ced8add57941554cde6a5fc53f6555e5200Response
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
        api_response = api_instance.ced8add57941554cde6a5fc53f6555e5(id)
        print("The response of DataCustodianNetworksApi->ced8add57941554cde6a5fc53f6555e5:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->ced8add57941554cde6a5fc53f6555e5: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetwork ID - summary | 

### Return type

[**Ced8add57941554cde6a5fc53f6555e5200Response**](Ced8add57941554cde6a5fc53f6555e5200Response.md)

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

# **ddc2f5ebf51037175006c6017e20d358**
> Ddc2f5ebf51037175006c6017e20d358200Response ddc2f5ebf51037175006c6017e20d358(id, c5bb5300d6a46cc5b1b6a3bb1c3fa869_request)

DataCustodianNetworks@update

Update a DataCustodianNetwork

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c5bb5300d6a46cc5b1b6a3bb1c3fa869_request import C5bb5300d6a46cc5b1b6a3bb1c3fa869Request
from gateway_api_sdk.models.ddc2f5ebf51037175006c6017e20d358200_response import Ddc2f5ebf51037175006c6017e20d358200Response
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
    c5bb5300d6a46cc5b1b6a3bb1c3fa869_request = gateway_api_sdk.C5bb5300d6a46cc5b1b6a3bb1c3fa869Request() # C5bb5300d6a46cc5b1b6a3bb1c3fa869Request | DataCustodianNetwork definition

    try:
        # DataCustodianNetworks@update
        api_response = api_instance.ddc2f5ebf51037175006c6017e20d358(id, c5bb5300d6a46cc5b1b6a3bb1c3fa869_request)
        print("The response of DataCustodianNetworksApi->ddc2f5ebf51037175006c6017e20d358:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataCustodianNetworksApi->ddc2f5ebf51037175006c6017e20d358: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DataCustodianNetworks ID | 
 **c5bb5300d6a46cc5b1b6a3bb1c3fa869_request** | [**C5bb5300d6a46cc5b1b6a3bb1c3fa869Request**](C5bb5300d6a46cc5b1b6a3bb1c3fa869Request.md)| DataCustodianNetwork definition | 

### Return type

[**Ddc2f5ebf51037175006c6017e20d358200Response**](Ddc2f5ebf51037175006c6017e20d358200Response.md)

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

