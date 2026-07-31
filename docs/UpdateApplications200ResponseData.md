# UpdateApplications200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**app_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**public** | **bool** |  | [optional] 
**counter** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_applications200_response_data import UpdateApplications200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateApplications200ResponseData from a JSON string
update_applications200_response_data_instance = UpdateApplications200ResponseData.from_json(json)
# print the JSON string representation of the object
print(UpdateApplications200ResponseData.to_json())

# convert the object into a dict
update_applications200_response_data_dict = update_applications200_response_data_instance.to_dict()
# create an instance of UpdateApplications200ResponseData from a dict
update_applications200_response_data_from_dict = UpdateApplications200ResponseData.from_dict(update_applications200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


