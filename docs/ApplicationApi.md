# gateway_api_sdk.ApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**c724575805bbca0f084a3001d71abd53**](ApplicationApi.md#c724575805bbca0f084a3001d71abd53) | **PATCH** /api/v1/applications/{id}/clientid | ApplicationController@generateClientIdById
[**call_3c8adeb001330f5198ca1072be78e299**](ApplicationApi.md#call_3c8adeb001330f5198ca1072be78e299) | **PUT** /api/v1/applications/{id} | ApplicationController@update
[**call_45ae3b415211ef0712a8ea070e66449f**](ApplicationApi.md#call_45ae3b415211ef0712a8ea070e66449f) | **PATCH** /api/v1/applications/{id} | ApplicationController@edit
[**ddca747ae792e5b6837b97c6ad510fd3**](ApplicationApi.md#ddca747ae792e5b6837b97c6ad510fd3) | **DELETE** /api/v1/applications/{id} | ApplicationController@delete
[**e210052adcf6fdcfc472998b430081aa**](ApplicationApi.md#e210052adcf6fdcfc472998b430081aa) | **POST** /api/v1/applications | ApplicationController@store
[**fetch_all_applications**](ApplicationApi.md#fetch_all_applications) | **GET** /api/v1/applications | ApplicationController@index
[**fetch_all_sitemap**](ApplicationApi.md#fetch_all_sitemap) | **GET** /api/v1/sitemap | SiteMapController@index
[**fetch_applications**](ApplicationApi.md#fetch_applications) | **GET** /api/v1/applications/{id} | ApplicationController@show


# **c724575805bbca0f084a3001d71abd53**
> Model3c8adeb001330f5198ca1072be78e299200Response c724575805bbca0f084a3001d71abd53(id)

ApplicationController@generateClientIdById

Generate Client ID application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model3c8adeb001330f5198ca1072be78e299200_response import Model3c8adeb001330f5198ca1072be78e299200Response
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
        api_response = api_instance.c724575805bbca0f084a3001d71abd53(id)
        print("The response of ApplicationApi->c724575805bbca0f084a3001d71abd53:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->c724575805bbca0f084a3001d71abd53: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 

### Return type

[**Model3c8adeb001330f5198ca1072be78e299200Response**](Model3c8adeb001330f5198ca1072be78e299200Response.md)

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

# **call_3c8adeb001330f5198ca1072be78e299**
> Model3c8adeb001330f5198ca1072be78e299200Response call_3c8adeb001330f5198ca1072be78e299(id, model3c8adeb001330f5198ca1072be78e299_request)

ApplicationController@update

Update application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model3c8adeb001330f5198ca1072be78e299200_response import Model3c8adeb001330f5198ca1072be78e299200Response
from gateway_api_sdk.models.model3c8adeb001330f5198ca1072be78e299_request import Model3c8adeb001330f5198ca1072be78e299Request
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
    model3c8adeb001330f5198ca1072be78e299_request = gateway_api_sdk.Model3c8adeb001330f5198ca1072be78e299Request() # Model3c8adeb001330f5198ca1072be78e299Request | ActivityLog definition

    try:
        # ApplicationController@update
        api_response = api_instance.call_3c8adeb001330f5198ca1072be78e299(id, model3c8adeb001330f5198ca1072be78e299_request)
        print("The response of ApplicationApi->call_3c8adeb001330f5198ca1072be78e299:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->call_3c8adeb001330f5198ca1072be78e299: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 
 **model3c8adeb001330f5198ca1072be78e299_request** | [**Model3c8adeb001330f5198ca1072be78e299Request**](Model3c8adeb001330f5198ca1072be78e299Request.md)| ActivityLog definition | 

### Return type

[**Model3c8adeb001330f5198ca1072be78e299200Response**](Model3c8adeb001330f5198ca1072be78e299200Response.md)

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

# **call_45ae3b415211ef0712a8ea070e66449f**
> Model3c8adeb001330f5198ca1072be78e299200Response call_45ae3b415211ef0712a8ea070e66449f(id, model45ae3b415211ef0712a8ea070e66449f_request)

ApplicationController@edit

Edit application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model3c8adeb001330f5198ca1072be78e299200_response import Model3c8adeb001330f5198ca1072be78e299200Response
from gateway_api_sdk.models.model45ae3b415211ef0712a8ea070e66449f_request import Model45ae3b415211ef0712a8ea070e66449fRequest
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
    model45ae3b415211ef0712a8ea070e66449f_request = gateway_api_sdk.Model45ae3b415211ef0712a8ea070e66449fRequest() # Model45ae3b415211ef0712a8ea070e66449fRequest | ActivityLog definition

    try:
        # ApplicationController@edit
        api_response = api_instance.call_45ae3b415211ef0712a8ea070e66449f(id, model45ae3b415211ef0712a8ea070e66449f_request)
        print("The response of ApplicationApi->call_45ae3b415211ef0712a8ea070e66449f:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->call_45ae3b415211ef0712a8ea070e66449f: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 
 **model45ae3b415211ef0712a8ea070e66449f_request** | [**Model45ae3b415211ef0712a8ea070e66449fRequest**](Model45ae3b415211ef0712a8ea070e66449fRequest.md)| ActivityLog definition | 

### Return type

[**Model3c8adeb001330f5198ca1072be78e299200Response**](Model3c8adeb001330f5198ca1072be78e299200Response.md)

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

# **ddca747ae792e5b6837b97c6ad510fd3**
> C29b5b3424f7317b69b4bda048ccfafb200Response ddca747ae792e5b6837b97c6ad510fd3(id)

ApplicationController@delete

Delete application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.c29b5b3424f7317b69b4bda048ccfafb200_response import C29b5b3424f7317b69b4bda048ccfafb200Response
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
        api_response = api_instance.ddca747ae792e5b6837b97c6ad510fd3(id)
        print("The response of ApplicationApi->ddca747ae792e5b6837b97c6ad510fd3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->ddca747ae792e5b6837b97c6ad510fd3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| application id | 

### Return type

[**C29b5b3424f7317b69b4bda048ccfafb200Response**](C29b5b3424f7317b69b4bda048ccfafb200Response.md)

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

# **e210052adcf6fdcfc472998b430081aa**
> E210052adcf6fdcfc472998b430081aa200Response e210052adcf6fdcfc472998b430081aa(e210052adcf6fdcfc472998b430081aa_request)

ApplicationController@store

Creates application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.e210052adcf6fdcfc472998b430081aa200_response import E210052adcf6fdcfc472998b430081aa200Response
from gateway_api_sdk.models.e210052adcf6fdcfc472998b430081aa_request import E210052adcf6fdcfc472998b430081aaRequest
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
    e210052adcf6fdcfc472998b430081aa_request = gateway_api_sdk.E210052adcf6fdcfc472998b430081aaRequest() # E210052adcf6fdcfc472998b430081aaRequest | Application definition

    try:
        # ApplicationController@store
        api_response = api_instance.e210052adcf6fdcfc472998b430081aa(e210052adcf6fdcfc472998b430081aa_request)
        print("The response of ApplicationApi->e210052adcf6fdcfc472998b430081aa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ApplicationApi->e210052adcf6fdcfc472998b430081aa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **e210052adcf6fdcfc472998b430081aa_request** | [**E210052adcf6fdcfc472998b430081aaRequest**](E210052adcf6fdcfc472998b430081aaRequest.md)| Application definition | 

### Return type

[**E210052adcf6fdcfc472998b430081aa200Response**](E210052adcf6fdcfc472998b430081aa200Response.md)

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

