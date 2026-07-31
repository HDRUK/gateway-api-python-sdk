# CreateFederationTeamRequest


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
**enabled** | **bool** |  | [optional] 
**notifications** | **List[List[object]]** |  | [optional] 
**tested** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_federation_team_request import CreateFederationTeamRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateFederationTeamRequest from a JSON string
create_federation_team_request_instance = CreateFederationTeamRequest.from_json(json)
# print the JSON string representation of the object
print(CreateFederationTeamRequest.to_json())

# convert the object into a dict
create_federation_team_request_dict = create_federation_team_request_instance.to_dict()
# create an instance of CreateFederationTeamRequest from a dict
create_federation_team_request_from_dict = CreateFederationTeamRequest.from_dict(create_federation_team_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


