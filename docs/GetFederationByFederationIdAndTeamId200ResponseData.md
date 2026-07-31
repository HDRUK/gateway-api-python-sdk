# GetFederationByFederationIdAndTeamId200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**federation_type** | **str** |  | [optional] 
**auth_type** | **str** |  | [optional] 
**auth_secret_key** | **str** |  | [optional] 
**endpoint_baseurl** | **str** |  | [optional] 
**endpoint_datasets** | **str** |  | [optional] 
**endpoint_dataset** | **str** |  | [optional] 
**run_time_hour** | **int** |  | [optional] 
**run_time_minute** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**counter** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**tested** | **bool** |  | [optional] 
**notifications** | **List[object]** |  | [optional] 
**is_running** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_federation_by_federation_id_and_team_id200_response_data import GetFederationByFederationIdAndTeamId200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of GetFederationByFederationIdAndTeamId200ResponseData from a JSON string
get_federation_by_federation_id_and_team_id200_response_data_instance = GetFederationByFederationIdAndTeamId200ResponseData.from_json(json)
# print the JSON string representation of the object
print(GetFederationByFederationIdAndTeamId200ResponseData.to_json())

# convert the object into a dict
get_federation_by_federation_id_and_team_id200_response_data_dict = get_federation_by_federation_id_and_team_id200_response_data_instance.to_dict()
# create an instance of GetFederationByFederationIdAndTeamId200ResponseData from a dict
get_federation_by_federation_id_and_team_id200_response_data_from_dict = GetFederationByFederationIdAndTeamId200ResponseData.from_dict(get_federation_by_federation_id_and_team_id200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


