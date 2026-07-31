# gateway_api_sdk.DataAccessSectionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_0df3660c2b63970f84f9beec8a6c334e**](DataAccessSectionApi.md#call_0df3660c2b63970f84f9beec8a6c334e) | **DELETE** /api/v1/dar/sections/{id} | DataAccessSection@destroy
[**call_22b4daa2ab6ab3638657b9f6eee22316**](DataAccessSectionApi.md#call_22b4daa2ab6ab3638657b9f6eee22316) | **PUT** /api/v1/dar/sections/{id} | DataAccessSection@update
[**call_24bb1d73f780293f012cbc187f5448f3**](DataAccessSectionApi.md#call_24bb1d73f780293f012cbc187f5448f3) | **POST** /api/v1/dar/sections | DataAccessSection@store
[**call_2935b32e38ac989b35eab8e0b7552cd3**](DataAccessSectionApi.md#call_2935b32e38ac989b35eab8e0b7552cd3) | **PATCH** /api/v1/dar/sections/{id} | DataAccessSection@update
[**call_94f1c18e47daa32c1346be4a0d0449e4**](DataAccessSectionApi.md#call_94f1c18e47daa32c1346be4a0d0449e4) | **GET** /api/v1/dar/sections | DataAccessSection@index
[**fc0e1e343f76b10d80b2332ca24fbfe0**](DataAccessSectionApi.md#fc0e1e343f76b10d80b2332ca24fbfe0) | **GET** /api/v1/dar/sections/{id} | DataAccessSection@show


# **call_0df3660c2b63970f84f9beec8a6c334e**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_0df3660c2b63970f84f9beec8a6c334e(id)

DataAccessSection@destroy

Delete a system DAR section

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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id

    try:
        # DataAccessSection@destroy
        api_response = api_instance.call_0df3660c2b63970f84f9beec8a6c334e(id)
        print("The response of DataAccessSectionApi->call_0df3660c2b63970f84f9beec8a6c334e:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->call_0df3660c2b63970f84f9beec8a6c334e: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 

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

# **call_22b4daa2ab6ab3638657b9f6eee22316**
> Fc0e1e343f76b10d80b2332ca24fbfe0200Response call_22b4daa2ab6ab3638657b9f6eee22316(id, model24bb1d73f780293f012cbc187f5448f3_request)

DataAccessSection@update

Update a system DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fc0e1e343f76b10d80b2332ca24fbfe0200_response import Fc0e1e343f76b10d80b2332ca24fbfe0200Response
from gateway_api_sdk.models.model24bb1d73f780293f012cbc187f5448f3_request import Model24bb1d73f780293f012cbc187f5448f3Request
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id
    model24bb1d73f780293f012cbc187f5448f3_request = gateway_api_sdk.Model24bb1d73f780293f012cbc187f5448f3Request() # Model24bb1d73f780293f012cbc187f5448f3Request | DataAccessSection definition

    try:
        # DataAccessSection@update
        api_response = api_instance.call_22b4daa2ab6ab3638657b9f6eee22316(id, model24bb1d73f780293f012cbc187f5448f3_request)
        print("The response of DataAccessSectionApi->call_22b4daa2ab6ab3638657b9f6eee22316:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->call_22b4daa2ab6ab3638657b9f6eee22316: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 
 **model24bb1d73f780293f012cbc187f5448f3_request** | [**Model24bb1d73f780293f012cbc187f5448f3Request**](Model24bb1d73f780293f012cbc187f5448f3Request.md)| DataAccessSection definition | 

### Return type

[**Fc0e1e343f76b10d80b2332ca24fbfe0200Response**](Fc0e1e343f76b10d80b2332ca24fbfe0200Response.md)

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

# **call_24bb1d73f780293f012cbc187f5448f3**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_24bb1d73f780293f012cbc187f5448f3(model24bb1d73f780293f012cbc187f5448f3_request)

DataAccessSection@store

Creates a new DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model24bb1d73f780293f012cbc187f5448f3_request import Model24bb1d73f780293f012cbc187f5448f3Request
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    model24bb1d73f780293f012cbc187f5448f3_request = gateway_api_sdk.Model24bb1d73f780293f012cbc187f5448f3Request() # Model24bb1d73f780293f012cbc187f5448f3Request | DataAccessSection definition

    try:
        # DataAccessSection@store
        api_response = api_instance.call_24bb1d73f780293f012cbc187f5448f3(model24bb1d73f780293f012cbc187f5448f3_request)
        print("The response of DataAccessSectionApi->call_24bb1d73f780293f012cbc187f5448f3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->call_24bb1d73f780293f012cbc187f5448f3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model24bb1d73f780293f012cbc187f5448f3_request** | [**Model24bb1d73f780293f012cbc187f5448f3Request**](Model24bb1d73f780293f012cbc187f5448f3Request.md)| DataAccessSection definition | 

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

# **call_2935b32e38ac989b35eab8e0b7552cd3**
> Fc0e1e343f76b10d80b2332ca24fbfe0200Response call_2935b32e38ac989b35eab8e0b7552cd3(id, model2935b32e38ac989b35eab8e0b7552cd3_request)

DataAccessSection@update

Edit a system DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fc0e1e343f76b10d80b2332ca24fbfe0200_response import Fc0e1e343f76b10d80b2332ca24fbfe0200Response
from gateway_api_sdk.models.model2935b32e38ac989b35eab8e0b7552cd3_request import Model2935b32e38ac989b35eab8e0b7552cd3Request
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id
    model2935b32e38ac989b35eab8e0b7552cd3_request = gateway_api_sdk.Model2935b32e38ac989b35eab8e0b7552cd3Request() # Model2935b32e38ac989b35eab8e0b7552cd3Request | DataAccessSection definition

    try:
        # DataAccessSection@update
        api_response = api_instance.call_2935b32e38ac989b35eab8e0b7552cd3(id, model2935b32e38ac989b35eab8e0b7552cd3_request)
        print("The response of DataAccessSectionApi->call_2935b32e38ac989b35eab8e0b7552cd3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->call_2935b32e38ac989b35eab8e0b7552cd3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 
 **model2935b32e38ac989b35eab8e0b7552cd3_request** | [**Model2935b32e38ac989b35eab8e0b7552cd3Request**](Model2935b32e38ac989b35eab8e0b7552cd3Request.md)| DataAccessSection definition | 

### Return type

[**Fc0e1e343f76b10d80b2332ca24fbfe0200Response**](Fc0e1e343f76b10d80b2332ca24fbfe0200Response.md)

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

# **call_94f1c18e47daa32c1346be4a0d0449e4**
> Model94f1c18e47daa32c1346be4a0d0449e4200Response call_94f1c18e47daa32c1346be4a0d0449e4(per_page=per_page)

DataAccessSection@index

List of DAR sections

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model94f1c18e47daa32c1346be4a0d0449e4200_response import Model94f1c18e47daa32c1346be4a0d0449e4200Response
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # DataAccessSection@index
        api_response = api_instance.call_94f1c18e47daa32c1346be4a0d0449e4(per_page=per_page)
        print("The response of DataAccessSectionApi->call_94f1c18e47daa32c1346be4a0d0449e4:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->call_94f1c18e47daa32c1346be4a0d0449e4: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**Model94f1c18e47daa32c1346be4a0d0449e4200Response**](Model94f1c18e47daa32c1346be4a0d0449e4200Response.md)

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

# **fc0e1e343f76b10d80b2332ca24fbfe0**
> Fc0e1e343f76b10d80b2332ca24fbfe0200Response fc0e1e343f76b10d80b2332ca24fbfe0(id)

DataAccessSection@show

Return a single DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fc0e1e343f76b10d80b2332ca24fbfe0200_response import Fc0e1e343f76b10d80b2332ca24fbfe0200Response
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id

    try:
        # DataAccessSection@show
        api_response = api_instance.fc0e1e343f76b10d80b2332ca24fbfe0(id)
        print("The response of DataAccessSectionApi->fc0e1e343f76b10d80b2332ca24fbfe0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->fc0e1e343f76b10d80b2332ca24fbfe0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 

### Return type

[**Fc0e1e343f76b10d80b2332ca24fbfe0200Response**](Fc0e1e343f76b10d80b2332ca24fbfe0200Response.md)

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

