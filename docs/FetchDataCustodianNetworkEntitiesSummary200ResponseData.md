# FetchDataCustodianNetworkEntitiesSummary200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**durs_total** | **int** |  | [optional] 
**durs** | **List[object]** |  | [optional] 
**tools_total** | **int** |  | [optional] 
**tools** | **List[object]** |  | [optional] 
**publications_total** | **int** |  | [optional] 
**publications** | **List[object]** |  | [optional] 
**collections_total** | **int** |  | [optional] 
**collections** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_data_custodian_network_entities_summary200_response_data import FetchDataCustodianNetworkEntitiesSummary200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDataCustodianNetworkEntitiesSummary200ResponseData from a JSON string
fetch_data_custodian_network_entities_summary200_response_data_instance = FetchDataCustodianNetworkEntitiesSummary200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchDataCustodianNetworkEntitiesSummary200ResponseData.to_json())

# convert the object into a dict
fetch_data_custodian_network_entities_summary200_response_data_dict = fetch_data_custodian_network_entities_summary200_response_data_instance.to_dict()
# create an instance of FetchDataCustodianNetworkEntitiesSummary200ResponseData from a dict
fetch_data_custodian_network_entities_summary200_response_data_from_dict = FetchDataCustodianNetworkEntitiesSummary200ResponseData.from_dict(fetch_data_custodian_network_entities_summary200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


