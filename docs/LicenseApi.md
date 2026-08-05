# gateway_api_sdk.LicenseApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_all_licenses**](LicenseApi.md#fetch_all_licenses) | **GET** /api/v1/licenses | License@index
[**fetch_licenses**](LicenseApi.md#fetch_licenses) | **GET** /api/v1/licenses/{id} | License@show


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

