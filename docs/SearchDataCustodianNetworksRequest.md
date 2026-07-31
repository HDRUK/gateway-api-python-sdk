# SearchDataCustodianNetworksRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**query** | **str** |  | [optional] 
**filters** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.search_data_custodian_networks_request import SearchDataCustodianNetworksRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataCustodianNetworksRequest from a JSON string
search_data_custodian_networks_request_instance = SearchDataCustodianNetworksRequest.from_json(json)
# print the JSON string representation of the object
print(SearchDataCustodianNetworksRequest.to_json())

# convert the object into a dict
search_data_custodian_networks_request_dict = search_data_custodian_networks_request_instance.to_dict()
# create an instance of SearchDataCustodianNetworksRequest from a dict
search_data_custodian_networks_request_from_dict = SearchDataCustodianNetworksRequest.from_dict(search_data_custodian_networks_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


