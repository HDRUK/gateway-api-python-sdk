# gateway_api_sdk.NightlyDatasetTestsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_nightly_dataset_tests_v2**](NightlyDatasetTestsApi.md#fetch_nightly_dataset_tests_v2) | **GET** /api/v2/nightly_dataset_tests | NightlyDatasetTestController@index


# **fetch_nightly_dataset_tests_v2**
> FetchDatasetLinkCheckResultsV2200Response fetch_nightly_dataset_tests_v2()

NightlyDatasetTestController@index

Get the results of the nightly dataset reachability check, with a summary and a list of failures

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
    api_instance = gateway_api_sdk.NightlyDatasetTestsApi(api_client)

    try:
        # NightlyDatasetTestController@index
        api_response = api_instance.fetch_nightly_dataset_tests_v2()
        print("The response of NightlyDatasetTestsApi->fetch_nightly_dataset_tests_v2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NightlyDatasetTestsApi->fetch_nightly_dataset_tests_v2: %s\n" % e)
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

