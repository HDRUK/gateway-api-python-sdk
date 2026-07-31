# Register200ResponseUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**email** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.register200_response_user import Register200ResponseUser

# TODO update the JSON string below
json = "{}"
# create an instance of Register200ResponseUser from a JSON string
register200_response_user_instance = Register200ResponseUser.from_json(json)
# print the JSON string representation of the object
print(Register200ResponseUser.to_json())

# convert the object into a dict
register200_response_user_dict = register200_response_user_instance.to_dict()
# create an instance of Register200ResponseUser from a dict
register200_response_user_from_dict = Register200ResponseUser.from_dict(register200_response_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


