# gateway_api_sdk.SearchPublicationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_9946399cbddb0dcadcbd5801e5ee1dd4**](SearchPublicationsApi.md#call_9946399cbddb0dcadcbd5801e5ee1dd4) | **POST** /api/v1/search/publications | Search@publications
[**call_9a0abfa6186327d43c51259d5b524fde**](SearchPublicationsApi.md#call_9a0abfa6186327d43c51259d5b524fde) | **POST** /api/v1/search/doi | Search@publications


# **call_9946399cbddb0dcadcbd5801e5ee1dd4**
> Model9946399cbddb0dcadcbd5801e5ee1dd4200Response call_9946399cbddb0dcadcbd5801e5ee1dd4(model9946399cbddb0dcadcbd5801e5ee1dd4_request, sort=sort, direction=direction, source=source)

Search@publications

Returns gateway publications related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model9946399cbddb0dcadcbd5801e5ee1dd4200_response import Model9946399cbddb0dcadcbd5801e5ee1dd4200Response
from gateway_api_sdk.models.model9946399cbddb0dcadcbd5801e5ee1dd4_request import Model9946399cbddb0dcadcbd5801e5ee1dd4Request
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
    api_instance = gateway_api_sdk.SearchPublicationsApi(api_client)
    model9946399cbddb0dcadcbd5801e5ee1dd4_request = gateway_api_sdk.Model9946399cbddb0dcadcbd5801e5ee1dd4Request() # Model9946399cbddb0dcadcbd5801e5ee1dd4Request | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)
    source = 'GAT' # str | Which source to search ('GAT' or 'FED', default: 'GAT') (optional)

    try:
        # Search@publications
        api_response = api_instance.call_9946399cbddb0dcadcbd5801e5ee1dd4(model9946399cbddb0dcadcbd5801e5ee1dd4_request, sort=sort, direction=direction, source=source)
        print("The response of SearchPublicationsApi->call_9946399cbddb0dcadcbd5801e5ee1dd4:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchPublicationsApi->call_9946399cbddb0dcadcbd5801e5ee1dd4: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model9946399cbddb0dcadcbd5801e5ee1dd4_request** | [**Model9946399cbddb0dcadcbd5801e5ee1dd4Request**](Model9946399cbddb0dcadcbd5801e5ee1dd4Request.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 
 **source** | **str**| Which source to search (&#39;GAT&#39; or &#39;FED&#39;, default: &#39;GAT&#39;) | [optional] 

### Return type

[**Model9946399cbddb0dcadcbd5801e5ee1dd4200Response**](Model9946399cbddb0dcadcbd5801e5ee1dd4200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **call_9a0abfa6186327d43c51259d5b524fde**
> Model9a0abfa6186327d43c51259d5b524fde200Response call_9a0abfa6186327d43c51259d5b524fde(model9a0abfa6186327d43c51259d5b524fde_request)

Search@publications

Returns publications from EuropePMC matching a give DOI

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.model9a0abfa6186327d43c51259d5b524fde200_response import Model9a0abfa6186327d43c51259d5b524fde200Response
from gateway_api_sdk.models.model9a0abfa6186327d43c51259d5b524fde_request import Model9a0abfa6186327d43c51259d5b524fdeRequest
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
    api_instance = gateway_api_sdk.SearchPublicationsApi(api_client)
    model9a0abfa6186327d43c51259d5b524fde_request = gateway_api_sdk.Model9a0abfa6186327d43c51259d5b524fdeRequest() # Model9a0abfa6186327d43c51259d5b524fdeRequest | Submit search query

    try:
        # Search@publications
        api_response = api_instance.call_9a0abfa6186327d43c51259d5b524fde(model9a0abfa6186327d43c51259d5b524fde_request)
        print("The response of SearchPublicationsApi->call_9a0abfa6186327d43c51259d5b524fde:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchPublicationsApi->call_9a0abfa6186327d43c51259d5b524fde: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model9a0abfa6186327d43c51259d5b524fde_request** | [**Model9a0abfa6186327d43c51259d5b524fdeRequest**](Model9a0abfa6186327d43c51259d5b524fdeRequest.md)| Submit search query | 

### Return type

[**Model9a0abfa6186327d43c51259d5b524fde200Response**](Model9a0abfa6186327d43c51259d5b524fde200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**204** | No match found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

