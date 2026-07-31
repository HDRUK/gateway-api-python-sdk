# EditApplicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**app_id** | **str** |  | [optional] 
**client_id** | **str** |  | [optional] 
**image_link** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**team_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**permissions** | **List[object]** |  | [optional] 
**notifications** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_applications_request import EditApplicationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditApplicationsRequest from a JSON string
edit_applications_request_instance = EditApplicationsRequest.from_json(json)
# print the JSON string representation of the object
print(EditApplicationsRequest.to_json())

# convert the object into a dict
edit_applications_request_dict = edit_applications_request_instance.to_dict()
# create an instance of EditApplicationsRequest from a dict
edit_applications_request_from_dict = EditApplicationsRequest.from_dict(edit_applications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


