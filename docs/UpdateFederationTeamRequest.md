# UpdateFederationTeamRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**federation_type** | **str** |  | [optional] 
**auth_type** | **str** |  | [optional] 
**auth_secret_key** | **str** |  | [optional] 
**endpoint_baseurl** | **str** |  | [optional] 
**endpoint_datasets** | **str** |  | [optional] 
**endpoint_dataset** | **str** |  | [optional] 
**run_time_hour** | **int** |  | [optional] 
**run_time_minute** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**notifications** | **List[List[object]]** |  | [optional] 
**tested** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_federation_team_request import UpdateFederationTeamRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateFederationTeamRequest from a JSON string
update_federation_team_request_instance = UpdateFederationTeamRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateFederationTeamRequest.to_json())

# convert the object into a dict
update_federation_team_request_dict = update_federation_team_request_instance.to_dict()
# create an instance of UpdateFederationTeamRequest from a dict
update_federation_team_request_from_dict = UpdateFederationTeamRequest.from_dict(update_federation_team_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


