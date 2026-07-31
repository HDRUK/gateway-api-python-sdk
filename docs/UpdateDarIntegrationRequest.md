# UpdateDarIntegrationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **int** |  | 
**notification_email** | **str** |  | 
**outbound_auth_type** | **str** |  | 
**outbound_auth_key** | **str** |  | 
**outbound_endpoints_base_url** | **str** |  | 
**outbound_endpoints_enquiry** | **str** |  | 
**outbound_endpoints_5safes** | **str** |  | 
**outbound_endpoints_5safes_files** | **str** |  | 
**inbound_service_account_id** | **str** |  | 

## Example

```python
from gateway_api_sdk.models.update_dar_integration_request import UpdateDarIntegrationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDarIntegrationRequest from a JSON string
update_dar_integration_request_instance = UpdateDarIntegrationRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateDarIntegrationRequest.to_json())

# convert the object into a dict
update_dar_integration_request_dict = update_dar_integration_request_instance.to_dict()
# create an instance of UpdateDarIntegrationRequest from a dict
update_dar_integration_request_from_dict = UpdateDarIntegrationRequest.from_dict(update_dar_integration_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


