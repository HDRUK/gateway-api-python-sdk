# UpdateApplicationsRequest


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
from gateway_api_sdk.models.update_applications_request import UpdateApplicationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateApplicationsRequest from a JSON string
update_applications_request_instance = UpdateApplicationsRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateApplicationsRequest.to_json())

# convert the object into a dict
update_applications_request_dict = update_applications_request_instance.to_dict()
# create an instance of UpdateApplicationsRequest from a dict
update_applications_request_from_dict = UpdateApplicationsRequest.from_dict(update_applications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


