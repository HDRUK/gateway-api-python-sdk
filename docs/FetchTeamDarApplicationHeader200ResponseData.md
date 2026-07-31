# FetchTeamDarApplicationHeader200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**applicant_id** | **int** |  | [optional] 
**project_title** | **str** |  | [optional] 
**application_type** | **str** |  | [optional] 
**project_id** | **int** |  | [optional] 
**is_joint** | **bool** |  | [optional] 
**approval_status** | **str** |  | [optional] 
**submission_status** | **str** |  | [optional] 
**status_review_id** | **int** |  | [optional] 
**days_since_submission** | **int** |  | [optional] 
**primary_applicant** | [**List[FetchTeamDarApplicationHeader200ResponseDataPrimaryApplicantInner]**](FetchTeamDarApplicationHeader200ResponseDataPrimaryApplicantInner.md) |  | [optional] 
**datasets** | [**List[FetchTeamDarApplicationHeader200ResponseDataDatasetsInner]**](FetchTeamDarApplicationHeader200ResponseDataDatasetsInner.md) |  | [optional] 
**teams** | [**List[FetchTeamDarApplicationHeader200ResponseDataTeamsInner]**](FetchTeamDarApplicationHeader200ResponseDataTeamsInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_dar_application_header200_response_data import FetchTeamDarApplicationHeader200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamDarApplicationHeader200ResponseData from a JSON string
fetch_team_dar_application_header200_response_data_instance = FetchTeamDarApplicationHeader200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchTeamDarApplicationHeader200ResponseData.to_json())

# convert the object into a dict
fetch_team_dar_application_header200_response_data_dict = fetch_team_dar_application_header200_response_data_instance.to_dict()
# create an instance of FetchTeamDarApplicationHeader200ResponseData from a dict
fetch_team_dar_application_header200_response_data_from_dict = FetchTeamDarApplicationHeader200ResponseData.from_dict(fetch_team_dar_application_header200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


