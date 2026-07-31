# gateway_api_sdk.NotificationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_notifications**](NotificationApi.md#create_notifications) | **POST** /api/v1/notifications | Notification@store
[**delete_notifications**](NotificationApi.md#delete_notifications) | **DELETE** /api/v1/notifications/{id} | Notification@destroy
[**edit_notifications**](NotificationApi.md#edit_notifications) | **PATCH** /api/v1/notifications/{id} | Notification@edit
[**fetch_all_notifications**](NotificationApi.md#fetch_all_notifications) | **GET** /api/v1/notifications | Notification@index
[**fetch_notifications**](NotificationApi.md#fetch_notifications) | **GET** /api/v1/notifications/{id} | Notification@show
[**update_notifications**](NotificationApi.md#update_notifications) | **PUT** /api/v1/notifications/{id} | Notification@update


# **create_notifications**
> CreateCategories200Response create_notifications(create_notifications_request)

Notification@store

Creates a new notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_notifications_request import CreateNotificationsRequest
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    create_notifications_request = gateway_api_sdk.CreateNotificationsRequest() # CreateNotificationsRequest | Notification definition

    try:
        # Notification@store
        api_response = api_instance.create_notifications(create_notifications_request)
        print("The response of NotificationApi->create_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->create_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_notifications_request** | [**CreateNotificationsRequest**](CreateNotificationsRequest.md)| Notification definition | 

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

# **delete_notifications**
> DeleteAliases200Response delete_notifications(id)

Notification@destroy

Delete a notification

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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id

    try:
        # Notification@destroy
        api_response = api_instance.delete_notifications(id)
        print("The response of NotificationApi->delete_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->delete_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 

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

# **edit_notifications**
> UpdateNotifications200Response edit_notifications(id, edit_notifications_request)

Notification@edit

Edit a notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.edit_notifications_request import EditNotificationsRequest
from gateway_api_sdk.models.update_notifications200_response import UpdateNotifications200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id
    edit_notifications_request = gateway_api_sdk.EditNotificationsRequest() # EditNotificationsRequest | Notification definition

    try:
        # Notification@edit
        api_response = api_instance.edit_notifications(id, edit_notifications_request)
        print("The response of NotificationApi->edit_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->edit_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 
 **edit_notifications_request** | [**EditNotificationsRequest**](EditNotificationsRequest.md)| Notification definition | 

### Return type

[**UpdateNotifications200Response**](UpdateNotifications200Response.md)

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

# **fetch_all_notifications**
> FetchAllNotifications200Response fetch_all_notifications()

Notification@index

Returns a list of notifications enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_notifications200_response import FetchAllNotifications200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)

    try:
        # Notification@index
        api_response = api_instance.fetch_all_notifications()
        print("The response of NotificationApi->fetch_all_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->fetch_all_notifications: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllNotifications200Response**](FetchAllNotifications200Response.md)

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

# **fetch_notifications**
> FetchNotifications200Response fetch_notifications(id)

Notification@show

Return a single notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_notifications200_response import FetchNotifications200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id

    try:
        # Notification@show
        api_response = api_instance.fetch_notifications(id)
        print("The response of NotificationApi->fetch_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->fetch_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 

### Return type

[**FetchNotifications200Response**](FetchNotifications200Response.md)

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

# **update_notifications**
> UpdateNotifications200Response update_notifications(id, create_notifications_request)

Notification@update

Update a notification

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_notifications_request import CreateNotificationsRequest
from gateway_api_sdk.models.update_notifications200_response import UpdateNotifications200Response
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
    api_instance = gateway_api_sdk.NotificationApi(api_client)
    id = 1 # int | notification id
    create_notifications_request = gateway_api_sdk.CreateNotificationsRequest() # CreateNotificationsRequest | Notification definition

    try:
        # Notification@update
        api_response = api_instance.update_notifications(id, create_notifications_request)
        print("The response of NotificationApi->update_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationApi->update_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| notification id | 
 **create_notifications_request** | [**CreateNotificationsRequest**](CreateNotificationsRequest.md)| Notification definition | 

### Return type

[**UpdateNotifications200Response**](UpdateNotifications200Response.md)

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

