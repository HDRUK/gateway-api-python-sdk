# SearchTools200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**source** | [**List[SearchTools200ResponseDataInnerSourceInner]**](SearchTools200ResponseDataInnerSourceInner.md) |  | [optional] 
**highlight** | [**List[SearchTools200ResponseDataInnerHighlightInner]**](SearchTools200ResponseDataInnerHighlightInner.md) |  | [optional] 
**uploader** | **str** |  | [optional] 
**team_name** | **str** |  | [optional] 
**type_category** | **List[object]** |  | [optional] 
**license** | **str** |  | [optional] 
**programming_language** | **List[object]** |  | [optional] 
**programming_package** | **List[object]** |  | [optional] 
**datasets** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_tools200_response_data_inner import SearchTools200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of SearchTools200ResponseDataInner from a JSON string
search_tools200_response_data_inner_instance = SearchTools200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(SearchTools200ResponseDataInner.to_json())

# convert the object into a dict
search_tools200_response_data_inner_dict = search_tools200_response_data_inner_instance.to_dict()
# create an instance of SearchTools200ResponseDataInner from a dict
search_tools200_response_data_inner_from_dict = SearchTools200ResponseDataInner.from_dict(search_tools200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


