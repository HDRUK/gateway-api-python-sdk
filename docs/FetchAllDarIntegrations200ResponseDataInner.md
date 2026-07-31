# FetchAllDarIntegrations200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**notification_email** | **str** |  | [optional] 
**outbound_auth_type** | **str** |  | [optional] 
**outbound_auth_key** | **str** |  | [optional] 
**outbound_endpoints_base_url** | **str** |  | [optional] 
**outbound_endpoints_enquiry** | **str** |  | [optional] 
**outbound_endpoints_5safes** | **str** |  | [optional] 
**outbound_endpoints_5safes_files** | **str** |  | [optional] 
**inbound_service_account_id** | **str** |  | [optional] 

## Example

```python
from gateway_api_sdk.models.fetch_all_dar_integrations200_response_data_inner import FetchAllDarIntegrations200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of FetchAllDarIntegrations200ResponseDataInner from a JSON string
fetch_all_dar_integrations200_response_data_inner_instance = FetchAllDarIntegrations200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(FetchAllDarIntegrations200ResponseDataInner.to_json())

# convert the object into a dict
fetch_all_dar_integrations200_response_data_inner_dict = fetch_all_dar_integrations200_response_data_inner_instance.to_dict()
# create an instance of FetchAllDarIntegrations200ResponseDataInner from a dict
fetch_all_dar_integrations200_response_data_inner_from_dict = FetchAllDarIntegrations200ResponseDataInner.from_dict(fetch_all_dar_integrations200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


