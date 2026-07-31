# gateway_api_sdk.NotificationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**a5ca86d5f19ecac396cb830333f307da**](NotificationApi.md#a5ca86d5f19ecac396cb830333f307da) | **PATCH** /api/v1/notifications/{id} | Notification@edit
[**b4f86f6c4f52e080b246d560038cdc9b**](NotificationApi.md#b4f86f6c4f52e080b246d560038cdc9b) | **PUT** /api/v1/notifications/{id} | Notification@update
[**cac3bdde44f0be0512f7d05c0a6064e4**](NotificationApi.md#cac3bdde44f0be0512f7d05c0a6064e4) | **GET** /api/v1/notifications | Notification@index
[**call_1fd84d2c66035574da4902f416cbd96a**](NotificationApi.md#call_1fd84d2c66035574da4902f416cbd96a) | **POST** /api/v1/notifications | Notification@store
[**call_22581e4d73af25a9036c6610c7e8fc72**](NotificationApi.md#call_22581e4d73af25a9036c6610c7e8fc72) | **GET** /api/v1/notifications/{id} | Notification@show
[**call_3f8fe68ea04e79015d8aad5912cadbc1**](NotificationApi.md#call_3f8fe68ea04e79015d8aad5912cadbc1) | **DELETE** /api/v1/notifications/{id} | Notification@destroy


# **a5ca86d5f19ecac396cb830333f307da**
> B4f86f6c4f52e080b246d560038cdc9b200Response a5ca86d5f19ecac396cb830333f307da(id, a5ca86d5f19ecac396cb830333f307da_request)

Notification@edit

Edit a notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a5ca86d5f19ecac396cb830333f307da_request import A5ca86d5f19ecac396cb830333f307daRequest
from gateway_api_sdk.models.b4f86f6c4f52e080b246d560038cdc9b200_response import B4f86f6c4f52e080b246d560038cdc9b200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id
    a5ca86d5f19ecac396cb830333f307da_request = gateway_api_sdk.A5ca86d5f19ecac396cb830333f307daRequest() # A5ca86d5f19ecac396cb830333f307daRequest | Notification definition

    try:
        # Notification@edit
        api_response = api_instance.a5ca86d5f19ecac396cb830333f307da(id, a5ca86d5f19ecac396cb830333f307da_request)
        print("The response of NotificationApi->a5ca86d5f19ecac396cb830333f307da:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->a5ca86d5f19ecac396cb830333f307da: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 
 **a5ca86d5f19ecac396cb830333f307da_request** | [**A5ca86d5f19ecac396cb830333f307daRequest**](A5ca86d5f19ecac396cb830333f307daRequest.md)| Notification definition | 

### Return type

[**B4f86f6c4f52e080b246d560038cdc9b200Response**](B4f86f6c4f52e080b246d560038cdc9b200Response.md)

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

# **b4f86f6c4f52e080b246d560038cdc9b**
> B4f86f6c4f52e080b246d560038cdc9b200Response b4f86f6c4f52e080b246d560038cdc9b(id, model1fd84d2c66035574da4902f416cbd96a_request)

Notification@update

Update a notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.b4f86f6c4f52e080b246d560038cdc9b200_response import B4f86f6c4f52e080b246d560038cdc9b200Response
from gateway_api_sdk.models.model1fd84d2c66035574da4902f416cbd96a_request import Model1fd84d2c66035574da4902f416cbd96aRequest
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id
    model1fd84d2c66035574da4902f416cbd96a_request = gateway_api_sdk.Model1fd84d2c66035574da4902f416cbd96aRequest() # Model1fd84d2c66035574da4902f416cbd96aRequest | Notification definition

    try:
        # Notification@update
        api_response = api_instance.b4f86f6c4f52e080b246d560038cdc9b(id, model1fd84d2c66035574da4902f416cbd96a_request)
        print("The response of NotificationApi->b4f86f6c4f52e080b246d560038cdc9b:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->b4f86f6c4f52e080b246d560038cdc9b: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 
 **model1fd84d2c66035574da4902f416cbd96a_request** | [**Model1fd84d2c66035574da4902f416cbd96aRequest**](Model1fd84d2c66035574da4902f416cbd96aRequest.md)| Notification definition | 

### Return type

[**B4f86f6c4f52e080b246d560038cdc9b200Response**](B4f86f6c4f52e080b246d560038cdc9b200Response.md)

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

# **cac3bdde44f0be0512f7d05c0a6064e4**
> Cac3bdde44f0be0512f7d05c0a6064e4200Response cac3bdde44f0be0512f7d05c0a6064e4()

Notification@index

Returns a list of notifications enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.cac3bdde44f0be0512f7d05c0a6064e4200_response import Cac3bdde44f0be0512f7d05c0a6064e4200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)

    try:
        # Notification@index
        api_response = api_instance.cac3bdde44f0be0512f7d05c0a6064e4()
        print("The response of NotificationApi->cac3bdde44f0be0512f7d05c0a6064e4:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->cac3bdde44f0be0512f7d05c0a6064e4: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Cac3bdde44f0be0512f7d05c0a6064e4200Response**](Cac3bdde44f0be0512f7d05c0a6064e4200Response.md)

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

# **call_1fd84d2c66035574da4902f416cbd96a**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_1fd84d2c66035574da4902f416cbd96a(model1fd84d2c66035574da4902f416cbd96a_request)

Notification@store

Creates a new notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model1fd84d2c66035574da4902f416cbd96a_request import Model1fd84d2c66035574da4902f416cbd96aRequest
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    model1fd84d2c66035574da4902f416cbd96a_request = gateway_api_sdk.Model1fd84d2c66035574da4902f416cbd96aRequest() # Model1fd84d2c66035574da4902f416cbd96aRequest | Notification definition

    try:
        # Notification@store
        api_response = api_instance.call_1fd84d2c66035574da4902f416cbd96a(model1fd84d2c66035574da4902f416cbd96a_request)
        print("The response of NotificationApi->call_1fd84d2c66035574da4902f416cbd96a:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->call_1fd84d2c66035574da4902f416cbd96a: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model1fd84d2c66035574da4902f416cbd96a_request** | [**Model1fd84d2c66035574da4902f416cbd96aRequest**](Model1fd84d2c66035574da4902f416cbd96aRequest.md)| Notification definition | 

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

# **call_22581e4d73af25a9036c6610c7e8fc72**
> Model22581e4d73af25a9036c6610c7e8fc72200Response call_22581e4d73af25a9036c6610c7e8fc72(id)

Notification@show

Return a single notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model22581e4d73af25a9036c6610c7e8fc72200_response import Model22581e4d73af25a9036c6610c7e8fc72200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id

    try:
        # Notification@show
        api_response = api_instance.call_22581e4d73af25a9036c6610c7e8fc72(id)
        print("The response of NotificationApi->call_22581e4d73af25a9036c6610c7e8fc72:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->call_22581e4d73af25a9036c6610c7e8fc72: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 

### Return type

[**Model22581e4d73af25a9036c6610c7e8fc72200Response**](Model22581e4d73af25a9036c6610c7e8fc72200Response.md)

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

# **call_3f8fe68ea04e79015d8aad5912cadbc1**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_3f8fe68ea04e79015d8aad5912cadbc1(id)

Notification@destroy

Delete a notification

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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id

    try:
        # Notification@destroy
        api_response = api_instance.call_3f8fe68ea04e79015d8aad5912cadbc1(id)
        print("The response of NotificationApi->call_3f8fe68ea04e79015d8aad5912cadbc1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->call_3f8fe68ea04e79015d8aad5912cadbc1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 

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

