# SearchDatasets200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[SearchDatasets200ResponseDataInnerSourceInner]**](SearchDatasets200ResponseDataInnerSourceInner.md) |  | [optional] 
**highlight** | [**List[SearchDatasets200ResponseDataInnerHighlightInner]**](SearchDatasets200ResponseDataInnerHighlightInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_datasets200_response_data_inner import SearchDatasets200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDatasets200ResponseDataInner from a JSON string
search_datasets200_response_data_inner_instance = SearchDatasets200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(SearchDatasets200ResponseDataInner.to_json())

# convert the object into a dict
search_datasets200_response_data_inner_dict = search_datasets200_response_data_inner_instance.to_dict()
# create an instance of SearchDatasets200ResponseDataInner from a dict
search_datasets200_response_data_inner_from_dict = SearchDatasets200ResponseDataInner.from_dict(search_datasets200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


