# UpdateUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_users_request import UpdateUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateUsersRequest from a JSON string
update_users_request_instance = UpdateUsersRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateUsersRequest.to_json())

# convert the object into a dict
update_users_request_dict = update_users_request_instance.to_dict()
# create an instance of UpdateUsersRequest from a dict
update_users_request_from_dict = UpdateUsersRequest.from_dict(update_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


