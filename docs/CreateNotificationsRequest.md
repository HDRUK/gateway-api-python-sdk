# CreateNotificationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**notification_type** | **str** |  | 
**message** | **str** |  | 
**opt_in** | **bool** |  | 
**enabled** | **bool** |  | 
**email** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_notifications_request import CreateNotificationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateNotificationsRequest from a JSON string
create_notifications_request_instance = CreateNotificationsRequest.from_json(json)
# print the JSON string representation of the object
print(CreateNotificationsRequest.to_json())

# convert the object into a dict
create_notifications_request_dict = create_notifications_request_instance.to_dict()
# create an instance of CreateNotificationsRequest from a dict
create_notifications_request_from_dict = CreateNotificationsRequest.from_dict(create_notifications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


