# SearchDataCustodianNetworks200ResponseDataInnerSourceInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**img_url** | **str** |  | [optional] 
**dataset_titles** | **List[object]** |  | [optional] 
**geographic_location** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_data_custodian_networks200_response_data_inner_source_inner import SearchDataCustodianNetworks200ResponseDataInnerSourceInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataCustodianNetworks200ResponseDataInnerSourceInner from a JSON string
search_data_custodian_networks200_response_data_inner_source_inner_instance = SearchDataCustodianNetworks200ResponseDataInnerSourceInner.from_json(json)
# print the JSON string representation of the object
print(SearchDataCustodianNetworks200ResponseDataInnerSourceInner.to_json())

# convert the object into a dict
search_data_custodian_networks200_response_data_inner_source_inner_dict = search_data_custodian_networks200_response_data_inner_source_inner_instance.to_dict()
# create an instance of SearchDataCustodianNetworks200ResponseDataInnerSourceInner from a dict
search_data_custodian_networks200_response_data_inner_source_inner_from_dict = SearchDataCustodianNetworks200ResponseDataInnerSourceInner.from_dict(search_data_custodian_networks200_response_data_inner_source_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


