# CreateAdminSearchReindexRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**entity** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_admin_search_reindex_request import CreateAdminSearchReindexRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAdminSearchReindexRequest from a JSON string
create_admin_search_reindex_request_instance = CreateAdminSearchReindexRequest.from_json(json)
# print the JSON string representation of the object
print(CreateAdminSearchReindexRequest.to_json())

# convert the object into a dict
create_admin_search_reindex_request_dict = create_admin_search_reindex_request_instance.to_dict()
# create an instance of CreateAdminSearchReindexRequest from a dict
create_admin_search_reindex_request_from_dict = CreateAdminSearchReindexRequest.from_dict(create_admin_search_reindex_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


