# EditDataProviderCollRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**summary** | **str** |  | [optional] 
**enabled** | **str** |  | [optional] 
**service** | **str** |  | [optional] 
**team_ids** | **List[int]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_data_provider_coll_request import EditDataProviderCollRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditDataProviderCollRequest from a JSON string
edit_data_provider_coll_request_instance = EditDataProviderCollRequest.from_json(json)
# print the JSON string representation of the object
print(EditDataProviderCollRequest.to_json())

# convert the object into a dict
edit_data_provider_coll_request_dict = edit_data_provider_coll_request_instance.to_dict()
# create an instance of EditDataProviderCollRequest from a dict
edit_data_provider_coll_request_from_dict = EditDataProviderCollRequest.from_dict(edit_data_provider_coll_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


