# SearchCollectionsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_collections_request import SearchCollectionsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchCollectionsRequest from a JSON string
search_collections_request_instance = SearchCollectionsRequest.from_json(json)
# print the JSON string representation of the object
print(SearchCollectionsRequest.to_json())

# convert the object into a dict
search_collections_request_dict = search_collections_request_instance.to_dict()
# create an instance of SearchCollectionsRequest from a dict
search_collections_request_from_dict = SearchCollectionsRequest.from_dict(search_collections_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


