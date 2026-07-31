# UpdateLibraries200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**user_id** | **int** |  | [optional] 
**dataset** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_libraries200_response_data import UpdateLibraries200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateLibraries200ResponseData from a JSON string
update_libraries200_response_data_instance = UpdateLibraries200ResponseData.from_json(json)
# print the JSON string representation of the object
print(UpdateLibraries200ResponseData.to_json())

# convert the object into a dict
update_libraries200_response_data_dict = update_libraries200_response_data_instance.to_dict()
# create an instance of UpdateLibraries200ResponseData from a dict
update_libraries200_response_data_from_dict = UpdateLibraries200ResponseData.from_dict(update_libraries200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


