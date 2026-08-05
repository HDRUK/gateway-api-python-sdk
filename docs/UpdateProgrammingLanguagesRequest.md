# UpdateProgrammingLanguagesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**enabled** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.update_programming_languages_request import UpdateProgrammingLanguagesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateProgrammingLanguagesRequest from a JSON string
update_programming_languages_request_instance = UpdateProgrammingLanguagesRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateProgrammingLanguagesRequest.to_json())

# convert the object into a dict
update_programming_languages_request_dict = update_programming_languages_request_instance.to_dict()
# create an instance of UpdateProgrammingLanguagesRequest from a dict
update_programming_languages_request_from_dict = UpdateProgrammingLanguagesRequest.from_dict(update_programming_languages_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


