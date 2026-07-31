# gateway_api_sdk.LicenseApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_licenses**](LicenseApi.md#create_licenses) | **POST** /api/v1/licenses | License@store
[**delete_licenses**](LicenseApi.md#delete_licenses) | **DELETE** /api/v1/licenses/{id} | License@destroy
[**edit_licenses**](LicenseApi.md#edit_licenses) | **PATCH** /api/v1/licenses/{id} | License@edit
[**fetch_all_licenses**](LicenseApi.md#fetch_all_licenses) | **GET** /api/v1/licenses | License@index
[**fetch_licenses**](LicenseApi.md#fetch_licenses) | **GET** /api/v1/licenses/{id} | License@show
[**update_licenses**](LicenseApi.md#update_licenses) | **PUT** /api/v1/licenses/{id} | License@update


# **create_licenses**
> CreateCategories200Response create_licenses(create_licenses_request)

License@store

Creates a new license

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_licenses_request import CreateLicensesRequest
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
    api_instance = gateway_api_sdk.LicenseApi(api_client)
    create_licenses_request = gateway_api_sdk.CreateLicensesRequest() # CreateLicensesRequest | License definition

    try:
        # License@store
        api_response = api_instance.create_licenses(create_licenses_request)
        print("The response of LicenseApi->create_licenses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->create_licenses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_licenses_request** | [**CreateLicensesRequest**](CreateLicensesRequest.md)| License definition | 

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

# **delete_licenses**
> DeleteAliases200Response delete_licenses(id)

License@destroy

Delete a License

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
    api_instance = gateway_api_sdk.LicenseApi(api_client)
    id = 1 # int | License id

    try:
        # License@destroy
        api_response = api_instance.delete_licenses(id)
        print("The response of LicenseApi->delete_licenses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->delete_licenses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| License id | 

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

# **edit_licenses**
> UpdateLicenses200Response edit_licenses(id, create_licenses_request)

License@edit

Edit a tool license

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_licenses_request import CreateLicensesRequest
from gateway_api_sdk.models.update_licenses200_response import UpdateLicenses200Response
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
    api_instance = gateway_api_sdk.LicenseApi(api_client)
    id = 1 # int | license id
    create_licenses_request = gateway_api_sdk.CreateLicensesRequest() # CreateLicensesRequest | Category definition

    try:
        # License@edit
        api_response = api_instance.edit_licenses(id, create_licenses_request)
        print("The response of LicenseApi->edit_licenses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->edit_licenses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| license id | 
 **create_licenses_request** | [**CreateLicensesRequest**](CreateLicensesRequest.md)| Category definition | 

### Return type

[**UpdateLicenses200Response**](UpdateLicenses200Response.md)

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

# **fetch_all_licenses**
> FetchAllLicenses200Response fetch_all_licenses()

License@index

Returns a list of licenses available

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_all_licenses200_response import FetchAllLicenses200Response
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
    api_instance = gateway_api_sdk.LicenseApi(api_client)

    try:
        # License@index
        api_response = api_instance.fetch_all_licenses()
        print("The response of LicenseApi->fetch_all_licenses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->fetch_all_licenses: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchAllLicenses200Response**](FetchAllLicenses200Response.md)

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

# **fetch_licenses**
> FetchLicenses200Response fetch_licenses(id)

License@show

Return a single license

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_licenses200_response import FetchLicenses200Response
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
    api_instance = gateway_api_sdk.LicenseApi(api_client)
    id = 1 # int | License ID

    try:
        # License@show
        api_response = api_instance.fetch_licenses(id)
        print("The response of LicenseApi->fetch_licenses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->fetch_licenses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| License ID | 

### Return type

[**FetchLicenses200Response**](FetchLicenses200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_licenses**
> UpdateLicenses200Response update_licenses(id, create_licenses_request)

License@update

Update a tool license

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_licenses_request import CreateLicensesRequest
from gateway_api_sdk.models.update_licenses200_response import UpdateLicenses200Response
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
    api_instance = gateway_api_sdk.LicenseApi(api_client)
    id = 1 # int | license id
    create_licenses_request = gateway_api_sdk.CreateLicensesRequest() # CreateLicensesRequest | Category definition

    try:
        # License@update
        api_response = api_instance.update_licenses(id, create_licenses_request)
        print("The response of LicenseApi->update_licenses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->update_licenses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| license id | 
 **create_licenses_request** | [**CreateLicensesRequest**](CreateLicensesRequest.md)| Category definition | 

### Return type

[**UpdateLicenses200Response**](UpdateLicenses200Response.md)

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

