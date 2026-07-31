# CreateDataProviderCollRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**summary** | **str** |  | 
**enabled** | **bool** |  | 
**service** | **str** |  | [optional] 
**team_ids** | **List[int]** |  | 

## Example

```python
from gateway_api_sdk.models.create_data_provider_coll_request import CreateDataProviderCollRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateDataProviderCollRequest from a JSON string
create_data_provider_coll_request_instance = CreateDataProviderCollRequest.from_json(json)
# print the JSON string representation of the object
print(CreateDataProviderCollRequest.to_json())

# convert the object into a dict
create_data_provider_coll_request_dict = create_data_provider_coll_request_instance.to_dict()
# create an instance of CreateDataProviderCollRequest from a dict
create_data_provider_coll_request_from_dict = CreateDataProviderCollRequest.from_dict(create_data_provider_coll_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


