# SearchDataCustodianNetworks200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_page** | **int** |  | [optional] 
**data** | [**List[SearchDataCustodianNetworks200ResponseDataInner]**](SearchDataCustodianNetworks200ResponseDataInner.md) |  | [optional] 
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
from gateway_api_sdk.models.search_data_custodian_networks200_response import SearchDataCustodianNetworks200Response

# TODO update the JSON string below
json = "{}"
# create an instance of SearchDataCustodianNetworks200Response from a JSON string
search_data_custodian_networks200_response_instance = SearchDataCustodianNetworks200Response.from_json(json)
# print the JSON string representation of the object
print(SearchDataCustodianNetworks200Response.to_json())

# convert the object into a dict
search_data_custodian_networks200_response_dict = search_data_custodian_networks200_response_instance.to_dict()
# create an instance of SearchDataCustodianNetworks200Response from a dict
search_data_custodian_networks200_response_from_dict = SearchDataCustodianNetworks200Response.from_dict(search_data_custodian_networks200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


