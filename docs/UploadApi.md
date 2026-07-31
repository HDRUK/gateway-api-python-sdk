# gateway_api_sdk.UploadApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_files**](UploadApi.md#create_files) | **POST** /api/v1/files | Upload@upload
[**delete_files_processed**](UploadApi.md#delete_files_processed) | **DELETE** /api/v1/files/processed/{id} | Upload@destroy
[**fetch_files**](UploadApi.md#fetch_files) | **GET** /api/v1/files/{uuid} | Upload@show
[**fetch_files_processed_content**](UploadApi.md#fetch_files_processed_content) | **GET** /api/v1/files/processed/{uuid}/download | Upload@content


# **create_files**
> CreateFiles200Response create_files(entity_flag=entity_flag, team_id=team_id, application_id=application_id, question_id=question_id)

Upload@upload

Upload a file to the gateway-api via scanning sub-service

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_files200_response import CreateFiles200Response
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
        api_response = api_instance.create_files(entity_flag=entity_flag, team_id=team_id, application_id=application_id, question_id=question_id)
        print("The response of UploadApi->create_files:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->create_files: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **entity_flag** | **str**| Flag to indicate the purpose of the file upload e.g. dur-from-upload | [optional] 
 **team_id** | **int**| Id of team associated with the file upload | [optional] 
 **application_id** | **int**| Id of dar application associated with the file upload | [optional] 
 **question_id** | **int**| Id of the question in the dar application associated with the file upload | [optional] 

### Return type

[**CreateFiles200Response**](CreateFiles200Response.md)

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

# **delete_files_processed**
> DeleteAliases200Response delete_files_processed(id)

Upload@destroy

Delete a processed file

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_aliases200_response import DeleteAliases200Response
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
        api_response = api_instance.delete_files_processed(id)
        print("The response of UploadApi->delete_files_processed:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->delete_files_processed: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| file uuid | 

### Return type

[**DeleteAliases200Response**](DeleteAliases200Response.md)

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

# **fetch_files**
> FetchFiles200Response fetch_files(uuid)

Upload@show

Get the scanning status of an upload

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_files200_response import FetchFiles200Response
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
        api_response = api_instance.fetch_files(uuid)
        print("The response of UploadApi->fetch_files:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->fetch_files: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **str**| upload id | 

### Return type

[**FetchFiles200Response**](FetchFiles200Response.md)

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

# **fetch_files_processed_content**
> FetchFilesProcessedContent200Response fetch_files_processed_content(uuid)

Upload@content

Get the content of a processed file

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_files_processed_content200_response import FetchFilesProcessedContent200Response
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
        api_response = api_instance.fetch_files_processed_content(uuid)
        print("The response of UploadApi->fetch_files_processed_content:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UploadApi->fetch_files_processed_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **str**| upload id | 

### Return type

[**FetchFilesProcessedContent200Response**](FetchFilesProcessedContent200Response.md)

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

