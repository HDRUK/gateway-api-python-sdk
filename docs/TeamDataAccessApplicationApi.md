# gateway_api_sdk.TeamDataAccessApplicationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_0dabe0dfdf4eebd0c76560fd691c6472**](TeamDataAccessApplicationApi.md#call_0dabe0dfdf4eebd0c76560fd691c6472) | **GET** /api/v1/teams/{teamId}/dar/applications/{id}/showHeader | TeamDataAccessApplicationController@showHeader
[**call_0ff8ad69b213abf8d671b3695d0b69b5**](TeamDataAccessApplicationApi.md#call_0ff8ad69b213abf8d671b3695d0b69b5) | **GET** /api/v1/teams/{teamId}/dar/applications | TeamDataAccessApplicationController@index
[**call_3f8472e47cdd8aaabb42e1065a7a0afb**](TeamDataAccessApplicationApi.md#call_3f8472e47cdd8aaabb42e1065a7a0afb) | **GET** /api/v1/teams/{teamId}/dar/applications/count | TeamDataAccessApplicationController@allCounts
[**call_4e4d590ec8943163168e4fc34bd166a1**](TeamDataAccessApplicationApi.md#call_4e4d590ec8943163168e4fc34bd166a1) | **GET** /api/v1/teams/{teamId}/dar/applications/{id} | TeamDataAccessApplicationController@show
[**count_unique_fields_dar_applications**](TeamDataAccessApplicationApi.md#count_unique_fields_dar_applications) | **GET** /api/v1/teams/{teamId}/dar/applications/count/{field} | TeamDataAccessApplicationController@count


# **call_0dabe0dfdf4eebd0c76560fd691c6472**
> Model0dabe0dfdf4eebd0c76560fd691c6472200Response call_0dabe0dfdf4eebd0c76560fd691c6472(team_id, id)

TeamDataAccessApplicationController@showHeader

Get header information about a specific DAR

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model0dabe0dfdf4eebd0c76560fd691c6472200_response import Model0dabe0dfdf4eebd0c76560fd691c6472200Response
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
    api_instance = gateway_api_sdk.TeamDataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # TeamDataAccessApplicationController@showHeader
        api_response = api_instance.call_0dabe0dfdf4eebd0c76560fd691c6472(team_id, id)
        print("The response of TeamDataAccessApplicationApi->call_0dabe0dfdf4eebd0c76560fd691c6472:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessApplicationApi->call_0dabe0dfdf4eebd0c76560fd691c6472: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model0dabe0dfdf4eebd0c76560fd691c6472200Response**](Model0dabe0dfdf4eebd0c76560fd691c6472200Response.md)

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

# **call_0ff8ad69b213abf8d671b3695d0b69b5**
> Model0ff8ad69b213abf8d671b3695d0b69b5200Response call_0ff8ad69b213abf8d671b3695d0b69b5(team_id)

TeamDataAccessApplicationController@index

List of dar applications belonging to a team

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model0ff8ad69b213abf8d671b3695d0b69b5200_response import Model0ff8ad69b213abf8d671b3695d0b69b5200Response
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
    api_instance = gateway_api_sdk.TeamDataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id

    try:
        # TeamDataAccessApplicationController@index
        api_response = api_instance.call_0ff8ad69b213abf8d671b3695d0b69b5(team_id)
        print("The response of TeamDataAccessApplicationApi->call_0ff8ad69b213abf8d671b3695d0b69b5:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessApplicationApi->call_0ff8ad69b213abf8d671b3695d0b69b5: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 

### Return type

[**Model0ff8ad69b213abf8d671b3695d0b69b5200Response**](Model0ff8ad69b213abf8d671b3695d0b69b5200Response.md)

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

# **call_3f8472e47cdd8aaabb42e1065a7a0afb**
> CountUniqueFieldsCollections200Response call_3f8472e47cdd8aaabb42e1065a7a0afb(team_id)

TeamDataAccessApplicationController@allCounts

Get Counts for all status fields in the model

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.count_unique_fields_collections200_response import CountUniqueFieldsCollections200Response
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
    api_instance = gateway_api_sdk.TeamDataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id

    try:
        # TeamDataAccessApplicationController@allCounts
        api_response = api_instance.call_3f8472e47cdd8aaabb42e1065a7a0afb(team_id)
        print("The response of TeamDataAccessApplicationApi->call_3f8472e47cdd8aaabb42e1065a7a0afb:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessApplicationApi->call_3f8472e47cdd8aaabb42e1065a7a0afb: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 

### Return type

[**CountUniqueFieldsCollections200Response**](CountUniqueFieldsCollections200Response.md)

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

# **call_4e4d590ec8943163168e4fc34bd166a1**
> Model4e4d590ec8943163168e4fc34bd166a1200Response call_4e4d590ec8943163168e4fc34bd166a1(team_id, id)

TeamDataAccessApplicationController@show

Return a single DAR application

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model4e4d590ec8943163168e4fc34bd166a1200_response import Model4e4d590ec8943163168e4fc34bd166a1200Response
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
    api_instance = gateway_api_sdk.TeamDataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    id = 1 # int | DAR application id

    try:
        # TeamDataAccessApplicationController@show
        api_response = api_instance.call_4e4d590ec8943163168e4fc34bd166a1(team_id, id)
        print("The response of TeamDataAccessApplicationApi->call_4e4d590ec8943163168e4fc34bd166a1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessApplicationApi->call_4e4d590ec8943163168e4fc34bd166a1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **id** | **int**| DAR application id | 

### Return type

[**Model4e4d590ec8943163168e4fc34bd166a1200Response**](Model4e4d590ec8943163168e4fc34bd166a1200Response.md)

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

# **count_unique_fields_dar_applications**
> CountUniqueFieldsCollections200Response count_unique_fields_dar_applications(team_id, var_field)

TeamDataAccessApplicationController@count

Get Counts for distinct entries of a field in the model

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.count_unique_fields_collections200_response import CountUniqueFieldsCollections200Response
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
    api_instance = gateway_api_sdk.TeamDataAccessApplicationApi(api_client)
    team_id = 1 # int | Team id
    var_field = 'approval_status' # str | name of the field to perform a count on

    try:
        # TeamDataAccessApplicationController@count
        api_response = api_instance.count_unique_fields_dar_applications(team_id, var_field)
        print("The response of TeamDataAccessApplicationApi->count_unique_fields_dar_applications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamDataAccessApplicationApi->count_unique_fields_dar_applications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **int**| Team id | 
 **var_field** | **str**| name of the field to perform a count on | 

### Return type

[**CountUniqueFieldsCollections200Response**](CountUniqueFieldsCollections200Response.md)

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

