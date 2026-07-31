# SearchDataUses200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[SearchDataUses200ResponseDataInnerSourceInner]**](SearchDataUses200ResponseDataInnerSourceInner.md) |  | [optional] 
**highlight** | [**List[SearchDataUses200ResponseDataInnerHighlightInner]**](SearchDataUses200ResponseDataInnerHighlightInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_data_uses200_response_data_inner import SearchDataUses200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataUses200ResponseDataInner from a JSON string
search_data_uses200_response_data_inner_instance = SearchDataUses200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(SearchDataUses200ResponseDataInner.to_json())

# convert the object into a dict
search_data_uses200_response_data_inner_dict = search_data_uses200_response_data_inner_instance.to_dict()
# create an instance of SearchDataUses200ResponseDataInner from a dict
search_data_uses200_response_data_inner_from_dict = SearchDataUses200ResponseDataInner.from_dict(search_data_uses200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


