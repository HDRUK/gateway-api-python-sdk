# SearchCollections200ResponseDataInnerSourceInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**keywords** | **str** |  | [optional] 
**related_objects_keywords** | **str** |  | [optional] 
**related_objects_title** | **str** |  | [optional] 
**related_objects_name** | **str** |  | [optional] 
**related_objects_description** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_collections200_response_data_inner_source_inner import SearchCollections200ResponseDataInnerSourceInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchCollections200ResponseDataInnerSourceInner from a JSON string
search_collections200_response_data_inner_source_inner_instance = SearchCollections200ResponseDataInnerSourceInner.from_json(json)
# print the JSON string representation of the object
print(SearchCollections200ResponseDataInnerSourceInner.to_json())

# convert the object into a dict
search_collections200_response_data_inner_source_inner_dict = search_collections200_response_data_inner_source_inner_instance.to_dict()
# create an instance of SearchCollections200ResponseDataInnerSourceInner from a dict
search_collections200_response_data_inner_source_inner_from_dict = SearchCollections200ResponseDataInnerSourceInner.from_dict(search_collections200_response_data_inner_source_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


