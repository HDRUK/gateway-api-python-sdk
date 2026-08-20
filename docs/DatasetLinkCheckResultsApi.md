# gateway_api_sdk.DatasetLinkCheckResultsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_dataset_link_check_results_v2**](DatasetLinkCheckResultsApi.md#fetch_dataset_link_check_results_v2) | **GET** /api/v2/dataset_link_check_results | DatasetLinkCheckResultController@index


# **fetch_dataset_link_check_results_v2**
> FetchDatasetLinkCheckResultsV2200Response fetch_dataset_link_check_results_v2()

DatasetLinkCheckResultController@index

Get the confirmed dead links (HTTP 404, verified across multiple checks) found in active dataset metadata by the nightly link check

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.fetch_dataset_link_check_results_v2200_response import FetchDatasetLinkCheckResultsV2200Response
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
    api_instance = gateway_api_sdk.DatasetLinkCheckResultsApi(api_client)

    try:
        # DatasetLinkCheckResultController@index
        api_response = api_instance.fetch_dataset_link_check_results_v2()
        print("The response of DatasetLinkCheckResultsApi->fetch_dataset_link_check_results_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DatasetLinkCheckResultsApi->fetch_dataset_link_check_results_v2: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FetchDatasetLinkCheckResultsV2200Response**](FetchDatasetLinkCheckResultsV2200Response.md)

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

