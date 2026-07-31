# UpdateSavedSearchesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**search_endpoint** | **str** |  | [optional] 
**filters** | [**List[CreateSavedSearchesRequestFiltersInner]**](CreateSavedSearchesRequestFiltersInner.md) |  | [optional] 
**enabled** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.update_saved_searches_request import UpdateSavedSearchesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSavedSearchesRequest from a JSON string
update_saved_searches_request_instance = UpdateSavedSearchesRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateSavedSearchesRequest.to_json())

# convert the object into a dict
update_saved_searches_request_dict = update_saved_searches_request_instance.to_dict()
# create an instance of UpdateSavedSearchesRequest from a dict
update_saved_searches_request_from_dict = UpdateSavedSearchesRequest.from_dict(update_saved_searches_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


