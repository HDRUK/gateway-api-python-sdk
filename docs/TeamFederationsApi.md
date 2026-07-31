# gateway_api_sdk.TeamFederationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_federation_team**](TeamFederationsApi.md#create_federation_team) | **POST** /api/v1/teams/{teamId}/federations | FederationController@store
[**delete_federation**](TeamFederationsApi.md#delete_federation) | **DELETE** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@destroy
[**edit_federation_team**](TeamFederationsApi.md#edit_federation_team) | **PATCH** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@edit
[**get_federation_by_federation_id_and_team_id**](TeamFederationsApi.md#get_federation_by_federation_id_and_team_id) | **GET** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@show
[**get_federation_history**](TeamFederationsApi.md#get_federation_history) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/history | FederationController@history
[**get_federation_team_id**](TeamFederationsApi.md#get_federation_team_id) | **GET** /api/v1/teams/{teamId}/federations | FederationController@index
[**run_federation**](TeamFederationsApi.md#run_federation) | **GET** /api/v1/teams/{teamId}/federations/{federationId}/run | FederationController@runNow
[**test_federation**](TeamFederationsApi.md#test_federation) | **POST** /api/v1/teams/{teamId}/federations/test | FederationController@testFederation
[**update_federation_team**](TeamFederationsApi.md#update_federation_team) | **PUT** /api/v1/teams/{teamId}/federations/{federationId} | FederationController@update


# **create_federation_team**
> CreateCategories200Response create_federation_team(team_id, create_federation_team_request)

FederationController@store

Create federation

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_federation_team_request import CreateFederationTeamRequest
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id
    create_federation_team_request = gateway_api_sdk.CreateFederationTeamRequest() # CreateFederationTeamRequest | Pass user credentials

    try:
        # FederationController@store
        api_response = api_instance.create_federation_team(team_id, create_federation_team_request)
        print("The response of TeamFederationsApi->create_federation_team:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->create_federation_team: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **create_federation_team_request** | [**CreateFederationTeamRequest**](CreateFederationTeamRequest.md)| Pass user credentials | 

### Return type

[**CreateCategories200Response**](CreateCategories200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_federation**
> DeleteFederation200Response delete_federation(team_id, federation_id)

FederationController@destroy

Delete federation for team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.delete_federation200_response import DeleteFederation200Response
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id
    federation_id = 1 # int | federation id

    try:
        # FederationController@destroy
        api_response = api_instance.delete_federation(team_id, federation_id)
        print("The response of TeamFederationsApi->delete_federation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->delete_federation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **federation_id** | **int**| federation id | 

### Return type

[**DeleteFederation200Response**](DeleteFederation200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**404** | Error response |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_federation_team**
> CreateCategories200Response edit_federation_team(team_id, federation_id, create_federation_team_request)

FederationController@edit

Edit federation for team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_federation_team_request import CreateFederationTeamRequest
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id
    federation_id = 1 # int | federation id
    create_federation_team_request = gateway_api_sdk.CreateFederationTeamRequest() # CreateFederationTeamRequest | Pass user credentials

    try:
        # FederationController@edit
        api_response = api_instance.edit_federation_team(team_id, federation_id, create_federation_team_request)
        print("The response of TeamFederationsApi->edit_federation_team:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->edit_federation_team: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **federation_id** | **int**| federation id | 
 **create_federation_team_request** | [**CreateFederationTeamRequest**](CreateFederationTeamRequest.md)| Pass user credentials | 

### Return type

[**CreateCategories200Response**](CreateCategories200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_federation_by_federation_id_and_team_id**
> GetFederationByFederationIdAndTeamId200Response get_federation_by_federation_id_and_team_id(team_id, federation_id)

FederationController@show

Get federation by federation id from team id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.get_federation_by_federation_id_and_team_id200_response import GetFederationByFederationIdAndTeamId200Response
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id
    federation_id = 1 # int | federation id

    try:
        # FederationController@show
        api_response = api_instance.get_federation_by_federation_id_and_team_id(team_id, federation_id)
        print("The response of TeamFederationsApi->get_federation_by_federation_id_and_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->get_federation_by_federation_id_and_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **federation_id** | **int**| federation id | 

### Return type

[**GetFederationByFederationIdAndTeamId200Response**](GetFederationByFederationIdAndTeamId200Response.md)

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

# **get_federation_history**
> GetFederationHistory200Response get_federation_history(team_id, federation_id, per_page=per_page)

FederationController@history

Get run history for a federation

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.get_federation_history200_response import GetFederationHistory200Response
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id
    federation_id = 1 # int | federation id
    per_page = 25 # int | per page (optional)

    try:
        # FederationController@history
        api_response = api_instance.get_federation_history(team_id, federation_id, per_page=per_page)
        print("The response of TeamFederationsApi->get_federation_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->get_federation_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **federation_id** | **int**| federation id | 
 **per_page** | **int**| per page | [optional] 

### Return type

[**GetFederationHistory200Response**](GetFederationHistory200Response.md)

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

# **get_federation_team_id**
> GetFederationTeamId200Response get_federation_team_id(team_id)

FederationController@index

Get federations by team id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.get_federation_team_id200_response import GetFederationTeamId200Response
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id

    try:
        # FederationController@index
        api_response = api_instance.get_federation_team_id(team_id)
        print("The response of TeamFederationsApi->get_federation_team_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->get_federation_team_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 

### Return type

[**GetFederationTeamId200Response**](GetFederationTeamId200Response.md)

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

# **run_federation**
> TestFederation200Response run_federation(team_id, federation_id)

FederationController@runNow

Run federation immediately

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.test_federation200_response import TestFederation200Response
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id
    federation_id = 1 # int | federation id

    try:
        # FederationController@runNow
        api_response = api_instance.run_federation(team_id, federation_id)
        print("The response of TeamFederationsApi->run_federation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->run_federation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **federation_id** | **int**| federation id | 

### Return type

[**TestFederation200Response**](TestFederation200Response.md)

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

# **test_federation**
> TestFederation200Response test_federation(team_id)

FederationController@testFederation

Test federation configuration

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.test_federation200_response import TestFederation200Response
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id

    try:
        # FederationController@testFederation
        api_response = api_instance.test_federation(team_id)
        print("The response of TeamFederationsApi->test_federation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->test_federation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 

### Return type

[**TestFederation200Response**](TestFederation200Response.md)

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

# **update_federation_team**
> CreateCategories200Response update_federation_team(team_id, federation_id, update_federation_team_request)

FederationController@update

Update federation for team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.update_federation_team_request import UpdateFederationTeamRequest
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
    api_instance = gateway_api_sdk.TeamFederationsApi(api_client)
    team_id = 1 # int | team id
    federation_id = 1 # int | federation id
    update_federation_team_request = gateway_api_sdk.UpdateFederationTeamRequest() # UpdateFederationTeamRequest | Pass user credentials

    try:
        # FederationController@update
        api_response = api_instance.update_federation_team(team_id, federation_id, update_federation_team_request)
        print("The response of TeamFederationsApi->update_federation_team:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamFederationsApi->update_federation_team: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| team id | 
 **federation_id** | **int**| federation id | 
 **update_federation_team_request** | [**UpdateFederationTeamRequest**](UpdateFederationTeamRequest.md)| Pass user credentials | 

### Return type

[**CreateCategories200Response**](CreateCategories200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

