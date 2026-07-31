# CreateAliases200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CreateAliases200ResponseData**](CreateAliases200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_aliases200_response import CreateAliases200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAliases200Response from a JSON string
create_aliases200_response_instance = CreateAliases200Response.from_json(json)
# print the JSON string representation of the object
print(CreateAliases200Response.to_json())

# convert the object into a dict
create_aliases200_response_dict = create_aliases200_response_instance.to_dict()
# create an instance of CreateAliases200Response from a dict
create_aliases200_response_from_dict = CreateAliases200Response.from_dict(create_aliases200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


