# FetchDataCustodianNetworkDatasetsSummary200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**datasets** | **List[object]** |  | [optional] 
**datasets_total** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_data_custodian_network_datasets_summary200_response_data import FetchDataCustodianNetworkDatasetsSummary200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDataCustodianNetworkDatasetsSummary200ResponseData from a JSON string
fetch_data_custodian_network_datasets_summary200_response_data_instance = FetchDataCustodianNetworkDatasetsSummary200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchDataCustodianNetworkDatasetsSummary200ResponseData.to_json())

# convert the object into a dict
fetch_data_custodian_network_datasets_summary200_response_data_dict = fetch_data_custodian_network_datasets_summary200_response_data_instance.to_dict()
# create an instance of FetchDataCustodianNetworkDatasetsSummary200ResponseData from a dict
fetch_data_custodian_network_datasets_summary200_response_data_from_dict = FetchDataCustodianNetworkDatasetsSummary200ResponseData.from_dict(fetch_data_custodian_network_datasets_summary200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


