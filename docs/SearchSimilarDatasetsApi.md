# gateway_api_sdk.SearchSimilarDatasetsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**cd41e1bd1b9f9918da2bb53a240b8bfe**](SearchSimilarDatasetsApi.md#cd41e1bd1b9f9918da2bb53a240b8bfe) | **POST** /api/v1/search/similar/datasets | Search@similarDatasets


# **cd41e1bd1b9f9918da2bb53a240b8bfe**
> Cd41e1bd1b9f9918da2bb53a240b8bfe200Response cd41e1bd1b9f9918da2bb53a240b8bfe(cd41e1bd1b9f9918da2bb53a240b8bfe_request)

Search@similarDatasets

Returns top three gateway datasets most similar to the provided dataset

### Example


```python
import gateway_api_sdk
from gateway_api_sdk.models.cd41e1bd1b9f9918da2bb53a240b8bfe200_response import Cd41e1bd1b9f9918da2bb53a240b8bfe200Response
from gateway_api_sdk.models.cd41e1bd1b9f9918da2bb53a240b8bfe_request import Cd41e1bd1b9f9918da2bb53a240b8bfeRequest
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
    api_instance = gateway_api_sdk.SearchSimilarDatasetsApi(api_client)
    cd41e1bd1b9f9918da2bb53a240b8bfe_request = gateway_api_sdk.Cd41e1bd1b9f9918da2bb53a240b8bfeRequest() # Cd41e1bd1b9f9918da2bb53a240b8bfeRequest | Submit dataset id

    try:
        # Search@similarDatasets
        api_response = api_instance.cd41e1bd1b9f9918da2bb53a240b8bfe(cd41e1bd1b9f9918da2bb53a240b8bfe_request)
        print("The response of SearchSimilarDatasetsApi->cd41e1bd1b9f9918da2bb53a240b8bfe:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchSimilarDatasetsApi->cd41e1bd1b9f9918da2bb53a240b8bfe: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cd41e1bd1b9f9918da2bb53a240b8bfe_request** | [**Cd41e1bd1b9f9918da2bb53a240b8bfeRequest**](Cd41e1bd1b9f9918da2bb53a240b8bfeRequest.md)| Submit dataset id | 

### Return type

[**Cd41e1bd1b9f9918da2bb53a240b8bfe200Response**](Cd41e1bd1b9f9918da2bb53a240b8bfe200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

