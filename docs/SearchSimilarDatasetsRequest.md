# SearchSimilarDatasetsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_similar_datasets_request import SearchSimilarDatasetsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchSimilarDatasetsRequest from a JSON string
search_similar_datasets_request_instance = SearchSimilarDatasetsRequest.from_json(json)
# print the JSON string representation of the object
print(SearchSimilarDatasetsRequest.to_json())

# convert the object into a dict
search_similar_datasets_request_dict = search_similar_datasets_request_instance.to_dict()
# create an instance of SearchSimilarDatasetsRequest from a dict
search_similar_datasets_request_from_dict = SearchSimilarDatasetsRequest.from_dict(search_similar_datasets_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


