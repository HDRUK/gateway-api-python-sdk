# gateway_api_sdk.DataAccessTemplatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dar_template_count_unique_fields**](DataAccessTemplatesApi.md#dar_template_count_unique_fields) | **GET** /api/v1/dar/templates/count/{field} | DataAccessTemplateController@count


# **dar_template_count_unique_fields**
> CountUniqueFieldsCollections200Response dar_template_count_unique_fields(var_field)

DataAccessTemplateController@count

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
    api_instance = gateway_api_sdk.DataAccessTemplatesApi(api_client)
    var_field = 'published' # str | name of the field to perform a count on

    try:
        # DataAccessTemplateController@count
        api_response = api_instance.dar_template_count_unique_fields(var_field)
        print("The response of DataAccessTemplatesApi->dar_template_count_unique_fields:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DataAccessTemplatesApi->dar_template_count_unique_fields: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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

