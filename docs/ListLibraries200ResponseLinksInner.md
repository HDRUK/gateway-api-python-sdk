# ListLibraries200ResponseLinksInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** |  | [optional] 
**label** | **str** |  | [optional] 
**active** | **bool** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.list_libraries200_response_links_inner import ListLibraries200ResponseLinksInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListLibraries200ResponseLinksInner from a JSON string
list_libraries200_response_links_inner_instance = ListLibraries200ResponseLinksInner.from_json(json)
# print the JSON string representation of the object
print(ListLibraries200ResponseLinksInner.to_json())

# convert the object into a dict
list_libraries200_response_links_inner_dict = list_libraries200_response_links_inner_instance.to_dict()
# create an instance of ListLibraries200ResponseLinksInner from a dict
list_libraries200_response_links_inner_from_dict = ListLibraries200ResponseLinksInner.from_dict(list_libraries200_response_links_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


