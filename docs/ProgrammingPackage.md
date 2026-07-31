# ProgrammingPackage

A programming package/library available for tagging tools

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.programming_package import ProgrammingPackage

# TODO update the JSON string below
json = "{}"
# create an instance of ProgrammingPackage from a JSON string
programming_package_instance = ProgrammingPackage.from_json(json)
# print the JSON string representation of the object
print(ProgrammingPackage.to_json())

# convert the object into a dict
programming_package_dict = programming_package_instance.to_dict()
# create an instance of ProgrammingPackage from a dict
programming_package_from_dict = ProgrammingPackage.from_dict(programming_package_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


