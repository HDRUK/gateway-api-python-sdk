# Tool

A software tool or model associated with datasets in the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**results_insights** | **str** |  | [optional] 
**license** | **int** | Foreign key to licenses table | [optional] 
**tech_stack** | **str** |  | [optional] 
**category_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**associated_authors** | **str** |  | [optional] 
**contact_address** | **str** |  | [optional] 
**any_dataset** | **bool** |  | [optional] 
**status** | **str** |  | [optional] 
**team_id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.tool import Tool

# TODO update the JSON string below
json = "{}"
# create an instance of Tool from a JSON string
tool_instance = Tool.from_json(json)
# print the JSON string representation of the object
print(Tool.to_json())

# convert the object into a dict
tool_dict = tool_instance.to_dict()
# create an instance of Tool from a dict
tool_from_dict = Tool.from_dict(tool_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


