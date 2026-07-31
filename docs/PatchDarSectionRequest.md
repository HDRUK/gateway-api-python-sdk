# PatchDarSectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**parent_section** | **int** |  | [optional] 
**order** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.patch_dar_section_request import PatchDarSectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PatchDarSectionRequest from a JSON string
patch_dar_section_request_instance = PatchDarSectionRequest.from_json(json)
# print the JSON string representation of the object
print(PatchDarSectionRequest.to_json())

# convert the object into a dict
patch_dar_section_request_dict = patch_dar_section_request_instance.to_dict()
# create an instance of PatchDarSectionRequest from a dict
patch_dar_section_request_from_dict = PatchDarSectionRequest.from_dict(patch_dar_section_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


