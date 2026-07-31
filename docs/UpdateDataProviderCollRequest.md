# UpdateDataProviderCollRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**summary** | **str** |  | 
**enabled** | **str** |  | 
**service** | **str** |  | [optional] 
**team_ids** | **List[int]** |  | 

## Example

```python
from gateway_api_sdk.models.update_data_provider_coll_request import UpdateDataProviderCollRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDataProviderCollRequest from a JSON string
update_data_provider_coll_request_instance = UpdateDataProviderCollRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateDataProviderCollRequest.to_json())

# convert the object into a dict
update_data_provider_coll_request_dict = update_data_provider_coll_request_instance.to_dict()
# create an instance of UpdateDataProviderCollRequest from a dict
update_data_provider_coll_request_from_dict = UpdateDataProviderCollRequest.from_dict(update_data_provider_coll_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


