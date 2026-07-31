# gateway_api_sdk.DataAccessTemplateApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**b1fa0f3b5f03176ce6b96d1d4ee27aa8**](DataAccessTemplateApi.md#b1fa0f3b5f03176ce6b96d1d4ee27aa8) | **GET** /ap1/v1/dar/templates/{id}/download | DataAccessTemplate@downloadFile
[**c0e9ad253ec08e6e03a40ed8759e744d**](DataAccessTemplateApi.md#c0e9ad253ec08e6e03a40ed8759e744d) | **DELETE** /api/v1/dar/templates/{id} | DataAccessTemplate@destroy
[**call_234386e06c6b29d5aaca2ed8f89cb9aa**](DataAccessTemplateApi.md#call_234386e06c6b29d5aaca2ed8f89cb9aa) | **GET** /api/v1/dar/templates | DataAccessTemplate@index
[**call_3f2b4dcc3b5e548e62f79a32aa8f0052**](DataAccessTemplateApi.md#call_3f2b4dcc3b5e548e62f79a32aa8f0052) | **GET** /api/v1/dar/templates/{id} | DataAccessTemplate@show
[**call_6196987e50c600396a439939cea635a3**](DataAccessTemplateApi.md#call_6196987e50c600396a439939cea635a3) | **PATCH** /api/v1/dar/templates/{id} | DataAccessTemplate@update
[**call_6dae0c2af6ca442f90a65e7c65a13252**](DataAccessTemplateApi.md#call_6dae0c2af6ca442f90a65e7c65a13252) | **PUT** /api/v1/dar/templates/{id} | DataAccessTemplate@update
[**call_70d4b0fcc281e6491f510f58028762c9**](DataAccessTemplateApi.md#call_70d4b0fcc281e6491f510f58028762c9) | **POST** /api/v1/dar/templates | DataAccessTemplate@store


# **b1fa0f3b5f03176ce6b96d1d4ee27aa8**
> b1fa0f3b5f03176ce6b96d1d4ee27aa8(id)

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
        api_instance.b1fa0f3b5f03176ce6b96d1d4ee27aa8(id)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->b1fa0f3b5f03176ce6b96d1d4ee27aa8: %s\n" % e)
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

# **c0e9ad253ec08e6e03a40ed8759e744d**
> C29b5b3424f7317b69b4bda048ccfafb200Response c0e9ad253ec08e6e03a40ed8759e744d(id)

DataAccessTemplate@destroy

Delete a system DAR template

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
    api_instance = gateway_api_sdk.DataAccessTemplateApi(api_client)
    id = 1 # int | DAR template id

    try:
        # DataAccessTemplate@destroy
        api_response = api_instance.c0e9ad253ec08e6e03a40ed8759e744d(id)
        print("The response of DataAccessTemplateApi->c0e9ad253ec08e6e03a40ed8759e744d:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->c0e9ad253ec08e6e03a40ed8759e744d: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 

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

# **call_234386e06c6b29d5aaca2ed8f89cb9aa**
> Model234386e06c6b29d5aaca2ed8f89cb9aa200Response call_234386e06c6b29d5aaca2ed8f89cb9aa(with_questions=with_questions, published=published)

DataAccessTemplate@index

List of DAR templates

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model234386e06c6b29d5aaca2ed8f89cb9aa200_response import Model234386e06c6b29d5aaca2ed8f89cb9aa200Response
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
        api_response = api_instance.call_234386e06c6b29d5aaca2ed8f89cb9aa(with_questions=with_questions, published=published)
        print("The response of DataAccessTemplateApi->call_234386e06c6b29d5aaca2ed8f89cb9aa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->call_234386e06c6b29d5aaca2ed8f89cb9aa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **with_questions** | **int**| Include questions in response | [optional] 
 **published** | **str**| Template publication status to filter by (true, false) | [optional] 

### Return type

[**Model234386e06c6b29d5aaca2ed8f89cb9aa200Response**](Model234386e06c6b29d5aaca2ed8f89cb9aa200Response.md)

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

# **call_3f2b4dcc3b5e548e62f79a32aa8f0052**
> Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response call_3f2b4dcc3b5e548e62f79a32aa8f0052(id)

DataAccessTemplate@show

Return a single DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model3f2b4dcc3b5e548e62f79a32aa8f0052200_response import Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response
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
        api_response = api_instance.call_3f2b4dcc3b5e548e62f79a32aa8f0052(id)
        print("The response of DataAccessTemplateApi->call_3f2b4dcc3b5e548e62f79a32aa8f0052:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->call_3f2b4dcc3b5e548e62f79a32aa8f0052: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 

### Return type

[**Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response**](Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response.md)

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

# **call_6196987e50c600396a439939cea635a3**
> Model6196987e50c600396a439939cea635a3200Response call_6196987e50c600396a439939cea635a3(id, model6196987e50c600396a439939cea635a3_request, section_id=section_id)

DataAccessTemplate@update

Edit a system DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model6196987e50c600396a439939cea635a3200_response import Model6196987e50c600396a439939cea635a3200Response
from gateway_api_sdk.models.model6196987e50c600396a439939cea635a3_request import Model6196987e50c600396a439939cea635a3Request
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
    model6196987e50c600396a439939cea635a3_request = gateway_api_sdk.Model6196987e50c600396a439939cea635a3Request() # Model6196987e50c600396a439939cea635a3Request | DataAccessTemplate definition
    section_id = 1 # int | Section id (optional)

    try:
        # DataAccessTemplate@update
        api_response = api_instance.call_6196987e50c600396a439939cea635a3(id, model6196987e50c600396a439939cea635a3_request, section_id=section_id)
        print("The response of DataAccessTemplateApi->call_6196987e50c600396a439939cea635a3:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->call_6196987e50c600396a439939cea635a3: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 
 **model6196987e50c600396a439939cea635a3_request** | [**Model6196987e50c600396a439939cea635a3Request**](Model6196987e50c600396a439939cea635a3Request.md)| DataAccessTemplate definition | 
 **section_id** | **int**| Section id | [optional] 

### Return type

[**Model6196987e50c600396a439939cea635a3200Response**](Model6196987e50c600396a439939cea635a3200Response.md)

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

# **call_6dae0c2af6ca442f90a65e7c65a13252**
> Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response call_6dae0c2af6ca442f90a65e7c65a13252(id, model6dae0c2af6ca442f90a65e7c65a13252_request)

DataAccessTemplate@update

Update a system DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model3f2b4dcc3b5e548e62f79a32aa8f0052200_response import Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response
from gateway_api_sdk.models.model6dae0c2af6ca442f90a65e7c65a13252_request import Model6dae0c2af6ca442f90a65e7c65a13252Request
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
    model6dae0c2af6ca442f90a65e7c65a13252_request = gateway_api_sdk.Model6dae0c2af6ca442f90a65e7c65a13252Request() # Model6dae0c2af6ca442f90a65e7c65a13252Request | DataAccessTemplate definition

    try:
        # DataAccessTemplate@update
        api_response = api_instance.call_6dae0c2af6ca442f90a65e7c65a13252(id, model6dae0c2af6ca442f90a65e7c65a13252_request)
        print("The response of DataAccessTemplateApi->call_6dae0c2af6ca442f90a65e7c65a13252:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->call_6dae0c2af6ca442f90a65e7c65a13252: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| DAR template id | 
 **model6dae0c2af6ca442f90a65e7c65a13252_request** | [**Model6dae0c2af6ca442f90a65e7c65a13252Request**](Model6dae0c2af6ca442f90a65e7c65a13252Request.md)| DataAccessTemplate definition | 

### Return type

[**Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response**](Model3f2b4dcc3b5e548e62f79a32aa8f0052200Response.md)

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

# **call_70d4b0fcc281e6491f510f58028762c9**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_70d4b0fcc281e6491f510f58028762c9(model70d4b0fcc281e6491f510f58028762c9_request)

DataAccessTemplate@store

Creates a new DAR template

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model70d4b0fcc281e6491f510f58028762c9_request import Model70d4b0fcc281e6491f510f58028762c9Request
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
    model70d4b0fcc281e6491f510f58028762c9_request = gateway_api_sdk.Model70d4b0fcc281e6491f510f58028762c9Request() # Model70d4b0fcc281e6491f510f58028762c9Request | DataAccessTemplate definition

    try:
        # DataAccessTemplate@store
        api_response = api_instance.call_70d4b0fcc281e6491f510f58028762c9(model70d4b0fcc281e6491f510f58028762c9_request)
        print("The response of DataAccessTemplateApi->call_70d4b0fcc281e6491f510f58028762c9:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplateApi->call_70d4b0fcc281e6491f510f58028762c9: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model70d4b0fcc281e6491f510f58028762c9_request** | [**Model70d4b0fcc281e6491f510f58028762c9Request**](Model70d4b0fcc281e6491f510f58028762c9Request.md)| DataAccessTemplate definition | 

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
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

