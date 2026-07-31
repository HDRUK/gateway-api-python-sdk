# gateway_api_sdk.UserRolesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_user_has_roles**](UserRolesApi.md#create_user_has_roles) | **POST** /api/v1/users/{userId}/roles | UserRoleController@store
[**delete_user_has_roles**](UserRolesApi.md#delete_user_has_roles) | **DELETE** /api/v1/users/{userId}/roles | UserRoleController@destroy
[**update_user_has_roles**](UserRolesApi.md#update_user_has_roles) | **PATCH** /api/v1/users/{userId}/roles | UserRoleController@edit


# **create_user_has_roles**
> C29b5b3424f7317b69b4bda048ccfafb200Response create_user_has_roles(user_id, create_user_has_roles_request)

UserRoleController@store

Create user has roles

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
from gateway_api_sdk.models.create_user_has_roles_request import CreateUserHasRolesRequest
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
    api_instance = gateway_api_sdk.UserRolesApi(api_client)
    user_id = 1 # int | user id
    create_user_has_roles_request = gateway_api_sdk.CreateUserHasRolesRequest() # CreateUserHasRolesRequest | Pass user credentials

    try:
        # UserRoleController@store
        api_response = api_instance.create_user_has_roles(user_id, create_user_has_roles_request)
        print("The response of UserRolesApi->create_user_has_roles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserRolesApi->create_user_has_roles: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 
 **create_user_has_roles_request** | [**CreateUserHasRolesRequest**](CreateUserHasRolesRequest.md)| Pass user credentials | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

# **delete_user_has_roles**
> DeleteFederation200Response delete_user_has_roles(user_id)

UserRoleController@destroy

Delete user - roles

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
    api_instance = gateway_api_sdk.UserRolesApi(api_client)
    user_id = 1 # int | user id

    try:
        # UserRoleController@destroy
        api_response = api_instance.delete_user_has_roles(user_id)
        print("The response of UserRolesApi->delete_user_has_roles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserRolesApi->delete_user_has_roles: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 

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

# **update_user_has_roles**
> C29b5b3424f7317b69b4bda048ccfafb200Response update_user_has_roles(user_id, update_user_has_roles_request)

UserRoleController@edit

Update user has roles

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
from gateway_api_sdk.models.update_user_has_roles_request import UpdateUserHasRolesRequest
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
    api_instance = gateway_api_sdk.UserRolesApi(api_client)
    user_id = 1 # int | user id
    update_user_has_roles_request = gateway_api_sdk.UpdateUserHasRolesRequest() # UpdateUserHasRolesRequest | Pass user credentials

    try:
        # UserRoleController@edit
        api_response = api_instance.update_user_has_roles(user_id, update_user_has_roles_request)
        print("The response of UserRolesApi->update_user_has_roles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserRolesApi->update_user_has_roles: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| user id | 
 **update_user_has_roles_request** | [**UpdateUserHasRolesRequest**](UpdateUserHasRolesRequest.md)| Pass user credentials | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

