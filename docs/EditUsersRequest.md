# EditUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_users_request import EditUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditUsersRequest from a JSON string
edit_users_request_instance = EditUsersRequest.from_json(json)
# print the JSON string representation of the object
print(EditUsersRequest.to_json())

# convert the object into a dict
edit_users_request_dict = edit_users_request_instance.to_dict()
# create an instance of EditUsersRequest from a dict
edit_users_request_from_dict = EditUsersRequest.from_dict(edit_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


