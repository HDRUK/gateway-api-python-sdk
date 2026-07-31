# CreateSavedSearchesRequestFiltersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**terms** | **List[object]** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.create_saved_searches_request_filters_inner import CreateSavedSearchesRequestFiltersInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSavedSearchesRequestFiltersInner from a JSON string
create_saved_searches_request_filters_inner_instance = CreateSavedSearchesRequestFiltersInner.from_json(json)
# print the JSON string representation of the object
print(CreateSavedSearchesRequestFiltersInner.to_json())

# convert the object into a dict
create_saved_searches_request_filters_inner_dict = create_saved_searches_request_filters_inner_instance.to_dict()
# create an instance of CreateSavedSearchesRequestFiltersInner from a dict
create_saved_searches_request_filters_inner_from_dict = CreateSavedSearchesRequestFiltersInner.from_dict(create_saved_searches_request_filters_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


