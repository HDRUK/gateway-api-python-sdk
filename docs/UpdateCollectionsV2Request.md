# UpdateCollectionsV2Request


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
**collaborators** | **List[int]** |  | [optional] 
**public** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_collections_v2_request import UpdateCollectionsV2Request

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateCollectionsV2Request from a JSON string
update_collections_v2_request_instance = UpdateCollectionsV2Request.from_json(json)
# print the JSON string representation of the object
print(UpdateCollectionsV2Request.to_json())

# convert the object into a dict
update_collections_v2_request_dict = update_collections_v2_request_instance.to_dict()
# create an instance of UpdateCollectionsV2Request from a dict
update_collections_v2_request_from_dict = UpdateCollectionsV2Request.from_dict(update_collections_v2_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


