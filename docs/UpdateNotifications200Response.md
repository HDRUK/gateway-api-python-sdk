# UpdateNotifications200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Notification**](Notification.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_notifications200_response import UpdateNotifications200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateNotifications200Response from a JSON string
update_notifications200_response_instance = UpdateNotifications200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateNotifications200Response.to_json())

# convert the object into a dict
update_notifications200_response_dict = update_notifications200_response_instance.to_dict()
# create an instance of UpdateNotifications200Response from a dict
update_notifications200_response_from_dict = UpdateNotifications200Response.from_dict(update_notifications200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


