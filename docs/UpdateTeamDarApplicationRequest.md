# UpdateTeamDarApplicationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**submission_status** | **str** |  | [optional] 
**approval_status** | **str** |  | [optional] 
**comment** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_team_dar_application_request import UpdateTeamDarApplicationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateTeamDarApplicationRequest from a JSON string
update_team_dar_application_request_instance = UpdateTeamDarApplicationRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateTeamDarApplicationRequest.to_json())

# convert the object into a dict
update_team_dar_application_request_dict = update_team_dar_application_request_instance.to_dict()
# create an instance of UpdateTeamDarApplicationRequest from a dict
update_team_dar_application_request_from_dict = UpdateTeamDarApplicationRequest.from_dict(update_team_dar_application_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


