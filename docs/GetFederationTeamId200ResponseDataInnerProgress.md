# GetFederationTeamId200ResponseDataInnerProgress

Only present while a sync is actively in progress

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** |  | [optional] 
**processed** | **int** |  | [optional] 
**failed** | **int** |  | [optional] 
**pending** | **int** |  | [optional] 
**started_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_federation_team_id200_response_data_inner_progress import GetFederationTeamId200ResponseDataInnerProgress

# TODO update the JSON string below
json = "{}"
# create an instance of GetFederationTeamId200ResponseDataInnerProgress from a JSON string
get_federation_team_id200_response_data_inner_progress_instance = GetFederationTeamId200ResponseDataInnerProgress.from_json(json)
# print the JSON string representation of the object
print(GetFederationTeamId200ResponseDataInnerProgress.to_json())

# convert the object into a dict
get_federation_team_id200_response_data_inner_progress_dict = get_federation_team_id200_response_data_inner_progress_instance.to_dict()
# create an instance of GetFederationTeamId200ResponseDataInnerProgress from a dict
get_federation_team_id200_response_data_inner_progress_from_dict = GetFederationTeamId200ResponseDataInnerProgress.from_dict(get_federation_team_id200_response_data_inner_progress_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


