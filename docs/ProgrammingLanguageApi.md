# gateway_api_sdk.ProgrammingLanguageApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ac545f07640e752592440f34e55b1ed3**](ProgrammingLanguageApi.md#ac545f07640e752592440f34e55b1ed3) | **POST** /api/v1/programming_languages | ProgrammingLanguage@store
[**ac75502b12db43904eeea0400eb245d8**](ProgrammingLanguageApi.md#ac75502b12db43904eeea0400eb245d8) | **GET** /api/v1/programming_languages | ProgrammingLanguage@index
[**b50ca1696491e4e1ff3cc267fa7e71ee**](ProgrammingLanguageApi.md#b50ca1696491e4e1ff3cc267fa7e71ee) | **GET** /api/v1/programming_languages/{id} | ProgrammingLanguage@show
[**call_00f9ccd45119f11eb3044b4d61f9e79d**](ProgrammingLanguageApi.md#call_00f9ccd45119f11eb3044b4d61f9e79d) | **DELETE** /api/v1/programming_languages/{id} | ProgrammingLanguage@destroy
[**call_9a975e45459cd2614334b378875d3108**](ProgrammingLanguageApi.md#call_9a975e45459cd2614334b378875d3108) | **PATCH** /api/v1/programming_languages/{id} | ProgrammingLanguage@update
[**f65686cb0c089366a7c7f67bf528c957**](ProgrammingLanguageApi.md#f65686cb0c089366a7c7f67bf528c957) | **PUT** /api/v1/programming_languages/{id} | ProgrammingLanguage@update


# **ac545f07640e752592440f34e55b1ed3**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response ac545f07640e752592440f34e55b1ed3(dd76b8d73b7ea8b4951f03d7c0904c92_request)

ProgrammingLanguage@store

Creates a new system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92_request import Dd76b8d73b7ea8b4951f03d7c0904c92Request
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    dd76b8d73b7ea8b4951f03d7c0904c92_request = gateway_api_sdk.Dd76b8d73b7ea8b4951f03d7c0904c92Request() # Dd76b8d73b7ea8b4951f03d7c0904c92Request | Programming language definition

    try:
        # ProgrammingLanguage@store
        api_response = api_instance.ac545f07640e752592440f34e55b1ed3(dd76b8d73b7ea8b4951f03d7c0904c92_request)
        print("The response of ProgrammingLanguageApi->ac545f07640e752592440f34e55b1ed3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->ac545f07640e752592440f34e55b1ed3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dd76b8d73b7ea8b4951f03d7c0904c92_request** | [**Dd76b8d73b7ea8b4951f03d7c0904c92Request**](Dd76b8d73b7ea8b4951f03d7c0904c92Request.md)| Programming language definition | 

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

# **ac75502b12db43904eeea0400eb245d8**
> Ac75502b12db43904eeea0400eb245d8200Response ac75502b12db43904eeea0400eb245d8()

ProgrammingLanguage@index

Returns a list of programming languages enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.ac75502b12db43904eeea0400eb245d8200_response import Ac75502b12db43904eeea0400eb245d8200Response
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)

    try:
        # ProgrammingLanguage@index
        api_response = api_instance.ac75502b12db43904eeea0400eb245d8()
        print("The response of ProgrammingLanguageApi->ac75502b12db43904eeea0400eb245d8:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->ac75502b12db43904eeea0400eb245d8: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Ac75502b12db43904eeea0400eb245d8200Response**](Ac75502b12db43904eeea0400eb245d8200Response.md)

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

# **b50ca1696491e4e1ff3cc267fa7e71ee**
> B50ca1696491e4e1ff3cc267fa7e71ee200Response b50ca1696491e4e1ff3cc267fa7e71ee(id)

ProgrammingLanguage@show

Return a single system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.b50ca1696491e4e1ff3cc267fa7e71ee200_response import B50ca1696491e4e1ff3cc267fa7e71ee200Response
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id

    try:
        # ProgrammingLanguage@show
        api_response = api_instance.b50ca1696491e4e1ff3cc267fa7e71ee(id)
        print("The response of ProgrammingLanguageApi->b50ca1696491e4e1ff3cc267fa7e71ee:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->b50ca1696491e4e1ff3cc267fa7e71ee: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 

### Return type

[**B50ca1696491e4e1ff3cc267fa7e71ee200Response**](B50ca1696491e4e1ff3cc267fa7e71ee200Response.md)

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

# **call_00f9ccd45119f11eb3044b4d61f9e79d**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_00f9ccd45119f11eb3044b4d61f9e79d(id)

ProgrammingLanguage@destroy

Delete a system programming language

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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id

    try:
        # ProgrammingLanguage@destroy
        api_response = api_instance.call_00f9ccd45119f11eb3044b4d61f9e79d(id)
        print("The response of ProgrammingLanguageApi->call_00f9ccd45119f11eb3044b4d61f9e79d:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->call_00f9ccd45119f11eb3044b4d61f9e79d: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 

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

# **call_9a975e45459cd2614334b378875d3108**
> F65686cb0c089366a7c7f67bf528c957200Response call_9a975e45459cd2614334b378875d3108(id, a5f6e0a9550d3c58c50dda55412cd051_request)

ProgrammingLanguage@update

Edit a system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a5f6e0a9550d3c58c50dda55412cd051_request import A5f6e0a9550d3c58c50dda55412cd051Request
from gateway_api_sdk.models.f65686cb0c089366a7c7f67bf528c957200_response import F65686cb0c089366a7c7f67bf528c957200Response
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id
    a5f6e0a9550d3c58c50dda55412cd051_request = gateway_api_sdk.A5f6e0a9550d3c58c50dda55412cd051Request() # A5f6e0a9550d3c58c50dda55412cd051Request | ProgrammingLanguage definition

    try:
        # ProgrammingLanguage@update
        api_response = api_instance.call_9a975e45459cd2614334b378875d3108(id, a5f6e0a9550d3c58c50dda55412cd051_request)
        print("The response of ProgrammingLanguageApi->call_9a975e45459cd2614334b378875d3108:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->call_9a975e45459cd2614334b378875d3108: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 
 **a5f6e0a9550d3c58c50dda55412cd051_request** | [**A5f6e0a9550d3c58c50dda55412cd051Request**](A5f6e0a9550d3c58c50dda55412cd051Request.md)| ProgrammingLanguage definition | 

### Return type

[**F65686cb0c089366a7c7f67bf528c957200Response**](F65686cb0c089366a7c7f67bf528c957200Response.md)

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

# **f65686cb0c089366a7c7f67bf528c957**
> F65686cb0c089366a7c7f67bf528c957200Response f65686cb0c089366a7c7f67bf528c957(id, model988e8695bc991d7f8e40131db5ba7a76_request)

ProgrammingLanguage@update

Update a system programming language

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.f65686cb0c089366a7c7f67bf528c957200_response import F65686cb0c089366a7c7f67bf528c957200Response
from gateway_api_sdk.models.model988e8695bc991d7f8e40131db5ba7a76_request import Model988e8695bc991d7f8e40131db5ba7a76Request
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
    api_instance = gateway_api_sdk.ProgrammingLanguageApi(api_client)
    id = 1 # int | programming language id
    model988e8695bc991d7f8e40131db5ba7a76_request = gateway_api_sdk.Model988e8695bc991d7f8e40131db5ba7a76Request() # Model988e8695bc991d7f8e40131db5ba7a76Request | ProgrammingLanguage definition

    try:
        # ProgrammingLanguage@update
        api_response = api_instance.f65686cb0c089366a7c7f67bf528c957(id, model988e8695bc991d7f8e40131db5ba7a76_request)
        print("The response of ProgrammingLanguageApi->f65686cb0c089366a7c7f67bf528c957:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProgrammingLanguageApi->f65686cb0c089366a7c7f67bf528c957: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| programming language id | 
 **model988e8695bc991d7f8e40131db5ba7a76_request** | [**Model988e8695bc991d7f8e40131db5ba7a76Request**](Model988e8695bc991d7f8e40131db5ba7a76Request.md)| ProgrammingLanguage definition | 

### Return type

[**F65686cb0c089366a7c7f67bf528c957200Response**](F65686cb0c089366a7c7f67bf528c957200Response.md)

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

