# ListLibraries200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[ListLibraries200ResponseDataInner]**](ListLibraries200ResponseDataInner.md) |  | [optional] 
**first_page_url** | **str** |  | [optional] 
**var_from** | **int** |  | [optional] 
**last_page** | **int** |  | [optional] 
**last_page_url** | **str** |  | [optional] 
**links** | [**List[ListLibraries200ResponseLinksInner]**](ListLibraries200ResponseLinksInner.md) |  | [optional] 
**next_page_url** | **str** |  | [optional] 
**path** | **str** |  | [optional] 
**per_page** | **int** |  | [optional] 
**prev_page_url** | **str** |  | [optional] 
**to** | **int** |  | [optional] 
**total** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.list_libraries200_response import ListLibraries200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListLibraries200Response from a JSON string
list_libraries200_response_instance = ListLibraries200Response.from_json(json)
# print the JSON string representation of the object
print(ListLibraries200Response.to_json())

# convert the object into a dict
list_libraries200_response_dict = list_libraries200_response_instance.to_dict()
# create an instance of ListLibraries200Response from a dict
list_libraries200_response_from_dict = ListLibraries200Response.from_dict(list_libraries200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


