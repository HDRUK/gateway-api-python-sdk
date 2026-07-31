# E210052adcf6fdcfc472998b430081aa200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**app_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**client_secret** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**team_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**permissions** | **List[object]** |  | [optional] 
**team** | **List[object]** |  | [optional] 
**user** | **List[object]** |  | [optional] 
**notifications** | **List[object]** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.e210052adcf6fdcfc472998b430081aa200_response_data_inner import E210052adcf6fdcfc472998b430081aa200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of E210052adcf6fdcfc472998b430081aa200ResponseDataInner from a JSON string
e210052adcf6fdcfc472998b430081aa200_response_data_inner_instance = E210052adcf6fdcfc472998b430081aa200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(E210052adcf6fdcfc472998b430081aa200ResponseDataInner.to_json())

# convert the object into a dict
e210052adcf6fdcfc472998b430081aa200_response_data_inner_dict = e210052adcf6fdcfc472998b430081aa200_response_data_inner_instance.to_dict()
# create an instance of E210052adcf6fdcfc472998b430081aa200ResponseDataInner from a dict
e210052adcf6fdcfc472998b430081aa200_response_data_inner_from_dict = E210052adcf6fdcfc472998b430081aa200ResponseDataInner.from_dict(e210052adcf6fdcfc472998b430081aa200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


