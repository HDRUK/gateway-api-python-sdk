# UpdateWidgetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**widget_name** | **str** |  | [optional] 
**size_width** | **int** |  | [optional] 
**size_height** | **int** |  | [optional] 
**unit** | **str** |  | [optional] 
**include_search_bar** | **bool** |  | [optional] 
**include_cohort_link** | **bool** |  | [optional] 
**keep_proportions** | **bool** |  | [optional] 
**permitted_domains** | **List[str]** |  | [optional] 
**included_datasets** | **List[int]** |  | [optional] 
**included_data_uses** | **List[int]** |  | [optional] 
**data_custodian_entities_ids** | **List[int]** |  | [optional] 
**included_scripts** | **List[int]** |  | [optional] 
**included_collections** | **List[int]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_widget_request import UpdateWidgetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateWidgetRequest from a JSON string
update_widget_request_instance = UpdateWidgetRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateWidgetRequest.to_json())

# convert the object into a dict
update_widget_request_dict = update_widget_request_instance.to_dict()
# create an instance of UpdateWidgetRequest from a dict
update_widget_request_from_dict = UpdateWidgetRequest.from_dict(update_widget_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


