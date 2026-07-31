# CreateTeamCollectionsRequestDatasetsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**reason** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_team_collections_request_datasets_inner import CreateTeamCollectionsRequestDatasetsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateTeamCollectionsRequestDatasetsInner from a JSON string
create_team_collections_request_datasets_inner_instance = CreateTeamCollectionsRequestDatasetsInner.from_json(json)
# print the JSON string representation of the object
print(CreateTeamCollectionsRequestDatasetsInner.to_json())

# convert the object into a dict
create_team_collections_request_datasets_inner_dict = create_team_collections_request_datasets_inner_instance.to_dict()
# create an instance of CreateTeamCollectionsRequestDatasetsInner from a dict
create_team_collections_request_datasets_inner_from_dict = CreateTeamCollectionsRequestDatasetsInner.from_dict(create_team_collections_request_datasets_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


