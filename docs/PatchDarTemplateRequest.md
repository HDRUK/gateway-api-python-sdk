# PatchDarTemplateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicant_id** | **int** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**approval_status** | **str** |  | [optional] 
**team_id** | **List[object]** |  | [optional] 
**questions** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.patch_dar_template_request import PatchDarTemplateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PatchDarTemplateRequest from a JSON string
patch_dar_template_request_instance = PatchDarTemplateRequest.from_json(json)
# print the JSON string representation of the object
print(PatchDarTemplateRequest.to_json())

# convert the object into a dict
patch_dar_template_request_dict = patch_dar_template_request_instance.to_dict()
# create an instance of PatchDarTemplateRequest from a dict
patch_dar_template_request_from_dict = PatchDarTemplateRequest.from_dict(patch_dar_template_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


