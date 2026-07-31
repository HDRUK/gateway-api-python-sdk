# TypeCategory

A category used to classify tool types

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.type_category import TypeCategory

# TODO update the JSON string below
json = "{}"
# create an instance of TypeCategory from a JSON string
type_category_instance = TypeCategory.from_json(json)
# print the JSON string representation of the object
print(TypeCategory.to_json())

# convert the object into a dict
type_category_dict = type_category_instance.to_dict()
# create an instance of TypeCategory from a dict
type_category_from_dict = TypeCategory.from_dict(type_category_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


