# EditTeamCollectionsRequest


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
**status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_team_collections_request import EditTeamCollectionsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditTeamCollectionsRequest from a JSON string
edit_team_collections_request_instance = EditTeamCollectionsRequest.from_json(json)
# print the JSON string representation of the object
print(EditTeamCollectionsRequest.to_json())

# convert the object into a dict
edit_team_collections_request_dict = edit_team_collections_request_instance.to_dict()
# create an instance of EditTeamCollectionsRequest from a dict
edit_team_collections_request_from_dict = EditTeamCollectionsRequest.from_dict(edit_team_collections_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


