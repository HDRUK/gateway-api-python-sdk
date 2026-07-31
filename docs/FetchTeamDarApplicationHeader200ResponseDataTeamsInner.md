# FetchTeamDarApplicationHeader200ResponseDataTeamsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_id** | **int** |  | [optional] 
**dar_application_id** | **int** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**approval_status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_dar_application_header200_response_data_teams_inner import FetchTeamDarApplicationHeader200ResponseDataTeamsInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamDarApplicationHeader200ResponseDataTeamsInner from a JSON string
fetch_team_dar_application_header200_response_data_teams_inner_instance = FetchTeamDarApplicationHeader200ResponseDataTeamsInner.from_json(json)
# print the JSON string representation of the object
print(FetchTeamDarApplicationHeader200ResponseDataTeamsInner.to_json())

# convert the object into a dict
fetch_team_dar_application_header200_response_data_teams_inner_dict = fetch_team_dar_application_header200_response_data_teams_inner_instance.to_dict()
# create an instance of FetchTeamDarApplicationHeader200ResponseDataTeamsInner from a dict
fetch_team_dar_application_header200_response_data_teams_inner_from_dict = FetchTeamDarApplicationHeader200ResponseDataTeamsInner.from_dict(fetch_team_dar_application_header200_response_data_teams_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


