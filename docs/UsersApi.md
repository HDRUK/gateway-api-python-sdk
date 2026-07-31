# gateway_api_sdk.UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_users**](UsersApi.md#create_users) | **POST** /api/v1/users | UserController@store
[**delete_users**](UsersApi.md#delete_users) | **DELETE** /api/v1/users/{id} | UserController@destroy
[**edit_users**](UsersApi.md#edit_users) | **PATCH** /api/v1/users/{id} | UserController@edit
[**fetch_all_users**](UsersApi.md#fetch_all_users) | **GET** /api/v1/users | UserController@index
[**fetch_users**](UsersApi.md#fetch_users) | **GET** /api/v1/users/{id} | UserController@show
[**resend_secondary_verification_email**](UsersApi.md#resend_secondary_verification_email) | **POST** /api/v1/users/{id}/resend-secondary-verification | Resend secondary email verification
[**update_users**](UsersApi.md#update_users) | **PUT** /api/v1/users/{id} | UserController@update
[**verify_secondary_email**](UsersApi.md#verify_secondary_email) | **GET** /api/v1/users/verify-secondary-email/{uuid} | Verify user&#39;s secondary email using a UUID


# **create_users**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response create_users(create_users_request)

UserController@store

Create a new user

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_users_request import CreateUsersRequest
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    create_users_request = gateway_api_sdk.CreateUsersRequest() # CreateUsersRequest | Pass user credentials

    try:
        # UserController@store
        api_response = api_instance.create_users(create_users_request)
        print("The response of UsersApi->create_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->create_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_users_request** | [**CreateUsersRequest**](CreateUsersRequest.md)| Pass user credentials | 

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
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_users**
> DeleteFederation200Response delete_users(id)

UserController@destroy

Delete User based in id

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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    id = 1 # int | user id

    try:
        # UserController@destroy
        api_response = api_instance.delete_users(id)
        print("The response of UsersApi->delete_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->delete_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| user id | 

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
**401** | Unauthorized |  -  |
**404** | Error response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_users**
> FetchUsers200Response edit_users(id, update_users_request)

UserController@edit

Edit user

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_users200_response import FetchUsers200Response
from gateway_api_sdk.models.update_users_request import UpdateUsersRequest
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    id = 1 # int | user id
    update_users_request = gateway_api_sdk.UpdateUsersRequest() # UpdateUsersRequest | Pass user credentials

    try:
        # UserController@edit
        api_response = api_instance.edit_users(id, update_users_request)
        print("The response of UsersApi->edit_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->edit_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| user id | 
 **update_users_request** | [**UpdateUsersRequest**](UpdateUsersRequest.md)| Pass user credentials | 

### Return type

[**FetchUsers200Response**](FetchUsers200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**404** | Error response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_all_users**
> FetchAllUsers200Response fetch_all_users(filter_names=filter_names)

UserController@index

Get All Users

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_users200_response import FetchAllUsers200Response
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    filter_names = 'abc' # str | Three or more characters to filter users names by (optional)

    try:
        # UserController@index
        api_response = api_instance.fetch_all_users(filter_names=filter_names)
        print("The response of UsersApi->fetch_all_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->fetch_all_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_names** | **str**| Three or more characters to filter users names by | [optional] 

### Return type

[**FetchAllUsers200Response**](FetchAllUsers200Response.md)

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

# **fetch_users**
> FetchUsers200Response fetch_users(id)

UserController@show

Get users by id

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_users200_response import FetchUsers200Response
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    id = 1 # int | user id

    try:
        # UserController@show
        api_response = api_instance.fetch_users(id)
        print("The response of UsersApi->fetch_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->fetch_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| user id | 

### Return type

[**FetchUsers200Response**](FetchUsers200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**401** | Unauthorized |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resend_secondary_verification_email**
> ResendSecondaryVerificationEmail200Response resend_secondary_verification_email(id)

Resend secondary email verification

Resends the verification email for the secondary email address. Old tokens are expired.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.resend_secondary_verification_email200_response import ResendSecondaryVerificationEmail200Response
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    id = 123 # int | User ID

    try:
        # Resend secondary email verification
        api_response = api_instance.resend_secondary_verification_email(id)
        print("The response of UsersApi->resend_secondary_verification_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->resend_secondary_verification_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 

### Return type

[**ResendSecondaryVerificationEmail200Response**](ResendSecondaryVerificationEmail200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Verification email resent |  -  |
**404** | User or secondary email not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_users**
> FetchUsers200Response update_users(id, update_users_request)

UserController@update

Update user

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_users200_response import FetchUsers200Response
from gateway_api_sdk.models.update_users_request import UpdateUsersRequest
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    id = 1 # int | user id
    update_users_request = gateway_api_sdk.UpdateUsersRequest() # UpdateUsersRequest | Pass user credentials

    try:
        # UserController@update
        api_response = api_instance.update_users(id, update_users_request)
        print("The response of UsersApi->update_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->update_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| user id | 
 **update_users_request** | [**UpdateUsersRequest**](UpdateUsersRequest.md)| Pass user credentials | 

### Return type

[**FetchUsers200Response**](FetchUsers200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Error |  -  |
**401** | Unauthorized |  -  |
**404** | Error response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **verify_secondary_email**
> VerifySecondaryEmail200Response verify_secondary_email(uuid)

Verify user's secondary email using a UUID

This endpoint verifies the secondary email for a user if the UUID is valid and not expired.

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.verify_secondary_email200_response import VerifySecondaryEmail200Response
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
    api_instance = gateway_api_sdk.UsersApi(api_client)
    uuid = '03af1f5e-5cd2-4c41-ae23-56dd2c9efc67' # str | Verification UUID

    try:
        # Verify user's secondary email using a UUID
        api_response = api_instance.verify_secondary_email(uuid)
        print("The response of UsersApi->verify_secondary_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->verify_secondary_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uuid** | **str**| Verification UUID | 

### Return type

[**VerifySecondaryEmail200Response**](VerifySecondaryEmail200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Email verified successfully |  -  |
**400** | Invalid or expired token |  -  |
**404** | UUID not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

