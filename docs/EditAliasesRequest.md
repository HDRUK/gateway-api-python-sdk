# EditAliasesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_aliases_request import EditAliasesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditAliasesRequest from a JSON string
edit_aliases_request_instance = EditAliasesRequest.from_json(json)
# print the JSON string representation of the object
print(EditAliasesRequest.to_json())

# convert the object into a dict
edit_aliases_request_dict = edit_aliases_request_instance.to_dict()
# create an instance of EditAliasesRequest from a dict
edit_aliases_request_from_dict = EditAliasesRequest.from_dict(edit_aliases_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


