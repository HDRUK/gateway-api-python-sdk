# UpdateTeamCollectionsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**datasets** | [**List[CreateTeamCollectionsRequestDatasetsInner]**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] 
**dur** | [**List[CreateTeamCollectionsRequestDatasetsInner]**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] 
**publications** | [**List[CreateTeamCollectionsRequestDatasetsInner]**](CreateTeamCollectionsRequestDatasetsInner.md) |  | [optional] 
**public** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_team_collections_request import UpdateTeamCollectionsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateTeamCollectionsRequest from a JSON string
update_team_collections_request_instance = UpdateTeamCollectionsRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateTeamCollectionsRequest.to_json())

# convert the object into a dict
update_team_collections_request_dict = update_team_collections_request_instance.to_dict()
# create an instance of UpdateTeamCollectionsRequest from a dict
update_team_collections_request_from_dict = UpdateTeamCollectionsRequest.from_dict(update_team_collections_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


