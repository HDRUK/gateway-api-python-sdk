# Register200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**access_token** | **str** |  | [optional] 
**token_type** | **str** |  | [optional] 
**user** | [**Register200ResponseUser**](Register200ResponseUser.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.register200_response import Register200Response

# TODO update the JSON string below
json = "{}"
# create an instance of Register200Response from a JSON string
register200_response_instance = Register200Response.from_json(json)
# print the JSON string representation of the object
print(Register200Response.to_json())

# convert the object into a dict
register200_response_dict = register200_response_instance.to_dict()
# create an instance of Register200Response from a dict
register200_response_from_dict = Register200Response.from_dict(register200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


