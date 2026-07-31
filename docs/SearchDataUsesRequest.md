# SearchDataUsesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_data_uses_request import SearchDataUsesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataUsesRequest from a JSON string
search_data_uses_request_instance = SearchDataUsesRequest.from_json(json)
# print the JSON string representation of the object
print(SearchDataUsesRequest.to_json())

# convert the object into a dict
search_data_uses_request_dict = search_data_uses_request_instance.to_dict()
# create an instance of SearchDataUsesRequest from a dict
search_data_uses_request_from_dict = SearchDataUsesRequest.from_dict(search_data_uses_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


