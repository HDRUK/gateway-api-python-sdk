# UpdateDurIntegrations200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**UpdateDurIntegrations200ResponseData**](UpdateDurIntegrations200ResponseData.md) |  | [optional] 

## Example

```python
from gateway_api_sdk.models.update_dur_integrations200_response import UpdateDurIntegrations200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateDurIntegrations200Response from a JSON string
update_dur_integrations200_response_instance = UpdateDurIntegrations200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateDurIntegrations200Response.to_json())

# convert the object into a dict
update_dur_integrations200_response_dict = update_dur_integrations200_response_instance.to_dict()
# create an instance of UpdateDurIntegrations200Response from a dict
update_dur_integrations200_response_from_dict = UpdateDurIntegrations200Response.from_dict(update_dur_integrations200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


