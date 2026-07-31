# gateway_api_sdk.SearchPublicationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**search_publications**](SearchPublicationsApi.md#search_publications) | **POST** /api/v1/search/publications | Search@publications
[**search_publications_by_doi**](SearchPublicationsApi.md#search_publications_by_doi) | **POST** /api/v1/search/doi | Search@publications


# **search_publications**
> SearchPublications200Response search_publications(search_publications_request, sort=sort, direction=direction, source=source)

Search@publications

Returns gateway publications related to the provided query term(s)

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.search_publications200_response import SearchPublications200Response
from gateway_api_sdk.models.search_publications_request import SearchPublicationsRequest
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
    search_publications_request = gateway_api_sdk.SearchPublicationsRequest() # SearchPublicationsRequest | Submit search query
    sort = 'created' # str | Field to sort by (default: 'score') (optional)
    direction = 'desc' # str | Sort direction ('asc' or 'desc', default: 'desc') (optional)
    source = 'GAT' # str | Which source to search ('GAT' or 'FED', default: 'GAT') (optional)

    try:
        # Search@publications
        api_response = api_instance.search_publications(search_publications_request, sort=sort, direction=direction, source=source)
        print("The response of SearchPublicationsApi->search_publications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchPublicationsApi->search_publications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_publications_request** | [**SearchPublicationsRequest**](SearchPublicationsRequest.md)| Submit search query | 
 **sort** | **str**| Field to sort by (default: &#39;score&#39;) | [optional] 
 **direction** | **str**| Sort direction (&#39;asc&#39; or &#39;desc&#39;, default: &#39;desc&#39;) | [optional] 
 **source** | **str**| Which source to search (&#39;GAT&#39; or &#39;FED&#39;, default: &#39;GAT&#39;) | [optional] 

### Return type

[**SearchPublications200Response**](SearchPublications200Response.md)

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

# **search_publications_by_doi**
> SearchPublicationsByDoi200Response search_publications_by_doi(search_publications_by_doi_request)

Search@publications

Returns publications from EuropePMC matching a give DOI

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import gateway_api_sdk
from gateway_api_sdk.models.search_publications_by_doi200_response import SearchPublicationsByDoi200Response
from gateway_api_sdk.models.search_publications_by_doi_request import SearchPublicationsByDoiRequest
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
    search_publications_by_doi_request = gateway_api_sdk.SearchPublicationsByDoiRequest() # SearchPublicationsByDoiRequest | Submit search query

    try:
        # Search@publications
        api_response = api_instance.search_publications_by_doi(search_publications_by_doi_request)
        print("The response of SearchPublicationsApi->search_publications_by_doi:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SearchPublicationsApi->search_publications_by_doi: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search_publications_by_doi_request** | [**SearchPublicationsByDoiRequest**](SearchPublicationsByDoiRequest.md)| Submit search query | 

### Return type

[**SearchPublicationsByDoi200Response**](SearchPublicationsByDoi200Response.md)

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

