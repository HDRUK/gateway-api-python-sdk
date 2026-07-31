# Model3c8adeb001330f5198ca1072be78e299Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**image_link** | **str** |  | 
**description** | **str** |  | 
**team_id** | **int** |  | 
**user_id** | **int** |  | 
**enabled** | **bool** |  | 
**permissions** | **List[object]** |  | 
**notifications** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.model3c8adeb001330f5198ca1072be78e299_request import Model3c8adeb001330f5198ca1072be78e299Request

# TODO update the JSON string below
json = "{}"
# create an instance of Model3c8adeb001330f5198ca1072be78e299Request from a JSON string
model3c8adeb001330f5198ca1072be78e299_request_instance = Model3c8adeb001330f5198ca1072be78e299Request.from_json(json)
# print the JSON string representation of the object
print(Model3c8adeb001330f5198ca1072be78e299Request.to_json())

# convert the object into a dict
model3c8adeb001330f5198ca1072be78e299_request_dict = model3c8adeb001330f5198ca1072be78e299_request_instance.to_dict()
# create an instance of Model3c8adeb001330f5198ca1072be78e299Request from a dict
model3c8adeb001330f5198ca1072be78e299_request_from_dict = Model3c8adeb001330f5198ca1072be78e299Request.from_dict(model3c8adeb001330f5198ca1072be78e299_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


