# UpdateDataCustodianNetwork200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**DataCustodianNetwork**](DataCustodianNetwork.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_data_custodian_network200_response import UpdateDataCustodianNetwork200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDataCustodianNetwork200Response from a JSON string
update_data_custodian_network200_response_instance = UpdateDataCustodianNetwork200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateDataCustodianNetwork200Response.to_json())

# convert the object into a dict
update_data_custodian_network200_response_dict = update_data_custodian_network200_response_instance.to_dict()
# create an instance of UpdateDataCustodianNetwork200Response from a dict
update_data_custodian_network200_response_from_dict = UpdateDataCustodianNetwork200Response.from_dict(update_data_custodian_network200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


