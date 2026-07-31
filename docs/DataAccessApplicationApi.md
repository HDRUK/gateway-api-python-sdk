# gateway_api_sdk.DataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**a3e2f5885d871929e4b5d81f58ddf867**](DataAccessApplicationApi.md#a3e2f5885d871929e4b5d81f58ddf867) | **GET** /api/v1/users/{userId}/dar/applications/{id}/files | DataAccessApplication@showFiles
[**a6ad90e00b65d8dbf974c30b43586052**](DataAccessApplicationApi.md#a6ad90e00b65d8dbf974c30b43586052) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile
[**bcfd40c79f3f5e7e33e2efd241a9b1a5**](DataAccessApplicationApi.md#bcfd40c79f3f5e7e33e2efd241a9b1a5) | **PUT** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@update
[**call_2692176ac531294e07a905f5735d15ac**](DataAccessApplicationApi.md#call_2692176ac531294e07a905f5735d15ac) | **POST** /api/v1/dar/applications | DataAccessApplication@store
[**call_27b8f8d036cdb3330072da6d0aaf7344**](DataAccessApplicationApi.md#call_27b8f8d036cdb3330072da6d0aaf7344) | **DELETE** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@destroy
[**call_2e4f31039d1a014480ec9444231e5f23**](DataAccessApplicationApi.md#call_2e4f31039d1a014480ec9444231e5f23) | **DELETE** /api/v1/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**call_3da503b7dd0562e285ce75c4c026ce76**](DataAccessApplicationApi.md#call_3da503b7dd0562e285ce75c4c026ce76) | **DELETE** /api/v1/dar/applications/{id} | DataAccessApplication@destroy
[**call_473ee45c3962ae2a02abbac5015dce6a**](DataAccessApplicationApi.md#call_473ee45c3962ae2a02abbac5015dce6a) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/answers | DataAccessApplication@showAnswers
[**call_5cd6e8b93c6db11618e96a968b037db9**](DataAccessApplicationApi.md#call_5cd6e8b93c6db11618e96a968b037db9) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/download | DataAccessApplication@download
[**call_74f3b5729b08a4be0d17e4b1c7fa2aa9**](DataAccessApplicationApi.md#call_74f3b5729b08a4be0d17e4b1c7fa2aa9) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/status | DataAccessApplication@status
[**call_897ef426f5db99512aaed03854777419**](DataAccessApplicationApi.md#call_897ef426f5db99512aaed03854777419) | **DELETE** /api/v1/users/{userId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**call_928c1c4e39f13593bdec88641ee83120**](DataAccessApplicationApi.md#call_928c1c4e39f13593bdec88641ee83120) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files | DataAccessApplication@showFiles
[**f07acaef191991ba38aa72f6d40d988f**](DataAccessApplicationApi.md#f07acaef191991ba38aa72f6d40d988f) | **GET** /api/v1/users/{userId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile
[**f5e83ee26e8a390328a3bf23e750b153**](DataAccessApplicationApi.md#f5e83ee26e8a390328a3bf23e750b153) | **PATCH** /api/v1/users/{userId}/dar/applications/{id} | DataAccessApplication@update
[**fe59a4a568b5a79e886e86951f29518a**](DataAccessApplicationApi.md#fe59a4a568b5a79e886e86951f29518a) | **PATCH** /api/v1/teams/{teamId}/dar/applications/{id} | DataAccessApplication@update
[**ff8efbb0c9dffd80c3eb2ea675a94c99**](DataAccessApplicationApi.md#ff8efbb0c9dffd80c3eb2ea675a94c99) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile


# **a3e2f5885d871929e4b5d81f58ddf867**
> Model928c1c4e39f13593bdec88641ee83120200Response a3e2f5885d871929e4b5d81f58ddf867(id, user_id)

DataAccessApplication@showFiles

Return a list of files associated with a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model928c1c4e39f13593bdec88641ee83120200_response import Model928c1c4e39f13593bdec88641ee83120200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    id = 1 # int | DAR application id
    user_id = 1 # int | User id

    try:
        # DataAccessApplication@showFiles
        api_response = api_instance.a3e2f5885d871929e4b5d81f58ddf867(id, user_id)
        print("The response of DataAccessApplicationApi->a3e2f5885d871929e4b5d81f58ddf867:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->a3e2f5885d871929e4b5d81f58ddf867: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR application id | 
 **user_id** | **int**| User id | 

### Return type

[**Model928c1c4e39f13593bdec88641ee83120200Response**](Model928c1c4e39f13593bdec88641ee83120200Response.md)

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

# **a6ad90e00b65d8dbf974c30b43586052**
> a6ad90e00b65d8dbf974c30b43586052(team_id, id, file_id)

DataAccessApplication@downloadFile

Download a file associated with a DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplication@downloadFile
        api_instance.a6ad90e00b65d8dbf974c30b43586052(team_id, id, file_id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->a6ad90e00b65d8dbf974c30b43586052: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
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

# **bcfd40c79f3f5e7e33e2efd241a9b1a5**
> Model4e4d590ec8943163168e4fc34bd166a1200Response bcfd40c79f3f5e7e33e2efd241a9b1a5(user_id, id, bcfd40c79f3f5e7e33e2efd241a9b1a5_request)

DataAccessApplication@update

Update a system DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.bcfd40c79f3f5e7e33e2efd241a9b1a5_request import Bcfd40c79f3f5e7e33e2efd241a9b1a5Request
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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    bcfd40c79f3f5e7e33e2efd241a9b1a5_request = gateway_api_sdk.Bcfd40c79f3f5e7e33e2efd241a9b1a5Request() # Bcfd40c79f3f5e7e33e2efd241a9b1a5Request | DataAccessApplication definition

    try:
        # DataAccessApplication@update
        api_response = api_instance.bcfd40c79f3f5e7e33e2efd241a9b1a5(user_id, id, bcfd40c79f3f5e7e33e2efd241a9b1a5_request)
        print("The response of DataAccessApplicationApi->bcfd40c79f3f5e7e33e2efd241a9b1a5:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->bcfd40c79f3f5e7e33e2efd241a9b1a5: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **bcfd40c79f3f5e7e33e2efd241a9b1a5_request** | [**Bcfd40c79f3f5e7e33e2efd241a9b1a5Request**](Bcfd40c79f3f5e7e33e2efd241a9b1a5Request.md)| DataAccessApplication definition | 

### Return type

[**Model4e4d590ec8943163168e4fc34bd166a1200Response**](Model4e4d590ec8943163168e4fc34bd166a1200Response.md)

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

# **call_2692176ac531294e07a905f5735d15ac**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_2692176ac531294e07a905f5735d15ac(model2692176ac531294e07a905f5735d15ac_request)

DataAccessApplication@store

Creates a new DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model2692176ac531294e07a905f5735d15ac_request import Model2692176ac531294e07a905f5735d15acRequest
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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    model2692176ac531294e07a905f5735d15ac_request = gateway_api_sdk.Model2692176ac531294e07a905f5735d15acRequest() # Model2692176ac531294e07a905f5735d15acRequest | DataAccessApplication definition

    try:
        # DataAccessApplication@store
        api_response = api_instance.call_2692176ac531294e07a905f5735d15ac(model2692176ac531294e07a905f5735d15ac_request)
        print("The response of DataAccessApplicationApi->call_2692176ac531294e07a905f5735d15ac:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_2692176ac531294e07a905f5735d15ac: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model2692176ac531294e07a905f5735d15ac_request** | [**Model2692176ac531294e07a905f5735d15acRequest**](Model2692176ac531294e07a905f5735d15acRequest.md)| DataAccessApplication definition | 

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

# **call_27b8f8d036cdb3330072da6d0aaf7344**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_27b8f8d036cdb3330072da6d0aaf7344(user_id, id)

DataAccessApplication@destroy

Delete a users DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplication@destroy
        api_response = api_instance.call_27b8f8d036cdb3330072da6d0aaf7344(user_id, id)
        print("The response of DataAccessApplicationApi->call_27b8f8d036cdb3330072da6d0aaf7344:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_27b8f8d036cdb3330072da6d0aaf7344: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

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
**401** | Unauthorized |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_2e4f31039d1a014480ec9444231e5f23**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_2e4f31039d1a014480ec9444231e5f23(id, file_id)

DataAccessApplication@destroyFile

Delete a file associated with a DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    id = 1 # int | DAR application id
    file_id = '1' # str | File id

    try:
        # DataAccessApplication@destroyFile
        api_response = api_instance.call_2e4f31039d1a014480ec9444231e5f23(id, file_id)
        print("The response of DataAccessApplicationApi->call_2e4f31039d1a014480ec9444231e5f23:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_2e4f31039d1a014480ec9444231e5f23: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR application id | 
 **file_id** | **str**| File id | 

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

# **call_3da503b7dd0562e285ce75c4c026ce76**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_3da503b7dd0562e285ce75c4c026ce76(id)

DataAccessApplication@destroy

Delete a system DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    id = 1 # int | DAR application id

    try:
        # DataAccessApplication@destroy
        api_response = api_instance.call_3da503b7dd0562e285ce75c4c026ce76(id)
        print("The response of DataAccessApplicationApi->call_3da503b7dd0562e285ce75c4c026ce76:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_3da503b7dd0562e285ce75c4c026ce76: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR application id | 

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

# **call_473ee45c3962ae2a02abbac5015dce6a**
> Model473ee45c3962ae2a02abbac5015dce6a200Response call_473ee45c3962ae2a02abbac5015dce6a(team_id, id)

DataAccessApplication@showAnswers

Return answers from a single DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplication@showAnswers
        api_response = api_instance.call_473ee45c3962ae2a02abbac5015dce6a(team_id, id)
        print("The response of DataAccessApplicationApi->call_473ee45c3962ae2a02abbac5015dce6a:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_473ee45c3962ae2a02abbac5015dce6a: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
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

# **call_5cd6e8b93c6db11618e96a968b037db9**
> call_5cd6e8b93c6db11618e96a968b037db9(team_id, id)

DataAccessApplication@download

Returns a DAR form as a CSV with attached files as a zip

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplication@download
        api_instance.call_5cd6e8b93c6db11618e96a968b037db9(team_id, id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_5cd6e8b93c6db11618e96a968b037db9: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

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

# **call_74f3b5729b08a4be0d17e4b1c7fa2aa9**
> Model74f3b5729b08a4be0d17e4b1c7fa2aa9200Response call_74f3b5729b08a4be0d17e4b1c7fa2aa9(team_id, id)

DataAccessApplication@status

Return the status history of a single DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model74f3b5729b08a4be0d17e4b1c7fa2aa9200_response import Model74f3b5729b08a4be0d17e4b1c7fa2aa9200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplication@status
        api_response = api_instance.call_74f3b5729b08a4be0d17e4b1c7fa2aa9(team_id, id)
        print("The response of DataAccessApplicationApi->call_74f3b5729b08a4be0d17e4b1c7fa2aa9:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_74f3b5729b08a4be0d17e4b1c7fa2aa9: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model74f3b5729b08a4be0d17e4b1c7fa2aa9200Response**](Model74f3b5729b08a4be0d17e4b1c7fa2aa9200Response.md)

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

# **call_897ef426f5db99512aaed03854777419**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_897ef426f5db99512aaed03854777419(id, user_id, file_id)

DataAccessApplication@destroyFile

Delete a file associated with a DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    id = 1 # int | DAR application id
    user_id = 1 # int | User id
    file_id = '1' # str | File uuid

    try:
        # DataAccessApplication@destroyFile
        api_response = api_instance.call_897ef426f5db99512aaed03854777419(id, user_id, file_id)
        print("The response of DataAccessApplicationApi->call_897ef426f5db99512aaed03854777419:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_897ef426f5db99512aaed03854777419: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR application id | 
 **user_id** | **int**| User id | 
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

# **call_928c1c4e39f13593bdec88641ee83120**
> Model928c1c4e39f13593bdec88641ee83120200Response call_928c1c4e39f13593bdec88641ee83120(team_id, id)

DataAccessApplication@showFiles

Return a list of files associated with a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model928c1c4e39f13593bdec88641ee83120200_response import Model928c1c4e39f13593bdec88641ee83120200Response
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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # DataAccessApplication@showFiles
        api_response = api_instance.call_928c1c4e39f13593bdec88641ee83120(team_id, id)
        print("The response of DataAccessApplicationApi->call_928c1c4e39f13593bdec88641ee83120:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->call_928c1c4e39f13593bdec88641ee83120: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model928c1c4e39f13593bdec88641ee83120200Response**](Model928c1c4e39f13593bdec88641ee83120200Response.md)

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

# **f07acaef191991ba38aa72f6d40d988f**
> f07acaef191991ba38aa72f6d40d988f(id, user_id, file_id)

DataAccessApplication@downloadFile

Download a file associated with a DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    id = 1 # int | DAR application id
    user_id = 1 # int | User id
    file_id = '1' # str | File id

    try:
        # DataAccessApplication@downloadFile
        api_instance.f07acaef191991ba38aa72f6d40d988f(id, user_id, file_id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->f07acaef191991ba38aa72f6d40d988f: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR application id | 
 **user_id** | **int**| User id | 
 **file_id** | **str**| File id | 

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

# **f5e83ee26e8a390328a3bf23e750b153**
> Model4e4d590ec8943163168e4fc34bd166a1200Response f5e83ee26e8a390328a3bf23e750b153(user_id, id, f5e83ee26e8a390328a3bf23e750b153_request)

DataAccessApplication@update

Edit a system DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.f5e83ee26e8a390328a3bf23e750b153_request import F5e83ee26e8a390328a3bf23e750b153Request
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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id
    f5e83ee26e8a390328a3bf23e750b153_request = gateway_api_sdk.F5e83ee26e8a390328a3bf23e750b153Request() # F5e83ee26e8a390328a3bf23e750b153Request | DataAccessApplication definition

    try:
        # DataAccessApplication@update
        api_response = api_instance.f5e83ee26e8a390328a3bf23e750b153(user_id, id, f5e83ee26e8a390328a3bf23e750b153_request)
        print("The response of DataAccessApplicationApi->f5e83ee26e8a390328a3bf23e750b153:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->f5e83ee26e8a390328a3bf23e750b153: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **f5e83ee26e8a390328a3bf23e750b153_request** | [**F5e83ee26e8a390328a3bf23e750b153Request**](F5e83ee26e8a390328a3bf23e750b153Request.md)| DataAccessApplication definition | 

### Return type

[**Model4e4d590ec8943163168e4fc34bd166a1200Response**](Model4e4d590ec8943163168e4fc34bd166a1200Response.md)

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

# **fe59a4a568b5a79e886e86951f29518a**
> Model4e4d590ec8943163168e4fc34bd166a1200Response fe59a4a568b5a79e886e86951f29518a(team_id, id, fe59a4a568b5a79e886e86951f29518a_request)

DataAccessApplication@update

Edit a system DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fe59a4a568b5a79e886e86951f29518a_request import Fe59a4a568b5a79e886e86951f29518aRequest
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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    fe59a4a568b5a79e886e86951f29518a_request = gateway_api_sdk.Fe59a4a568b5a79e886e86951f29518aRequest() # Fe59a4a568b5a79e886e86951f29518aRequest | DataAccessApplication definition

    try:
        # DataAccessApplication@update
        api_response = api_instance.fe59a4a568b5a79e886e86951f29518a(team_id, id, fe59a4a568b5a79e886e86951f29518a_request)
        print("The response of DataAccessApplicationApi->fe59a4a568b5a79e886e86951f29518a:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->fe59a4a568b5a79e886e86951f29518a: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **fe59a4a568b5a79e886e86951f29518a_request** | [**Fe59a4a568b5a79e886e86951f29518aRequest**](Fe59a4a568b5a79e886e86951f29518aRequest.md)| DataAccessApplication definition | 

### Return type

[**Model4e4d590ec8943163168e4fc34bd166a1200Response**](Model4e4d590ec8943163168e4fc34bd166a1200Response.md)

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

# **ff8efbb0c9dffd80c3eb2ea675a94c99**
> C29b5b3424f7317b69b4bda048ccfafb200Response ff8efbb0c9dffd80c3eb2ea675a94c99(team_id, id, file_id)

DataAccessApplication@destroyFile

Delete a file associated with a DAR application

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
    api_instance = gateway_api_sdk.DataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id
    file_id = 1 # int | File id

    try:
        # DataAccessApplication@destroyFile
        api_response = api_instance.ff8efbb0c9dffd80c3eb2ea675a94c99(team_id, id, file_id)
        print("The response of DataAccessApplicationApi->ff8efbb0c9dffd80c3eb2ea675a94c99:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->ff8efbb0c9dffd80c3eb2ea675a94c99: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **file_id** | **int**| File id | 

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

