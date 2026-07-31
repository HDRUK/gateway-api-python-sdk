# CreateToolsRequestCollectionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**reason** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_tools_request_collections_inner import CreateToolsRequestCollectionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateToolsRequestCollectionsInner from a JSON string
create_tools_request_collections_inner_instance = CreateToolsRequestCollectionsInner.from_json(json)
# print the JSON string representation of the object
print(CreateToolsRequestCollectionsInner.to_json())

# convert the object into a dict
create_tools_request_collections_inner_dict = create_tools_request_collections_inner_instance.to_dict()
# create an instance of CreateToolsRequestCollectionsInner from a dict
create_tools_request_collections_inner_from_dict = CreateToolsRequestCollectionsInner.from_dict(create_tools_request_collections_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


