# DataCustodianNetwork

A data custodian network (data provider collection) record managed by the Gateway

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**name** | **str** |  | [optional] 
**summary** | **str** |  | [optional] 
**img_url** | **str** |  | [optional] 
**url** | **str** |  | [optional] 
**service** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.data_custodian_network import DataCustodianNetwork

# TODO update the JSON string below
json = "{}"
# create an instance of DataCustodianNetwork from a JSON string
data_custodian_network_instance = DataCustodianNetwork.from_json(json)
# print the JSON string representation of the object
print(DataCustodianNetwork.to_json())

# convert the object into a dict
data_custodian_network_dict = data_custodian_network_instance.to_dict()
# create an instance of DataCustodianNetwork from a dict
data_custodian_network_from_dict = DataCustodianNetwork.from_dict(data_custodian_network_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


