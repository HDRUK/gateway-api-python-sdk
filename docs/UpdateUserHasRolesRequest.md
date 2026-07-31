# UpdateUserHasRolesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**roles** | [**UpdateUserHasRolesRequestRoles**](UpdateUserHasRolesRequestRoles.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_user_has_roles_request import UpdateUserHasRolesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateUserHasRolesRequest from a JSON string
update_user_has_roles_request_instance = UpdateUserHasRolesRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateUserHasRolesRequest.to_json())

# convert the object into a dict
update_user_has_roles_request_dict = update_user_has_roles_request_instance.to_dict()
# create an instance of UpdateUserHasRolesRequest from a dict
update_user_has_roles_request_from_dict = UpdateUserHasRolesRequest.from_dict(update_user_has_roles_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


