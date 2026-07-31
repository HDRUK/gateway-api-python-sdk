# gateway_api_sdk.DataAccessTemplateApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_dar_template**](DataAccessTemplateApi.md#create_dar_template) | **POST** /api/v1/dar/templates | DataAccessTemplate@store
[**delete_dar_template**](DataAccessTemplateApi.md#delete_dar_template) | **DELETE** /api/v1/dar/templates/{id} | DataAccessTemplate@destroy
[**download_dar_template_file**](DataAccessTemplateApi.md#download_dar_template_file) | **GET** /api/v1/dar/templates/{id}/download | DataAccessTemplate@downloadFile
[**fetch_dar_template**](DataAccessTemplateApi.md#fetch_dar_template) | **GET** /api/v1/dar/templates/{id} | DataAccessTemplate@show
[**fetch_dar_templates**](DataAccessTemplateApi.md#fetch_dar_templates) | **GET** /api/v1/dar/templates | DataAccessTemplate@index
[**patch_dar_template**](DataAccessTemplateApi.md#patch_dar_template) | **PATCH** /api/v1/dar/templates/{id} | DataAccessTemplate@update
[**update_dar_template**](DataAccessTemplateApi.md#update_dar_template) | **PUT** /api/v1/dar/templates/{id} | DataAccessTemplate@update


# **create_dar_template**
> CreateCategories200Response create_dar_template(create_dar_template_request)

DataAccessTemplate@store

Creates a new DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.create_categories200_response import CreateCategories200Response
from gateway_api_sdk.models.create_dar_template_request import CreateDarTemplateRequest
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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    create_dar_template_request = gateway_api_sdk.CreateDarTemplateRequest() # CreateDarTemplateRequest | DataAccessTemplate definition

    try:
        # DataAccessTemplate@store
        api_response = api_instance.create_dar_template(create_dar_template_request)
        print("The response of DataAccessTemplateApi->create_dar_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->create_dar_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_dar_template_request** | [**CreateDarTemplateRequest**](CreateDarTemplateRequest.md)| DataAccessTemplate definition | 

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

# **delete_dar_template**
> DeleteAliases200Response delete_dar_template(id)

DataAccessTemplate@destroy

Delete a system DAR template

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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    id = 1 # int | DAR template id

    try:
        # DataAccessTemplate@destroy
        api_response = api_instance.delete_dar_template(id)
        print("The response of DataAccessTemplateApi->delete_dar_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->delete_dar_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 

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

# **download_dar_template_file**
> download_dar_template_file(id)

DataAccessTemplate@downloadFile

Download the template for a file based DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    id = 1 # int | DAR template id

    try:
        # DataAccessTemplate@downloadFile
        api_instance.download_dar_template_file(id)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->download_dar_template_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 

### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: file, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **fetch_dar_template**
> FetchDarTemplate200Response fetch_dar_template(id)

DataAccessTemplate@show

Return a single DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dar_template200_response import FetchDarTemplate200Response
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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    id = 1 # int | DAR template id

    try:
        # DataAccessTemplate@show
        api_response = api_instance.fetch_dar_template(id)
        print("The response of DataAccessTemplateApi->fetch_dar_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->fetch_dar_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 

### Return type

[**FetchDarTemplate200Response**](FetchDarTemplate200Response.md)

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

# **fetch_dar_templates**
> FetchDarTemplates200Response fetch_dar_templates(with_questions=with_questions, published=published)

DataAccessTemplate@index

List of DAR templates

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dar_templates200_response import FetchDarTemplates200Response
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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    with_questions = 1 # int | Include questions in response (optional)
    published = 'true' # str | Template publication status to filter by (true, false) (optional)

    try:
        # DataAccessTemplate@index
        api_response = api_instance.fetch_dar_templates(with_questions=with_questions, published=published)
        print("The response of DataAccessTemplateApi->fetch_dar_templates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->fetch_dar_templates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **with_questions** | **int**| Include questions in response | [optional] 
 **published** | **str**| Template publication status to filter by (true, false) | [optional] 

### Return type

[**FetchDarTemplates200Response**](FetchDarTemplates200Response.md)

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

# **patch_dar_template**
> PatchDarTemplate200Response patch_dar_template(id, patch_dar_template_request, section_id=section_id)

DataAccessTemplate@update

Edit a system DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.patch_dar_template200_response import PatchDarTemplate200Response
from gateway_api_sdk.models.patch_dar_template_request import PatchDarTemplateRequest
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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    id = 1 # int | DAR template id
    patch_dar_template_request = gateway_api_sdk.PatchDarTemplateRequest() # PatchDarTemplateRequest | DataAccessTemplate definition
    section_id = 1 # int | Section id (optional)

    try:
        # DataAccessTemplate@update
        api_response = api_instance.patch_dar_template(id, patch_dar_template_request, section_id=section_id)
        print("The response of DataAccessTemplateApi->patch_dar_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->patch_dar_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 
 **patch_dar_template_request** | [**PatchDarTemplateRequest**](PatchDarTemplateRequest.md)| DataAccessTemplate definition | 
 **section_id** | **int**| Section id | [optional] 

### Return type

[**PatchDarTemplate200Response**](PatchDarTemplate200Response.md)

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

# **update_dar_template**
> FetchDarTemplate200Response update_dar_template(id, update_dar_template_request)

DataAccessTemplate@update

Update a system DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dar_template200_response import FetchDarTemplate200Response
from gateway_api_sdk.models.update_dar_template_request import UpdateDarTemplateRequest
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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    id = 1 # int | DAR template id
    update_dar_template_request = gateway_api_sdk.UpdateDarTemplateRequest() # UpdateDarTemplateRequest | DataAccessTemplate definition

    try:
        # DataAccessTemplate@update
        api_response = api_instance.update_dar_template(id, update_dar_template_request)
        print("The response of DataAccessTemplateApi->update_dar_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->update_dar_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 
 **update_dar_template_request** | [**UpdateDarTemplateRequest**](UpdateDarTemplateRequest.md)| DataAccessTemplate definition | 

### Return type

[**FetchDarTemplate200Response**](FetchDarTemplate200Response.md)

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

