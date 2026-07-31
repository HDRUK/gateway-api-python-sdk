# Model928c1c4e39f13593bdec88641ee83120200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**filename** | **str** |  | [optional] 
**file_location** | **str** |  | [optional] 
**user_id** | **str** |  | [optional] 
**status** | **str** |  | [optional] 
**application_id** | **int** |  | [optional] 
**question_id** | **int** |  | [optional] 
**error** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.model928c1c4e39f13593bdec88641ee83120200_response_data import Model928c1c4e39f13593bdec88641ee83120200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of Model928c1c4e39f13593bdec88641ee83120200ResponseData from a JSON string
model928c1c4e39f13593bdec88641ee83120200_response_data_instance = Model928c1c4e39f13593bdec88641ee83120200ResponseData.from_json(json)
# print the JSON string representation of the object
print(Model928c1c4e39f13593bdec88641ee83120200ResponseData.to_json())

# convert the object into a dict
model928c1c4e39f13593bdec88641ee83120200_response_data_dict = model928c1c4e39f13593bdec88641ee83120200_response_data_instance.to_dict()
# create an instance of Model928c1c4e39f13593bdec88641ee83120200ResponseData from a dict
model928c1c4e39f13593bdec88641ee83120200_response_data_from_dict = Model928c1c4e39f13593bdec88641ee83120200ResponseData.from_dict(model928c1c4e39f13593bdec88641ee83120200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


