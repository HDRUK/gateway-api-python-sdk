# gateway_api_sdk.UserDataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_02454c833604944c4ab43341c54819b5**](UserDataAccessApplicationApi.md#call_02454c833604944c4ab43341c54819b5) | **GET** /api/v1/users/{userId}/dar/applications/count | UserDataAccessApplicationController@allCounts
[**call_34fca475ca3526cfda7bd59f33676ca9**](UserDataAccessApplicationApi.md#call_34fca475ca3526cfda7bd59f33676ca9) | **GET** /api/v1/users/{userId}/dar/applications/{id} | UserDataAccessApplicationController@show
[**call_3ed5d58afc4b6c7bb2d955fa4c0f1671**](UserDataAccessApplicationApi.md#call_3ed5d58afc4b6c7bb2d955fa4c0f1671) | **GET** /api/v1/users/{userId}/dar/applications | UserDataAccessApplicationController@index
[**call_7090c41ba0c1412e6f1e62c5d9db14ba**](UserDataAccessApplicationApi.md#call_7090c41ba0c1412e6f1e62c5d9db14ba) | **GET** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplicationController@showAnswers
[**call_7710dee56f16ff46e25d95111beb5ce0**](UserDataAccessApplicationApi.md#call_7710dee56f16ff46e25d95111beb5ce0) | **GET** /api/v1/users/{userId}/dar/applications/{id}/showHeader | UserDataAccessApplicationController@showHeader
[**call_7753eafda891afa178f7cbff9e66ff10**](UserDataAccessApplicationApi.md#call_7753eafda891afa178f7cbff9e66ff10) | **GET** /api/v1/users/{userId}/dar/applications/count/{field} | UserDataAccessApplicationController@count
[**d05df7a52fe05d677aa184236d61de56**](UserDataAccessApplicationApi.md#d05df7a52fe05d677aa184236d61de56) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplication@storeAnswers


# **call_02454c833604944c4ab43341c54819b5**
> CountUniqueFieldsCollections200Response call_02454c833604944c4ab43341c54819b5(user_id)

UserDataAccessApplicationController@allCounts

Get Counts for all status fields in the model

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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id

    try:
        # UserDataAccessApplicationController@allCounts
        api_response = api_instance.call_02454c833604944c4ab43341c54819b5(user_id)
        print("The response of UserDataAccessApplicationApi->call_02454c833604944c4ab43341c54819b5:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->call_02454c833604944c4ab43341c54819b5: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 

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

# **call_34fca475ca3526cfda7bd59f33676ca9**
> Model4e4d590ec8943163168e4fc34bd166a1200Response call_34fca475ca3526cfda7bd59f33676ca9(user_id, id)

UserDataAccessApplicationController@show

Return a DAR application belonging to the user

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model4e4d590ec8943163168e4fc34bd166a1200_response import Model4e4d590ec8943163168e4fc34bd166a1200Response
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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id

    try:
        # UserDataAccessApplicationController@show
        api_response = api_instance.call_34fca475ca3526cfda7bd59f33676ca9(user_id, id)
        print("The response of UserDataAccessApplicationApi->call_34fca475ca3526cfda7bd59f33676ca9:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->call_34fca475ca3526cfda7bd59f33676ca9: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model4e4d590ec8943163168e4fc34bd166a1200Response**](Model4e4d590ec8943163168e4fc34bd166a1200Response.md)

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

# **call_3ed5d58afc4b6c7bb2d955fa4c0f1671**
> Model0ff8ad69b213abf8d671b3695d0b69b5200Response call_3ed5d58afc4b6c7bb2d955fa4c0f1671(user_id)

UserDataAccessApplicationController@index

List of dar applications belonging to a user

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model0ff8ad69b213abf8d671b3695d0b69b5200_response import Model0ff8ad69b213abf8d671b3695d0b69b5200Response
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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id

    try:
        # UserDataAccessApplicationController@index
        api_response = api_instance.call_3ed5d58afc4b6c7bb2d955fa4c0f1671(user_id)
        print("The response of UserDataAccessApplicationApi->call_3ed5d58afc4b6c7bb2d955fa4c0f1671:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->call_3ed5d58afc4b6c7bb2d955fa4c0f1671: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 

### Return type

[**Model0ff8ad69b213abf8d671b3695d0b69b5200Response**](Model0ff8ad69b213abf8d671b3695d0b69b5200Response.md)

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

# **call_7090c41ba0c1412e6f1e62c5d9db14ba**
> Model473ee45c3962ae2a02abbac5015dce6a200Response call_7090c41ba0c1412e6f1e62c5d9db14ba(user_id, id)

UserDataAccessApplicationController@showAnswers

Return answers from the user's DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model473ee45c3962ae2a02abbac5015dce6a200_response import Model473ee45c3962ae2a02abbac5015dce6a200Response
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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id

    try:
        # UserDataAccessApplicationController@showAnswers
        api_response = api_instance.call_7090c41ba0c1412e6f1e62c5d9db14ba(user_id, id)
        print("The response of UserDataAccessApplicationApi->call_7090c41ba0c1412e6f1e62c5d9db14ba:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->call_7090c41ba0c1412e6f1e62c5d9db14ba: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model473ee45c3962ae2a02abbac5015dce6a200Response**](Model473ee45c3962ae2a02abbac5015dce6a200Response.md)

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

# **call_7710dee56f16ff46e25d95111beb5ce0**
> Model4e4d590ec8943163168e4fc34bd166a1200Response call_7710dee56f16ff46e25d95111beb5ce0(user_id, id)

UserDataAccessApplicationController@showHeader

Get header information about a specific DAR

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model4e4d590ec8943163168e4fc34bd166a1200_response import Model4e4d590ec8943163168e4fc34bd166a1200Response
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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id

    try:
        # UserDataAccessApplicationController@showHeader
        api_response = api_instance.call_7710dee56f16ff46e25d95111beb5ce0(user_id, id)
        print("The response of UserDataAccessApplicationApi->call_7710dee56f16ff46e25d95111beb5ce0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->call_7710dee56f16ff46e25d95111beb5ce0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model4e4d590ec8943163168e4fc34bd166a1200Response**](Model4e4d590ec8943163168e4fc34bd166a1200Response.md)

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

# **call_7753eafda891afa178f7cbff9e66ff10**
> CountUniqueFieldsCollections200Response call_7753eafda891afa178f7cbff9e66ff10(user_id, var_field)

UserDataAccessApplicationController@count

Get Counts for distinct entries of a field in the model

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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    var_field = 'approval_status' # str | name of the field to perform a count on

    try:
        # UserDataAccessApplicationController@count
        api_response = api_instance.call_7753eafda891afa178f7cbff9e66ff10(user_id, var_field)
        print("The response of UserDataAccessApplicationApi->call_7753eafda891afa178f7cbff9e66ff10:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->call_7753eafda891afa178f7cbff9e66ff10: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
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

# **d05df7a52fe05d677aa184236d61de56**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response d05df7a52fe05d677aa184236d61de56(user_id, id, d05df7a52fe05d677aa184236d61de56_request)

UserDataAccessApplication@storeAnswers

Add answers to the user's DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.d05df7a52fe05d677aa184236d61de56_request import D05df7a52fe05d677aa184236d61de56Request
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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    d05df7a52fe05d677aa184236d61de56_request = gateway_api_sdk.D05df7a52fe05d677aa184236d61de56Request() # D05df7a52fe05d677aa184236d61de56Request | UserDataAccessApplication definition

    try:
        # UserDataAccessApplication@storeAnswers
        api_response = api_instance.d05df7a52fe05d677aa184236d61de56(user_id, id, d05df7a52fe05d677aa184236d61de56_request)
        print("The response of UserDataAccessApplicationApi->d05df7a52fe05d677aa184236d61de56:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->d05df7a52fe05d677aa184236d61de56: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **d05df7a52fe05d677aa184236d61de56_request** | [**D05df7a52fe05d677aa184236d61de56Request**](D05df7a52fe05d677aa184236d61de56Request.md)| UserDataAccessApplication definition | 

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

