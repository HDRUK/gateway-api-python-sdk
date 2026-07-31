# SearchDataCustodiansRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_data_custodians_request import SearchDataCustodiansRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataCustodiansRequest from a JSON string
search_data_custodians_request_instance = SearchDataCustodiansRequest.from_json(json)
# print the JSON string representation of the object
print(SearchDataCustodiansRequest.to_json())

# convert the object into a dict
search_data_custodians_request_dict = search_data_custodians_request_instance.to_dict()
# create an instance of SearchDataCustodiansRequest from a dict
search_data_custodians_request_from_dict = SearchDataCustodiansRequest.from_dict(search_data_custodians_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


