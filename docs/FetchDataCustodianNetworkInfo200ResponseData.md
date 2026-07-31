# FetchDataCustodianNetworkInfo200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**img_url** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**summary** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**service** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_data_custodian_network_info200_response_data import FetchDataCustodianNetworkInfo200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of FetchDataCustodianNetworkInfo200ResponseData from a JSON string
fetch_data_custodian_network_info200_response_data_instance = FetchDataCustodianNetworkInfo200ResponseData.from_json(json)
# print the JSON string representation of the object
print(FetchDataCustodianNetworkInfo200ResponseData.to_json())

# convert the object into a dict
fetch_data_custodian_network_info200_response_data_dict = fetch_data_custodian_network_info200_response_data_instance.to_dict()
# create an instance of FetchDataCustodianNetworkInfo200ResponseData from a dict
fetch_data_custodian_network_info200_response_data_from_dict = FetchDataCustodianNetworkInfo200ResponseData.from_dict(fetch_data_custodian_network_info200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


