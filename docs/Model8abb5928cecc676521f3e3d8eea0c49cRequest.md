# Model8abb5928cecc676521f3e3d8eea0c49cRequest


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
from gateway_api_sdk.models.model8abb5928cecc676521f3e3d8eea0c49c_request import Model8abb5928cecc676521f3e3d8eea0c49cRequest

# TODO update the JSON string below
json = "{}"
# create an instance of Model8abb5928cecc676521f3e3d8eea0c49cRequest from a JSON string
model8abb5928cecc676521f3e3d8eea0c49c_request_instance = Model8abb5928cecc676521f3e3d8eea0c49cRequest.from_json(json)
# print the JSON string representation of the object
print(Model8abb5928cecc676521f3e3d8eea0c49cRequest.to_json())

# convert the object into a dict
model8abb5928cecc676521f3e3d8eea0c49c_request_dict = model8abb5928cecc676521f3e3d8eea0c49c_request_instance.to_dict()
# create an instance of Model8abb5928cecc676521f3e3d8eea0c49cRequest from a dict
model8abb5928cecc676521f3e3d8eea0c49c_request_from_dict = Model8abb5928cecc676521f3e3d8eea0c49cRequest.from_dict(model8abb5928cecc676521f3e3d8eea0c49c_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


