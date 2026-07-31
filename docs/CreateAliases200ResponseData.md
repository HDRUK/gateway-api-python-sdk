# CreateAliases200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**alias** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_aliases200_response_data import CreateAliases200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAliases200ResponseData from a JSON string
create_aliases200_response_data_instance = CreateAliases200ResponseData.from_json(json)
# print the JSON string representation of the object
print(CreateAliases200ResponseData.to_json())

# convert the object into a dict
create_aliases200_response_data_dict = create_aliases200_response_data_instance.to_dict()
# create an instance of CreateAliases200ResponseData from a dict
create_aliases200_response_data_from_dict = CreateAliases200ResponseData.from_dict(create_aliases200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


