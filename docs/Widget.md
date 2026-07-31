# Widget

A widget record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**team_id** | **int** |  | [optional] 
**data_custodian_entities_ids** | **str** |  | [optional] 
**included_datasets** | **str** |  | [optional] 
**included_data_uses** | **str** |  | [optional] 
**included_scripts** | **str** |  | [optional] 
**included_collections** | **str** |  | [optional] 
**include_search_bar** | **bool** |  | [optional] 
**include_cohort_link** | **bool** |  | [optional] 
**size_width** | **int** |  | [optional] 
**size_height** | **int** |  | [optional] 
**unit** | **str** |  | [optional] 
**keep_proportions** | **bool** |  | [optional] 
**widget_name** | **str** |  | [optional] 
**permitted_domains** | **str** |  | [optional] 
**branding_primary** | **str** |  | [optional] 
**branding_secondary** | **str** |  | [optional] 
**branding_neutral** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.widget import Widget

# TODO update the JSON string below
json = "{}"
# create an instance of Widget from a JSON string
widget_instance = Widget.from_json(json)
# print the JSON string representation of the object
print(Widget.to_json())

# convert the object into a dict
widget_dict = widget_instance.to_dict()
# create an instance of Widget from a dict
widget_from_dict = Widget.from_dict(widget_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


