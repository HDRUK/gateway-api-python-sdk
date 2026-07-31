# gateway_api_sdk.DataAccessSectionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dar_section**](DataAccessSectionApi.md#create_dar_section) | **POST** /api/v1/dar/sections | DataAccessSection@store
[**delete_dar_section**](DataAccessSectionApi.md#delete_dar_section) | **DELETE** /api/v1/dar/sections/{id} | DataAccessSection@destroy
[**fetch_dar_section**](DataAccessSectionApi.md#fetch_dar_section) | **GET** /api/v1/dar/sections/{id} | DataAccessSection@show
[**fetch_dar_sections**](DataAccessSectionApi.md#fetch_dar_sections) | **GET** /api/v1/dar/sections | DataAccessSection@index
[**patch_dar_section**](DataAccessSectionApi.md#patch_dar_section) | **PATCH** /api/v1/dar/sections/{id} | DataAccessSection@update
[**update_dar_section**](DataAccessSectionApi.md#update_dar_section) | **PUT** /api/v1/dar/sections/{id} | DataAccessSection@update


# **create_dar_section**
> CreateCategories200Response create_dar_section(create_dar_section_request)

DataAccessSection@store

Creates a new DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_dar_section_request import CreateDarSectionRequest
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    create_dar_section_request = gateway_api_sdk.CreateDarSectionRequest() # CreateDarSectionRequest | DataAccessSection definition

    try:
        # DataAccessSection@store
        api_response = api_instance.create_dar_section(create_dar_section_request)
        print("The response of DataAccessSectionApi->create_dar_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->create_dar_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_dar_section_request** | [**CreateDarSectionRequest**](CreateDarSectionRequest.md)| DataAccessSection definition | 

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

# **delete_dar_section**
> DeleteAliases200Response delete_dar_section(id)

DataAccessSection@destroy

Delete a system DAR section

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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id

    try:
        # DataAccessSection@destroy
        api_response = api_instance.delete_dar_section(id)
        print("The response of DataAccessSectionApi->delete_dar_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->delete_dar_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 

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

# **fetch_dar_section**
> FetchDarSection200Response fetch_dar_section(id)

DataAccessSection@show

Return a single DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dar_section200_response import FetchDarSection200Response
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id

    try:
        # DataAccessSection@show
        api_response = api_instance.fetch_dar_section(id)
        print("The response of DataAccessSectionApi->fetch_dar_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->fetch_dar_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 

### Return type

[**FetchDarSection200Response**](FetchDarSection200Response.md)

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

# **fetch_dar_sections**
> FetchDarSections200Response fetch_dar_sections(per_page=per_page)

DataAccessSection@index

List of DAR sections

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dar_sections200_response import FetchDarSections200Response
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # DataAccessSection@index
        api_response = api_instance.fetch_dar_sections(per_page=per_page)
        print("The response of DataAccessSectionApi->fetch_dar_sections:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->fetch_dar_sections: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

[**FetchDarSections200Response**](FetchDarSections200Response.md)

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

# **patch_dar_section**
> FetchDarSection200Response patch_dar_section(id, patch_dar_section_request)

DataAccessSection@update

Edit a system DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dar_section200_response import FetchDarSection200Response
from gateway_api_sdk.models.patch_dar_section_request import PatchDarSectionRequest
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id
    patch_dar_section_request = gateway_api_sdk.PatchDarSectionRequest() # PatchDarSectionRequest | DataAccessSection definition

    try:
        # DataAccessSection@update
        api_response = api_instance.patch_dar_section(id, patch_dar_section_request)
        print("The response of DataAccessSectionApi->patch_dar_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->patch_dar_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 
 **patch_dar_section_request** | [**PatchDarSectionRequest**](PatchDarSectionRequest.md)| DataAccessSection definition | 

### Return type

[**FetchDarSection200Response**](FetchDarSection200Response.md)

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

# **update_dar_section**
> FetchDarSection200Response update_dar_section(id, create_dar_section_request)

DataAccessSection@update

Update a system DAR section

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_section_request import CreateDarSectionRequest
from gateway_api_sdk.models.fetch_dar_section200_response import FetchDarSection200Response
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
    api_instance = gateway_api_sdk.DataAccessSectionApi(api_client)
    id = 1 # int | DAR section id
    create_dar_section_request = gateway_api_sdk.CreateDarSectionRequest() # CreateDarSectionRequest | DataAccessSection definition

    try:
        # DataAccessSection@update
        api_response = api_instance.update_dar_section(id, create_dar_section_request)
        print("The response of DataAccessSectionApi->update_dar_section:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessSectionApi->update_dar_section: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR section id | 
 **create_dar_section_request** | [**CreateDarSectionRequest**](CreateDarSectionRequest.md)| DataAccessSection definition | 

### Return type

[**FetchDarSection200Response**](FetchDarSection200Response.md)

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

