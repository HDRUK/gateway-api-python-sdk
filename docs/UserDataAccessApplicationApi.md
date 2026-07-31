# gateway_api_sdk.UserDataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**count_all_user_dar_applications**](UserDataAccessApplicationApi.md#count_all_user_dar_applications) | **GET** /api/v1/users/{userId}/dar/applications/count | UserDataAccessApplicationController@allCounts
[**count_user_dar_applications_by_field**](UserDataAccessApplicationApi.md#count_user_dar_applications_by_field) | **GET** /api/v1/users/{userId}/dar/applications/count/{field} | UserDataAccessApplicationController@count
[**create_user_dar_application_answers**](UserDataAccessApplicationApi.md#create_user_dar_application_answers) | **PUT** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplication@storeAnswers
[**fetch_user_dar_application_answers**](UserDataAccessApplicationApi.md#fetch_user_dar_application_answers) | **GET** /api/v1/users/{userId}/dar/applications/{id}/answers | UserDataAccessApplicationController@showAnswers
[**fetch_user_dar_application_details**](UserDataAccessApplicationApi.md#fetch_user_dar_application_details) | **GET** /api/v1/users/{userId}/dar/applications/{id} | UserDataAccessApplicationController@show
[**fetch_user_dar_application_header**](UserDataAccessApplicationApi.md#fetch_user_dar_application_header) | **GET** /api/v1/users/{userId}/dar/applications/{id}/showHeader | UserDataAccessApplicationController@showHeader
[**fetch_user_dar_applications**](UserDataAccessApplicationApi.md#fetch_user_dar_applications) | **GET** /api/v1/users/{userId}/dar/applications | UserDataAccessApplicationController@index


# **count_all_user_dar_applications**
> CountUniqueFieldsCollections200Response count_all_user_dar_applications(user_id)

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
        api_response = api_instance.count_all_user_dar_applications(user_id)
        print("The response of UserDataAccessApplicationApi->count_all_user_dar_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->count_all_user_dar_applications: %s\n" % e)
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

# **count_user_dar_applications_by_field**
> CountUniqueFieldsCollections200Response count_user_dar_applications_by_field(user_id, var_field)

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
        api_response = api_instance.count_user_dar_applications_by_field(user_id, var_field)
        print("The response of UserDataAccessApplicationApi->count_user_dar_applications_by_field:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->count_user_dar_applications_by_field: %s\n" % e)
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

# **create_user_dar_application_answers**
> CreateCategories200Response create_user_dar_application_answers(user_id, id, create_user_dar_application_answers_request)

UserDataAccessApplication@storeAnswers

Add answers to the user's DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_user_dar_application_answers_request import CreateUserDarApplicationAnswersRequest
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
    create_user_dar_application_answers_request = gateway_api_sdk.CreateUserDarApplicationAnswersRequest() # CreateUserDarApplicationAnswersRequest | UserDataAccessApplication definition

    try:
        # UserDataAccessApplication@storeAnswers
        api_response = api_instance.create_user_dar_application_answers(user_id, id, create_user_dar_application_answers_request)
        print("The response of UserDataAccessApplicationApi->create_user_dar_application_answers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->create_user_dar_application_answers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 
 **create_user_dar_application_answers_request** | [**CreateUserDarApplicationAnswersRequest**](CreateUserDarApplicationAnswersRequest.md)| UserDataAccessApplication definition | 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_user_dar_application_answers**
> FetchTeamDarApplicationAnswers200Response fetch_user_dar_application_answers(user_id, id)

UserDataAccessApplicationController@showAnswers

Return answers from the user's DAR application

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
    api_instance = gateway_api_sdk.UserDataAccessApplicationApi(api_client)
    user_id = 1 # int | User id
    id = 1 # int | DAR application id

    try:
        # UserDataAccessApplicationController@showAnswers
        api_response = api_instance.fetch_user_dar_application_answers(user_id, id)
        print("The response of UserDataAccessApplicationApi->fetch_user_dar_application_answers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->fetch_user_dar_application_answers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
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

# **fetch_user_dar_application_details**
> FetchTeamDarApplication200Response fetch_user_dar_application_details(user_id, id)

UserDataAccessApplicationController@show

Return a DAR application belonging to the user

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application200_response import FetchTeamDarApplication200Response
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
        api_response = api_instance.fetch_user_dar_application_details(user_id, id)
        print("The response of UserDataAccessApplicationApi->fetch_user_dar_application_details:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->fetch_user_dar_application_details: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

### Return type

[**FetchTeamDarApplication200Response**](FetchTeamDarApplication200Response.md)

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

# **fetch_user_dar_application_header**
> FetchTeamDarApplication200Response fetch_user_dar_application_header(user_id, id)

UserDataAccessApplicationController@showHeader

Get header information about a specific DAR

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_application200_response import FetchTeamDarApplication200Response
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
        api_response = api_instance.fetch_user_dar_application_header(user_id, id)
        print("The response of UserDataAccessApplicationApi->fetch_user_dar_application_header:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->fetch_user_dar_application_header: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 
 **id** | **int**| DAR application id | 

### Return type

[**FetchTeamDarApplication200Response**](FetchTeamDarApplication200Response.md)

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

# **fetch_user_dar_applications**
> FetchTeamDarApplications200Response fetch_user_dar_applications(user_id)

UserDataAccessApplicationController@index

List of dar applications belonging to a user

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_team_dar_applications200_response import FetchTeamDarApplications200Response
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
        api_response = api_instance.fetch_user_dar_applications(user_id)
        print("The response of UserDataAccessApplicationApi->fetch_user_dar_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserDataAccessApplicationApi->fetch_user_dar_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User id | 

### Return type

[**FetchTeamDarApplications200Response**](FetchTeamDarApplications200Response.md)

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

