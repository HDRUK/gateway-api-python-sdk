# gateway_api_sdk.AliasApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**alias_controllerindex**](AliasApi.md#alias_controllerindex) | **GET** /api/v1/aliases | List of aliases
[**alias_controllershow**](AliasApi.md#alias_controllershow) | **GET** /api/v1/aliases/{id} | Return a single alias
[**b801ec1af9f360216286166894719a1e**](AliasApi.md#b801ec1af9f360216286166894719a1e) | **PUT** /api/v1/aliases/{id} | AliasController@update
[**c29b5b3424f7317b69b4bda048ccfafb**](AliasApi.md#c29b5b3424f7317b69b4bda048ccfafb) | **DELETE** /api/v1/aliases/{id} | AliasController@destroy
[**call_079b2d545c7f4705016912f5de1bf444**](AliasApi.md#call_079b2d545c7f4705016912f5de1bf444) | **POST** /api/v1/aliases | AliasController@store
[**e93f53867884432d9a6b592066431af3**](AliasApi.md#e93f53867884432d9a6b592066431af3) | **PATCH** /api/v1/aliases/{id} | AliasController@edit


# **alias_controllerindex**
> AliasControllerIndex200Response alias_controllerindex()

List of aliases

Returns a list of aliases

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.alias_controller_index200_response import AliasControllerIndex200Response
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
        api_response = api_instance.alias_controllerindex()
        print("The response of AliasApi->alias_controllerindex:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->alias_controllerindex: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AliasControllerIndex200Response**](AliasControllerIndex200Response.md)

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

# **alias_controllershow**
> AliasControllerShow200Response alias_controllershow(id)

Return a single alias

Return a single alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.alias_controller_show200_response import AliasControllerShow200Response
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
        api_response = api_instance.alias_controllershow(id)
        print("The response of AliasApi->alias_controllershow:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->alias_controllershow: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 

### Return type

[**AliasControllerShow200Response**](AliasControllerShow200Response.md)

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

# **b801ec1af9f360216286166894719a1e**
> B801ec1af9f360216286166894719a1e200Response b801ec1af9f360216286166894719a1e(id, model079b2d545c7f4705016912f5de1bf444_request)

AliasController@update

Update a alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.b801ec1af9f360216286166894719a1e200_response import B801ec1af9f360216286166894719a1e200Response
from gateway_api_sdk.models.model079b2d545c7f4705016912f5de1bf444_request import Model079b2d545c7f4705016912f5de1bf444Request
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
    model079b2d545c7f4705016912f5de1bf444_request = gateway_api_sdk.Model079b2d545c7f4705016912f5de1bf444Request() # Model079b2d545c7f4705016912f5de1bf444Request | Alias definition

    try:
        # AliasController@update
        api_response = api_instance.b801ec1af9f360216286166894719a1e(id, model079b2d545c7f4705016912f5de1bf444_request)
        print("The response of AliasApi->b801ec1af9f360216286166894719a1e:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->b801ec1af9f360216286166894719a1e: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 
 **model079b2d545c7f4705016912f5de1bf444_request** | [**Model079b2d545c7f4705016912f5de1bf444Request**](Model079b2d545c7f4705016912f5de1bf444Request.md)| Alias definition | 

### Return type

[**B801ec1af9f360216286166894719a1e200Response**](B801ec1af9f360216286166894719a1e200Response.md)

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

# **c29b5b3424f7317b69b4bda048ccfafb**
> C29b5b3424f7317b69b4bda048ccfafb200Response c29b5b3424f7317b69b4bda048ccfafb(id)

AliasController@destroy

Delete an alias

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
    api_instance = gateway_api_sdk.AliasApi(api_client)
    id = 1 # int | alias id

    try:
        # AliasController@destroy
        api_response = api_instance.c29b5b3424f7317b69b4bda048ccfafb(id)
        print("The response of AliasApi->c29b5b3424f7317b69b4bda048ccfafb:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->c29b5b3424f7317b69b4bda048ccfafb: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 

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

# **call_079b2d545c7f4705016912f5de1bf444**
> Model079b2d545c7f4705016912f5de1bf444200Response call_079b2d545c7f4705016912f5de1bf444(model079b2d545c7f4705016912f5de1bf444_request)

AliasController@store

Creates a new alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model079b2d545c7f4705016912f5de1bf444200_response import Model079b2d545c7f4705016912f5de1bf444200Response
from gateway_api_sdk.models.model079b2d545c7f4705016912f5de1bf444_request import Model079b2d545c7f4705016912f5de1bf444Request
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
    model079b2d545c7f4705016912f5de1bf444_request = gateway_api_sdk.Model079b2d545c7f4705016912f5de1bf444Request() # Model079b2d545c7f4705016912f5de1bf444Request | Alias definition

    try:
        # AliasController@store
        api_response = api_instance.call_079b2d545c7f4705016912f5de1bf444(model079b2d545c7f4705016912f5de1bf444_request)
        print("The response of AliasApi->call_079b2d545c7f4705016912f5de1bf444:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->call_079b2d545c7f4705016912f5de1bf444: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model079b2d545c7f4705016912f5de1bf444_request** | [**Model079b2d545c7f4705016912f5de1bf444Request**](Model079b2d545c7f4705016912f5de1bf444Request.md)| Alias definition | 

### Return type

[**Model079b2d545c7f4705016912f5de1bf444200Response**](Model079b2d545c7f4705016912f5de1bf444200Response.md)

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

# **e93f53867884432d9a6b592066431af3**
> B801ec1af9f360216286166894719a1e200Response e93f53867884432d9a6b592066431af3(id, e93f53867884432d9a6b592066431af3_request)

AliasController@edit

Edit a alias

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.b801ec1af9f360216286166894719a1e200_response import B801ec1af9f360216286166894719a1e200Response
from gateway_api_sdk.models.e93f53867884432d9a6b592066431af3_request import E93f53867884432d9a6b592066431af3Request
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
    e93f53867884432d9a6b592066431af3_request = gateway_api_sdk.E93f53867884432d9a6b592066431af3Request() # E93f53867884432d9a6b592066431af3Request | Alias definition

    try:
        # AliasController@edit
        api_response = api_instance.e93f53867884432d9a6b592066431af3(id, e93f53867884432d9a6b592066431af3_request)
        print("The response of AliasApi->e93f53867884432d9a6b592066431af3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AliasApi->e93f53867884432d9a6b592066431af3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| alias id | 
 **e93f53867884432d9a6b592066431af3_request** | [**E93f53867884432d9a6b592066431af3Request**](E93f53867884432d9a6b592066431af3Request.md)| Alias definition | 

### Return type

[**B801ec1af9f360216286166894719a1e200Response**](B801ec1af9f360216286166894719a1e200Response.md)

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

