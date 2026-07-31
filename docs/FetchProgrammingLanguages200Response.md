# FetchProgrammingLanguages200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ProgrammingLanguage**](ProgrammingLanguage.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_programming_languages200_response import FetchProgrammingLanguages200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchProgrammingLanguages200Response from a JSON string
fetch_programming_languages200_response_instance = FetchProgrammingLanguages200Response.from_json(json)
# print the JSON string representation of the object
print(FetchProgrammingLanguages200Response.to_json())

# convert the object into a dict
fetch_programming_languages200_response_dict = fetch_programming_languages200_response_instance.to_dict()
# create an instance of FetchProgrammingLanguages200Response from a dict
fetch_programming_languages200_response_from_dict = FetchProgrammingLanguages200Response.from_dict(fetch_programming_languages200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


