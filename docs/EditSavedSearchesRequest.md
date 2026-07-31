# EditSavedSearchesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**filters** | [**List[CreateSavedSearchesRequestFiltersInner]**](CreateSavedSearchesRequestFiltersInner.md) |  | [optional] 
**enabled** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.edit_saved_searches_request import EditSavedSearchesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditSavedSearchesRequest from a JSON string
edit_saved_searches_request_instance = EditSavedSearchesRequest.from_json(json)
# print the JSON string representation of the object
print(EditSavedSearchesRequest.to_json())

# convert the object into a dict
edit_saved_searches_request_dict = edit_saved_searches_request_instance.to_dict()
# create an instance of EditSavedSearchesRequest from a dict
edit_saved_searches_request_from_dict = EditSavedSearchesRequest.from_dict(edit_saved_searches_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


