# SearchDataUses200ResponseDataInnerSourceInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_title** | **str** |  | [optional] 
**lay_summary** | **str** |  | [optional] 
**public_benefit_statement** | **str** |  | [optional] 
**technical_summary** | **str** |  | [optional] 
**funders_and_sponsors** | **str** |  | [optional] 
**dataset_titles** | **List[object]** |  | [optional] 
**keywords** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_data_uses200_response_data_inner_source_inner import SearchDataUses200ResponseDataInnerSourceInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataUses200ResponseDataInnerSourceInner from a JSON string
search_data_uses200_response_data_inner_source_inner_instance = SearchDataUses200ResponseDataInnerSourceInner.from_json(json)
# print the JSON string representation of the object
print(SearchDataUses200ResponseDataInnerSourceInner.to_json())

# convert the object into a dict
search_data_uses200_response_data_inner_source_inner_dict = search_data_uses200_response_data_inner_source_inner_instance.to_dict()
# create an instance of SearchDataUses200ResponseDataInnerSourceInner from a dict
search_data_uses200_response_data_inner_source_inner_from_dict = SearchDataUses200ResponseDataInnerSourceInner.from_dict(search_data_uses200_response_data_inner_source_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


