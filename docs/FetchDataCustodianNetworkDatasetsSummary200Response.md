# FetchDataCustodianNetworkDatasetsSummary200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchDataCustodianNetworkDatasetsSummary200ResponseData**](FetchDataCustodianNetworkDatasetsSummary200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_data_custodian_network_datasets_summary200_response import FetchDataCustodianNetworkDatasetsSummary200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDataCustodianNetworkDatasetsSummary200Response from a JSON string
fetch_data_custodian_network_datasets_summary200_response_instance = FetchDataCustodianNetworkDatasetsSummary200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDataCustodianNetworkDatasetsSummary200Response.to_json())

# convert the object into a dict
fetch_data_custodian_network_datasets_summary200_response_dict = fetch_data_custodian_network_datasets_summary200_response_instance.to_dict()
# create an instance of FetchDataCustodianNetworkDatasetsSummary200Response from a dict
fetch_data_custodian_network_datasets_summary200_response_from_dict = FetchDataCustodianNetworkDatasetsSummary200Response.from_dict(fetch_data_custodian_network_datasets_summary200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


