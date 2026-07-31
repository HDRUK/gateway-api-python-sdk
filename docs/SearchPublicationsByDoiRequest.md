# SearchPublicationsByDoiRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_publications_by_doi_request import SearchPublicationsByDoiRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchPublicationsByDoiRequest from a JSON string
search_publications_by_doi_request_instance = SearchPublicationsByDoiRequest.from_json(json)
# print the JSON string representation of the object
print(SearchPublicationsByDoiRequest.to_json())

# convert the object into a dict
search_publications_by_doi_request_dict = search_publications_by_doi_request_instance.to_dict()
# create an instance of SearchPublicationsByDoiRequest from a dict
search_publications_by_doi_request_from_dict = SearchPublicationsByDoiRequest.from_dict(search_publications_by_doi_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


