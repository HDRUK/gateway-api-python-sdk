# gateway_api_sdk.DataAccessApplicationReviewApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bdc71807f7e3ab85967e343d06f95228**](DataAccessApplicationReviewApi.md#bdc71807f7e3ab85967e343d06f95228) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews | DataAccessApplicationReview@store
[**call_05c982367b9c911ca1ec6d6352fa23fe**](DataAccessApplicationReviewApi.md#call_05c982367b9c911ca1ec6d6352fa23fe) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/files/{fileId} | DataAccessApplicationReview@destroyFile
[**call_154214db8250a7ff2fbbc9b6050ce1ab**](DataAccessApplicationReviewApi.md#call_154214db8250a7ff2fbbc9b6050ce1ab) | **GET** /ap1/v1/teams/{teamId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadFile
[**call_1fe1b50e52ecaba3d4a895720df962c7**](DataAccessApplicationReviewApi.md#call_1fe1b50e52ecaba3d4a895720df962c7) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@destroyGlobal
[**call_3f912cdc3d1bff9db206309ee384c782**](DataAccessApplicationReviewApi.md#call_3f912cdc3d1bff9db206309ee384c782) | **GET** /ap1/v1/users/{userId}/dar/applications/{id}/reviews/{reviewId}/download/{fileId} | DataAccessApplicationReview@downloadUserFile
[**call_53ba4c05c761d4787bfd1f1841d4b345**](DataAccessApplicationReviewApi.md#call_53ba4c05c761d4787bfd1f1841d4b345) | **DELETE** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@destroy
[**call_5766dcceb641169f89fecb537e8f79e4**](DataAccessApplicationReviewApi.md#call_5766dcceb641169f89fecb537e8f79e4) | **GET** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@index
[**call_63f5c8e9d4d96d169c64e6e0bd4d8ae1**](DataAccessApplicationReviewApi.md#call_63f5c8e9d4d96d169c64e6e0bd4d8ae1) | **GET** /api/v1/users/{userId}/dar/applications/{id}/reviews | DataAccessApplicationReview@index
[**call_64625be7555cbc341f14b96ee6677188**](DataAccessApplicationReviewApi.md#call_64625be7555cbc341f14b96ee6677188) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@userUpdate
[**call_657e412d92e286b217a1892e7f84395c**](DataAccessApplicationReviewApi.md#call_657e412d92e286b217a1892e7f84395c) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/questions/{questionId}/reviews/{reviewId} | DataAccessApplicationReview@update
[**call_98785fe27d508b80baad6eb609d00f49**](DataAccessApplicationReviewApi.md#call_98785fe27d508b80baad6eb609d00f49) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@userUpdateGlobal
[**dd0ec98127c9183bf7f9d4a24085d8a8**](DataAccessApplicationReviewApi.md#dd0ec98127c9183bf7f9d4a24085d8a8) | **PUT** /api/v1/teams/{team_id}/dar/applications/{id}/reviews/{reviewId} | DataAccessApplicationReview@updateGlobal
[**de86e9675c626354e1d2c5d385712d90**](DataAccessApplicationReviewApi.md#de86e9675c626354e1d2c5d385712d90) | **POST** /api/v1/teams/{team_id}/dar/applications/{id}/reviews | DataAccessApplicationReview@storeGlobal


# **bdc71807f7e3ab85967e343d06f95228**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response bdc71807f7e3ab85967e343d06f95228(team_id, id, question_id, de86e9675c626354e1d2c5d385712d90_request)

DataAccessApplicationReview@store

Create a new review comment on a question in a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.de86e9675c626354e1d2c5d385712d90_request import De86e9675c626354e1d2c5d385712d90Request
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    de86e9675c626354e1d2c5d385712d90_request = gateway_api_sdk.De86e9675c626354e1d2c5d385712d90Request() # De86e9675c626354e1d2c5d385712d90Request | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@store
        api_response = api_instance.bdc71807f7e3ab85967e343d06f95228(team_id, id, question_id, de86e9675c626354e1d2c5d385712d90_request)
        print("The response of DataAccessApplicationReviewApi->bdc71807f7e3ab85967e343d06f95228:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->bdc71807f7e3ab85967e343d06f95228: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **de86e9675c626354e1d2c5d385712d90_request** | [**De86e9675c626354e1d2c5d385712d90Request**](De86e9675c626354e1d2c5d385712d90Request.md)| DataAccessApplicationReview definition | 

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

# **call_05c982367b9c911ca1ec6d6352fa23fe**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_05c982367b9c911ca1ec6d6352fa23fe(team_id, id, review_id, file_id)

DataAccessApplicationReview@destroyFile

Delete a file associated with a DAR review

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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | Dar application id
    review_id = 1 # int | Review id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplicationReview@destroyFile
        api_response = api_instance.call_05c982367b9c911ca1ec6d6352fa23fe(team_id, id, review_id, file_id)
        print("The response of DataAccessApplicationReviewApi->call_05c982367b9c911ca1ec6d6352fa23fe:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_05c982367b9c911ca1ec6d6352fa23fe: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| Dar application id | 
 **review_id** | **int**| Review id | 
 **file_id** | **str**| File uuid | 

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

# **call_154214db8250a7ff2fbbc9b6050ce1ab**
> call_154214db8250a7ff2fbbc9b6050ce1ab(team_id, id, review_id, file_id)

DataAccessApplicationReview@downloadFile

Download a file associated with a DAR application review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplicationReview@downloadFile
        api_instance.call_154214db8250a7ff2fbbc9b6050ce1ab(team_id, id, review_id, file_id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_154214db8250a7ff2fbbc9b6050ce1ab: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **file_id** | **str**| File uuid | 

### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: file, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_1fe1b50e52ecaba3d4a895720df962c7**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_1fe1b50e52ecaba3d4a895720df962c7(team_id, id, review_id)

DataAccessApplicationReview@destroyGlobal

Delete a review from a DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id

    try:
        # DataAccessApplicationReview@destroyGlobal
        api_response = api_instance.call_1fe1b50e52ecaba3d4a895720df962c7(team_id, id, review_id)
        print("The response of DataAccessApplicationReviewApi->call_1fe1b50e52ecaba3d4a895720df962c7:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_1fe1b50e52ecaba3d4a895720df962c7: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 

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

# **call_3f912cdc3d1bff9db206309ee384c782**
> call_3f912cdc3d1bff9db206309ee384c782(user_id, id, review_id, file_id)

DataAccessApplicationReview@downloadUserFile

Download a file associated with a DAR application review

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplicationReview@downloadUserFile
        api_instance.call_3f912cdc3d1bff9db206309ee384c782(user_id, id, review_id, file_id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_3f912cdc3d1bff9db206309ee384c782: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **file_id** | **str**| File uuid | 

### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: file, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_53ba4c05c761d4787bfd1f1841d4b345**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_53ba4c05c761d4787bfd1f1841d4b345(team_id, id, question_id, review_id)

DataAccessApplicationReview@destroy

Delete a review from a DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    review_id = 1 # int | DAR application review id

    try:
        # DataAccessApplicationReview@destroy
        api_response = api_instance.call_53ba4c05c761d4787bfd1f1841d4b345(team_id, id, question_id, review_id)
        print("The response of DataAccessApplicationReviewApi->call_53ba4c05c761d4787bfd1f1841d4b345:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_53ba4c05c761d4787bfd1f1841d4b345: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **review_id** | **int**| DAR application review id | 

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

# **call_5766dcceb641169f89fecb537e8f79e4**
> Model5766dcceb641169f89fecb537e8f79e4200Response call_5766dcceb641169f89fecb537e8f79e4(team_id, id)

DataAccessApplicationReview@index

Return all reviews on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model5766dcceb641169f89fecb537e8f79e4200_response import Model5766dcceb641169f89fecb537e8f79e4200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplicationReview@index
        api_response = api_instance.call_5766dcceb641169f89fecb537e8f79e4(team_id, id)
        print("The response of DataAccessApplicationReviewApi->call_5766dcceb641169f89fecb537e8f79e4:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_5766dcceb641169f89fecb537e8f79e4: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model5766dcceb641169f89fecb537e8f79e4200Response**](Model5766dcceb641169f89fecb537e8f79e4200Response.md)

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

# **call_63f5c8e9d4d96d169c64e6e0bd4d8ae1**
> Model5766dcceb641169f89fecb537e8f79e4200Response call_63f5c8e9d4d96d169c64e6e0bd4d8ae1(user_id, id)

DataAccessApplicationReview@index

Return all reviews on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model5766dcceb641169f89fecb537e8f79e4200_response import Model5766dcceb641169f89fecb537e8f79e4200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplicationReview@index
        api_response = api_instance.call_63f5c8e9d4d96d169c64e6e0bd4d8ae1(user_id, id)
        print("The response of DataAccessApplicationReviewApi->call_63f5c8e9d4d96d169c64e6e0bd4d8ae1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_63f5c8e9d4d96d169c64e6e0bd4d8ae1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model5766dcceb641169f89fecb537e8f79e4200Response**](Model5766dcceb641169f89fecb537e8f79e4200Response.md)

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

# **call_64625be7555cbc341f14b96ee6677188**
> Model657e412d92e286b217a1892e7f84395c200Response call_64625be7555cbc341f14b96ee6677188(user_id, id, question_id, review_id, de86e9675c626354e1d2c5d385712d90_request)

DataAccessApplicationReview@userUpdate

User endpoint to update a review comment on a question in a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.de86e9675c626354e1d2c5d385712d90_request import De86e9675c626354e1d2c5d385712d90Request
from gateway_api_sdk.models.model657e412d92e286b217a1892e7f84395c200_response import Model657e412d92e286b217a1892e7f84395c200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    review_id = 1 # int | DAR application review id
    de86e9675c626354e1d2c5d385712d90_request = gateway_api_sdk.De86e9675c626354e1d2c5d385712d90Request() # De86e9675c626354e1d2c5d385712d90Request | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@userUpdate
        api_response = api_instance.call_64625be7555cbc341f14b96ee6677188(user_id, id, question_id, review_id, de86e9675c626354e1d2c5d385712d90_request)
        print("The response of DataAccessApplicationReviewApi->call_64625be7555cbc341f14b96ee6677188:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_64625be7555cbc341f14b96ee6677188: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **review_id** | **int**| DAR application review id | 
 **de86e9675c626354e1d2c5d385712d90_request** | [**De86e9675c626354e1d2c5d385712d90Request**](De86e9675c626354e1d2c5d385712d90Request.md)| DataAccessApplicationReview definition | 

### Return type

[**Model657e412d92e286b217a1892e7f84395c200Response**](Model657e412d92e286b217a1892e7f84395c200Response.md)

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

# **call_657e412d92e286b217a1892e7f84395c**
> Model657e412d92e286b217a1892e7f84395c200Response call_657e412d92e286b217a1892e7f84395c(team_id, id, question_id, review_id, de86e9675c626354e1d2c5d385712d90_request)

DataAccessApplicationReview@update

Update a review comment on a question in a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.de86e9675c626354e1d2c5d385712d90_request import De86e9675c626354e1d2c5d385712d90Request
from gateway_api_sdk.models.model657e412d92e286b217a1892e7f84395c200_response import Model657e412d92e286b217a1892e7f84395c200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    question_id = 1 # int | DAR application question id
    review_id = 1 # int | DAR application review id
    de86e9675c626354e1d2c5d385712d90_request = gateway_api_sdk.De86e9675c626354e1d2c5d385712d90Request() # De86e9675c626354e1d2c5d385712d90Request | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@update
        api_response = api_instance.call_657e412d92e286b217a1892e7f84395c(team_id, id, question_id, review_id, de86e9675c626354e1d2c5d385712d90_request)
        print("The response of DataAccessApplicationReviewApi->call_657e412d92e286b217a1892e7f84395c:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_657e412d92e286b217a1892e7f84395c: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **question_id** | **int**| DAR application question id | 
 **review_id** | **int**| DAR application review id | 
 **de86e9675c626354e1d2c5d385712d90_request** | [**De86e9675c626354e1d2c5d385712d90Request**](De86e9675c626354e1d2c5d385712d90Request.md)| DataAccessApplicationReview definition | 

### Return type

[**Model657e412d92e286b217a1892e7f84395c200Response**](Model657e412d92e286b217a1892e7f84395c200Response.md)

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

# **call_98785fe27d508b80baad6eb609d00f49**
> Model657e412d92e286b217a1892e7f84395c200Response call_98785fe27d508b80baad6eb609d00f49(user_id, id, review_id, de86e9675c626354e1d2c5d385712d90_request)

DataAccessApplicationReview@userUpdateGlobal

User endpoint to update a review comment on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.de86e9675c626354e1d2c5d385712d90_request import De86e9675c626354e1d2c5d385712d90Request
from gateway_api_sdk.models.model657e412d92e286b217a1892e7f84395c200_response import Model657e412d92e286b217a1892e7f84395c200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    de86e9675c626354e1d2c5d385712d90_request = gateway_api_sdk.De86e9675c626354e1d2c5d385712d90Request() # De86e9675c626354e1d2c5d385712d90Request | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@userUpdateGlobal
        api_response = api_instance.call_98785fe27d508b80baad6eb609d00f49(user_id, id, review_id, de86e9675c626354e1d2c5d385712d90_request)
        print("The response of DataAccessApplicationReviewApi->call_98785fe27d508b80baad6eb609d00f49:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->call_98785fe27d508b80baad6eb609d00f49: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **de86e9675c626354e1d2c5d385712d90_request** | [**De86e9675c626354e1d2c5d385712d90Request**](De86e9675c626354e1d2c5d385712d90Request.md)| DataAccessApplicationReview definition | 

### Return type

[**Model657e412d92e286b217a1892e7f84395c200Response**](Model657e412d92e286b217a1892e7f84395c200Response.md)

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

# **dd0ec98127c9183bf7f9d4a24085d8a8**
> Model657e412d92e286b217a1892e7f84395c200Response dd0ec98127c9183bf7f9d4a24085d8a8(team_id, id, review_id, de86e9675c626354e1d2c5d385712d90_request)

DataAccessApplicationReview@updateGlobal

Update a review comment on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.de86e9675c626354e1d2c5d385712d90_request import De86e9675c626354e1d2c5d385712d90Request
from gateway_api_sdk.models.model657e412d92e286b217a1892e7f84395c200_response import Model657e412d92e286b217a1892e7f84395c200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    review_id = 1 # int | DAR application review id
    de86e9675c626354e1d2c5d385712d90_request = gateway_api_sdk.De86e9675c626354e1d2c5d385712d90Request() # De86e9675c626354e1d2c5d385712d90Request | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@updateGlobal
        api_response = api_instance.dd0ec98127c9183bf7f9d4a24085d8a8(team_id, id, review_id, de86e9675c626354e1d2c5d385712d90_request)
        print("The response of DataAccessApplicationReviewApi->dd0ec98127c9183bf7f9d4a24085d8a8:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->dd0ec98127c9183bf7f9d4a24085d8a8: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **review_id** | **int**| DAR application review id | 
 **de86e9675c626354e1d2c5d385712d90_request** | [**De86e9675c626354e1d2c5d385712d90Request**](De86e9675c626354e1d2c5d385712d90Request.md)| DataAccessApplicationReview definition | 

### Return type

[**Model657e412d92e286b217a1892e7f84395c200Response**](Model657e412d92e286b217a1892e7f84395c200Response.md)

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

# **de86e9675c626354e1d2c5d385712d90**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response de86e9675c626354e1d2c5d385712d90(team_id, id, de86e9675c626354e1d2c5d385712d90_request)

DataAccessApplicationReview@storeGlobal

Create a new review comment on a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.de86e9675c626354e1d2c5d385712d90_request import De86e9675c626354e1d2c5d385712d90Request
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
    api_instance = gateway_api_sdk.DataAccessApplicationReviewApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    de86e9675c626354e1d2c5d385712d90_request = gateway_api_sdk.De86e9675c626354e1d2c5d385712d90Request() # De86e9675c626354e1d2c5d385712d90Request | DataAccessApplicationReview definition

    try:
        # DataAccessApplicationReview@storeGlobal
        api_response = api_instance.de86e9675c626354e1d2c5d385712d90(team_id, id, de86e9675c626354e1d2c5d385712d90_request)
        print("The response of DataAccessApplicationReviewApi->de86e9675c626354e1d2c5d385712d90:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationReviewApi->de86e9675c626354e1d2c5d385712d90: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **de86e9675c626354e1d2c5d385712d90_request** | [**De86e9675c626354e1d2c5d385712d90Request**](De86e9675c626354e1d2c5d385712d90Request.md)| DataAccessApplicationReview definition | 

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

