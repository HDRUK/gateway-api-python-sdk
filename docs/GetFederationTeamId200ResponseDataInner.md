# GetFederationTeamId200ResponseDataInner


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
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**tested** | **bool** |  | [optional] 
**is_running** | **bool** |  | [optional] 
**notifications** | **List[object]** |  | [optional] 
**last_run_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.get_federation_team_id200_response_data_inner import GetFederationTeamId200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetFederationTeamId200ResponseDataInner from a JSON string
get_federation_team_id200_response_data_inner_instance = GetFederationTeamId200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(GetFederationTeamId200ResponseDataInner.to_json())

# convert the object into a dict
get_federation_team_id200_response_data_inner_dict = get_federation_team_id200_response_data_inner_instance.to_dict()
# create an instance of GetFederationTeamId200ResponseDataInner from a dict
get_federation_team_id200_response_data_inner_from_dict = GetFederationTeamId200ResponseDataInner.from_dict(get_federation_team_id200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


