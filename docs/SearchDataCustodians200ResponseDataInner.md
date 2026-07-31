# SearchDataCustodians200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[SearchDataCustodians200ResponseDataInnerSourceInner]**](SearchDataCustodians200ResponseDataInnerSourceInner.md) |  | [optional] 
**highlight** | [**List[SearchDataUses200ResponseDataInnerHighlightInner]**](SearchDataUses200ResponseDataInnerHighlightInner.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_data_custodians200_response_data_inner import SearchDataCustodians200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataCustodians200ResponseDataInner from a JSON string
search_data_custodians200_response_data_inner_instance = SearchDataCustodians200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(SearchDataCustodians200ResponseDataInner.to_json())

# convert the object into a dict
search_data_custodians200_response_data_inner_dict = search_data_custodians200_response_data_inner_instance.to_dict()
# create an instance of SearchDataCustodians200ResponseDataInner from a dict
search_data_custodians200_response_data_inner_from_dict = SearchDataCustodians200ResponseDataInner.from_dict(search_data_custodians200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


