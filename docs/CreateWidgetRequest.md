# CreateWidgetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**widget_name** | **str** |  | 
**size_width** | **int** |  | [optional] 
**size_height** | **int** |  | [optional] 
**unit** | **str** |  | [optional] 
**include_search_bar** | **bool** |  | [optional] 
**include_cohort_link** | **bool** |  | [optional] 
**keep_proportions** | **bool** |  | [optional] 
**permitted_domains** | **List[str]** |  | [optional] 
**included_datasets** | **List[int]** |  | [optional] 
**included_data_uses** | **List[int]** |  | [optional] 
**included_scripts** | **List[int]** |  | [optional] 
**included_collections** | **List[int]** |  | [optional] 
**data_custodian_entities_ids** | **List[int]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_widget_request import CreateWidgetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateWidgetRequest from a JSON string
create_widget_request_instance = CreateWidgetRequest.from_json(json)
# print the JSON string representation of the object
print(CreateWidgetRequest.to_json())

# convert the object into a dict
create_widget_request_dict = create_widget_request_instance.to_dict()
# create an instance of CreateWidgetRequest from a dict
create_widget_request_from_dict = CreateWidgetRequest.from_dict(create_widget_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


