# CreateSavedSearchesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**search_endpoint** | **str** |  | [optional] 
**filters** | [**List[CreateSavedSearchesRequestFiltersInner]**](CreateSavedSearchesRequestFiltersInner.md) |  | [optional] 
**enabled** | **bool** |  | 

## Example

```python
from gateway_api_sdk.models.create_saved_searches_request import CreateSavedSearchesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSavedSearchesRequest from a JSON string
create_saved_searches_request_instance = CreateSavedSearchesRequest.from_json(json)
# print the JSON string representation of the object
print(CreateSavedSearchesRequest.to_json())

# convert the object into a dict
create_saved_searches_request_dict = create_saved_searches_request_instance.to_dict()
# create an instance of CreateSavedSearchesRequest from a dict
create_saved_searches_request_from_dict = CreateSavedSearchesRequest.from_dict(create_saved_searches_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


