# CreateCollectionsIntegrationsRequest


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
**public** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_collections_integrations_request import CreateCollectionsIntegrationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateCollectionsIntegrationsRequest from a JSON string
create_collections_integrations_request_instance = CreateCollectionsIntegrationsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateCollectionsIntegrationsRequest.to_json())

# convert the object into a dict
create_collections_integrations_request_dict = create_collections_integrations_request_instance.to_dict()
# create an instance of CreateCollectionsIntegrationsRequest from a dict
create_collections_integrations_request_from_dict = CreateCollectionsIntegrationsRequest.from_dict(create_collections_integrations_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


