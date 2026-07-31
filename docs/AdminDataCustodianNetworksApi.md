# gateway_api_sdk.AdminDataCustodianNetworksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fetch_admin_data_custodian_networks**](AdminDataCustodianNetworksApi.md#fetch_admin_data_custodian_networks) | **GET** /api/v2/admin/data_custodian_networks | DataCustodianNetworks@adminIndex


# **fetch_admin_data_custodian_networks**
> fetch_admin_data_custodian_networks(per_page=per_page)

DataCustodianNetworks@adminIndex

Superadmin-only listing used by the network management admin screen — unlike index(), this is not filtered to enabled=1, so disabled networks remain visible/manageable.

### Example


```python
import gateway_api_sdk
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
    api_instance = gateway_api_sdk.AdminDataCustodianNetworksApi(api_client)
    per_page = 1 # int | per page (optional)

    try:
        # DataCustodianNetworks@adminIndex
        api_instance.fetch_admin_data_custodian_networks(per_page=per_page)
    except Exception as e:
        print("Exception when calling AdminDataCustodianNetworksApi->fetch_admin_data_custodian_networks: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **per_page** | **int**| per page | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

