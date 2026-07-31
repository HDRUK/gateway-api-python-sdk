# EditNotificationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**notification_type** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**opt_in** | **bool** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**email** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_notifications_request import EditNotificationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditNotificationsRequest from a JSON string
edit_notifications_request_instance = EditNotificationsRequest.from_json(json)
# print the JSON string representation of the object
print(EditNotificationsRequest.to_json())

# convert the object into a dict
edit_notifications_request_dict = edit_notifications_request_instance.to_dict()
# create an instance of EditNotificationsRequest from a dict
edit_notifications_request_from_dict = EditNotificationsRequest.from_dict(edit_notifications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


