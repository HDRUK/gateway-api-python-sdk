# FetchDataCustodianNetworkEntitiesSummary200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**FetchDataCustodianNetworkEntitiesSummary200ResponseData**](FetchDataCustodianNetworkEntitiesSummary200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_data_custodian_network_entities_summary200_response import FetchDataCustodianNetworkEntitiesSummary200Response

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDataCustodianNetworkEntitiesSummary200Response from a JSON string
fetch_data_custodian_network_entities_summary200_response_instance = FetchDataCustodianNetworkEntitiesSummary200Response.from_json(json)
# print the JSON string representation of the object
print(FetchDataCustodianNetworkEntitiesSummary200Response.to_json())

# convert the object into a dict
fetch_data_custodian_network_entities_summary200_response_dict = fetch_data_custodian_network_entities_summary200_response_instance.to_dict()
# create an instance of FetchDataCustodianNetworkEntitiesSummary200Response from a dict
fetch_data_custodian_network_entities_summary200_response_from_dict = FetchDataCustodianNetworkEntitiesSummary200Response.from_dict(fetch_data_custodian_network_entities_summary200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


