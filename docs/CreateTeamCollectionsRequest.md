# CreateTeamCollectionsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**datasets** | [**List[CreateTeamCollectionsRequestDatasetsInner]**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] 
**tools** | [**List[CreateTeamCollectionsRequestDatasetsInner]**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] 
**dur** | [**List[CreateTeamCollectionsRequestDatasetsInner]**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] 
**publications** | [**List[CreateTeamCollectionsRequestDatasetsInner]**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] 
**public** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_team_collections_request import CreateTeamCollectionsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTeamCollectionsRequest from a JSON string
create_team_collections_request_instance = CreateTeamCollectionsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateTeamCollectionsRequest.to_json())

# convert the object into a dict
create_team_collections_request_dict = create_team_collections_request_instance.to_dict()
# create an instance of CreateTeamCollectionsRequest from a dict
create_team_collections_request_from_dict = CreateTeamCollectionsRequest.from_dict(create_team_collections_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


