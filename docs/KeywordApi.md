# gateway_api_sdk.KeywordApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**c144e4dec467e0666f1a6eb1b905a080**](KeywordApi.md#c144e4dec467e0666f1a6eb1b905a080) | **DELETE** /api/v1/keywords/{id} | KeywordController@destroy
[**call_5e7d6f311632134045864947649b04d4**](KeywordApi.md#call_5e7d6f311632134045864947649b04d4) | **PATCH** /api/v1/keywords/{id} | KeywordController@update
[**d59dbdaa4244200f6b9060e166e337d9**](KeywordApi.md#d59dbdaa4244200f6b9060e166e337d9) | **GET** /api/v1/keywords | KeywordController@index
[**ec00b8619507d4ac62cec63eb9684501**](KeywordApi.md#ec00b8619507d4ac62cec63eb9684501) | **POST** /api/v1/keywords | KeywordController@store
[**f2450127ddd5aa4ad77c822ba256e01a**](KeywordApi.md#f2450127ddd5aa4ad77c822ba256e01a) | **PUT** /api/v1/keywords/{id} | KeywordController@update
[**faadd5f355273c0ee61ef48436d03ded**](KeywordApi.md#faadd5f355273c0ee61ef48436d03ded) | **GET** /api/v1/keywords/{id} | KeywordController@show


# **c144e4dec467e0666f1a6eb1b905a080**
> C29b5b3424f7317b69b4bda048ccfafb200Response c144e4dec467e0666f1a6eb1b905a080(id)

KeywordController@destroy

Delete a keyword by id

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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id

    try:
        # KeywordController@destroy
        api_response = api_instance.c144e4dec467e0666f1a6eb1b905a080(id)
        print("The response of KeywordApi->c144e4dec467e0666f1a6eb1b905a080:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->c144e4dec467e0666f1a6eb1b905a080: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 

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

# **call_5e7d6f311632134045864947649b04d4**
> F2450127ddd5aa4ad77c822ba256e01a200Response call_5e7d6f311632134045864947649b04d4(id, a5f6e0a9550d3c58c50dda55412cd051_request)

KeywordController@update

Edit a keyword by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.a5f6e0a9550d3c58c50dda55412cd051_request import A5f6e0a9550d3c58c50dda55412cd051Request
from gateway_api_sdk.models.f2450127ddd5aa4ad77c822ba256e01a200_response import F2450127ddd5aa4ad77c822ba256e01a200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id
    a5f6e0a9550d3c58c50dda55412cd051_request = gateway_api_sdk.A5f6e0a9550d3c58c50dda55412cd051Request() # A5f6e0a9550d3c58c50dda55412cd051Request | Category definition

    try:
        # KeywordController@update
        api_response = api_instance.call_5e7d6f311632134045864947649b04d4(id, a5f6e0a9550d3c58c50dda55412cd051_request)
        print("The response of KeywordApi->call_5e7d6f311632134045864947649b04d4:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->call_5e7d6f311632134045864947649b04d4: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 
 **a5f6e0a9550d3c58c50dda55412cd051_request** | [**A5f6e0a9550d3c58c50dda55412cd051Request**](A5f6e0a9550d3c58c50dda55412cd051Request.md)| Category definition | 

### Return type

[**F2450127ddd5aa4ad77c822ba256e01a200Response**](F2450127ddd5aa4ad77c822ba256e01a200Response.md)

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

# **d59dbdaa4244200f6b9060e166e337d9**
> D59dbdaa4244200f6b9060e166e337d9200Response d59dbdaa4244200f6b9060e166e337d9(per_page=per_page)

KeywordController@index

Returns a list of keywords

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.d59dbdaa4244200f6b9060e166e337d9200_response import D59dbdaa4244200f6b9060e166e337d9200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    per_page = 56 # int | Alternative output schema version. (optional)

    try:
        # KeywordController@index
        api_response = api_instance.d59dbdaa4244200f6b9060e166e337d9(per_page=per_page)
        print("The response of KeywordApi->d59dbdaa4244200f6b9060e166e337d9:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->d59dbdaa4244200f6b9060e166e337d9: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| Alternative output schema version. | [optional] 

### Return type

[**D59dbdaa4244200f6b9060e166e337d9200Response**](D59dbdaa4244200f6b9060e166e337d9200Response.md)

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

# **ec00b8619507d4ac62cec63eb9684501**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response ec00b8619507d4ac62cec63eb9684501(dd76b8d73b7ea8b4951f03d7c0904c92_request)

KeywordController@store

Creates a new keyword

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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    dd76b8d73b7ea8b4951f03d7c0904c92_request = gateway_api_sdk.Dd76b8d73b7ea8b4951f03d7c0904c92Request() # Dd76b8d73b7ea8b4951f03d7c0904c92Request | Keyword definition

    try:
        # KeywordController@store
        api_response = api_instance.ec00b8619507d4ac62cec63eb9684501(dd76b8d73b7ea8b4951f03d7c0904c92_request)
        print("The response of KeywordApi->ec00b8619507d4ac62cec63eb9684501:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->ec00b8619507d4ac62cec63eb9684501: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dd76b8d73b7ea8b4951f03d7c0904c92_request** | [**Dd76b8d73b7ea8b4951f03d7c0904c92Request**](Dd76b8d73b7ea8b4951f03d7c0904c92Request.md)| Keyword definition | 

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
**409** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **f2450127ddd5aa4ad77c822ba256e01a**
> F2450127ddd5aa4ad77c822ba256e01a200Response f2450127ddd5aa4ad77c822ba256e01a(id, model988e8695bc991d7f8e40131db5ba7a76_request)

KeywordController@update

Update a keyword by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.f2450127ddd5aa4ad77c822ba256e01a200_response import F2450127ddd5aa4ad77c822ba256e01a200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id
    model988e8695bc991d7f8e40131db5ba7a76_request = gateway_api_sdk.Model988e8695bc991d7f8e40131db5ba7a76Request() # Model988e8695bc991d7f8e40131db5ba7a76Request | Keyword definition

    try:
        # KeywordController@update
        api_response = api_instance.f2450127ddd5aa4ad77c822ba256e01a(id, model988e8695bc991d7f8e40131db5ba7a76_request)
        print("The response of KeywordApi->f2450127ddd5aa4ad77c822ba256e01a:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->f2450127ddd5aa4ad77c822ba256e01a: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 
 **model988e8695bc991d7f8e40131db5ba7a76_request** | [**Model988e8695bc991d7f8e40131db5ba7a76Request**](Model988e8695bc991d7f8e40131db5ba7a76Request.md)| Keyword definition | 

### Return type

[**F2450127ddd5aa4ad77c822ba256e01a200Response**](F2450127ddd5aa4ad77c822ba256e01a200Response.md)

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

# **faadd5f355273c0ee61ef48436d03ded**
> Faadd5f355273c0ee61ef48436d03ded200Response faadd5f355273c0ee61ef48436d03ded(id)

KeywordController@show

Return a single keyword

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.faadd5f355273c0ee61ef48436d03ded200_response import Faadd5f355273c0ee61ef48436d03ded200Response
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
    api_instance = gateway_api_sdk.KeywordApi(api_client)
    id = 1 # int | keyword id

    try:
        # KeywordController@show
        api_response = api_instance.faadd5f355273c0ee61ef48436d03ded(id)
        print("The response of KeywordApi->faadd5f355273c0ee61ef48436d03ded:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling KeywordApi->faadd5f355273c0ee61ef48436d03ded: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| keyword id | 

### Return type

[**Faadd5f355273c0ee61ef48436d03ded200Response**](Faadd5f355273c0ee61ef48436d03ded200Response.md)

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

