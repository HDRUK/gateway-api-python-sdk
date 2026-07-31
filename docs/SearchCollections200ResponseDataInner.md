# SearchCollections200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[SearchCollections200ResponseDataInnerSourceInner]**](SearchCollections200ResponseDataInnerSourceInner.md) |  | [optional] 
**highlight** | [**List[SearchTools200ResponseDataInnerHighlightInner]**](SearchTools200ResponseDataInnerHighlightInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_collections200_response_data_inner import SearchCollections200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchCollections200ResponseDataInner from a JSON string
search_collections200_response_data_inner_instance = SearchCollections200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(SearchCollections200ResponseDataInner.to_json())

# convert the object into a dict
search_collections200_response_data_inner_dict = search_collections200_response_data_inner_instance.to_dict()
# create an instance of SearchCollections200ResponseDataInner from a dict
search_collections200_response_data_inner_from_dict = SearchCollections200ResponseDataInner.from_dict(search_collections200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


