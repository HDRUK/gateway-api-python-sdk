# ProgrammingLanguage

A programming language available for tagging tools

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
from gateway_api_sdk.models.programming_language import ProgrammingLanguage

# TODO update the JSON string below
json = "{}"
# create an instance of ProgrammingLanguage from a JSON string
programming_language_instance = ProgrammingLanguage.from_json(json)
# print the JSON string representation of the object
print(ProgrammingLanguage.to_json())

# convert the object into a dict
programming_language_dict = programming_language_instance.to_dict()
# create an instance of ProgrammingLanguage from a dict
programming_language_from_dict = ProgrammingLanguage.from_dict(programming_language_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


