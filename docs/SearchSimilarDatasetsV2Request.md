# SearchSimilarDatasetsV2Request


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Dataset id | 

## Example

```python
from gateway_api_sdk.models.search_similar_datasets_v2_request import SearchSimilarDatasetsV2Request

# TODO update the JSON string below
json = "{}"
# create an instance of SearchSimilarDatasetsV2Request from a JSON string
search_similar_datasets_v2_request_instance = SearchSimilarDatasetsV2Request.from_json(json)
# print the JSON string representation of the object
print(SearchSimilarDatasetsV2Request.to_json())

# convert the object into a dict
search_similar_datasets_v2_request_dict = search_similar_datasets_v2_request_instance.to_dict()
# create an instance of SearchSimilarDatasetsV2Request from a dict
search_similar_datasets_v2_request_from_dict = SearchSimilarDatasetsV2Request.from_dict(search_similar_datasets_v2_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


