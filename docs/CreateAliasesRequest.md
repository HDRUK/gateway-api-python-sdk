# CreateAliasesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.create_aliases_request import CreateAliasesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAliasesRequest from a JSON string
create_aliases_request_instance = CreateAliasesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateAliasesRequest.to_json())

# convert the object into a dict
create_aliases_request_dict = create_aliases_request_instance.to_dict()
# create an instance of CreateAliasesRequest from a dict
create_aliases_request_from_dict = CreateAliasesRequest.from_dict(create_aliases_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


