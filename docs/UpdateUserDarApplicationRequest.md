# UpdateUserDarApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicant_id** | **int** |  | 
**submission_status** | **str** |  | 
**project_title** | **str** |  | [optional] 
**approval_status** | **str** |  | 
**team_ids** | **List[int]** |  | [optional] 
**answers** | [**List[UpdateUserDarApplicationRequestAnswersInner]**](UpdateUserDarApplicationRequestAnswersInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_user_dar_application_request import UpdateUserDarApplicationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateUserDarApplicationRequest from a JSON string
update_user_dar_application_request_instance = UpdateUserDarApplicationRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateUserDarApplicationRequest.to_json())

# convert the object into a dict
update_user_dar_application_request_dict = update_user_dar_application_request_instance.to_dict()
# create an instance of UpdateUserDarApplicationRequest from a dict
update_user_dar_application_request_from_dict = UpdateUserDarApplicationRequest.from_dict(update_user_dar_application_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


