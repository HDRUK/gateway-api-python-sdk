# SearchDatasetsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 
**sort** | **str** |  | [optional] 
**direction** | **str** |  | [optional] 
**filters** | **str** |  | [optional] 
**per_page** | **int** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_datasets_request import SearchDatasetsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDatasetsRequest from a JSON string
search_datasets_request_instance = SearchDatasetsRequest.from_json(json)
# print the JSON string representation of the object
print(SearchDatasetsRequest.to_json())

# convert the object into a dict
search_datasets_request_dict = search_datasets_request_instance.to_dict()
# create an instance of SearchDatasetsRequest from a dict
search_datasets_request_from_dict = SearchDatasetsRequest.from_dict(search_datasets_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


