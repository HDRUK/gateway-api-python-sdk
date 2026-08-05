# EditProgrammingLanguagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**enabled** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_programming_languages_request import EditProgrammingLanguagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditProgrammingLanguagesRequest from a JSON string
edit_programming_languages_request_instance = EditProgrammingLanguagesRequest.from_json(json)
# print the JSON string representation of the object
print(EditProgrammingLanguagesRequest.to_json())

# convert the object into a dict
edit_programming_languages_request_dict = edit_programming_languages_request_instance.to_dict()
# create an instance of EditProgrammingLanguagesRequest from a dict
edit_programming_languages_request_from_dict = EditProgrammingLanguagesRequest.from_dict(edit_programming_languages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


