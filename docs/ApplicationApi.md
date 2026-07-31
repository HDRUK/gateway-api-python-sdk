# gateway_api_sdk.ApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_applications**](ApplicationApi.md#create_applications) | **POST** /api/v1/applications | ApplicationController@store
[**delete_applications**](ApplicationApi.md#delete_applications) | **DELETE** /api/v1/applications/{id} | ApplicationController@delete
[**edit_applications**](ApplicationApi.md#edit_applications) | **PATCH** /api/v1/applications/{id} | ApplicationController@edit
[**fetch_all_applications**](ApplicationApi.md#fetch_all_applications) | **GET** /api/v1/applications | ApplicationController@index
[**fetch_all_sitemap**](ApplicationApi.md#fetch_all_sitemap) | **GET** /api/v1/sitemap | SiteMapController@index
[**fetch_applications**](ApplicationApi.md#fetch_applications) | **GET** /api/v1/applications/{id} | ApplicationController@show
[**patch_applications_client_id**](ApplicationApi.md#patch_applications_client_id) | **PATCH** /api/v1/applications/{id}/clientid | ApplicationController@generateClientIdById
[**update_applications**](ApplicationApi.md#update_applications) | **PUT** /api/v1/applications/{id} | ApplicationController@update


# **create_applications**
> CreateApplications200Response create_applications(create_applications_request)

ApplicationController@store

Creates application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_applications200_response import CreateApplications200Response
from gateway_api_sdk.models.create_applications_request import CreateApplicationsRequest
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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)
    create_applications_request = gateway_api_sdk.CreateApplicationsRequest() # CreateApplicationsRequest | Application definition

    try:
        # ApplicationController@store
        api_response = api_instance.create_applications(create_applications_request)
        print("The response of ApplicationApi->create_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->create_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_applications_request** | [**CreateApplicationsRequest**](CreateApplicationsRequest.md)| Application definition | 

### Return type

[**CreateApplications200Response**](CreateApplications200Response.md)

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

# **delete_applications**
> DeleteAliases200Response delete_applications(id)

ApplicationController@delete

Delete application

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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)
    id = 1 # int | application id

    try:
        # ApplicationController@delete
        api_response = api_instance.delete_applications(id)
        print("The response of ApplicationApi->delete_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->delete_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 

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

# **edit_applications**
> UpdateApplications200Response edit_applications(id, edit_applications_request)

ApplicationController@edit

Edit application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_applications_request import EditApplicationsRequest
from gateway_api_sdk.models.update_applications200_response import UpdateApplications200Response
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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)
    id = 1 # int | application id
    edit_applications_request = gateway_api_sdk.EditApplicationsRequest() # EditApplicationsRequest | ActivityLog definition

    try:
        # ApplicationController@edit
        api_response = api_instance.edit_applications(id, edit_applications_request)
        print("The response of ApplicationApi->edit_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->edit_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 
 **edit_applications_request** | [**EditApplicationsRequest**](EditApplicationsRequest.md)| ActivityLog definition | 

### Return type

[**UpdateApplications200Response**](UpdateApplications200Response.md)

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

# **fetch_all_applications**
> FetchAllApplications200Response fetch_all_applications(team_id=team_id, text=text, status=status)

ApplicationController@index

Returns a list of applications

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_applications200_response import FetchAllApplications200Response
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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)
    team_id = 56 # int | Filter Apps by the teamId (optional)
    text = 'text_example' # str | Search term to filter by application name or description. (optional)
    status = 'status_example' # str | Filter by application status is enabled or not (true or false). (optional)

    try:
        # ApplicationController@index
        api_response = api_instance.fetch_all_applications(team_id=team_id, text=text, status=status)
        print("The response of ApplicationApi->fetch_all_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->fetch_all_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Filter Apps by the teamId | [optional] 
 **text** | **str**| Search term to filter by application name or description. | [optional] 
 **status** | **str**| Filter by application status is enabled or not (true or false). | [optional] 

### Return type

[**FetchAllApplications200Response**](FetchAllApplications200Response.md)

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

# **fetch_all_sitemap**
> FetchAllSitemap200Response fetch_all_sitemap()

SiteMapController@index

Returns a list of all ids and last updated date for Collections, Data Custodians, Data Custodian Networks, Durs, DataSets, Tools

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_sitemap200_response import FetchAllSitemap200Response
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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)

    try:
        # SiteMapController@index
        api_response = api_instance.fetch_all_sitemap()
        print("The response of ApplicationApi->fetch_all_sitemap:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->fetch_all_sitemap: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllSitemap200Response**](FetchAllSitemap200Response.md)

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

# **fetch_applications**
> FetchApplications200Response fetch_applications(id)

ApplicationController@show

Get application by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_applications200_response import FetchApplications200Response
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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)
    id = 1 # int | application id

    try:
        # ApplicationController@show
        api_response = api_instance.fetch_applications(id)
        print("The response of ApplicationApi->fetch_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->fetch_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 

### Return type

[**FetchApplications200Response**](FetchApplications200Response.md)

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

# **patch_applications_client_id**
> UpdateApplications200Response patch_applications_client_id(id)

ApplicationController@generateClientIdById

Generate Client ID application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_applications200_response import UpdateApplications200Response
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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)
    id = 1 # int | application id

    try:
        # ApplicationController@generateClientIdById
        api_response = api_instance.patch_applications_client_id(id)
        print("The response of ApplicationApi->patch_applications_client_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->patch_applications_client_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 

### Return type

[**UpdateApplications200Response**](UpdateApplications200Response.md)

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

# **update_applications**
> UpdateApplications200Response update_applications(id, update_applications_request)

ApplicationController@update

Update application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.update_applications200_response import UpdateApplications200Response
from gateway_api_sdk.models.update_applications_request import UpdateApplicationsRequest
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
    api_instance = gateway_api_sdk.ApplicationApi(api_client)
    id = 1 # int | application id
    update_applications_request = gateway_api_sdk.UpdateApplicationsRequest() # UpdateApplicationsRequest | ActivityLog definition

    try:
        # ApplicationController@update
        api_response = api_instance.update_applications(id, update_applications_request)
        print("The response of ApplicationApi->update_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->update_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 
 **update_applications_request** | [**UpdateApplicationsRequest**](UpdateApplicationsRequest.md)| ActivityLog definition | 

### Return type

[**UpdateApplications200Response**](UpdateApplications200Response.md)

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

