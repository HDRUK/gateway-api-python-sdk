# EditCollectionsV2Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**keywords** | **List[str]** |  | [optional] 
**datasets** | [**List[CreateCollectionsIntegrationsRequestDatasetsInner]**](CreateCollectionsIntegrationsRequestDatasetsInner.md) |  | [optional] 
**dur** | [**List[CreateCollectionsIntegrationsRequestDatasetsInner]**](CreateCollectionsIntegrationsRequestDatasetsInner.md) |  | [optional] 
**publications** | [**List[CreateCollectionsIntegrationsRequestDatasetsInner]**](CreateCollectionsIntegrationsRequestDatasetsInner.md) |  | [optional] 
**collaborators** | **List[int]** |  | [optional] 
**public** | **bool** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_collections_v2_request import EditCollectionsV2Request

# TODO update the JSON string below
json = "{}"
# create an instance of EditCollectionsV2Request from a JSON string
edit_collections_v2_request_instance = EditCollectionsV2Request.from_json(json)
# print the JSON string representation of the object
print(EditCollectionsV2Request.to_json())

# convert the object into a dict
edit_collections_v2_request_dict = edit_collections_v2_request_instance.to_dict()
# create an instance of EditCollectionsV2Request from a dict
edit_collections_v2_request_from_dict = EditCollectionsV2Request.from_dict(edit_collections_v2_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


