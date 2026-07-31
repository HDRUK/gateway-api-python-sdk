# gateway_api_sdk.UploadApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ba8ab1a2710efebacb7909736d7d2d52**](UploadApi.md#ba8ab1a2710efebacb7909736d7d2d52) | **DELETE** /api/v1/files/processed/{id} | Upload@destroy
[**call_21a780f609f0b91c198ab5de91dc27c6**](UploadApi.md#call_21a780f609f0b91c198ab5de91dc27c6) | **GET** /api/v1/files/processed/{uuid}/download | Upload@content
[**e72aa4b4f0a80caa9fe872bdff983455**](UploadApi.md#e72aa4b4f0a80caa9fe872bdff983455) | **GET** /api/v1/files/{uuid} | Upload@show
[**fceeda218a8998a137b9d7692e7947b6**](UploadApi.md#fceeda218a8998a137b9d7692e7947b6) | **POST** /api/v1/files | Upload@upload


# **ba8ab1a2710efebacb7909736d7d2d52**
> C29b5b3424f7317b69b4bda048ccfafb200Response ba8ab1a2710efebacb7909736d7d2d52(id)

Upload@destroy

Delete a processed file

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
    api_instance = gateway_api_sdk.UploadApi(api_client)
    id = '1' # str | file uuid

    try:
        # Upload@destroy
        api_response = api_instance.ba8ab1a2710efebacb7909736d7d2d52(id)
        print("The response of UploadApi->ba8ab1a2710efebacb7909736d7d2d52:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->ba8ab1a2710efebacb7909736d7d2d52: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| file uuid | 

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

# **call_21a780f609f0b91c198ab5de91dc27c6**
> Model21a780f609f0b91c198ab5de91dc27c6200Response call_21a780f609f0b91c198ab5de91dc27c6(uuid)

Upload@content

Get the content of a processed file

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.model21a780f609f0b91c198ab5de91dc27c6200_response import Model21a780f609f0b91c198ab5de91dc27c6200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.UploadApi(api_client)
    uuid = '1' # str | upload id

    try:
        # Upload@content
        api_response = api_instance.call_21a780f609f0b91c198ab5de91dc27c6(uuid)
        print("The response of UploadApi->call_21a780f609f0b91c198ab5de91dc27c6:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->call_21a780f609f0b91c198ab5de91dc27c6: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **str**| upload id | 

### Return type

[**Model21a780f609f0b91c198ab5de91dc27c6200Response**](Model21a780f609f0b91c198ab5de91dc27c6200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **e72aa4b4f0a80caa9fe872bdff983455**
> E72aa4b4f0a80caa9fe872bdff983455200Response e72aa4b4f0a80caa9fe872bdff983455(uuid)

Upload@show

Get the scanning status of an upload

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.e72aa4b4f0a80caa9fe872bdff983455200_response import E72aa4b4f0a80caa9fe872bdff983455200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.UploadApi(api_client)
    uuid = '1' # str | upload id

    try:
        # Upload@show
        api_response = api_instance.e72aa4b4f0a80caa9fe872bdff983455(uuid)
        print("The response of UploadApi->e72aa4b4f0a80caa9fe872bdff983455:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->e72aa4b4f0a80caa9fe872bdff983455: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **str**| upload id | 

### Return type

[**E72aa4b4f0a80caa9fe872bdff983455200Response**](E72aa4b4f0a80caa9fe872bdff983455200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fceeda218a8998a137b9d7692e7947b6**
> Fceeda218a8998a137b9d7692e7947b6200Response fceeda218a8998a137b9d7692e7947b6(entity_flag=entity_flag, team_id=team_id, application_id=application_id, question_id=question_id)

Upload@upload

Upload a file to the gateway-api via scanning sub-service

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fceeda218a8998a137b9d7692e7947b6200_response import Fceeda218a8998a137b9d7692e7947b6200Response
from gateway_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = gateway_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.UploadApi(api_client)
    entity_flag = 'dur-from-upload' # str | Flag to indicate the purpose of the file upload e.g. dur-from-upload (optional)
    team_id = 10 # int | Id of team associated with the file upload (optional)
    application_id = 10 # int | Id of dar application associated with the file upload (optional)
    question_id = 10 # int | Id of the question in the dar application associated with the file upload (optional)

    try:
        # Upload@upload
        api_response = api_instance.fceeda218a8998a137b9d7692e7947b6(entity_flag=entity_flag, team_id=team_id, application_id=application_id, question_id=question_id)
        print("The response of UploadApi->fceeda218a8998a137b9d7692e7947b6:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->fceeda218a8998a137b9d7692e7947b6: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **entity_flag** | **str**| Flag to indicate the purpose of the file upload e.g. dur-from-upload | [optional] 
 **team_id** | **int**| Id of team associated with the file upload | [optional] 
 **application_id** | **int**| Id of dar application associated with the file upload | [optional] 
 **question_id** | **int**| Id of the question in the dar application associated with the file upload | [optional] 

### Return type

[**Fceeda218a8998a137b9d7692e7947b6200Response**](Fceeda218a8998a137b9d7692e7947b6200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Upload complete |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

