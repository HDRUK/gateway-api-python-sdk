# UpdateUserHasRolesRequestRoles


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**read** | **bool** |  | [optional] 
**create** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_user_has_roles_request_roles import UpdateUserHasRolesRequestRoles

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateUserHasRolesRequestRoles from a JSON string
update_user_has_roles_request_roles_instance = UpdateUserHasRolesRequestRoles.from_json(json)
# print the JSON string representation of the object
print(UpdateUserHasRolesRequestRoles.to_json())

# convert the object into a dict
update_user_has_roles_request_roles_dict = update_user_has_roles_request_roles_instance.to_dict()
# create an instance of UpdateUserHasRolesRequestRoles from a dict
update_user_has_roles_request_roles_from_dict = UpdateUserHasRolesRequestRoles.from_dict(update_user_has_roles_request_roles_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


