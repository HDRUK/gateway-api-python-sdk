# gateway_api_sdk.LicenseApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**b34ab4eadc1eaed469678151e6e71b9f**](LicenseApi.md#b34ab4eadc1eaed469678151e6e71b9f) | **GET** /api/v1/licenses | License@index
[**call_2721b23c1df3b4e71706e4ab04f9b0a8**](LicenseApi.md#call_2721b23c1df3b4e71706e4ab04f9b0a8) | **POST** /api/v1/licenses | License@store
[**call_50c6be78401c528ffdf4ed00414e7678**](LicenseApi.md#call_50c6be78401c528ffdf4ed00414e7678) | **GET** /api/v1/licenses/{id} | License@show
[**call_98a20646cb4164cddd79725baf3dcf61**](LicenseApi.md#call_98a20646cb4164cddd79725baf3dcf61) | **PUT** /api/v1/licenses/{id} | License@update
[**call_991d716a8c83b7e3c4747583eeffc0ee**](LicenseApi.md#call_991d716a8c83b7e3c4747583eeffc0ee) | **DELETE** /api/v1/licenses/{id} | License@destroy
[**fc8a99b7173f11228400fac2754185fa**](LicenseApi.md#fc8a99b7173f11228400fac2754185fa) | **PATCH** /api/v1/licenses/{id} | License@edit


# **b34ab4eadc1eaed469678151e6e71b9f**
> B34ab4eadc1eaed469678151e6e71b9f200Response b34ab4eadc1eaed469678151e6e71b9f()

License@index

Returns a list of licenses available

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.b34ab4eadc1eaed469678151e6e71b9f200_response import B34ab4eadc1eaed469678151e6e71b9f200Response
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
        api_response = api_instance.b34ab4eadc1eaed469678151e6e71b9f()
        print("The response of LicenseApi->b34ab4eadc1eaed469678151e6e71b9f:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->b34ab4eadc1eaed469678151e6e71b9f: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**B34ab4eadc1eaed469678151e6e71b9f200Response**](B34ab4eadc1eaed469678151e6e71b9f200Response.md)

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

# **call_2721b23c1df3b4e71706e4ab04f9b0a8**
> Dd76b8d73b7ea8b4951f03d7c0904c92200Response call_2721b23c1df3b4e71706e4ab04f9b0a8(model2721b23c1df3b4e71706e4ab04f9b0a8_request)

License@store

Creates a new license

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.dd76b8d73b7ea8b4951f03d7c0904c92200_response import Dd76b8d73b7ea8b4951f03d7c0904c92200Response
from gateway_api_sdk.models.model2721b23c1df3b4e71706e4ab04f9b0a8_request import Model2721b23c1df3b4e71706e4ab04f9b0a8Request
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
    model2721b23c1df3b4e71706e4ab04f9b0a8_request = gateway_api_sdk.Model2721b23c1df3b4e71706e4ab04f9b0a8Request() # Model2721b23c1df3b4e71706e4ab04f9b0a8Request | License definition

    try:
        # License@store
        api_response = api_instance.call_2721b23c1df3b4e71706e4ab04f9b0a8(model2721b23c1df3b4e71706e4ab04f9b0a8_request)
        print("The response of LicenseApi->call_2721b23c1df3b4e71706e4ab04f9b0a8:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->call_2721b23c1df3b4e71706e4ab04f9b0a8: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model2721b23c1df3b4e71706e4ab04f9b0a8_request** | [**Model2721b23c1df3b4e71706e4ab04f9b0a8Request**](Model2721b23c1df3b4e71706e4ab04f9b0a8Request.md)| License definition | 

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

# **call_50c6be78401c528ffdf4ed00414e7678**
> Model50c6be78401c528ffdf4ed00414e7678200Response call_50c6be78401c528ffdf4ed00414e7678(id)

License@show

Return a single license

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.model50c6be78401c528ffdf4ed00414e7678200_response import Model50c6be78401c528ffdf4ed00414e7678200Response
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
        api_response = api_instance.call_50c6be78401c528ffdf4ed00414e7678(id)
        print("The response of LicenseApi->call_50c6be78401c528ffdf4ed00414e7678:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->call_50c6be78401c528ffdf4ed00414e7678: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| License ID | 

### Return type

[**Model50c6be78401c528ffdf4ed00414e7678200Response**](Model50c6be78401c528ffdf4ed00414e7678200Response.md)

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

# **call_98a20646cb4164cddd79725baf3dcf61**
> Model98a20646cb4164cddd79725baf3dcf61200Response call_98a20646cb4164cddd79725baf3dcf61(id, model2721b23c1df3b4e71706e4ab04f9b0a8_request)

License@update

Update a tool license

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model2721b23c1df3b4e71706e4ab04f9b0a8_request import Model2721b23c1df3b4e71706e4ab04f9b0a8Request
from gateway_api_sdk.models.model98a20646cb4164cddd79725baf3dcf61200_response import Model98a20646cb4164cddd79725baf3dcf61200Response
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
    model2721b23c1df3b4e71706e4ab04f9b0a8_request = gateway_api_sdk.Model2721b23c1df3b4e71706e4ab04f9b0a8Request() # Model2721b23c1df3b4e71706e4ab04f9b0a8Request | Category definition

    try:
        # License@update
        api_response = api_instance.call_98a20646cb4164cddd79725baf3dcf61(id, model2721b23c1df3b4e71706e4ab04f9b0a8_request)
        print("The response of LicenseApi->call_98a20646cb4164cddd79725baf3dcf61:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->call_98a20646cb4164cddd79725baf3dcf61: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| license id | 
 **model2721b23c1df3b4e71706e4ab04f9b0a8_request** | [**Model2721b23c1df3b4e71706e4ab04f9b0a8Request**](Model2721b23c1df3b4e71706e4ab04f9b0a8Request.md)| Category definition | 

### Return type

[**Model98a20646cb4164cddd79725baf3dcf61200Response**](Model98a20646cb4164cddd79725baf3dcf61200Response.md)

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

# **call_991d716a8c83b7e3c4747583eeffc0ee**
> C29b5b3424f7317b69b4bda048ccfafb200Response call_991d716a8c83b7e3c4747583eeffc0ee(id)

License@destroy

Delete a License

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
    api_instance = gateway_api_sdk.LicenseApi(api_client)
    id = 1 # int | License id

    try:
        # License@destroy
        api_response = api_instance.call_991d716a8c83b7e3c4747583eeffc0ee(id)
        print("The response of LicenseApi->call_991d716a8c83b7e3c4747583eeffc0ee:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->call_991d716a8c83b7e3c4747583eeffc0ee: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| License id | 

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

# **fc8a99b7173f11228400fac2754185fa**
> Model98a20646cb4164cddd79725baf3dcf61200Response fc8a99b7173f11228400fac2754185fa(id, model2721b23c1df3b4e71706e4ab04f9b0a8_request)

License@edit

Edit a tool license

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model2721b23c1df3b4e71706e4ab04f9b0a8_request import Model2721b23c1df3b4e71706e4ab04f9b0a8Request
from gateway_api_sdk.models.model98a20646cb4164cddd79725baf3dcf61200_response import Model98a20646cb4164cddd79725baf3dcf61200Response
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
    model2721b23c1df3b4e71706e4ab04f9b0a8_request = gateway_api_sdk.Model2721b23c1df3b4e71706e4ab04f9b0a8Request() # Model2721b23c1df3b4e71706e4ab04f9b0a8Request | Category definition

    try:
        # License@edit
        api_response = api_instance.fc8a99b7173f11228400fac2754185fa(id, model2721b23c1df3b4e71706e4ab04f9b0a8_request)
        print("The response of LicenseApi->fc8a99b7173f11228400fac2754185fa:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LicenseApi->fc8a99b7173f11228400fac2754185fa: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| license id | 
 **model2721b23c1df3b4e71706e4ab04f9b0a8_request** | [**Model2721b23c1df3b4e71706e4ab04f9b0a8Request**](Model2721b23c1df3b4e71706e4ab04f9b0a8Request.md)| Category definition | 

### Return type

[**Model98a20646cb4164cddd79725baf3dcf61200Response**](Model98a20646cb4164cddd79725baf3dcf61200Response.md)

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

