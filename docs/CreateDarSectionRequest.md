# CreateDarSectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**description** | **str** |  | 
**parent_section** | **int** |  | [optional] 
**order** | **int** |  | 

## Example

```python
from gateway_api_sdk.models.create_dar_section_request import CreateDarSectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDarSectionRequest from a JSON string
create_dar_section_request_instance = CreateDarSectionRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDarSectionRequest.to_json())

# convert the object into a dict
create_dar_section_request_dict = create_dar_section_request_instance.to_dict()
# create an instance of CreateDarSectionRequest from a dict
create_dar_section_request_from_dict = CreateDarSectionRequest.from_dict(create_dar_section_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


