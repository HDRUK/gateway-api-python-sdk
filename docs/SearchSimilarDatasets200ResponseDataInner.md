# SearchSimilarDatasets200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[SearchDatasets200ResponseDataInnerSourceInner]**](SearchDatasets200ResponseDataInnerSourceInner.md) |  | [optional] 
**metadata** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_similar_datasets200_response_data_inner import SearchSimilarDatasets200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchSimilarDatasets200ResponseDataInner from a JSON string
search_similar_datasets200_response_data_inner_instance = SearchSimilarDatasets200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(SearchSimilarDatasets200ResponseDataInner.to_json())

# convert the object into a dict
search_similar_datasets200_response_data_inner_dict = search_similar_datasets200_response_data_inner_instance.to_dict()
# create an instance of SearchSimilarDatasets200ResponseDataInner from a dict
search_similar_datasets200_response_data_inner_from_dict = SearchSimilarDatasets200ResponseDataInner.from_dict(search_similar_datasets200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


