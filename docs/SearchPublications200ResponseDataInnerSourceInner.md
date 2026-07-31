# SearchPublications200ResponseDataInnerSourceInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**abstract** | **str** |  | [optional] 
**authors** | **str** |  | [optional] 
**dataset_titles** | **str** |  | [optional] 
**journal_name** | **str** |  | [optional] 
**publication_date** | **str** |  | [optional] 
**publication_type** | **List[object]** |  | [optional] 
**title** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_publications200_response_data_inner_source_inner import SearchPublications200ResponseDataInnerSourceInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchPublications200ResponseDataInnerSourceInner from a JSON string
search_publications200_response_data_inner_source_inner_instance = SearchPublications200ResponseDataInnerSourceInner.from_json(json)
# print the JSON string representation of the object
print(SearchPublications200ResponseDataInnerSourceInner.to_json())

# convert the object into a dict
search_publications200_response_data_inner_source_inner_dict = search_publications200_response_data_inner_source_inner_instance.to_dict()
# create an instance of SearchPublications200ResponseDataInnerSourceInner from a dict
search_publications200_response_data_inner_source_inner_from_dict = SearchPublications200ResponseDataInnerSourceInner.from_dict(search_publications200_response_data_inner_source_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


