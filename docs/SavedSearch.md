# SavedSearch

A user's saved search definition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**search_term** | **str** |  | [optional] 
**search_endpoint** | **str** |  | [optional] 
**sort_order** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**deleted_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.saved_search import SavedSearch

# TODO update the JSON string below
json = "{}"
# create an instance of SavedSearch from a JSON string
saved_search_instance = SavedSearch.from_json(json)
# print the JSON string representation of the object
print(SavedSearch.to_json())

# convert the object into a dict
saved_search_dict = saved_search_instance.to_dict()
# create an instance of SavedSearch from a dict
saved_search_from_dict = SavedSearch.from_dict(saved_search_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


