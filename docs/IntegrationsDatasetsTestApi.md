# gateway_api_sdk.IntegrationsDatasetsTestApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**integrations_datasets_test**](IntegrationsDatasetsTestApi.md#integrations_datasets_test) | **POST** /api/v1/integrations/datasets/test | IntegrationDatasetController@datasetTest


# **integrations_datasets_test**
> CreateDarIntegration201Response integrations_datasets_test(datasets_test_request)

IntegrationDatasetController@datasetTest

Integrations datasets test

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.create_dar_integration201_response import CreateDarIntegration201Response
from gateway_api_sdk.models.datasets_test_request import DatasetsTestRequest
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
    api_instance = gateway_api_sdk.IntegrationsDatasetsTestApi(api_client)
    datasets_test_request = gateway_api_sdk.DatasetsTestRequest() # DatasetsTestRequest | Pass datasets payload

    try:
        # IntegrationDatasetController@datasetTest
        api_response = api_instance.integrations_datasets_test(datasets_test_request)
        print("The response of IntegrationsDatasetsTestApi->integrations_datasets_test:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IntegrationsDatasetsTestApi->integrations_datasets_test: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **datasets_test_request** | [**DatasetsTestRequest**](DatasetsTestRequest.md)| Pass datasets payload | 

### Return type

[**CreateDarIntegration201Response**](CreateDarIntegration201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**401** | Unauthorized |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

