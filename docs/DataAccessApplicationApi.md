# gateway_api_sdk.DataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_dar_application_files**](DataAccessApplicationApi.md#delete_dar_application_files) | **DELETE** /api/v1/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**delete_dar_applications**](DataAccessApplicationApi.md#delete_dar_applications) | **DELETE** /api/v1/dar/applications/{id} | DataAccessApplication@destroy
[**delete_team_dar_application_file**](DataAccessApplicationApi.md#delete_team_dar_application_file) | **DELETE** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId} | DataAccessApplication@destroyFile
[**fetch_team_dar_application_answers**](DataAccessApplicationApi.md#fetch_team_dar_application_answers) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/answers | DataAccessApplication@showAnswers
[**fetch_team_dar_application_download_zip**](DataAccessApplicationApi.md#fetch_team_dar_application_download_zip) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/download | DataAccessApplication@download
[**fetch_team_dar_application_file**](DataAccessApplicationApi.md#fetch_team_dar_application_file) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files/{fileId}/download | DataAccessApplication@downloadFile
[**fetch_team_dar_application_files**](DataAccessApplicationApi.md#fetch_team_dar_application_files) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/files | DataAccessApplication@showFiles
[**fetch_team_dar_application_status_history**](DataAccessApplicationApi.md#fetch_team_dar_application_status_history) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/status | DataAccessApplication@status
[**update_team_dar_application**](DataAccessApplicationApi.md#update_team_dar_application) | **PATCH** /api/v1/teams/{teamId}/dar/applications/{id} | DataAccessApplication@update


# **delete_dar_application_files**
> DeleteApplications200Response delete_dar_application_files(id, file_id)

DataAccessApplication@destroyFile

Delete a file associated with a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_applications200_response import DeleteApplications200Response
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
        api_response = api_instance.delete_dar_application_files(id, file_id)
        print("The response of DataAccessApplicationApi->delete_dar_application_files:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->delete_dar_application_files: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR application id | 
 **file_id** | **str**| File id | 

### Return type

[**DeleteApplications200Response**](DeleteApplications200Response.md)

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

# **delete_dar_applications**
> DeleteApplications200Response delete_dar_applications(id)

DataAccessApplication@destroy

Delete a system DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_applications200_response import DeleteApplications200Response
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
        api_response = api_instance.delete_dar_applications(id)
        print("The response of DataAccessApplicationApi->delete_dar_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->delete_dar_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR application id | 

### Return type

[**DeleteApplications200Response**](DeleteApplications200Response.md)

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

# **delete_team_dar_application_file**
> DeleteApplications200Response delete_team_dar_application_file(team_id, id, file_id)

DataAccessApplication@destroyFile

Delete a file associated with a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_applications200_response import DeleteApplications200Response
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
        api_response = api_instance.delete_team_dar_application_file(team_id, id, file_id)
        print("The response of DataAccessApplicationApi->delete_team_dar_application_file:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->delete_team_dar_application_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **file_id** | **int**| File id | 

### Return type

[**DeleteApplications200Response**](DeleteApplications200Response.md)

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

# **fetch_team_dar_application_answers**
> FetchTeamDarApplicationAnswers200Response fetch_team_dar_application_answers(team_id, id)

DataAccessApplication@showAnswers

Return answers from a single DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application_answers200_response import FetchTeamDarApplicationAnswers200Response
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
        api_response = api_instance.fetch_team_dar_application_answers(team_id, id)
        print("The response of DataAccessApplicationApi->fetch_team_dar_application_answers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->fetch_team_dar_application_answers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**FetchTeamDarApplicationAnswers200Response**](FetchTeamDarApplicationAnswers200Response.md)

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

# **fetch_team_dar_application_download_zip**
> fetch_team_dar_application_download_zip(team_id, id)

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
        api_instance.fetch_team_dar_application_download_zip(team_id, id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->fetch_team_dar_application_download_zip: %s\n" % e)
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

# **fetch_team_dar_application_file**
> fetch_team_dar_application_file(team_id, id, file_id)

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
        api_instance.fetch_team_dar_application_file(team_id, id, file_id)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->fetch_team_dar_application_file: %s\n" % e)
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

# **fetch_team_dar_application_files**
> FetchTeamDarApplicationFiles200Response fetch_team_dar_application_files(team_id, id)

DataAccessApplication@showFiles

Return a list of files associated with a DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application_files200_response import FetchTeamDarApplicationFiles200Response
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
        api_response = api_instance.fetch_team_dar_application_files(team_id, id)
        print("The response of DataAccessApplicationApi->fetch_team_dar_application_files:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->fetch_team_dar_application_files: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**FetchTeamDarApplicationFiles200Response**](FetchTeamDarApplicationFiles200Response.md)

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

# **fetch_team_dar_application_status_history**
> FetchTeamDarApplicationStatusHistory200Response fetch_team_dar_application_status_history(team_id, id)

DataAccessApplication@status

Return the status history of a single DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application_status_history200_response import FetchTeamDarApplicationStatusHistory200Response
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
        api_response = api_instance.fetch_team_dar_application_status_history(team_id, id)
        print("The response of DataAccessApplicationApi->fetch_team_dar_application_status_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->fetch_team_dar_application_status_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**FetchTeamDarApplicationStatusHistory200Response**](FetchTeamDarApplicationStatusHistory200Response.md)

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

# **update_team_dar_application**
> FetchTeamDarApplication200Response update_team_dar_application(team_id, id, update_team_dar_application_request)

DataAccessApplication@update

Edit a system DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application200_response import FetchTeamDarApplication200Response
from gateway_api_sdk.models.update_team_dar_application_request import UpdateTeamDarApplicationRequest
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
    update_team_dar_application_request = gateway_api_sdk.UpdateTeamDarApplicationRequest() # UpdateTeamDarApplicationRequest | DataAccessApplication definition

    try:
        # DataAccessApplication@update
        api_response = api_instance.update_team_dar_application(team_id, id, update_team_dar_application_request)
        print("The response of DataAccessApplicationApi->update_team_dar_application:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessApplicationApi->update_team_dar_application: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 
 **update_team_dar_application_request** | [**UpdateTeamDarApplicationRequest**](UpdateTeamDarApplicationRequest.md)| DataAccessApplication definition | 

### Return type

[**FetchTeamDarApplication200Response**](FetchTeamDarApplication200Response.md)

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

