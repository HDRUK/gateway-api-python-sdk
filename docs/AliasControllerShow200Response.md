# AliasControllerShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Alias**](Alias.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.alias_controller_show200_response import AliasControllerShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of AliasControllerShow200Response from a JSON string
alias_controller_show200_response_instance = AliasControllerShow200Response.from_json(json)
# print the JSON string representation of the object
print(AliasControllerShow200Response.to_json())

# convert the object into a dict
alias_controller_show200_response_dict = alias_controller_show200_response_instance.to_dict()
# create an instance of AliasControllerShow200Response from a dict
alias_controller_show200_response_from_dict = AliasControllerShow200Response.from_dict(alias_controller_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


