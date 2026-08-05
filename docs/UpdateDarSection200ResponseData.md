# UpdateDarSection200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**parent_section** | **int** |  | [optional] 
**order** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_dar_section200_response_data import UpdateDarSection200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDarSection200ResponseData from a JSON string
update_dar_section200_response_data_instance = UpdateDarSection200ResponseData.from_json(json)
# print the JSON string representation of the object
print(UpdateDarSection200ResponseData.to_json())

# convert the object into a dict
update_dar_section200_response_data_dict = update_dar_section200_response_data_instance.to_dict()
# create an instance of UpdateDarSection200ResponseData from a dict
update_dar_section200_response_data_from_dict = UpdateDarSection200ResponseData.from_dict(update_dar_section200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


