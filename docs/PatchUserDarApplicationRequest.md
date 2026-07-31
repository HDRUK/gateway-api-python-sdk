# PatchUserDarApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicant_id** | **int** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**project_title** | **str** |  | [optional] 
**approval_status** | **str** |  | [optional] 
**team_ids** | **List[int]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.patch_user_dar_application_request import PatchUserDarApplicationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PatchUserDarApplicationRequest from a JSON string
patch_user_dar_application_request_instance = PatchUserDarApplicationRequest.from_json(json)
# print the JSON string representation of the object
print(PatchUserDarApplicationRequest.to_json())

# convert the object into a dict
patch_user_dar_application_request_dict = patch_user_dar_application_request_instance.to_dict()
# create an instance of PatchUserDarApplicationRequest from a dict
patch_user_dar_application_request_from_dict = PatchUserDarApplicationRequest.from_dict(patch_user_dar_application_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


