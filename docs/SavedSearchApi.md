# gateway_api_sdk.SavedSearchApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_39500344ecf1a14150bbe26c4a138c56**](SavedSearchApi.md#call_39500344ecf1a14150bbe26c4a138c56) | **POST** /api/v1/saved_searches | SavedSearch@store
[**call_3b59d921ea47286a669054ef67350b03**](SavedSearchApi.md#call_3b59d921ea47286a669054ef67350b03) | **PUT** /api/v1/saved_searches/{id} | SavedSearch@update
[**call_4f2a3c56631a5fccb45a9e7972df02b0**](SavedSearchApi.md#call_4f2a3c56631a5fccb45a9e7972df02b0) | **GET** /api/v1/saved_searches | SavedSearch@index
[**call_8d6878e4937dd67c5e2480c6f4e9149f**](SavedSearchApi.md#call_8d6878e4937dd67c5e2480c6f4e9149f) | **GET** /api/v1/saved_searches/{id} | SavedSearch@show
[**cdcdceead49fe1554534af83c50c8af5**](SavedSearchApi.md#cdcdceead49fe1554534af83c50c8af5) | **DELETE** /api/v1/saved_searches/{id} | SavedSearch@destroy
[**fa314398c7a73002fee4ffc7e62e9fb6**](SavedSearchApi.md#fa314398c7a73002fee4ffc7e62e9fb6) | **PATCH** /api/v1/saved_searches/{id} | SavedSearch@update


# **call_39500344ecf1a14150bbe26c4a138c56**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_39500344ecf1a14150bbe26c4a138c56(model39500344ecf1a14150bbe26c4a138c56_request)

SavedSearch@store

Creates a new saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model39500344ecf1a14150bbe26c4a138c56_request import Model39500344ecf1a14150bbe26c4a138c56Request
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    model39500344ecf1a14150bbe26c4a138c56_request = gateway_api_sdk.Model39500344ecf1a14150bbe26c4a138c56Request() # Model39500344ecf1a14150bbe26c4a138c56Request | Saved search definition

    try:
        # SavedSearch@store
        api_response = api_instance.call_39500344ecf1a14150bbe26c4a138c56(model39500344ecf1a14150bbe26c4a138c56_request)
        print("The response of SavedSearchApi->call_39500344ecf1a14150bbe26c4a138c56:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->call_39500344ecf1a14150bbe26c4a138c56: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model39500344ecf1a14150bbe26c4a138c56_request** | [**Model39500344ecf1a14150bbe26c4a138c56Request**](Model39500344ecf1a14150bbe26c4a138c56Request.md)| Saved search definition | 

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

# **call_3b59d921ea47286a669054ef67350b03**
> Model3b59d921ea47286a669054ef67350b03200Response call_3b59d921ea47286a669054ef67350b03(id, model3b59d921ea47286a669054ef67350b03_request)

SavedSearch@update

Update a saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model3b59d921ea47286a669054ef67350b03200_response import Model3b59d921ea47286a669054ef67350b03200Response
from gateway_api_sdk.models.model3b59d921ea47286a669054ef67350b03_request import Model3b59d921ea47286a669054ef67350b03Request
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id
    model3b59d921ea47286a669054ef67350b03_request = gateway_api_sdk.Model3b59d921ea47286a669054ef67350b03Request() # Model3b59d921ea47286a669054ef67350b03Request | Saved search definition

    try:
        # SavedSearch@update
        api_response = api_instance.call_3b59d921ea47286a669054ef67350b03(id, model3b59d921ea47286a669054ef67350b03_request)
        print("The response of SavedSearchApi->call_3b59d921ea47286a669054ef67350b03:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->call_3b59d921ea47286a669054ef67350b03: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 
 **model3b59d921ea47286a669054ef67350b03_request** | [**Model3b59d921ea47286a669054ef67350b03Request**](Model3b59d921ea47286a669054ef67350b03Request.md)| Saved search definition | 

### Return type

[**Model3b59d921ea47286a669054ef67350b03200Response**](Model3b59d921ea47286a669054ef67350b03200Response.md)

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

# **call_4f2a3c56631a5fccb45a9e7972df02b0**
> Model4f2a3c56631a5fccb45a9e7972df02b0200Response call_4f2a3c56631a5fccb45a9e7972df02b0(per_page=per_page)

SavedSearch@index

Returns a list of saved searches enabled on the system

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model4f2a3c56631a5fccb45a9e7972df02b0200_response import Model4f2a3c56631a5fccb45a9e7972df02b0200Response
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    per_page = 56 # int | Specify number of results per page (optional)

    try:
        # SavedSearch@index
        api_response = api_instance.call_4f2a3c56631a5fccb45a9e7972df02b0(per_page=per_page)
        print("The response of SavedSearchApi->call_4f2a3c56631a5fccb45a9e7972df02b0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->call_4f2a3c56631a5fccb45a9e7972df02b0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| Specify number of results per page | [optional] 

### Return type

[**Model4f2a3c56631a5fccb45a9e7972df02b0200Response**](Model4f2a3c56631a5fccb45a9e7972df02b0200Response.md)

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

# **call_8d6878e4937dd67c5e2480c6f4e9149f**
> Model4f2a3c56631a5fccb45a9e7972df02b0200Response call_8d6878e4937dd67c5e2480c6f4e9149f(id)

SavedSearch@show

Return a single saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model4f2a3c56631a5fccb45a9e7972df02b0200_response import Model4f2a3c56631a5fccb45a9e7972df02b0200Response
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id

    try:
        # SavedSearch@show
        api_response = api_instance.call_8d6878e4937dd67c5e2480c6f4e9149f(id)
        print("The response of SavedSearchApi->call_8d6878e4937dd67c5e2480c6f4e9149f:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->call_8d6878e4937dd67c5e2480c6f4e9149f: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 

### Return type

[**Model4f2a3c56631a5fccb45a9e7972df02b0200Response**](Model4f2a3c56631a5fccb45a9e7972df02b0200Response.md)

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

# **cdcdceead49fe1554534af83c50c8af5**
> C29b5b3424f7317b69b4bda048ccfafb200Response cdcdceead49fe1554534af83c50c8af5(id)

SavedSearch@destroy

Delete a saved search

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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id

    try:
        # SavedSearch@destroy
        api_response = api_instance.cdcdceead49fe1554534af83c50c8af5(id)
        print("The response of SavedSearchApi->cdcdceead49fe1554534af83c50c8af5:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->cdcdceead49fe1554534af83c50c8af5: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 

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

# **fa314398c7a73002fee4ffc7e62e9fb6**
> Model3b59d921ea47286a669054ef67350b03200Response fa314398c7a73002fee4ffc7e62e9fb6(id, fa314398c7a73002fee4ffc7e62e9fb6_request)

SavedSearch@update

Edit a saved search

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.fa314398c7a73002fee4ffc7e62e9fb6_request import Fa314398c7a73002fee4ffc7e62e9fb6Request
from gateway_api_sdk.models.model3b59d921ea47286a669054ef67350b03200_response import Model3b59d921ea47286a669054ef67350b03200Response
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
    api_instance = gateway_api_sdk.SavedSearchApi(api_client)
    id = 1 # int | saved search id
    fa314398c7a73002fee4ffc7e62e9fb6_request = gateway_api_sdk.Fa314398c7a73002fee4ffc7e62e9fb6Request() # Fa314398c7a73002fee4ffc7e62e9fb6Request | Saved search definition

    try:
        # SavedSearch@update
        api_response = api_instance.fa314398c7a73002fee4ffc7e62e9fb6(id, fa314398c7a73002fee4ffc7e62e9fb6_request)
        print("The response of SavedSearchApi->fa314398c7a73002fee4ffc7e62e9fb6:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavedSearchApi->fa314398c7a73002fee4ffc7e62e9fb6: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| saved search id | 
 **fa314398c7a73002fee4ffc7e62e9fb6_request** | [**Fa314398c7a73002fee4ffc7e62e9fb6Request**](Fa314398c7a73002fee4ffc7e62e9fb6Request.md)| Saved search definition | 

### Return type

[**Model3b59d921ea47286a669054ef67350b03200Response**](Model3b59d921ea47286a669054ef67350b03200Response.md)

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

