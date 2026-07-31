# CreateUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_users_request import CreateUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateUsersRequest from a JSON string
create_users_request_instance = CreateUsersRequest.from_json(json)
# print the JSON string representation of the object
print(CreateUsersRequest.to_json())

# convert the object into a dict
create_users_request_dict = create_users_request_instance.to_dict()
# create an instance of CreateUsersRequest from a dict
create_users_request_from_dict = CreateUsersRequest.from_dict(create_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


