# SearchToolsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_tools_request import SearchToolsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchToolsRequest from a JSON string
search_tools_request_instance = SearchToolsRequest.from_json(json)
# print the JSON string representation of the object
print(SearchToolsRequest.to_json())

# convert the object into a dict
search_tools_request_dict = search_tools_request_instance.to_dict()
# create an instance of SearchToolsRequest from a dict
search_tools_request_from_dict = SearchToolsRequest.from_dict(search_tools_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


