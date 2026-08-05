# EditUsers200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**User**](User.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_users200_response import EditUsers200Response

# TODO update the JSON string below
json = "{}"
# create an instance of EditUsers200Response from a JSON string
edit_users200_response_instance = EditUsers200Response.from_json(json)
# print the JSON string representation of the object
print(EditUsers200Response.to_json())

# convert the object into a dict
edit_users200_response_dict = edit_users200_response_instance.to_dict()
# create an instance of EditUsers200Response from a dict
edit_users200_response_from_dict = EditUsers200Response.from_dict(edit_users200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


