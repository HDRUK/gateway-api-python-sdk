# SearchSimilarDatasetsV2200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[SearchSimilarDatasetsV2200ResponseDataInner]**](SearchSimilarDatasetsV2200ResponseDataInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_similar_datasets_v2200_response import SearchSimilarDatasetsV2200Response

# TODO update the JSON string below
json = "{}"
# create an instance of SearchSimilarDatasetsV2200Response from a JSON string
search_similar_datasets_v2200_response_instance = SearchSimilarDatasetsV2200Response.from_json(json)
# print the JSON string representation of the object
print(SearchSimilarDatasetsV2200Response.to_json())

# convert the object into a dict
search_similar_datasets_v2200_response_dict = search_similar_datasets_v2200_response_instance.to_dict()
# create an instance of SearchSimilarDatasetsV2200Response from a dict
search_similar_datasets_v2200_response_from_dict = SearchSimilarDatasetsV2200Response.from_dict(search_similar_datasets_v2200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


