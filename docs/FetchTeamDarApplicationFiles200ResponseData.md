# FetchTeamDarApplicationFiles200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**filename** | **str** |  | [optional] 
**file_location** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**application_id** | **int** |  | [optional] 
**question_id** | **int** |  | [optional] 
**error** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_team_dar_application_files200_response_data import FetchTeamDarApplicationFiles200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchTeamDarApplicationFiles200ResponseData from a JSON string
fetch_team_dar_application_files200_response_data_instance = FetchTeamDarApplicationFiles200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchTeamDarApplicationFiles200ResponseData.to_json())

# convert the object into a dict
fetch_team_dar_application_files200_response_data_dict = fetch_team_dar_application_files200_response_data_instance.to_dict()
# create an instance of FetchTeamDarApplicationFiles200ResponseData from a dict
fetch_team_dar_application_files200_response_data_from_dict = FetchTeamDarApplicationFiles200ResponseData.from_dict(fetch_team_dar_application_files200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


