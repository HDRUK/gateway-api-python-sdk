# SearchDatasets200ResponseDataInnerSourceInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**abstract** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**keywords** | **str** |  | [optional] 
**named_entities** | **List[object]** |  | [optional] 
**publisher_name** | **str** |  | [optional] 
**short_title** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**created_at** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_datasets200_response_data_inner_source_inner import SearchDatasets200ResponseDataInnerSourceInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDatasets200ResponseDataInnerSourceInner from a JSON string
search_datasets200_response_data_inner_source_inner_instance = SearchDatasets200ResponseDataInnerSourceInner.from_json(json)
# print the JSON string representation of the object
print(SearchDatasets200ResponseDataInnerSourceInner.to_json())

# convert the object into a dict
search_datasets200_response_data_inner_source_inner_dict = search_datasets200_response_data_inner_source_inner_instance.to_dict()
# create an instance of SearchDatasets200ResponseDataInnerSourceInner from a dict
search_datasets200_response_data_inner_source_inner_from_dict = SearchDatasets200ResponseDataInnerSourceInner.from_dict(search_datasets200_response_data_inner_source_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


