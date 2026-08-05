# CreateProgrammingLanguagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**enabled** | **bool** |  | 

## Example

```python
from gateway_api_sdk.models.create_programming_languages_request import CreateProgrammingLanguagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateProgrammingLanguagesRequest from a JSON string
create_programming_languages_request_instance = CreateProgrammingLanguagesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateProgrammingLanguagesRequest.to_json())

# convert the object into a dict
create_programming_languages_request_dict = create_programming_languages_request_instance.to_dict()
# create an instance of CreateProgrammingLanguagesRequest from a dict
create_programming_languages_request_from_dict = CreateProgrammingLanguagesRequest.from_dict(create_programming_languages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


