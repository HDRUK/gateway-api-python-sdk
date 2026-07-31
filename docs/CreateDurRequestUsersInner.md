# CreateDurRequestUsersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**firstname** | **str** |  | [optional] 
**lastname** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_dur_request_users_inner import CreateDurRequestUsersInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDurRequestUsersInner from a JSON string
create_dur_request_users_inner_instance = CreateDurRequestUsersInner.from_json(json)
# print the JSON string representation of the object
print(CreateDurRequestUsersInner.to_json())

# convert the object into a dict
create_dur_request_users_inner_dict = create_dur_request_users_inner_instance.to_dict()
# create an instance of CreateDurRequestUsersInner from a dict
create_dur_request_users_inner_from_dict = CreateDurRequestUsersInner.from_dict(create_dur_request_users_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


