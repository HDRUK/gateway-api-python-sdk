# gateway_api_sdk.ProjectGrantApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_all_project_grants**](ProjectGrantApi.md#fetch_all_project_grants) | **GET** /api/v1/project_grants | ProjectGrantController@index
[**fetch_project_grant**](ProjectGrantApi.md#fetch_project_grant) | **GET** /api/v1/project_grants/{id} | ProjectGrantController@show


# **fetch_all_project_grants**
> FetchAllProjectGrants200Response fetch_all_project_grants(pid=pid, version=version, project_grant_name=project_grant_name, user_id=user_id, team_id=team_id, with_related=with_related)

ProjectGrantController@index

Get all project grants

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_project_grants200_response import FetchAllProjectGrants200Response
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
    api_instance = gateway_api_sdk.ProjectGrantApi(api_client)
    pid = 'pid_example' # str | Filter by dataset pid (optional)
    version = 56 # int | Filter by dataset version number (optional)
    project_grant_name = 'project_grant_name_example' # str | Filter by project grant name (optional)
    user_id = 56 # int | Filter by owning user id (optional)
    team_id = 56 # int | Filter by owning team id (optional)
    with_related = true # bool |  (optional)

    try:
        # ProjectGrantController@index
        api_response = api_instance.fetch_all_project_grants(pid=pid, version=version, project_grant_name=project_grant_name, user_id=user_id, team_id=team_id, with_related=with_related)
        print("The response of ProjectGrantApi->fetch_all_project_grants:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectGrantApi->fetch_all_project_grants: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pid** | **str**| Filter by dataset pid | [optional] 
 **version** | **int**| Filter by dataset version number | [optional] 
 **project_grant_name** | **str**| Filter by project grant name | [optional] 
 **user_id** | **int**| Filter by owning user id | [optional] 
 **team_id** | **int**| Filter by owning team id | [optional] 
 **with_related** | **bool**|  | [optional] 

### Return type

[**FetchAllProjectGrants200Response**](FetchAllProjectGrants200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_project_grant**
> CountUniqueFieldsCollections200Response fetch_project_grant(id, with_related=with_related)

ProjectGrantController@show

Get a single project grant

### Example


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


# Enter a context with an instance of the API client
with gateway_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = gateway_api_sdk.ProjectGrantApi(api_client)
    id = 56 # int | 
    with_related = true # bool |  (optional)

    try:
        # ProjectGrantController@show
        api_response = api_instance.fetch_project_grant(id, with_related=with_related)
        print("The response of ProjectGrantApi->fetch_project_grant:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectGrantApi->fetch_project_grant: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 
 **with_related** | **bool**|  | [optional] 

### Return type

[**CountUniqueFieldsCollections200Response**](CountUniqueFieldsCollections200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

