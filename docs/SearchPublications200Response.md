# SearchPublications200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[SearchPublications200ResponseDataInner]**](SearchPublications200ResponseDataInner.md) |  | [optional] 
**first_page_url** | **str** |  | [optional] 
**var_from** | **int** |  | [optional] 
**last_page** | **int** |  | [optional] 
**last_page_url** | **str** |  | [optional] 
**links** | **List[List[object]]** |  | [optional] 
**next_page_url** | **str** |  | [optional] 
**path** | **str** |  | [optional] 
**per_page** | **int** |  | [optional] 
**prev_page_url** | **str** |  | [optional] 
**to** | **int** |  | [optional] 
**total** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_publications200_response import SearchPublications200Response

# TODO update the JSON string below
json = "{}"
# create an instance of SearchPublications200Response from a JSON string
search_publications200_response_instance = SearchPublications200Response.from_json(json)
# print the JSON string representation of the object
print(SearchPublications200Response.to_json())

# convert the object into a dict
search_publications200_response_dict = search_publications200_response_instance.to_dict()
# create an instance of SearchPublications200Response from a dict
search_publications200_response_from_dict = SearchPublications200Response.from_dict(search_publications200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


