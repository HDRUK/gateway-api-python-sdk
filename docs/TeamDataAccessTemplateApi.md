# gateway_api_sdk.TeamDataAccessTemplateApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_team_dar_template_file**](TeamDataAccessTemplateApi.md#delete_team_dar_template_file) | **DELETE** /api/v1/teams/{teamId}/dar/templates/{id}/files/{fileId} | TeamDataAccessTemplateController@destroyFile
[**fetch_team_dar_templates**](TeamDataAccessTemplateApi.md#fetch_team_dar_templates) | **GET** /api/v1/teams/{teamId}/dar/templates | TeamDataAccessTemplateController@index
[**team_dar_template_count_unique_fields**](TeamDataAccessTemplateApi.md#team_dar_template_count_unique_fields) | **GET** /api/v1/teams/{teamId}/dar/templates/count/{field} | TeamDataAccessTemplateController@count


# **delete_team_dar_template_file**
> DeleteApplications200Response delete_team_dar_template_file(team_id, id, file_id)

TeamDataAccessTemplateController@destroyFile

Delete a file associated with a DAR template

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
    api_instance = gateway_api_sdk.TeamDataAccessTemplateApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR template id
    file_id = '1' # str | File id

    try:
        # TeamDataAccessTemplateController@destroyFile
        api_response = api_instance.delete_team_dar_template_file(team_id, id, file_id)
        print("The response of TeamDataAccessTemplateApi->delete_team_dar_template_file:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessTemplateApi->delete_team_dar_template_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR template id | 
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
**401** | Unauthorized |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_team_dar_templates**
> FetchDarTemplates200Response fetch_team_dar_templates(team_id, published=published)

TeamDataAccessTemplateController@index

List of dar templates belonging to a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dar_templates200_response import FetchDarTemplates200Response
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
    api_instance = gateway_api_sdk.TeamDataAccessTemplateApi(api_client)
    team_id = 1 # int | Team id
    published = 'true' # str | Template publication status to filter by (true, false) (optional)

    try:
        # TeamDataAccessTemplateController@index
        api_response = api_instance.fetch_team_dar_templates(team_id, published=published)
        print("The response of TeamDataAccessTemplateApi->fetch_team_dar_templates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessTemplateApi->fetch_team_dar_templates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **published** | **str**| Template publication status to filter by (true, false) | [optional] 

### Return type

[**FetchDarTemplates200Response**](FetchDarTemplates200Response.md)

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

# **team_dar_template_count_unique_fields**
> CountUniqueFieldsCollections200Response team_dar_template_count_unique_fields(team_id, var_field)

TeamDataAccessTemplateController@count

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
    api_instance = gateway_api_sdk.TeamDataAccessTemplateApi(api_client)
    team_id = 1 # int | Team id
    var_field = 'published' # str | name of the field to perform a count on

    try:
        # TeamDataAccessTemplateController@count
        api_response = api_instance.team_dar_template_count_unique_fields(team_id, var_field)
        print("The response of TeamDataAccessTemplateApi->team_dar_template_count_unique_fields:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessTemplateApi->team_dar_template_count_unique_fields: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
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

