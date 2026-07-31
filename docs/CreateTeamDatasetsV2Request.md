# CreateTeamDatasetsV2Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**create_origin** | **str** |  | [optional] 
**mongo_object_id** | **str** |  | [optional] 
**mongo_id** | **str** |  | [optional] 
**mongo_pid** | **str** |  | [optional] 
**metadata** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_team_datasets_v2_request import CreateTeamDatasetsV2Request

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTeamDatasetsV2Request from a JSON string
create_team_datasets_v2_request_instance = CreateTeamDatasetsV2Request.from_json(json)
# print the JSON string representation of the object
print(CreateTeamDatasetsV2Request.to_json())

# convert the object into a dict
create_team_datasets_v2_request_dict = create_team_datasets_v2_request_instance.to_dict()
# create an instance of CreateTeamDatasetsV2Request from a dict
create_team_datasets_v2_request_from_dict = CreateTeamDatasetsV2Request.from_dict(create_team_datasets_v2_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


