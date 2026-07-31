# SearchPublicationsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_publications_request import SearchPublicationsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchPublicationsRequest from a JSON string
search_publications_request_instance = SearchPublicationsRequest.from_json(json)
# print the JSON string representation of the object
print(SearchPublicationsRequest.to_json())

# convert the object into a dict
search_publications_request_dict = search_publications_request_instance.to_dict()
# create an instance of SearchPublicationsRequest from a dict
search_publications_request_from_dict = SearchPublicationsRequest.from_dict(search_publications_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


