# AliasControllerIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[Alias]**](Alias.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.alias_controller_index200_response import AliasControllerIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of AliasControllerIndex200Response from a JSON string
alias_controller_index200_response_instance = AliasControllerIndex200Response.from_json(json)
# print the JSON string representation of the object
print(AliasControllerIndex200Response.to_json())

# convert the object into a dict
alias_controller_index200_response_dict = alias_controller_index200_response_instance.to_dict()
# create an instance of AliasControllerIndex200Response from a dict
alias_controller_index200_response_from_dict = AliasControllerIndex200Response.from_dict(alias_controller_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


