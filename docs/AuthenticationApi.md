# gateway_api_sdk.AuthenticationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authentication**](AuthenticationApi.md#authentication) | **POST** /api/v1/auth | AuthController@checkAuthorization
[**login**](AuthenticationApi.md#login) | **POST** /api/v1/auth/login | AuthController@login
[**register**](AuthenticationApi.md#register) | **POST** /api/v1/auth/register | AuthController@register


# **authentication**
> Authentication200Response authentication(authentication_request)

AuthController@checkAuthorization

Generate Jwt based on email and password

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.authentication200_response import Authentication200Response
from gateway_api_sdk.models.authentication_request import AuthenticationRequest
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
    api_instance = gateway_api_sdk.AuthenticationApi(api_client)
    authentication_request = gateway_api_sdk.AuthenticationRequest() # AuthenticationRequest | Pass user credentials

    try:
        # AuthController@checkAuthorization
        api_response = api_instance.authentication(authentication_request)
        print("The response of AuthenticationApi->authentication:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthenticationApi->authentication: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authentication_request** | [**AuthenticationRequest**](AuthenticationRequest.md)| Pass user credentials | 

### Return type

[**Authentication200Response**](Authentication200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**401** | Missing Property |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **login**
> Register200Response login(login_request)

AuthController@login

Login with email and password

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.login_request import LoginRequest
from gateway_api_sdk.models.register200_response import Register200Response
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
    api_instance = gateway_api_sdk.AuthenticationApi(api_client)
    login_request = gateway_api_sdk.LoginRequest() # LoginRequest | Pass user credentials

    try:
        # AuthController@login
        api_response = api_instance.login(login_request)
        print("The response of AuthenticationApi->login:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthenticationApi->login: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **login_request** | [**LoginRequest**](LoginRequest.md)| Pass user credentials | 

### Return type

[**Register200Response**](Register200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Validation error |  -  |
**401** | Invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **register**
> Register200Response register(register_request)

AuthController@register

Register a new user with email and password

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.register200_response import Register200Response
from gateway_api_sdk.models.register_request import RegisterRequest
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
    api_instance = gateway_api_sdk.AuthenticationApi(api_client)
    register_request = gateway_api_sdk.RegisterRequest() # RegisterRequest | Pass user registration data

    try:
        # AuthController@register
        api_response = api_instance.register(register_request)
        print("The response of AuthenticationApi->register:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthenticationApi->register: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **register_request** | [**RegisterRequest**](RegisterRequest.md)| Pass user registration data | 

### Return type

[**Register200Response**](Register200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Validation error |  -  |
**409** | Email already exists |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

