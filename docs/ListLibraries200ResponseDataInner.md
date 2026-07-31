# ListLibraries200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**user_id** | **int** |  | [optional] 
**dataset_id** | **str** |  | [optional] 
**dataset_status** | **str** |  | [optional] 
**data_provider_id** | **str** |  | [optional] 
**data_provider_dar_status** | **bool** |  | [optional] 
**data_provider_name** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.list_libraries200_response_data_inner import ListLibraries200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListLibraries200ResponseDataInner from a JSON string
list_libraries200_response_data_inner_instance = ListLibraries200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListLibraries200ResponseDataInner.to_json())

# convert the object into a dict
list_libraries200_response_data_inner_dict = list_libraries200_response_data_inner_instance.to_dict()
# create an instance of ListLibraries200ResponseDataInner from a dict
list_libraries200_response_data_inner_from_dict = ListLibraries200ResponseDataInner.from_dict(list_libraries200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


