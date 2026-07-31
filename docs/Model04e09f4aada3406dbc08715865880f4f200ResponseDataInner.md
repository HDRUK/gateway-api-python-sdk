# Model04e09f4aada3406dbc08715865880f4f200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**section_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**locked** | **bool** |  | [optional] 
**archived** | **bool** |  | [optional] 
**archived_date** | **datetime** |  | [optional] 
**force_required** | **bool** |  | [optional] 
**allow_guidance_override** | **bool** |  | [optional] 
**is_child** | **bool** |  | [optional] 
**question_type** | **str** |  | [optional] 
**latest_version** | **object** |  | [optional] 
**versions** | **object** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.model04e09f4aada3406dbc08715865880f4f200_response_data_inner import Model04e09f4aada3406dbc08715865880f4f200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of Model04e09f4aada3406dbc08715865880f4f200ResponseDataInner from a JSON string
model04e09f4aada3406dbc08715865880f4f200_response_data_inner_instance = Model04e09f4aada3406dbc08715865880f4f200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(Model04e09f4aada3406dbc08715865880f4f200ResponseDataInner.to_json())

# convert the object into a dict
model04e09f4aada3406dbc08715865880f4f200_response_data_inner_dict = model04e09f4aada3406dbc08715865880f4f200_response_data_inner_instance.to_dict()
# create an instance of Model04e09f4aada3406dbc08715865880f4f200ResponseDataInner from a dict
model04e09f4aada3406dbc08715865880f4f200_response_data_inner_from_dict = Model04e09f4aada3406dbc08715865880f4f200ResponseDataInner.from_dict(model04e09f4aada3406dbc08715865880f4f200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


