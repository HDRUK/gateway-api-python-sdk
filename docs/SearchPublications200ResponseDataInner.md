# SearchPublications200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[SearchPublications200ResponseDataInnerSourceInner]**](SearchPublications200ResponseDataInnerSourceInner.md) |  | [optional] 
**highlight** | [**List[SearchPublications200ResponseDataInnerHighlightInner]**](SearchPublications200ResponseDataInnerHighlightInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_publications200_response_data_inner import SearchPublications200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchPublications200ResponseDataInner from a JSON string
search_publications200_response_data_inner_instance = SearchPublications200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(SearchPublications200ResponseDataInner.to_json())

# convert the object into a dict
search_publications200_response_data_inner_dict = search_publications200_response_data_inner_instance.to_dict()
# create an instance of SearchPublications200ResponseDataInner from a dict
search_publications200_response_data_inner_from_dict = SearchPublications200ResponseDataInner.from_dict(search_publications200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


