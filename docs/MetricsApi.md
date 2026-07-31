# gateway_api_sdk.MetricsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_key_metrics_v2**](MetricsApi.md#fetch_key_metrics_v2) | **GET** /api/v2/metrics | KeyMetricController@index


# **fetch_key_metrics_v2**
> FetchKeyMetricsV2200Response fetch_key_metrics_v2()

KeyMetricController@index

Get key metrics

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_key_metrics_v2200_response import FetchKeyMetricsV2200Response
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
    api_instance = gateway_api_sdk.MetricsApi(api_client)

    try:
        # KeyMetricController@index
        api_response = api_instance.fetch_key_metrics_v2()
        print("The response of MetricsApi->fetch_key_metrics_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetricsApi->fetch_key_metrics_v2: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchKeyMetricsV2200Response**](FetchKeyMetricsV2200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

