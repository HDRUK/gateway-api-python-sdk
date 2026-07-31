# CreateUserHasRolesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**roles** | **List[str]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_user_has_roles_request import CreateUserHasRolesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateUserHasRolesRequest from a JSON string
create_user_has_roles_request_instance = CreateUserHasRolesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateUserHasRolesRequest.to_json())

# convert the object into a dict
create_user_has_roles_request_dict = create_user_has_roles_request_instance.to_dict()
# create an instance of CreateUserHasRolesRequest from a dict
create_user_has_roles_request_from_dict = CreateUserHasRolesRequest.from_dict(create_user_has_roles_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


